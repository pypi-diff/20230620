# Comparing `tmp/apache-airflow-providers-qubole-3.4.0rc2.tar.gz` & `tmp/apache-airflow-providers-qubole-3.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-qubole-3.4.0rc2.tar", last modified: Fri May 19 17:53:18 2023, max compression
+gzip compressed data, was "apache-airflow-providers-qubole-3.4.1rc1.tar", last modified: Tue Jun 20 11:42:57 2023, max compression
```

## Comparing `apache-airflow-providers-qubole-3.4.0rc2.tar` & `apache-airflow-providers-qubole-3.4.1rc1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:18.000000 apache-airflow-providers-qubole-3.4.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-qubole-3.4.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:16.000000 apache-airflow-providers-qubole-3.4.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-qubole-3.4.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14040 2023-05-19 17:53:18.000000 apache-airflow-providers-qubole-3.4.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12486 2023-05-19 17:53:16.000000 apache-airflow-providers-qubole-3.4.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-05-19 12:20:35.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3289 2023-05-19 17:53:16.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11208 2023-04-13 08:25:21.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/qubole.py
--rw-r--r--   0 root         (0) root         (0)     4084 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/qubole_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12541 2023-05-04 19:17:30.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/qubole.py
--rw-r--r--   0 root         (0) root         (0)     8381 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/qubole_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4240 2023-02-24 18:43:53.000000 apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/sensors/qubole.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:18.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14040 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      902 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      141 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:17.000000 apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-qubole-3.4.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1894 2023-05-19 17:53:18.000000 apache-airflow-providers-qubole-3.4.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-19 17:53:16.000000 apache-airflow-providers-qubole-3.4.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.949615 apache-airflow-providers-qubole-3.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-qubole-3.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:56.000000 apache-airflow-providers-qubole-3.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-qubole-3.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14376 2023-06-20 11:42:57.950640 apache-airflow-providers-qubole-3.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12821 2023-06-20 11:42:56.000000 apache-airflow-providers-qubole-3.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.865399 apache-airflow-providers-qubole-3.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.866678 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.900743 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2023-06-20 11:42:56.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.909317 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11222 2023-06-02 11:31:21.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/qubole.py
+-rw-r--r--   0 root         (0) root         (0)     4091 2023-06-02 11:31:21.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/qubole_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.917766 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12547 2023-06-02 11:31:21.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/qubole.py
+-rw-r--r--   0 root         (0) root         (0)     8386 2023-06-02 11:31:21.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/qubole_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.923568 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-06-01 06:14:28.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/sensors/qubole.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.947039 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14376 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-qubole-3.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-06-20 11:42:57.952557 apache-airflow-providers-qubole-3.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:42:56.000000 apache-airflow-providers-qubole-3.4.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/LICENSE` & `apache-airflow-providers-qubole-3.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/MANIFEST.in` & `apache-airflow-providers-qubole-3.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/PKG-INFO` & `apache-airflow-providers-qubole-3.4.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-qubole
-Version: 3.4.0rc2
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-qubole package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.1/
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
 
 
 Package ``apache-airflow-providers-qubole``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `Qubole <https://www.qubole.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``qubole`` provider. All classes for this provider package
 are in ``airflow.providers.qubole`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-qubole``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -130,14 +130,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.1
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
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/README.rst` & `apache-airflow-providers-qubole-3.4.1rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-qubole``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `Qubole <https://www.qubole.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``qubole`` provider. All classes for this provider package
 are in ``airflow.providers.qubole`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-qubole``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -96,14 +96,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.1
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
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/__init__.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.4.0"
+__version__ = "3.4.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/get_provider_info.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-qubole",
         "name": "Qubole",
         "description": "`Qubole <https://www.qubole.com/>`__\n",
         "suspended": False,
         "versions": [
+            "3.4.1",
             "3.4.0",
             "3.3.1",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.0",
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/__init__.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/qubole.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/qubole.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Qubole hook"""
+"""Qubole hook."""
 from __future__ import annotations
 
 import datetime
 import logging
 import os
 import pathlib
 import time
@@ -68,32 +68,32 @@
     "jupytercmd": JupyterNotebookCommand,
 }
 
 POSITIONAL_ARGS = {"hadoopcmd": ["sub_command"], "shellcmd": ["parameters"], "pigcmd": ["parameters"]}
 
 
 def flatten_list(list_of_lists) -> list:
-    """Flatten the list"""
+    """Flatten the list."""
     return [element for array in list_of_lists for element in array]
 
 
 def filter_options(options: list) -> list:
-    """Remove options from the list"""
+    """Remove options from the list."""
     options_to_remove = ["help", "print-logs-live", "print-logs", "pool"]
     return [option for option in options if option not in options_to_remove]
 
 
 def get_options_list(command_class) -> list:
-    """Get options list"""
+    """Get options list."""
     options_list = [option.get_opt_string().strip("--") for option in command_class.optparser.option_list]
     return filter_options(options_list)
 
 
 def build_command_args() -> tuple[dict[str, list], list]:
-    """Build Command argument from command and options"""
+    """Build Command argument from command and options."""
     command_args, hyphen_args = {}, set()
     for cmd in COMMAND_CLASSES:
 
         # get all available options from the class
         opts_list = get_options_list(COMMAND_CLASSES[cmd])
 
         # append positional args if any for the command
@@ -110,24 +110,24 @@
     return command_args, list(hyphen_args)
 
 
 COMMAND_ARGS, HYPHEN_ARGS = build_command_args()
 
 
 class QuboleHook(BaseHook):
-    """Hook for Qubole communication"""
+    """Hook for Qubole communication."""
 
     conn_name_attr: str = "qubole_conn_id"
     default_conn_name = "qubole_default"
     conn_type = "qubole"
     hook_name = "Qubole"
 
     @staticmethod
     def get_ui_field_behaviour() -> dict[str, Any]:
-        """Returns custom field behaviour"""
+        """Returns custom field behaviour."""
         return {
             "hidden_fields": ["login", "schema", "port", "extra"],
             "relabeling": {
                 "host": "API Endpoint",
                 "password": "Auth Token",
             },
             "placeholders": {"host": "https://<env>.qubole.com/api"},
@@ -142,30 +142,30 @@
         self.kwargs = kwargs
         self.cls = COMMAND_CLASSES[self.kwargs["command_type"]]
         self.cmd: Command | None = None
         self.task_instance: TaskInstance | TaskInstancePydantic | None = None
 
     @staticmethod
     def handle_failure_retry(context) -> None:
-        """Handle retries in case of failures"""
+        """Handle retries in case of failures."""
         ti = context["ti"]
         cmd_id = ti.xcom_pull(key="qbol_cmd_id", task_ids=ti.task_id)
 
         if cmd_id is not None:
             cmd = Command.find(cmd_id)
             if cmd is not None:
                 if cmd.status == "done":
                     log.info("Command ID: %s has been succeeded, hence marking this TI as Success.", cmd_id)
                     ti.state = State.SUCCESS
                 elif cmd.status == "running":
                     log.info("Cancelling the Qubole Command Id: %s", cmd_id)
                     cmd.cancel()
 
     def execute(self, context: Context) -> None:
-        """Execute call"""
+        """Execute call."""
         args = self.cls.parse(self.create_cmd_args(context))
         self.cmd = self.cls.create(**args)
         self.task_instance = context["task_instance"]
         context["task_instance"].xcom_push(key="qbol_cmd_id", value=self.cmd.id)  # type: ignore[attr-defined]
         self.log.info(
             "Qubole command created with Id: %s and Status: %s",
             self.cmd.id,  # type: ignore[attr-defined]
@@ -189,15 +189,15 @@
                 "Command Id: {} failed with Status: {}".format(
                     self.cmd.id, self.cmd.status  # type: ignore[attr-defined]
                 )
             )
 
     def kill(self, ti):
         """
-        Kill (cancel) a Qubole command
+        Kill (cancel) a Qubole command.
 
         :param ti: Task Instance of the dag, used to determine the Quboles command id
         :return: response from Qubole
         """
         if self.cmd is None:
             if not ti and not self.task_instance:
                 raise Exception("Unable to cancel Qubole Command, context is unavailable!")
@@ -215,15 +215,15 @@
         fp=None,
         inline: bool = True,
         delim=None,
         fetch: bool = True,
         include_headers: bool = False,
     ) -> str:
         """
-        Get results (or just s3 locations) of a command from Qubole and save into a file
+        Get results (or just s3 locations) of a command from Qubole and save into a file.
 
         :param ti: Task Instance of the dag, used to determine the Quboles command id
         :param fp: Optional file pointer, will create one and return if None passed
         :param inline: True to download actual results, False to get s3 locations only
         :param delim: Replaces the CTL-A chars with the given delim, defaults to ','
         :param fetch: when inline is True, get results directly from s3 (if large)
         :return: file location containing actual results or s3 locations of results
@@ -246,36 +246,36 @@
         )  # type: ignore[attr-defined]
         fp.flush()
         fp.close()
         return fp.name
 
     def get_log(self, ti) -> None:
         """
-        Get Logs of a command from Qubole
+        Get Logs of a command from Qubole.
 
         :param ti: Task Instance of the dag, used to determine the Quboles command id
         :return: command log as text
         """
         if self.cmd is None:
             cmd_id = ti.xcom_pull(key="qbol_cmd_id", task_ids=self.task_id)
         Command.get_log_id(cmd_id)
 
     def get_jobs_id(self, ti) -> None:
         """
-        Get jobs associated with a Qubole commands
+        Get jobs associated with a Qubole commands.
 
         :param ti: Task Instance of the dag, used to determine the Quboles command id
         :return: Job information associated with command
         """
         if self.cmd is None:
             cmd_id = ti.xcom_pull(key="qbol_cmd_id", task_ids=self.task_id)
         Command.get_jobs_id(cmd_id)
 
     def create_cmd_args(self, context) -> list[str]:
