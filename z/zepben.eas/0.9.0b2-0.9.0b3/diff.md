# Comparing `tmp/zepben.eas-0.9.0b2-py3-none-any.whl.zip` & `tmp/zepben.eas-0.9.0b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 12903 bytes, number of entries: 10
--rw-r--r--  2.0 unx      427 b- defN 23-Apr-13 05:46 zepben/eas/__init__.py
--rw-r--r--  2.0 unx      372 b- defN 23-Apr-13 05:46 zepben/eas/client/__init__.py
--rw-r--r--  2.0 unx    11374 b- defN 23-Apr-13 05:46 zepben/eas/client/eas_client.py
--rw-r--r--  2.0 unx     1421 b- defN 23-Apr-13 05:46 zepben/eas/client/study.py
--rw-r--r--  2.0 unx      448 b- defN 23-Apr-13 05:46 zepben/eas/client/util.py
--rw-r--r--  2.0 unx    16725 b- defN 23-Apr-13 05:47 zepben.eas-0.9.0b2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4564 b- defN 23-Apr-13 05:47 zepben.eas-0.9.0b2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 05:47 zepben.eas-0.9.0b2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-13 05:47 zepben.eas-0.9.0b2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      827 b- defN 23-Apr-13 05:47 zepben.eas-0.9.0b2.dist-info/RECORD
-10 files, 36257 bytes uncompressed, 11487 bytes compressed:  68.3%
+Zip file size: 13594 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      382 b- defN 23-Apr-14 00:56 zepben/eas/__init__.py
+-rw-r--r--  2.0 unx      455 b- defN 23-Apr-14 00:56 zepben/eas/client/__init__.py
+-rw-r--r--  2.0 unx    13691 b- defN 23-Apr-14 00:56 zepben/eas/client/eas_client.py
+-rw-r--r--  2.0 unx     1421 b- defN 23-Apr-14 00:56 zepben/eas/client/study.py
+-rw-r--r--  2.0 unx      448 b- defN 23-Apr-14 00:56 zepben/eas/client/util.py
+-rw-r--r--  2.0 unx      490 b- defN 23-Apr-14 00:56 zepben/eas/client/work_package.py
+-rw-r--r--  2.0 unx    16725 b- defN 23-Apr-14 00:57 zepben.eas-0.9.0b3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4564 b- defN 23-Apr-14 00:57 zepben.eas-0.9.0b3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 00:57 zepben.eas-0.9.0b3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-14 00:57 zepben.eas-0.9.0b3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      916 b- defN 23-Apr-14 00:57 zepben.eas-0.9.0b3.dist-info/RECORD
+11 files, 39191 bytes uncompressed, 12036 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -9,23 +9,26 @@
 
 Filename: zepben/eas/client/study.py
 Comment: 
 
 Filename: zepben/eas/client/util.py
 Comment: 
 
-Filename: zepben.eas-0.9.0b2.dist-info/LICENSE
+Filename: zepben/eas/client/work_package.py
 Comment: 
 
-Filename: zepben.eas-0.9.0b2.dist-info/METADATA
+Filename: zepben.eas-0.9.0b3.dist-info/LICENSE
 Comment: 
 
-Filename: zepben.eas-0.9.0b2.dist-info/WHEEL
+Filename: zepben.eas-0.9.0b3.dist-info/METADATA
 Comment: 
 
-Filename: zepben.eas-0.9.0b2.dist-info/top_level.txt
+Filename: zepben.eas-0.9.0b3.dist-info/WHEEL
 Comment: 
 
-Filename: zepben.eas-0.9.0b2.dist-info/RECORD
+Filename: zepben.eas-0.9.0b3.dist-info/top_level.txt
+Comment: 
+
+Filename: zepben.eas-0.9.0b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zepben/eas/__init__.py

```diff
@@ -1,12 +1,10 @@
 #  Copyright 2020 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 #
 
-__all__ = ["EasClient", "Study", "Result", "Section", "StateOverlay", "GeoJsonOverlay"]
-
 from zepben.eas.client.eas_client import EasClient
 from zepben.eas.client.study import *
-
+from zepben.eas.client.work_package import *
```

## zepben/eas/client/__init__.py

```diff
@@ -1,10 +1,11 @@
 #  Copyright 2020 Zeppelin Bend Pty Ltd
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
-__all__ = ["EasClient", "Study"]
+__all__ = ["EasClient", "Study", "WorkPackageConfig"]
 
 from zepben.eas.client.eas_client import EasClient
-from zepben.eas.client.study import Study
+from zepben.eas.client.study import Study
+from zepben.eas.client.work_package import WorkPackageConfig
```

