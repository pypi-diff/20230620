# Comparing `tmp/mystring-0.0.94.tar.gz` & `tmp/mystring-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystring-0.0.94.tar", last modified: Thu Jun 15 03:13:52 2023, max compression
+gzip compressed data, was "mystring-0.0.95.tar", last modified: Tue Jun 20 04:30:36 2023, max compression
```

## Comparing `mystring-0.0.94.tar` & `mystring-0.0.95.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:13:52.526021 mystring-0.0.94/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 03:13:47.000000 mystring-0.0.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-15 03:13:52.526021 mystring-0.0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 03:13:47.000000 mystring-0.0.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:13:52.526021 mystring-0.0.94/mystring/
--rw-r--r--   0 runner    (1001) docker     (123)    17766 2023-06-15 03:13:47.000000 mystring-0.0.94/mystring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:13:52.526021 mystring-0.0.94/mystring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-15 03:13:52.000000 mystring-0.0.94/mystring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-15 03:13:52.000000 mystring-0.0.94/mystring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:13:52.000000 mystring-0.0.94/mystring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 03:13:52.000000 mystring-0.0.94/mystring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 03:13:52.000000 mystring-0.0.94/mystring.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 03:13:52.526021 mystring-0.0.94/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-06-15 03:13:47.000000 mystring-0.0.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:30:36.077448 mystring-0.0.95/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 04:30:32.000000 mystring-0.0.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-20 04:30:36.077448 mystring-0.0.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 04:30:32.000000 mystring-0.0.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:30:36.077448 mystring-0.0.95/mystring/
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-06-20 04:30:32.000000 mystring-0.0.95/mystring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:30:36.077448 mystring-0.0.95/mystring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-20 04:30:36.000000 mystring-0.0.95/mystring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 04:30:36.000000 mystring-0.0.95/mystring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:30:36.000000 mystring-0.0.95/mystring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 04:30:36.000000 mystring-0.0.95/mystring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 04:30:36.000000 mystring-0.0.95/mystring.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 04:30:36.077448 mystring-0.0.95/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-06-20 04:30:32.000000 mystring-0.0.95/setup.py
```

### Comparing `mystring-0.0.94/LICENSE` & `mystring-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `mystring-0.0.94/mystring/__init__.py` & `mystring-0.0.95/mystring/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,23 +138,23 @@
 			else:
 				temp_list = string(joiner.join(output_list)).splitsies(splitter,joiner=joiner)
 				output_list = []
 				for temp_item in temp_list:
 					for temp_split_item in temp_item.split(joiner):
 						output_list.append(temp_split_item)
 
-		return output_list
+		return [mystring(x) for x in output_list]
 
 	def tohash(self, hash_type='sha512', encoding='utf-8'):
 		import hashlib
-		return getattr(hashlib, hash_type)(self.encode(encoding)).hexdigest()
+		return mystring(getattr(hashlib, hash_type)(self.encode(encoding)).hexdigest())
 
 	def tobase64(self, encoding='utf-8'):
 		import base64
-		return base64.b64encode(self.encode(encoding)).decode(encoding)
+		return mystring(base64.b64encode(self.encode(encoding)).decode(encoding))
 
 	@staticmethod
 	def frombase64(string, encoding='utf-8'):
 		import base64
 		return base64.b64decode(string.encode(encoding)).decode(encoding)
 
 import pandas as pd
```

### Comparing `mystring-0.0.94/setup.py` & `mystring-0.0.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.94"
+VERSION = "0.0.95"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

