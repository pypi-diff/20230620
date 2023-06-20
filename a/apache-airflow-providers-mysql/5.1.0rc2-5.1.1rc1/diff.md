# Comparing `tmp/apache-airflow-providers-mysql-5.1.0rc2.tar.gz` & `tmp/apache-airflow-providers-mysql-5.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-mysql-5.1.0rc2.tar", last modified: Fri May 19 17:52:58 2023, max compression
+gzip compressed data, was "apache-airflow-providers-mysql-5.1.1rc1.tar", last modified: Tue Jun 20 11:42:37 2023, max compression
```

## Comparing `apache-airflow-providers-mysql-5.1.0rc2.tar` & `apache-airflow-providers-mysql-5.1.1rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-mysql-5.1.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:57.000000 apache-airflow-providers-mysql-5.1.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-mysql-5.1.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15446 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13764 2023-05-19 17:52:57.000000 apache-airflow-providers-mysql-5.1.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-05-19 12:14:13.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-05-19 17:52:57.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12081 2023-04-14 10:21:56.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/hooks/mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2862 2023-05-03 19:47:07.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/operators/mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3268 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/transfers/presto_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/transfers/s3_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/transfers/trino_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     6469 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/transfers/vertica_to_mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/apache_airflow_providers_mysql.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15446 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/apache_airflow_providers_mysql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/apache_airflow_providers_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/apache_airflow_providers_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/apache_airflow_providers_mysql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/apache_airflow_providers_mysql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/apache_airflow_providers_mysql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/apache_airflow_providers_mysql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-mysql-5.1.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1891 2023-05-19 17:52:58.000000 apache-airflow-providers-mysql-5.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2018 2023-05-19 17:52:57.000000 apache-airflow-providers-mysql-5.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.914753 apache-airflow-providers-mysql-5.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:36.000000 apache-airflow-providers-mysql-5.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15845 2023-06-20 11:42:37.915873 apache-airflow-providers-mysql-5.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14162 2023-06-20 11:42:36.000000 apache-airflow-providers-mysql-5.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.819560 apache-airflow-providers-mysql-5.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.820891 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.859270 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3769 2023-06-20 11:42:36.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.865202 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12081 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/hooks/mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.870902 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2863 2023-06-02 11:31:21.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/operators/mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.885529 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3268 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/presto_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/s3_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/trino_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     6455 2023-06-08 05:42:54.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.909948 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15845 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-mysql-5.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-06-20 11:42:37.917878 apache-airflow-providers-mysql-5.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2018 2023-06-20 11:42:36.000000 apache-airflow-providers-mysql-5.1.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/LICENSE` & `apache-airflow-providers-mysql-5.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/MANIFEST.in` & `apache-airflow-providers-mysql-5.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/PKG-INFO` & `apache-airflow-providers-mysql-5.1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 5.1.0rc2
+Version: 5.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mysql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.1/
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
 Provides-Extra: amazon
 Provides-Extra: common.sql
 Provides-Extra: presto
 Provides-Extra: trino
 Provides-Extra: vertica
 Provides-Extra: mysql-connector-python
@@ -54,38 +54,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.1.0rc2``
+Release: ``5.1.1rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-mysql``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -138,14 +138,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.1.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Replace unicodecsv with standard csv library (#31693)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 5.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/README.rst` & `apache-airflow-providers-mysql-5.1.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.1.0rc2``
+Release: ``5.1.1rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-mysql``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -99,14 +99,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.1.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Replace unicodecsv with standard csv library (#31693)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 5.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/__init__.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "5.1.0"
+__version__ = "5.1.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/get_provider_info.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-mysql",
         "name": "MySQL",
         "description": "`MySQL <https://www.mysql.com/products/>`__\n",
         "suspended": False,
         "versions": [
+            "5.1.1",
             "5.1.0",
             "5.0.0",
             "4.0.2",
             "4.0.1",
             "4.0.0",
             "3.4.0",
             "3.3.0",
```

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/hooks/__init__.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/hooks/mysql.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/operators/__init__.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/operators/mysql.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/operators/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 
 
 class MySqlOperator(SQLExecuteQueryOperator):
     """
-    Executes sql code in a specific MySQL database
+    Executes sql code in a specific MySQL database.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:MySqlOperator`
 
     :param sql: the sql code to be executed. Can receive a str representing a
         sql statement, a list of str (sql statements), or reference to a template file.
```

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/transfers/__init__.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/transfers/presto_to_mysql.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/presto_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/transfers/s3_to_mysql.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/s3_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/transfers/trino_to_mysql.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/trino_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/airflow/providers/mysql/transfers/vertica_to_mysql.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+import csv
 from contextlib import closing
 from tempfile import NamedTemporaryFile
 from typing import TYPE_CHECKING, Sequence
 
 import MySQLdb
-import unicodecsv as csv
 
 from airflow.models import BaseOperator
 from airflow.providers.mysql.hooks.mysql import MySqlHook
 from airflow.providers.vertica.hooks.vertica import VerticaHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
@@ -121,19 +121,19 @@
 
     def _bulk_load_transfer(self, mysql, vertica):
         count = 0
         with closing(vertica.get_conn()) as conn:
             with closing(conn.cursor()) as cursor:
                 cursor.execute(self.sql)
                 selected_columns = [d.name for d in cursor.description]
-                with NamedTemporaryFile("w") as tmpfile:
+                with NamedTemporaryFile("w", encoding="utf-8") as tmpfile:
                     self.log.info("Selecting rows from Vertica to local file %s...", tmpfile.name)
                     self.log.info(self.sql)
 
-                    csv_writer = csv.writer(tmpfile, delimiter="\t", encoding="utf-8")
+                    csv_writer = csv.writer(tmpfile, delimiter="\t")
                     for row in cursor.iterate():
                         csv_writer.writerow(row)
                         count += 1
 
                     tmpfile.flush()
         self._run_preoperator(mysql)
         try:
```

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/apache_airflow_providers_mysql.egg-info/PKG-INFO` & `apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 5.1.0rc2
+Version: 5.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mysql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.1/
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
 Provides-Extra: amazon
 Provides-Extra: common.sql
 Provides-Extra: presto
 Provides-Extra: trino
 Provides-Extra: vertica
 Provides-Extra: mysql-connector-python
@@ -54,38 +54,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.1.0rc2``
+Release: ``5.1.1rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-mysql``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -138,14 +138,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.1.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Replace unicodecsv with standard csv library (#31693)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 5.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/apache_airflow_providers_mysql.egg-info/SOURCES.txt` & `apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/pyproject.toml` & `apache-airflow-providers-mysql-5.1.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/setup.cfg` & `apache-airflow-providers-mysql-5.1.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.1/
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
 	provider_info=airflow.providers.mysql.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.mysql
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-mysql-5.1.0rc2/setup.py` & `apache-airflow-providers-mysql-5.1.1rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-mysql package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.1.0"
+version = "5.1.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-mysql setup."""
     setup(
         version=version,
         extras_require={
```

