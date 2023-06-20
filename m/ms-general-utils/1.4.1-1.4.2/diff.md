# Comparing `tmp/ms_general_utils-1.4.1.tar.gz` & `tmp/ms_general_utils-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_general_utils-1.4.1.tar", last modified: Fri May 19 16:20:00 2023, max compression
+gzip compressed data, was "ms_general_utils-1.4.2.tar", last modified: Tue Jun 20 09:51:53 2023, max compression
```

## Comparing `ms_general_utils-1.4.1.tar` & `ms_general_utils-1.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 16:20:00.447266 ms_general_utils-1.4.1/
--rw-rw-rw-   0        0        0     1073 2023-03-14 11:56:37.000000 ms_general_utils-1.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0      354 2023-05-19 16:20:00.441265 ms_general_utils-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-03-14 15:40:50.000000 ms_general_utils-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 16:20:00.243964 ms_general_utils-1.4.1/ms_general_utils.egg-info/
--rw-rw-rw-   0        0        0      354 2023-05-19 16:20:00.000000 ms_general_utils-1.4.1/ms_general_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-05-19 16:20:00.000000 ms_general_utils-1.4.1/ms_general_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 16:20:00.000000 ms_general_utils-1.4.1/ms_general_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 16:20:00.000000 ms_general_utils-1.4.1/ms_general_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-19 16:20:00.430736 ms_general_utils-1.4.1/ms_utils/
--rw-rw-rw-   0        0        0      555 2023-03-27 15:14:21.000000 ms_general_utils-1.4.1/ms_utils/__init__.py
--rw-rw-rw-   0        0        0      386 2023-03-17 12:23:38.000000 ms_general_utils-1.4.1/ms_utils/abstract_model.py
--rw-rw-rw-   0        0        0     1034 2023-03-17 11:27:17.000000 ms_general_utils-1.4.1/ms_utils/binary_uuid.py
--rw-rw-rw-   0        0        0      695 2023-03-17 08:52:55.000000 ms_general_utils-1.4.1/ms_utils/func_date.py
--rw-rw-rw-   0        0        0     2570 2023-04-03 15:04:19.000000 ms_general_utils-1.4.1/ms_utils/generic_crud_class.py
--rw-rw-rw-   0        0        0      706 2023-03-17 08:52:56.000000 ms_general_utils-1.4.1/ms_utils/generic_pagination.py
--rw-rw-rw-   0        0        0     1527 2023-04-03 17:16:10.000000 ms_general_utils-1.4.1/ms_utils/model_utils.py
--rw-rw-rw-   0        0        0      341 2023-03-17 08:52:56.000000 ms_general_utils-1.4.1/ms_utils/prepare_json_response.py
--rw-rw-rw-   0        0        0      622 2023-05-19 16:18:44.000000 ms_general_utils-1.4.1/ms_utils/validation_utils.py
--rw-rw-rw-   0        0        0     4472 2023-05-19 16:16:18.000000 ms_general_utils-1.4.1/ms_utils/view_utils.py
--rw-rw-rw-   0        0        0       42 2023-05-19 16:20:00.457261 ms_general_utils-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      676 2023-05-19 16:19:26.000000 ms_general_utils-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:51:53.372537 ms_general_utils-1.4.2/
+-rw-rw-rw-   0        0        0     1073 2023-03-14 11:56:37.000000 ms_general_utils-1.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      354 2023-06-20 09:51:53.368533 ms_general_utils-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-06-20 09:51:32.000000 ms_general_utils-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 09:51:53.308971 ms_general_utils-1.4.2/ms_general_utils.egg-info/
+-rw-rw-rw-   0        0        0      354 2023-06-20 09:51:53.000000 ms_general_utils-1.4.2/ms_general_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-06-20 09:51:53.000000 ms_general_utils-1.4.2/ms_general_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 09:51:53.000000 ms_general_utils-1.4.2/ms_general_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 09:51:53.000000 ms_general_utils-1.4.2/ms_general_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 09:51:53.365532 ms_general_utils-1.4.2/ms_utils/
+-rw-rw-rw-   0        0        0      555 2023-03-27 15:14:21.000000 ms_general_utils-1.4.2/ms_utils/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-03-17 12:23:38.000000 ms_general_utils-1.4.2/ms_utils/abstract_model.py
+-rw-rw-rw-   0        0        0     1034 2023-03-17 11:27:17.000000 ms_general_utils-1.4.2/ms_utils/binary_uuid.py
+-rw-rw-rw-   0        0        0      695 2023-03-17 08:52:55.000000 ms_general_utils-1.4.2/ms_utils/func_date.py
+-rw-rw-rw-   0        0        0     2570 2023-04-03 15:04:19.000000 ms_general_utils-1.4.2/ms_utils/generic_crud_class.py
+-rw-rw-rw-   0        0        0      706 2023-03-17 08:52:56.000000 ms_general_utils-1.4.2/ms_utils/generic_pagination.py
+-rw-rw-rw-   0        0        0     1527 2023-04-03 17:16:10.000000 ms_general_utils-1.4.2/ms_utils/model_utils.py
+-rw-rw-rw-   0        0        0      341 2023-03-17 08:52:56.000000 ms_general_utils-1.4.2/ms_utils/prepare_json_response.py
+-rw-rw-rw-   0        0        0      622 2023-05-19 16:18:44.000000 ms_general_utils-1.4.2/ms_utils/validation_utils.py
+-rw-rw-rw-   0        0        0     4724 2023-06-20 09:49:09.000000 ms_general_utils-1.4.2/ms_utils/view_utils.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 09:51:53.373529 ms_general_utils-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      676 2023-06-20 09:50:09.000000 ms_general_utils-1.4.2/setup.py
```

### Comparing `ms_general_utils-1.4.1/LICENSE.txt` & `ms_general_utils-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.1/ms_utils/__init__.py` & `ms_general_utils-1.4.2/ms_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.1/ms_utils/binary_uuid.py` & `ms_general_utils-1.4.2/ms_utils/binary_uuid.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.1/ms_utils/func_date.py` & `ms_general_utils-1.4.2/ms_utils/func_date.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.1/ms_utils/generic_crud_class.py` & `ms_general_utils-1.4.2/ms_utils/generic_crud_class.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.1/ms_utils/generic_pagination.py` & `ms_general_utils-1.4.2/ms_utils/generic_pagination.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.1/ms_utils/model_utils.py` & `ms_general_utils-1.4.2/ms_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.1/ms_utils/validation_utils.py` & `ms_general_utils-1.4.2/ms_utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.1/ms_utils/view_utils.py` & `ms_general_utils-1.4.2/ms_utils/view_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,19 +18,23 @@
     db = None
 
     def __int__(self, ma, app, db):
         self.db = db
         self.ma = ma
         self.ma.init_app(app)
 
