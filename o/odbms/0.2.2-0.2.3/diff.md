# Comparing `tmp/odbms-0.2.2.tar.gz` & `tmp/odbms-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbms-0.2.2.tar", last modified: Mon Dec 12 00:17:56 2022, max compression
+gzip compressed data, was "odbms-0.2.3.tar", last modified: Tue Jun 20 01:13:12 2023, max compression
```

## Comparing `odbms-0.2.2.tar` & `odbms-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-12-12 00:17:56.943207 odbms-0.2.2/
--rw-rw-rw-   0        0        0    35802 2022-10-19 17:29:18.000000 odbms-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       18 2022-12-11 19:54:49.000000 odbms-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1033 2022-12-12 00:17:56.936210 odbms-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      121 2022-12-11 19:56:35.000000 odbms-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-12 00:17:56.788206 odbms-0.2.2/odbms/
--rw-rw-rw-   0        0        0       77 2022-11-06 17:48:58.000000 odbms-0.2.2/odbms/__init__.py
--rw-rw-rw-   0        0        0     1112 2022-12-11 19:54:16.000000 odbms-0.2.2/odbms/app.py
--rw-rw-rw-   0        0        0     2350 2022-10-25 15:06:39.000000 odbms-0.2.2/odbms/database.py
--rw-rw-rw-   0        0        0     3159 2022-12-11 19:53:53.000000 odbms-0.2.2/odbms/dbms.py
--rw-rw-rw-   0        0        0     9351 2022-12-11 23:35:11.000000 odbms-0.2.2/odbms/model.py
--rw-rw-rw-   0        0        0     1564 2022-11-25 19:37:34.000000 odbms-0.2.2/odbms/mongodb.py
--rw-rw-rw-   0        0        0     6911 2022-11-06 18:44:52.000000 odbms-0.2.2/odbms/mysqldb.py
--rw-rw-rw-   0        0        0     5964 2022-11-02 20:27:27.000000 odbms-0.2.2/odbms/sqlitedb.py
-drwxrwxrwx   0        0        0        0 2022-12-12 00:17:56.926208 odbms-0.2.2/odbms.egg-info/
--rw-rw-rw-   0        0        0     1033 2022-12-12 00:17:56.000000 odbms-0.2.2/odbms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2022-12-12 00:17:56.000000 odbms-0.2.2/odbms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-12 00:17:56.000000 odbms-0.2.2/odbms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2022-12-12 00:17:56.000000 odbms-0.2.2/odbms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-12-12 00:17:56.000000 odbms-0.2.2/odbms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-12 00:17:56.944205 odbms-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1303 2022-12-11 19:56:00.000000 odbms-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:13:12.156293 odbms-0.2.3/
+-rw-rw-rw-   0        0        0    35802 2022-10-19 17:29:18.000000 odbms-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       18 2022-12-11 19:54:49.000000 odbms-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1074 2023-06-20 01:13:12.153294 odbms-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      121 2022-12-11 19:56:35.000000 odbms-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 01:13:12.105776 odbms-0.2.3/odbms/
+-rw-rw-rw-   0        0        0       77 2022-11-06 17:48:58.000000 odbms-0.2.3/odbms/__init__.py
+-rw-rw-rw-   0        0        0     1112 2022-12-11 19:54:16.000000 odbms-0.2.3/odbms/app.py
+-rw-rw-rw-   0        0        0     2350 2022-10-25 15:06:39.000000 odbms-0.2.3/odbms/database.py
+-rw-rw-rw-   0        0        0     3159 2022-12-11 19:53:53.000000 odbms-0.2.3/odbms/dbms.py
+-rw-rw-rw-   0        0        0     9785 2022-12-19 15:51:16.000000 odbms-0.2.3/odbms/model.py
+-rw-rw-rw-   0        0        0     1613 2022-12-19 15:50:11.000000 odbms-0.2.3/odbms/mongodb.py
+-rw-rw-rw-   0        0        0     6911 2022-11-06 18:44:52.000000 odbms-0.2.3/odbms/mysqldb.py
+-rw-rw-rw-   0        0        0     5964 2022-11-02 20:27:27.000000 odbms-0.2.3/odbms/sqlitedb.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:13:12.148291 odbms-0.2.3/odbms.egg-info/
+-rw-rw-rw-   0        0        0     1074 2023-06-20 01:13:11.000000 odbms-0.2.3/odbms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-06-20 01:13:11.000000 odbms-0.2.3/odbms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 01:13:11.000000 odbms-0.2.3/odbms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-20 01:13:11.000000 odbms-0.2.3/odbms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 01:13:11.000000 odbms-0.2.3/odbms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 01:13:12.156293 odbms-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2023-06-20 01:11:08.000000 odbms-0.2.3/setup.py
```

### Comparing `odbms-0.2.2/LICENSE` & `odbms-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `odbms-0.2.2/PKG-INFO` & `odbms-0.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbms
-Version: 0.2.2
+Version: 0.2.3
 Summary: Database client for Mysql, MongoDB and Sqlite
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/odbms/
 Project-URL: Tracker, https://github.com/theonlyamos/odbms/issues
 Keywords: python3 runit developer serverless architecture docker mysql mongodb
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # odbms
 Python package for Managing Mysql, Mongodb and Sqlite instances
 
 ## Installation
```

