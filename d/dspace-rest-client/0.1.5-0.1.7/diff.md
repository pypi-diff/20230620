# Comparing `tmp/dspace_rest_client-0.1.5-py3-none-any.whl.zip` & `tmp/dspace_rest_client-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 16675 bytes, number of entries: 8
+Zip file size: 17573 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx       16 b- defN 22-Jul-31 01:15 dspace_rest_client/__init__.py
--rw-rw-r--  2.0 unx    37323 b- defN 23-May-02 23:13 dspace_rest_client/client.py
--rw-rw-r--  2.0 unx    16302 b- defN 23-Jun-05 01:41 dspace_rest_client/models.py
--rw-rw-r--  2.0 unx     1475 b- defN 23-Jun-05 23:46 dspace_rest_client-0.1.5.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     4134 b- defN 23-Jun-05 23:46 dspace_rest_client-0.1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-05 23:46 dspace_rest_client-0.1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       19 b- defN 23-Jun-05 23:46 dspace_rest_client-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      702 b- defN 23-Jun-05 23:46 dspace_rest_client-0.1.5.dist-info/RECORD
-8 files, 60063 bytes uncompressed, 15437 bytes compressed:  74.3%
+-rw-rw-r--  2.0 unx    41325 b- defN 23-Jun-20 17:12 dspace_rest_client/client.py
+-rw-rw-r--  2.0 unx    18483 b- defN 23-Jun-20 14:23 dspace_rest_client/models.py
+-rw-rw-r--  2.0 unx     1475 b- defN 23-Jun-20 17:15 dspace_rest_client-0.1.7.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     4134 b- defN 23-Jun-20 17:15 dspace_rest_client-0.1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-20 17:15 dspace_rest_client-0.1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       19 b- defN 23-Jun-20 17:15 dspace_rest_client-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      702 b- defN 23-Jun-20 17:15 dspace_rest_client-0.1.7.dist-info/RECORD
+8 files, 66246 bytes uncompressed, 16335 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: dspace_rest_client/client.py
 Comment: 
 
 Filename: dspace_rest_client/models.py
 Comment: 
 
-Filename: dspace_rest_client-0.1.5.dist-info/LICENSE.txt
+Filename: dspace_rest_client-0.1.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dspace_rest_client-0.1.5.dist-info/METADATA
+Filename: dspace_rest_client-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: dspace_rest_client-0.1.5.dist-info/WHEEL
+Filename: dspace_rest_client-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: dspace_rest_client-0.1.5.dist-info/top_level.txt
+Filename: dspace_rest_client-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: dspace_rest_client-0.1.5.dist-info/RECORD
+Filename: dspace_rest_client-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dspace_rest_client/client.py

