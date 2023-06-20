# Comparing `tmp/fx_lib-0.4.0.tar.gz` & `tmp/fx_lib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fx_lib-0.4.0.tar", last modified: Sun Apr 25 12:39:17 2021, max compression
+gzip compressed data, was "fx_lib-0.5.0.tar", last modified: Tue Jun 20 16:16:16 2023, max compression
```

## Comparing `fx_lib-0.4.0.tar` & `fx_lib-0.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-25 12:39:17.261713 fx_lib-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3515 2021-04-25 12:39:13.000000 fx_lib-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-04-25 12:39:13.000000 fx_lib-0.4.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-04-25 12:39:13.000000 fx_lib-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      242 2021-04-25 12:39:13.000000 fx_lib-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-04-25 12:39:17.261713 fx_lib-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      845 2021-04-25 12:39:13.000000 fx_lib-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-25 12:39:17.257713 fx_lib-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      607 2021-04-25 12:39:13.000000 fx_lib-0.4.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (121)     4784 2021-04-25 12:39:13.000000 fx_lib-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-04-25 12:39:13.000000 fx_lib-0.4.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-04-25 12:39:13.000000 fx_lib-0.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      292 2021-04-25 12:39:13.000000 fx_lib-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-04-25 12:39:13.000000 fx_lib-0.4.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      768 2021-04-25 12:39:13.000000 fx_lib-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-04-25 12:39:13.000000 fx_lib-0.4.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-04-25 12:39:13.000000 fx_lib-0.4.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-25 12:39:17.261713 fx_lib-0.4.0/fx_lib/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-04-25 12:39:13.000000 fx_lib-0.4.0/fx_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2559 2021-04-25 12:39:13.000000 fx_lib-0.4.0/fx_lib/datetime_ext.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2021-04-25 12:39:13.000000 fx_lib-0.4.0/fx_lib/func.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-04-25 12:39:13.000000 fx_lib-0.4.0/fx_lib/fx_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-04-25 12:39:13.000000 fx_lib-0.4.0/fx_lib/list_ext.py
--rw-r--r--   0 runner    (1001) docker     (121)     5046 2021-04-25 12:39:13.000000 fx_lib-0.4.0/fx_lib/log.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-04-25 12:39:13.000000 fx_lib-0.4.0/fx_lib/math.py
--rw-r--r--   0 runner    (1001) docker     (121)      311 2021-04-25 12:39:13.000000 fx_lib-0.4.0/fx_lib/str_ext.py
--rw-r--r--   0 runner    (1001) docker     (121)     2216 2021-04-25 12:39:13.000000 fx_lib-0.4.0/fx_lib/zoho_email.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-25 12:39:17.261713 fx_lib-0.4.0/fx_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-04-25 12:39:17.000000 fx_lib-0.4.0/fx_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      629 2021-04-25 12:39:17.000000 fx_lib-0.4.0/fx_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-25 12:39:17.000000 fx_lib-0.4.0/fx_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-25 12:39:17.000000 fx_lib-0.4.0/fx_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-04-25 12:39:17.000000 fx_lib-0.4.0/fx_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-25 12:39:17.000000 fx_lib-0.4.0/fx_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      389 2021-04-25 12:39:17.261713 fx_lib-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2021-04-25 12:39:13.000000 fx_lib-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-25 12:39:17.261713 fx_lib-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-04-25 12:39:13.000000 fx_lib-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2021-04-25 12:39:13.000000 fx_lib-0.4.0/tests/test_fx_lib.py
--rw-r--r--   0 runner    (1001) docker     (121)      518 2021-04-25 12:39:13.000000 fx_lib-0.4.0/tests/test_zoho_email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:16:16.468576 fx_lib-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-20 16:16:09.000000 fx_lib-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 16:16:09.000000 fx_lib-0.5.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 16:16:09.000000 fx_lib-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-20 16:16:09.000000 fx_lib-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-20 16:16:16.468576 fx_lib-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-20 16:16:09.000000 fx_lib-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:16:16.464576 fx_lib-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 16:16:09.000000 fx_lib-0.5.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4784 2023-06-20 16:16:09.000000 fx_lib-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 16:16:09.000000 fx_lib-0.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 16:16:09.000000 fx_lib-0.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-20 16:16:09.000000 fx_lib-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-20 16:16:09.000000 fx_lib-0.5.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-20 16:16:09.000000 fx_lib-0.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 16:16:09.000000 fx_lib-0.5.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 16:16:09.000000 fx_lib-0.5.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:16:16.468576 fx_lib-0.5.0/fx_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 16:16:09.000000 fx_lib-0.5.0/fx_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-20 16:16:09.000000 fx_lib-0.5.0/fx_lib/datetime_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-20 16:16:09.000000 fx_lib-0.5.0/fx_lib/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 16:16:09.000000 fx_lib-0.5.0/fx_lib/fx_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-20 16:16:09.000000 fx_lib-0.5.0/fx_lib/list_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-20 16:16:09.000000 fx_lib-0.5.0/fx_lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 16:16:09.000000 fx_lib-0.5.0/fx_lib/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-20 16:16:09.000000 fx_lib-0.5.0/fx_lib/str_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-20 16:16:09.000000 fx_lib-0.5.0/fx_lib/zoho_email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:16:16.468576 fx_lib-0.5.0/fx_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-20 16:16:16.000000 fx_lib-0.5.0/fx_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 16:16:16.000000 fx_lib-0.5.0/fx_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:16:16.000000 fx_lib-0.5.0/fx_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:16:16.000000 fx_lib-0.5.0/fx_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 16:16:16.000000 fx_lib-0.5.0/fx_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 16:16:16.000000 fx_lib-0.5.0/fx_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-20 16:16:16.468576 fx_lib-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-20 16:16:09.000000 fx_lib-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:16:16.468576 fx_lib-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-20 16:16:09.000000 fx_lib-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-20 16:16:09.000000 fx_lib-0.5.0/tests/test_fx_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-20 16:16:09.000000 fx_lib-0.5.0/tests/test_zoho_email.py
```

### Comparing `fx_lib-0.4.0/CONTRIBUTING.rst` & `fx_lib-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fx_lib-0.4.0/LICENSE` & `fx_lib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fx_lib-0.4.0/README.rst` & `fx_lib-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `fx_lib-0.4.0/docs/Makefile` & `fx_lib-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fx_lib-0.4.0/docs/conf.py` & `fx_lib-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fx_lib-0.4.0/docs/installation.rst` & `fx_lib-0.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `fx_lib-0.4.0/docs/make.bat` & `fx_lib-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fx_lib-0.4.0/fx_lib/datetime_ext.py` & `fx_lib-0.5.0/fx_lib/datetime_ext.py`

 * *Files identical despite different names*

### Comparing `fx_lib-0.4.0/fx_lib/func.py` & `fx_lib-0.5.0/fx_lib/func.py`

 * *Files identical despite different names*

### Comparing `fx_lib-0.4.0/fx_lib/log.py` & `fx_lib-0.5.0/fx_lib/log.py`

 * *Files identical despite different names*

### Comparing `fx_lib-0.4.0/fx_lib/zoho_email.py` & `fx_lib-0.5.0/fx_lib/zoho_email.py`

 * *Files identical despite different names*

### Comparing `fx_lib-0.4.0/fx_lib.egg-info/SOURCES.txt` & `fx_lib-0.5.0/fx_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fx_lib-0.4.0/setup.py` & `fx_lib-0.5.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,23 +22,26 @@
     author_email='frank@frankxu.me',
     classifiers=[
         "License :: OSI Approved :: MIT License",
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        "Operating System :: OS Independent",
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     description="FX's personal common lib",
     install_requires=requirements,
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='fx_lib',
     name='fx_lib',
     packages=find_packages(include=['fx_lib']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/frankyxhl/py_fx_lib',
-    version='0.4.0',
+    version='0.5.0',
     zip_safe=False,
 )
```

### Comparing `fx_lib-0.4.0/tests/test_zoho_email.py` & `fx_lib-0.5.0/tests/test_zoho_email.py`

 * *Files identical despite different names*

