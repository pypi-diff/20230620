# Comparing `tmp/openshift-python-utilities-4.14.1.tar.gz` & `tmp/openshift-python-utilities-4.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift-python-utilities-4.14.1.tar", last modified: Tue Jun 13 06:57:44 2023, max compression
+gzip compressed data, was "openshift-python-utilities-4.14.2.tar", last modified: Tue Jun 20 09:56:51 2023, max compression
```

## Comparing `openshift-python-utilities-4.14.1.tar` & `openshift-python-utilities-4.14.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:57:44.813129 openshift-python-utilities-4.14.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-13 06:57:40.000000 openshift-python-utilities-4.14.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1455 2023-06-13 06:57:44.812129 openshift-python-utilities-4.14.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      670 2023-06-13 06:57:40.000000 openshift-python-utilities-4.14.1/README.md
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-13 06:57:43.000000 openshift-python-utilities-4.14.1/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:57:44.812129 openshift-python-utilities-4.14.1/ocp_utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 06:57:40.000000 openshift-python-utilities-4.14.1/ocp_utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-06-13 06:57:40.000000 openshift-python-utilities-4.14.1/ocp_utilities/debugger.py
--rw-r--r--   0 root         (0) root         (0)      452 2023-06-13 06:57:40.000000 openshift-python-utilities-4.14.1/ocp_utilities/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13883 2023-06-13 06:57:40.000000 openshift-python-utilities-4.14.1/ocp_utilities/infra.py
--rw-r--r--   0 root         (0) root         (0)     6799 2023-06-13 06:57:40.000000 openshift-python-utilities-4.14.1/ocp_utilities/monitoring.py
--rw-r--r--   0 root         (0) root         (0)     1877 2023-06-13 06:57:40.000000 openshift-python-utilities-4.14.1/ocp_utilities/must_gather.py
--rw-r--r--   0 root         (0) root         (0)    12216 2023-06-13 06:57:40.000000 openshift-python-utilities-4.14.1/ocp_utilities/operators.py
--rw-r--r--   0 root         (0) root         (0)     3104 2023-06-13 06:57:40.000000 openshift-python-utilities-4.14.1/ocp_utilities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:57:44.812129 openshift-python-utilities-4.14.1/openshift_python_utilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1455 2023-06-13 06:57:44.000000 openshift-python-utilities-4.14.1/openshift_python_utilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-13 06:57:44.000000 openshift-python-utilities-4.14.1/openshift_python_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 06:57:44.000000 openshift-python-utilities-4.14.1/openshift_python_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-06-13 06:57:44.000000 openshift-python-utilities-4.14.1/openshift_python_utilities.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 06:57:44.000000 openshift-python-utilities-4.14.1/openshift_python_utilities.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1494 2023-06-13 06:57:40.000000 openshift-python-utilities-4.14.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 06:57:44.813129 openshift-python-utilities-4.14.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:51.696307 openshift-python-utilities-4.14.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-06-20 09:56:51.695307 openshift-python-utilities-4.14.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      670 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/README.md
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-20 09:56:50.000000 openshift-python-utilities-4.14.2/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:51.695307 openshift-python-utilities-4.14.2/ocp_utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      517 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/debugger.py
+-rw-r--r--   0 root         (0) root         (0)      452 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13883 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/infra.py
+-rw-r--r--   0 root         (0) root         (0)     6799 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/must_gather.py
+-rw-r--r--   0 root         (0) root         (0)    12232 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/operators.py
+-rw-r--r--   0 root         (0) root         (0)     3104 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:51.695307 openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-06-20 09:56:51.000000 openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-20 09:56:51.000000 openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 09:56:51.000000 openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-06-20 09:56:51.000000 openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-20 09:56:51.000000 openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 09:56:51.696307 openshift-python-utilities-4.14.2/setup.cfg
```

### Comparing `openshift-python-utilities-4.14.1/LICENSE` & `openshift-python-utilities-4.14.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.1/PKG-INFO` & `openshift-python-utilities-4.14.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-python-utilities
-Version: 4.14.1
+Version: 4.14.2
 Summary: A utilities repository for https://github.com/RedHatQE/openshift-python-wrapper
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-python-utilities
 Project-URL: Download, https://pypi.org/project/openshift-python-utilities/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/openshift-python-utilities/issues
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-python-utilities/blob/main/README.md
 Keywords: Openshift
```

### Comparing `openshift-python-utilities-4.14.1/README.md` & `openshift-python-utilities-4.14.2/README.md`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.1/ocp_utilities/debugger.py` & `openshift-python-utilities-4.14.2/ocp_utilities/debugger.py`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.1/ocp_utilities/infra.py` & `openshift-python-utilities-4.14.2/ocp_utilities/infra.py`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.1/ocp_utilities/monitoring.py` & `openshift-python-utilities-4.14.2/ocp_utilities/monitoring.py`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.1/ocp_utilities/must_gather.py` & `openshift-python-utilities-4.14.2/ocp_utilities/must_gather.py`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.1/ocp_utilities/operators.py` & `openshift-python-utilities-4.14.2/ocp_utilities/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     operator_market_namespace = "openshift-marketplace"
 
     if iib_index_image:
         if not brew_token:
             raise ValueError("brew_token must be provided for iib_index_image")
 
         catalog_source = create_catalog_source_for_iib_install(
-            name="iib-catalog",
+            name=f"iib-catalog-{name.lower()}",
             iib_index_image=iib_index_image,
             brew_token=brew_token,
             operator_market_namespace=operator_market_namespace,
         )
     else:
         if not source:
             raise ValueError("source must be provided if not using iib_index_image")
```

### Comparing `openshift-python-utilities-4.14.1/ocp_utilities/utils.py` & `openshift-python-utilities-4.14.2/ocp_utilities/utils.py`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.1/openshift_python_utilities.egg-info/PKG-INFO` & `openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-python-utilities
-Version: 4.14.1
+Version: 4.14.2
 Summary: A utilities repository for https://github.com/RedHatQE/openshift-python-wrapper
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-python-utilities
 Project-URL: Download, https://pypi.org/project/openshift-python-utilities/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/openshift-python-utilities/issues
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-python-utilities/blob/main/README.md
 Keywords: Openshift
```

### Comparing `openshift-python-utilities-4.14.1/pyproject.toml` & `openshift-python-utilities-4.14.2/pyproject.toml`

 * *Files identical despite different names*