```diff
@@ -13,17 +13,19 @@
 better abstracting and handling of HAL-like API responses, plus just all the other endpoints and operations implemented.
 
 @author Kim Shepherd <kim@shepherd.nz>
 """
 import code
 import json
 import logging
+import sys
 
 import requests
 from requests import Request
+import pysolr
 import os
 from uuid import UUID
 from .models import *
 
 __all__ = ['DSpaceClient']
 
 logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.INFO)
@@ -50,45 +52,53 @@
     Low-level api_get, api_post, api_put, api_delete, api_patch functions are defined to handle the requests and do
     retries / XSRF refreshes where necessary.
     Higher level get, create, update, partial_update (patch) functions are implemented for each DSO type
     """
     # Set up basic environment, variables
     session = None
     API_ENDPOINT = 'http://localhost:8080/server/api'
+    SOLR_ENDPOINT = 'http://localhost:8983/solr'
+    SOLR_AUTH = None
     if 'DSPACE_API_ENDPOINT' in os.environ:
         API_ENDPOINT = os.environ['DSPACE_API_ENDPOINT']
     LOGIN_URL = f'{API_ENDPOINT}/authn/login'
     USERNAME = 'username@test.system.edu'
     if 'DSPACE_API_USERNAME' in os.environ:
         USERNAME = os.environ['DSPACE_API_USERNAME']
     PASSWORD = 'password'
     if 'DSPACE_API_PASSWORD' in os.environ:
         PASSWORD = os.environ['DSPACE_API_PASSWORD']
-
+    if 'SOLR_ENDPOINT' in os.environ:
+        SOLR_ENDPOINT = os.environ['SOLR_ENDPOINT']
+    if 'SOLR_AUTH' in os.environ:
+        SOLR_AUTH = os.environ['SOLR_AUTH']
     verbose = False
 
     # Simple enum for patch operation types
     class PatchOperation:
         ADD = 'add'
         REMOVE = 'remove'
         REPLACE = 'replace'
         MOVE = 'move'
 
-    def __init__(self, api_endpoint=API_ENDPOINT, username=USERNAME, password=PASSWORD):
+    def __init__(self, api_endpoint=API_ENDPOINT, username=USERNAME, password=PASSWORD, solr_endpoint=SOLR_ENDPOINT,
+                 solr_auth=SOLR_AUTH):
         """
         Accept optional API endpoint, username, password arguments using the OS environment variables as defaults
         :param api_endpoint:    base path to DSpace REST API, eg. http://localhost:8080/server/api
         :param username:        username with appropriate privileges to perform operations on REST API
         :param password:        password for the above username
         """
         self.session = requests.Session()
         self.API_ENDPOINT = api_endpoint
         self.LOGIN_URL = f'{self.API_ENDPOINT}/authn/login'
         self.USERNAME = username
         self.PASSWORD = password
+        self.SOLR_ENDPOINT = solr_endpoint
+        self.solr = pysolr.Solr(url=solr_endpoint, always_commit=True, timeout=300, auth=solr_auth)
 
     def authenticate(self):
         """
         Authenticate with the DSpace REST API. As with other operations, perform XSRF refreshes when necessary.
         After POST, check /authn/status and log success if the authenticated json property is true
         @return: response object
         """
@@ -156,14 +166,43 @@
                     logging.warning(f'Too many retries updating token: {r.status_code}: {r.text}')
                 else:
                     logging.debug("Retrying request with updated CSRF token")
                     return self.api_post(url, params=params, json=json, retry=True)
 
         return r
 
+    def api_post_uri(self, url, params, uri_list, retry=False):
+        """
+        Perform a POST request. Refresh XSRF token if necessary.
+        POSTs are typically used to create objects.
+        @param url:     DSpace REST API URL
+        @param params:  Any parameters to include (eg ?parent=abbc-....)
+        @param uri_list: One or more URIs referencing objects
+        @param retry:   Has this method already been retried? Used if we need to refresh XSRF.
+        @return:        Response from API
+        """
+        h = {'Content-type': 'text/uri-list'}
+        r = self.session.post(url, data=uri_list, params=params, headers=h)
+        self.update_token(r)
+
+        if r.status_code == 403:
+            # 403 Forbidden
+            # If we had a CSRF failure, retry the request with the updated token
+            # After speaking in #dev it seems that these do need occasional refreshes but I suspect
+            # it's happening too often for me, so check for accidentally triggering it
+            r_json = r.json()
+            if 'message' in r_json and 'CSRF token' in r_json['message']:
+                if retry:
+                    logging.warning(f'Too many retries updating token: {r.status_code}: {r.text}')
+                else:
+                    logging.debug("Retrying request with updated CSRF token")
+                    return self.api_post(url, params=params, json=json, retry=True)
+
+        return r
+
     def api_put(self, url, params, json, retry=False):
         """
         Perform a PUT request. Refresh XSRF token if necessary.
         PUTs are typically used to update objects.
         @param url:     DSpace REST API URL
         @param params:  Any parameters to include (eg ?parent=abbc-....)
         @param json:    Data in json-ready form (dict) to send as PUT body (eg. item.as_dict())
@@ -274,32 +313,42 @@
         elif r.status_code == 200:
             # 200 Success
             print(f'successful patch update to {r.json()["type"]} {r.json()["id"]}')
 
         # Return the raw API response
         return r
 
-    def search_objects(self, query=None, filters=None, dsoType=None):
+    # PAGINATION
+    def search_objects(self, query=None, filters=None, page=0, size=20, sort=None, dsoType=None):
         """
-        Do a basic search with optional query, filters and dsoType params. TODO: pagination
+        Do a basic search with optional query, filters and dsoType params.
         @param query:   query string
         @param filters: discovery filters as dict eg. {'f.entityType': 'Publication,equals', ... }
+        @param page: page number (not like 'start' as this is not row number, but page number of size {size})
+        @param size: size of page (aka. 'rows'), affects the page parameter above
+        @param sort: sort eg. 'title,asc'
         @param dsoType: DSO type to further filter results
         @return:        list of DspaceObject objects constructed from API resources
         """
         dsos = []
         if filters is None:
             filters = {}
         url = f'{self.API_ENDPOINT}/discover/search/objects'
         # we will add params to filters, so
         params = {}
         if query is not None:
             params['query'] = query
         if dsoType is not None:
             params['dsoType'] = dsoType
+        if size is not None:
+            params['size'] = size
+        if page is not None:
+            params['page'] = page
+        if sort is not None:
+            params['sort'] = sort
 
         r_json = self.fetch_resource(url=url, params={**params, **filters})
 
         # instead lots of 'does this key exist, etc etc' checks, just go for it and wrap in a try?
         try:
             results = r_json['_embedded']['searchResult']['_embedded']['objects']
             for result in results:
@@ -442,15 +491,16 @@
                 print(f'update operation failed: {r.status_code}: {r.text} ({url})')
                 return None
 
         except ValueError as e:
             print(f'{e}')
             return None
 
-    def get_bundles(self, parent=None, uuid=None):
+    # PAGINATION
+    def get_bundles(self, parent=None, uuid=None, page=0, size=20, sort=None):
         """
         Get bundles for an item
         @param parent:  python Item object, from which the UUID will be referenced in the URL.
                         This is mutually exclusive to the 'uuid' argument, returning all bundles for the item.
         @param uuid:    Bundle UUID. This is mutually exclusive to the 'parent' argument, returning just this bundle
         @return:        List of bundles (single UUID bundle result is wrapped in a list before returning)
         """
@@ -461,16 +511,22 @@
         if uuid is not None:
             url = f'{self.API_ENDPOINT}/core/bundles/{uuid}'
             single_result = True
         elif parent is not None:
             url = f'{self.API_ENDPOINT}/core/items/{parent.uuid}/bundles'
         else:
             return list()
-
-        r_json = self.fetch_resource(url, params=None)
+        params = {}
+        if size is not None:
+            params['size'] = size
+        if page is not None:
+            params['page'] = page
+        if sort is not None:
+            params['sort'] = sort
+        r_json = self.fetch_resource(url, params=params)
         try:
             if single_result:
                 bundles.append(Bundle(r_json))
             if not single_result:
                 resources = r_json['_embedded']['bundles']
                 for resource in resources:
                     bundles.append(Bundle(resource))
@@ -490,15 +546,16 @@
         # TODO: It is probably wise to allow the parent UUID to be simply passed as an alternative to having the full
         #  python object as constructed by this REST client, for more flexible usage.
         if parent is None:
             return None
         url = f'{self.API_ENDPOINT}/core/items/{parent.uuid}/bundles'
         return Bundle(api_resource=parse_json(self.api_post(url, params=None, json={'name': name, 'metadata': {}})))
 
-    def get_bitstreams(self, uuid=None, bundle=None, page=0, size=20):
+    # PAGINATION
+    def get_bitstreams(self, uuid=None, bundle=None, page=0, size=20, sort=None):
         """
         Get a specific bitstream UUID, or all bitstreams for a specific bundle
         @param uuid:    UUID of a specific bitstream to retrieve
         @param bundle:  A python Bundle object to parse for bitstream links to retrieve
         @param page:    Page number, for pagination over large result sets (default: 0)
         @param size:    Size of results per page (default: 20)
         @return:        list of python Bitstream objects
@@ -509,15 +566,22 @@
         if uuid is None and isinstance(bundle, Bundle):
             if 'bitstreams' in bundle.links:
                 url = bundle.links['bitstreams']['href']
             else:
                 url = f'{self.API_ENDPOINT}/core/bundles/{bundle.uuid}/bitstreams'
                 print(f'Cannot find bundle bitstream links, will try to construct manually: {url}')
         # Perform the actual request. By now, our URL and parameter should be properly set
-        r_json = self.fetch_resource(url, params={'page': page, 'size': size})
+        params = {}
+        if size is not None:
+            params['size'] = size
+        if page is not None:
+            params['page'] = page
+        if sort is not None:
+            params['sort'] = sort
+        r_json = self.fetch_resource(url, params=params)
         if '_embedded' in r_json:
             if 'bitstreams' in r_json['_embedded']:
                 bitstreams = list()
                 for bitstream_resource in r_json['_embedded']['bitstreams']:
                     bitstreams.append(Bitstream(bitstream_resource))
                 return bitstreams
 
@@ -570,25 +634,32 @@
         if r.status_code == 201 or r.status_code == 200:
             # Success
             return Bitstream(api_resource=parse_json(r))
         else:
             print(f'Error creating bitstream: {r.status_code}: {r.text}')
             return None
 
-    def get_communities(self, uuid=None, page=0, size=20, top=False):
+    # PAGINATION
+    def get_communities(self, uuid=None, page=0, size=20, sort=None, top=False):
         """
         Get communities - either all, for single UUID, or all top-level (ie no sub-communities)
         @param uuid:    string UUID if getting single community
         @param page:    integer page (default: 0)
         @param size:    integer size (default: 20)
         @param top:     whether to restrict search to top communities (default: false)
         @return:        list of communities, or None if error
         """
         url = f'{self.API_ENDPOINT}/core/communities'
-        params = {'page': page, 'size': size}
+        params = {}
+        if size is not None:
+            params['size'] = size
+        if page is not None:
+            params['page'] = page
+        if sort is not None:
+            params['sort'] = sort
         if uuid is not None:
             try:
                 # This isn't used, but it'll throw a ValueError if not a valid UUID
                 id = UUID(uuid).version
                 # Set URL and parameters
                 url = f'{url}/{uuid}'
                 params = None
@@ -624,26 +695,32 @@
         #  to be passed instead of just the UUID as a string
         url = f'{self.API_ENDPOINT}/core/communities'
         params = None
         if parent is not None:
             params = {'parent': parent}
         return Community(api_resource=parse_json(self.create_dso(url, params, data)))
 
-    def get_collections(self, uuid=None, community=None, page=0, size=20):
+    def get_collections(self, uuid=None, community=None, page=0, size=20, sort=None):
         """
         Get collections - all, or single UUID, or for a specific community
         @param uuid:        UUID string. If present, just a single collection is returned (overrides community arg)
         @param community:   Community object. If present (and no uuid present), collections for a community
         @param page:        Integer for page / offset of results. Default: 0
         @param size:        Integer for page size. Default: 20 (same as REST API default)
         @return:            list of Collection objects, or None if there was an error
                             for consistency of handling results, even the uuid search will be a list of one
         """
         url = f'{self.API_ENDPOINT}/core/collections'
-        params = {'page': page, 'size': size}
+        params = {}
+        if size is not None:
+            params['size'] = size
+        if page is not None:
+            params['page'] = page
+        if sort is not None:
+            params['sort'] = sort
         # First, handle case of UUID. It overrides the other arguments as it is a request for a single collection
         if uuid is not None:
             try:
                 id = UUID(uuid).version
                 # Update URL and parameters
                 url = f'{url}/{uuid}'
                 params = None
@@ -788,18 +865,26 @@
 
     def delete_user(self, user):
         if not isinstance(user, User):
             print(f'Must be a valid user')
             return None
         return self.delete_dso(user)
 
-    def get_users(self):
+    # PAGINATION
+    def get_users(self, page=0, size=20, sort=None):
         url = f'{self.API_ENDPOINT}/eperson/epersons'
         users = list()
-        r = self.api_get(url)
+        params = {}
+        if size is not None:
+            params['size'] = size
+        if page is not None:
+            params['page'] = page
+        if sort is not None:
+            params['sort'] = sort
+        r = self.api_get(url, params=params)
         r_json = parse_json(response=r)
         if '_embedded' in r_json:
             if 'epersons' in r_json['_embedded']:
                 for user_resource in r_json['_embedded']['epersons']:
                     users.append(User(user_resource))
         return users
 
@@ -813,14 +898,19 @@
         data = group
         if isinstance(group, Group):
             data = group.as_dict()
             # TODO: Validation. Note, at least here I will just allow a dict instead of the pointless cast<->cast
             # that you see for other DSO types - still figuring out the best way
         return Group(api_resource=parse_json(self.create_dso(url, params=None, data=data)))
 
+    def start_workflow(self, workspace_item):
+        url = f'{self.API_ENDPOINT}/workflow/workflowitems'
+        res = parse_json(self.api_post_uri(url, params=None, uri_list=workspace_item))
+        print(res)
+
     def update_token(self, r):
         """
         Refresh / update the XSRF (aka. CSRF) token if DSPACE-XSRF-TOKEN found in response headers
         This is used by all the base methods like api_put,
         See: https://github.com/DSpace/RestContract/blob/main/csrf-tokens.md
         :param r:
         :return:
@@ -829,7 +919,17 @@
             logging.debug('Session state not found, setting...')
             self.session = requests.Session()
         if 'DSPACE-XSRF-TOKEN' in r.headers:
             t = r.headers['DSPACE-XSRF-TOKEN']
             logging.debug(f'Updating XSRF token to {t}')
             self.session.headers.update({'X-XSRF-Token': t})
             self.session.cookies.update({'X-XSRF-Token': t})
+
+    #WRAPPER
+    def solr_query(self, query, filters=None, fields=None, start=0, rows=999999999):
+        if fields is None:
+            fields = []
+        if filters is None:
+            filters = []
+        return self.solr.search(query, fq=filters, start=start, rows=rows, **{
+            'fl': ','.join(fields)
+        })
```

