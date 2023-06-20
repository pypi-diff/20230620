# Comparing `tmp/openshield-0.1.0.tar.gz` & `tmp/openshield-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshield-0.1.0.tar", last modified: Sun Apr 23 16:08:55 2023, max compression
+gzip compressed data, was "openshield-0.1.1.tar", last modified: Tue Jun 20 03:35:13 2023, max compression
```

## Comparing `openshield-0.1.0.tar` & `openshield-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-04-23 16:08:55.720904 openshield-0.1.0/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1070 2023-04-19 14:30:59.000000 openshield-0.1.0/LICENSE
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1653 2023-04-23 16:08:55.712904 openshield-0.1.0/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1018 2023-04-23 16:06:37.000000 openshield-0.1.0/README.md
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-04-23 16:08:55.708904 openshield-0.1.0/openshield/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       22 2023-04-23 15:13:18.000000 openshield-0.1.0/openshield/__init__.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1863 2023-04-23 16:07:39.000000 openshield-0.1.0/openshield/__main__.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3612 2023-04-23 16:07:47.000000 openshield-0.1.0/openshield/scanner.py
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-04-23 16:08:55.712904 openshield-0.1.0/openshield.egg-info/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1653 2023-04-23 16:08:55.000000 openshield-0.1.0/openshield.egg-info/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      300 2023-04-23 16:08:55.000000 openshield-0.1.0/openshield.egg-info/SOURCES.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-04-23 16:08:55.000000 openshield-0.1.0/openshield.egg-info/dependency_links.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       56 2023-04-23 16:08:55.000000 openshield-0.1.0/openshield.egg-info/entry_points.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       32 2023-04-23 16:08:55.000000 openshield-0.1.0/openshield.egg-info/requires.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       11 2023-04-23 16:08:55.000000 openshield-0.1.0/openshield.egg-info/top_level.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-04-23 16:08:55.720904 openshield-0.1.0/setup.cfg
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1063 2023-04-23 16:08:49.000000 openshield-0.1.0/setup.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-20 03:35:13.459065 openshield-0.1.1/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1070 2023-06-20 02:38:20.000000 openshield-0.1.1/LICENSE
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1653 2023-06-20 03:35:13.459065 openshield-0.1.1/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1018 2023-06-20 03:35:04.000000 openshield-0.1.1/README.md
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-20 03:35:13.439065 openshield-0.1.1/openshield/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       22 2023-06-20 03:24:56.000000 openshield-0.1.1/openshield/__init__.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1863 2023-06-20 02:38:20.000000 openshield-0.1.1/openshield/__main__.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     3547 2023-06-20 03:02:07.000000 openshield-0.1.1/openshield/scanner.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-20 03:35:13.455065 openshield-0.1.1/openshield.egg-info/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1653 2023-06-20 03:35:13.000000 openshield-0.1.1/openshield.egg-info/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      300 2023-06-20 03:35:13.000000 openshield-0.1.1/openshield.egg-info/SOURCES.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-06-20 03:35:13.000000 openshield-0.1.1/openshield.egg-info/dependency_links.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       56 2023-06-20 03:35:13.000000 openshield-0.1.1/openshield.egg-info/entry_points.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       32 2023-06-20 03:35:13.000000 openshield-0.1.1/openshield.egg-info/requires.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       11 2023-06-20 03:35:13.000000 openshield-0.1.1/openshield.egg-info/top_level.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-06-20 03:35:13.459065 openshield-0.1.1/setup.cfg
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1063 2023-06-20 03:28:02.000000 openshield-0.1.1/setup.py
```

### Comparing `openshield-0.1.0/LICENSE` & `openshield-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openshield-0.1.0/PKG-INFO` & `openshield-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshield
-Version: 0.1.0
+Version: 0.1.1
 Summary: OpenShield, a fast and easy-to-use CLI antivirus.
 Home-page: https://github.com/jaedsonpys/openshield
 Author: Jaedson Silva
 Author-email: jaedson.dev@proton.me
 License: MIT
 Keywords: antivirus,malware,scanner,cli
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openshield-0.1.0/README.md` & `openshield-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openshield-0.1.0/openshield/__main__.py` & `openshield-0.1.1/openshield/__main__.py`

 * *Files identical despite different names*

### Comparing `openshield-0.1.0/openshield/scanner.py` & `openshield-0.1.1/openshield/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,16 @@
         :return: Generator of hash list
         :rtype: typing.Generator
         :yield: MD5 Hash
         :rtype: Iterator[typing.Generator]
         """
 
         with open(HASH_DATA_PATH) as _file:
-            hash_txt = _file.read()
-            filelines = hash_txt.split('\n')
-
-        for _hash in filelines:
-            yield _hash
+            for _hash in _file:
+                yield _hash.rstrip('\n')
 
     def scan(self, files: list) -> typing.List[typing.Tuple[str]]:
         """Scan a file list.
 
         This method generate a file MD5 hash and checks
         if this hash is in malware database.
```

### Comparing `openshield-0.1.0/openshield.egg-info/PKG-INFO` & `openshield-0.1.1/openshield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshield
-Version: 0.1.0
+Version: 0.1.1
 Summary: OpenShield, a fast and easy-to-use CLI antivirus.
 Home-page: https://github.com/jaedsonpys/openshield
 Author: Jaedson Silva
 Author-email: jaedson.dev@proton.me
 License: MIT
 Keywords: antivirus,malware,scanner,cli
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openshield-0.1.0/setup.py` & `openshield-0.1.1/setup.py`

 * *Files identical despite different names*