-        """Creates command arguments"""
+        """Creates command arguments."""
         args = []
         cmd_type = self.kwargs["command_type"]
         inplace_args = None
         tags = {self.dag_id, self.task_id, context["run_id"]}
         positional_args_list = flatten_list(POSITIONAL_ARGS.values())
 
         for key, value in self.kwargs.items():
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/hooks/qubole_check.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/qubole_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,41 +29,41 @@
 log = logging.getLogger(__name__)
 
 COL_DELIM = "\t"
 ROW_DELIM = "\r\n"
 
 
 def isint(value) -> bool:
-    """Whether Qubole column are integer"""
+    """Whether Qubole column are integer."""
     try:
         int(value)
         return True
     except ValueError:
         return False
 
 
 def isfloat(value) -> bool:
-    """Whether Qubole column are float"""
+    """Whether Qubole column are float."""
     try:
         float(value)
         return True
     except ValueError:
         return False
 
 
 def isbool(value) -> bool:
-    """Whether Qubole column are boolean"""
+    """Whether Qubole column are boolean."""
     try:
         return value.lower() in ["true", "false"]
     except ValueError:
         return False
 
 
 def parse_first_row(row_list) -> list[bool | float | int | str]:
-    """Parse Qubole first record list"""
+    """Parse Qubole first record list."""
     record_list = []
     first_row = row_list[0] if row_list else ""
 
     for col_value in first_row.split(COL_DELIM):
         if isint(col_value):
             col_value = int(col_value)
         elif isfloat(col_value):