## zepben/eas/client/eas_client.py

```diff
@@ -13,37 +13,38 @@
 import aiohttp
 from aiohttp import ClientSession
 from urllib3.exceptions import InsecureRequestWarning
 from zepben.auth import AuthMethod, ZepbenTokenFetcher, create_token_fetcher
 
 from zepben.eas.client.study import Study
 from zepben.eas.client.util import construct_url
+from zepben.eas.client.work_package import WorkPackageConfig
 
 __all__ = ["EasClient"]
 
 
 class EasClient:
     """
     A class used to represent a client to the Evolve App Server, with methods that represent requests to its API.
     """
 
     def __init__(
-        self,
-        host: str,
-        port: int,
-        protocol: str = "https",
-        client_id: Optional[str] = None,
-        username: Optional[str] = None,
-        password: Optional[str] = None,
-        client_secret: Optional[str] = None,
-        token_fetcher: Optional[ZepbenTokenFetcher] = None,
-        verify_certificate: bool = True,
-        ca_filename: Optional[str] = None,
-        session: ClientSession = None,
-        json_serialiser = None
+            self,
+            host: str,
+            port: int,
+            protocol: str = "https",
+            client_id: Optional[str] = None,
+            username: Optional[str] = None,
+            password: Optional[str] = None,
+            client_secret: Optional[str] = None,
+            token_fetcher: Optional[ZepbenTokenFetcher] = None,
+            verify_certificate: bool = True,
+            ca_filename: Optional[str] = None,
+            session: ClientSession = None,
+            json_serialiser=None
     ):
         """
         Construct a client for the Evolve App Server. If the server is HTTPS, authentication may be configured.
         Authentication may be configured in one of two ways:
             - Specifying the client ID of the Auth0 application via the client_id parameter, plus one of the following:
                 - A username and password pair via the username and password parameters (account authentication)
                 - The client secret via the client_secret parameter (M2M authentication)
@@ -165,14 +166,60 @@
         headers = {"content-type": content_type}
         if self._token_fetcher is None:
             return headers
         else:
             headers["authorization"] = self._token_fetcher.fetch_token()
         return headers
 
+    def run_hosting_capacity_work_package(self, work_package: WorkPackageConfig):
+        """
+        Send request to hosting capacity service to run work package
+
+        :param work_package: An instance of the `WorkPackageConfig` data class representing the work package configuration for the run
+        :return: The HTTP response received from the Evolve App Server after attempting to run work package
+        """
+        return get_event_loop().run_until_complete(self.async_run_hosting_capacity_work_package(work_package))
+
+    async def async_run_hosting_capacity_work_package(self, work_package: WorkPackageConfig):
+        """
+        Send asynchronous request to hosting capacity service to run work package
+
+        :param work_package: An instance of the `WorkPackageConfig` data class representing the work package configuration for the run
+        :return: The HTTP response received from the Evolve App Server after attempting to run work package
+        """
+        with warnings.catch_warnings():
+            if not self._verify_certificate:
+                warnings.filterwarnings("ignore", category=InsecureRequestWarning)
+            json = {
+                "query": """
+                    mutation runHostingCapacity($input: WorkPackageInput!) {
+                        runHostingCapacity(input: $input)
+                    }
+                """,
+                "variables": {
+                    "input": {
+                        "feeders": work_package.feeders
+                    }
+                }
+            }
+            if self._verify_certificate:
+                sslcontext = ssl.create_default_context(cafile=self._ca_filename)
+
+            async with self.session.post(
+                    construct_url(protocol=self._protocol, host=self._host, port=self._port, path="/api/graphql"),
+                    headers=self._get_request_headers(),
+                    json=json,
+                    ssl=sslcontext if self._verify_certificate else False
+            ) as response:
+                if response.ok:
+                    response = await response.json()
+                else:
+                    response = await response.text()
+                return response
+
     def upload_study(self, study: Study):
         """
         Uploads a new study to the Evolve App Server
         :param study: An instance of a data class representing a new study
         """
         return get_event_loop().run_until_complete(self.async_upload_study(study))
```

## Comparing `zepben.eas-0.9.0b2.dist-info/LICENSE` & `zepben.eas-0.9.0b3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zepben.eas-0.9.0b2.dist-info/METADATA` & `zepben.eas-0.9.0b3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zepben.eas
-Version: 0.9.0b2
+Version: 0.9.0b3
 Summary: Python SDK for interacting with the Evolve App Server
 Home-page: https://bitbucket.org/zepben/eas-python-client
 Author: Ramon Bouckaert
 Author-email: ramon.bouckaert@zepben.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

