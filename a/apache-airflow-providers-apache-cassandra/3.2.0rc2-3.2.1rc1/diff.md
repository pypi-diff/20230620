# Comparing `tmp/apache-airflow-providers-apache-cassandra-3.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-apache-cassandra-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-cassandra-3.2.0rc2.tar", last modified: Fri May 19 17:51:32 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-cassandra-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:08 2023, max compression
```

## Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2.tar` & `apache-airflow-providers-apache-cassandra-3.2.1rc1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:31.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10801 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9244 2023-05-19 17:51:31.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/
--rw-r--r--   0 root         (0) root         (0)     1541 2023-05-19 11:59:54.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2778 2023-05-19 17:51:31.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7870 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/hooks/cassandra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/sensors/record.py
--rw-r--r--   0 root         (0) root         (0)     2543 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/sensors/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/apache_airflow_providers_apache_cassandra.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10801 2023-05-19 17:51:31.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/apache_airflow_providers_apache_cassandra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      897 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/apache_airflow_providers_apache_cassandra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/apache_airflow_providers_apache_cassandra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/apache_airflow_providers_apache_cassandra.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:31.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/apache_airflow_providers_apache_cassandra.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/apache_airflow_providers_apache_cassandra.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/apache_airflow_providers_apache_cassandra.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1914 2023-05-19 17:51:32.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1698 2023-05-19 17:51:31.000000 apache-airflow-providers-apache-cassandra-3.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.477367 apache-airflow-providers-apache-cassandra-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:07.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11149 2023-06-20 11:41:08.478418 apache-airflow-providers-apache-cassandra-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9591 2023-06-20 11:41:07.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.398358 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.399560 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.400829 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.432494 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-06-20 11:41:07.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.438338 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7874 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/hooks/cassandra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.446914 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/record.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.475004 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11149 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      897 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-06-20 11:41:08.480313 apache-airflow-providers-apache-cassandra-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-20 11:41:07.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/LICENSE` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/MANIFEST.in` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/PKG-INFO` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-cassandra
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-cassandra package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.1/
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
 
 
 Package ``apache-airflow-providers-apache-cassandra``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Apache Cassandra <http://cassandra.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.cassandra`` provider. All classes for this provider package
 are in ``airflow.providers.apache.cassandra`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-cassandra``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ====================  ==================
 PIP package           Version required
 ====================  ==================
@@ -109,14 +109,29 @@
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
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/README.rst` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-cassandra``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Apache Cassandra <http://cassandra.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.cassandra`` provider. All classes for this provider package
 are in ``airflow.providers.apache.cassandra`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-cassandra``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ====================  ==================
 PIP package           Version required
 ====================  ==================
@@ -76,14 +76,29 @@
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
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/__init__.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/__init__.py`

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

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/get_provider_info.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-cassandra",
         "name": "Apache Cassandra",
         "description": "`Apache Cassandra <http://cassandra.apache.org/>`__.\n",
         "suspended": False,
         "versions": [
+            "3.2.1",
             "3.2.0",
             "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.1.3",
             "2.1.2",
             "2.1.1",
```

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/hooks/__init__.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/hooks/cassandra.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/hooks/cassandra.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from airflow.utils.log.logging_mixin import LoggingMixin
 
 Policy = Union[DCAwareRoundRobinPolicy, RoundRobinPolicy, TokenAwarePolicy, WhiteListRoundRobinPolicy]
 
 
 class CassandraHook(BaseHook, LoggingMixin):
     """
-    Hook used to interact with Cassandra
+    Hook used to interact with Cassandra.
 
     Contact points can be specified as a comma-separated string in the 'hosts'
     field of the connection.
 
     Port can be specified in the port field of the connection.
 
     If SSL is enabled in Cassandra, pass in a dict in the extra field as kwargs for
@@ -121,15 +121,15 @@
             conn_config["protocol_version"] = protocol_version
 
         self.cluster = Cluster(**conn_config)
         self.keyspace = conn.schema
         self.session = None
 
     def get_conn(self) -> Session:
-        """Returns a cassandra Session object"""
+        """Returns a cassandra Session object."""
         if self.session and not self.session.is_shutdown:
             return self.session
         self.session = self.cluster.connect(self.keyspace)
         return self.session
 
     def get_cluster(self) -> Cluster:
         """Returns Cassandra cluster."""
@@ -173,28 +173,28 @@
             return TokenAwarePolicy(child_policy)
 
         # Fallback to default RoundRobinPolicy
         return RoundRobinPolicy()
 
     def table_exists(self, table: str) -> bool:
         """
-        Checks if a table exists in Cassandra
+        Checks if a table exists in Cassandra.
 
         :param table: Target Cassandra table.
                       Use dot notation to target a specific keyspace.
         """
         keyspace = self.keyspace
         if "." in table:
             keyspace, table = table.split(".", 1)
         cluster_metadata = self.get_conn().cluster.metadata
         return keyspace in cluster_metadata.keyspaces and table in cluster_metadata.keyspaces[keyspace].tables
 
     def record_exists(self, table: str, keys: dict[str, str]) -> bool:
         """
-        Checks if a record exists in Cassandra
+        Checks if a record exists in Cassandra.
 
         :param table: Target Cassandra table.
                       Use dot notation to target a specific keyspace.
         :param keys: The keys and their values to check the existence.
         """
         keyspace = self.keyspace
         if "." in table:
```

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/sensors/__init__.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/sensors/record.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/record.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/airflow/providers/apache/cassandra/sensors/table.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/table.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/apache_airflow_providers_apache_cassandra.egg-info/PKG-INFO` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-cassandra
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-cassandra package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.1/
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
 
 
 Package ``apache-airflow-providers-apache-cassandra``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Apache Cassandra <http://cassandra.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.cassandra`` provider. All classes for this provider package
 are in ``airflow.providers.apache.cassandra`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-cassandra``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ====================  ==================
 PIP package           Version required
 ====================  ==================
@@ -109,14 +109,29 @@
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
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/apache_airflow_providers_apache_cassandra.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/pyproject.toml` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/setup.cfg` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.1/
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
 	cassandra-driver>=3.13.0
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.cassandra.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.cassandra
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-cassandra-3.2.0rc2/setup.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-cassandra package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.0"
+version = "3.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-cassandra setup."""
     setup(
         version=version,
         extras_require={},
```
