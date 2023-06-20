# Comparing `tmp/eligibility_api-2023.1.1.tar.gz` & `tmp/eligibility_api-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eligibility_api-2023.1.1.tar", last modified: Thu Jan  5 21:39:10 2023, max compression
+gzip compressed data, was "eligibility_api-2023.6.1.tar", last modified: Tue Jun 20 20:52:53 2023, max compression
```

## Comparing `eligibility_api-2023.1.1.tar` & `eligibility_api-2023.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 calitp    (1000) calitp    (1000)        0 2023-01-05 21:39:10.483052 eligibility_api-2023.1.1/
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)    11357 2021-11-18 00:28:09.000000 eligibility_api-2023.1.1/LICENSE
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)      801 2023-01-05 21:39:10.485555 eligibility_api-2023.1.1/PKG-INFO
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)      277 2021-11-18 00:28:13.000000 eligibility_api-2023.1.1/README.md
-drwxrwxrwx   0 calitp    (1000) calitp    (1000)        0 2023-01-05 21:39:10.388858 eligibility_api-2023.1.1/eligibility_api/
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)        0 2022-05-20 18:47:52.000000 eligibility_api-2023.1.1/eligibility_api/__init__.py
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)     3570 2022-06-06 17:46:07.000000 eligibility_api-2023.1.1/eligibility_api/client.py
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)     2221 2022-12-14 02:58:46.000000 eligibility_api-2023.1.1/eligibility_api/server.py
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)     4262 2022-06-06 17:46:07.000000 eligibility_api-2023.1.1/eligibility_api/tokens.py
-drwxrwxrwx   0 calitp    (1000) calitp    (1000)        0 2023-01-05 21:39:10.456441 eligibility_api-2023.1.1/eligibility_api.egg-info/
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)      801 2023-01-05 21:39:10.000000 eligibility_api-2023.1.1/eligibility_api.egg-info/PKG-INFO
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)      381 2023-01-05 21:39:10.000000 eligibility_api-2023.1.1/eligibility_api.egg-info/SOURCES.txt
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)        1 2023-01-05 21:39:10.000000 eligibility_api-2023.1.1/eligibility_api.egg-info/dependency_links.txt
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)       31 2023-01-05 21:39:10.000000 eligibility_api-2023.1.1/eligibility_api.egg-info/requires.txt
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)       22 2023-01-05 21:39:10.000000 eligibility_api-2023.1.1/eligibility_api.egg-info/top_level.txt
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)      182 2023-01-05 21:18:30.000000 eligibility_api-2023.1.1/pyproject.toml
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)      666 2023-01-05 21:39:10.490552 eligibility_api-2023.1.1/setup.cfg
-drwxrwxrwx   0 calitp    (1000) calitp    (1000)        0 2023-01-05 21:39:10.476053 eligibility_api-2023.1.1/tests/
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)        0 2022-06-06 17:46:07.000000 eligibility_api-2023.1.1/tests/__init__.py
--rwxr-xr-x   0 calitp    (1000) calitp    (1000)     7718 2022-06-06 17:46:07.000000 eligibility_api-2023.1.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:52:53.827357 eligibility_api-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 20:52:30.000000 eligibility_api-2023.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-20 20:52:53.827357 eligibility_api-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-20 20:52:30.000000 eligibility_api-2023.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:52:53.823357 eligibility_api-2023.6.1/eligibility_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 20:52:30.000000 eligibility_api-2023.6.1/eligibility_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-20 20:52:30.000000 eligibility_api-2023.6.1/eligibility_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-20 20:52:30.000000 eligibility_api-2023.6.1/eligibility_api/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-20 20:52:30.000000 eligibility_api-2023.6.1/eligibility_api/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:52:53.823357 eligibility_api-2023.6.1/eligibility_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-20 20:52:53.000000 eligibility_api-2023.6.1/eligibility_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-20 20:52:53.000000 eligibility_api-2023.6.1/eligibility_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:52:53.000000 eligibility_api-2023.6.1/eligibility_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 20:52:53.000000 eligibility_api-2023.6.1/eligibility_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 20:52:53.000000 eligibility_api-2023.6.1/eligibility_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-20 20:52:30.000000 eligibility_api-2023.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-20 20:52:53.827357 eligibility_api-2023.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:52:53.827357 eligibility_api-2023.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 20:52:30.000000 eligibility_api-2023.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-06-20 20:52:30.000000 eligibility_api-2023.6.1/tests/test_client.py
```

### Comparing `eligibility_api-2023.1.1/LICENSE` & `eligibility_api-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eligibility_api-2023.1.1/PKG-INFO` & `eligibility_api-2023.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eligibility_api
-Version: 2023.1.1
+Version: 2023.6.1
 Summary: Data exchange to verify eligibility for transit benefits
 Home-page: https://github.com/cal-itp/eligibility-api
 License: 'Apache 2.0'
 Project-URL: Bug Tracker, https://github.com/cal-itp/eligibility-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `eligibility_api-2023.1.1/eligibility_api/client.py` & `eligibility_api-2023.6.1/eligibility_api/client.py`

 * *Files identical despite different names*

### Comparing `eligibility_api-2023.1.1/eligibility_api/server.py` & `eligibility_api-2023.6.1/eligibility_api/server.py`

 * *Files identical despite different names*

### Comparing `eligibility_api-2023.1.1/eligibility_api/tokens.py` & `eligibility_api-2023.6.1/eligibility_api/tokens.py`

 * *Files identical despite different names*

### Comparing `eligibility_api-2023.1.1/eligibility_api.egg-info/PKG-INFO` & `eligibility_api-2023.6.1/eligibility_api.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eligibility-api
-Version: 2023.1.1
+Version: 2023.6.1
 Summary: Data exchange to verify eligibility for transit benefits
 Home-page: https://github.com/cal-itp/eligibility-api
 License: 'Apache 2.0'
 Project-URL: Bug Tracker, https://github.com/cal-itp/eligibility-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `eligibility_api-2023.1.1/setup.cfg` & `eligibility_api-2023.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eligibility_api
-version = 2023.01.1
+version = 2023.06.1
 description = Data exchange to verify eligibility for transit benefits
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cal-itp/eligibility-api
 project_urls = 
 	Bug Tracker = https://github.com/cal-itp/eligibility-api/issues
 license = 'Apache 2.0'
```

### Comparing `eligibility_api-2023.1.1/tests/test_client.py` & `eligibility_api-2023.6.1/tests/test_client.py`

 * *Files identical despite different names*

