# Comparing `tmp/apache-airflow-providers-exasol-4.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-exasol-4.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-exasol-4.2.0rc2.tar", last modified: Fri May 19 17:52:22 2023, max compression
+gzip compressed data, was "apache-airflow-providers-exasol-4.2.1rc1.tar", last modified: Tue Jun 20 11:42:00 2023, max compression
```

## Comparing `apache-airflow-providers-exasol-4.2.0rc2.tar` & `apache-airflow-providers-exasol-4.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-exasol-4.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:21.000000 apache-airflow-providers-exasol-4.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-exasol-4.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12685 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11131 2023-05-19 17:52:21.000000 apache-airflow-providers-exasol-4.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-05-19 12:06:11.000000 apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2620 2023-05-19 17:52:21.000000 apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10928 2023-02-24 18:43:53.000000 apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/hooks/exasol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2347 2023-02-24 18:43:53.000000 apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/operators/exasol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/apache_airflow_providers_exasol.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12685 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/apache_airflow_providers_exasol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      716 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/apache_airflow_providers_exasol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/apache_airflow_providers_exasol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/apache_airflow_providers_exasol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/apache_airflow_providers_exasol.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/apache_airflow_providers_exasol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/apache_airflow_providers_exasol.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-exasol-4.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1910 2023-05-19 17:52:22.000000 apache-airflow-providers-exasol-4.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-19 17:52:21.000000 apache-airflow-providers-exasol-4.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.090548 apache-airflow-providers-exasol-4.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13071 2023-06-20 11:42:00.091679 apache-airflow-providers-exasol-4.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11516 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.010967 apache-airflow-providers-exasol-4.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.012178 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.051802 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.057572 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10925 2023-06-05 12:50:36.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/exasol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.063339 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-06-02 11:31:21.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/exasol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.087791 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13071 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-exasol-4.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-06-20 11:42:00.093634 apache-airflow-providers-exasol-4.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/LICENSE` & `apache-airflow-providers-exasol-4.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/MANIFEST.in` & `apache-airflow-providers-exasol-4.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/PKG-INFO` & `apache-airflow-providers-exasol-4.2.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-exasol
-Version: 4.2.0rc2
+Version: 4.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-exasol package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.1/
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
 
 
 Package ``apache-airflow-providers-exasol``
 
-Release: ``4.2.0rc2``
+Release: ``4.2.1rc1``
 
 
 `Exasol <https://docs.exasol.com/home.htm>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``exasol`` provider. All classes for this provider package
 are in ``airflow.providers.exasol`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-exasol``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -131,14 +131,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.2.1
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
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 4.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/README.rst` & `apache-airflow-providers-exasol-4.2.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-exasol``
 
