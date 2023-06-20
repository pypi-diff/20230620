# Comparing `tmp/polyswarm-api-3.2.0.tar.gz` & `tmp/polyswarm-api-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyswarm-api-3.2.0.tar", last modified: Tue Mar 21 20:11:10 2023, max compression
+gzip compressed data, was "polyswarm-api-3.3.2.tar", last modified: Tue Jun 20 20:09:43 2023, max compression
```

## Comparing `polyswarm-api-3.2.0.tar` & `polyswarm-api-3.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:11:10.382619 polyswarm-api-3.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1756 2023-03-21 20:11:10.382619 polyswarm-api-3.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-21 20:11:10.382619 polyswarm-api-3.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:11:10.382619 polyswarm-api-3.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:11:10.382619 polyswarm-api-3.2.0/src/polyswarm_api/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/src/polyswarm_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    31285 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/src/polyswarm_api/api.py
--rw-rw-rw-   0 root         (0) root         (0)    20072 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/src/polyswarm_api/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/src/polyswarm_api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    36029 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/src/polyswarm_api/resources.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/src/polyswarm_api/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:11:10.382619 polyswarm-api-3.2.0/src/polyswarm_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1756 2023-03-21 20:11:10.000000 polyswarm-api-3.2.0/src/polyswarm_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-03-21 20:11:10.000000 polyswarm-api-3.2.0/src/polyswarm_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-21 20:11:10.000000 polyswarm-api-3.2.0/src/polyswarm_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-03-21 20:11:10.000000 polyswarm-api-3.2.0/src/polyswarm_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-21 20:11:10.000000 polyswarm-api-3.2.0/src/polyswarm_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:09:43.832358 polyswarm-api-3.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-06-20 20:09:43.828359 polyswarm-api-3.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 20:09:43.832358 polyswarm-api-3.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:09:43.828359 polyswarm-api-3.3.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:09:43.828359 polyswarm-api-3.3.2/src/polyswarm_api/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/src/polyswarm_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    35276 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/src/polyswarm_api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20066 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/src/polyswarm_api/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/src/polyswarm_api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    39808 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/src/polyswarm_api/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2023-06-20 20:09:20.000000 polyswarm-api-3.3.2/src/polyswarm_api/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:09:43.828359 polyswarm-api-3.3.2/src/polyswarm_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-06-20 20:09:43.000000 polyswarm-api-3.3.2/src/polyswarm_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-20 20:09:43.000000 polyswarm-api-3.3.2/src/polyswarm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 20:09:43.000000 polyswarm-api-3.3.2/src/polyswarm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-20 20:09:43.000000 polyswarm-api-3.3.2/src/polyswarm_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-20 20:09:43.000000 polyswarm-api-3.3.2/src/polyswarm_api.egg-info/top_level.txt
```

### Comparing `polyswarm-api-3.2.0/LICENSE` & `polyswarm-api-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.2.0/PKG-INFO` & `polyswarm-api-3.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: polyswarm-api
-Version: 3.2.0
+Version: 3.3.2
 Summary: Client library to simplify interacting with the PolySwarm consumer API
 Home-page: https://github.com/polyswarm/polyswarm-api
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,<4
+Requires-Python: >=3.5,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # polyswarm-api
 
 An interface to the PolySwarm Customer APIs.
 For an easy-to-use CLI tool, or as an example of how to use these APIs, please see [polyswarm-cli](https://github.com/polyswarm/polyswarm-cli)
```

### Comparing `polyswarm-api-3.2.0/README.md` & `polyswarm-api-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.2.0/setup.py` & `polyswarm-api-3.3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,36 +5,34 @@
 # The README.md will be used as the content for the PyPi package details page on the Python Package Index.
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 
 setup(
     name='polyswarm-api',
-    version='3.2.0',
+    version='3.3.2',
     description='Client library to simplify interacting with the PolySwarm consumer API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='PolySwarm Developers',
     author_email='info@polyswarm.io',
     url='https://github.com/polyswarm/polyswarm-api',
     license='MIT',
-    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,<4',
+    python_requires='>=3.5,<4',
     install_requires=[
         'requests~=2.22',
         'future~=0.18',
         'python-dateutil~=2.8',
     ],
     extras_require={':python_version < "3.0"': ['enum34==1.1.6']},
     include_package_data=True,
     packages=find_packages('src'),
     package_dir={'': 'src'},
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: Implementation :: PyPy',
     ]
 )
