# Comparing `tmp/apache-airflow-providers-apache-spark-4.1.0rc2.tar.gz` & `tmp/apache-airflow-providers-apache-spark-4.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-spark-4.1.0rc2.tar", last modified: Fri May 19 17:51:53 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-spark-4.1.1rc1.tar", last modified: Tue Jun 20 11:41:30 2023, max compression
```

## Comparing `apache-airflow-providers-apache-spark-4.1.0rc2.tar` & `apache-airflow-providers-apache-spark-4.1.1rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-spark-4.1.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:52.000000 apache-airflow-providers-apache-spark-4.1.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-spark-4.1.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11818 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10273 2023-05-19 17:51:52.000000 apache-airflow-providers-apache-spark-4.1.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-19 12:02:48.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3495 2023-05-19 17:51:52.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11382 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/hooks/spark_jdbc.py
--rw-r--r--   0 root         (0) root         (0)     6750 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
--rw-r--r--   0 root         (0) root         (0)     7052 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/hooks/spark_sql.py
--rw-r--r--   0 root         (0) root         (0)    28715 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/hooks/spark_submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9972 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/operators/spark_jdbc.py
--rw-r--r--   0 root         (0) root         (0)     4505 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/operators/spark_sql.py
--rw-r--r--   0 root         (0) root         (0)     8419 2023-03-16 20:46:35.000000 apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/operators/spark_submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/apache_airflow_providers_apache_spark.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11818 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/apache_airflow_providers_apache_spark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1074 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/apache_airflow_providers_apache_spark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/apache_airflow_providers_apache_spark.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/apache_airflow_providers_apache_spark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/apache_airflow_providers_apache_spark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/apache_airflow_providers_apache_spark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-apache-spark-4.1.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1873 2023-05-19 17:51:53.000000 apache-airflow-providers-apache-spark-4.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-19 17:51:52.000000 apache-airflow-providers-apache-spark-4.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.186280 apache-airflow-providers-apache-spark-4.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12344 2023-06-20 11:41:30.187336 apache-airflow-providers-apache-spark-4.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-20 11:41:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.094919 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.096025 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.097257 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.132264 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3516 2023-06-20 11:41:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.147465 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11383 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py
+-rw-r--r--   0 root         (0) root         (0)     6753 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
+-rw-r--r--   0 root         (0) root         (0)     7054 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_sql.py
+-rw-r--r--   0 root         (0) root         (0)    28715 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.159330 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9973 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_jdbc.py
+-rw-r--r--   0 root         (0) root         (0)     4508 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_sql.py
+-rw-r--r--   0 root         (0) root         (0)     8414 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.183585 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12344 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-spark-4.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-06-20 11:41:30.189305 apache-airflow-providers-apache-spark-4.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:41:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/LICENSE` & `apache-airflow-providers-apache-spark-4.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/MANIFEST.in` & `apache-airflow-providers-apache-spark-4.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/PKG-INFO` & `apache-airflow-providers-apache-spark-4.1.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-spark
-Version: 4.1.0rc2
+Version: 4.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-spark package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.1/
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
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.1.0rc2``
+Release: ``4.1.1rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.spark`` provider. All classes for this provider package
 are in ``airflow.providers.apache.spark`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-spark``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -109,14 +109,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``SparkSubmitOperator: rename spark_conn_id to conn_id (#31952)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 4.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/README.rst` & `apache-airflow-providers-apache-spark-4.1.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.1.0rc2``
+Release: ``4.1.1rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.spark`` provider. All classes for this provider package
 are in ``airflow.providers.apache.spark`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-spark``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -76,14 +76,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``SparkSubmitOperator: rename spark_conn_id to conn_id (#31952)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 4.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/__init__.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.1.0"
+__version__ = "4.1.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/get_provider_info.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-spark",
         "name": "Apache Spark",
         "description": "`Apache Spark <https://spark.apache.org/>`__\n",
         "suspended": False,
         "versions": [
+            "4.1.1",
             "4.1.0",
             "4.0.1",
             "4.0.0",
             "3.0.0",
             "2.1.3",
             "2.1.2",
             "2.1.1",
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/hooks/__init__.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/hooks/spark_jdbc.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,13 +219,13 @@
         if self._save_format:
             arguments += ["-saveFormat", self._save_format]
         if self._create_table_column_types:
             arguments += ["-createTableColumnTypes", self._create_table_column_types]
         return arguments
 
     def submit_jdbc_job(self) -> None:
-        """Submit Spark JDBC job"""
+        """Submit Spark JDBC job."""
         self._application_args = self._build_jdbc_application_arguments(self._jdbc_connection)
         self.submit(application=f"{os.path.dirname(os.path.abspath(__file__))}/spark_jdbc_script.py")
 
     def get_conn(self) -> Any:
         pass
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/hooks/spark_jdbc_script.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     url: str = "localhost:5432",
     jdbc_table: str = "default.default",
     user: str = "root",
     password: str = "root",
     driver: str = "driver",
 ) -> Any:
     """
-    Get Spark source from JDBC connection
+    Get Spark source from JDBC connection.
 
     :param spark_source: Spark source, here is Spark reader or writer
     :param url: JDBC resource url
     :param jdbc_table: JDBC resource table name
     :param user: JDBC resource user name
     :param password: JDBC resource password
     :param driver: JDBC resource driver
@@ -65,15 +65,15 @@
     driver: Any,
     truncate: bool,
     save_mode: str,
     batch_size: int,
     num_partitions: int,
     create_table_column_types: str,
 ) -> None:
-    """Transfer data from Spark to JDBC source"""
+    """Transfer data from Spark to JDBC source."""
     writer = spark_session.table(metastore_table).write
     # first set common options
     writer = set_common_options(writer, url, jdbc_table, user, password, driver)
 
     # now set write-specific options
     if truncate:
         writer = writer.option("truncate", truncate)
@@ -99,15 +99,15 @@
     save_format: str,
     fetch_size: int,
     num_partitions: int,
     partition_column: str,
     lower_bound: str,
     upper_bound: str,
 ) -> None:
-    """Transfer data from JDBC source to Spark"""
+    """Transfer data from JDBC source to Spark."""
     # first set common options
     reader = set_common_options(spark_session.read, url, jdbc_table, user, password, driver)
 
     # now set specific read options
     if fetch_size:
         reader = reader.option("fetchsize", fetch_size)
     if num_partitions:
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/hooks/spark_sql.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
         self.log.debug("Spark-Sql cmd: %s", connection_cmd)
 
         return connection_cmd
 
     def run_query(self, cmd: str = "", **kwargs: Any) -> None:
         """
-        Remote Popen (actually execute the Spark-sql query)
+        Remote Popen (actually execute the Spark-sql query).
 
         :param cmd: command to append to the spark-sql command
         :param kwargs: extra arguments to Popen (see subprocess.Popen)
         """
         spark_sql_cmd = self._prepare_command(cmd)
 
         self._sp = subprocess.Popen(
@@ -181,11 +181,11 @@
         if returncode:
             raise AirflowException(
                 f"Cannot execute '{self._sql}' on {self._master} (additional parameters: '{cmd}'). "
                 f"Process exit code: {returncode}."
             )
 
     def kill(self) -> None:
-        """Kill Spark job"""
+        """Kill Spark job."""
         if self._sp and self._sp.poll() is None:
             self.log.info("Killing the Spark-Sql job")
             self._sp.kill()
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/hooks/spark_submit.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_submit.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     conn_name_attr = "conn_id"
     default_conn_name = "spark_default"
     conn_type = "spark"
     hook_name = "Spark"
 
     @staticmethod
     def get_ui_field_behaviour() -> dict[str, Any]:
-        """Returns custom field behaviour"""
+        """Returns custom field behaviour."""
         return {
             "hidden_fields": ["schema", "login", "password"],
             "relabeling": {},
         }
 
     def __init__(
         self,
@@ -162,17 +162,19 @@
         self._should_track_driver_status = self._resolve_should_track_driver_status()
         self._driver_id: str | None = None
         self._driver_status: str | None = None
         self._spark_exit_code: int | None = None
         self._env: dict[str, Any] | None = None
 
     def _resolve_should_track_driver_status(self) -> bool:
-        """
-        Determines whether this hook should poll the spark driver status through
-        subsequent spark-submit status requests after the initial spark-submit request
+        """Check if we should track the driver status.
+
+        If so, we should send subsequent spark-submit status requests after the
+        initial spark-submit request.
+
         :return: if the driver status should be tracked
         """
         return "spark://" in self._connection["master"] and self._connection["deploy_mode"] == "cluster"
 
     def _resolve_connection(self) -> dict[str, Any]:
         # Build from connection master or default to yarn if not available
         conn_data = {
@@ -381,15 +383,15 @@
 
         self.log.debug("Poll driver status cmd: %s", connection_cmd)
 
         return connection_cmd
 
     def submit(self, application: str = "", **kwargs: Any) -> None:
         """
-        Remote Popen to execute the spark-submit job
+        Remote Popen to execute the spark-submit job.
 
         :param application: Submitted application, jar or py file
         :param kwargs: extra arguments to Popen (see subprocess.Popen)
         """
         spark_submit_cmd = self._build_spark_submit_command(application)
 
         if self._env:
@@ -487,15 +489,15 @@
                     self._driver_id = match_driver_id.groups()[0]
                     self.log.info("identified spark driver id: %s", self._driver_id)
 
             self.log.info(line)
 
     def _process_spark_status_log(self, itr: Iterator[Any]) -> None:
         """
-        Parses the logs of the spark driver status query process
+        Parses the logs of the spark driver status query process.
 
         :param itr: An iterator which iterates over the input of the subprocess
         """
         driver_found = False
         valid_response = False
         # Consume the iterator
         for line in itr:
@@ -578,14 +580,15 @@
                         f"Failed to poll for the driver status {max_missed_job_status_reports} times: "
                         f"returncode = {returncode}"
                     )
 
     def _build_spark_driver_kill_command(self) -> list[str]:
         """
         Construct the spark-submit command to kill a driver.
+
         :return: full command to kill a driver
         """
         # Assume that spark-submit is present in the path to the executing user
         connection_cmd = [self._connection["spark_binary"]]
 
         # The url to the spark master
         connection_cmd += ["--master", self._connection["master"]]
@@ -595,15 +598,15 @@
             connection_cmd += ["--kill", self._driver_id]
 
         self.log.debug("Spark-Kill cmd: %s", connection_cmd)
 
         return connection_cmd
 
     def on_kill(self) -> None:
-        """Kill Spark submit command"""
+        """Kill Spark submit command."""
         self.log.debug("Kill Command is being called")
 
         if self._should_track_driver_status and self._driver_id:
             self.log.info("Killing driver %s on cluster", self._driver_id)
 
             kill_cmd = self._build_spark_driver_kill_command()
             with subprocess.Popen(kill_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE) as driver_kill:
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/operators/__init__.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/operators/spark_jdbc.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_jdbc.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         self._partition_column = partition_column
         self._lower_bound = lower_bound
         self._upper_bound = upper_bound
         self._create_table_column_types = create_table_column_types
         self._hook: SparkJDBCHook | None = None
 
     def execute(self, context: Context) -> None:
-        """Call the SparkSubmitHook to run the provided spark job"""
+        """Call the SparkSubmitHook to run the provided spark job."""
         if self._hook is None:
             self._hook = self._get_hook()
         self._hook.submit_jdbc_job()
 
     def on_kill(self) -> None:
         if self._hook is None:
             self._hook = self._get_hook()
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/operators/spark_sql.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SparkSqlOperator(BaseOperator):
     """
-    Execute Spark SQL query
+    Execute Spark SQL query.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SparkSqlOperator`
 
     :param sql: The SQL query to execute. (templated)
     :param conf: arbitrary Spark configuration property
@@ -87,26 +87,26 @@
         self._name = name
         self._num_executors = num_executors
         self._verbose = verbose
         self._yarn_queue = yarn_queue
         self._hook: SparkSqlHook | None = None
 
     def execute(self, context: Context) -> None:
-        """Call the SparkSqlHook to run the provided sql query"""
+        """Call the SparkSqlHook to run the provided sql query."""
         if self._hook is None:
             self._hook = self._get_hook()
         self._hook.run_query()
 
     def on_kill(self) -> None:
         if self._hook is None:
             self._hook = self._get_hook()
         self._hook.kill()
 
     def _get_hook(self) -> SparkSqlHook:
-        """Get SparkSqlHook"""
+        """Get SparkSqlHook."""
         return SparkSqlHook(
             sql=self._sql,
             conf=self._conf,
             conn_id=self._conn_id,
             total_executor_cores=self._total_executor_cores,
             executor_cores=self._executor_cores,
             executor_memory=self._executor_memory,
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/airflow/providers/apache/spark/operators/spark_submit.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_submit.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SparkSubmitOperator`
 
     :param application: The application that submitted as a job, either jar or py file. (templated)
     :param conf: Arbitrary Spark configuration properties (templated)
-    :param spark_conn_id: The :ref:`spark connection id <howto/connection:spark>` as configured
+    :param conn_id: The :ref:`spark connection id <howto/connection:spark>` as configured
         in Airflow administration. When an invalid connection_id is supplied, it will default to yarn.
     :param files: Upload additional files to the executor running the job, separated by a
                   comma. Files will be placed in the working directory of each executor.
                   For example, serialized objects. (templated)
     :param py_files: Additional python files used by the job, can be .zip, .egg or .py. (templated)
     :param jars: Submit additional jars to upload and place them in executor classpath. (templated)
     :param driver_class_path: Additional, driver-specific, classpath settings. (templated)
@@ -147,15 +147,15 @@
         self._env_vars = env_vars
         self._verbose = verbose
         self._spark_binary = spark_binary
         self._hook: SparkSubmitHook | None = None
         self._conn_id = conn_id
 
     def execute(self, context: Context) -> None:
-        """Call the SparkSubmitHook to run the provided spark job"""
+        """Call the SparkSubmitHook to run the provided spark job."""
         if self._hook is None:
             self._hook = self._get_hook()
         self._hook.submit(self._application)
 
     def on_kill(self) -> None:
         if self._hook is None:
             self._hook = self._get_hook()
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/apache_airflow_providers_apache_spark.egg-info/PKG-INFO` & `apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-spark
-Version: 4.1.0rc2
+Version: 4.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-spark package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.1/
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
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.1.0rc2``
+Release: ``4.1.1rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.spark`` provider. All classes for this provider package
 are in ``airflow.providers.apache.spark`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-spark``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -109,14 +109,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``SparkSubmitOperator: rename spark_conn_id to conn_id (#31952)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 4.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/pyproject.toml` & `apache-airflow-providers-apache-spark-4.1.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/setup.cfg` & `apache-airflow-providers-apache-spark-4.1.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.1/
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
 	pyspark
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.spark.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.spark
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-spark-4.1.0rc2/setup.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-spark package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.1.0"
+version = "4.1.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-spark setup."""
     setup(
         version=version,
         extras_require={},
```

