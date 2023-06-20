# Comparing `tmp/neomaril-codex-1.0.3.tar.gz` & `tmp/neomaril-codex-1.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neomaril-codex-1.0.3.tar", last modified: Mon Jun 19 17:22:37 2023, max compression
+gzip compressed data, was "neomaril-codex-1.0.3a0.tar", last modified: Tue Jun 20 13:32:01 2023, max compression
```

## Comparing `neomaril-codex-1.0.3.tar` & `neomaril-codex-1.0.3a0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-19 17:22:37.341009 neomaril-codex-1.0.3/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1060 2023-03-06 17:55:16.000000 neomaril-codex-1.0.3/LICENSE.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       24 2023-03-13 13:54:26.000000 neomaril-codex-1.0.3/MANIFEST.in
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1018 2023-06-19 17:22:37.341009 neomaril-codex-1.0.3/PKG-INFO
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      618 2023-03-15 18:53:09.000000 neomaril-codex-1.0.3/README.md
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       59 2023-02-08 17:56:54.000000 neomaril-codex-1.0.3/requirements.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       79 2023-06-19 17:22:37.341009 neomaril-codex-1.0.3/setup.cfg
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1028 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3/setup.py
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-19 17:22:37.337009 neomaril-codex-1.0.3/src/
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-19 17:22:37.341009 neomaril-codex-1.0.3/src/neomaril_codex/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-02-08 17:56:54.000000 neomaril-codex-1.0.3/src/neomaril_codex/__init__.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12206 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3/src/neomaril_codex/base.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      755 2023-02-08 17:56:54.000000 neomaril-codex-1.0.3/src/neomaril_codex/exceptions.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     4487 2023-03-06 17:39:34.000000 neomaril-codex-1.0.3/src/neomaril_codex/logging.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    44245 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3/src/neomaril_codex/model.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12562 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3/src/neomaril_codex/pipeline.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    32065 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3/src/neomaril_codex/training.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      655 2023-03-07 18:36:14.000000 neomaril-codex-1.0.3/src/neomaril_codex/utils.py
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-19 17:22:37.341009 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1018 2023-06-19 17:22:37.000000 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      558 2023-06-19 17:22:37.000000 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-06-19 17:22:37.000000 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-02-07 14:57:39.000000 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/not-zip-safe
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       60 2023-06-19 17:22:37.000000 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/requires.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       15 2023-06-19 17:22:37.000000 neomaril-codex-1.0.3/src/neomaril_codex.egg-info/top_level.txt
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-20 13:32:01.729350 neomaril-codex-1.0.3a0/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1060 2023-03-06 17:55:16.000000 neomaril-codex-1.0.3a0/LICENSE.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       24 2023-03-13 13:54:26.000000 neomaril-codex-1.0.3a0/MANIFEST.in
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1021 2023-06-20 13:32:01.729350 neomaril-codex-1.0.3a0/PKG-INFO
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      618 2023-03-15 18:53:09.000000 neomaril-codex-1.0.3a0/README.md
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       59 2023-06-20 13:15:46.000000 neomaril-codex-1.0.3a0/requirements.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       79 2023-06-20 13:32:01.733350 neomaril-codex-1.0.3a0/setup.cfg
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1029 2023-06-20 13:31:42.000000 neomaril-codex-1.0.3a0/setup.py
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-20 13:32:01.725350 neomaril-codex-1.0.3a0/src/
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-20 13:32:01.729350 neomaril-codex-1.0.3a0/src/neomaril_codex/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-02-08 17:56:54.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/__init__.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12206 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/base.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      755 2023-02-08 17:56:54.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/exceptions.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     4487 2023-03-06 17:39:34.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/logging.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    44245 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/model.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12562 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/pipeline.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    32127 2023-06-20 13:15:32.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/training.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      655 2023-06-20 13:15:46.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/utils.py
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-20 13:32:01.729350 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1021 2023-06-20 13:32:01.000000 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      558 2023-06-20 13:32:01.000000 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-06-20 13:32:01.000000 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-06-20 13:32:01.000000 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/not-zip-safe
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       60 2023-06-20 13:32:01.000000 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/requires.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       15 2023-06-20 13:32:01.000000 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/top_level.txt
```

### Comparing `neomaril-codex-1.0.3/LICENSE.txt` & `neomaril-codex-1.0.3a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3/PKG-INFO` & `neomaril-codex-1.0.3a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: neomaril-codex
-Version: 1.0.3
+Version: 1.0.3a0
 Summary: Python tools for interact with Neomaril
 Home-page: https://datarisk-io.github.io/mlops-neomaril-codex/
-Download-URL: https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v1.0.3.tar.gz
+Download-URL: https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v1.0.3a.tar.gz
 Author: Datarisk
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Neomaril Codex
```

### Comparing `neomaril-codex-1.0.3/README.md` & `neomaril-codex-1.0.3a0/README.md`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3/setup.py` & `neomaril-codex-1.0.3a0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os.path import join
 
 from setuptools import setup, find_packages
 
 MODULE_NAME = 'neomaril-codex'
 MODULE_NAME_IMPORT = 'neomaril_codex'
 REPO_NAME = 'mlops-neomaril-codex'
-MODULE_VERSION='1.0.3'
+MODULE_VERSION='1.0.3a'
 
 def requirements_from_pip(filename='requirements.txt'):
     with open(filename, 'r') as pip:
         return [l.strip() for l in pip if not l.startswith('#') and l.strip()]
 
 
 setup(name=MODULE_NAME,
```

### Comparing `neomaril-codex-1.0.3/src/neomaril_codex/base.py` & `neomaril-codex-1.0.3a0/src/neomaril_codex/base.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3/src/neomaril_codex/exceptions.py` & `neomaril-codex-1.0.3a0/src/neomaril_codex/exceptions.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3/src/neomaril_codex/logging.py` & `neomaril-codex-1.0.3a0/src/neomaril_codex/logging.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3/src/neomaril_codex/model.py` & `neomaril-codex-1.0.3a0/src/neomaril_codex/model.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3/src/neomaril_codex/pipeline.py` & `neomaril-codex-1.0.3a0/src/neomaril_codex/pipeline.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3/src/neomaril_codex/training.py` & `neomaril-codex-1.0.3a0/src/neomaril_codex/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,18 @@
         self.status = result['Status']
         self.execution_data['ExecutionState'] = result['Status']
         if self.status == 'Succeeded':
             url = f"{self.base_url}/training/describe/{self.group}/{self.training_id}/{self.exec_id}"
             response = requests.get(url, headers={'Authorization': 'Bearer ' + self.__credentials})
             self.execution_data = response.json()['Description']
             self.run_data = self.execution_data['RunData']
-            del self.run_data['tags']
+            try:
+                del self.run_data['tags']
+            except:
+                pass
         return result
 
     def __host_model(self, operation:str, model_id:str) -> None:
         """
         Builds the model execution environment
 
         Arguments
```

### Comparing `neomaril-codex-1.0.3/src/neomaril_codex/utils.py` & `neomaril-codex-1.0.3a0/src/neomaril_codex/utils.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3/src/neomaril_codex.egg-info/PKG-INFO` & `neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: neomaril-codex
-Version: 1.0.3
+Version: 1.0.3a0
 Summary: Python tools for interact with Neomaril
 Home-page: https://datarisk-io.github.io/mlops-neomaril-codex/
-Download-URL: https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v1.0.3.tar.gz
+Download-URL: https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v1.0.3a.tar.gz
 Author: Datarisk
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Neomaril Codex
```

### Comparing `neomaril-codex-1.0.3/src/neomaril_codex.egg-info/SOURCES.txt` & `neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

