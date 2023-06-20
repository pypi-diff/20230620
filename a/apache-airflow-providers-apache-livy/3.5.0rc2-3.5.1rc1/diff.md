# Comparing `tmp/apache-airflow-providers-apache-livy-3.5.0rc2.tar.gz` & `tmp/apache-airflow-providers-apache-livy-3.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-livy-3.5.0rc2.tar", last modified: Fri May 19 17:51:48 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-livy-3.5.1rc1.tar", last modified: Tue Jun 20 11:41:24 2023, max compression
```

## Comparing `apache-airflow-providers-apache-livy-3.5.0rc2.tar` & `apache-airflow-providers-apache-livy-3.5.1rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-livy-3.5.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:47.000000 apache-airflow-providers-apache-livy-3.5.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-livy-3.5.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12386 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10823 2023-05-19 17:51:47.000000 apache-airflow-providers-apache-livy-3.5.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-19 12:02:21.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3070 2023-05-19 17:51:47.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31534 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/hooks/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8738 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/operators/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2574 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/sensors/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6238 2023-04-24 21:04:25.000000 apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/triggers/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/apache_airflow_providers_apache_livy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12386 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/apache_airflow_providers_apache_livy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      971 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/apache_airflow_providers_apache_livy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/apache_airflow_providers_apache_livy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/apache_airflow_providers_apache_livy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/apache_airflow_providers_apache_livy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/apache_airflow_providers_apache_livy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-apache-livy-3.5.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1907 2023-05-19 17:51:48.000000 apache-airflow-providers-apache-livy-3.5.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1709 2023-05-19 17:51:47.000000 apache-airflow-providers-apache-livy-3.5.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.829920 apache-airflow-providers-apache-livy-3.5.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:23.000000 apache-airflow-providers-apache-livy-3.5.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13010 2023-06-20 11:41:24.831002 apache-airflow-providers-apache-livy-3.5.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11446 2023-06-20 11:41:23.000000 apache-airflow-providers-apache-livy-3.5.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.735007 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.736232 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.737260 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.773034 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-06-20 11:41:23.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.778826 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31553 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.785185 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9572 2023-06-05 12:50:36.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.793079 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.798737 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.827293 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13010 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      971 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-livy-3.5.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1908 2023-06-20 11:41:24.833029 apache-airflow-providers-apache-livy-3.5.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-20 11:41:23.000000 apache-airflow-providers-apache-livy-3.5.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/LICENSE` & `apache-airflow-providers-apache-livy-3.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/MANIFEST.in` & `apache-airflow-providers-apache-livy-3.5.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/PKG-INFO` & `apache-airflow-providers-apache-livy-3.5.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-livy
-Version: 3.5.0rc2
+Version: 3.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-livy package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.1/
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
 Provides-Extra: http
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -49,38 +49,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-livy``
 
