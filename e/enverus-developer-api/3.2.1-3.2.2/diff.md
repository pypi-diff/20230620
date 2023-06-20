# Comparing `tmp/enverus-developer-api-3.2.1.tar.gz` & `tmp/enverus-developer-api-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enverus-developer-api-3.2.1.tar", last modified: Tue Mar 21 13:37:31 2023, max compression
+gzip compressed data, was "enverus-developer-api-3.2.2.tar", last modified: Tue Jun 20 17:28:26 2023, max compression
```

## Comparing `enverus-developer-api-3.2.1.tar` & `enverus-developer-api-3.2.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 13:37:31.882371 enverus-developer-api-3.2.1/
--rw-rw-rw-   0        0        0     1068 2023-03-21 12:05:03.000000 enverus-developer-api-3.2.1/LICENSE.md
--rw-rw-rw-   0        0        0     9611 2023-03-21 13:37:31.882371 enverus-developer-api-3.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     8608 2023-03-21 12:05:03.000000 enverus-developer-api-3.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-21 13:37:31.868843 enverus-developer-api-3.2.1/enverus_developer_api/
--rw-rw-rw-   0        0        0    27282 2023-03-21 12:05:03.000000 enverus-developer-api-3.2.1/enverus_developer_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-21 13:37:31.880386 enverus-developer-api-3.2.1/enverus_developer_api.egg-info/
--rw-rw-rw-   0        0        0     9611 2023-03-21 13:37:31.000000 enverus-developer-api-3.2.1/enverus_developer_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-03-21 13:37:31.000000 enverus-developer-api-3.2.1/enverus_developer_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 13:37:31.000000 enverus-developer-api-3.2.1/enverus_developer_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-03-21 13:37:31.000000 enverus-developer-api-3.2.1/enverus_developer_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-03-21 13:37:31.000000 enverus-developer-api-3.2.1/enverus_developer_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-03-21 13:37:31.883891 enverus-developer-api-3.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1757 2023-03-21 12:16:13.000000 enverus-developer-api-3.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:28:26.911379 enverus-developer-api-3.2.2/
+-rw-rw-rw-   0        0        0     1068 2023-06-20 17:00:05.000000 enverus-developer-api-3.2.2/LICENSE.md
+-rw-rw-rw-   0        0        0     9916 2023-06-20 17:28:26.911379 enverus-developer-api-3.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8906 2023-06-20 17:00:05.000000 enverus-developer-api-3.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 17:28:26.887164 enverus-developer-api-3.2.2/enverus_developer_api/
+-rw-rw-rw-   0        0        0    27468 2023-06-20 17:00:06.000000 enverus-developer-api-3.2.2/enverus_developer_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:28:26.908867 enverus-developer-api-3.2.2/enverus_developer_api.egg-info/
+-rw-rw-rw-   0        0        0     9916 2023-06-20 17:28:26.000000 enverus-developer-api-3.2.2/enverus_developer_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-20 17:28:26.000000 enverus-developer-api-3.2.2/enverus_developer_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 17:28:26.000000 enverus-developer-api-3.2.2/enverus_developer_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-06-20 17:28:26.000000 enverus-developer-api-3.2.2/enverus_developer_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-20 17:28:26.000000 enverus-developer-api-3.2.2/enverus_developer_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-06-20 17:28:26.916805 enverus-developer-api-3.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1807 2023-06-20 17:02:15.000000 enverus-developer-api-3.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:28:26.909866 enverus-developer-api-3.2.2/tests/
+-rw-rw-rw-   0        0        0     9122 2023-06-20 17:00:06.000000 enverus-developer-api-3.2.2/tests/test___init__.py
```

### Comparing `enverus-developer-api-3.2.1/LICENSE.md` & `enverus-developer-api-3.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `enverus-developer-api-3.2.1/PKG-INFO` & `enverus-developer-api-3.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enverus-developer-api
-Version: 3.2.1
+Version: 3.2.2
 Summary: Enverus Developer API Python Client
 Home-page: https://github.com/enverus-ea/enverus-developer-api
 Author: Direct Access
 Author-email: directaccess@enverus.com
 License: MIT
 Keywords: enverus,drillinginfo,directaccess,oil,gas
 Classifier: Development Status :: 5 - Production/Stable
@@ -255,7 +255,13 @@
   converters={
     "StateProvince": lambda x: "TEXAS",
     "ENVOperator": lambda x: x.replace(",", "")
   }
 )
 df.head(10)
 ```
