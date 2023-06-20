# Comparing `tmp/apache-airflow-providers-snowflake-4.1.0rc2.tar.gz` & `tmp/apache-airflow-providers-snowflake-4.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-snowflake-4.1.0rc2.tar", last modified: Fri May 19 17:53:35 2023, max compression
+gzip compressed data, was "apache-airflow-providers-snowflake-4.2.0rc1.tar", last modified: Tue Jun 20 11:43:15 2023, max compression
```

## Comparing `apache-airflow-providers-snowflake-4.1.0rc2.tar` & `apache-airflow-providers-snowflake-4.2.0rc1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-snowflake-4.1.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:34.000000 apache-airflow-providers-snowflake-4.1.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-snowflake-4.1.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    19277 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17692 2023-05-19 17:53:34.000000 apache-airflow-providers-snowflake-4.1.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-05-19 12:21:57.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4589 2023-05-19 17:53:34.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17835 2023-04-30 16:55:41.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/hooks/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15272 2023-05-03 19:47:07.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5782 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     6053 2023-05-03 19:47:07.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/s3_to_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     5078 2023-05-03 19:47:07.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/snowflake_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/utils/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19277 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1079 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-snowflake-4.1.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1789 2023-05-19 17:53:34.000000 apache-airflow-providers-snowflake-4.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.974181 apache-airflow-providers-snowflake-4.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    19907 2023-06-20 11:43:15.975546 apache-airflow-providers-snowflake-4.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18321 2023-06-20 11:43:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.861078 apache-airflow-providers-snowflake-4.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.862300 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.902943 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4724 2023-06-20 11:43:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.912718 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17859 2023-06-05 12:50:36.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)    11759 2023-06-08 05:42:54.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.918823 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22918 2023-06-17 16:45:00.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.931338 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5786 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     5078 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.942711 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/common.py
+-rw-r--r--   0 root         (0) root         (0)     6878 2023-06-01 07:44:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.970806 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19907 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-snowflake-4.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-06-20 11:43:15.977871 apache-airflow-providers-snowflake-4.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-06-20 11:43:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/LICENSE` & `apache-airflow-providers-snowflake-4.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/MANIFEST.in` & `apache-airflow-providers-snowflake-4.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/PKG-INFO` & `apache-airflow-providers-snowflake-4.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.1.0rc2
+Version: 4.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.2.0/
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
 Provides-Extra: slack
 License-File: LICENSE
 License-File: NOTICE
 
 
