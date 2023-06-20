# Comparing `tmp/apache-airflow-providers-airbyte-3.3.0rc2.tar.gz` & `tmp/apache-airflow-providers-airbyte-3.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-airbyte-3.3.0rc2.tar", last modified: Fri May 19 17:51:22 2023, max compression
+gzip compressed data, was "apache-airflow-providers-airbyte-3.3.1rc1.tar", last modified: Tue Jun 20 11:40:58 2023, max compression
```

## Comparing `apache-airflow-providers-airbyte-3.3.0rc2.tar` & `apache-airflow-providers-airbyte-3.3.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-airbyte-3.3.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:21.000000 apache-airflow-providers-airbyte-3.3.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-airbyte-3.3.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11567 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10016 2023-05-19 17:51:21.000000 apache-airflow-providers-airbyte-3.3.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-05-19 11:55:01.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-05-19 17:51:21.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5059 2023-03-11 12:12:47.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/hooks/airbyte.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3869 2023-03-11 12:12:47.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/operators/airbyte.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2793 2023-03-11 12:12:47.000000 apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/sensors/airbyte.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/apache_airflow_providers_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11567 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/apache_airflow_providers_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      822 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/apache_airflow_providers_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/apache_airflow_providers_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/apache_airflow_providers_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/apache_airflow_providers_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       95 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/apache_airflow_providers_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/apache_airflow_providers_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-airbyte-3.3.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1865 2023-05-19 17:51:22.000000 apache-airflow-providers-airbyte-3.3.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1685 2023-05-19 17:51:21.000000 apache-airflow-providers-airbyte-3.3.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.726176 apache-airflow-providers-airbyte-3.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-airbyte-3.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:40:57.000000 apache-airflow-providers-airbyte-3.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-airbyte-3.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11904 2023-06-20 11:40:58.727218 apache-airflow-providers-airbyte-3.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10352 2023-06-20 11:40:57.000000 apache-airflow-providers-airbyte-3.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.634029 apache-airflow-providers-airbyte-3.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.635088 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.669079 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-06-20 11:40:57.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.676813 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5062 2023-06-02 11:31:21.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/hooks/airbyte.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.682876 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-06-02 11:31:21.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/operators/airbyte.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.690628 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-06-01 06:14:28.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/sensors/airbyte.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.723493 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11904 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      822 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-airbyte-3.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-06-20 11:40:58.729147 apache-airflow-providers-airbyte-3.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-06-20 11:40:57.000000 apache-airflow-providers-airbyte-3.3.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/LICENSE` & `apache-airflow-providers-airbyte-3.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/MANIFEST.in` & `apache-airflow-providers-airbyte-3.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/PKG-INFO` & `apache-airflow-providers-airbyte-3.3.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-airbyte
-Version: 3.3.0rc2
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-airbyte package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.1/
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
 
 
 Package ``apache-airflow-providers-airbyte``
 
-Release: ``3.3.0rc2``
+Release: ``3.3.1rc1``
 
 
 `Airbyte <https://airbyte.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``airbyte`` provider. All classes for this provider package
 are in ``airflow.providers.airbyte`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-airbyte``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -129,14 +129,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+
+3.3.1
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
 3.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/README.rst` & `apache-airflow-providers-airbyte-3.3.1rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-airbyte``
 
-Release: ``3.3.0rc2``
+Release: ``3.3.1rc1``
 
 
 `Airbyte <https://airbyte.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``airbyte`` provider. All classes for this provider package
 are in ``airflow.providers.airbyte`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-airbyte``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -95,14 +95,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+
+3.3.1
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
 3.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/__init__.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.3.0"
