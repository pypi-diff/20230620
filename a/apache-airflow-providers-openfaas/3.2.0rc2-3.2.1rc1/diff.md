# Comparing `tmp/apache-airflow-providers-openfaas-3.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-openfaas-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-openfaas-3.2.0rc2.tar", last modified: Fri May 19 17:53:04 2023, max compression
+gzip compressed data, was "apache-airflow-providers-openfaas-3.2.1rc1.tar", last modified: Tue Jun 20 11:42:43 2023, max compression
```

## Comparing `apache-airflow-providers-openfaas-3.2.0rc2.tar` & `apache-airflow-providers-openfaas-3.2.1rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:04.000000 apache-airflow-providers-openfaas-3.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-openfaas-3.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-openfaas-3.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9147 2023-05-19 17:53:04.000000 apache-airflow-providers-openfaas-3.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7614 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/airflow/providers/openfaas/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-19 12:14:45.000000 apache-airflow-providers-openfaas-3.2.0rc2/airflow/providers/openfaas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/airflow/providers/openfaas/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:04.000000 apache-airflow-providers-openfaas-3.2.0rc2/airflow/providers/openfaas/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-openfaas-3.2.0rc2/airflow/providers/openfaas/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4884 2023-02-24 18:43:53.000000 apache-airflow-providers-openfaas-3.2.0rc2/airflow/providers/openfaas/hooks/openfaas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:04.000000 apache-airflow-providers-openfaas-3.2.0rc2/apache_airflow_providers_openfaas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9147 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/apache_airflow_providers_openfaas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      648 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/apache_airflow_providers_openfaas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/apache_airflow_providers_openfaas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/apache_airflow_providers_openfaas.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/apache_airflow_providers_openfaas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/apache_airflow_providers_openfaas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/apache_airflow_providers_openfaas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-openfaas-3.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1840 2023-05-19 17:53:04.000000 apache-airflow-providers-openfaas-3.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1650 2023-05-19 17:53:03.000000 apache-airflow-providers-openfaas-3.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:43.305360 apache-airflow-providers-openfaas-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-openfaas-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:42.000000 apache-airflow-providers-openfaas-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-openfaas-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9483 2023-06-20 11:42:43.306616 apache-airflow-providers-openfaas-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7949 2023-06-20 11:42:42.000000 apache-airflow-providers-openfaas-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:43.229118 apache-airflow-providers-openfaas-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:43.230451 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:43.267907 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-06-20 11:42:42.000000 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:43.275174 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2023-06-02 11:31:21.000000 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/hooks/openfaas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:43.302457 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9483 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      648 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-openfaas-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-06-20 11:42:43.308871 apache-airflow-providers-openfaas-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:42:42.000000 apache-airflow-providers-openfaas-3.2.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/LICENSE` & `apache-airflow-providers-openfaas-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/MANIFEST.in` & `apache-airflow-providers-openfaas-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/PKG-INFO` & `apache-airflow-providers-openfaas-3.2.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openfaas
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-openfaas package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.1/
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
 
 
 Package ``apache-airflow-providers-openfaas``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `OpenFaaS <https://www.openfaas.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openfaas`` provider. All classes for this provider package
 are in ``airflow.providers.openfaas`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openfaas``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -108,14 +108,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.1
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
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/README.rst` & `apache-airflow-providers-openfaas-3.2.1rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-openfaas``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `OpenFaaS <https://www.openfaas.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openfaas`` provider. All classes for this provider package
 are in ``airflow.providers.openfaas`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openfaas``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -75,14 +75,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.1
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
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/airflow/providers/openfaas/__init__.py` & `apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.2.0"
+__version__ = "3.2.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/airflow/providers/openfaas/get_provider_info.py` & `apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-openfaas",
         "name": "OpenFaaS",
         "description": "`OpenFaaS <https://www.openfaas.com/>`__\n",
         "suspended": False,
         "versions": [
+            "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.0.3",
             "2.0.2",
             "2.0.1",
             "2.0.0",
```

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/airflow/providers/openfaas/hooks/__init__.py` & `apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/airflow/providers/openfaas/hooks/openfaas.py` & `apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/hooks/openfaas.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from airflow.hooks.base import BaseHook
 
 OK_STATUS_CODE = 202
 
 
 class OpenFaasHook(BaseHook):
     """
-    Interact with OpenFaaS to query, deploy, invoke and update function
+    Interact with OpenFaaS to query, deploy, invoke and update function.
 
     :param function_name: Name of the function, Defaults to None
     :param conn_id: openfaas connection to use, Defaults to open_faas_default
         for example host : http://openfaas.faas.com, Connection Type : Http
     """
 
     GET_FUNCTION = "/system/function/"
@@ -48,15 +48,15 @@
         self.conn_id = conn_id
 
     def get_conn(self):
         conn = self.get_connection(self.conn_id)
         return conn
 
     def deploy_function(self, overwrite_function_if_exist: bool, body: dict[str, Any]) -> None:
-        """Deploy OpenFaaS function"""
+        """Deploy OpenFaaS function."""
         if overwrite_function_if_exist:
             self.log.info("Function already exist %s going to update", self.function_name)
             self.update_function(body)
         else:
             url = self.get_conn().host + self.DEPLOY_FUNCTION
             self.log.info("Deploying function %s", url)
             response = requests.post(url, body)
@@ -64,51 +64,51 @@
                 self.log.error("Response status %d", response.status_code)
                 self.log.error("Failed to deploy")
                 raise AirflowException("failed to deploy")
             else:
                 self.log.info("Function deployed %s", self.function_name)
 
     def invoke_async_function(self, body: dict[str, Any]) -> None:
-        """Invoking function asynchronously"""
+        """Invoking function asynchronously."""
         url = self.get_conn().host + self.INVOKE_ASYNC_FUNCTION + self.function_name
         self.log.info("Invoking function asynchronously %s", url)
         response = requests.post(url, body)
         if response.ok:
             self.log.info("Invoked %s", self.function_name)
         else:
             self.log.error("Response status %d", response.status_code)
             raise AirflowException("failed to invoke function")
 
     def invoke_function(self, body: dict[str, Any]) -> None:
-        """Invoking function synchronously, will block until function completes and returns"""
+        """Invoking function synchronously, will block until function completes and returns."""
         url = self.get_conn().host + self.INVOKE_FUNCTION + self.function_name
         self.log.info("Invoking function synchronously %s", url)
         response = requests.post(url, body)
         if response.ok:
             self.log.info("Invoked %s", self.function_name)
             self.log.info("Response code %s", response.status_code)
             self.log.info("Response %s", response.text)
         else:
             self.log.error("Response status %d", response.status_code)
             raise AirflowException("failed to invoke function")
 
     def update_function(self, body: dict[str, Any]) -> None:
-        """Update OpenFaaS function"""
+        """Update OpenFaaS function."""
         url = self.get_conn().host + self.UPDATE_FUNCTION
         self.log.info("Updating function %s", url)
         response = requests.put(url, body)
         if response.status_code != OK_STATUS_CODE:
             self.log.error("Response status %d", response.status_code)
             self.log.error("Failed to update response %s", response.content.decode("utf-8"))
             raise AirflowException("failed to update " + self.function_name)
         else:
             self.log.info("Function was updated")
 
     def does_function_exist(self) -> bool:
-        """Whether OpenFaaS function exists or not"""
+        """Whether OpenFaaS function exists or not."""
         url = self.get_conn().host + self.GET_FUNCTION + self.function_name
 
         response = requests.get(url)
         if response.ok:
             return True
         else:
             self.log.error("Failed to find function %s", self.function_name)
```

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/apache_airflow_providers_openfaas.egg-info/PKG-INFO` & `apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openfaas
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-openfaas package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.1/
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
 
 
 Package ``apache-airflow-providers-openfaas``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `OpenFaaS <https://www.openfaas.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openfaas`` provider. All classes for this provider package
 are in ``airflow.providers.openfaas`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openfaas``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -108,14 +108,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.1
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
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/apache_airflow_providers_openfaas.egg-info/SOURCES.txt` & `apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/pyproject.toml` & `apache-airflow-providers-openfaas-3.2.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/setup.cfg` & `apache-airflow-providers-openfaas-3.2.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.1/
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
 
@@ -52,10 +52,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.openfaas.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.openfaas
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-openfaas-3.2.0rc2/setup.py` & `apache-airflow-providers-openfaas-3.2.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-openfaas package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.0"
+version = "3.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-openfaas setup."""
     setup(
         version=version,
         extras_require={},
```