-Release: ``3.5.0rc2``
+Release: ``3.5.1rc1``
 
 
 `Apache Livy <https://livy.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.livy`` provider. All classes for this provider package
 are in ``airflow.providers.apache.livy`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-livy``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -131,14 +131,37 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.5.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Push Spark appId to XCOM for LivyOperator with deferrable mode (#31201)``
+
+Misc
+~~~~
+
+* ``Optimize deferred mode execution (#31685)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.5.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/README.rst` & `apache-airflow-providers-apache-livy-3.5.1rc1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-livy``
 
-Release: ``3.5.0rc2``
+Release: ``3.5.1rc1``
 
 
 `Apache Livy <https://livy.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.livy`` provider. All classes for this provider package
 are in ``airflow.providers.apache.livy`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-livy``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -97,14 +97,37 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.5.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Push Spark appId to XCOM for LivyOperator with deferrable mode (#31201)``
+
+Misc
+~~~~
+
+* ``Optimize deferred mode execution (#31685)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.5.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/__init__.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.5.0"
+__version__ = "3.5.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/get_provider_info.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-livy",
         "name": "Apache Livy",
         "description": "`Apache Livy <https://livy.apache.org/>`__\n",
         "suspended": False,
         "versions": [
+            "3.5.1",
             "3.5.0",
             "3.4.0",
             "3.3.0",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.2.3",
@@ -72,15 +73,15 @@
                 "integration-name": "Apache Livy",
                 "python-modules": ["airflow.providers.apache.livy.hooks.livy"],
             }
         ],
         "triggers": [
             {
                 "integration-name": "Apache Livy",
-                "class-names": ["airflow.providers.apache.livy.triggers.livy.LivyTrigger"],
+                "python-modules": ["airflow.providers.apache.livy.triggers.livy"],
             }
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.apache.livy.hooks.livy.LivyHook",
                 "connection-type": "livy",
             }
```

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/hooks/__init__.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/hooks/livy.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/livy.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from airflow.exceptions import AirflowException
 from airflow.models import Connection
 from airflow.providers.http.hooks.http import HttpAsyncHook, HttpHook
 from airflow.utils.log.logging_mixin import LoggingMixin
 
 
 class BatchState(Enum):
-    """Batch session states"""
+    """Batch session states."""
 
     NOT_STARTED = "not_started"
     STARTING = "starting"
     RUNNING = "running"
     IDLE = "idle"
     BUSY = "busy"
     SHUTTING_DOWN = "shutting_down"
@@ -88,15 +88,15 @@
         self.extra_headers = extra_headers or {}
         self.extra_options = extra_options or {}
         if auth_type:
             self.auth_type = auth_type
 
     def get_conn(self, headers: dict[str, Any] | None = None) -> Any:
         """
-        Returns http session for use with requests
+        Returns http session for use with requests.
 
         :param headers: additional headers to be passed through as a dictionary
         :return: requests session
         """
         tmp_headers = self._def_headers.copy()  # setting default headers
         if headers:
             tmp_headers.update(headers)
@@ -107,15 +107,15 @@
         endpoint: str,
         method: str = "GET",
         data: Any | None = None,
         headers: dict[str, Any] | None = None,
         retry_args: dict[str, Any] | None = None,
     ) -> Any:
         """
-        Wrapper for HttpHook, allows to change method on the same HttpHook
+        Wrapper for HttpHook, allows to change method on the same HttpHook.
 
         :param method: http method
         :param endpoint: endpoint
         :param data: request payload
         :param headers: headers
         :param retry_args: Arguments which define the retry behaviour.
             See Tenacity documentation at https://github.com/jd/tenacity
@@ -142,15 +142,15 @@
 
         finally:
             self.method = back_method
         return result
 
     def post_batch(self, *args: Any, **kwargs: Any) -> int:
         """
-        Perform request to submit batch
+        Perform request to submit batch.
 
         :return: batch session id
         """
         batch_submit_body = json.dumps(self.build_post_batch_body(*args, **kwargs))
 
         if self.base_url is None:
             # need to init self.base_url
@@ -175,15 +175,15 @@
             raise AirflowException("Unable to parse the batch session id")
         self.log.info("Batch submitted with session id: %d", batch_id)
 
         return batch_id
 
     def get_batch(self, session_id: int | str) -> dict:
         """
-        Fetch info about the specified batch
+        Fetch info about the specified batch.
 
         :param session_id: identifier of the batch sessions
         :return: response body
         """
         self._validate_session_id(session_id)
 
         self.log.debug("Fetching info for batch session %d", session_id)
@@ -197,15 +197,15 @@
                 f"Unable to fetch batch with id: {session_id}. Message: {err.response.text}"
             )
 
         return response.json()
 
     def get_batch_state(self, session_id: int | str, retry_args: dict[str, Any] | None = None) -> BatchState:
         """
-        Fetch the state of the specified batch
+        Fetch the state of the specified batch.
 
         :param session_id: identifier of the batch sessions
         :param retry_args: Arguments which define the retry behaviour.
             See Tenacity documentation at https://github.com/jd/tenacity
         :return: batch state
         """
         self._validate_session_id(session_id)
@@ -226,15 +226,15 @@
         jresp = response.json()
         if "state" not in jresp:
             raise AirflowException(f"Unable to get state for batch with id: {session_id}")
         return BatchState(jresp["state"])
 
     def delete_batch(self, session_id: int | str) -> dict:
         """
-        Delete the specified batch
+        Delete the specified batch.
 
         :param session_id: identifier of the batch sessions
         :return: response body
         """
         self._validate_session_id(session_id)
 
         self.log.info("Deleting batch session %d", session_id)
@@ -251,14 +251,15 @@
             )
 
         return response.json()
 
     def get_batch_logs(self, session_id: int | str, log_start_position, log_batch_size) -> dict:
         """
         Gets the session logs for a specified batch.
+
         :param session_id: identifier of the batch sessions
         :param log_start_position: Position from where to pull the logs
         :param log_batch_size: Number of lines to pull in one batch
 
         :return: response body
         """
         self._validate_session_id(session_id)
@@ -274,15 +275,15 @@
                 f"Could not fetch the logs for batch with session id: {session_id}. "
                 f"Message: {err.response.text}"
             )
         return response.json()
 
     def dump_batch_logs(self, session_id: int | str) -> None:
         """
-        Dumps the session logs for a specified batch
+        Dumps the session logs for a specified batch.
 
         :param session_id: identifier of the batch sessions
         :return: response body
         """
         self.log.info("Fetching the logs for batch session with id: %d", session_id)
         log_start_line = 0
         log_total_lines = 0
@@ -296,37 +297,37 @@
             log_lines = self._parse_request_response(response, "log")
             for log_line in log_lines:
                 self.log.info(log_line)
 
     @staticmethod
     def _validate_session_id(session_id: int | str) -> None:
         """
-        Validate session id is a int
+        Validate session id is a int.
 
         :param session_id: session id
         """
         try:
             int(session_id)
         except (TypeError, ValueError):
             raise TypeError("'session_id' must be an integer")
 
     @staticmethod
     def _parse_post_response(response: dict[Any, Any]) -> int | None:
         """
-        Parse batch response for batch id
+        Parse batch response for batch id.
 
         :param response: response body
         :return: session id
         """
         return response.get("id")
 
     @staticmethod
     def _parse_request_response(response: dict[Any, Any], parameter):
         """
-        Parse batch response for batch id
+        Parse batch response for batch id.
 
         :param response: response body
         :return: value of parameter
         """
         return response.get(parameter, [])
 
     @staticmethod
@@ -450,15 +451,15 @@
             if any(True for k, v in conf.items() if not (v and isinstance(v, str) or isinstance(v, int))):
                 raise ValueError("'conf' values must be either strings or ints")
         return True
 
 
 class LivyAsyncHook(HttpAsyncHook, LoggingMixin):
     """
-    Hook for Apache Livy through the REST API asynchronously
+    Hook for Apache Livy through the REST API asynchronously.
 
     :param livy_conn_id: reference to a pre-defined Livy Connection.
     :param extra_options: A dictionary of options passed to Livy.
     :param extra_headers: A dictionary of headers passed to the HTTP request to livy.
 
     .. seealso::
         For more details refer to the Apache Livy API reference:
@@ -493,15 +494,15 @@
         self,
         endpoint: str | None = None,
         data: dict[str, Any] | str | None = None,
         headers: dict[str, Any] | None = None,
         extra_options: dict[str, Any] | None = None,
     ) -> Any:
         """
-        Performs an asynchronous HTTP request call
+        Performs an asynchronous HTTP request call.
 
         :param endpoint: the endpoint to be called i.e. resource/v1/query?
         :param data: payload to be uploaded or request parameters
         :param headers: additional headers to be passed through as a dictionary
         :param extra_options: Additional kwargs to pass when creating a request.
             For example, ``run(json=obj)`` is passed as ``aiohttp.ClientSession().get(json=obj)``
         """
@@ -586,15 +587,15 @@
         self,
         endpoint: str,
         method: str = "GET",
         data: Any | None = None,
         headers: dict[str, Any] | None = None,
     ) -> Any:
         """
-        Wrapper for HttpAsyncHook, allows to change method on the same HttpAsyncHook
+        Wrapper for HttpAsyncHook, allows to change method on the same HttpAsyncHook.
 
         :param method: http method
         :param endpoint: endpoint
         :param data: request payload
         :param headers: headers
         :return: http response
         """
@@ -657,15 +658,15 @@
         if result["status"] == "error":
             self.log.info(result)
             return {"response": result["response"], "status": "error"}
         return {"response": result["response"], "status": "success"}
 
     async def dump_batch_logs(self, session_id: int | str) -> Any:
         """
-        Dumps the session logs for a specified batch asynchronously
+        Dumps the session logs for a specified batch asynchronously.
 
         :param session_id: identifier of the batch sessions
         :return: response body
         """
         self.log.info("Fetching the logs for batch session with id: %d", session_id)
         log_start_line = 0
         log_total_lines = 0
@@ -683,37 +684,37 @@
             else:
                 self.log.info(result["response"])
                 return result["response"]
 
     @staticmethod
     def _validate_session_id(session_id: int | str) -> None:
         """
-        Validate session id is a int
+        Validate session id is a int.
 
         :param session_id: session id
         """
         try:
             int(session_id)
         except (TypeError, ValueError):
             raise TypeError("'session_id' must be an integer")
 
     @staticmethod
     def _parse_post_response(response: dict[Any, Any]) -> Any:
         """
-        Parse batch response for batch id
+        Parse batch response for batch id.
 
         :param response: response body
         :return: session id
         """
         return response.get("id")
 
     @staticmethod
     def _parse_request_response(response: dict[Any, Any], parameter: Any) -> Any:
         """
-        Parse batch response for batch id
+        Parse batch response for batch id.
 
         :param response: response body
         :return: value of parameter
         """
         return response.get(parameter)
 
     @staticmethod
```

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/operators/__init__.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/operators/livy.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/livy.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,26 +147,38 @@
         # Wait for the job to complete
         if not self.deferrable:
             if self._polling_interval > 0:
                 self.poll_for_termination(self._batch_id)
             context["ti"].xcom_push(key="app_id", value=self.get_hook().get_batch(self._batch_id)["appId"])
             return self._batch_id
 
-        self.defer(
-            timeout=self.execution_timeout,
-            trigger=LivyTrigger(
-                batch_id=self._batch_id,
-                spark_params=self.spark_params,
-                livy_conn_id=self._livy_conn_id,
-                polling_interval=self._polling_interval,
-                extra_options=self._extra_options,
-                extra_headers=self._extra_headers,
-            ),
-            method_name="execute_complete",
-        )
+        hook = self.get_hook()
+        state = hook.get_batch_state(self._batch_id, retry_args=self.retry_args)
+        self.log.debug("Batch with id %s is in state: %s", self._batch_id, state.value)
+        if state not in hook.TERMINAL_STATES:
+            self.defer(
+                timeout=self.execution_timeout,
+                trigger=LivyTrigger(
+                    batch_id=self._batch_id,
+                    spark_params=self.spark_params,
+                    livy_conn_id=self._livy_conn_id,
+                    polling_interval=self._polling_interval,
+                    extra_options=self._extra_options,
+                    extra_headers=self._extra_headers,
+                ),
+                method_name="execute_complete",
+            )
+        else:
+            self.log.info("Batch with id %s terminated with state: %s", self._batch_id, state.value)
+            hook.dump_batch_logs(self._batch_id)
+            if state != BatchState.SUCCESS:
+                raise AirflowException(f"Batch {self._batch_id} did not succeed")
+
+            context["ti"].xcom_push(key="app_id", value=self.get_hook().get_batch(self._batch_id)["appId"])
+            return self._batch_id
 
     def poll_for_termination(self, batch_id: int | str) -> None:
         """
         Pool Livy for batch termination.
 
         :param batch_id: id of the batch session to monitor.
         """
@@ -203,8 +215,9 @@
         if event["status"] == "error":
             raise AirflowException(event["response"])
         self.log.info(
             "%s completed with response %s",
             self.task_id,
             event["response"],
         )
+        context["ti"].xcom_push(key="app_id", value=self.get_hook().get_batch(event["batch_id"])["appId"])
         return event["batch_id"]
```

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/sensors/__init__.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/sensors/livy.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/triggers/__init__.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/airflow/providers/apache/livy/triggers/livy.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/livy.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from airflow.providers.apache.livy.hooks.livy import BatchState, LivyAsyncHook
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
 class LivyTrigger(BaseTrigger):
     """
-    Check for the state of a previously submitted job with batch_id
+    Check for the state of a previously submitted job with batch_id.
 
     :param batch_id: Batch job id
     :param spark_params: Spark parameters; for example,
             spark_params = {"file": "test/pi.py", "class_name": "org.apache.spark.examples.SparkPi",
             "args": ["/usr/lib/spark/bin/run-example", "SparkPi", "10"],"jars": "command-runner.jar",
             "driver_cores": 1, "executor_cores": 4,"num_executors": 1}
     :param livy_conn_id: reference to a pre-defined Livy Connection.
@@ -75,18 +75,18 @@
                 "extra_options": self._extra_options,
                 "extra_headers": self._extra_headers,
                 "livy_hook_async": self._livy_hook_async,
             },
         )
 
     async def run(self) -> AsyncIterator[TriggerEvent]:
-        """
-        Checks if the _polling_interval > 0, in that case it pools Livy for
-        batch termination asynchronously.
-        else returns the success response
+        """Run the trigger.
+
+        If ``_polling_interval > 0``, this pools Livy for batch termination
+        asynchronously. Otherwise the success response is created immediately.
         """
         try:
             if self._polling_interval > 0:
                 response = await self.poll_for_termination(self._batch_id)
                 yield TriggerEvent(response)
             yield TriggerEvent(
                 {
```

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/apache_airflow_providers_apache_livy.egg-info/PKG-INFO` & `apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-livy
-Version: 3.5.0rc2
+Version: 3.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-livy package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.1/
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
 Provides-Extra: http
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -49,38 +49,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-livy``
 
-Release: ``3.5.0rc2``
+Release: ``3.5.1rc1``
 
 
 `Apache Livy <https://livy.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.livy`` provider. All classes for this provider package
 are in ``airflow.providers.apache.livy`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-livy``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -131,14 +131,37 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.5.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Push Spark appId to XCOM for LivyOperator with deferrable mode (#31201)``
+
+Misc
+~~~~
+
+* ``Optimize deferred mode execution (#31685)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.5.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/pyproject.toml` & `apache-airflow-providers-apache-livy-3.5.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/setup.cfg` & `apache-airflow-providers-apache-livy-3.5.1rc1/setup.cfg`

 * *Files 5% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.1/
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
 	aiohttp
 	apache-airflow-providers-http
@@ -55,10 +55,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.livy.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.livy
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-livy-3.5.0rc2/setup.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-livy package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.5.0"
+version = "3.5.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-livy setup."""
     setup(
         version=version,
         extras_require={"http": ["apache-airflow-providers-http"]},
```