```

### Comparing `polyswarm-api-3.2.0/src/polyswarm_api/api.py` & `polyswarm-api-3.3.2/src/polyswarm_api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -651,24 +651,95 @@
         logger.info('Downloading %s into %s', hash_, out_dir)
         hash_ = resources.Hash.from_hashable(hash_, hash_type=hash_type)
         artifact = resources.LocalArtifact.download(self, hash_.hash, hash_.hash_type, folder=out_dir).result()
         artifact.handle.close()
 
         return artifact
 
-    def sandbox(self, instance_id):
-        logger.info('Sandboxing %s', instance_id)
-        return resources.SandboxResult.create(self, artifact_id=instance_id).result()
+    def download_id(self, out_dir, instance_id):
+        """
+        Grab the data of artifact identified by hash, and write the data to a file in the provided directory
+        under a file named after the hash_.
+        :param out_dir: Destination directory to download the file.
+        :param instance_id: The instance id we should use to lookup the artifact to download.
+        :return: A LocalArtifact resource
+        """
+        logger.info('Downloading %s into %s', instance_id, out_dir)
+        artifact = resources.LocalArtifact.download_id(self, instance_id, folder=out_dir).result()
+        artifact.handle.close()
+
+        return artifact
+
+    def sandbox(self, instance_id, sandbox):
+        logger.info('Sandboxing %s in %s', instance_id, sandbox)
+        return resources.SandboxTask.create(self, artifact_id=instance_id, sandbox=sandbox).result()
+
+    def sandbox_file(self, artifact, sandbox, artifact_type=resources.ArtifactType.FILE, artifact_name=None):
+        logger.info('Sandboxing file in %s', sandbox)
+        artifact_type = resources.ArtifactType.parse(artifact_type)
+        # TODO This is a python 2.7 check if artifact is a file-like instance, consider changing
+        #  to isinstance(artifact, io.IOBase) when deprecating 2.7 and implementing making LocalHandle
+        #  inherit io.IOBase, although this will change the method delegation logic in the resource
+        if hasattr(artifact, 'read') and hasattr(artifact.read, '__call__'):
+            artifact = resources.LocalArtifact.from_handle(self, artifact, artifact_name=artifact_name or '',
+                                                           artifact_type=artifact_type)
+        elif isinstance(artifact, string_types):
+            if artifact_type == resources.ArtifactType.FILE:
+                artifact = resources.LocalArtifact.from_path(self, artifact, artifact_type=artifact_type,
+                                                             artifact_name=artifact_name)
+            elif artifact_type == resources.ArtifactType.URL:
+                artifact = resources.LocalArtifact.from_content(self, artifact,
+                                                                artifact_name=artifact_name or artifact,
+                                                                artifact_type=artifact_type)
+        if isinstance(artifact, resources.LocalArtifact):
+            task = resources.SandboxTask.create_file(self,
+                                                     artifact_name=artifact.artifact_name,
+                                                     artifact_type=artifact.artifact_type.name,
+                                                     community=self.community,
+                                                     sandbox=sandbox).result()
+            task.upload_file(artifact)
+            return resources.SandboxTask.update_file(self, id=task.id).result()
+        else:
+            raise exceptions.InvalidValueException(
+                'Artifacts should be a path to a file or a LocalArtifact instance')
 
-    def sandbox_list(self):
+    def sandbox_providers(self):
         """
         List sandboxes available in polyswarm.
         """
         logger.info('Listing sandbox names')