-Release: ``4.2.0rc2``
+Release: ``4.2.1rc1``
 
 
 `Exasol <https://docs.exasol.com/home.htm>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``exasol`` provider. All classes for this provider package
 are in ``airflow.providers.exasol`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-exasol``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -97,14 +97,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.2.1
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
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 4.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/__init__.py` & `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.2.0"
+__version__ = "4.2.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/get_provider_info.py` & `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-exasol",
         "name": "Exasol",
         "description": "`Exasol <https://docs.exasol.com/home.htm>`__\n",
         "suspended": False,
         "versions": [
+            "4.2.1",
             "4.2.0",
             "4.1.3",
             "4.1.2",
             "4.1.1",
             "4.1.0",
             "4.0.1",
             "4.0.0",
```

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/hooks/__init__.py` & `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/hooks/exasol.py` & `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/exasol.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 import pyexasol
 from pyexasol import ExaConnection, ExaStatement
 
 from airflow.providers.common.sql.hooks.sql import DbApiHook, return_single_query_results
 
 
 class ExasolHook(DbApiHook):
-    """
-    Interact with Exasol.
+    """Interact with Exasol.
+
     You can specify the pyexasol ``compression``, ``encryption``, ``json_lib``
     and ``client_name``  parameters in the extra field of your connection
     as ``{"compression": True, "json_lib": "rapidjson", etc}``.
+
     See `pyexasol reference
     <https://github.com/badoo/pyexasol/blob/master/docs/REFERENCE.md#connect>`_
     for more details.
     """
 
     conn_name_attr = "exasol_conn_id"
     default_conn_name = "exasol_default"
@@ -62,45 +63,44 @@
             if arg_name in ["compression", "encryption", "json_lib", "client_name"]:
                 conn_args[arg_name] = arg_val
 
         conn = pyexasol.connect(**conn_args)
         return conn
 
     def get_pandas_df(self, sql: str, parameters: dict | None = None, **kwargs) -> pd.DataFrame:
-        """
-        Executes the sql and returns a pandas dataframe
+        """Execute the SQL and return a Pandas dataframe.
 
-        :param sql: the sql statement to be executed (str) or a list of
-            sql statements to execute
+        :param sql: The sql statement to be executed (str) or a list of
+            sql statements to execute.
         :param parameters: The parameters to render the SQL query with.
-        :param kwargs: (optional) passed into pyexasol.ExaConnection.export_to_pandas method
+
+        Other keyword arguments are all forwarded into
+        ``pyexasol.ExaConnection.export_to_pandas``.
         """
         with closing(self.get_conn()) as conn:
             df = conn.export_to_pandas(sql, query_params=parameters, **kwargs)
             return df
 
     def get_records(
         self,
         sql: str | list[str],
         parameters: Iterable | Mapping | None = None,
     ) -> list[dict | tuple[Any, ...]]:
-        """
-        Executes the sql and returns a set of records.
+        """Execute the SQL and return a set of records.
 
         :param sql: the sql statement to be executed (str) or a list of
             sql statements to execute
         :param parameters: The parameters to render the SQL query with.
         """
         with closing(self.get_conn()) as conn:
             with closing(conn.execute(sql, parameters)) as cur:
                 return cur.fetchall()
 
     def get_first(self, sql: str | list[str], parameters: Iterable | Mapping | None = None) -> Any:
-        """
-        Executes the sql and returns the first resulting row.
+        """Execute the SQL and return the first resulting row.
 
         :param sql: the sql statement to be executed (str) or a list of
             sql statements to execute
         :param parameters: The parameters to render the SQL query with.
         """
         with closing(self.get_conn()) as conn:
             with closing(conn.execute(sql, parameters)) as cur:
@@ -109,16 +109,15 @@
     def export_to_file(
         self,
         filename: str,
         query_or_table: str,
         query_params: dict | None = None,
         export_params: dict | None = None,
     ) -> None:
-        """
-        Exports data to a file.
+        """Export data to a file.
 
         :param filename: Path to the file to which the data has to be exported
         :param query_or_table: the sql statement to be executed or table name to export
         :param query_params: Query parameters passed to underlying ``export_to_file``
             method of :class:`~pyexasol.connection.ExaConnection`.
         :param export_params: Extra parameters passed to underlying ``export_to_file``
             method of :class:`~pyexasol.connection.ExaConnection`.
@@ -131,17 +130,19 @@
                 query_params=query_params,
                 export_params=export_params,
             )
         self.log.info("Data saved to %s", filename)
 
     @staticmethod
     def get_description(statement: ExaStatement) -> Sequence[Sequence]:
-        """
-        Copied implementation from DB2-API wrapper.
-        More info https://github.com/exasol/pyexasol/blob/master/docs/DBAPI_COMPAT.md#db-api-20-wrapper
+        """Copied implementation from DB2-API wrapper.
+
+        For more info, see
+        https://github.com/exasol/pyexasol/blob/master/docs/DBAPI_COMPAT.md#db-api-20-wrapper
+
         :param statement: Exasol statement
         :return: description sequence of t
         """
         cols = []
         for k, v in statement.columns().items():
             cols.append(
                 (
@@ -161,18 +162,18 @@
         sql: str | Iterable[str],
         autocommit: bool = False,
         parameters: Iterable | Mapping | None = None,
         handler: Callable | None = None,
         split_statements: bool = False,
         return_last: bool = True,
     ) -> Any | list[Any] | None:
-        """
-        Runs a command or a list of commands. Pass a list of sql
-        statements to the sql parameter to get them to execute
-        sequentially
+        """Run a command or a list of commands.
+
+        Pass a list of SQL statements to the SQL parameter to get them to
+        execute sequentially.
 
         :param sql: the sql statement to be executed (str) or a list of
             sql statements to execute
         :param autocommit: What to set the connection's autocommit setting to
             before executing the query.
         :param parameters: The parameters to render the SQL query with.
         :param handler: The result handler which is called with the result of each statement.
@@ -220,60 +221,56 @@
         if return_single_query_results(sql, return_last, split_statements):
             self.descriptions = [_last_columns]
             return _last_result
         else:
             return results
 
     def set_autocommit(self, conn, autocommit: bool) -> None:
-        """
-        Sets the autocommit flag on the connection
+        """Set the autocommit flag on the connection.
 
         :param conn: Connection to set autocommit setting to.
         :param autocommit: The autocommit setting to set.
         """
         if not self.supports_autocommit and autocommit:
             self.log.warning(
                 "%s connection doesn't support autocommit but autocommit activated.",
                 getattr(self, self.conn_name_attr),
             )
         conn.set_autocommit(autocommit)
 
     def get_autocommit(self, conn) -> bool:
-        """
-        Get autocommit setting for the provided connection.
-        Return True if autocommit is set.
-        Return False if autocommit is not set or set to False or conn
-        does not support autocommit.
+        """Get autocommit setting for the provided connection.
 
         :param conn: Connection to get autocommit setting from.
-        :return: connection autocommit setting.
+        :return: connection autocommit setting. True if ``autocommit`` is set
+            to True on the connection. False if it is either not set, set to
+            False, or the connection does not support auto-commit.
         """
         autocommit = conn.attr.get("autocommit")
         if autocommit is None:
             autocommit = super().get_autocommit(conn)
         return autocommit
 
     @staticmethod
     def _serialize_cell(cell, conn=None) -> Any:
-        """
-        Exasol will adapt all arguments to the execute() method internally,
+        """Override to disable cell serialization.
+
+        Exasol will adapt all arguments to the ``execute()`` method internally,
         hence we return cell without any conversion.
 
         :param cell: The cell to insert into the table
         :param conn: The database connection
         :return: The cell
         """
         return cell
 
 
 def exasol_fetch_all_handler(statement: ExaStatement) -> list[tuple] | None:
     if statement.result_type == "resultSet":
         return statement.fetchall()
-    else:
-        return None
+    return None
 
 
 def exasol_fetch_one_handler(statement: ExaStatement) -> list[tuple] | None:
     if statement.result_type == "resultSet":
         return statement.fetchone()
-    else:
-        return None
+    return None
```

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/operators/__init__.py` & `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/airflow/providers/exasol/operators/exasol.py` & `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/exasol.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 from airflow.providers.exasol.hooks.exasol import exasol_fetch_all_handler
 
 
 class ExasolOperator(SQLExecuteQueryOperator):
     """
-    Executes sql code in a specific Exasol database
+    Executes sql code in a specific Exasol database.
 
     :param sql: the SQL code to be executed as a single string, or
         a list of str (sql statements), or a reference to a template file.
         template references are recognized by str ending in '.sql'
     :param exasol_conn_id: reference to a specific Exasol database
     :param autocommit: if True, each command is automatically committed.
         (default value: False)
```

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/apache_airflow_providers_exasol.egg-info/PKG-INFO` & `apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-exasol
-Version: 4.2.0rc2
+Version: 4.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-exasol package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.1/
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
 
 
 Package ``apache-airflow-providers-exasol``
 
-Release: ``4.2.0rc2``
+Release: ``4.2.1rc1``
 
 
 `Exasol <https://docs.exasol.com/home.htm>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``exasol`` provider. All classes for this provider package
 are in ``airflow.providers.exasol`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-exasol``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -131,14 +131,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.2.1
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
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 4.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/apache_airflow_providers_exasol.egg-info/SOURCES.txt` & `apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/pyproject.toml` & `apache-airflow-providers-exasol-4.2.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/setup.cfg` & `apache-airflow-providers-exasol-4.2.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.1/
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
 	provider_info=airflow.providers.exasol.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.exasol
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-exasol-4.2.0rc2/setup.py` & `apache-airflow-providers-exasol-4.2.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-exasol package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.2.0"
+version = "4.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-exasol setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

