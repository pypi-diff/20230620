# Comparing `tmp/apache-airflow-providers-pagerduty-3.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-pagerduty-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-pagerduty-3.2.0rc2.tar", last modified: Fri May 19 17:53:09 2023, max compression
+gzip compressed data, was "apache-airflow-providers-pagerduty-3.3.0rc1.tar", last modified: Tue Jun 20 11:42:48 2023, max compression
```

## Comparing `apache-airflow-providers-pagerduty-3.2.0rc2.tar` & `apache-airflow-providers-pagerduty-3.3.0rc1.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-pagerduty-3.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:08.000000 apache-airflow-providers-pagerduty-3.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-pagerduty-3.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10029 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8493 2023-05-19 17:53:08.000000 apache-airflow-providers-pagerduty-3.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-05-19 12:18:55.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2587 2023-05-19 17:53:08.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7253 2023-05-18 08:56:29.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/pagerduty.py
--rw-r--r--   0 root         (0) root         (0)     8326 2023-05-19 11:18:18.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/pagerduty_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10029 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      714 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-pagerduty-3.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1862 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1656 2023-05-19 17:53:08.000000 apache-airflow-providers-pagerduty-3.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.942650 apache-airflow-providers-pagerduty-3.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-pagerduty-3.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:47.000000 apache-airflow-providers-pagerduty-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-pagerduty-3.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10478 2023-06-20 11:42:48.943701 apache-airflow-providers-pagerduty-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8941 2023-06-20 11:42:47.000000 apache-airflow-providers-pagerduty-3.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.864393 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.865464 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.897002 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-06-20 11:42:47.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.909189 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-06-02 11:31:21.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/pagerduty.py
+-rw-r--r--   0 root         (0) root         (0)    12253 2023-06-02 11:31:21.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.915660 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-17 16:45:00.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-06-17 16:45:00.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/notifications/pagerduty.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.939944 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10478 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      823 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-pagerduty-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-06-20 11:42:48.945687 apache-airflow-providers-pagerduty-3.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-06-20 11:42:47.000000 apache-airflow-providers-pagerduty-3.3.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/LICENSE` & `apache-airflow-providers-pagerduty-3.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/MANIFEST.in` & `apache-airflow-providers-pagerduty-3.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/PKG-INFO` & `apache-airflow-providers-pagerduty-3.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pagerduty
-Version: 3.2.0rc2
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-pagerduty package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.3.0/
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
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.2.0rc2``
+Release: ``3.3.0rc1``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``pagerduty`` provider. All classes for this provider package
 are in ``airflow.providers.pagerduty`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-pagerduty``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -109,14 +109,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* ``Add notifier for pagerduty (#31207)``
+* ``Add send_event method in PagerdutyEventsHook (#31290)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/README.rst` & `apache-airflow-providers-pagerduty-3.3.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.2.0rc2``
+Release: ``3.3.0rc1``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``pagerduty`` provider. All classes for this provider package
 are in ``airflow.providers.pagerduty`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-pagerduty``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -76,14 +76,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* ``Add notifier for pagerduty (#31207)``
+* ``Add send_event method in PagerdutyEventsHook (#31290)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/__init__.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.2.0"
+__version__ = "3.3.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/get_provider_info.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-pagerduty",
         "name": "Pagerduty",
         "description": "`Pagerduty <https://www.pagerduty.com/>`__\n",
         "suspended": False,
         "versions": [
+            "3.3.0",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.1.3",
             "2.1.2",
             "2.1.1",
             "2.1.0",
@@ -65,8 +66,9 @@
                 "integration-name": "Pagerduty",
                 "python-modules": [
                     "airflow.providers.pagerduty.hooks.pagerduty",
                     "airflow.providers.pagerduty.hooks.pagerduty_events",
                 ],
             }
         ],
+        "notifications": ["airflow.providers.pagerduty.notifications.pagerduty.PagerdutyNotifier"],
     }
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/__init__.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/pagerduty.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/pagerduty.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     conn_name_attr = "pagerduty_conn_id"
     default_conn_name = "pagerduty_default"
     conn_type = "pagerduty"
     hook_name = "Pagerduty"
 
     @staticmethod
     def get_ui_field_behaviour() -> dict[str, Any]:
