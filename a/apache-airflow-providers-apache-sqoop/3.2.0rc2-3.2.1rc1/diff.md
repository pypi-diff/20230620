# Comparing `tmp/apache-airflow-providers-apache-sqoop-3.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-apache-sqoop-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-sqoop-3.2.0rc2.tar", last modified: Fri May 19 17:51:55 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-sqoop-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:31 2023, max compression
```

## Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2.tar` & `apache-airflow-providers-apache-sqoop-3.2.1rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10389 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8844 2023-05-19 17:51:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-19 12:03:00.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2594 2023-05-19 17:51:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15813 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/hooks/sqoop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11404 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/operators/sqoop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10389 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-19 17:51:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.954770 apache-airflow-providers-apache-sqoop-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10796 2023-06-20 11:41:31.955793 apache-airflow-providers-apache-sqoop-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9250 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.877949 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.881474 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.882725 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.916856 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.922633 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15763 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/hooks/sqoop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.928480 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11403 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/operators/sqoop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.952468 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10796 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1865 2023-06-20 11:41:31.957659 apache-airflow-providers-apache-sqoop-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/LICENSE` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/MANIFEST.in` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/PKG-INFO` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-sqoop
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-sqoop package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.1/
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
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.sqoop`` provider. All classes for this provider package
 are in ``airflow.providers.apache.sqoop`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-sqoop``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -108,14 +108,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+
+3.2.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+
+Misc
+~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/README.rst` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.sqoop`` provider. All classes for this provider package
 are in ``airflow.providers.apache.sqoop`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-sqoop``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -75,14 +75,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+
+3.2.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+
+Misc
+~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/__init__.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/__init__.py`

 * *Files 1% similar despite different names*

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

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/get_provider_info.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-sqoop",
         "name": "Apache Sqoop",
         "description": "`Apache Sqoop <https://sqoop.apache.org/>`__\n",
         "suspended": False,
         "versions": [
+            "3.2.1",
             "3.2.0",
             "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.1.3",
             "2.1.2",
             "2.1.1",
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/hooks/__init__.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/hooks/sqoop.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/hooks/sqoop.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""This module contains a sqoop 1.x hook"""
+"""This module contains a sqoop 1.x hook."""
 from __future__ import annotations
 
 import subprocess
 from copy import deepcopy
 from typing import Any
 
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 
 
 class SqoopHook(BaseHook):
-    """
-    This hook is a wrapper around the sqoop 1 binary. To be able to use the hook
-    it is required that "sqoop" is in the PATH.
+    """Wrapper around the sqoop 1 binary.
+
+    To be able to use the hook, it is required that "sqoop" is in the PATH.
 
     Additional arguments that can be passed via the 'extra' JSON field of the
     sqoop connection:
 
         * ``job_tracker``: Job tracker local|jobtracker:port.
         * ``namenode``: Namenode.
         * ``files``: Comma separated files to be copied to the map reduce cluster.
@@ -81,26 +81,25 @@
         self.sub_process_pid: int
         self.log.info("Using connection to: %s:%s/%s", self.conn.host, self.conn.port, self.conn.schema)
 
     def get_conn(self) -> Any:
         return self.conn
 
     def cmd_mask_password(self, cmd_orig: list[str]) -> list[str]:
-        """Mask command password for safety"""
+        """Mask command password for safety."""
         cmd = deepcopy(cmd_orig)
         try:
             password_index = cmd.index("--password")
             cmd[password_index + 1] = "MASKED"
         except ValueError:
             self.log.debug("No password in sqoop cmd")
         return cmd
 
     def popen(self, cmd: list[str], **kwargs: Any) -> None:
-        """
-        Remote Popen
+        """Remote Popen.
 
         :param cmd: command to remotely execute
         :param kwargs: extra arguments to Popen (see subprocess.Popen)
         :return: handle to subprocess
         """
         masked_cmd = " ".join(self.cmd_mask_password(cmd))
         self.log.info("Executing command: %s", masked_cmd)
@@ -219,17 +218,17 @@
         split_by: str | None = None,
         where: str | None = None,
         direct: bool = False,
         driver: Any = None,
         extra_import_options: dict[str, Any] | None = None,
         schema: str | None = None,
     ) -> Any:
-        """
-        Imports table from remote location to target dir. Arguments are
-        copies of direct sqoop command line arguments
+        """Import table from remote location to target dir.
+
+        Arguments are copies of direct sqoop command line arguments.
 
         :param table: Table to read
         :param schema: Schema name
         :param target_dir: HDFS destination dir
         :param append: Append data to an existing dataset in HDFS
         :param file_type: "avro", "sequence", "text" or "parquet".
             Imports data to into the specified format. Defaults to text.
@@ -262,16 +261,15 @@
         append: bool = False,
         file_type: str = "text",
         split_by: str | None = None,
         direct: bool | None = None,
         driver: Any | None = None,
         extra_import_options: dict[str, Any] | None = None,
     ) -> Any:
-        """
-        Imports a specific query from the rdbms to hdfs
+        """Import a specific query from the rdbms to hdfs.
 
         :param query: Free format query to run
         :param target_dir: HDFS destination dir
         :param append: Append data to an existing dataset in HDFS
         :param file_type: "avro", "sequence", "text" or "parquet"
             Imports data to hdfs into the specified format. Defaults to text.
         :param split_by: Column of the table used to split work units
@@ -371,17 +369,17 @@
         input_lines_terminated_by: str | None = None,
         input_optionally_enclosed_by: str | None = None,
         batch: bool = False,
         relaxed_isolation: bool = False,
         extra_export_options: dict[str, Any] | None = None,
         schema: str | None = None,
     ) -> None:
-        """
-        Exports Hive table to remote location. Arguments are copies of direct
-        sqoop command line Arguments
+        """Export Hive table to remote location.
+
+        Arguments are copies of direct Sqoop command line Arguments
 
         :param table: Table remote destination
         :param schema: Schema name
         :param export_dir: Hive table to export
         :param input_null_string: The string to be interpreted as null for
             string columns
         :param input_null_non_string: The string to be interpreted as null
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/operators/__init__.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/operators/sqoop.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/operators/sqoop.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""This module contains a sqoop 1 operator"""
+"""This module contains a sqoop 1 operator."""
 from __future__ import annotations
 
 import os
 import signal
 from typing import TYPE_CHECKING, Any, Sequence
 
 from airflow.exceptions import AirflowException
@@ -29,16 +29,16 @@
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SqoopOperator(BaseOperator):
     """
     Execute a Sqoop job.
-    Documentation for Apache Sqoop can be found here:
-    https://sqoop.apache.org/docs/1.4.2/SqoopUserGuide.html
+
+    Documentation for Apache Sqoop can be found here: https://sqoop.apache.org/docs/1.4.2/SqoopUserGuide.html
 
     :param conn_id: str
     :param cmd_type: str specify command to execute "export" or "import"
     :param schema: Schema name
     :param table: Table to read
     :param query: Import result of arbitrary SQL query. Instead of using the table,
         columns and where arguments, you can specify a SQL statement with the query
@@ -188,15 +188,15 @@
         self.extra_import_options = extra_import_options or {}
         self.extra_export_options = extra_export_options or {}
         self.hook: SqoopHook | None = None
         self.schema = schema
         self.libjars = libjars
 
     def execute(self, context: Context) -> None:
-        """Execute sqoop job"""
+        """Execute sqoop job."""
         if self.hook is None:
             self.hook = self._get_hook()
 
         if self.cmd_type == "export":
             self.hook.export_table(
                 table=self.table,  # type: ignore
                 export_dir=self.export_dir,
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-sqoop
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-sqoop package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.1/
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
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.sqoop`` provider. All classes for this provider package
 are in ``airflow.providers.apache.sqoop`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-sqoop``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -108,14 +108,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+
+3.2.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+
+Misc
+~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/pyproject.toml` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/setup.cfg` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.1/
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
 	provider_info=airflow.providers.apache.sqoop.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.sqoop
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc2/setup.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-sqoop package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.0"
+version = "3.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-sqoop setup."""
     setup(
         version=version,
         extras_require={},
```

