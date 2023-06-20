# Comparing `tmp/scpkit-0.3.1.tar.gz` & `tmp/scpkit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scpkit-0.3.1.tar", last modified: Wed May 31 12:49:38 2023, max compression
+gzip compressed data, was "scpkit-0.3.2.tar", last modified: Tue Jun 20 16:41:26 2023, max compression
```

## Comparing `scpkit-0.3.1.tar` & `scpkit-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:38.043012 scpkit-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 12:49:24.000000 scpkit-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-31 12:49:38.043012 scpkit-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-31 12:49:24.000000 scpkit-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 12:49:24.000000 scpkit-0.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:38.039012 scpkit-0.3.1/scpkit/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:38.043012 scpkit-0.3.1/scpkit/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/src/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/src/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/src/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-31 12:49:24.000000 scpkit-0.3.1/scpkit/src/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:38.043012 scpkit-0.3.1/scpkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-31 12:49:38.000000 scpkit-0.3.1/scpkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-31 12:49:38.000000 scpkit-0.3.1/scpkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:49:38.000000 scpkit-0.3.1/scpkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-31 12:49:38.000000 scpkit-0.3.1/scpkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:49:37.000000 scpkit-0.3.1/scpkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 12:49:38.000000 scpkit-0.3.1/scpkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 12:49:38.000000 scpkit-0.3.1/scpkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-31 12:49:38.043012 scpkit-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:49:24.000000 scpkit-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:38.043012 scpkit-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-31 12:49:24.000000 scpkit-0.3.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:41:26.256280 scpkit-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 16:41:13.000000 scpkit-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-20 16:41:26.256280 scpkit-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-20 16:41:13.000000 scpkit-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 16:41:13.000000 scpkit-0.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:41:26.252280 scpkit-0.3.2/scpkit/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 16:41:13.000000 scpkit-0.3.2/scpkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-20 16:41:13.000000 scpkit-0.3.2/scpkit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:41:26.256280 scpkit-0.3.2/scpkit/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:41:13.000000 scpkit-0.3.2/scpkit/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-06-20 16:41:13.000000 scpkit-0.3.2/scpkit/src/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-20 16:41:13.000000 scpkit-0.3.2/scpkit/src/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-20 16:41:13.000000 scpkit-0.3.2/scpkit/src/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-20 16:41:13.000000 scpkit-0.3.2/scpkit/src/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:41:26.252280 scpkit-0.3.2/scpkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-20 16:41:26.000000 scpkit-0.3.2/scpkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 16:41:26.000000 scpkit-0.3.2/scpkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:41:26.000000 scpkit-0.3.2/scpkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 16:41:26.000000 scpkit-0.3.2/scpkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:41:26.000000 scpkit-0.3.2/scpkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 16:41:26.000000 scpkit-0.3.2/scpkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 16:41:26.000000 scpkit-0.3.2/scpkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-20 16:41:26.256280 scpkit-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:41:13.000000 scpkit-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:41:26.256280 scpkit-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-20 16:41:13.000000 scpkit-0.3.2/tests/test.py
```

### Comparing `scpkit-0.3.1/LICENSE` & `scpkit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scpkit-0.3.1/PKG-INFO` & `scpkit-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scpkit
-Version: 0.3.1
+Version: 0.3.2
 Summary: This package helps consolidate service control policies in AWS
 Home-page: https://www.aquia.us
 Author: Aquia
 Author-email: info@aquia.us
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/aquia-inc/scpkit/issues
 Project-URL: Source, https://github.com/aquia-inc/scpkit
```

### Comparing `scpkit-0.3.1/README.md` & `scpkit-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `scpkit-0.3.1/scpkit/main.py` & `scpkit-0.3.2/scpkit/main.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.3.1/scpkit/src/merge.py` & `scpkit-0.3.2/scpkit/src/merge.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.3.1/scpkit/src/model.py` & `scpkit-0.3.2/scpkit/src/model.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.3.1/scpkit/src/util.py` & `scpkit-0.3.2/scpkit/src/util.py`

 * *Files identical despite different names*

### Comparing `scpkit-0.3.1/scpkit/src/validate.py` & `scpkit-0.3.2/scpkit/src/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,12 +45,12 @@
             if(console):
                 print(f"    🚨 Error(s) in {scp.name}:")
                 for finding in scp.findings:
                     print(f"       {finding['issueCode']} - {finding['findingDetails']}")
             if outdir:
                 scp.write_findings_for_scp(outdir)
                 if(console):
-                    print("    ℹ️  More details check log file {outdir}/{scp.name}-findings.json")
+                    print(f"    ℹ️  More details check log file {outdir}/{scp.name}-findings.json")
             else:
                 print(scp.findings_json)
                 if(console):
                     print(f"   ℹ️  More details check log file ./{scp.name}-findings.json")
```

### Comparing `scpkit-0.3.1/scpkit.egg-info/PKG-INFO` & `scpkit-0.3.2/scpkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scpkit
-Version: 0.3.1
+Version: 0.3.2
 Summary: This package helps consolidate service control policies in AWS
 Home-page: https://www.aquia.us
 Author: Aquia
 Author-email: info@aquia.us
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/aquia-inc/scpkit/issues
 Project-URL: Source, https://github.com/aquia-inc/scpkit
```

### Comparing `scpkit-0.3.1/setup.cfg` & `scpkit-0.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 project_urls = 
 	Bug Tracker = https://github.com/aquia-inc/scpkit/issues
 	Source = https://github.com/aquia-inc/scpkit
 description = This package helps consolidate service control policies in AWS
 license = Apache License 2.0
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.3.1
+version = 0.3.2
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = file: requirements.txt
```

### Comparing `scpkit-0.3.1/tests/test.py` & `scpkit-0.3.2/tests/test.py`

 * *Files identical despite different names*

