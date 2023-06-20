# Comparing `tmp/otools-rpc-0.3.0.tar.gz` & `tmp/otools-rpc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otools-rpc-0.3.0.tar", last modified: Tue May 30 13:54:57 2023, max compression
+gzip compressed data, was "otools-rpc-0.3.1.tar", last modified: Tue Jun 20 08:50:11 2023, max compression
```

## Comparing `otools-rpc-0.3.0.tar` & `otools-rpc-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-30 13:54:57.795054 otools-rpc-0.3.0/
--rw-r--r--   0 opennet   (1000) opennet   (1000)     1326 2023-05-30 13:44:29.000000 otools-rpc-0.3.0/LICENSE.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     4072 2023-05-30 13:54:57.795054 otools-rpc-0.3.0/PKG-INFO
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     3450 2023-05-30 13:44:29.000000 otools-rpc-0.3.0/README.md
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-30 13:54:57.791054 otools-rpc-0.3.0/otools_rpc/
--rw-r--r--   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:36:09.000000 otools-rpc-0.3.0/otools_rpc/__init__.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-30 13:54:57.795054 otools-rpc-0.3.0/otools_rpc/db_manager/
--rw-r--r--   0 opennet   (1000) opennet   (1000)       38 2023-05-30 12:59:41.000000 otools-rpc-0.3.0/otools_rpc/db_manager/__init__.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     1168 2023-05-30 13:44:29.000000 otools-rpc-0.3.0/otools_rpc/db_manager/database_utils.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-30 13:54:57.795054 otools-rpc-0.3.0/otools_rpc/external_api/
--rw-r--r--   0 opennet   (1000) opennet   (1000)       37 2023-05-22 13:36:09.000000 otools-rpc-0.3.0/otools_rpc/external_api/__init__.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     1943 2023-05-30 13:50:43.000000 otools-rpc-0.3.0/otools_rpc/external_api/common.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     5083 2023-05-30 13:50:43.000000 otools-rpc-0.3.0/otools_rpc/external_api/environment.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     6943 2023-05-30 13:50:43.000000 otools-rpc-0.3.0/otools_rpc/external_api/recordset.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-30 13:54:57.795054 otools-rpc-0.3.0/otools_rpc.egg-info/
--rw-r--r--   0 opennet   (1000) opennet   (1000)     4072 2023-05-30 13:54:57.000000 otools-rpc-0.3.0/otools_rpc.egg-info/PKG-INFO
--rw-r--r--   0 opennet   (1000) opennet   (1000)      442 2023-05-30 13:54:57.000000 otools-rpc-0.3.0/otools_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 opennet   (1000) opennet   (1000)        1 2023-05-30 13:54:57.000000 otools-rpc-0.3.0/otools_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 opennet   (1000) opennet   (1000)       63 2023-05-30 13:54:57.000000 otools-rpc-0.3.0/otools_rpc.egg-info/requires.txt
--rw-r--r--   0 opennet   (1000) opennet   (1000)       11 2023-05-30 13:54:57.000000 otools-rpc-0.3.0/otools_rpc.egg-info/top_level.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)       38 2023-05-30 13:54:57.795054 otools-rpc-0.3.0/setup.cfg
--rw-r--r--   0 opennet   (1000) opennet   (1000)     1047 2023-05-30 13:50:43.000000 otools-rpc-0.3.0/setup.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-20 08:50:11.218897 otools-rpc-0.3.1/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1326 2023-05-30 13:44:29.000000 otools-rpc-0.3.1/LICENSE.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     4072 2023-06-20 08:50:11.218897 otools-rpc-0.3.1/PKG-INFO
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     3450 2023-05-30 13:44:29.000000 otools-rpc-0.3.1/README.md
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-20 08:50:11.214897 otools-rpc-0.3.1/otools_rpc/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:36:09.000000 otools-rpc-0.3.1/otools_rpc/__init__.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-20 08:50:11.218897 otools-rpc-0.3.1/otools_rpc/db_manager/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       38 2023-05-30 12:59:41.000000 otools-rpc-0.3.1/otools_rpc/db_manager/__init__.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1168 2023-05-30 13:44:29.000000 otools-rpc-0.3.1/otools_rpc/db_manager/database_utils.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-20 08:50:11.218897 otools-rpc-0.3.1/otools_rpc/external_api/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       62 2023-06-20 08:47:34.000000 otools-rpc-0.3.1/otools_rpc/external_api/__init__.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     3402 2023-06-20 08:47:34.000000 otools-rpc-0.3.1/otools_rpc/external_api/cache.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1969 2023-06-16 14:20:26.000000 otools-rpc-0.3.1/otools_rpc/external_api/common.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     5257 2023-06-20 08:47:34.000000 otools-rpc-0.3.1/otools_rpc/external_api/environment.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     6930 2023-06-20 08:47:34.000000 otools-rpc-0.3.1/otools_rpc/external_api/recordset.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-20 08:50:11.218897 otools-rpc-0.3.1/otools_rpc.egg-info/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     4072 2023-06-20 08:50:11.000000 otools-rpc-0.3.1/otools_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 opennet   (1000) opennet   (1000)      475 2023-06-20 08:50:11.000000 otools-rpc-0.3.1/otools_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)        1 2023-06-20 08:50:11.000000 otools-rpc-0.3.1/otools_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       63 2023-06-20 08:50:11.000000 otools-rpc-0.3.1/otools_rpc.egg-info/requires.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       11 2023-06-20 08:50:11.000000 otools-rpc-0.3.1/otools_rpc.egg-info/top_level.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)       38 2023-06-20 08:50:11.218897 otools-rpc-0.3.1/setup.cfg
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1047 2023-06-20 08:47:33.000000 otools-rpc-0.3.1/setup.py
```

### Comparing `otools-rpc-0.3.0/LICENSE.txt` & `otools-rpc-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.3.0/PKG-INFO` & `otools-rpc-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otools-rpc
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tool to interact with Odoo's external API.
 Home-page: https://github.com/MrFaBemol/otools-rpc
 Author: Gautier Casabona
 Author-email: gcasabona.pro@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `otools-rpc-0.3.0/README.md` & `otools-rpc-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.3.0/otools_rpc/db_manager/database_utils.py` & `otools-rpc-0.3.1/otools_rpc/db_manager/database_utils.py`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.3.0/otools_rpc/external_api/common.py` & `otools-rpc-0.3.1/otools_rpc/external_api/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             return fn(self, other)
         return wrapper
     return decorator
 
 def cache(op=None):
     def decorator(fn):
         def wrapper(self, *args, **kwargs):
