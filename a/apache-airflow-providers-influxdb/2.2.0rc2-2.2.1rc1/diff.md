# Comparing `tmp/apache-airflow-providers-influxdb-2.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-influxdb-2.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-influxdb-2.2.0rc2.tar", last modified: Fri May 19 17:52:43 2023, max compression
+gzip compressed data, was "apache-airflow-providers-influxdb-2.2.1rc1.tar", last modified: Tue Jun 20 11:42:22 2023, max compression
```

## Comparing `apache-airflow-providers-influxdb-2.2.0rc2.tar` & `apache-airflow-providers-influxdb-2.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-influxdb-2.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:42.000000 apache-airflow-providers-influxdb-2.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-influxdb-2.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8499 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6966 2023-05-19 17:52:42.000000 apache-airflow-providers-influxdb-2.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-19 12:12:48.000000 apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2209 2023-05-19 17:52:42.000000 apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5697 2023-02-24 18:43:53.000000 apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/hooks/influxdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-02-24 18:43:53.000000 apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/operators/influxdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/apache_airflow_providers_influxdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8499 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/apache_airflow_providers_influxdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/apache_airflow_providers_influxdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/apache_airflow_providers_influxdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/apache_airflow_providers_influxdb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/apache_airflow_providers_influxdb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       68 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/apache_airflow_providers_influxdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/apache_airflow_providers_influxdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-influxdb-2.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1883 2023-05-19 17:52:43.000000 apache-airflow-providers-influxdb-2.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1650 2023-05-19 17:52:42.000000 apache-airflow-providers-influxdb-2.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.140363 apache-airflow-providers-influxdb-2.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-influxdb-2.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:21.000000 apache-airflow-providers-influxdb-2.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-influxdb-2.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8954 2023-06-20 11:42:22.141500 apache-airflow-providers-influxdb-2.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7420 2023-06-20 11:42:21.000000 apache-airflow-providers-influxdb-2.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.061728 apache-airflow-providers-influxdb-2.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.062916 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.098077 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-06-20 11:42:21.000000 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.104101 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-06-08 05:42:54.000000 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/hooks/influxdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.110916 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-06-02 11:31:21.000000 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/operators/influxdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.136226 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8954 2023-06-20 11:42:21.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:42:22.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:22.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:42:22.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:22.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-20 11:42:22.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:22.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-influxdb-2.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-06-20 11:42:22.143583 apache-airflow-providers-influxdb-2.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:42:20.000000 apache-airflow-providers-influxdb-2.2.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/LICENSE` & `apache-airflow-providers-influxdb-2.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/MANIFEST.in` & `apache-airflow-providers-influxdb-2.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/PKG-INFO` & `apache-airflow-providers-influxdb-2.2.1rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-influxdb
-Version: 2.2.0rc2
+Version: 2.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-influxdb package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.1/
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
 
 
 Package ``apache-airflow-providers-influxdb``
 
-Release: ``2.2.0rc2``
+Release: ``2.2.1rc1``
 
 
 `InfluxDB <https://www.influxdata.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``influxdb`` provider. All classes for this provider package
 are in ``airflow.providers.influxdb`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-influxdb``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