### Comparing `odbms-0.2.2/odbms/app.py` & `odbms-0.2.3/odbms/app.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.2/odbms/database.py` & `odbms-0.2.3/odbms/database.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.2/odbms/dbms.py` & `odbms-0.2.3/odbms/dbms.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.2/odbms/model.py` & `odbms-0.2.3/odbms/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+from typing import Union
 import uuid
 
 from bson.objectid import ObjectId
 from .dbms import DBMS
 
 class Model():
     '''A model class'''
@@ -171,24 +172,36 @@
         @params None
         @return List[Model] instance(s)
         '''
 
         return [cls(**cls.normalise(elem)) for elem in DBMS.Database.find(cls.TABLE_NAME, {})]
         
     @classmethod
-    def find(cls, params: dict)-> list:
+    def find(cls, params: dict, projection: Union[list,dict] = [])-> list:
         '''
         Class Method for retrieving models
         by provided parameters
 
         @param params
         @return List[Model]
         '''
 
-        return [cls(**cls.normalise(elem)) for elem in DBMS.Database.find(cls.TABLE_NAME, cls.normalise(params, 'params'))]
+        return [cls(**cls.normalise(elem)) for elem in DBMS.Database.find(cls.TABLE_NAME, cls.normalise(params, 'params'), projection)]
+    
+    @classmethod
+    def find_one(cls, params: dict, projection: Union[list,dict] = []):
+        '''
+        Class Method for retrieving one model
+        imstance by provided parameters
+
+        @param params
+        @return List[Model]
+        '''
+
+        return cls(**DBMS.Database.find_one(cls.TABLE_NAME, cls.normalise(params, 'params'), projection))
     
     @classmethod
     def query(cls, column: str, search: str):
         '''
         Class Method for retrieving products
         by their names
```

### Comparing `odbms-0.2.2/odbms/mongodb.py` & `odbms-0.2.3/odbms/mongodb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pymongo import MongoClient
 
 import os
+from typing import Union
 from dotenv import load_dotenv
 
 load_dotenv()
 
 
 class MongoDB(object):
     db = None
@@ -19,19 +20,19 @@
         MongoDB.db = client[database]
 
     @staticmethod
     def insert(collection: str, data: dict):
         return MongoDB.db[collection].insert_one(data)
 
     @staticmethod
-    def find(collection: str, filter: dict = {}, projection: list = []):
+    def find(collection: str, filter: dict = {}, projection: Union[list,dict] = []):
         return MongoDB.db[collection].find(filter, projection)
 
     @staticmethod
-    def find_one(collection: str, filter: dict = {}, projection: list = []):
+    def find_one(collection: str, filter: dict = {}, projection: Union[list,dict] = []):
         return MongoDB.db[collection].find_one(filter, projection)
 
     @staticmethod
     def remove(collection: str, filter: dict):
         return MongoDB.db[collection].delete_many(filter)
 
     @staticmethod
```

### Comparing `odbms-0.2.2/odbms/mysqldb.py` & `odbms-0.2.3/odbms/mysqldb.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.2/odbms/sqlitedb.py` & `odbms-0.2.3/odbms/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.2/odbms.egg-info/PKG-INFO` & `odbms-0.2.3/odbms.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbms
-Version: 0.2.2
+Version: 0.2.3
 Summary: Database client for Mysql, MongoDB and Sqlite
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/odbms/
 Project-URL: Tracker, https://github.com/theonlyamos/odbms/issues
 Keywords: python3 runit developer serverless architecture docker mysql mongodb
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # odbms
 Python package for Managing Mysql, Mongodb and Sqlite instances
 
 ## Installation
```

### Comparing `odbms-0.2.2/setup.py` & `odbms-0.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 
 with open('README.md', 'rt') as file:
     description = file.read()
 
 setup(
     name='odbms',
     version=VERSION,
     author='Amos Amissah',
     author_email='theonlyamos@gmail.com',
     description='Database client for Mysql, MongoDB and Sqlite',
     long_description=description,
     packages=find_packages(),
+    long_description_content_type = "text/markdown",
     include_package_data=True,
     install_requires=['python-dotenv','pymongo', 'mysql', 'mysql-connector', 'mysql-connector-python'],
     keywords='python3 runit developer serverless architecture docker mysql mongodb',
     project_urls={
         'Source': 'https://github.com/theonlyamos/odbms/',
         'Tracker': 'https://github.com/theonlyamos/odbms/issues',
     },
```

