# Comparing `tmp/apache-airflow-providers-sqlite-3.4.1rc1.tar.gz` & `tmp/apache-airflow-providers-sqlite-3.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-sqlite-3.4.1rc1.tar", last modified: Wed May 24 07:20:30 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sqlite-3.4.2rc1.tar", last modified: Tue Jun 20 11:43:17 2023, max compression
```

## Comparing `apache-airflow-providers-sqlite-3.4.1rc1.tar` & `apache-airflow-providers-sqlite-3.4.2rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:20:29.000000 apache-airflow-providers-sqlite-3.4.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13135 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11530 2023-05-24 07:20:29.000000 apache-airflow-providers-sqlite-3.4.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-05-24 07:09:22.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-05-24 07:20:29.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2400 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/hooks/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/operators/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13135 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      716 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      125 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-sqlite-3.4.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1917 2023-05-24 07:20:30.000000 apache-airflow-providers-sqlite-3.4.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-24 07:20:29.000000 apache-airflow-providers-sqlite-3.4.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.927449 apache-airflow-providers-sqlite-3.4.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-sqlite-3.4.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:16.000000 apache-airflow-providers-sqlite-3.4.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-sqlite-3.4.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13415 2023-06-20 11:43:17.928638 apache-airflow-providers-sqlite-3.4.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11860 2023-06-20 11:43:16.000000 apache-airflow-providers-sqlite-3.4.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.844732 apache-airflow-providers-sqlite-3.4.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.845749 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.881811 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-06-20 11:43:16.000000 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.887856 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2023-06-02 11:31:21.000000 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/hooks/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.893672 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-06-02 11:31:21.000000 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/operators/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.924270 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13415 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-sqlite-3.4.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1878 2023-06-20 11:43:17.930945 apache-airflow-providers-sqlite-3.4.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:43:16.000000 apache-airflow-providers-sqlite-3.4.2rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/LICENSE` & `apache-airflow-providers-sqlite-3.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/MANIFEST.in` & `apache-airflow-providers-sqlite-3.4.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/PKG-INFO` & `apache-airflow-providers-sqlite-3.4.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sqlite
-Version: 3.4.1rc1
+Version: 3.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sqlite package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.2/
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: common.sql
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -50,38 +49,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sqlite``
 
-Release: ``3.4.1rc1``
+Release: ``3.4.2rc1``
 
 
 `SQLite <https://www.sqlite.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sqlite`` provider. All classes for this provider package
 are in ``airflow.providers.sqlite`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-sqlite``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -130,14 +129,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.2
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
 3.4.1
 .....
 
 Misc
 ~~~~
 
 * ``Bring back min-airflow-version for preinstalled providers (#31469)``
```

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/README.rst` & `apache-airflow-providers-sqlite-3.4.2rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sqlite``
 
-Release: ``3.4.1rc1``
+Release: ``3.4.2rc1``
 
 
 `SQLite <https://www.sqlite.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sqlite`` provider. All classes for this provider package
 are in ``airflow.providers.sqlite`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-sqlite``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -95,14 +95,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.2
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
 3.4.1
 .....
 
 Misc
 ~~~~
 
 * ``Bring back min-airflow-version for preinstalled providers (#31469)``
```

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/__init__.py` & `apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.4.1"
+__version__ = "3.4.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/get_provider_info.py` & `apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-sqlite",
         "name": "SQLite",
         "description": "`SQLite <https://www.sqlite.org/>`__\n",
         "suspended": False,
         "versions": [
+            "3.4.2",
             "3.4.1",
             "3.4.0",
             "3.3.2",
             "3.3.1",
             "3.3.0",
             "3.2.1",
             "3.2.0",
```

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/hooks/__init__.py` & `apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/hooks/sqlite.py` & `apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/hooks/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,24 +29,24 @@
     conn_name_attr = "sqlite_conn_id"
     default_conn_name = "sqlite_default"
     conn_type = "sqlite"
     hook_name = "Sqlite"
     placeholder = "?"
 
     def get_conn(self) -> sqlite3.dbapi2.Connection:
-        """Returns a sqlite connection object"""
+        """Returns a sqlite connection object."""
         sqlalchemy_uri = self.get_uri()
         # The sqlite3 connection does not use the sqlite scheme.
         # See https://docs.sqlalchemy.org/en/14/dialects/sqlite.html#uri-connections for details.
         sqlite_uri = sqlalchemy_uri.replace("sqlite:///", "file:")
         conn = sqlite3.connect(sqlite_uri, uri=True)
         return conn
 
     def get_uri(self) -> str:
-        """Override DbApiHook get_uri method for get_sqlalchemy_engine()"""
+        """Override DbApiHook get_uri method for get_sqlalchemy_engine()."""
         conn_id = getattr(self, self.conn_name_attr)
         airflow_conn = self.get_connection(conn_id)
         if airflow_conn.conn_type is None:
             airflow_conn.conn_type = self.conn_type
         airflow_uri = unquote(airflow_conn.get_uri())
         # For sqlite, there is no schema in the connection URI. So we need to drop the trailing slash.
         airflow_sqlite_uri = airflow_uri.replace("/?", "?")
```

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/operators/__init__.py` & `apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/airflow/providers/sqlite/operators/sqlite.py` & `apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/operators/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 
 
 class SqliteOperator(SQLExecuteQueryOperator):
     """
-    Executes sql code in a specific Sqlite database
+    Executes sql code in a specific Sqlite database.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SqliteOperator`
 
     :param sql: the sql code to be executed. Can receive a str representing a
         sql statement, a list of str (sql statements), or reference to a template file.
```

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/PKG-INFO` & `apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sqlite
-Version: 3.4.1rc1
+Version: 3.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sqlite package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.2/
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: common.sql
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -50,38 +49,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sqlite``
 
-Release: ``3.4.1rc1``
+Release: ``3.4.2rc1``
 
 
 `SQLite <https://www.sqlite.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sqlite`` provider. All classes for this provider package
 are in ``airflow.providers.sqlite`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-sqlite``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -130,14 +129,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.2
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
 3.4.1
 .....
 
 Misc
 ~~~~
 
 * ``Bring back min-airflow-version for preinstalled providers (#31469)``
```

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/apache_airflow_providers_sqlite.egg-info/SOURCES.txt` & `apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/pyproject.toml` & `apache-airflow-providers-sqlite-3.4.2rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/setup.cfg` & `apache-airflow-providers-sqlite-3.4.2rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -17,35 +17,34 @@
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
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.2/
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
 	apache-airflow-providers-common-sql>=1.3.1.dev0
 	apache-airflow>=2.4.0.dev0
```

### Comparing `apache-airflow-providers-sqlite-3.4.1rc1/setup.py` & `apache-airflow-providers-sqlite-3.4.2rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-sqlite package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.1"
+version = "3.4.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-sqlite setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

