# Comparing `tmp/quickstart-vdk-0.2.903875796.dev11543.tar.gz` & `tmp/quickstart-vdk-0.2.905084255.dev11599.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.903875796.dev11543.tar", last modified: Mon Jun 19 04:23:04 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.905084255.dev11599.tar", last modified: Tue Jun 20 04:23:42 2023, max compression
```

## Comparing `quickstart-vdk-0.2.903875796.dev11543.tar` & `quickstart-vdk-0.2.905084255.dev11599.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 04:23:04.501013 quickstart-vdk-0.2.903875796.dev11543/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-19 04:23:04.497013 quickstart-vdk-0.2.903875796.dev11543/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-19 04:20:15.000000 quickstart-vdk-0.2.903875796.dev11543/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 04:23:04.497013 quickstart-vdk-0.2.903875796.dev11543/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-19 04:23:04.000000 quickstart-vdk-0.2.903875796.dev11543/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-19 04:23:04.000000 quickstart-vdk-0.2.903875796.dev11543/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 04:23:04.000000 quickstart-vdk-0.2.903875796.dev11543/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-19 04:23:04.000000 quickstart-vdk-0.2.903875796.dev11543/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-19 04:23:04.000000 quickstart-vdk-0.2.903875796.dev11543/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 04:23:04.501013 quickstart-vdk-0.2.903875796.dev11543/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-19 04:22:52.000000 quickstart-vdk-0.2.903875796.dev11543/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 04:23:04.497013 quickstart-vdk-0.2.903875796.dev11543/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-19 04:20:15.000000 quickstart-vdk-0.2.903875796.dev11543/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:23:42.304133 quickstart-vdk-0.2.905084255.dev11599/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-20 04:23:42.304133 quickstart-vdk-0.2.905084255.dev11599/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-20 04:20:40.000000 quickstart-vdk-0.2.905084255.dev11599/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:23:42.304133 quickstart-vdk-0.2.905084255.dev11599/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-20 04:23:42.000000 quickstart-vdk-0.2.905084255.dev11599/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-20 04:23:42.000000 quickstart-vdk-0.2.905084255.dev11599/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 04:23:42.000000 quickstart-vdk-0.2.905084255.dev11599/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 04:23:42.000000 quickstart-vdk-0.2.905084255.dev11599/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-20 04:23:42.000000 quickstart-vdk-0.2.905084255.dev11599/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 04:23:42.304133 quickstart-vdk-0.2.905084255.dev11599/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-20 04:23:30.000000 quickstart-vdk-0.2.905084255.dev11599/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 04:23:42.304133 quickstart-vdk-0.2.905084255.dev11599/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-20 04:20:40.000000 quickstart-vdk-0.2.905084255.dev11599/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.903875796.dev11543/PKG-INFO` & `quickstart-vdk-0.2.905084255.dev11599/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.903875796.dev11543
+Version: 0.2.905084255.dev11599
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.903875796.dev11543/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.905084255.dev11599/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.903875796.dev11543
+Version: 0.2.905084255.dev11599
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.903875796.dev11543/setup.py` & `quickstart-vdk-0.2.905084255.dev11599/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.903875796.dev11543"
+__version__ = "0.2.905084255.dev11599"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

