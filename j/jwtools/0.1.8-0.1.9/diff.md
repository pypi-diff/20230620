# Comparing `tmp/jwtools-0.1.8.tar.gz` & `tmp/jwtools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwtools-0.1.8.tar", last modified: Wed May 24 02:20:54 2023, max compression
+gzip compressed data, was "jwtools-0.1.9.tar", last modified: Fri May 26 02:36:31 2023, max compression
```

## Comparing `jwtools-0.1.8.tar` & `jwtools-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 02:20:54.338264 jwtools-0.1.8/
--rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 jwtools-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1452 2023-05-24 02:20:54.338264 jwtools-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      899 2023-05-24 02:20:37.000000 jwtools-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 02:20:54.324502 jwtools-0.1.8/jwtools/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.8/jwtools/__init__.py
--rw-rw-rw-   0        0        0      142 2023-05-19 10:02:42.000000 jwtools-0.1.8/jwtools/dt.py
--rw-rw-rw-   0        0        0     2012 2023-05-24 02:13:13.000000 jwtools-0.1.8/jwtools/func.py
--rw-rw-rw-   0        0        0     1428 2023-05-24 02:12:16.000000 jwtools-0.1.8/jwtools/io_util.py
-drwxrwxrwx   0        0        0        0 2023-05-24 02:20:54.329498 jwtools-0.1.8/jwtools/tests/
--rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.8/jwtools/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 02:20:54.331494 jwtools-0.1.8/jwtools/tests/feature/
--rw-rw-rw-   0        0        0        0 2023-05-23 04:43:26.000000 jwtools-0.1.8/jwtools/tests/feature/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 02:20:54.334254 jwtools-0.1.8/jwtools/tests/script/
--rw-rw-rw-   0        0        0        0 2023-05-23 06:26:31.000000 jwtools-0.1.8/jwtools/tests/script/__init__.py
--rw-rw-rw-   0        0        0      209 2023-05-18 03:36:21.000000 jwtools-0.1.8/jwtools/tests/script/test1.py
--rw-rw-rw-   0        0        0      747 2023-05-23 04:42:50.000000 jwtools-0.1.8/jwtools/tests/script/test2.py
--rw-rw-rw-   0        0        0      183 2023-05-22 03:25:04.000000 jwtools-0.1.8/jwtools/tests/test_base.py
-drwxrwxrwx   0        0        0        0 2023-05-24 02:20:54.337257 jwtools-0.1.8/jwtools/tests/unit/
--rw-rw-rw-   0        0        0        0 2023-05-23 04:43:33.000000 jwtools-0.1.8/jwtools/tests/unit/__init__.py
--rw-rw-rw-   0        0        0     1480 2023-05-23 06:24:25.000000 jwtools-0.1.8/jwtools/tests/unit/func_test.py
--rw-rw-rw-   0        0        0      747 2023-05-24 02:14:16.000000 jwtools-0.1.8/jwtools/tests/unit/io_test.py
-drwxrwxrwx   0        0        0        0 2023-05-24 02:20:54.327498 jwtools-0.1.8/jwtools.egg-info/
--rw-rw-rw-   0        0        0     1452 2023-05-24 02:20:54.000000 jwtools-0.1.8/jwtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-05-24 02:20:54.000000 jwtools-0.1.8/jwtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 02:20:54.000000 jwtools-0.1.8/jwtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-24 02:20:54.000000 jwtools-0.1.8/jwtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 02:20:54.338264 jwtools-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-05-24 02:20:08.000000 jwtools-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:31.780742 jwtools-0.1.9/
+-rw-rw-rw-   0        0        0     1164 2023-05-17 09:27:51.000000 jwtools-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1452 2023-05-26 02:36:31.779419 jwtools-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      899 2023-05-24 02:20:37.000000 jwtools-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:31.757198 jwtools-0.1.9/jwtools/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.9/jwtools/__init__.py
+-rw-rw-rw-   0        0        0     1758 2023-05-26 02:35:25.000000 jwtools-0.1.9/jwtools/dt.py
+-rw-rw-rw-   0        0        0     2012 2023-05-24 02:13:13.000000 jwtools-0.1.9/jwtools/func.py
+-rw-rw-rw-   0        0        0     1428 2023-05-24 02:12:16.000000 jwtools-0.1.9/jwtools/io_util.py
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:31.764632 jwtools-0.1.9/jwtools/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-17 08:55:41.000000 jwtools-0.1.9/jwtools/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:31.767471 jwtools-0.1.9/jwtools/tests/feature/
+-rw-rw-rw-   0        0        0        0 2023-05-23 04:43:26.000000 jwtools-0.1.9/jwtools/tests/feature/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:31.771415 jwtools-0.1.9/jwtools/tests/script/
+-rw-rw-rw-   0        0        0        0 2023-05-23 06:26:31.000000 jwtools-0.1.9/jwtools/tests/script/__init__.py
+-rw-rw-rw-   0        0        0      209 2023-05-18 03:36:21.000000 jwtools-0.1.9/jwtools/tests/script/test1.py
+-rw-rw-rw-   0        0        0      747 2023-05-23 04:42:50.000000 jwtools-0.1.9/jwtools/tests/script/test2.py
+-rw-rw-rw-   0        0        0      183 2023-05-22 03:25:04.000000 jwtools-0.1.9/jwtools/tests/test_base.py
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:31.777414 jwtools-0.1.9/jwtools/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-05-23 04:43:33.000000 jwtools-0.1.9/jwtools/tests/unit/__init__.py
+-rw-rw-rw-   0        0        0     1107 2023-05-26 02:33:33.000000 jwtools-0.1.9/jwtools/tests/unit/dt_test.py
+-rw-rw-rw-   0        0        0     1480 2023-05-23 06:24:25.000000 jwtools-0.1.9/jwtools/tests/unit/func_test.py
+-rw-rw-rw-   0        0        0      747 2023-05-24 02:14:16.000000 jwtools-0.1.9/jwtools/tests/unit/io_test.py
+drwxrwxrwx   0        0        0        0 2023-05-26 02:36:31.762634 jwtools-0.1.9/jwtools.egg-info/
+-rw-rw-rw-   0        0        0     1452 2023-05-26 02:36:31.000000 jwtools-0.1.9/jwtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2023-05-26 02:36:31.000000 jwtools-0.1.9/jwtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 02:36:31.000000 jwtools-0.1.9/jwtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 02:36:31.000000 jwtools-0.1.9/jwtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 02:36:31.780742 jwtools-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-05-26 02:36:15.000000 jwtools-0.1.9/setup.py
```

### Comparing `jwtools-0.1.8/LICENSE` & `jwtools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.8/PKG-INFO` & `jwtools-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwtools
-Version: 0.1.8
+Version: 0.1.9
 Summary: It is a micro-toolbox that includes various common operations and will continue to be improved in the future.
 Home-page: https://github.com/jinghewang/python-jwtools.git
 Author: jinghewang
 Author-email: jinghewang@163.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jwtools-0.1.8/README.md` & `jwtools-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.8/jwtools/func.py` & `jwtools-0.1.9/jwtools/func.py`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.8/jwtools/io_util.py` & `jwtools-0.1.9/jwtools/io_util.py`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.8/jwtools/tests/script/test2.py` & `jwtools-0.1.9/jwtools/tests/script/test2.py`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.8/jwtools/tests/unit/func_test.py` & `jwtools-0.1.9/jwtools/tests/unit/func_test.py`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.8/jwtools/tests/unit/io_test.py` & `jwtools-0.1.9/jwtools/tests/unit/io_test.py`

 * *Files identical despite different names*

### Comparing `jwtools-0.1.8/jwtools.egg-info/PKG-INFO` & `jwtools-0.1.9/jwtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwtools
-Version: 0.1.8
+Version: 0.1.9
 Summary: It is a micro-toolbox that includes various common operations and will continue to be improved in the future.
 Home-page: https://github.com/jinghewang/python-jwtools.git
 Author: jinghewang
 Author-email: jinghewang@163.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jwtools-0.1.8/setup.py` & `jwtools-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jwtools',
-    version='0.1.8',
+    version='0.1.9',
     description="It is a micro-toolbox that includes various common operations and will continue to be improved in the future.",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     author='jinghewang',
     author_email='jinghewang@163.com',
     license='MIT License',
```