-        return resources.SandboxName.list(self)
+        return resources.SandboxProvider.list(self)
+
+    def sandbox_task_status(self, sandbox_task_id):
+        """
+        Check the status of a sandbox task.
+        """
+        logger.info('Checking the status of sandbox task %s', sandbox_task_id)
+        return resources.SandboxTask.get(self, sandbox_task_id=sandbox_task_id).result()
+
+    def sandbox_task_latest(self, sha256, sandbox):
+        """
+        Check the latest status of a sandbox task.
+        """
+        logger.info('Checking the sandbox task for %s', sha256)
+        return resources.SandboxTask.latest(self, sha256=sha256, sandbox=sandbox).result()
+
+    def sandbox_my_tasks_list(self, **kwargs):
+        """
+        Check the latest status of a sandbox task.
+        """
+        logger.info('Checking the latest tasks created by my account')
+        return resources.SandboxTask.my_tasks(self, **kwargs).result()
+
+    def sandbox_task_list(self, sha256, **kwargs):
+        """
+        Check the list of a sandbox tasks.
+        """
+        logger.info('Checking the sandbox tasks for %s', sha256)
+        return resources.SandboxTask.list(self, sha256=sha256, **kwargs).result()
 
     def download_archive(self, out_dir, s3_path):
         """
         Grab the data in the s3 path provided in the stream() method, and write the contents
         in the provided directory.
         :param out_dir: Destination directory to download the file.
         :param s3_path: Target S3 object to download.
```

### Comparing `polyswarm-api-3.2.0/src/polyswarm_api/core.py` & `polyswarm-api-3.3.2/src/polyswarm_api/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 
     def consume_results(self):
         # StopIteration is deprecated
         # As per https://www.python.org/dev/peps/pep-0479/
         # We simply return upon termination condition
         request = self
         while True:
-            # consume items items from list if iterable
+            # consume items from list if iterable
             # of yield the single result if not
             try:
                 for result in request._result:
                     yield result
             except TypeError:
                 yield request._result
                 # if the result is not a list, there is not next page
```

### Comparing `polyswarm-api-3.2.0/src/polyswarm_api/exceptions.py` & `polyswarm-api-3.3.2/src/polyswarm_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.2.0/src/polyswarm_api/resources.py` & `polyswarm-api-3.3.2/src/polyswarm_api/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -638,14 +638,30 @@
             result_parser=cls,
             handle=handle,
             folder=folder,
             artifact_name=artifact_name,
         ).execute()
 
     @classmethod
+    def download_id(cls, api, instance_id, handle=None, folder=None, artifact_name=None):
+        return core.PolyswarmRequest(
+            api,
+            {
+                'method': 'GET',
+                'url': '{}/instance/download'.format(api.uri),
+                'stream': True,
+                'params': {'instance_id': instance_id},
+            },
+            result_parser=cls,
+            handle=handle,
+            folder=folder,
+            artifact_name=artifact_name,
+        ).execute()
+
+    @classmethod
     def download_archive(cls, api, u, handle=None, folder=None, artifact_name=None):
         """ This method is special, in that it is simply for downloading from S3 """
         return core.PolyswarmRequest(
             api,
             {
                 'method': 'GET',
                 'url': u,
@@ -971,18 +987,89 @@
     def __str__(self):
         return self.hash
 
     def __repr__(self):
         return "{}={}".format(self.hash_type, self.hash)
 
 
-class SandboxResult(ArtifactInstance):
-    RESOURCE_ENDPOINT = "/sandbox"
-    RESOURCE_ID_KEYS = ['artifact_id']
+class SandboxTask(core.BaseJsonResource):
+    RESOURCE_ENDPOINT = '/sandbox/sandboxtask'
+
+    def __init__(self, content, api=None):
+        super(SandboxTask, self).__init__(content, api=api)
+        self.id = content['id']
+        self.community = content['community']
+        self.sandbox = content['sandbox']
+        self.created = content['created']
+        self.expiration = content['expiration']
+        self.status = content['status']
+        self.account_number = content['account_number']
+        self.team_account_number = content['team_account_number']
+        self.instance_id = content['instance_id']
+        self.sha256 = content['sha256']
+        self.report = content['report']
+        self.upload_url = content['upload_url']
+        self.sandbox_artifacts = [SandboxArtifact(a, api=api) for a in content.get('sandbox_artifacts', [])]
+
+    def upload_file(self, artifact, attempts=3, **kwargs):
+        if not self.upload_url:
+            raise exceptions.InvalidValueException('upload_url must be set to upload a file')
+        if not artifact:
+            raise exceptions.InvalidValueException('A LocalArtifact must be provided in order to upload')
+        r = None
+        while attempts > 0 and not r:
+            attempts -= 1
+            artifact.seek(0, io.SEEK_END)
+            length = artifact.tell()
+            artifact.seek(0)
+            # https://github.com/psf/requests/issues/4215#issuecomment-319521235
+            # We have to manually handle the case when the file is empty
+            # in a way that requests won't set Transfer-Encoding: chunked
+            if not length:
+                artifact = ''
+            r = requests.put(self.upload_url, data=artifact, **kwargs)
+            r.raise_for_status()
+        return r
+
+    @classmethod
+    def get(cls, api, **kwargs):
+        return super().get(api, community=api.community, **kwargs)
+
+    @classmethod
+    def latest(cls, api, **kwargs):
+        params, _ = cls._get_params(community=api.community, **kwargs)
+        url = cls._endpoint(api) + '/latest'
+        parameters = {'method': 'GET', 'url': url, 'params': params}
+        return core.PolyswarmRequest(api, parameters, result_parser=cls).execute()
+
+    @classmethod
+    def my_tasks(cls, api, **kwargs):
+        params, _ = cls._get_params(community=api.community, **kwargs)
+        url = cls._endpoint(api) + '/my-tasks'
+        parameters = {'method': 'GET', 'url': url, 'params': params}
+        return core.PolyswarmRequest(api, parameters, result_parser=cls).execute()
+
+    @classmethod
+    def create_file(cls, api, **kwargs):
+        return cls._build_request(api, 'POST', cls._create_endpoint(api, **kwargs) + '/instance',
+                                  cls._create_headers(api), *cls._create_params(**kwargs)).execute()
 
+    @classmethod
+    def update_file(cls, api, **kwargs):
+        return cls._build_request(api, 'PUT', cls._update_endpoint(api, **kwargs) + '/instance',
+                                  cls._update_headers(api), *cls._update_params(**kwargs)).execute()
 
-class SandboxName(core.BaseJsonResource):
-    RESOURCE_ENDPOINT = "/sandbox/name"
 
+class SandboxArtifact(core.BaseJsonResource):
     def __init__(self, content, api=None):
-        super(SandboxName, self).__init__(content, api=api)
-        self.name = content
+        super(SandboxArtifact, self).__init__(content, api=api)
+        self.created = content['created']
+        self.id = content['id']
+        self.instance_id = content['instance_id']
+        self.name = content['name']
+        self.mimetype = content['mimetype']
+        self.extended_type = content['extended_type']
+        self.type = content['type']
+
+
+class SandboxProvider(core.BaseJsonResource):
+    RESOURCE_ENDPOINT = "/sandbox/provider"
```

### Comparing `polyswarm-api-3.2.0/src/polyswarm_api/settings.py` & `polyswarm-api-3.3.2/src/polyswarm_api/settings.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.2.0/src/polyswarm_api.egg-info/PKG-INFO` & `polyswarm-api-3.3.2/src/polyswarm_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: polyswarm-api
-Version: 3.2.0
+Version: 3.3.2
 Summary: Client library to simplify interacting with the PolySwarm consumer API
 Home-page: https://github.com/polyswarm/polyswarm-api
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,<4
+Requires-Python: >=3.5,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # polyswarm-api
 
 An interface to the PolySwarm Customer APIs.
 For an easy-to-use CLI tool, or as an example of how to use these APIs, please see [polyswarm-cli](https://github.com/polyswarm/polyswarm-cli)
```