+Reset the index of the DataFrame, and use the default one instead. [reset_index()](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.reset_index.html)
+```python
+    df = v3.to_dataframe(dataset, pagesize=10000, ENVBasin="SACRAMENTO")
+    df.reset_index(inplace=True)
+    df.head(10)
+```
```

### Comparing `enverus-developer-api-3.2.1/README.md` & `enverus-developer-api-3.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -235,7 +235,13 @@
   converters={
     "StateProvince": lambda x: "TEXAS",
     "ENVOperator": lambda x: x.replace(",", "")
   }
 )
 df.head(10)
 ```
+Reset the index of the DataFrame, and use the default one instead. [reset_index()](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.reset_index.html)
+```python
+    df = v3.to_dataframe(dataset, pagesize=10000, ENVBasin="SACRAMENTO")
+    df.reset_index(inplace=True)
+    df.head(10)
+```
```

### Comparing `enverus-developer-api-3.2.1/enverus_developer_api/__init__.py` & `enverus-developer-api-3.2.2/enverus_developer_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from collections import OrderedDict
 
 import requests
 import unicodecsv as csv
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 from requests.utils import parse_header_links
+
+
 class DAAuthException(Exception):
     pass
 
 
 class DAQueryException(Exception):
     pass
 
@@ -67,14 +69,22 @@
             total=self.retries,
             backoff_factor=self.backoff_factor,
             allowed_methods=frozenset(["GET", "POST", "HEAD"]),
             status_forcelist=self._status_forcelist,
         )
         self.session.mount("https://", HTTPAdapter(max_retries=retries))
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if self.session:
+            self.session.close()
+        self.session = None
+
     def get_access_token(self):
         raise NotImplementedError
 
     def to_csv(self, query, path, log_progress=True, **kwargs):
         """
         Write query results to CSV. Optional keyword arguments are
         provided to the csv writer object, allowing control over
```

### Comparing `enverus-developer-api-3.2.1/enverus_developer_api.egg-info/PKG-INFO` & `enverus-developer-api-3.2.2/enverus_developer_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enverus-developer-api
-Version: 3.2.1
+Version: 3.2.2
 Summary: Enverus Developer API Python Client
 Home-page: https://github.com/enverus-ea/enverus-developer-api
 Author: Direct Access
 Author-email: directaccess@enverus.com
 License: MIT
 Keywords: enverus,drillinginfo,directaccess,oil,gas
 Classifier: Development Status :: 5 - Production/Stable
@@ -255,7 +255,13 @@
   converters={
     "StateProvince": lambda x: "TEXAS",
     "ENVOperator": lambda x: x.replace(",", "")
   }
 )
 df.head(10)
 ```
+Reset the index of the DataFrame, and use the default one instead. [reset_index()](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.reset_index.html)
+```python
+    df = v3.to_dataframe(dataset, pagesize=10000, ENVBasin="SACRAMENTO")
+    df.reset_index(inplace=True)
+    df.head(10)
+```
```

### Comparing `enverus-developer-api-3.2.1/setup.py` & `enverus-developer-api-3.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import os
 import sys
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
-VERSION = '3.2.1'
+VERSION = '3.2.2'
 
 
 class VerifyVersionCommand(install):
     description = 'verify that git tag matches VERSION prior to publishing to pypi'
 
     def run(self):
         tag = os.getenv('CIRCLE_TAG')
@@ -40,15 +40,19 @@
     author='Direct Access',
     author_email='directaccess@enverus.com',
     url='https://github.com/enverus-ea/enverus-developer-api',
     license='MIT',
     keywords=['enverus', 'drillinginfo', 'directaccess', 'oil', 'gas'],
     packages=find_packages(exclude=('test*', )),
     package_dir={'enverus_developer_api': 'enverus_developer_api'},
-    install_requires=['requests>=2.5.1, <3', 'unicodecsv==0.14.1'],
+    install_requires=[
+        'requests>=2.5.1,<3',
+        'unicodecsv==0.14.1',
+        'urllib3>=1.26.14',
+    ],
     extras_require={'pandas': pandas},
     cmdclass={
         'verify': VerifyVersionCommand,
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