@@ -111,14 +111,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+2.2.1
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
+   * ``Replace spelling directive with spelling:word-list (#31752)``
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 2.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/README.rst` & `apache-airflow-providers-influxdb-2.2.1rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-influxdb``
 
-Release: ``2.2.0rc2``
+Release: ``2.2.1rc1``
 
 
 `InfluxDB <https://www.influxdata.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``influxdb`` provider. All classes for this provider package
 are in ``airflow.providers.influxdb`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-influxdb``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
@@ -78,14 +78,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+2.2.1
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
+   * ``Replace spelling directive with spelling:word-list (#31752)``
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 2.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/__init__.py` & `apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/get_provider_info.py` & `apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-influxdb",
         "name": "Influxdb",
         "description": "`InfluxDB <https://www.influxdata.com/>`__\n",
         "dependencies": ["apache-airflow>=2.4.0", "influxdb-client>=1.19.0", "requests>=2.26.0"],
         "suspended": False,
-        "versions": ["2.2.0", "2.1.0", "2.0.0", "1.1.3", "1.1.2", "1.1.1", "1.1.0", "1.0.0"],
+        "versions": ["2.2.1", "2.2.0", "2.1.0", "2.0.0", "1.1.3", "1.1.2", "1.1.1", "1.1.0", "1.0.0"],
         "integrations": [
             {
                 "integration-name": "Influxdb",
                 "external-doc-url": "https://www.influxdata.com/",
                 "tags": ["software"],
             }
         ],
```

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/hooks/__init__.py` & `apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/hooks/influxdb.py` & `apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/hooks/influxdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """
 This module allows to connect to a InfluxDB database.
 
-.. spelling::
+.. spelling:word-list::
 
     FluxTable
 """
 from __future__ import annotations
 
 import pandas as pd
 from influxdb_client import InfluxDBClient
@@ -31,16 +31,15 @@
 from influxdb_client.client.write_api import SYNCHRONOUS
 
 from airflow.hooks.base import BaseHook
 from airflow.models import Connection
 
 
 class InfluxDBHook(BaseHook):
-    """
-    Interact with InfluxDB.
+    """Interact with InfluxDB.
 
     Performs a connection to InfluxDB and retrieves client.
 
     :param influxdb_conn_id: Reference to :ref:`Influxdb connection id <howto/connection:influxdb>`.
     """
 
     conn_name_attr = "influxdb_conn_id"
@@ -57,28 +56,21 @@
         self.uri = None
         self.org_name = None
 
     def get_client(self, uri, token, org_name):
         return InfluxDBClient(url=uri, token=token, org=org_name)
 
     def get_uri(self, conn: Connection):
-        """
-        Function to add additional parameters to the URI
-        based on SSL or other InfluxDB host requirements
-
-        """
+        """Add additional parameters to the URI based on InfluxDB host requirements."""
         conn_scheme = "https" if conn.schema is None else conn.schema
         conn_port = 7687 if conn.port is None else conn.port
         return f"{conn_scheme}://{conn.host}:{conn_port}"
 
     def get_conn(self) -> InfluxDBClient:
-        """
-        Function that initiates a new InfluxDB connection
-        with token and organization name
-        """
+        """Initiate a new InfluxDB connection with token and organization name."""
         self.connection = self.get_connection(self.influxdb_conn_id)
         self.extras = self.connection.extra_dejson.copy()
 
         self.uri = self.get_uri(self.connection)
         self.log.info("URI: %s", self.uri)
 
         if self.client is not None:
@@ -91,74 +83,71 @@
         self.log.info("Organization: %s", self.org_name)
 
         self.client = self.get_client(self.uri, token, self.org_name)
 
         return self.client
 
     def query(self, query) -> list[FluxTable]:
-        """
-        Function to to run the query.
-        Note: The bucket name
-        should be included in the query
+        """Run the query.
+
+        Note: The bucket name should be included in the query.
 
         :param query: InfluxDB query
         :return: List
         """
         client = self.get_conn()
 
         query_api = client.query_api()
         return query_api.query(query)
 
     def query_to_df(self, query) -> pd.DataFrame:
-        """
-        Function to run the query and
-        return a pandas dataframe
-        Note: The bucket name
-        should be included in the query
+        """Run the query and return a pandas dataframe.
+
+        Note: The bucket name should be included in the query.
 
         :param query: InfluxDB query
         :return: pd.DataFrame
         """
         client = self.get_conn()
 
         query_api = client.query_api()
         return query_api.query_data_frame(query)
 
     def write(self, bucket_name, point_name, tag_name, tag_value, field_name, field_value, synchronous=False):
-        """
-        Writes a Point to the bucket specified.
-        Example: Point("my_measurement").tag("location", "Prague").field("temperature", 25.3)
+        """Write a Point to the bucket specified.
+
+        Example: ``Point("my_measurement").tag("location", "Prague").field("temperature", 25.3)``
         """
         # By defaults its Batching
         if synchronous:
             write_api = self.client.write_api(write_options=SYNCHRONOUS)
         else:
             write_api = self.client.write_api()
 
         p = Point(point_name).tag(tag_name, tag_value).field(field_name, field_value)
 
         write_api.write(bucket=bucket_name, record=p)
 
     def create_organization(self, name):
-        """Function to create a new organization"""
+        """Create a new organization."""
         return self.client.organizations_api().create_organization(name=name)
 
     def delete_organization(self, org_id):
-        """Function to delete organization by organization id"""
+        """Delete an organization by ID."""
         return self.client.organizations_api().delete_organization(org_id=org_id)
 
     def create_bucket(self, bucket_name, description, org_id, retention_rules=None):
-        """Function to create a bucket for an organization"""
+        """Create a bucket for an organization."""
         return self.client.buckets_api().create_bucket(
             bucket_name=bucket_name, description=description, org_id=org_id, retention_rules=None
         )
 
     def find_bucket_id_by_name(self, bucket_name):
-        """Function to get bucket id by name."""
+        """Get bucket ID by name."""
         bucket = self.client.buckets_api().find_bucket_by_name(bucket_name)
 
         return "" if bucket is None else bucket.id
 
     def delete_bucket(self, bucket_name):
-        """Function to delete bucket by bucket name."""
+        """Delete bucket by name."""
         bucket = self.find_bucket_id_by_name(bucket_name)
         return self.client.buckets_api().delete_bucket(bucket)
```

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/operators/__init__.py` & `apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/airflow/providers/influxdb/operators/influxdb.py` & `apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/operators/influxdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class InfluxDBOperator(BaseOperator):
     """
-    Executes sql code in a specific InfluxDB database
+    Executes sql code in a specific InfluxDB database.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:InfluxDBOperator`
 
     :param sql: the sql code to be executed. Can receive a str representing a
         sql statement
```

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/apache_airflow_providers_influxdb.egg-info/PKG-INFO` & `apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-influxdb
-Version: 2.2.0rc2
+Version: 2.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-influxdb package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.1/
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
 
 
 Package ``apache-airflow-providers-influxdb``
 
-Release: ``2.2.0rc2``
+Release: ``2.2.1rc1``
 
 
 `InfluxDB <https://www.influxdata.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``influxdb`` provider. All classes for this provider package
 are in ``airflow.providers.influxdb`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-influxdb``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
@@ -111,14 +111,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+2.2.1
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
+   * ``Replace spelling directive with spelling:word-list (#31752)``
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 2.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/apache_airflow_providers_influxdb.egg-info/SOURCES.txt` & `apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/pyproject.toml` & `apache-airflow-providers-influxdb-2.2.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/setup.cfg` & `apache-airflow-providers-influxdb-2.2.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.1/
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
 	influxdb-client>=1.19.0
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.influxdb.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.influxdb
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-influxdb-2.2.0rc2/setup.py` & `apache-airflow-providers-influxdb-2.2.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-influxdb package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "2.2.0"
+version = "2.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-influxdb setup."""
     setup(
         version=version,
         extras_require={},
```