-        """Returns custom field behaviour"""
+        """Returns custom field behaviour."""
         return {
             "hidden_fields": ["port", "login", "schema", "host"],
             "relabeling": {
                 "password": "Pagerduty API token",
             },
         }
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/pagerduty_events.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Hook for sending or receiving data from PagerDuty as well as creating PagerDuty incidents."""
 from __future__ import annotations
 
+import warnings
 from datetime import datetime
 from typing import Any
 
 import pdpyras
 
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 
 
 class PagerdutyEventsHook(BaseHook):
     """
     This class can be used to interact with the Pagerduty Events API.
 
@@ -42,15 +43,15 @@
     conn_name_attr = "pagerduty_events_conn_id"
     default_conn_name = "pagerduty_events_default"
     conn_type = "pagerduty_events"
     hook_name = "Pagerduty Events"
 
     @staticmethod
     def get_ui_field_behaviour() -> dict[str, Any]:
-        """Returns custom field behaviour"""
+        """Returns custom field behaviour."""
         return {
             "hidden_fields": ["port", "login", "schema", "host", "extra"],
             "relabeling": {
                 "password": "Pagerduty Integration key",
             },
         }
 
@@ -111,14 +112,116 @@
             `alt`: [Optional] Alternative text for the image.
         :param links: List of links to include. Each dictionary in the list accepts the following keys:
             `href`: URL of the link to be attached.
             `text`: [Optional] Plain text that describes the purpose of the link, and can be used as the
             link's text.
         :return: PagerDuty Events API v2 response.
         """
+        warnings.warn(
+            "This method will be deprecated. Please use the "
+            "`PagerdutyEventsHook.send_event` to interact with the Events API",
+            AirflowProviderDeprecationWarning,
+            stacklevel=1,
+        )
+
+        data = PagerdutyEventsHook.prepare_event_data(
+            summary=summary,
+            severity=severity,
+            source=source,
+            custom_details=custom_details,
+            component=component,
+            group=group,
+            class_type=class_type,
+            action=action,
+            dedup_key=dedup_key,
+            images=images,
+            links=links,
+            action_key_name="event_action",
+        )
+
+        session = pdpyras.EventsAPISession(self.integration_key)
+        resp = session.post("/v2/enqueue", json=data)
+        resp.raise_for_status()
+        return resp.json()
+
+    def send_event(
+        self,
+        summary: str,
+        severity: str,
+        source: str = "airflow",
+        action: str = "trigger",
+        dedup_key: str | None = None,
+        custom_details: Any | None = None,
+        group: str | None = None,
+        component: str | None = None,
+        class_type: str | None = None,
+        images: list[Any] | None = None,
+        links: list[Any] | None = None,
+    ) -> dict:
+        """
+        Create event for service integration.
+
+        :param summary: Summary for the event
+        :param severity: Severity for the event, needs to be one of: info, warning, error, critical
+        :param source: Specific human-readable unique identifier, such as a
+            hostname, for the system having the problem.
+        :param action: Event action, needs to be one of: trigger, acknowledge,
+            resolve. Default to trigger if not specified.
+        :param dedup_key: A string which identifies the alert triggered for the given event.
+            Required for the actions acknowledge and resolve.
+        :param custom_details: Free-form details from the event. Can be a dictionary or a string.
+            If a dictionary is passed it will show up in PagerDuty as a table.
+        :param group: A cluster or grouping of sources. For example, sources
+            "prod-datapipe-02" and "prod-datapipe-03" might both be part of "prod-datapipe"
+        :param component: The part or component of the affected system that is broken.
+        :param class_type: The class/type of the event.
+        :param images: List of images to include. Each dictionary in the list accepts the following keys:
+            `src`: The source (URL) of the image being attached to the incident. This image must be served via
+            HTTPS.
+            `href`: [Optional] URL to make the image a clickable link.
+            `alt`: [Optional] Alternative text for the image.
+        :param links: List of links to include. Each dictionary in the list accepts the following keys:
+            `href`: URL of the link to be attached.
+            `text`: [Optional] Plain text that describes the purpose of the link, and can be used as the
+            link's text.
+        :return: PagerDuty Events API v2 response.
+        """
+        data = PagerdutyEventsHook.prepare_event_data(
+            summary=summary,
+            severity=severity,
+            source=source,
+            custom_details=custom_details,
+            component=component,
+            group=group,
+            class_type=class_type,
+            action=action,
+            dedup_key=dedup_key,
+            images=images,
+            links=links,
+        )
+
+        session = pdpyras.EventsAPISession(self.integration_key)
+        return session.send_event(**data)
+
+    @staticmethod
+    def prepare_event_data(
+        summary,
+        severity,
+        source,
+        custom_details,
+        component,
+        group,
+        class_type,
+        action,
+        dedup_key,
+        images,
+        links,
+        action_key_name: str = "action",
+    ) -> dict:
+        """Prepare event data for send_event / post('/v2/enqueue') method."""
         payload = {
             "summary": summary,
             "severity": severity,
             "source": source,
         }
         if custom_details is not None:
             payload["custom_details"] = custom_details
@@ -129,33 +232,30 @@
         if class_type:
             payload["class"] = class_type
 
         actions = ("trigger", "acknowledge", "resolve")
         if action not in actions:
             raise ValueError(f"Event action must be one of: {', '.join(actions)}")
         data = {
-            "event_action": action,
+            action_key_name: action,
             "payload": payload,
         }
         if dedup_key:
             data["dedup_key"] = dedup_key
         elif action != "trigger":
             raise ValueError(
-                f"The dedup_key property is required for event_action={action} events, "
-                f"and it must be a string."
+                f"The dedup_key property is required for {action_key_name}={action} events,"
+                f" and it must be a string."
             )
         if images is not None:
             data["images"] = images
         if links is not None:
             data["links"] = links
 
-        session = pdpyras.EventsAPISession(self.integration_key)
-        resp = session.post("/v2/enqueue", json=data)
-        resp.raise_for_status()
-        return resp.json()
+        return data
 
     def create_change_event(
         self,
         summary: str,
         source: str = "airflow",
         custom_details: Any | None = None,
         timestamp: datetime | None = None,
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/PKG-INFO` & `apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pagerduty
-Version: 3.2.0rc2
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-pagerduty package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.3.0/
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
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.2.0rc2``
+Release: ``3.3.0rc1``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``pagerduty`` provider. All classes for this provider package
 are in ``airflow.providers.pagerduty`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-pagerduty``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -109,14 +109,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* ``Add notifier for pagerduty (#31207)``
+* ``Add send_event method in PagerdutyEventsHook (#31290)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt` & `apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 setup.cfg
 setup.py
 airflow/providers/pagerduty/__init__.py
 airflow/providers/pagerduty/get_provider_info.py
 airflow/providers/pagerduty/hooks/__init__.py
 airflow/providers/pagerduty/hooks/pagerduty.py
 airflow/providers/pagerduty/hooks/pagerduty_events.py
+airflow/providers/pagerduty/notifications/__init__.py
+airflow/providers/pagerduty/notifications/pagerduty.py
 apache_airflow_providers_pagerduty.egg-info/PKG-INFO
 apache_airflow_providers_pagerduty.egg-info/SOURCES.txt
 apache_airflow_providers_pagerduty.egg-info/dependency_links.txt
 apache_airflow_providers_pagerduty.egg-info/entry_points.txt
 apache_airflow_providers_pagerduty.egg-info/not-zip-safe
 apache_airflow_providers_pagerduty.egg-info/requires.txt
 apache_airflow_providers_pagerduty.egg-info/top_level.txt
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/pyproject.toml` & `apache-airflow-providers-pagerduty-3.3.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/setup.cfg` & `apache-airflow-providers-pagerduty-3.3.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.3.0/
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
 	pdpyras>=4.1.2
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.pagerduty.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.pagerduty
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc2/setup.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-pagerduty package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.0"
+version = "3.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-pagerduty setup."""
     setup(
         version=version,
         extras_require={},
```