+__version__ = "3.3.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/get_provider_info.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-airbyte",
         "name": "Airbyte",
         "description": "`Airbyte <https://airbyte.io/>`__\n",
         "suspended": False,
         "versions": [
+            "3.3.1",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.1.4",
             "2.1.3",
```

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/hooks/__init__.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/hooks/airbyte.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/hooks/airbyte.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from airflow.exceptions import AirflowException
 from airflow.providers.http.hooks.http import HttpHook
 
 
 class AirbyteHook(HttpHook):
     """
-    Hook for Airbyte API
+    Hook for Airbyte API.
 
     :param airbyte_conn_id: Optional. The name of the Airflow connection to get
         connection information for Airbyte. Defaults to "airbyte_default".
     :param api_version: Optional. Airbyte API version. Defaults to "v1".
     """
 
     conn_name_attr = "airbyte_conn_id"
@@ -105,26 +105,26 @@
             endpoint=f"api/{self.api_version}/jobs/get",
             json={"id": job_id},
             headers={"accept": "application/json"},
         )
 
     def cancel_job(self, job_id: int) -> Any:
         """
-        Cancel the job when task is cancelled
+        Cancel the job when task is cancelled.
 
         :param job_id: Required. Id of the Airbyte job
         """
         return self.run(
             endpoint=f"api/{self.api_version}/jobs/cancel",
             json={"id": job_id},
             headers={"accept": "application/json"},
         )
 
     def test_connection(self):
-        """Tests the Airbyte connection by hitting the health API"""
+        """Tests the Airbyte connection by hitting the health API."""
         self.method = "GET"
         try:
             res = self.run(
                 endpoint=f"api/{self.api_version}/health",
                 headers={"accept": "application/json"},
                 extra_options={"check_response": False},
             )
```

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/operators/__init__.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/operators/airbyte.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/operators/airbyte.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,25 +65,25 @@
         self.connection_id = connection_id
         self.timeout = timeout
         self.api_version = api_version
         self.wait_seconds = wait_seconds
         self.asynchronous = asynchronous
 
     def execute(self, context: Context) -> None:
-        """Create Airbyte Job and wait to finish"""
+        """Create Airbyte Job and wait to finish."""
         self.hook = AirbyteHook(airbyte_conn_id=self.airbyte_conn_id, api_version=self.api_version)
         job_object = self.hook.submit_sync_connection(connection_id=self.connection_id)
         self.job_id = job_object.json()["job"]["id"]
 
         self.log.info("Job %s was submitted to Airbyte Server", self.job_id)
         if not self.asynchronous:
             self.log.info("Waiting for job %s to complete", self.job_id)
             self.hook.wait_for_job(job_id=self.job_id, wait_seconds=self.wait_seconds, timeout=self.timeout)
             self.log.info("Job %s completed successfully", self.job_id)
 
         return self.job_id
 
     def on_kill(self):
-        """Cancel the job if task is cancelled"""
+        """Cancel the job if task is cancelled."""
         if self.job_id:
             self.log.info("on_kill: cancel the airbyte Job %s", self.job_id)
             self.hook.cancel_job(self.job_id)
```

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/sensors/__init__.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/airflow/providers/airbyte/sensors/airbyte.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/sensors/airbyte.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/apache_airflow_providers_airbyte.egg-info/PKG-INFO` & `apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-airbyte
-Version: 3.3.0rc2
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-airbyte package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.1/
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
 
 
 Package ``apache-airflow-providers-airbyte``
 
-Release: ``3.3.0rc2``
+Release: ``3.3.1rc1``
 
 
 `Airbyte <https://airbyte.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``airbyte`` provider. All classes for this provider package
 are in ``airflow.providers.airbyte`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-airbyte``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -129,14 +129,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+
+3.3.1
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
 3.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/apache_airflow_providers_airbyte.egg-info/SOURCES.txt` & `apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/pyproject.toml` & `apache-airflow-providers-airbyte-3.3.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/setup.cfg` & `apache-airflow-providers-airbyte-3.3.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.1/
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
 	apache-airflow-providers-http
 	apache-airflow>=2.4.0.dev0
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.airbyte.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.airbyte
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-airbyte-3.3.0rc2/setup.py` & `apache-airflow-providers-airbyte-3.3.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-airbyte package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.3.0"
+version = "3.3.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-airbyte setup."""
     setup(
         version=version,
         extras_require={"http": ["apache-airflow-providers-http"]},
```

