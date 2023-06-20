# Comparing `tmp/apache-airflow-providers-trino-5.1.0rc2.tar.gz` & `tmp/apache-airflow-providers-trino-5.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-trino-5.1.0rc2.tar", last modified: Fri May 19 17:53:46 2023, max compression
+gzip compressed data, was "apache-airflow-providers-trino-5.1.1rc1.tar", last modified: Tue Jun 20 11:43:27 2023, max compression
```

## Comparing `apache-airflow-providers-trino-5.1.0rc2.tar` & `apache-airflow-providers-trino-5.1.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-trino-5.1.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:45.000000 apache-airflow-providers-trino-5.1.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-trino-5.1.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14302 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12728 2023-05-19 17:53:45.000000 apache-airflow-providers-trino-5.1.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-05-19 12:22:50.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3026 2023-05-19 17:53:45.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9383 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/hooks/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3169 2023-05-03 19:47:07.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/operators/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/transfers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4998 2023-04-21 10:05:41.000000 apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/transfers/gcs_to_trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/apache_airflow_providers_trino.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14302 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/apache_airflow_providers_trino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      797 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/apache_airflow_providers_trino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/apache_airflow_providers_trino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/apache_airflow_providers_trino.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/apache_airflow_providers_trino.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/apache_airflow_providers_trino.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/apache_airflow_providers_trino.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-trino-5.1.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1903 2023-05-19 17:53:46.000000 apache-airflow-providers-trino-5.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1767 2023-05-19 17:53:45.000000 apache-airflow-providers-trino-5.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.095581 apache-airflow-providers-trino-5.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:25.000000 apache-airflow-providers-trino-5.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14638 2023-06-20 11:43:27.096913 apache-airflow-providers-trino-5.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13063 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.000669 apache-airflow-providers-trino-5.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.001882 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.041528 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2023-06-20 11:43:25.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.048823 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9387 2023-06-02 11:31:21.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/hooks/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.055590 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3169 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/operators/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.063905 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/transfers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4999 2023-06-02 11:31:21.000000 apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/transfers/gcs_to_trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:27.092900 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14638 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      797 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:26.000000 apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-trino-5.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1904 2023-06-20 11:43:27.099356 apache-airflow-providers-trino-5.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-06-20 11:43:25.000000 apache-airflow-providers-trino-5.1.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-trino-5.1.0rc2/LICENSE` & `apache-airflow-providers-trino-5.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.0rc2/MANIFEST.in` & `apache-airflow-providers-trino-5.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.0rc2/PKG-INFO` & `apache-airflow-providers-trino-5.1.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 5.1.0rc2
+Version: 5.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-trino package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.1/
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
 Provides-Extra: google
 License-File: LICENSE
 License-File: NOTICE
 
 
