# Comparing `tmp/apache-airflow-providers-mongo-3.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-mongo-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-mongo-3.2.0rc2.tar", last modified: Fri May 19 17:52:57 2023, max compression
+gzip compressed data, was "apache-airflow-providers-mongo-3.2.1rc1.tar", last modified: Tue Jun 20 11:42:36 2023, max compression
```

## Comparing `apache-airflow-providers-mongo-3.2.0rc2.tar` & `apache-airflow-providers-mongo-3.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:57.000000 apache-airflow-providers-mongo-3.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-mongo-3.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:55.000000 apache-airflow-providers-mongo-3.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-mongo-3.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10429 2023-05-19 17:52:57.000000 apache-airflow-providers-mongo-3.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8905 2023-05-19 17:52:55.000000 apache-airflow-providers-mongo-3.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:56.000000 apache-airflow-providers-mongo-3.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:56.000000 apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:57.000000 apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-05-19 12:14:08.000000 apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2349 2023-05-19 17:52:55.000000 apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:57.000000 apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13758 2023-05-16 07:40:59.000000 apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/hooks/mongo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:57.000000 apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-02-24 18:43:53.000000 apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/sensors/mongo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:57.000000 apache-airflow-providers-mongo-3.2.0rc2/apache_airflow_providers_mongo.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10429 2023-05-19 17:52:56.000000 apache-airflow-providers-mongo-3.2.0rc2/apache_airflow_providers_mongo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      697 2023-05-19 17:52:56.000000 apache-airflow-providers-mongo-3.2.0rc2/apache_airflow_providers_mongo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:56.000000 apache-airflow-providers-mongo-3.2.0rc2/apache_airflow_providers_mongo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-19 17:52:56.000000 apache-airflow-providers-mongo-3.2.0rc2/apache_airflow_providers_mongo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:56.000000 apache-airflow-providers-mongo-3.2.0rc2/apache_airflow_providers_mongo.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-19 17:52:56.000000 apache-airflow-providers-mongo-3.2.0rc2/apache_airflow_providers_mongo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:56.000000 apache-airflow-providers-mongo-3.2.0rc2/apache_airflow_providers_mongo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-mongo-3.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1857 2023-05-19 17:52:57.000000 apache-airflow-providers-mongo-3.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1632 2023-05-19 17:52:55.000000 apache-airflow-providers-mongo-3.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:36.009263 apache-airflow-providers-mongo-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-mongo-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:34.000000 apache-airflow-providers-mongo-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-mongo-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10765 2023-06-20 11:42:36.010449 apache-airflow-providers-mongo-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9240 2023-06-20 11:42:34.000000 apache-airflow-providers-mongo-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:35.929404 apache-airflow-providers-mongo-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:35.930711 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:35.965918 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-06-20 11:42:34.000000 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:35.971897 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13773 2023-06-02 11:31:21.000000 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/hooks/mongo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:35.977864 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2422 2023-06-02 11:31:21.000000 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/sensors/mongo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:36.006364 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10765 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      697 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-mongo-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-06-20 11:42:36.012547 apache-airflow-providers-mongo-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-06-20 11:42:34.000000 apache-airflow-providers-mongo-3.2.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/LICENSE` & `apache-airflow-providers-mongo-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/MANIFEST.in` & `apache-airflow-providers-mongo-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/PKG-INFO` & `apache-airflow-providers-mongo-3.2.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mongo
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mongo package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -48,38 +48,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mongo``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `MongoDB <https://www.mongodb.com/what-is-mongodb>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mongo`` provider. All classes for this provider package
 are in ``airflow.providers.mongo`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-mongo``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -110,14 +110,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/README.rst` & `apache-airflow-providers-mongo-3.2.1rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mongo``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `MongoDB <https://www.mongodb.com/what-is-mongodb>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mongo`` provider. All classes for this provider package
 are in ``airflow.providers.mongo`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-mongo``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -77,14 +77,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/__init__.py` & `apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.2.0"