-    def generic_list(self, model, schema, **kwargs):
+    def generic_list(self, model, schema, is_paginated=True, **kwargs):
         """
         Generic list
         :return: jsonify
         """
+        if not is_paginated:
+            query = model.query.all()
+            data = generic_get_serialize_data(schema(many=True), query)
+            return prepare_json_response(f'{model.__name__} get successfully', data=data)
         page = int(request.args.get('page')) if request.args.get('page') else 1
         per_page = int(request.args.get('per_page')) if request.args.get('per_page') else 10
 
         query = model.query.filter_by(**kwargs) \
             .paginate(page=page, per_page=per_page) if request.args.get(
             'q') else model.query.paginate(page=page, per_page=per_page)
         query.items = generic_get_serialize_data(schema(many=True), query.items)
```

### Comparing `ms_general_utils-1.4.1/setup.py` & `ms_general_utils-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ms_general_utils',
     packages=find_packages(),
     include_package_data=True,
-    version='1.4.1',
+    version='1.4.2',
     description='General functions for the implementation of microservices.',
     authors=[
         {"name": "Alejandro A. Serrano Correa", "email": "alejandroasc93@gmail.com"},
         {"name": "Rene Gonzalez Ramos", "email": "rgramos9310@gmail.com"}
     ],
     license="GPLv3",
     url="https://github.com/rgramos/ms-utils.git",
```

