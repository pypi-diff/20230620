# Comparing `tmp/apache-airflow-providers-microsoft-mssql-3.4.0rc2.tar.gz` & `tmp/apache-airflow-providers-microsoft-mssql-3.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-microsoft-mssql-3.4.0rc2.tar", last modified: Fri May 19 17:52:51 2023, max compression
+gzip compressed data, was "apache-airflow-providers-microsoft-mssql-3.4.1rc1.tar", last modified: Tue Jun 20 11:42:30 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2.tar` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:50.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12471 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10890 2023-05-19 17:52:50.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-05-19 12:13:37.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2976 2023-05-19 17:52:50.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/hooks/mssql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/operators/mssql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/apache_airflow_providers_microsoft_mssql.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12471 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/apache_airflow_providers_microsoft_mssql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/apache_airflow_providers_microsoft_mssql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/apache_airflow_providers_microsoft_mssql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/apache_airflow_providers_microsoft_mssql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/apache_airflow_providers_microsoft_mssql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1947 2023-05-19 17:52:51.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1745 2023-05-19 17:52:50.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.262299 apache-airflow-providers-microsoft-mssql-3.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12912 2023-06-20 11:42:30.263458 apache-airflow-providers-microsoft-mssql-3.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11330 2023-06-20 11:42:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.188032 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.189095 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.190231 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.224205 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-06-20 11:01:09.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-06-20 11:42:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.230075 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4227 2023-06-19 10:14:19.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/mssql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.235908 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/mssql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.259868 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12912 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      140 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-06-20 11:42:30.265458 apache-airflow-providers-microsoft-mssql-3.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-06-20 11:42:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/LICENSE` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/MANIFEST.in` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/PKG-INFO` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-mssql
-Version: 3.4.0rc2
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-mssql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.1/
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
 Provides-Extra: common.sql
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -49,38 +49,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.mssql`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.mssql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-mssql``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -130,14 +130,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Check if sqlalchemy_scheme extra contains forbidden characters (#31984)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Microsoft provider only (#31425)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/README.rst` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.mssql`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.mssql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-mssql``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -96,14 +96,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Check if sqlalchemy_scheme extra contains forbidden characters (#31984)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Microsoft provider only (#31425)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.4.0"
+__version__ = "3.4.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/get_provider_info.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-mssql",
         "name": "Microsoft SQL Server (MSSQL)",
         "description": "`Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__\n",
         "suspended": False,
         "versions": [
+            "3.4.1",
             "3.4.0",
             "3.3.2",
             "3.3.1",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/hooks/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/hooks/mssql.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/mssql.py`

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
-"""Microsoft SQLServer hook module"""
+"""Microsoft SQLServer hook module."""
 from __future__ import annotations
 
 from typing import Any
 
 import pymssql
 
 from airflow.providers.common.sql.hooks.sql import DbApiHook
@@ -59,19 +59,18 @@
         """
         conn = self.get_connection(self.mssql_conn_id)  # type: ignore[attr-defined]
         return {k.lower(): v for k, v in conn.extra_dejson.items()}
 
     @property
     def sqlalchemy_scheme(self) -> str:
         """Sqlalchemy scheme either from constructor, connection extras or default."""
-        return (
-            self._sqlalchemy_scheme
-            or self.connection_extra_lower.get("sqlalchemy_scheme")
-            or self.DEFAULT_SQLALCHEMY_SCHEME
-        )
+        extra_scheme = self.connection_extra_lower.get("sqlalchemy_scheme")
+        if not self._sqlalchemy_scheme and extra_scheme and (":" in extra_scheme or "/" in extra_scheme):
+            raise RuntimeError("sqlalchemy_scheme in connection extra should not contain : or / characters")
+        return self._sqlalchemy_scheme or extra_scheme or self.DEFAULT_SQLALCHEMY_SCHEME
 
     def get_uri(self) -> str:
         from urllib.parse import parse_qs, urlencode, urlsplit, urlunsplit
 
         r = list(urlsplit(super().get_uri()))
         # change pymssql driver:
         r[0] = self.sqlalchemy_scheme
@@ -82,20 +81,20 @@
                 qs.pop(k, None)
         r[3] = urlencode(qs, doseq=True)
         return urlunsplit(r)
 
     def get_sqlalchemy_connection(
         self, connect_kwargs: dict | None = None, engine_kwargs: dict | None = None
     ) -> Any:
-        """Sqlalchemy connection object"""
+        """Sqlalchemy connection object."""
         engine = self.get_sqlalchemy_engine(engine_kwargs=engine_kwargs)
         return engine.connect(**(connect_kwargs or {}))
 
     def get_conn(self) -> pymssql.connect:
-        """Returns a mssql connection object"""
+        """Returns a mssql connection object."""
         conn = self.get_connection(self.mssql_conn_id)  # type: ignore[attr-defined]
 
         conn = pymssql.connect(
             server=conn.host,
             user=conn.login,
             password=conn.password,
             database=self.schema or conn.schema,
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/operators/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/airflow/providers/microsoft/mssql/operators/mssql.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/mssql.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 
 
 class MsSqlOperator(SQLExecuteQueryOperator):
     """
-    Executes sql code in a specific Microsoft SQL database
+    Executes sql code in a specific Microsoft SQL database.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:MsSqlOperator`
 
     This operator may use one of two hooks, depending on the ``conn_type`` of the connection.
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-mssql
-Version: 3.4.0rc2
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-mssql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.1/
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
 Provides-Extra: common.sql
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -49,38 +49,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.mssql`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.mssql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-mssql``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -130,14 +130,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Check if sqlalchemy_scheme extra contains forbidden characters (#31984)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Microsoft provider only (#31425)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/pyproject.toml` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/setup.cfg` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.1/
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
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.microsoft.mssql.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.microsoft.mssql
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.0rc2/setup.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-microsoft-mssql package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.0"
+version = "3.4.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-microsoft-mssql setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

