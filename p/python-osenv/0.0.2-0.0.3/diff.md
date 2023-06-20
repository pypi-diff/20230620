# Comparing `tmp/python_osenv-0.0.2.tar.gz` & `tmp/python_osenv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_osenv-0.0.2.tar", max compression
+gzip compressed data, was "python_osenv-0.0.3.tar", max compression
```

## Comparing `python_osenv-0.0.2.tar` & `python_osenv-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-01-25 13:04:40.809165 python_osenv-0.0.2/README.md
--rw-r--r--   0        0        0      704 2023-06-16 15:13:38.941468 python_osenv-0.0.2/osenv/__init__.py
--rw-r--r--   0        0        0      362 2023-06-16 15:12:49.303071 python_osenv-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 python_osenv-0.0.2/setup.py
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 python_osenv-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-01-25 13:04:40.809165 python_osenv-0.0.3/README.md
+-rw-r--r--   0        0        0     1030 2023-06-20 11:54:49.809737 python_osenv-0.0.3/osenv/__init__.py
+-rw-r--r--   0        0        0      362 2023-06-20 11:55:01.768988 python_osenv-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 python_osenv-0.0.3/setup.py
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 python_osenv-0.0.3/PKG-INFO
```

### Comparing `python_osenv-0.0.2/setup.py` & `python_osenv-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['python-dotenv==1.0.0']
 
 setup_kwargs = {
     'name': 'python-osenv',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'osenv',
     'long_description': '',
     'author': 'wayfaring-stranger',
     'author_email': 'zw6p226m@duck.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `python_osenv-0.0.2/PKG-INFO` & `python_osenv-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-osenv
-Version: 0.0.2
+Version: 0.0.3
 Summary: osenv
 License: MIT
 Author: wayfaring-stranger
 Author-email: zw6p226m@duck.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

