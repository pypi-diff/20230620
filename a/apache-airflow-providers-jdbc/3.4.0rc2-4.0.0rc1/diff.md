# Comparing `tmp/apache-airflow-providers-jdbc-3.4.0rc2.tar.gz` & `tmp/apache-airflow-providers-jdbc-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-jdbc-3.4.0rc2.tar", last modified: Fri May 19 17:52:45 2023, max compression
+gzip compressed data, was "apache-airflow-providers-jdbc-4.0.0rc1.tar", last modified: Tue Jun 20 11:42:23 2023, max compression
```

## Comparing `apache-airflow-providers-jdbc-3.4.0rc2.tar` & `apache-airflow-providers-jdbc-4.0.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-jdbc-3.4.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:44.000000 apache-airflow-providers-jdbc-3.4.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-jdbc-3.4.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13011 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11463 2023-05-19 17:52:44.000000 apache-airflow-providers-jdbc-3.4.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-05-19 12:12:57.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2811 2023-05-19 17:52:44.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4254 2023-02-24 18:43:53.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/hooks/jdbc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-05-03 19:47:07.000000 apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/operators/jdbc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13011 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      143 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-jdbc-3.4.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1884 2023-05-19 17:52:45.000000 apache-airflow-providers-jdbc-3.4.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-19 17:52:44.000000 apache-airflow-providers-jdbc-3.4.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.924525 apache-airflow-providers-jdbc-4.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-jdbc-4.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:22.000000 apache-airflow-providers-jdbc-4.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-jdbc-4.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14107 2023-06-20 11:42:23.925592 apache-airflow-providers-jdbc-4.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12558 2023-06-20 11:42:22.000000 apache-airflow-providers-jdbc-4.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.852378 apache-airflow-providers-jdbc-4.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.853627 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.885976 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-06-20 11:42:22.000000 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.891740 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7023 2023-06-17 16:45:00.000000 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/hooks/jdbc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.897447 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/operators/jdbc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.921741 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14107 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      143 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-jdbc-4.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-06-20 11:42:23.927528 apache-airflow-providers-jdbc-4.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-20 11:42:22.000000 apache-airflow-providers-jdbc-4.0.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/LICENSE` & `apache-airflow-providers-jdbc-4.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/MANIFEST.in` & `apache-airflow-providers-jdbc-4.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/PKG-INFO` & `apache-airflow-providers-jdbc-4.0.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jdbc
-Version: 3.4.0rc2
+Version: 4.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-jdbc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jdbc/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jdbc/4.0.0/
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
 
 
 Package ``apache-airflow-providers-jdbc``
 
-Release: ``3.4.0rc2``
+Release: ``4.0.0rc1``
 
 
 `Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``jdbc`` provider. All classes for this provider package
 are in ``airflow.providers.jdbc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-jdbc/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-jdbc/4.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-jdbc``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -130,14 +130,37 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.0.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+To configure driver parameters (driver path and driver class), you can use the following methods:
+
+1. Supply them as constructor arguments when instantiating the hook.
+2. Set the "driver_path" and/or "driver_class" parameters in the "hook_params" dictionary when creating the hook using SQL operators.
+3. Set the "driver_path" and/or "driver_class" extra in the connection and correspondingly enable the "allow_driver_path_in_extra" and/or "allow_driver_class_in_extra" options in the "providers.jdbc" section of the Airflow configuration.
+4. Patch the "JdbcHook.default_driver_path" and/or "JdbcHook.default_driver_class" values in the "local_settings.py" file.
+
+* ``Restrict direct usage of driver params via extras for JDBC connection (#31849)``
+
+.. Review and move the new changes to one of the sections above:
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/README.rst` & `apache-airflow-providers-jdbc-4.0.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-jdbc``
 
-Release: ``3.4.0rc2``
+Release: ``4.0.0rc1``
 
 
 `Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``jdbc`` provider. All classes for this provider package
 are in ``airflow.providers.jdbc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-jdbc/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-jdbc/4.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-jdbc``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -96,14 +96,37 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.0.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+To configure driver parameters (driver path and driver class), you can use the following methods:
+
+1. Supply them as constructor arguments when instantiating the hook.
+2. Set the "driver_path" and/or "driver_class" parameters in the "hook_params" dictionary when creating the hook using SQL operators.
+3. Set the "driver_path" and/or "driver_class" extra in the connection and correspondingly enable the "allow_driver_path_in_extra" and/or "allow_driver_class_in_extra" options in the "providers.jdbc" section of the Airflow configuration.
+4. Patch the "JdbcHook.default_driver_path" and/or "JdbcHook.default_driver_class" values in the "local_settings.py" file.
+
+* ``Restrict direct usage of driver params via extras for JDBC connection (#31849)``
+
+.. Review and move the new changes to one of the sections above:
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/__init__.py` & `apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.4.0"
+__version__ = "4.0.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/get_provider_info.py` & `apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-jdbc",
         "name": "Java Database Connectivity (JDBC)",
         "description": "`Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__\n",
         "suspended": False,
         "versions": [
+            "4.0.0",
             "3.4.0",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.1.3",
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/hooks/__init__.py` & `apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/operators/__init__.py` & `apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/airflow/providers/jdbc/operators/jdbc.py` & `apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/operators/jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/PKG-INFO` & `apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jdbc
-Version: 3.4.0rc2
+Version: 4.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-jdbc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jdbc/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jdbc/4.0.0/
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
 
 
 Package ``apache-airflow-providers-jdbc``
 
-Release: ``3.4.0rc2``
+Release: ``4.0.0rc1``
 
 
 `Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``jdbc`` provider. All classes for this provider package
 are in ``airflow.providers.jdbc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-jdbc/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-jdbc/4.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-jdbc``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -130,14 +130,37 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.0.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+To configure driver parameters (driver path and driver class), you can use the following methods:
+
+1. Supply them as constructor arguments when instantiating the hook.
+2. Set the "driver_path" and/or "driver_class" parameters in the "hook_params" dictionary when creating the hook using SQL operators.
+3. Set the "driver_path" and/or "driver_class" extra in the connection and correspondingly enable the "allow_driver_path_in_extra" and/or "allow_driver_class_in_extra" options in the "providers.jdbc" section of the Airflow configuration.
+4. Patch the "JdbcHook.default_driver_path" and/or "JdbcHook.default_driver_class" values in the "local_settings.py" file.
+
+* ``Restrict direct usage of driver params via extras for JDBC connection (#31849)``
+
+.. Review and move the new changes to one of the sections above:
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/apache_airflow_providers_jdbc.egg-info/SOURCES.txt` & `apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/pyproject.toml` & `apache-airflow-providers-jdbc-4.0.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/setup.cfg` & `apache-airflow-providers-jdbc-4.0.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-jdbc/3.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-jdbc/4.0.0/
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
 	provider_info=airflow.providers.jdbc.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.jdbc
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-jdbc-3.4.0rc2/setup.py` & `apache-airflow-providers-jdbc-4.0.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-jdbc package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.0"
+version = "4.0.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-jdbc setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