## dspace_rest_client/models.py

```diff
@@ -38,14 +38,24 @@
             if 'type' in api_resource:
                 self.type = api_resource['type']
             if '_links' in api_resource:
                 self.links = api_resource['_links'].copy()
             else:
                 self.links = {'self': {'href': None}}
 
+class AddressableHALResource(HALResource):
+    id = None
+    def __init__(self, api_resource=None):
+        super().__init__(api_resource)
+        if api_resource is not None:
+            if 'id' in api_resource:
+                self.id = api_resource['id']
+
+    def as_dict(self):
+        return {'id': self.id}
 
 class ExternalDataObject(HALResource):
     """
     Generic External Data Object as configured in DSpace's external data providers framework
     """
     id = None
     display = None
@@ -447,7 +457,64 @@
         @return: dict of User for API use
         """
         dso_dict = super(User, self).as_dict()
         user_dict = {'name': self.name, 'netid': self.netid, 'lastActive': self.lastActive, 'canLogIn': self.canLogIn,
                      'email': self.email, 'requireCertificate': self.requireCertificate,
                      'selfRegistered': self.selfRegistered}
         return {**dso_dict, **user_dict}
+
+class InProgressSubmission(AddressableHALResource):
+    lastModified = None
+    step = None
+    sections = {}
+    type = None
+
+    def __init__(self, api_resource):
+        super(InProgressSubmission, self).__init__(api_resource)
+        if 'lastModified' in api_resource:
+            self.lastModified = api_resource['lastModified']
+        if 'step' in api_resource:
+            self.step = api_resource['lastModified']
+        if 'sections' in api_resource:
+            self.sections = api_resource['sections'].copy()
+        if 'type' in api_resource:
+            self.lastModified = api_resource['lastModified']
+
+    def as_dict(self):
+        parent_dict = super(InProgressSubmission, self).as_dict()
+        dict = {
+            'lastModified': self.lastModified,
+            'step': self.step,
+            'sections': self.sections,
+            'type': self.type
+        }
+        return {**parent_dict, **dict}
+
+class WorkspaceItem(InProgressSubmission):
+
+    def __init__(self, api_resource):
+        super(WorkspaceItem, self).__init__(api_resource)
+
+    def as_dict(self):
+        return super(WorkspaceItem, self).as_dict()
+
+class EntityType(AddressableHALResource):
+    """
+    Extends Addressable HAL Resource to model an entity type (aka item type)
+    used in entities and relationships. For example, Publication, Person, Project and Journal
+    are all common entity types used in DSpace 7+
+    """
+    def __init__(self, api_resource):
+        super(EntityType, self).__init__(api_resource)
+        if 'label' in api_resource:
+            self.label = api_resource['label']
+        if 'type' in api_resource:
+            self.label = api_resource['type']
+
+class RelationshipType(AddressableHALResource):
+    """
+    TODO: RelationshipType
+    """
+    def __init__(self, api_resource):
+        super(RelationshipType, self).__init__(api_resource)
+
+
```

