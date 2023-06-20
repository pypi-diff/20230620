# Comparing `tmp/bs_common_fastapi_mongodb-0.2.0.tar.gz` & `tmp/bs_common_fastapi_mongodb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_common_fastapi_mongodb-0.2.0.tar", max compression
+gzip compressed data, was "bs_common_fastapi_mongodb-0.2.1.tar", max compression
```

## Comparing `bs_common_fastapi_mongodb-0.2.0.tar` & `bs_common_fastapi_mongodb-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       27 2023-06-19 21:48:08.450249 bs_common_fastapi_mongodb-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-19 21:52:57.103108 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 21:55:09.317338 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 21:55:15.837448 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/application/__init__.py
--rw-r--r--   0        0        0     3665 2023-06-19 22:02:54.305191 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/application/base.py
--rw-r--r--   0        0        0        0 2023-06-19 22:06:14.214350 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/config/__init__.py
--rw-r--r--   0        0        0      516 2023-06-19 22:08:14.018068 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/config/base.py
--rw-r--r--   0        0        0        0 2023-06-19 22:04:33.818873 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/dependencies/__init__.py
--rw-r--r--   0        0        0      917 2023-06-19 23:50:05.543807 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/dependencies/base.py
--rw-r--r--   0        0        0        0 2023-06-20 00:09:45.267778 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/model/__init__.py
--rw-r--r--   0        0        0      682 2023-06-20 00:13:07.226705 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/model/base_default_model.py
--rw-r--r--   0        0        0      388 2023-06-20 00:13:33.681189 bs_common_fastapi_mongodb-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 bs_common_fastapi_mongodb-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-06-19 21:48:08.450249 bs_common_fastapi_mongodb-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 21:52:57.103108 bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 21:55:09.317338 bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 21:55:15.837448 bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/application/__init__.py
+-rw-r--r--   0        0        0     3671 2023-06-20 00:31:21.233462 bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/application/base.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:06:14.214350 bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/config/__init__.py
+-rw-r--r--   0        0        0      549 2023-06-20 00:24:57.661356 bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/config/base.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:04:33.818873 bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/dependencies/__init__.py
+-rw-r--r--   0        0        0      944 2023-06-20 00:31:39.821962 bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/dependencies/base.py
+-rw-r--r--   0        0        0        0 2023-06-20 00:09:45.267778 bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/model/__init__.py
+-rw-r--r--   0        0        0      682 2023-06-20 00:13:07.226705 bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/model/base_default_model.py
+-rw-r--r--   0        0        0      388 2023-06-20 00:31:59.354481 bs_common_fastapi_mongodb-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 bs_common_fastapi_mongodb-0.2.1/PKG-INFO
```

### Comparing `bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/application/base.py` & `bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/application/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 from abc import abstractmethod
 
 from bson.errors import InvalidId
 from bson.objectid import ObjectId
-from bs_common_fastapi.common.config.base import BaseConfig
+from bs_common_fastapi.common.config.base import base_settings
 from bs_common_fastapi.common.exception import NotFoundException, AppException
 from pydantic.utils import deep_update
 
 
 class BaseApplication:
 
     def __init__(self, db):
@@ -37,15 +37,15 @@
     @staticmethod
     def clean_data(data: dict):
         data.pop('_id', None)
         return data
 
     async def find_all(
             self,
-            limit: int = BaseConfig.APP_MAX_LIMIT_VALUE,
+            limit: int = base_settings.APP_MAX_LIMIT_VALUE,
             skip: int = 0,
             query: dict | None = None,
             sort: dict | None = None,
             projection: dict | None = None
     ):
         q = {x: y for x, y in query.items()} if query is not None else {}
         projection = projection if projection is not None else {}
```

### Comparing `bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/config/base.py` & `bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/config/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,7 +6,10 @@
     MONGODB_HOST: str = os.getenv('MONGODB_HOST')
     MONGODB_USER: str = os.getenv('MONGODB_USER')
     MONGODB_PASS: str = os.getenv('MONGODB_PASS')
     MONGODB_DBNAME: str = os.getenv('MONGODB_DBNAME')
     MONGODB_DRIVER: str = os.getenv('MONGODB_DRIVER')
     MONGODB_ARGS: str = os.getenv('MONGODB_ARGS')
     MONGODB_URI: str = f'{MONGODB_DRIVER}://{MONGODB_USER}:{MONGODB_PASS}@{MONGODB_HOST}/{MONGODB_ARGS}'
+
+
+mongo_settings = MongoConfig()
```

### Comparing `bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/dependencies/base.py` & `bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/dependencies/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import motor.motor_asyncio
 
-from bs_common_fastapi_mongodb.common.config.base import MongoConfig
+from bs_common_fastapi_mongodb.common.config.base import mongo_settings
 from fastapi import Query
 
 
 async def get_db():
-    db = motor.motor_asyncio.AsyncIOMotorClient(MongoConfig.MONGODB_URI)
-    database = db[MongoConfig.MONGODB_DBNAME]
+    db = motor.motor_asyncio.AsyncIOMotorClient(mongo_settings.MONGODB_URI)
+    database = db[mongo_settings.MONGODB_DBNAME]
     try:
         yield database
     finally:
         db.close()
 
 
 async def pagination_parameters(
-    skip: int = Query(description=MongoConfig.APP_DESCRIPTION_SKIP, default=0),
-    limit: int = Query(description=MongoConfig.APP_DESCRIPTION_LIMIT, default=MongoConfig.APP_MAX_LIMIT_VALUE)
+    skip: int = Query(description=mongo_settings.APP_DESCRIPTION_SKIP, default=0),
+    limit: int = Query(description=mongo_settings.APP_DESCRIPTION_LIMIT, default=mongo_settings.APP_MAX_LIMIT_VALUE)
 ):
-    limit = MongoConfig.APP_MAX_LIMIT_VALUE if limit > MongoConfig.APP_MAX_LIMIT_VALUE else limit
+    limit = mongo_settings.APP_MAX_LIMIT_VALUE if limit > mongo_settings.APP_MAX_LIMIT_VALUE else limit
     return {'skip': skip, 'limit': limit}
 
 
 async def projection_parameters(
-        fields: str | None = Query(description=MongoConfig.APP_DESCRIPTION_FIELDS, default=None)
+        fields: str | None = Query(description=mongo_settings.APP_DESCRIPTION_FIELDS, default=None)
 ):
     return {x.strip(): 1 for x in fields.split(',')} if fields is not None else None
```

### Comparing `bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/model/base_default_model.py` & `bs_common_fastapi_mongodb-0.2.1/bs_common_fastapi_mongodb/common/model/base_default_model.py`

 * *Files identical despite different names*

