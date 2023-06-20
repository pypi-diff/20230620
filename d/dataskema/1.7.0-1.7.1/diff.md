# Comparing `tmp/dataskema-1.7.0.tar.gz` & `tmp/dataskema-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dataskema-1.7.0.tar", last modified: Sun Jun 18 09:54:19 2023, max compression
+gzip compressed data, was "dist/dataskema-1.7.1.tar", last modified: Tue Jun 20 06:16:56 2023, max compression
```

## Comparing `dataskema-1.7.0.tar` & `dataskema-1.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lagor      (501) staff       (20)        0 2023-06-18 09:54:19.000000 dataskema-1.7.0/
--rw-r--r--   0 lagor      (501) staff       (20)    25324 2023-06-18 09:54:19.000000 dataskema-1.7.0/PKG-INFO
--rw-r--r--   0 lagor      (501) staff       (20)     1080 2022-04-04 16:22:31.000000 dataskema-1.7.0/LICENSE
--rw-r--r--   0 lagor      (501) staff       (20)    20387 2023-06-18 09:52:00.000000 dataskema-1.7.0/README.md
--rw-r--r--   0 lagor      (501) staff       (20)      955 2023-06-18 09:52:13.000000 dataskema-1.7.0/setup.py
-drwxr-xr-x   0 lagor      (501) staff       (20)        0 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema/
--rw-r--r--   0 lagor      (501) staff       (20)    26776 2023-06-18 09:54:05.000000 dataskema-1.7.0/dataskema/validator.py
--rw-r--r--   0 lagor      (501) staff       (20)     4137 2023-06-18 09:38:01.000000 dataskema-1.7.0/dataskema/lang.py
--rw-r--r--   0 lagor      (501) staff       (20)     4008 2023-06-18 09:37:38.000000 dataskema-1.7.0/dataskema/data_schema.py
-drwxr-xr-x   0 lagor      (501) staff       (20)        0 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema/decorators/
--rw-r--r--   0 lagor      (501) staff       (20)     1794 2023-06-18 09:43:11.000000 dataskema-1.7.0/dataskema/decorators/flask.py
--rw-r--r--   0 lagor      (501) staff       (20)        0 2022-04-03 18:14:32.000000 dataskema-1.7.0/dataskema/decorators/__init__.py
--rw-r--r--   0 lagor      (501) staff       (20)      546 2022-06-08 14:36:28.000000 dataskema-1.7.0/dataskema/decorators/args.py
--rw-r--r--   0 lagor      (501) staff       (20)     1448 2022-04-20 06:53:20.000000 dataskema-1.7.0/dataskema/util.py
--rw-r--r--   0 lagor      (501) staff       (20)      136 2022-06-08 14:00:23.000000 dataskema-1.7.0/dataskema/__init__.py
--rw-r--r--   0 lagor      (501) staff       (20)    10989 2022-06-07 06:08:56.000000 dataskema-1.7.0/dataskema/data_types.py
--rw-r--r--   0 lagor      (501) staff       (20)       38 2023-06-18 09:54:19.000000 dataskema-1.7.0/setup.cfg
-drwxr-xr-x   0 lagor      (501) staff       (20)        0 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema.egg-info/
--rw-r--r--   0 lagor      (501) staff       (20)    25324 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema.egg-info/PKG-INFO
--rw-r--r--   0 lagor      (501) staff       (20)        1 2022-04-17 19:18:28.000000 dataskema-1.7.0/dataskema.egg-info/not-zip-safe
--rw-r--r--   0 lagor      (501) staff       (20)      444 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema.egg-info/SOURCES.txt
--rw-r--r--   0 lagor      (501) staff       (20)        6 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema.egg-info/requires.txt
--rw-r--r--   0 lagor      (501) staff       (20)       10 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema.egg-info/top_level.txt
--rw-r--r--   0 lagor      (501) staff       (20)        1 2023-06-18 09:54:19.000000 dataskema-1.7.0/dataskema.egg-info/dependency_links.txt
+drwxr-xr-x   0 lagor      (501) staff       (20)        0 2023-06-20 06:16:56.000000 dataskema-1.7.1/
+-rw-r--r--   0 lagor      (501) staff       (20)    25392 2023-06-20 06:16:56.000000 dataskema-1.7.1/PKG-INFO
+-rw-r--r--   0 lagor      (501) staff       (20)     1080 2022-04-04 16:22:31.000000 dataskema-1.7.1/LICENSE
+-rw-r--r--   0 lagor      (501) staff       (20)    20431 2023-06-20 06:16:05.000000 dataskema-1.7.1/README.md
+-rw-r--r--   0 lagor      (501) staff       (20)      955 2023-06-20 06:16:52.000000 dataskema-1.7.1/setup.py
+drwxr-xr-x   0 lagor      (501) staff       (20)        0 2023-06-20 06:16:56.000000 dataskema-1.7.1/dataskema/
+-rw-r--r--   0 lagor      (501) staff       (20)    26776 2023-06-18 09:54:05.000000 dataskema-1.7.1/dataskema/validator.py
+-rw-r--r--   0 lagor      (501) staff       (20)     4306 2023-06-19 11:56:12.000000 dataskema-1.7.1/dataskema/lang.py
+-rw-r--r--   0 lagor      (501) staff       (20)     4008 2023-06-18 09:37:38.000000 dataskema-1.7.1/dataskema/data_schema.py
+drwxr-xr-x   0 lagor      (501) staff       (20)        0 2023-06-20 06:16:56.000000 dataskema-1.7.1/dataskema/decorators/
+-rw-r--r--   0 lagor      (501) staff       (20)     1794 2023-06-18 09:43:11.000000 dataskema-1.7.1/dataskema/decorators/flask.py
+-rw-r--r--   0 lagor      (501) staff       (20)        0 2022-04-03 18:14:32.000000 dataskema-1.7.1/dataskema/decorators/__init__.py
+-rw-r--r--   0 lagor      (501) staff       (20)      546 2022-06-08 14:36:28.000000 dataskema-1.7.1/dataskema/decorators/args.py
+-rw-r--r--   0 lagor      (501) staff       (20)     1448 2022-04-20 06:53:20.000000 dataskema-1.7.1/dataskema/util.py
+-rw-r--r--   0 lagor      (501) staff       (20)      136 2022-06-08 14:00:23.000000 dataskema-1.7.1/dataskema/__init__.py
+-rw-r--r--   0 lagor      (501) staff       (20)    10989 2022-06-07 06:08:56.000000 dataskema-1.7.1/dataskema/data_types.py
+-rw-r--r--   0 lagor      (501) staff       (20)       38 2023-06-20 06:16:56.000000 dataskema-1.7.1/setup.cfg
+drwxr-xr-x   0 lagor      (501) staff       (20)        0 2023-06-20 06:16:56.000000 dataskema-1.7.1/dataskema.egg-info/
+-rw-r--r--   0 lagor      (501) staff       (20)    25392 2023-06-20 06:16:56.000000 dataskema-1.7.1/dataskema.egg-info/PKG-INFO
+-rw-r--r--   0 lagor      (501) staff       (20)        1 2022-04-17 19:18:28.000000 dataskema-1.7.1/dataskema.egg-info/not-zip-safe
+-rw-r--r--   0 lagor      (501) staff       (20)      444 2023-06-20 06:16:56.000000 dataskema-1.7.1/dataskema.egg-info/SOURCES.txt
+-rw-r--r--   0 lagor      (501) staff       (20)        6 2023-06-20 06:16:56.000000 dataskema-1.7.1/dataskema.egg-info/requires.txt
+-rw-r--r--   0 lagor      (501) staff       (20)       10 2023-06-20 06:16:56.000000 dataskema-1.7.1/dataskema.egg-info/top_level.txt
+-rw-r--r--   0 lagor      (501) staff       (20)        1 2023-06-20 06:16:56.000000 dataskema-1.7.1/dataskema.egg-info/dependency_links.txt
```

### Comparing `dataskema-1.7.0/PKG-INFO` & `dataskema-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: dataskema
-Version: 1.7.0
+Version: 1.7.1
 Summary: Data schema to validate parameters easily, quickly and with minimal code
 Home-page: https://github.com/lagor-github/dataskema
 Author: Luis A. González
 Author-email: lagor55@gmail.com
 License: MIT
 Description: # `dataskema`
         Data schema validation for python
         
