# Comparing `tmp/apache-airflow-providers-presto-5.1.0rc2.tar.gz` & `tmp/apache-airflow-providers-presto-5.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-presto-5.1.0rc2.tar", last modified: Fri May 19 17:53:16 2023, max compression
+gzip compressed data, was "apache-airflow-providers-presto-5.1.1rc1.tar", last modified: Tue Jun 20 11:42:56 2023, max compression
```

## Comparing `apache-airflow-providers-presto-5.1.0rc2.tar` & `apache-airflow-providers-presto-5.1.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-presto-5.1.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:15.000000 apache-airflow-providers-presto-5.1.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-presto-5.1.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13940 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12363 2023-05-19 17:53:15.000000 apache-airflow-providers-presto-5.1.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-05-19 12:20:24.000000 apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2906 2023-05-19 17:53:15.000000 apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8828 2023-02-24 18:43:53.000000 apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/hooks/presto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-04-21 10:05:41.000000 apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/transfers/gcs_to_presto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/apache_airflow_providers_presto.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13940 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/apache_airflow_providers_presto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      723 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/apache_airflow_providers_presto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/apache_airflow_providers_presto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/apache_airflow_providers_presto.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/apache_airflow_providers_presto.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      210 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/apache_airflow_providers_presto.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/apache_airflow_providers_presto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-presto-5.1.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1922 2023-05-19 17:53:16.000000 apache-airflow-providers-presto-5.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1773 2023-05-19 17:53:15.000000 apache-airflow-providers-presto-5.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.163627 apache-airflow-providers-presto-5.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:55.000000 apache-airflow-providers-presto-5.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14276 2023-06-20 11:42:56.164703 apache-airflow-providers-presto-5.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12698 2023-06-20 11:42:55.000000 apache-airflow-providers-presto-5.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.088803 apache-airflow-providers-presto-5.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.090015 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.122350 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2023-06-20 11:42:55.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.128435 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8832 2023-06-02 11:31:21.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/presto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.136308 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4836 2023-06-02 11:31:21.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/gcs_to_presto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.160935 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14276 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      723 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-presto-5.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-06-20 11:42:56.166648 apache-airflow-providers-presto-5.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-06-20 11:42:55.000000 apache-airflow-providers-presto-5.1.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-presto-5.1.0rc2/LICENSE` & `apache-airflow-providers-presto-5.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.0rc2/MANIFEST.in` & `apache-airflow-providers-presto-5.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.0rc2/PKG-INFO` & `apache-airflow-providers-presto-5.1.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-presto
-Version: 5.1.0rc2
+Version: 5.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-presto package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.1/
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
 
 
 Package ``apache-airflow-providers-presto``
 
-Release: ``5.1.0rc2``
+Release: ``5.1.1rc1``
 
 
 `Presto <https://prestodb.github.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``presto`` provider. All classes for this provider package
 are in ``airflow.providers.presto`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-presto``
 
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

### Comparing `apache-airflow-providers-presto-5.1.0rc2/README.rst` & `apache-airflow-providers-presto-5.1.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-presto``
 
-Release: ``5.1.0rc2``
+Release: ``5.1.1rc1``
 
 
 `Presto <https://prestodb.github.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``presto`` provider. All classes for this provider package
 are in ``airflow.providers.presto`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-presto``
 
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

### Comparing `apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/__init__.py` & `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/__init__.py`

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

### Comparing `apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/get_provider_info.py` & `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-presto",
         "name": "Presto",
         "description": "`Presto <https://prestodb.github.io/>`__\n",
         "suspended": False,
         "versions": [
+            "5.1.1",
             "5.1.0",
             "5.0.0",
             "4.2.2",
             "4.2.1",
             "4.2.0",
             "4.1.0",
             "4.0.1",
```

### Comparing `apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/hooks/__init__.py` & `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/hooks/presto.py` & `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/presto.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from airflow.configuration import conf
 from airflow.models import Connection
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 from airflow.utils.operator_helpers import AIRFLOW_VAR_NAME_FORMAT_MAPPING, DEFAULT_FORMAT_PREFIX
 
 
 def generate_presto_client_info() -> str:
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
 
 
 class PrestoException(Exception):
-    """Presto exception"""
+    """Presto exception."""
 
 
 def _boolify(value):
     if isinstance(value, bool):
         return value
     if isinstance(value, str):
         if value.lower() == "false":
@@ -79,15 +79,15 @@
     conn_name_attr = "presto_conn_id"
     default_conn_name = "presto_default"
     conn_type = "presto"
     hook_name = "Presto"
     placeholder = "?"
 
     def get_conn(self) -> Connection:
-        """Returns a connection object"""
+        """Returns a connection object."""
         db = self.get_connection(self.presto_conn_id)  # type: ignore[attr-defined]
         extra = db.extra_dejson
         auth = None
         if db.password and extra.get("auth") == "kerberos":
             raise AirflowException("Kerberos authorization doesn't support password.")
         elif db.password:
             auth = prestodb.auth.BasicAuthentication(db.login, db.password)
@@ -124,15 +124,15 @@
             # The PR is merged in the presto library, but has not been released.
             # See: https://github.com/prestosql/presto-python-client/pull/31
             presto_conn._http_session.verify = _boolify(extra["verify"])
 
         return presto_conn
 
     def get_isolation_level(self) -> Any:
-        """Returns an isolation level"""
+        """Returns an isolation level."""
         db = self.get_connection(self.presto_conn_id)  # type: ignore[attr-defined]
         isolation_level = db.extra_dejson.get("isolation_level", "AUTOCOMMIT").upper()
         return getattr(IsolationLevel, isolation_level, IsolationLevel.AUTOCOMMIT)
 
     def get_records(
         self,
         sql: str | list[str] = "",
```

### Comparing `apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/transfers/__init__.py` & `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.0rc2/airflow/providers/presto/transfers/gcs_to_presto.py` & `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/gcs_to_presto.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class GCSToPrestoOperator(BaseOperator):
     """
     Loads a csv file from Google Cloud Storage into a Presto table.
+
     Assumptions:
     1. CSV file should not have headers
     2. Presto table with requisite columns is already created
     3. Optionally, a separate JSON file with headers or list of headers can be provided
 
     :param source_bucket: Source GCS bucket that contains the csv
     :param source_object: csv file including the path
```

### Comparing `apache-airflow-providers-presto-5.1.0rc2/apache_airflow_providers_presto.egg-info/PKG-INFO` & `apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-presto
-Version: 5.1.0rc2
+Version: 5.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-presto package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.1/
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
 
 
 Package ``apache-airflow-providers-presto``
 
-Release: ``5.1.0rc2``
+Release: ``5.1.1rc1``
 
 
 `Presto <https://prestodb.github.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``presto`` provider. All classes for this provider package
 are in ``airflow.providers.presto`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-presto``
 
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

### Comparing `apache-airflow-providers-presto-5.1.0rc2/apache_airflow_providers_presto.egg-info/SOURCES.txt` & `apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.0rc2/pyproject.toml` & `apache-airflow-providers-presto-5.1.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-presto-5.1.0rc2/setup.cfg` & `apache-airflow-providers-presto-5.1.1rc1/setup.cfg`

 * *Files 9% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.1/
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
 	provider_info=airflow.providers.presto.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.presto
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-presto-5.1.0rc2/setup.py` & `apache-airflow-providers-presto-5.1.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-presto package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.1.0"
+version = "5.1.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-presto setup."""
     setup(
         version=version,
         extras_require={
```

