# Comparing `tmp/classutils-1.8.0.tar.gz` & `tmp/classutils-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/classutils-1.8.0.tar", last modified: Tue May  1 15:46:02 2018, max compression
+gzip compressed data, was "dist/classutils-1.9.0.tar", last modified: Thu May  3 15:44:27 2018, max compression
```

## Comparing `classutils-1.8.0.tar` & `classutils-1.9.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-01 15:46:02.000000 classutils-1.8.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-01 15:46:02.000000 classutils-1.8.0/classutils/
--rw-rw-rw-   0 root         (0) root         (0)      977 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/observer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-01 15:46:02.000000 classutils-1.8.0/classutils/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      875 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/unittests/test_json_api_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     4840 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/unittests/test_json_api_class_creator.py
--rw-rw-rw-   0 root         (0) root         (0)     3016 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/unittests/test_observer.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/unittests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-01 15:46:02.000000 classutils-1.8.0/classutils/unittests/class_augmentations/
--rw-rw-rw-   0 root         (0) root         (0)       92 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/unittests/class_augmentations/augment_example.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/unittests/class_augmentations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5078 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/unittests/test_in_class_result_cache.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/unittests/test_singleton.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-01 15:46:02.000000 classutils-1.8.0/classutils/api_support/
--rw-rw-rw-   0 root         (0) root         (0)       74 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/api_support/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     7135 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/api_support/properties.py
--rw-rw-rw-   0 root         (0) root         (0)    23483 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/api_support/json_api_class_creator.py
--rw-rw-rw-   0 root         (0) root         (0)     1189 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/api_support/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4551 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/api_support/request_response.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/singleton.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-01 15:46:02.000000 classutils-1.8.0/classutils/decorators/
--rw-rw-rw-   0 root         (0) root         (0)     5806 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/decorators/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/decorators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4998 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/decorators/in_class_result_caching.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/decorators/deprecation_warning.py
--rw-rw-rw-   0 root         (0) root         (0)     6523 2018-05-01 15:45:59.000000 classutils-1.8.0/classutils/thread_pool.py
--rw-rw-rw-   0 root         (0) root         (0)       76 2018-05-01 15:45:59.000000 classutils-1.8.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       93 2018-05-01 15:45:59.000000 classutils-1.8.0/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-01 15:46:02.000000 classutils-1.8.0/classutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      142 2018-05-01 15:46:02.000000 classutils-1.8.0/classutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1138 2018-05-01 15:46:02.000000 classutils-1.8.0/classutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2018-05-01 15:46:02.000000 classutils-1.8.0/classutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2018-05-01 15:46:02.000000 classutils-1.8.0/classutils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       20 2018-05-01 15:46:02.000000 classutils-1.8.0/classutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      891 2018-05-01 15:46:02.000000 classutils-1.8.0/classutils.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4038 2018-05-01 15:45:59.000000 classutils-1.8.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      136 2018-05-01 15:46:02.000000 classutils-1.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      891 2018-05-01 15:46:02.000000 classutils-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1066 2018-05-01 15:45:59.000000 classutils-1.8.0/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-03 15:44:27.000000 classutils-1.9.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-03 15:44:27.000000 classutils-1.9.0/classutils/
+-rw-rw-rw-   0 root         (0) root         (0)      977 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/observer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-03 15:44:27.000000 classutils-1.9.0/classutils/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      875 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/unittests/test_json_api_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4840 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/unittests/test_json_api_class_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3016 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/unittests/test_observer.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/unittests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-03 15:44:27.000000 classutils-1.9.0/classutils/unittests/class_augmentations/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/unittests/class_augmentations/augment_example.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/unittests/class_augmentations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5078 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/unittests/test_in_class_result_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/unittests/test_singleton.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-03 15:44:27.000000 classutils-1.9.0/classutils/api_support/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/api_support/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7135 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/api_support/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)    24677 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/api_support/json_api_class_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1189 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/api_support/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4551 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/api_support/request_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/singleton.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-03 15:44:27.000000 classutils-1.9.0/classutils/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)     5806 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/decorators/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/decorators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4998 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/decorators/in_class_result_caching.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/decorators/deprecation_warning.py
+-rw-rw-rw-   0 root         (0) root         (0)     6523 2018-05-03 15:44:25.000000 classutils-1.9.0/classutils/thread_pool.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2018-05-03 15:44:25.000000 classutils-1.9.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       93 2018-05-03 15:44:25.000000 classutils-1.9.0/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-05-03 15:44:27.000000 classutils-1.9.0/classutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      142 2018-05-03 15:44:27.000000 classutils-1.9.0/classutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1138 2018-05-03 15:44:27.000000 classutils-1.9.0/classutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2018-05-03 15:44:27.000000 classutils-1.9.0/classutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2018-05-03 15:44:27.000000 classutils-1.9.0/classutils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2018-05-03 15:44:27.000000 classutils-1.9.0/classutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      891 2018-05-03 15:44:27.000000 classutils-1.9.0/classutils.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2018-05-03 15:44:25.000000 classutils-1.9.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      136 2018-05-03 15:44:27.000000 classutils-1.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      891 2018-05-03 15:44:27.000000 classutils-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2018-05-03 15:44:25.000000 classutils-1.9.0/LICENSE.txt
```

### Comparing `classutils-1.8.0/classutils/profiling.py` & `classutils-1.9.0/classutils/profiling.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/observer.py` & `classutils-1.9.0/classutils/observer.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/unittests/test_json_api_helper.py` & `classutils-1.9.0/classutils/unittests/test_json_api_helper.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/unittests/test_json_api_class_creator.py` & `classutils-1.9.0/classutils/unittests/test_json_api_class_creator.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/unittests/test_observer.py` & `classutils-1.9.0/classutils/unittests/test_observer.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/unittests/test_in_class_result_cache.py` & `classutils-1.9.0/classutils/unittests/test_in_class_result_cache.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/unittests/test_singleton.py` & `classutils-1.9.0/classutils/unittests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/api_support/properties.py` & `classutils-1.9.0/classutils/api_support/properties.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/api_support/json_api_class_creator.py` & `classutils-1.9.0/classutils/api_support/json_api_class_creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import os
 import inspect
 import json