@@ -50,38 +50,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.1.0rc2``
+Release: ``4.2.0rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-snowflake``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -133,14 +133,38 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.2.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* ``Add SnowflakeSqlApiOperator operator (#30698)``
+
+Misc
+~~~~
+
+* ``SnowflakeSqlApiOperator - Change the base class (#31751)``
+* ``Moved sql_api_generate_jwt out of hooks folder (#31586)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check (#31742)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 4.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/README.rst` & `apache-airflow-providers-snowflake-4.2.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.1.0rc2``
+Release: ``4.2.0rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-snowflake``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -98,14 +98,38 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.2.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* ``Add SnowflakeSqlApiOperator operator (#30698)``
+
+Misc
+~~~~
+
+* ``SnowflakeSqlApiOperator - Change the base class (#31751)``
+* ``Moved sql_api_generate_jwt out of hooks folder (#31586)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check (#31742)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 4.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/__init__.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.1.0"
+__version__ = "4.2.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/get_provider_info.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-snowflake",
         "name": "Snowflake",
         "description": "`Snowflake <https://www.snowflake.com/>`__\n",
         "suspended": False,
         "versions": [
+            "4.2.0",
             "4.1.0",
             "4.0.5",
             "4.0.4",
             "4.0.3",
             "4.0.2",
             "4.0.1",
             "4.0.0",
@@ -78,15 +79,18 @@
                 "integration-name": "Snowflake",
                 "python-modules": ["airflow.providers.snowflake.operators.snowflake"],
             }
         ],
         "hooks": [
             {
                 "integration-name": "Snowflake",
-                "python-modules": ["airflow.providers.snowflake.hooks.snowflake"],
+                "python-modules": [
+                    "airflow.providers.snowflake.hooks.snowflake",
+                    "airflow.providers.snowflake.hooks.snowflake_sql_api",
+                ],
             }
         ],
         "transfers": [
             {
                 "source-integration-name": "Amazon Simple Storage Service (S3)",
                 "target-integration-name": "Snowflake",
                 "python-module": "airflow.providers.snowflake.transfers.s3_to_snowflake",
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/hooks/__init__.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/hooks/snowflake.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,17 @@
 
 def _try_to_boolean(value: Any):
     if isinstance(value, (str, type(None))):
         return to_boolean(value)
     return value
 
 
+# TODO: Remove this when provider min airflow version >= 2.5.0 since this is
+# handled by provider manager from that version.
 def _ensure_prefixes(conn_type):
-    """
-    Remove when provider min airflow version >= 2.5.0 since this is handled by
-    provider manager from that version.
-    """
-
     def dec(func):
         @wraps(func)
         def inner():
             field_behaviors = func()
             conn_attrs = {"host", "schema", "login", "password", "port", "extra"}
 
             def _ensure_prefix(field):
@@ -67,16 +64,15 @@
 
         return inner
 
     return dec
 
 
 class SnowflakeHook(DbApiHook):
-    """
-    A client to interact with Snowflake.
+    """A client to interact with Snowflake.
 
     This hook requires the snowflake_conn_id connection. The snowflake account, login,
     and, password field must be setup in the connection. Other inputs can be defined
     in the connection or hook instantiation.
 
     :param snowflake_conn_id: Reference to
         :ref:`Snowflake connection id<howto/connection:snowflake>`
@@ -112,15 +108,15 @@
     conn_type = "snowflake"
     hook_name = "Snowflake"
     supports_autocommit = True
     _test_connection_sql = "select 1"
 
     @staticmethod
     def get_connection_form_widgets() -> dict[str, Any]:
-        """Returns connection widgets to add to connection form"""
+        """Returns connection widgets to add to connection form."""
         from flask_appbuilder.fieldwidgets import BS3TextAreaFieldWidget, BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import BooleanField, StringField
 
         return {
             "account": StringField(lazy_gettext("Account"), widget=BS3TextFieldWidget()),
             "warehouse": StringField(lazy_gettext("Warehouse"), widget=BS3TextFieldWidget()),
@@ -135,15 +131,15 @@
                 label=lazy_gettext("Insecure mode"), description="Turns off OCSP certificate checks"
             ),
         }
 
     @staticmethod
     @_ensure_prefixes(conn_type="snowflake")
     def get_ui_field_behaviour() -> dict[str, Any]:
-        """Returns custom field behaviour"""
+        """Returns custom field behaviour."""
         import json
 
         return {
             "hidden_fields": ["port", "host"],
             "relabeling": {},
             "placeholders": {
                 "extra": json.dumps(
@@ -197,17 +193,17 @@
                     f"Using value for `{field_name}`.  Please ensure this is the correct "
                     f"value and remove the backcompat key `{backcompat_key}`."
                 )
             return extra_dict[field_name] or None
         return extra_dict.get(backcompat_key) or None
 
     def _get_conn_params(self) -> dict[str, str | None]:
-        """
-        One method to fetch connection params as a dict
-        used in get_uri() and get_connection()
+        """Fetch connection params as a dict.
+
+        This is used in ``get_uri()`` and ``get_connection()``.
         """
         conn = self.get_connection(self.snowflake_conn_id)  # type: ignore[attr-defined]
         extra_dict = conn.extra_dejson
         account = self._get_field(extra_dict, "account") or ""
         warehouse = self._get_field(extra_dict, "warehouse") or ""
         database = self._get_field(extra_dict, "database") or ""
         region = self._get_field(extra_dict, "region") or ""
@@ -273,36 +269,35 @@
 
             conn_config["private_key"] = pkb
             conn_config.pop("password", None)
 
         return conn_config
 
     def get_uri(self) -> str:
-        """Override DbApiHook get_uri method for get_sqlalchemy_engine()"""
+        """Override DbApiHook get_uri method for get_sqlalchemy_engine()."""
         conn_params = self._get_conn_params()
         return self._conn_params_to_sqlalchemy_uri(conn_params)
 
     def _conn_params_to_sqlalchemy_uri(self, conn_params: dict) -> str:
         return URL(
             **{
                 k: v
                 for k, v in conn_params.items()
                 if v and k not in ["session_parameters", "insecure_mode", "private_key"]
             }
         )
 
     def get_conn(self) -> SnowflakeConnection:
-        """Returns a snowflake.connection object"""
+        """Returns a snowflake.connection object."""
         conn_config = self._get_conn_params()
         conn = connector.connect(**conn_config)
         return conn
 
     def get_sqlalchemy_engine(self, engine_kwargs=None):
-        """
-        Get an sqlalchemy_engine object.
+        """Get an sqlalchemy_engine object.
 
         :param engine_kwargs: Kwargs used in :func:`~sqlalchemy.create_engine`.
         :return: the created engine.
         """
         engine_kwargs = engine_kwargs or {}
         conn_params = self._get_conn_params()
         if "insecure_mode" in conn_params:
@@ -327,34 +322,38 @@
         autocommit: bool = False,
         parameters: Iterable | Mapping | None = None,
         handler: Callable | None = None,
         split_statements: bool = True,
         return_last: bool = True,
         return_dictionaries: bool = False,
     ) -> Any | list[Any] | None:
-        """
-        Runs a command or a list of commands. Pass a list of sql
-        statements to the sql parameter to get them to execute
-        sequentially. The variable execution_info is returned so that
-        it can be used in the Operators to modify the behavior
-        depending on the result of the query (i.e fail the operator
-        if the copy has processed 0 files)
+        """Runs a command or a list of commands.
+
+        Pass a list of SQL statements to the SQL parameter to get them to
+        execute sequentially. The variable ``execution_info`` is returned so
+        that it can be used in the Operators to modify the behavior depending on
+        the result of the query (i.e fail the operator if the copy has processed
+        0 files).
 
-        :param sql: the sql string to be executed with possibly multiple statements,
-          or a list of sql statements to execute
+        :param sql: The SQL string to be executed with possibly multiple
+            statements, or a list of sql statements to execute
         :param autocommit: What to set the connection's autocommit setting to
             before executing the query.
         :param parameters: The parameters to render the SQL query with.
-        :param handler: The result handler which is called with the result of each statement.
-        :param split_statements: Whether to split a single SQL string into statements and run separately
-        :param return_last: Whether to return result for only last statement or for all after split
-        :param return_dictionaries: Whether to return dictionaries rather than regular DBApi sequences
-            as rows in the result. The dictionaries are of form:
-            ``{ 'column1_name': value1, 'column2_name': value2 ... }``.
-        :return: return only result of the LAST SQL expression if handler was provided.
+        :param handler: The result handler which is called with the result of
+            each statement.
+        :param split_statements: Whether to split a single SQL string into
+            statements and run separately
+        :param return_last: Whether to return result for only last statement or
+            for all after split.
+        :param return_dictionaries: Whether to return dictionaries rather than
+            regular DBAPI sequences as rows in the result. The dictionaries are
+            of form ``{ 'column1_name': value1, 'column2_name': value2 ... }``.
+        :return: Result of the last SQL statement if *handler* is set.
+            *None* otherwise.
         """
         self.query_ids = []
 
         if isinstance(sql, str):
             if split_statements:
                 split_statements_tuple = util_text.split_statements(StringIO(sql))
                 sql_list: Iterable[str] = [
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/operators/__init__.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/operators/snowflake.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/snowflake.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,29 +13,38 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+import time
 import warnings
-from typing import Any, Iterable, Mapping, Sequence, SupportsAbs
+from datetime import timedelta
+from typing import TYPE_CHECKING, Any, Iterable, Mapping, Sequence, SupportsAbs
 
+from airflow import AirflowException
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.common.sql.operators.sql import (
     SQLCheckOperator,
     SQLExecuteQueryOperator,
     SQLIntervalCheckOperator,
     SQLValueCheckOperator,
 )
+from airflow.providers.snowflake.hooks.snowflake_sql_api import (
+    SnowflakeSqlApiHook,
+)
+
+if TYPE_CHECKING:
+    from airflow.utils.context import Context
 
 
 class SnowflakeOperator(SQLExecuteQueryOperator):
     """
-    Executes SQL code in a Snowflake database
+    Executes SQL code in a Snowflake database.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SnowflakeOperator`
 
     :param snowflake_conn_id: Reference to
         :ref:`Snowflake connection id<howto/connection:snowflake>`
@@ -355,7 +364,156 @@
         self.warehouse = warehouse
         self.database = database
         self.role = role
         self.schema = schema
         self.authenticator = authenticator
         self.session_parameters = session_parameters
         self.query_ids: list[str] = []
+
+
+class SnowflakeSqlApiOperator(SQLExecuteQueryOperator):
+    """
+    Implemented Snowflake SQL API Operator to support multiple SQL statements sequentially,
+    which is the behavior of the SnowflakeOperator, the Snowflake SQL API allows submitting
+    multiple SQL statements in a single request. It make post request to submit SQL
+    statements for execution, poll to check the status of the execution of a statement. Fetch query results
+    concurrently.
+    This Operator currently uses key pair authentication, so you need to provide private key raw content or
+    private key file path in the snowflake connection along with other details
+
+    .. seealso::
+
+        `Snowflake SQL API key pair Authentication <https://docs.snowflake.com/en/developer-guide/sql-api/authenticating.html#label-sql-api-authenticating-key-pair>`_
+
+    Where can this operator fit in?
+         - To execute multiple SQL statements in a single request
+         - To execute the SQL statement asynchronously and to execute standard queries and most DDL and DML statements
+         - To develop custom applications and integrations that perform queries
+         - To create provision users and roles, create table, etc.
+
+    The following commands are not supported:
+        - The PUT command (in Snowflake SQL)
+        - The GET command (in Snowflake SQL)
+        - The CALL command with stored procedures that return a table(stored procedures with the RETURNS TABLE clause).
+
+    .. seealso::
+
+        - `Snowflake SQL API <https://docs.snowflake.com/en/developer-guide/sql-api/intro.html#introduction-to-the-sql-api>`_
+        - `API Reference <https://docs.snowflake.com/en/developer-guide/sql-api/reference.html#snowflake-sql-api-reference>`_
+        - `Limitation on snowflake SQL API <https://docs.snowflake.com/en/developer-guide/sql-api/intro.html#limitations-of-the-sql-api>`_
+
+    :param snowflake_conn_id: Reference to Snowflake connection id
+    :param sql: the sql code to be executed. (templated)
+    :param autocommit: if True, each command is automatically committed.
+        (default value: True)
+    :param parameters: (optional) the parameters to render the SQL query with.
+    :param warehouse: name of warehouse (will overwrite any warehouse
+        defined in the connection's extra JSON)
+    :param database: name of database (will overwrite database defined
+        in connection)
+    :param schema: name of schema (will overwrite schema defined in
+        connection)
+    :param role: name of role (will overwrite any role defined in
+        connection's extra JSON)
+    :param authenticator: authenticator for Snowflake.
+        'snowflake' (default) to use the internal Snowflake authenticator
+        'externalbrowser' to authenticate using your web browser and
+        Okta, ADFS or any other SAML 2.0-compliant identify provider
+        (IdP) that has been defined for your account
+        'https://<your_okta_account_name>.okta.com' to authenticate
+        through native Okta.
+    :param session_parameters: You can set session-level parameters at
+        the time you connect to Snowflake
+    :param poll_interval: the interval in seconds to poll the query
+    :param statement_count: Number of SQL statement to be executed
+    :param token_life_time: lifetime of the JWT Token
+    :param token_renewal_delta: Renewal time of the JWT Token
+    :param bindings: (Optional) Values of bind variables in the SQL statement.
+            When executing the statement, Snowflake replaces placeholders (? and :name) in
+            the statement with these specified values.
+    """  # noqa
+
+    LIFETIME = timedelta(minutes=59)  # The tokens will have a 59 minutes lifetime
+    RENEWAL_DELTA = timedelta(minutes=54)  # Tokens will be renewed after 54 minutes
+
+    def __init__(
+        self,
+        *,
+        snowflake_conn_id: str = "snowflake_default",
+        warehouse: str | None = None,
+        database: str | None = None,
+        role: str | None = None,
+        schema: str | None = None,
+        authenticator: str | None = None,
+        session_parameters: dict[str, Any] | None = None,
+        poll_interval: int = 5,
+        statement_count: int = 0,
+        token_life_time: timedelta = LIFETIME,
+        token_renewal_delta: timedelta = RENEWAL_DELTA,
+        bindings: dict[str, Any] | None = None,
+        **kwargs: Any,
+    ) -> None:
+        self.snowflake_conn_id = snowflake_conn_id
+        self.poll_interval = poll_interval
+        self.statement_count = statement_count
+        self.token_life_time = token_life_time
+        self.token_renewal_delta = token_renewal_delta
+        self.bindings = bindings
+        self.execute_async = False
+        if any([warehouse, database, role, schema, authenticator, session_parameters]):  # pragma: no cover
+            hook_params = kwargs.pop("hook_params", {})  # pragma: no cover
+            kwargs["hook_params"] = {
+                "warehouse": warehouse,
+                "database": database,
+                "role": role,
+                "schema": schema,
+                "authenticator": authenticator,
+                "session_parameters": session_parameters,
+                **hook_params,
+            }
+        super().__init__(conn_id=snowflake_conn_id, **kwargs)  # pragma: no cover
+
+    def execute(self, context: Context) -> None:
+        """
+        Make a POST API request to snowflake by using SnowflakeSQL and execute the query to get the ids.
+        By deferring the SnowflakeSqlApiTrigger class passed along with query ids.
+        """
+        self.log.info("Executing: %s", self.sql)
+        self._hook = SnowflakeSqlApiHook(
+            snowflake_conn_id=self.snowflake_conn_id,
+            token_life_time=self.token_life_time,
+            token_renewal_delta=self.token_renewal_delta,
+        )
+        self.query_ids = self._hook.execute_query(
+            self.sql, statement_count=self.statement_count, bindings=self.bindings  # type: ignore[arg-type]
+        )
+        self.log.info("List of query ids %s", self.query_ids)
+
+        if self.do_xcom_push:
+            context["ti"].xcom_push(key="query_ids", value=self.query_ids)
+
+        statement_status = self.poll_on_queries()
+        if statement_status["error"]:
+            raise AirflowException(statement_status["error"])
+        self._hook.check_query_output(self.query_ids)
+
+    def poll_on_queries(self):
+        """Poll on requested queries."""
+        queries_in_progress = set(self.query_ids)
+        statement_success_status = {}
+        statement_error_status = {}
+        for query_id in self.query_ids:
+            if not len(queries_in_progress):
+                break
+            self.log.info("checking : %s", query_id)
+            try:
+                statement_status = self._hook.get_sql_api_query_status(query_id)
+            except Exception as e:
+                raise ValueError({"status": "error", "message": str(e)})
+            if statement_status.get("status") == "error":
+                queries_in_progress.remove(query_id)
+                statement_error_status[query_id] = statement_status
+            if statement_status.get("status") == "success":
+                statement_success_status[query_id] = statement_status
+                queries_in_progress.remove(query_id)
+            time.sleep(self.poll_interval)
+        return {"success": statement_success_status, "error": statement_error_status}
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/__init__.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,29 +11,30 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""This module contains abstract operator that child classes implements
-COPY INTO <TABLE> SQL in Snowflake
+"""
+This module contains abstract operator that child classes
+implement "COPY INTO <TABLE> SQL in Snowflake".
 """
 from __future__ import annotations
 
 from typing import Any, Sequence
 
 from airflow.models import BaseOperator
 from airflow.providers.snowflake.hooks.snowflake import SnowflakeHook
 from airflow.providers.snowflake.utils.common import enclose_param
 
 
 class CopyFromExternalStageToSnowflakeOperator(BaseOperator):
     """
-    Executes a COPY INTO command to load files from an external stage from clouds to Snowflake
+    Executes a COPY INTO command to load files from an external stage from clouds to Snowflake.
 
     This operator requires the snowflake_conn_id connection. The snowflake host, login,
     and, password field must be setup in the connection. Other inputs can be defined
     in the connection or hook instantiation.
 
     :param namespace: snowflake namespace
     :param table: snowflake table
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/s3_to_snowflake.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from airflow.models import BaseOperator
 from airflow.providers.snowflake.hooks.snowflake import SnowflakeHook
 from airflow.providers.snowflake.utils.common import enclose_param
 
 
 class S3ToSnowflakeOperator(BaseOperator):
     """
-    Executes an COPY command to load files from s3 to Snowflake
+    Executes an COPY command to load files from s3 to Snowflake.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:S3ToSnowflakeOperator`
 
     :param s3_keys: reference to a list of S3 keys
     :param table: reference to a specific table in snowflake database
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/snowflake_to_slack.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/utils/__init__.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/utils/common.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/PKG-INFO` & `apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.1.0rc2
+Version: 4.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.2.0/
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
 Provides-Extra: slack
 License-File: LICENSE
 License-File: NOTICE
 
 
@@ -50,38 +50,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.1.0rc2``
+Release: ``4.2.0rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-snowflake``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -133,14 +133,38 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.2.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* ``Add SnowflakeSqlApiOperator operator (#30698)``
+
+Misc
+~~~~
+
+* ``SnowflakeSqlApiOperator - Change the base class (#31751)``
+* ``Moved sql_api_generate_jwt out of hooks folder (#31586)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check (#31742)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 4.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/SOURCES.txt` & `apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 pyproject.toml
 setup.cfg
 setup.py
 airflow/providers/snowflake/__init__.py
 airflow/providers/snowflake/get_provider_info.py
 airflow/providers/snowflake/hooks/__init__.py
 airflow/providers/snowflake/hooks/snowflake.py
+airflow/providers/snowflake/hooks/snowflake_sql_api.py
 airflow/providers/snowflake/operators/__init__.py
 airflow/providers/snowflake/operators/snowflake.py
 airflow/providers/snowflake/transfers/__init__.py
 airflow/providers/snowflake/transfers/copy_into_snowflake.py
 airflow/providers/snowflake/transfers/s3_to_snowflake.py
 airflow/providers/snowflake/transfers/snowflake_to_slack.py
 airflow/providers/snowflake/utils/__init__.py
 airflow/providers/snowflake/utils/common.py
+airflow/providers/snowflake/utils/sql_api_generate_jwt.py
 apache_airflow_providers_snowflake.egg-info/PKG-INFO
 apache_airflow_providers_snowflake.egg-info/SOURCES.txt
 apache_airflow_providers_snowflake.egg-info/dependency_links.txt
 apache_airflow_providers_snowflake.egg-info/entry_points.txt
 apache_airflow_providers_snowflake.egg-info/not-zip-safe
 apache_airflow_providers_snowflake.egg-info/requires.txt
 apache_airflow_providers_snowflake.egg-info/top_level.txt
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/pyproject.toml` & `apache-airflow-providers-snowflake-4.2.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/setup.cfg` & `apache-airflow-providers-snowflake-4.2.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.2.0/
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
@@ -55,10 +55,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.snowflake.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.snowflake
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc2/setup.py` & `apache-airflow-providers-snowflake-4.2.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-snowflake package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.1.0"
+version = "4.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-snowflake setup."""
     setup(
         version=version,
         extras_require={
```