-        v1.7.0
-        - Now dict types can have schema in its fields using 'schema' keyword
+        v1.7.1
+        - Message with wrong formatting fixed 
+        
+        - v1.7.0
+        - Now dict fields can have its own schema using 'schema' keyword
         - Use 'only-schema-keys' keyword to reject no declareted fields
         - New 'null-when-zero' keyword that rewrites incoming value to None value when zero (number or string)
         - Some minor bugs fixed
         
         v1.6.7
         - Bug fixed in @dataskema.flask_url
```

### Comparing `dataskema-1.7.0/LICENSE` & `dataskema-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataskema-1.7.0/README.md` & `dataskema-1.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # `dataskema`
 Data schema validation for python
 
-v1.7.0
-- Now dict types can have schema in its fields using 'schema' keyword
+v1.7.1
+- Message with wrong formatting fixed 
+
+- v1.7.0
+- Now dict fields can have its own schema using 'schema' keyword
 - Use 'only-schema-keys' keyword to reject no declareted fields
 - New 'null-when-zero' keyword that rewrites incoming value to None value when zero (number or string)
 - Some minor bugs fixed
 
 v1.6.7
 - Bug fixed in @dataskema.flask_url
```

### Comparing `dataskema-1.7.0/setup.py` & `dataskema-1.7.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r") as fh:
     readme_description = fh.read()
 
 setup(
     name='dataskema',
     packages=['dataskema', 'dataskema.decorators'],
     include_package_data=True,  # -- para que se incluyan archivos sin extension .py
-    version='1.7.0',
+    version='1.7.1',
     description='Data schema to validate parameters easily, quickly and with minimal code',
     long_description=readme_description,
     long_description_content_type="text/markdown",
     zip_safe=False,
     install_requires=[
         'flask',
     ],
```

### Comparing `dataskema-1.7.0/dataskema/validator.py` & `dataskema-1.7.1/dataskema/validator.py`

 * *Files identical despite different names*

### Comparing `dataskema-1.7.0/dataskema/lang.py` & `dataskema-1.7.1/dataskema/lang.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,17 +58,20 @@
 
 
 def get_message(val_message: str, val_params: dict, anonymize: bool or None = False) -> str:
     ex_message = val_message
     for (key, value) in val_params.items():
         if key == 'label':
             value = "'" + value + "'" if not anonymize else _get_anonymous()
+            ex_message = util.trim(ex_message.replace('\'{' + key + '}\'', str(value)))
+            ex_message = ex_message[0].upper() + ex_message[1:]
+            continue
         if value is None:
             value = ''
-        ex_message = util.trim(ex_message.replace('\'{' + key + '}\'', str(value)))
+        ex_message = util.trim(ex_message.replace('{' + key + '}', str(value)))
         ex_message = ex_message[0].upper() + ex_message[1:]
     return ex_message
 
 
 VAL_ERROR_PARAM_IS_MANDATORY = {
     EN: "'{label}' is mandatory",
     ES: "'{label}' es obligatorio",
```

### Comparing `dataskema-1.7.0/dataskema/data_schema.py` & `dataskema-1.7.1/dataskema/data_schema.py`

 * *Files identical despite different names*

### Comparing `dataskema-1.7.0/dataskema/decorators/flask.py` & `dataskema-1.7.1/dataskema/decorators/flask.py`

 * *Files identical despite different names*

### Comparing `dataskema-1.7.0/dataskema/decorators/args.py` & `dataskema-1.7.1/dataskema/decorators/args.py`

 * *Files identical despite different names*

### Comparing `dataskema-1.7.0/dataskema/util.py` & `dataskema-1.7.1/dataskema/util.py`

 * *Files identical despite different names*

### Comparing `dataskema-1.7.0/dataskema/data_types.py` & `dataskema-1.7.1/dataskema/data_types.py`

 * *Files identical despite different names*

### Comparing `dataskema-1.7.0/dataskema.egg-info/PKG-INFO` & `dataskema-1.7.1/dataskema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: dataskema
-Version: 1.7.0
+Version: 1.7.1
 Summary: Data schema to validate parameters easily, quickly and with minimal code
 Home-page: https://github.com/lagor-github/dataskema
 Author: Luis A. González
 Author-email: lagor55@gmail.com
 License: MIT
 Description: # `dataskema`
         Data schema validation for python
         
-        v1.7.0
-        - Now dict types can have schema in its fields using 'schema' keyword
+        v1.7.1
+        - Message with wrong formatting fixed 
+        
+        - v1.7.0
+        - Now dict fields can have its own schema using 'schema' keyword
         - Use 'only-schema-keys' keyword to reject no declareted fields
         - New 'null-when-zero' keyword that rewrites incoming value to None value when zero (number or string)
         - Some minor bugs fixed
         
         v1.6.7
         - Bug fixed in @dataskema.flask_url
```