@@ -72,15 +72,15 @@
             col_value = col_value.lower() == "true"
         record_list.append(col_value)
 
     return record_list
 
 
 class QuboleCheckHook(QuboleHook, DbApiHook):
-    """Qubole check hook"""
+    """Qubole check hook."""
 
     def __init__(self, context, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.results_parser_callable = parse_first_row
         if "results_parser_callable" in kwargs and kwargs["results_parser_callable"] is not None:
             if not callable(kwargs["results_parser_callable"]):
                 raise AirflowException("`results_parser_callable` param must be callable")
@@ -96,23 +96,23 @@
             cmd = Command.find(cmd_id)
             if cmd is not None:
                 if cmd.status == "running":
                     log.info("Cancelling the Qubole Command Id: %s", cmd_id)
                     cmd.cancel()
 
     def get_first(self, sql):
-        """Get Qubole query first record list"""
+        """Get Qubole query first record list."""
         self.execute(context=self.context)
         query_result = self.get_query_results()
         row_list = list(filter(None, query_result.split(ROW_DELIM)))
         record_list = self.results_parser_callable(row_list)
         return record_list
 
     def get_query_results(self) -> str | None:
-        """Get Qubole query result"""
+        """Get Qubole query result."""
         if self.cmd is not None:
             cmd_id = self.cmd.id
             self.log.info("command id: %d", cmd_id)
             query_result_buffer = StringIO()
             self.cmd.get_results(fp=query_result_buffer, inline=True, delim=COL_DELIM, arguments=["true"])
             query_result = query_result_buffer.getvalue()
             query_result_buffer.close()
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/__init__.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/qubole.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/qubole.py`

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
-"""Qubole operator"""
+"""Qubole operator."""
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING, Sequence
 
 from airflow.hooks.base import BaseHook
 from airflow.models import BaseOperator, BaseOperatorLink, XCom
@@ -34,15 +34,15 @@
 if TYPE_CHECKING:
 
     from airflow.models.taskinstancekey import TaskInstanceKey
     from airflow.utils.context import Context
 
 
 class QDSLink(BaseOperatorLink):
-    """Link to QDS"""
+    """Link to QDS."""
 
     name = "Go to QDS"
 
     def get_link(
         self,
         operator: BaseOperator,
         *,
@@ -264,27 +264,27 @@
         ti=None,
         fp=None,
         inline: bool = True,
         delim=None,
         fetch: bool = True,
         include_headers: bool = False,
     ) -> str:
-        """get_results from Qubole"""
+        """get_results from Qubole."""
         return self.get_hook().get_results(ti, fp, inline, delim, fetch, include_headers)
 
     def get_log(self, ti) -> None:
-        """get_log from Qubole"""
+        """get_log from Qubole."""
         return self.get_hook().get_log(ti)
 
     def get_jobs_id(self, ti) -> None:
-        """Get jobs_id from Qubole"""
+        """Get jobs_id from Qubole."""
         return self.get_hook().get_jobs_id(ti)
 
     def get_hook(self) -> QuboleHook:
-        """Reinitialising the hook, as some template fields might have changed"""
+        """Reinitialising the hook, as some template fields might have changed."""
         return QuboleHook(**self.kwargs)
 
     def __getattribute__(self, name: str) -> str:
         if name in _get_template_fields(self):
             if name in self.kwargs:
                 return self.kwargs[name]
             else:
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/operators/qubole_check.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/qubole_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,29 +22,29 @@
 from airflow.exceptions import AirflowException
 from airflow.providers.common.sql.operators.sql import SQLCheckOperator, SQLValueCheckOperator
 from airflow.providers.qubole.hooks.qubole_check import QuboleCheckHook
 from airflow.providers.qubole.operators.qubole import QuboleOperator
 
 
 class _QuboleCheckOperatorMixin:
-    """This is a Mixin for Qubole related check operators"""
+    """This is a Mixin for Qubole related check operators."""
 
     kwargs: dict
     results_parser_callable: Callable | None
 
     def execute(self, context=None) -> None:
-        """Execute a check operation against Qubole"""
+        """Execute a check operation against Qubole."""
         try:
             self._hook_context = context
             super().execute(context=context)  # type: ignore[misc]
         except AirflowException as e:
             handle_airflow_exception(e, self.get_hook())
 
     def get_db_hook(self) -> QuboleCheckHook:
-        """Get QuboleCheckHook"""
+        """Get QuboleCheckHook."""
         return self.get_hook()
 
     def get_hook(self) -> QuboleCheckHook:
         """
         Reinitialising the hook, as some template fields might have changed
         This method overwrites the original QuboleOperator.get_hook() which returns a QuboleHook.
         """
@@ -173,25 +173,25 @@
         self.results_parser_callable = results_parser_callable
         self.on_failure_callback = QuboleCheckHook.handle_failure_retry
         self.on_retry_callback = QuboleCheckHook.handle_failure_retry
         self._hook_context = None
 
 
 def get_sql_from_qbol_cmd(params) -> str:
-    """Get Qubole sql from Qubole command"""
+    """Get Qubole sql from Qubole command."""
     sql = ""
     if "query" in params:
         sql = params["query"]
     elif "sql" in params:
         sql = params["sql"]
     return sql
 
 
 def handle_airflow_exception(airflow_exception, hook: QuboleCheckHook):
-    """Qubole check handle Airflow exception"""
+    """Qubole check handle Airflow exception."""
     cmd = hook.cmd
     if cmd is not None:
         if cmd.is_success(cmd.status):
             qubole_command_results = hook.get_query_results()
             qubole_command_id = cmd.id
             exception_message = (
                 f"\nQubole Command Id: {qubole_command_id}\nQubole Command Results:\n{qubole_command_results}"
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/sensors/__init__.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/airflow/providers/qubole/sensors/qubole.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/sensors/qubole.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/PKG-INFO` & `apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-qubole
-Version: 3.4.0rc2
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-qubole package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.1/
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
 
 
 Package ``apache-airflow-providers-qubole``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `Qubole <https://www.qubole.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``qubole`` provider. All classes for this provider package
 are in ``airflow.providers.qubole`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-qubole``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -130,14 +130,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.1
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
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/apache_airflow_providers_qubole.egg-info/SOURCES.txt` & `apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/pyproject.toml` & `apache-airflow-providers-qubole-3.4.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/setup.cfg` & `apache-airflow-providers-qubole-3.4.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.1/
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
 	provider_info=airflow.providers.qubole.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.qubole
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-qubole-3.4.0rc2/setup.py` & `apache-airflow-providers-qubole-3.4.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-qubole package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.0"
+version = "3.4.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-qubole setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

