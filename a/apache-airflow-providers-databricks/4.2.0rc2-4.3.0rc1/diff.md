# Comparing `tmp/apache-airflow-providers-databricks-4.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-databricks-4.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-databricks-4.2.0rc2.tar", last modified: Fri May 19 17:52:09 2023, max compression
+gzip compressed data, was "apache-airflow-providers-databricks-4.3.0rc1.tar", last modified: Tue Jun 20 11:41:47 2023, max compression
```

## Comparing `apache-airflow-providers-databricks-4.2.0rc2.tar` & `apache-airflow-providers-databricks-4.3.0rc1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:08.000000 apache-airflow-providers-databricks-4.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    20261 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18695 2023-05-19 17:52:08.000000 apache-airflow-providers-databricks-4.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-05-19 12:04:45.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5547 2023-05-19 17:52:08.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16761 2023-05-12 08:38:07.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/databricks.py
--rw-r--r--   0 root         (0) root         (0)    26704 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/databricks_base.py
--rw-r--r--   0 root         (0) root         (0)     9278 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33394 2023-05-04 19:17:30.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/databricks.py
--rw-r--r--   0 root         (0) root         (0)    13226 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/databricks_repos.py
--rw-r--r--   0 root         (0) root         (0)    16793 2023-05-12 08:38:07.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-13 08:25:21.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10015 2023-05-15 07:14:11.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/databricks_partition.py
--rw-r--r--   0 root         (0) root         (0)     5558 2023-04-13 08:25:21.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3997 2023-04-24 21:04:25.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/triggers/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2909 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/utils/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20261 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1362 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-databricks-4.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1981 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1715 2023-05-19 17:52:08.000000 apache-airflow-providers-databricks-4.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.334610 apache-airflow-providers-databricks-4.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:46.000000 apache-airflow-providers-databricks-4.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    21143 2023-06-20 11:41:47.335992 apache-airflow-providers-databricks-4.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    19576 2023-06-20 11:41:46.000000 apache-airflow-providers-databricks-4.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.212152 apache-airflow-providers-databricks-4.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.213485 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.255680 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-20 11:01:09.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5506 2023-06-20 11:41:46.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.269076 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16771 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    26695 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks_base.py
+-rw-r--r--   0 root         (0) root         (0)     9359 2023-06-17 16:45:00.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.281889 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33383 2023-06-19 10:14:19.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    13212 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks_repos.py
+-rw-r--r--   0 root         (0) root         (0)    16994 2023-06-17 16:45:00.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.290943 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10000 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/databricks_partition.py
+-rw-r--r--   0 root         (0) root         (0)     5543 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.297042 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2023-06-18 13:29:11.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.303088 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.330922 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    21143 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      200 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-databricks-4.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-06-20 11:41:47.340065 apache-airflow-providers-databricks-4.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-06-20 11:41:46.000000 apache-airflow-providers-databricks-4.3.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/LICENSE` & `apache-airflow-providers-databricks-4.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/MANIFEST.in` & `apache-airflow-providers-databricks-4.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/PKG-INFO` & `apache-airflow-providers-databricks-4.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.2.0rc2
+Version: 4.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.0/
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
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.2.0rc2``
+Release: ``4.3.0rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-databricks``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ===================
 PIP package                              Version required
 =======================================  ===================
