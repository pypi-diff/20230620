# Comparing `tmp/apache-airflow-providers-imap-3.2.1rc1.tar.gz` & `tmp/apache-airflow-providers-imap-3.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-imap-3.2.1rc1.tar", last modified: Wed May 24 07:20:28 2023, max compression
+gzip compressed data, was "apache-airflow-providers-imap-3.2.2rc1.tar", last modified: Tue Jun 20 11:42:20 2023, max compression
```

## Comparing `apache-airflow-providers-imap-3.2.1rc1.tar` & `apache-airflow-providers-imap-3.2.2rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-imap-3.2.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:20:27.000000 apache-airflow-providers-imap-3.2.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-imap-3.2.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10178 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8606 2023-05-24 07:20:27.000000 apache-airflow-providers-imap-3.2.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-05-24 07:09:22.000000 apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-05-24 07:20:27.000000 apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14090 2023-05-23 11:35:14.000000 apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/hooks/imap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3054 2023-05-23 11:35:14.000000 apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/sensors/imap_attachment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/apache_airflow_providers_imap.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10178 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/apache_airflow_providers_imap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      693 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/apache_airflow_providers_imap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/apache_airflow_providers_imap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/apache_airflow_providers_imap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/apache_airflow_providers_imap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/apache_airflow_providers_imap.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-imap-3.2.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1856 2023-05-24 07:20:28.000000 apache-airflow-providers-imap-3.2.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-05-24 07:20:27.000000 apache-airflow-providers-imap-3.2.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.226959 apache-airflow-providers-imap-3.2.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.2.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:19.000000 apache-airflow-providers-imap-3.2.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.2.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10402 2023-06-20 11:42:20.228169 apache-airflow-providers-imap-3.2.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8880 2023-06-20 11:42:19.000000 apache-airflow-providers-imap-3.2.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.147596 apache-airflow-providers-imap-3.2.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.148910 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.187214 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2023-06-20 11:42:19.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.193153 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14090 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/imap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.198967 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/imap_attachment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.223903 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10402 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      693 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-imap-3.2.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-06-20 11:42:20.230574 apache-airflow-providers-imap-3.2.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-20 11:42:19.000000 apache-airflow-providers-imap-3.2.2rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-imap-3.2.1rc1/LICENSE` & `apache-airflow-providers-imap-3.2.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.1rc1/MANIFEST.in` & `apache-airflow-providers-imap-3.2.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.1rc1/PKG-INFO` & `apache-airflow-providers-imap-3.2.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-imap
-Version: 3.2.1rc1
+Version: 3.2.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-imap package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.2/
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -49,38 +48,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.2.1rc1``
+Release: ``3.2.2rc1``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``imap`` provider. All classes for this provider package
 are in ``airflow.providers.imap`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-imap``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -109,14 +108,28 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.2
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
+
 3.2.1
 .....
 
 Misc
 ~~~~
 
 * ``Bring back min-airflow-version for preinstalled providers (#31469)``
```

### Comparing `apache-airflow-providers-imap-3.2.1rc1/README.rst` & `apache-airflow-providers-imap-3.2.2rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.2.1rc1``
+Release: ``3.2.2rc1``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``imap`` provider. All classes for this provider package
 are in ``airflow.providers.imap`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-imap``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -75,14 +75,28 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.2
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
+
 3.2.1
 .....
 
 Misc
 ~~~~
 
 * ``Bring back min-airflow-version for preinstalled providers (#31469)``
```

### Comparing `apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/__init__.py` & `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.2.1"
+__version__ = "3.2.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/get_provider_info.py` & `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-imap",
         "name": "Internet Message Access Protocol (IMAP)",
         "description": "`Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__\n",
         "suspended": False,
         "versions": [
+            "3.2.2",
             "3.2.1",
             "3.2.0",
             "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.2.3",
             "2.2.2",
```

### Comparing `apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/hooks/__init__.py` & `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/hooks/imap.py` & `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/imap.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/sensors/__init__.py` & `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.1rc1/airflow/providers/imap/sensors/imap_attachment.py` & `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/imap_attachment.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.1rc1/apache_airflow_providers_imap.egg-info/PKG-INFO` & `apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-imap
-Version: 3.2.1rc1
+Version: 3.2.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-imap package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.2/
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -49,38 +48,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.2.1rc1``
+Release: ``3.2.2rc1``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``imap`` provider. All classes for this provider package
 are in ``airflow.providers.imap`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-imap``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -109,14 +108,28 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.2
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
+
 3.2.1
 .....
 
 Misc
 ~~~~
 
 * ``Bring back min-airflow-version for preinstalled providers (#31469)``
```

### Comparing `apache-airflow-providers-imap-3.2.1rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt` & `apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.1rc1/pyproject.toml` & `apache-airflow-providers-imap-3.2.2rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-imap-3.2.1rc1/setup.cfg` & `apache-airflow-providers-imap-3.2.2rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -17,35 +17,34 @@
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
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.2/
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
```

### Comparing `apache-airflow-providers-imap-3.2.1rc1/setup.py` & `apache-airflow-providers-imap-3.2.2rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-imap package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.1"
+version = "3.2.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-imap setup."""
     setup(
         version=version,
         extras_require={},
```