+import yaml
 import codecs
 import logging_helper
 from future.builtins import str
 from fdutil.path_tools import ensure_path_exists, path_in_site_or_user_packages
 logging = logging_helper.setup_logging()
 
 MODULE = u'module'  # TODO: Change this
@@ -550,14 +551,40 @@
                                              "col": {"mandatory":  false,
                                                      "properties": ["color", "colour"]},
 
                                              "border": {"mandatory": false,
                                                         "property": "border",
                                                         "default": 1}
                                              })]
+
+                        e.g. rectangle.yaml contains:
+                            ---
+                            - class_name: Rectangle
+                              key: rectangle
+                              property_name: rect
+                              attributes:
+                                w:
+                                  mandatory: true
+                                  properties:
+                                  - w
+                                  - width
+                                h:
+                                  mandatory: true
+                                  properties:
+                                  - h
+                                  - height
+                                col:
+                                  mandatory: false
+                                  properties:
+                                  - color
+                                  - colour
+                                border:
+                                  mandatory: false
+                                  property: border
+                                  default: 1
     :return: N/A
     """
 
     # Get the path to the calling folder
     frame = inspect.stack()[1]
     module_ = inspect.getmodule(frame[0])
     folder_path = os.path.dirname(module_.__file__)
@@ -566,13 +593,14 @@
 
     if path_in_site_or_user_packages(folder_path):
         logging.debug(u'Site or user package location has been detected. '
                       u'Not generating code for {api_definition_file}'
                       .format(api_definition_file=api_definition_file))
         return
 
+    loader = json.load if api_definition_file.endswith(u'.json') else yaml.load
     with open(api_definition_file) as f:
-        api = json.load(f)
+        api = loader(f)
 
     for class_params in api:
         JsonApiPropertiesClassCreator(source=api_definition_file,
                                       **class_params).write_source_code()
```

### Comparing `classutils-1.8.0/classutils/api_support/__init__.py` & `classutils-1.9.0/classutils/api_support/__init__.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/api_support/request_response.py` & `classutils-1.9.0/classutils/api_support/request_response.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/singleton.py` & `classutils-1.9.0/classutils/singleton.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/_metadata.py` & `classutils-1.9.0/classutils/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # encoding: utf-8
 
 # Variables for setup (these must be string only!)
 __module_name__ = u'classutils'
 __description__ = u'A collection of utilites to enhance Python classes.'
 
-__version__ = u'1.8.0'
+__version__ = u'1.9.0'
 
 __author__ = u'Hywel Thomas'
 __authorshort__ = u'HT'
 __authoremail__ = u'hywel.thomas@mac.com'
 
 __license__ = u'MIT'
```

### Comparing `classutils-1.8.0/classutils/decorators/profiling.py` & `classutils-1.9.0/classutils/decorators/profiling.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/decorators/in_class_result_caching.py` & `classutils-1.9.0/classutils/decorators/in_class_result_caching.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/decorators/deprecation_warning.py` & `classutils-1.9.0/classutils/decorators/deprecation_warning.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils/thread_pool.py` & `classutils-1.9.0/classutils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils.egg-info/SOURCES.txt` & `classutils-1.9.0/classutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/classutils.egg-info/PKG-INFO` & `classutils-1.9.0/classutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: classutils
-Version: 1.8.0
+Version: 1.9.0
 Summary: A collection of utilites to enhance Python classes.
 Home-page: https://bitbucket.org/daycoder/classutils.git
 Author: Hywel Thomas
 Author-email: hywel.thomas@mac.com
 License: MIT
-Download-URL: https://bitbucket.org/daycoder/classutils.git/get/1.8.0.tar
+Download-URL: https://bitbucket.org/daycoder/classutils.git/get/1.9.0.tar
 Description: 
         classutils
         ==========
         
         A collections of utilities for enhancing classes.
```

### Comparing `classutils-1.8.0/setup.py` & `classutils-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `classutils-1.8.0/PKG-INFO` & `classutils-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: classutils
-Version: 1.8.0
+Version: 1.9.0
 Summary: A collection of utilites to enhance Python classes.
 Home-page: https://bitbucket.org/daycoder/classutils.git
 Author: Hywel Thomas
 Author-email: hywel.thomas@mac.com
 License: MIT
-Download-URL: https://bitbucket.org/daycoder/classutils.git/get/1.8.0.tar
+Download-URL: https://bitbucket.org/daycoder/classutils.git/get/1.9.0.tar
 Description: 
         classutils
         ==========
         
         A collections of utilities for enhancing classes.
```

### Comparing `classutils-1.8.0/LICENSE.txt` & `classutils-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