@@ -50,38 +50,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.1.0rc2``
+Release: ``5.1.1rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``trino`` provider. All classes for this provider package
 are in ``airflow.providers.trino`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-trino``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -133,14 +133,29 @@
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
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 5.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-trino-5.1.0rc2/README.rst` & `apache-airflow-providers-trino-5.1.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.1.0rc2``
+Release: ``5.1.1rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``trino`` provider. All classes for this provider package
 are in ``airflow.providers.trino`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-trino``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -98,14 +98,29 @@
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
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 5.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/__init__.py` & `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/__init__.py`

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

### Comparing `apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/get_provider_info.py` & `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-trino",
         "name": "Trino",
         "description": "`Trino <https://trino.io/>`__\n",
         "suspended": False,
         "versions": [
+            "5.1.1",
             "5.1.0",
             "5.0.0",
             "4.3.2",
             "4.3.1",
             "4.3.0",
             "4.2.0",
             "4.1.0",
```

### Comparing `apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/hooks/__init__.py` & `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/hooks/trino.py` & `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/hooks/trino.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from airflow.configuration import conf
 from airflow.models import Connection
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 from airflow.utils.operator_helpers import AIRFLOW_VAR_NAME_FORMAT_MAPPING, DEFAULT_FORMAT_PREFIX
 
 
 def generate_trino_client_info() -> str:
-    """Return json string with dag_id, task_id, execution_date and try_number"""
+    """Return json string with dag_id, task_id, execution_date and try_number."""
     context_var = {
         format_map["default"].replace(DEFAULT_FORMAT_PREFIX, ""): os.environ.get(
             format_map["env_var_format"], ""
         )
         for format_map in AIRFLOW_VAR_NAME_FORMAT_MAPPING.values()
     }
     task_info = {
@@ -48,15 +48,15 @@
         "dag_run_id": context_var["dag_run_id"],
         "dag_owner": context_var["dag_owner"],
     }
     return json.dumps(task_info, sort_keys=True)
 
 
 class TrinoException(Exception):
-    """Trino exception"""
+    """Trino exception."""
 
 
 def _boolify(value):
     if isinstance(value, bool):
         return value
     if isinstance(value, str):
         if value.lower() == "false":
@@ -81,15 +81,15 @@
     conn_type = "trino"
     hook_name = "Trino"
     query_id = ""
     placeholder = "?"
     _test_connection_sql = "select 1"
 
     def get_conn(self) -> Connection:
-        """Returns a connection object"""
+        """Returns a connection object."""
         db = self.get_connection(self.trino_conn_id)  # type: ignore[attr-defined]
         extra = db.extra_dejson
         auth = None
         user = db.login
         if db.password and extra.get("auth") in ("kerberos", "certs"):
             raise AirflowException(f"The {extra.get('auth')!r} authorization type doesn't support password.")
         elif db.password:
@@ -137,15 +137,15 @@
             session_properties=extra.get("session_properties") or None,
             client_tags=extra.get("client_tags") or None,
         )
 
         return trino_conn
 
     def get_isolation_level(self) -> Any:
-        """Returns an isolation level"""
+        """Returns an isolation level."""
         db = self.get_connection(self.trino_conn_id)  # type: ignore[attr-defined]
         isolation_level = db.extra_dejson.get("isolation_level", "AUTOCOMMIT").upper()
         return getattr(IsolationLevel, isolation_level, IsolationLevel.AUTOCOMMIT)
 
     def get_records(
         self,
         sql: str | list[str] = "",
```

### Comparing `apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/operators/__init__.py` & `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/operators/trino.py` & `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/operators/trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/transfers/__init__.py` & `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.0rc2/airflow/providers/trino/transfers/gcs_to_trino.py` & `apache-airflow-providers-trino-5.1.1rc1/airflow/providers/trino/transfers/gcs_to_trino.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class GCSToTrinoOperator(BaseOperator):
     """
     Loads a csv file from Google Cloud Storage into a Trino table.
+
     Assumptions:
     1. CSV file should not have headers
     2. Trino table with requisite columns is already created
     3. Optionally, a separate JSON file with headers can be provided
 
     :param source_bucket: Source GCS bucket that contains the csv
     :param source_object: csv file including the path
```

### Comparing `apache-airflow-providers-trino-5.1.0rc2/apache_airflow_providers_trino.egg-info/PKG-INFO` & `apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 5.1.0rc2
+Version: 5.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-trino package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.1/
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
 Provides-Extra: google
 License-File: LICENSE
 License-File: NOTICE
 
 
@@ -50,38 +50,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.1.0rc2``
+Release: ``5.1.1rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``trino`` provider. All classes for this provider package
 are in ``airflow.providers.trino`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-trino``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -133,14 +133,29 @@
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
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 5.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-trino-5.1.0rc2/apache_airflow_providers_trino.egg-info/SOURCES.txt` & `apache-airflow-providers-trino-5.1.1rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.1.0rc2/pyproject.toml` & `apache-airflow-providers-trino-5.1.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-trino-5.1.0rc2/setup.cfg` & `apache-airflow-providers-trino-5.1.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-trino/5.1.1/
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
 	provider_info=airflow.providers.trino.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.trino
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-trino-5.1.0rc2/setup.py` & `apache-airflow-providers-trino-5.1.1rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-trino package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.1.0"
+version = "5.1.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-trino setup."""
     setup(
         version=version,
         extras_require={
```