+__version__ = "3.2.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/get_provider_info.py` & `apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-mongo",
         "name": "MongoDB",
         "description": "`MongoDB <https://www.mongodb.com/what-is-mongodb>`__\n",
         "suspended": False,
         "versions": [
+            "3.2.1",
             "3.2.0",
             "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.3.3",
             "2.3.2",
             "2.3.1",
```

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/hooks/__init__.py` & `apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/hooks/mongo.py` & `apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/hooks/mongo.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Hook for Mongo DB"""
+"""Hook for Mongo DB."""
 from __future__ import annotations
 
 from ssl import CERT_NONE
 from types import TracebackType
 from typing import Any, overload
 from urllib.parse import quote_plus, urlunsplit
 
@@ -29,14 +29,15 @@
 from airflow.hooks.base import BaseHook
 from airflow.typing_compat import Literal
 
 
 class MongoHook(BaseHook):
     """
     Interact with Mongo. This hook uses the Mongo conn_id.
+
     PyMongo Wrapper to Interact With Mongo Database
     Mongo Connection Documentation
     https://docs.mongodb.com/manual/reference/connection-string/index.html
     You can specify connection string options in extra field of your connection
     https://docs.mongodb.com/manual/reference/connection-string/index.html#connection-string-options
 
     If you want use DNS seedlist, set `srv` to True.
@@ -71,15 +72,15 @@
         exc_tb: TracebackType | None,
     ) -> None:
         if self.client is not None:
             self.client.close()
             self.client = None
 
     def get_conn(self) -> MongoClient:
-        """Fetches PyMongo Client"""
+        """Fetches PyMongo Client."""
         if self.client is not None:
             return self.client
 
         # Mongo Connection Options dict that is unpacked when passed to MongoClient
         options = self.extras
 
         # If we are using SSL disable requiring certs from specific hostname
@@ -124,15 +125,16 @@
 
         return mongo_conn.get_database(mongo_db).get_collection(mongo_collection)
 
     def aggregate(
         self, mongo_collection: str, aggregate_query: list, mongo_db: str | None = None, **kwargs
     ) -> pymongo.command_cursor.CommandCursor:
         """
-        Runs an aggregation pipeline and returns the results
+        Runs an aggregation pipeline and returns the results.
+
         https://pymongo.readthedocs.io/en/stable/api/pymongo/collection.html#pymongo.collection.Collection.aggregate
         https://pymongo.readthedocs.io/en/stable/examples/aggregation.html
         """
         collection = self.get_collection(mongo_collection, mongo_db=mongo_db)
 
         return collection.aggregate(aggregate_query, **kwargs)
 
@@ -166,40 +168,43 @@
         query: dict,
         find_one: bool = False,
         mongo_db: str | None = None,
         projection: list | dict | None = None,
         **kwargs,
     ) -> pymongo.cursor.Cursor | Any | None:
         """
-        Runs a mongo find query and returns the results
+        Runs a mongo find query and returns the results.
+
         https://pymongo.readthedocs.io/en/stable/api/pymongo/collection.html#pymongo.collection.Collection.find
         """
         collection = self.get_collection(mongo_collection, mongo_db=mongo_db)
 
         if find_one:
             return collection.find_one(query, projection, **kwargs)
         else:
             return collection.find(query, projection, **kwargs)
 
     def insert_one(
         self, mongo_collection: str, doc: dict, mongo_db: str | None = None, **kwargs
     ) -> pymongo.results.InsertOneResult:
         """
-        Inserts a single document into a mongo collection
+        Inserts a single document into a mongo collection.
+
         https://pymongo.readthedocs.io/en/stable/api/pymongo/collection.html#pymongo.collection.Collection.insert_one
         """
         collection = self.get_collection(mongo_collection, mongo_db=mongo_db)
 
         return collection.insert_one(doc, **kwargs)
 
     def insert_many(
         self, mongo_collection: str, docs: dict, mongo_db: str | None = None, **kwargs
     ) -> pymongo.results.InsertManyResult:
         """
         Inserts many docs into a mongo collection.
+
         https://pymongo.readthedocs.io/en/stable/api/pymongo/collection.html#pymongo.collection.Collection.insert_many
         """
         collection = self.get_collection(mongo_collection, mongo_db=mongo_db)
 
         return collection.insert_many(docs, **kwargs)
 
     def update_one(
@@ -208,14 +213,15 @@
         filter_doc: dict,
         update_doc: dict,
         mongo_db: str | None = None,
         **kwargs,
     ) -> pymongo.results.UpdateResult:
         """
         Updates a single document in a mongo collection.
+
         https://pymongo.readthedocs.io/en/stable/api/pymongo/collection.html#pymongo.collection.Collection.update_one
 
         :param mongo_collection: The name of the collection to update.
         :param filter_doc: A query that matches the documents to update.
         :param update_doc: The modifications to apply.
         :param mongo_db: The name of the database to use.
             Can be omitted; then the database from the connection string is used.
@@ -231,14 +237,15 @@
         filter_doc: dict,
         update_doc: dict,
         mongo_db: str | None = None,
         **kwargs,
     ) -> pymongo.results.UpdateResult:
         """
         Updates one or more documents in a mongo collection.
+
         https://pymongo.readthedocs.io/en/stable/api/pymongo/collection.html#pymongo.collection.Collection.update_many
 
         :param mongo_collection: The name of the collection to update.
         :param filter_doc: A query that matches the documents to update.
         :param update_doc: The modifications to apply.
         :param mongo_db: The name of the database to use.
             Can be omitted; then the database from the connection string is used.
@@ -253,14 +260,15 @@
         doc: dict,
         filter_doc: dict | None = None,
         mongo_db: str | None = None,
         **kwargs,
     ) -> pymongo.results.UpdateResult:
         """
         Replaces a single document in a mongo collection.
+
         https://pymongo.readthedocs.io/en/stable/api/pymongo/collection.html#pymongo.collection.Collection.replace_one
 
         .. note::
             If no ``filter_doc`` is given, it is assumed that the replacement
             document contain the ``_id`` field which is then used as filters.
 
         :param mongo_collection: The name of the collection to update.
@@ -322,14 +330,15 @@
         return collection.bulk_write(requests, **kwargs)
 
     def delete_one(
         self, mongo_collection: str, filter_doc: dict, mongo_db: str | None = None, **kwargs
     ) -> pymongo.results.DeleteResult:
         """
         Deletes a single document in a mongo collection.
+
         https://pymongo.readthedocs.io/en/stable/api/pymongo/collection.html#pymongo.collection.Collection.delete_one
 
         :param mongo_collection: The name of the collection to delete from.
         :param filter_doc: A query that matches the document to delete.
         :param mongo_db: The name of the database to use.
             Can be omitted; then the database from the connection string is used.
         """
@@ -338,14 +347,15 @@
         return collection.delete_one(filter_doc, **kwargs)
 
     def delete_many(
         self, mongo_collection: str, filter_doc: dict, mongo_db: str | None = None, **kwargs
     ) -> pymongo.results.DeleteResult:
         """
         Deletes one or more documents in a mongo collection.
+
         https://pymongo.readthedocs.io/en/stable/api/pymongo/collection.html#pymongo.collection.Collection.delete_many
 
         :param mongo_collection: The name of the collection to delete from.
         :param filter_doc: A query that matches the documents to delete.
         :param mongo_db: The name of the database to use.
             Can be omitted; then the database from the connection string is used.
         """
```

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/sensors/__init__.py` & `apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/airflow/providers/mongo/sensors/mongo.py` & `apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/sensors/mongo.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,22 +24,25 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class MongoSensor(BaseSensorOperator):
     """
-    Checks for the existence of a document which
-    matches the given query in MongoDB. Example:
+    Checks for the existence of a document which matches the given query in MongoDB.
 
-    >>> mongo_sensor = MongoSensor(collection="coll",
-    ...                            query={"key": "value"},
-    ...                            mongo_conn_id="mongo_default",
-    ...                            mongo_db="admin",
-    ...                            task_id="mongo_sensor")
+    .. code-block:: python
+
+        mongo_sensor = MongoSensor(
+            collection="coll",
+            query={"key": "value"},
+            mongo_conn_id="mongo_default",
+            mongo_db="admin",
+            task_id="mongo_sensor",
+        )
 
     :param collection: Target MongoDB collection.
     :param query: The query to find the target document.
     :param mongo_conn_id: The :ref:`Mongo connection id <howto/connection:mongo>` to use
         when connecting to MongoDB.
     :param mongo_db: Target MongoDB name.
     """
```

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/apache_airflow_providers_mongo.egg-info/PKG-INFO` & `apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mongo
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mongo package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -48,38 +48,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mongo``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `MongoDB <https://www.mongodb.com/what-is-mongodb>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mongo`` provider. All classes for this provider package
 are in ``airflow.providers.mongo`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-mongo``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -110,14 +110,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/apache_airflow_providers_mongo.egg-info/SOURCES.txt` & `apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/pyproject.toml` & `apache-airflow-providers-mongo-3.2.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,42 +22,43 @@
 # and we have to pin it to 63.4.3 version
 # The problem is tracked (and this limitation might be removed if it is solved) in:
 # https://github.com/pypa/setuptools/issues/3548
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
+[project]
+requires-python = ">=3.8"
+
 [tool.ruff]
 typing-modules = ["airflow.typing_compat"]
 line-length = 110
 extend-exclude = [
     ".eggs",
     "airflow/_vendor/*",
     "airflow/providers/google/ads/_vendor/*",
     # The files generated by stubgen aren't 100% valid syntax it turns out, and we don't ship them, so we can
     # ignore them in ruff
-    "airflow/providers/common/sql/*/*.pyi"
+    "airflow/providers/common/sql/*/*.pyi",
+    "airflow/migrations/versions/*.py"
 ]
 
-# TODO: Bump to Python 3.8 when support for Python 3.7 is dropped in Airflow.
-target-version = "py37"
-
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
     # implicit single-line string concatenation
     "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
-    # "D400", WIP: see #31135
+    "D400",
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
     "D403",
     "D412",
     "D419"
 ]
 extend-ignore = [
```

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/setup.cfg` & `apache-airflow-providers-mongo-3.2.1rc1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 	Environment :: Console
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	Framework :: Apache Airflow
 	Framework :: Apache Airflow :: Provider
 	License :: OSI Approved :: Apache Software License
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.1/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
 python_tag = py3
 
 [options]
 zip_safe = False
 include_package_data = True
-python_requires = ~=3.7
+python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow>=2.4.0.dev0
 	dnspython>=1.13.0
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.mongo.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.mongo
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-mongo-3.2.0rc2/setup.py` & `apache-airflow-providers-mongo-3.2.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-mongo package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.0"
+version = "3.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-mongo setup."""
     setup(
         version=version,
         extras_require={},
```