@@ -132,14 +132,44 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.3.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* ``add a return when the event is yielded in a loop to stop the execution (#31985)``
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix type annotation (#31888)``
+* ``Fix Databricks SQL operator serialization (#31780)``
+* ``Making Databricks run related multi-query string in one session again (#31898) (#31899)``
+
+Misc
+~~~~
+* ``Remove return statement after yield from triggers class (#31703)``
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 4.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/README.rst` & `apache-airflow-providers-databricks-4.3.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.2.0rc2``
+Release: ``4.3.0rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-databricks``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ===================
 PIP package                              Version required
 =======================================  ===================
@@ -98,14 +98,44 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.3.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* ``add a return when the event is yielded in a loop to stop the execution (#31985)``
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix type annotation (#31888)``
+* ``Fix Databricks SQL operator serialization (#31780)``
+* ``Making Databricks run related multi-query string in one session again (#31898) (#31899)``
+
+Misc
+~~~~
+* ``Remove return statement after yield from triggers class (#31703)``
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 4.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/__init__.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.2.0"
+__version__ = "4.3.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/get_provider_info.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-databricks",
         "name": "Databricks",
         "description": "`Databricks <https://databricks.com/>`__\n",
         "suspended": False,
         "versions": [
+            "4.3.0",
             "4.2.0",
             "4.1.0",
             "4.0.1",
             "4.0.0",
             "3.4.0",
             "3.3.0",
             "3.2.0",
@@ -117,17 +118,15 @@
                 "integration-name": "Databricks SQL",
                 "python-modules": ["airflow.providers.databricks.hooks.databricks_sql"],
             },
         ],
         "triggers": [
             {
                 "integration-name": "Databricks",
-                "class-names": [
-                    "airflow.providers.databricks.triggers.databricks.DatabricksExecutionTrigger"
-                ],
+                "python-modules": ["airflow.providers.databricks.triggers.databricks"],
             }
         ],
         "sensors": [
             {
                 "integration-name": "Databricks",
                 "python-modules": [
                     "airflow.providers.databricks.sensors.databricks_sql",
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/__init__.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/databricks.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                     "guide for troubleshooting information"
                 ).format(self.life_cycle_state)
             )
         return self.life_cycle_state in ("TERMINATED", "SKIPPED", "INTERNAL_ERROR")
 
     @property
     def is_successful(self) -> bool:
-        """True if the result state is SUCCESS"""
+        """True if the result state is SUCCESS."""
         return self.result_state == "SUCCESS"
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, RunState):
             return NotImplemented
         return (
             self.life_cycle_state == other.life_cycle_state
@@ -219,14 +219,15 @@
         json = {"run_id": run_id}
         response = self._do_api_call(GET_RUN_ENDPOINT, json)
         return response["run_page_url"]
 
     async def a_get_run_page_url(self, run_id: int) -> str:
         """
         Async version of `get_run_page_url()`.
+
         :param run_id: id of the run
         :return: URL of the run page
         """
         json = {"run_id": run_id}
         response = await self._a_do_api_call(GET_RUN_ENDPOINT, json)
         return response["run_page_url"]
 
@@ -260,14 +261,15 @@
         response = self._do_api_call(GET_RUN_ENDPOINT, json)
         state = response["state"]
         return RunState(**state)
 
     async def a_get_run_state(self, run_id: int) -> RunState:
         """
         Async version of `get_run_state()`.
+
         :param run_id: id of the run
         :return: state of the run
         """
         json = {"run_id": run_id}
         response = await self._a_do_api_call(GET_RUN_ENDPOINT, json)
         state = response["state"]
         return RunState(**state)
@@ -305,33 +307,33 @@
         run_state_str = (
             f"State: {state.life_cycle_state}. Result: {state.result_state}. {state.state_message}"
         )
         return run_state_str
 
     def get_run_state_lifecycle(self, run_id: int) -> str:
         """
-        Returns the lifecycle state of the run
+        Returns the lifecycle state of the run.
 
         :param run_id: id of the run
         :return: string with lifecycle state
         """
         return self.get_run_state(run_id).life_cycle_state
 
     def get_run_state_result(self, run_id: int) -> str:
         """
-        Returns the resulting state of the run
+        Returns the resulting state of the run.
 
         :param run_id: id of the run
         :return: string with resulting state
         """
         return self.get_run_state(run_id).result_state
 
     def get_run_state_message(self, run_id: int) -> str:
         """
-        Returns the state message for the run
+        Returns the state message for the run.
 
         :param run_id: id of the run
         :return: string with state message
         """
         return self.get_run_state(run_id).state_message
 
     def get_run_output(self, run_id: int) -> dict:
@@ -422,36 +424,36 @@
 
         :param json: json dictionary containing cluster_id and an array of library
         """
         self._do_api_call(UNINSTALL_LIBS_ENDPOINT, json)
 
     def update_repo(self, repo_id: str, json: dict[str, Any]) -> dict:
         """
-        Updates given Databricks Repos
+        Updates given Databricks Repos.
 
         :param repo_id: ID of Databricks Repos
         :param json: payload
         :return: metadata from update
         """
         repos_endpoint = ("PATCH", f"api/2.0/repos/{repo_id}")
         return self._do_api_call(repos_endpoint, json)
 
     def delete_repo(self, repo_id: str):
         """
-        Deletes given Databricks Repos
+        Deletes given Databricks Repos.
 
         :param repo_id: ID of Databricks Repos
         :return:
         """
         repos_endpoint = ("DELETE", f"api/2.0/repos/{repo_id}")
         self._do_api_call(repos_endpoint)
 
     def create_repo(self, json: dict[str, Any]) -> dict:
         """
-        Creates a Databricks Repos
+        Creates a Databricks Repos.
 
         :param json: payload
         :return:
         """
         repos_endpoint = ("POST", "api/2.0/repos")
         return self._do_api_call(repos_endpoint, json)
 
@@ -468,15 +470,15 @@
         except requests_exceptions.HTTPError as e:
             if e.response.status_code != 404:
                 raise e
 
         return None
 
     def test_connection(self) -> tuple[bool, str]:
-        """Test the Databricks connectivity from UI"""
+        """Test the Databricks connectivity from UI."""
         hook = DatabricksHook(databricks_conn_id=self.databricks_conn_id)
         try:
             hook._do_api_call(endpoint_info=SPARK_VERSIONS_ENDPOINT).get("versions")
             status = True
             message = "Connection successfully tested"
         except Exception as e:
             status = False
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/databricks_base.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 `endpoint <https://docs.databricks.com/api/latest/jobs.html#runs-submit>`_.
 """
 from __future__ import annotations
 
 import copy
 import platform
 import time
+from functools import cached_property
 from typing import Any
 from urllib.parse import urlsplit
 
 import aiohttp
 import requests
 from requests import PreparedRequest, exceptions as requests_exceptions
 from requests.auth import AuthBase, HTTPBasicAuth
@@ -41,15 +42,14 @@
     Retrying,
     retry_if_exception,
     stop_after_attempt,
     wait_exponential,
 )
 
 from airflow import __version__
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 from airflow.models import Connection
 from airflow.providers_manager import ProvidersManager
 
 # https://docs.microsoft.com/en-us/azure/databricks/dev-tools/api/latest/aad/service-prin-aad-token#--get-an-azure-active-directory-access-token
 # https://docs.microsoft.com/en-us/graph/deployments#app-registration-and-token-service-root-endpoints
@@ -193,21 +193,23 @@
         else:
             # In this case, host = xx.cloud.databricks.com
             return host
 
     def _get_retry_object(self) -> Retrying:
         """
         Instantiate a retry object.
+
         :return: instance of Retrying class
         """
         return Retrying(**self.retry_args)
 
     def _a_get_retry_object(self) -> AsyncRetrying:
         """
         Instantiate an async retry object.
+
         :return: instance of AsyncRetrying class
         """
         return AsyncRetrying(**self.retry_args)
 
     def _get_aad_token(self, resource: str) -> str:
         """
         Function to get AAD token for given resource.
@@ -274,14 +276,15 @@
             raise AirflowException(f"Response: {e.response.content}, Status Code: {e.response.status_code}")
 
         return token
 
     async def _a_get_aad_token(self, resource: str) -> str:
         """
         Async version of `_get_aad_token()`.
+
         :param resource: resource to issue token to
         :return: AAD token, or raise an exception
         """
         aad_token = self.aad_tokens.get(resource)
         if aad_token and self._is_aad_token_valid(aad_token):
             return aad_token["token"]
 
@@ -340,28 +343,30 @@
             raise AirflowException(f"Response: {err.message}, Status Code: {err.status}")
 
         return token
 
     def _get_aad_headers(self) -> dict:
         """
         Fill AAD headers if necessary (SPN is outside of the workspace).
+
         :return: dictionary with filled AAD headers
         """
         headers = {}
         if "azure_resource_id" in self.databricks_conn.extra_dejson:
             mgmt_token = self._get_aad_token(AZURE_MANAGEMENT_ENDPOINT)
             headers["X-Databricks-Azure-Workspace-Resource-Id"] = self.databricks_conn.extra_dejson[
                 "azure_resource_id"
             ]
             headers["X-Databricks-Azure-SP-Management-Token"] = mgmt_token
         return headers
 
     async def _a_get_aad_headers(self) -> dict:
         """
         Async version of `_get_aad_headers()`.
+
         :return: dictionary with filled AAD headers
         """
         headers = {}
         if "azure_resource_id" in self.databricks_conn.extra_dejson:
             mgmt_token = await self._a_get_aad_token(AZURE_MANAGEMENT_ENDPOINT)
             headers["X-Databricks-Azure-Workspace-Resource-Id"] = self.databricks_conn.extra_dejson[
                 "azure_resource_id"
@@ -382,14 +387,15 @@
             return True
         return False
 
     @staticmethod
     def _check_azure_metadata_service() -> None:
         """
         Check for Azure Metadata Service.
+
         https://docs.microsoft.com/en-us/azure/virtual-machines/linux/instance-metadata-service
         """
         try:
             jsn = requests.get(
                 AZURE_METADATA_SERVICE_INSTANCE_URL,
                 params={"api-version": "2021-02-01"},
                 headers={"Metadata": "true"},
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 from airflow.providers.common.sql.hooks.sql import DbApiHook, return_single_query_results
 from airflow.providers.databricks.hooks.databricks_base import BaseDatabricksHook
 
 LIST_SQL_ENDPOINTS_ENDPOINT = ("GET", "api/2.0/sql/endpoints")
 
 
 class DatabricksSqlHook(BaseDatabricksHook, DbApiHook):
-    """
-    Hook to interact with Databricks SQL.
+    """Hook to interact with Databricks SQL.
 
     :param databricks_conn_id: Reference to the
         :ref:`Databricks connection <howto/connection:databricks>`.
     :param http_path: Optional string specifying HTTP path of Databricks SQL Endpoint or cluster.
         If not specified, it should be either specified in the Databricks connection's extra parameters,
         or ``sql_endpoint_name`` must be specified.
     :param sql_endpoint_name: Optional name of Databricks SQL Endpoint. If not specified, ``http_path``
@@ -91,15 +90,15 @@
             raise AirflowException("Can't list Databricks SQL endpoints")
         lst = [endpoint for endpoint in result["endpoints"] if endpoint["name"] == endpoint_name]
         if len(lst) == 0:
             raise AirflowException(f"Can't f Databricks SQL endpoint with name '{endpoint_name}'")
         return lst[0]
 
     def get_conn(self) -> Connection:
-        """Returns a Databricks SQL connection object"""
+        """Returns a Databricks SQL connection object."""
         if not self._http_path:
             if self._sql_endpoint_name:
                 endpoint = self._get_sql_endpoint_by_name(self._sql_endpoint_name)
                 self._http_path = endpoint["odbc_params"]["path"]
             elif "http_path" in self.databricks_conn.extra_dejson:
                 self._http_path = self.databricks_conn.extra_dejson["http_path"]
             else:
@@ -144,18 +143,18 @@
         sql: str | Iterable[str],
         autocommit: bool = False,
         parameters: Iterable | Mapping | None = None,
         handler: Callable | None = None,
         split_statements: bool = True,
         return_last: bool = True,
     ) -> Any | list[Any] | None:
-        """
-        Runs a command or a list of commands. Pass a list of sql
-        statements to the sql parameter to get them to execute
-        sequentially.
+        """Runs a command or a list of commands.
+
+        Pass a list of SQL statements to the SQL parameter to get them to
+        execute sequentially.
 
         :param sql: the sql statement to be executed (str) or a list of
             sql statements to execute
         :param autocommit: What to set the connection's autocommit setting to
             before executing the query. Note that currently there is no commit functionality
             in Databricks SQL so this flag has no effect.
 
@@ -176,31 +175,34 @@
             sql_list = [self.strip_sql_string(s) for s in sql]
 
         if sql_list:
             self.log.debug("Executing following statements against Databricks DB: %s", sql_list)
         else:
             raise ValueError("List of SQL statements is empty")
 
+        conn = None
         results = []
         for sql_statement in sql_list:
             # when using AAD tokens, it could expire if previous query run longer than token lifetime
-            with closing(self.get_conn()) as conn:
+            conn = self.get_conn()
+            with closing(conn.cursor()) as cur:
                 self.set_autocommit(conn, autocommit)
 
                 with closing(conn.cursor()) as cur:
                     self._run_command(cur, sql_statement, parameters)
                     if handler is not None:
                         result = handler(cur)
                         if return_single_query_results(sql, return_last, split_statements):
                             results = [result]
                             self.descriptions = [cur.description]
                         else:
                             results.append(result)
                             self.descriptions.append(cur.description)
-
+        if conn:
+            conn.close()
             self._sql_conn = None
 
         if handler is None:
             return None
         if return_single_query_results(sql, return_last, split_statements):
             return results[-1]
         else:
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/__init__.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/databricks.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Databricks operators."""
 from __future__ import annotations
 
 import time
 import warnings
+from functools import cached_property
 from logging import Logger
 from typing import TYPE_CHECKING, Any, Sequence
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator, BaseOperatorLink, XCom
 from airflow.providers.databricks.hooks.databricks import DatabricksHook, RunState
 from airflow.providers.databricks.triggers.databricks import DatabricksExecutionTrigger
 from airflow.providers.databricks.utils.databricks import normalise_json_content, validate_trigger_event
 
 if TYPE_CHECKING:
@@ -38,15 +38,15 @@
 XCOM_RUN_ID_KEY = "run_id"
 XCOM_JOB_ID_KEY = "job_id"
 XCOM_RUN_PAGE_URL_KEY = "run_page_url"
 
 
 def _handle_databricks_operator_execution(operator, hook, log, context) -> None:
     """
-    Handles the Airflow + Databricks lifecycle logic for a Databricks operator
+    Handles the Airflow + Databricks lifecycle logic for a Databricks operator.
 
     :param operator: Databricks operator being handled
     :param context: Airflow context
     """
     if operator.do_xcom_push and context is not None:
         context["ti"].xcom_push(key=XCOM_RUN_ID_KEY, value=operator.run_id)
     log.info("Run submitted with run_id: %s", operator.run_id)
@@ -96,15 +96,15 @@
                 time.sleep(operator.polling_period_seconds)
     else:
         log.info("View run status, Spark UI, and logs at %s", run_page_url)
 
 
 def _handle_deferrable_databricks_operator_execution(operator, hook, log, context) -> None:
     """
-    Handles the Airflow + Databricks lifecycle logic for deferrable Databricks operators
+    Handles the Airflow + Databricks lifecycle logic for deferrable Databricks operators.
 
     :param operator: Databricks async operator being handled
     :param context: Airflow context
     """
     job_id = hook.get_job_id(operator.run_id)
     if operator.do_xcom_push and context is not None:
         context["ti"].xcom_push(key=XCOM_JOB_ID_KEY, value=job_id)
@@ -299,15 +299,15 @@
         notebook_task: dict[str, str] | None = None,
         spark_python_task: dict[str, str | list[str]] | None = None,
         spark_submit_task: dict[str, list[str]] | None = None,
         pipeline_task: dict[str, str] | None = None,
         dbt_task: dict[str, str | list[str]] | None = None,
         new_cluster: dict[str, object] | None = None,
         existing_cluster_id: str | None = None,
-        libraries: list[dict[str, str]] | None = None,
+        libraries: list[dict[str, Any]] | None = None,
         run_name: str | None = None,
         timeout_seconds: int | None = None,
         databricks_conn_id: str = "databricks_default",
         polling_period_seconds: int = 30,
         databricks_retry_limit: int = 3,
         databricks_retry_delay: int = 1,
         databricks_retry_args: dict[Any, Any] | None = None,
@@ -400,15 +400,15 @@
             self.log.error("Error: Task: %s with invalid run_id was requested to be cancelled.", self.task_id)
 
     def execute_complete(self, context: dict | None, event: dict):
         _handle_deferrable_databricks_operator_completion(event, self.log)
 
 
 class DatabricksSubmitRunDeferrableOperator(DatabricksSubmitRunOperator):
-    """Deferrable version of ``DatabricksSubmitRunOperator``"""
+    """Deferrable version of ``DatabricksSubmitRunOperator``."""
 
     def __init__(self, *args, **kwargs):
         warnings.warn(
             "`DatabricksSubmitRunDeferrableOperator` has been deprecated. "
             "Please use `airflow.providers.databricks.operators.DatabricksSubmitRunOperator` with "
             "`deferrable=True` instead.",
             AirflowProviderDeprecationWarning,
@@ -679,15 +679,15 @@
                 "Task: %s with run_id: %s was requested to be cancelled.", self.task_id, self.run_id
             )
         else:
             self.log.error("Error: Task: %s with invalid run_id was requested to be cancelled.", self.task_id)
 
 
 class DatabricksRunNowDeferrableOperator(DatabricksRunNowOperator):
-    """Deferrable version of ``DatabricksRunNowOperator``"""
+    """Deferrable version of ``DatabricksRunNowOperator``."""
 
     def __init__(self, *args, **kwargs):
         warnings.warn(
             "`DatabricksRunNowDeferrableOperator` has been deprecated. "
             "Please use `airflow.providers.databricks.operators.DatabricksRunNowOperator` with "
             "`deferrable=True` instead.",
             AirflowProviderDeprecationWarning,
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/databricks_repos.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks_repos.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Databricks operators."""
 from __future__ import annotations
 
 import re
+from functools import cached_property
 from typing import TYPE_CHECKING, Sequence
 from urllib.parse import urlsplit
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.providers.databricks.hooks.databricks import DatabricksHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -125,15 +125,15 @@
             retry_limit=self.databricks_retry_limit,
             retry_delay=self.databricks_retry_delay,
             caller="DatabricksReposCreateOperator",
         )
 
     def execute(self, context: Context):
         """
-        Creates a Databricks Repo
+        Creates a Databricks Repo.
 
         :param context: context
         :return: Repo ID
         """
         payload = {
             "url": self.git_url,
             "provider": self.git_provider,
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,33 @@
 """This module contains Databricks operators."""
 from __future__ import annotations
 
 import csv
 import json
 from typing import TYPE_CHECKING, Any, Sequence
 
+from databricks.sql.types import Row
 from databricks.sql.utils import ParamEscaper
 
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 from airflow.providers.databricks.hooks.databricks_sql import DatabricksSqlHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
+def make_serializable(val: Row):
+    return tuple(val)
+
+
 class DatabricksSqlOperator(SQLExecuteQueryOperator):
     """
-    Executes SQL code in a Databricks SQL endpoint or a Databricks cluster
+    Executes SQL code in a Databricks SQL endpoint or a Databricks cluster.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:DatabricksSqlOperator`
 
     :param databricks_conn_id: Reference to
         :ref:`Databricks connection id<howto/connection:databricks>` (templated)
@@ -121,15 +126,15 @@
         return DatabricksSqlHook(self.databricks_conn_id, **hook_params)
 
     def _should_run_output_processing(self) -> bool:
         return self.do_xcom_push or bool(self._output_path)
 
     def _process_output(self, results: list[Any], descriptions: list[Sequence[Sequence] | None]) -> list[Any]:
         if not self._output_path:
-            return list(zip(descriptions, results))
+            return list(zip(descriptions, [[make_serializable(row) for row in res] for res in results]))
         if not self._output_format:
             raise AirflowException("Output format should be specified!")
         # Output to a file only the result of last query
         last_description = descriptions[-1]
         last_results = results[-1]
         if last_description is None:
             raise AirflowException("There is missing description present for the output file. .")
@@ -154,15 +159,15 @@
         elif self._output_format.lower() == "jsonl":
             with open(self._output_path, "w") as file:
                 for row in last_results:
                     file.write(json.dumps(row.asDict()))
                     file.write("\n")
         else:
             raise AirflowException(f"Unsupported output format: '{self._output_format}'")
-        return list(zip(descriptions, results))
+        return list(zip(descriptions, [[make_serializable(row) for row in res] for res in results]))
 
 
 COPY_INTO_APPROVED_FORMATS = ["CSV", "JSON", "AVRO", "ORC", "PARQUET", "TEXT", "BINARYFILE"]
 
 
 class DatabricksCopyIntoOperator(BaseOperator):
     """
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/__init__.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/databricks_partition.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/databricks_partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 # under the License.
 #
 """This module contains Databricks sensors."""
 
 from __future__ import annotations
 
 from datetime import datetime
+from functools import cached_property
 from typing import TYPE_CHECKING, Any, Callable, Sequence
 
 from databricks.sql.utils import ParamEscaper
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException
 from airflow.providers.common.sql.hooks.sql import fetch_all_handler
 from airflow.providers.databricks.hooks.databricks_sql import DatabricksSqlHook
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/databricks_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 # specific language governing permissions and limitations
 # under the License.
 #
 """This module contains Databricks sensors."""
 
 from __future__ import annotations
 
+from functools import cached_property
 from typing import TYPE_CHECKING, Any, Callable, Iterable, Sequence
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException
 from airflow.providers.common.sql.hooks.sql import fetch_all_handler
 from airflow.providers.databricks.hooks.databricks_sql import DatabricksSqlHook
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/triggers/__init__.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/triggers/databricks.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/utils/__init__.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/utils/databricks.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/databricks.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         msg = f"Type {param_type} used for parameter {json_path} is not a number or a string"
         raise AirflowException(msg)
 
 
 def validate_trigger_event(event: dict):
     """
     Validates correctness of the event
-    received from :class:`~airflow.providers.databricks.triggers.databricks.DatabricksExecutionTrigger`
+    received from :class:`~airflow.providers.databricks.triggers.databricks.DatabricksExecutionTrigger`.
     """
     keys_to_check = ["run_id", "run_page_url", "run_state"]
     for key in keys_to_check:
         if key not in event:
             raise AirflowException(f"Could not find `{key}` in the event: {event}")
 
     try:
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/PKG-INFO` & `apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.2.0rc2
+Version: 4.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.0/
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
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.2.0rc2``
+Release: ``4.3.0rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-databricks``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ===================
 PIP package                              Version required
 =======================================  ===================
@@ -132,14 +132,44 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.3.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* ``add a return when the event is yielded in a loop to stop the execution (#31985)``
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix type annotation (#31888)``
+* ``Fix Databricks SQL operator serialization (#31780)``
+* ``Making Databricks run related multi-query string in one session again (#31898) (#31899)``
+
+Misc
+~~~~
+* ``Remove return statement after yield from triggers class (#31703)``
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 4.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/SOURCES.txt` & `apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/pyproject.toml` & `apache-airflow-providers-databricks-4.3.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/setup.cfg` & `apache-airflow-providers-databricks-4.3.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.0/
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
 	aiohttp>=3.6.3, <4
 	apache-airflow-providers-common-sql>=1.5.0.dev0
@@ -56,10 +56,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.databricks.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.databricks
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc2/setup.py` & `apache-airflow-providers-databricks-4.3.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-databricks package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.2.0"
+version = "4.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-databricks setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