-            print(f"Cache {op or fn.__name__} on {self}")
+            self.env.logger.log("FTRACE", f"[CACHE] {op or fn.__name__} on {self}")
             return fn(self, *args, **kwargs)
         return wrapper
     return decorator
 
 
 
 # --------------------------------------------
```

### Comparing `otools-rpc-0.3.0/otools_rpc/external_api/environment.py` & `otools-rpc-0.3.1/otools_rpc/external_api/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import xmlrpc.client
 import re
 import copy
 from typing import Union
 from loguru import logger as loguru_logger
 from .recordset import RecordSet
 from .common import frozendict
+from .cache import Cache
 
 
 class Environment(dict):
     # Todo: Add a cache system
 
     def __init__(
             self,
@@ -29,23 +30,25 @@
         self._password = password
         self._db = db or self._extract_db_from_url()
 
         self.common = xmlrpc.client.ServerProxy(f"{self._url}/xmlrpc/2/common", allow_none=True)
         self.models = None
 
         self.requests = list()
-        self.cache = {}
+        # self.cache = Cache(self)
+        self.cache = dict()
         self._context = frozendict()
 
         # Todo: make it an object
         self.user = None
 
         self.logger = logger if isinstance(logger, type(loguru_logger)) else loguru_logger
         if logger is None:
             self.logger.remove()
+            self.logger.level("FTRACE", no=3, color="<blue>")
             self.logger.add(sys.stderr, level=log_level or "INFO")
 
         if auto_auth:
             self.authenticate()
 
     def __missing__(self, key):
         res = RecordSet(key, self, context=self._context)
@@ -111,15 +114,16 @@
     def with_context(self, **kw):
         self._context = self._context.copy(**kw)
         return self
 
 
     def log_request(self, recordset, *args, **kwargs):
         # Todo: add more infos about performance.
-        self.logger.trace(f"Executing {args[0]} on {recordset} with args: {args[1:]} / kwargs: {kwargs}")
+        self.logger.trace(f"Executing {args[0]} on {recordset}")
+        self.logger.log("FTRACE", f"└── with args: {args[1:]} / kwargs: {kwargs}")
         self.requests.append({
             'model': recordset._name,
             'method': args[0],
             'args': args[1:],
             'kwargs': kwargs
         })
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `otools-rpc-0.3.0/otools_rpc/external_api/recordset.py` & `otools-rpc-0.3.1/otools_rpc/external_api/recordset.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,26 +126,26 @@
 
         except Exception as e:
             if isinstance(e, xmlrpc.client.Fault) and 'cannot marshal' in str(e):
                 return None
             self.logger.error(f"Error while executing {self._name}.{method}():")
             self.logger.debug(f"args / kwargs:\n {args} \n {kw}")
             self.logger.error("Odoo API Response:\n" + str(e).replace('\\n', '\n'))
+            raise e
 
     # --------------------------------------------
     #                   ORM
     # --------------------------------------------
 
 
     def browse(self, ids: Union[int, list[int]]) -> "RecordSet":
         return self._recordset(ids)
 
-    def fields_get(self, attributes: list[str] = None):
-        attributes = attributes or ['string', 'help', 'type']
-        return self._execute('fields_get', attributes=attributes)
+    # def fields_get(self, attributes: list[str] = None):
+    #     return self._execute('fields_get', attributes=attributes)
 
     @model
     def check_object_reference(self, module, xml_id):
         # Extra safety check, don't delete (even if nobody should use it directly)
         if self._name != 'ir.model.data':
             return self['ir.model.data'].check_object_reference(module, xml_id)
         return self._execute('check_object_reference', module, xml_id)
@@ -177,27 +177,28 @@
         return self._recordset([r.get('id') for r in res])
 
     @model
     def search_count(self, domain: list[tuple]):
         return self._execute('search_count', self._format_domain(domain))
 
     @model
+    @cache('create')
     def create(self, vals_list: Union[dict, list[dict]]):
         vals_list = vals_list if isinstance(vals_list, list) else [vals_list]
         ids = self._execute('create', vals_list)
         return self._recordset(ids)
 
     def write(self, vals: dict):
         return self._execute('write', vals)
 
     @cache('delete')
     def unlink(self):
         res = self._execute('unlink')
-        if res:
-            self._env.delete_cached_records(self._name, self._ids)
+        # if res:
+        #     self._env.delete_cached_records(self._name, self._ids)
         return res
 
     def copy(self):
         res_id = self._execute('copy')
         return self._recordset(res_id)
```

### Comparing `otools-rpc-0.3.0/otools_rpc.egg-info/PKG-INFO` & `otools-rpc-0.3.1/otools_rpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otools-rpc
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tool to interact with Odoo's external API.
 Home-page: https://github.com/MrFaBemol/otools-rpc
 Author: Gautier Casabona
 Author-email: gcasabona.pro@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `otools-rpc-0.3.0/setup.py` & `otools-rpc-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="otools-rpc",
-    version="0.3.0",
+    version="0.3.1",
     description="A tool to interact with Odoo's external API.",
     packages=find_packages(exclude=["tests"]),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MrFaBemol/otools-rpc",
     author="Gautier Casabona",
     author_email="gcasabona.pro@gmail.com",
```