## Comparing `dspace_rest_client-0.1.5.dist-info/LICENSE.txt` & `dspace_rest_client-0.1.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dspace_rest_client-0.1.5.dist-info/METADATA` & `dspace_rest_client-0.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspace-rest-client
-Version: 0.1.5
+Version: 0.1.7
 Summary: A DSpace 7 REST API client library
 Home-page: https://github.com/the-library-code/dspace-rest-client
 Author: Kim Shepherd
 Author-email: kim@the-library-code.de
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `dspace_rest_client-0.1.5.dist-info/RECORD` & `dspace_rest_client-0.1.7.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 dspace_rest_client/__init__.py,sha256=Il5Q9ATdX8yXqVxtP_nYqUhExzxPC_qk_WXQ_4h0exg,16
-dspace_rest_client/client.py,sha256=CGW7dk1Og3_wVV43aMNQvpSuKbSmt5W7CcliLSABUW4,37323
-dspace_rest_client/models.py,sha256=573_3NbK_RqfDdyu0WK_yGKbSFVNOzmpzge1XlkZiTM,16302
-dspace_rest_client-0.1.5.dist-info/LICENSE.txt,sha256=D_YfO8FXUsXKnidXIpVw-G8F190GLqtsWYqmrb5w8pw,1475
-dspace_rest_client-0.1.5.dist-info/METADATA,sha256=faMtIO3Vazze4v_mZ8knIVp317dfYow_2CWF84T39l4,4134
-dspace_rest_client-0.1.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dspace_rest_client-0.1.5.dist-info/top_level.txt,sha256=NyNlqh1QKmVdtI188gUy3xXEMdHvPT3dhiCCiLhZIJ8,19
-dspace_rest_client-0.1.5.dist-info/RECORD,,
+dspace_rest_client/client.py,sha256=4EIZFQccD0NwVnFLBacBAdvar6SVBG-927MaELOWNCY,41325
+dspace_rest_client/models.py,sha256=nWdPbXvaabbsUtpsQaWzOtfwOj_8yWap62SwqpFfDxY,18483
+dspace_rest_client-0.1.7.dist-info/LICENSE.txt,sha256=D_YfO8FXUsXKnidXIpVw-G8F190GLqtsWYqmrb5w8pw,1475
+dspace_rest_client-0.1.7.dist-info/METADATA,sha256=PPNs3c6bRnKo6LknuJkRpD5kllpAZ-4PQKtqNPU7qAc,4134
+dspace_rest_client-0.1.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dspace_rest_client-0.1.7.dist-info/top_level.txt,sha256=NyNlqh1QKmVdtI188gUy3xXEMdHvPT3dhiCCiLhZIJ8,19
+dspace_rest_client-0.1.7.dist-info/RECORD,,
```

