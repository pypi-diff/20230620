# Comparing `tmp/apache-airflow-providers-alibaba-2.4.0rc2.tar.gz` & `tmp/apache-airflow-providers-alibaba-2.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-alibaba-2.4.0rc2.tar", last modified: Fri May 19 17:51:24 2023, max compression
+gzip compressed data, was "apache-airflow-providers-alibaba-2.4.1rc1.tar", last modified: Tue Jun 20 11:41:00 2023, max compression
```

## Comparing `apache-airflow-providers-alibaba-2.4.0rc2.tar` & `apache-airflow-providers-alibaba-2.4.1rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-alibaba-2.4.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:23.000000 apache-airflow-providers-alibaba-2.4.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-alibaba-2.4.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9850 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8320 2023-05-19 17:51:23.000000 apache-airflow-providers-alibaba-2.4.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-05-19 11:57:33.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12634 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/hooks/oss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8645 2023-03-10 19:31:58.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/log/oss_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6314 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/operators/oss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/sensors/oss_key.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-05-19 17:51:23.000000 apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/apache_airflow_providers_alibaba.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9850 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/apache_airflow_providers_alibaba.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      998 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/apache_airflow_providers_alibaba.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/apache_airflow_providers_alibaba.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/apache_airflow_providers_alibaba.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/apache_airflow_providers_alibaba.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/apache_airflow_providers_alibaba.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/apache_airflow_providers_alibaba.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-alibaba-2.4.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1848 2023-05-19 17:51:24.000000 apache-airflow-providers-alibaba-2.4.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-05-19 17:51:23.000000 apache-airflow-providers-alibaba-2.4.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.613326 apache-airflow-providers-alibaba-2.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:40:59.000000 apache-airflow-providers-alibaba-2.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10231 2023-06-20 11:41:00.614390 apache-airflow-providers-alibaba-2.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8700 2023-06-20 11:40:59.000000 apache-airflow-providers-alibaba-2.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.507688 apache-airflow-providers-alibaba-2.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.509220 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.557541 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.560595 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.566586 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12646 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/oss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.572527 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8634 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.578845 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6320 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/oss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.585396 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-06-20 11:40:59.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.610519 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10231 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      998 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-alibaba-2.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-06-20 11:41:00.616407 apache-airflow-providers-alibaba-2.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:40:59.000000 apache-airflow-providers-alibaba-2.4.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/LICENSE` & `apache-airflow-providers-alibaba-2.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/MANIFEST.in` & `apache-airflow-providers-alibaba-2.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/PKG-INFO` & `apache-airflow-providers-alibaba-2.4.1rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-alibaba
-Version: 2.4.0rc2
+Version: 2.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-alibaba package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.1/
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
 
 
 Package ``apache-airflow-providers-alibaba``
 
-Release: ``2.4.0rc2``
+Release: ``2.4.1rc1``
 
 
 Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``alibaba`` provider. All classes for this provider package
 are in ``airflow.providers.alibaba`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-alibaba``
 
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
 
+2.4.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+
+Misc
+~~~~
+
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 2.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/README.rst` & `apache-airflow-providers-alibaba-2.4.1rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-alibaba``
 
-Release: ``2.4.0rc2``
+Release: ``2.4.1rc1``
 
 
 Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``alibaba`` provider. All classes for this provider package
 are in ``airflow.providers.alibaba`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-alibaba``
 
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
 
+2.4.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+
+Misc
+~~~~
+
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 2.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/__init__.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/__init__.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/hooks/__init__.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/hooks/oss.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/oss.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,28 +133,28 @@
         except ClientError as e:
             self.log.error(e.message)
             return False
 
     @provide_bucket_name
     def get_bucket(self, bucket_name: str | None = None) -> oss2.api.Bucket:
         """
-        Returns a oss2.Bucket object
+        Returns a oss2.Bucket object.
 
         :param bucket_name: the name of the bucket
         :return: the bucket object to the bucket name.
         """
         auth = self.get_credential()
         assert self.region is not None
         return oss2.Bucket(auth, f"https://oss-{self.region}.aliyuncs.com", bucket_name)
 
     @provide_bucket_name
     @unify_bucket_name_and_key
     def load_string(self, key: str, content: str, bucket_name: str | None = None) -> None:
         """
-        Loads a string to OSS
+        Loads a string to OSS.
 
         :param key: the path of the object
         :param content: str to set as content for the key.
         :param bucket_name: the name of the bucket
         """
         try:
             self.get_bucket(bucket_name).put_object(key, content)
@@ -166,15 +166,15 @@
     def upload_local_file(
         self,
         key: str,
         file: str,
         bucket_name: str | None = None,
     ) -> None:
         """
-        Upload a local file to OSS
+        Upload a local file to OSS.
 
         :param key: the OSS path of the object
         :param file: local file to upload.
         :param bucket_name: the name of the bucket
         """
         try:
             self.get_bucket(bucket_name).put_object_from_file(key, file)
@@ -186,15 +186,15 @@
     def download_file(
         self,
         key: str,
         local_file: str,
         bucket_name: str | None = None,
     ) -> str | None:
         """
-        Download file from OSS
+        Download file from OSS.
 
         :param key: key of the file-like object to download.
         :param local_file: local path + file name to save.
         :param bucket_name: the name of the bucket
         :return: the file name.
         """
         try:
@@ -208,15 +208,15 @@
     @unify_bucket_name_and_key
     def delete_object(
         self,
         key: str,
         bucket_name: str | None = None,
     ) -> None:
         """
-        Delete object from OSS
+        Delete object from OSS.
 
         :param key: key of the object to delete.
         :param bucket_name: the name of the bucket
         """
         try:
             self.get_bucket(bucket_name).delete_object(key)
         except Exception as e:
@@ -227,15 +227,15 @@
     @unify_bucket_name_and_key
     def delete_objects(
         self,
         key: list,
         bucket_name: str | None = None,
     ) -> None:
         """
-        Delete objects from OSS
+        Delete objects from OSS.
 
         :param key: keys list of the objects to delete.
         :param bucket_name: the name of the bucket
         """
         try:
             self.get_bucket(bucket_name).batch_delete_objects(key)
         except Exception as e:
@@ -244,15 +244,15 @@
 
     @provide_bucket_name
     def delete_bucket(
         self,
         bucket_name: str | None = None,
     ) -> None:
         """
-        Delete bucket from OSS
+        Delete bucket from OSS.
 
         :param bucket_name: the name of the bucket
         """
         try:
             self.get_bucket(bucket_name).delete_bucket()
         except Exception as e:
             self.log.error(e)
@@ -260,29 +260,29 @@
 
     @provide_bucket_name
     def create_bucket(
         self,
         bucket_name: str | None = None,
     ) -> None:
         """
-        Create bucket
+        Create bucket.
 
         :param bucket_name: the name of the bucket
         """
         try:
             self.get_bucket(bucket_name).create_bucket()
         except Exception as e:
             self.log.error(e)
             raise AirflowException(f"Errors when create bucket: {bucket_name}")
 
     @provide_bucket_name
     @unify_bucket_name_and_key
     def append_string(self, bucket_name: str | None, content: str, key: str, pos: int) -> None:
         """
-        Append string to a remote existing file
+        Append string to a remote existing file.
 
         :param bucket_name: the name of the bucket
         :param content: content to be appended
         :param key: oss bucket key
         :param pos: position of the existing file where the content will be appended
         """
         self.log.info("Write oss bucket. key: %s, pos: %s", key, pos)
@@ -292,15 +292,15 @@
             self.log.error(e)
             raise AirflowException(f"Errors when append string for object: {key}")
 
     @provide_bucket_name
     @unify_bucket_name_and_key
     def read_key(self, bucket_name: str | None, key: str) -> str:
         """
-        Read oss remote object content with the specified key
+        Read oss remote object content with the specified key.
 
         :param bucket_name: the name of the bucket
         :param key: oss bucket key
         """
         self.log.info("Read oss key: %s", key)
         try:
             return self.get_bucket(bucket_name).get_object(key).read().decode("utf-8")
@@ -308,15 +308,15 @@
             self.log.error(e)
             raise AirflowException(f"Errors when read bucket object: {key}")
 
     @provide_bucket_name
     @unify_bucket_name_and_key
     def head_key(self, bucket_name: str | None, key: str) -> oss2.models.HeadObjectResult:
         """
-        Get meta info of the specified remote object
+        Get meta info of the specified remote object.
 
         :param bucket_name: the name of the bucket
         :param key: oss bucket key
         """
         self.log.info("Head Object oss key: %s", key)
         try:
             return self.get_bucket(bucket_name).head_object(key)
@@ -324,15 +324,15 @@
             self.log.error(e)
             raise AirflowException(f"Errors when head bucket object: {key}")
 
     @provide_bucket_name
     @unify_bucket_name_and_key
     def key_exist(self, bucket_name: str | None, key: str) -> bool:
         """
-        Find out whether the specified key exists in the oss remote storage
+        Find out whether the specified key exists in the oss remote storage.
 
         :param bucket_name: the name of the bucket
         :param key: oss bucket key
         """
         # full_path = None
         self.log.info("Looking up oss bucket %s for bucket key %s ...", bucket_name, key)
         try:
```

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/log/__init__.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/log/oss_task_handler.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,26 +17,27 @@
 # under the License.
 from __future__ import annotations
 
 import contextlib
 import os
 import pathlib
 import shutil
+from functools import cached_property
 
 from packaging.version import Version
 
-from airflow.compat.functools import cached_property
 from airflow.configuration import conf
 from airflow.providers.alibaba.cloud.hooks.oss import OSSHook
 from airflow.utils.log.file_task_handler import FileTaskHandler
 from airflow.utils.log.logging_mixin import LoggingMixin
 
 
 def get_default_delete_local_copy():
-    """Load delete_local_logs conf if Airflow version > 2.6 and return False if not
+    """Load delete_local_logs conf if Airflow version > 2.6 and return False if not.
+
     TODO: delete this function when min airflow version >= 2.6
     """
     from airflow.version import version
 
     if Version(version) < Version("2.6"):
         return False
     return conf.getboolean("logging", "delete_local_logs")
@@ -73,15 +74,15 @@
                 'Could not create an OSSHook with connection id "%s". '
                 "Please make sure that airflow[oss] is installed and "
                 "the OSS connection exists.",
                 remote_conn_id,
             )
 
     def set_context(self, ti):
-        """This function is used to set the context of the handler"""
+        """This function is used to set the context of the handler."""
         super().set_context(ti)
         # Local location and remote location is needed to open and
         # upload local log file to OSS remote storage.
         self.log_relative_path = self._render_filename(ti, ti.try_number)
         self.upload_on_close = not ti.raw
 
         # Clear the file first so that duplicate data is not uploaded
@@ -139,15 +140,15 @@
         # returned remote_log will contain error messages.
         remote_log = self.oss_read(remote_loc, return_error=True)
         log = f"*** Reading remote log from {remote_loc}.\n{remote_log}\n"
         return log, {"end_of_log": True}
 
     def oss_log_exists(self, remote_log_location):
         """
-        Check if remote_log_location exists in remote storage
+        Check if remote_log_location exists in remote storage.
 
         :param remote_log_location: log's location in remote storage
         :return: True if location exists else False
         """
         oss_remote_log_location = f"{self.base_folder}/{remote_log_location}"
         with contextlib.suppress(Exception):
             return self.hook.key_exist(self.bucket_name, oss_remote_log_location)
```

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/operators/__init__.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/operators/oss.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/oss.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class OSSCreateBucketOperator(BaseOperator):
     """
-    This operator creates an OSS bucket
+    This operator creates an OSS bucket.
 
     :param region: OSS region you want to create bucket
     :param bucket_name: This is bucket name you want to create
     :param oss_conn_id: The Airflow connection used for OSS credentials.
     """
 
     def __init__(
@@ -51,15 +51,15 @@
     def execute(self, context: Context):
         oss_hook = OSSHook(oss_conn_id=self.oss_conn_id, region=self.region)
         oss_hook.create_bucket(bucket_name=self.bucket_name)
 
 
 class OSSDeleteBucketOperator(BaseOperator):
     """
-    This operator to delete an OSS bucket
+    This operator to delete an OSS bucket.
 
     :param region: OSS region you want to create bucket
     :param bucket_name: This is bucket name you want to delete
     :param oss_conn_id: The Airflow connection used for OSS credentials.
     """
 
     def __init__(
@@ -77,15 +77,15 @@
     def execute(self, context: Context):
         oss_hook = OSSHook(oss_conn_id=self.oss_conn_id, region=self.region)
         oss_hook.delete_bucket(bucket_name=self.bucket_name)
 
 
 class OSSUploadObjectOperator(BaseOperator):
     """
-    This operator to upload an file-like object
+    This operator to upload an file-like object.
 
     :param key: the OSS path of the object
     :param file: local file to upload.
     :param region: OSS region you want to create bucket
     :param bucket_name: This is bucket name you want to create
     :param oss_conn_id: The Airflow connection used for OSS credentials.
     """
@@ -109,15 +109,15 @@
     def execute(self, context: Context):
         oss_hook = OSSHook(oss_conn_id=self.oss_conn_id, region=self.region)
         oss_hook.upload_local_file(bucket_name=self.bucket_name, key=self.key, file=self.file)
 
 
 class OSSDownloadObjectOperator(BaseOperator):
     """
-    This operator to Download an OSS object
+    This operator to Download an OSS object.
 
     :param key: key of the object to download.
     :param local_file: local path + file name to save.
     :param region: OSS region
     :param bucket_name: OSS bucket name
     :param oss_conn_id: The Airflow connection used for OSS credentials.
     """
@@ -141,15 +141,15 @@
     def execute(self, context: Context):
         oss_hook = OSSHook(oss_conn_id=self.oss_conn_id, region=self.region)
         oss_hook.download_file(bucket_name=self.bucket_name, key=self.key, local_file=self.file)
 
 
 class OSSDeleteBatchObjectOperator(BaseOperator):
     """
-    This operator to delete OSS objects
+    This operator to delete OSS objects.
 
     :param key: key list of the objects to delete.
     :param region: OSS region
     :param bucket_name: OSS bucket name
     :param oss_conn_id: The Airflow connection used for OSS credentials.
     """
 
@@ -170,15 +170,15 @@
     def execute(self, context: Context):
         oss_hook = OSSHook(oss_conn_id=self.oss_conn_id, region=self.region)
         oss_hook.delete_objects(bucket_name=self.bucket_name, key=self.keys)
 
 
 class OSSDeleteObjectOperator(BaseOperator):
     """
-    This operator to delete an OSS object
+    This operator to delete an OSS object.
 
     :param key: key of the object to delete.
     :param region: OSS region
     :param bucket_name: OSS bucket name
     :param oss_conn_id: The Airflow connection used for OSS credentials.
     """
```

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/sensors/__init__.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/cloud/sensors/oss_key.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+from functools import cached_property
 from typing import TYPE_CHECKING, Sequence
 from urllib.parse import urlsplit
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException
 from airflow.providers.alibaba.cloud.hooks.oss import OSSHook
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -60,17 +60,18 @@
         self.region = region
         self.oss_conn_id = oss_conn_id
         self.hook: OSSHook | None = None
 
     def poke(self, context: Context):
         """
         Check if the object exists in the bucket to pull key.
-        @param self - the object itself
-        @param context - the context of the object
-        @returns True if the object exists, False otherwise
+
+        :param self: the object itself
+        :param context: the context of the object
+        :returns: True if the object exists, False otherwise
         """
         if self.bucket_name is None:
             parsed_url = urlsplit(self.bucket_key)
             if parsed_url.netloc == "":
                 raise AirflowException("If key is a relative path from root, please provide a bucket_name")
             self.bucket_name = parsed_url.netloc
             self.bucket_key = parsed_url.path.lstrip("/")
@@ -84,13 +85,13 @@
                 )
 
         self.log.info("Poking for key : oss://%s/%s", self.bucket_name, self.bucket_key)
         return self.get_hook.object_exists(key=self.bucket_key, bucket_name=self.bucket_name)
 
     @cached_property
     def get_hook(self) -> OSSHook:
-        """Create and return an OSSHook"""
+        """Create and return an OSSHook."""
         if self.hook:
             return self.hook
 
         self.hook = OSSHook(oss_conn_id=self.oss_conn_id, region=self.region)
         return self.hook
```

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/airflow/providers/alibaba/get_provider_info.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-alibaba",
         "name": "Alibaba",
         "description": "Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).\n",
         "suspended": False,
         "versions": [
+            "2.4.1",
             "2.4.0",
             "2.3.0",
             "2.2.0",
             "2.1.0",
             "2.0.1",
             "2.0.0",
             "1.1.1",
```

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/apache_airflow_providers_alibaba.egg-info/PKG-INFO` & `apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-alibaba
-Version: 2.4.0rc2
+Version: 2.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-alibaba package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.1/
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
 
 
 Package ``apache-airflow-providers-alibaba``
 
-Release: ``2.4.0rc2``
+Release: ``2.4.1rc1``
 
 
 Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``alibaba`` provider. All classes for this provider package
 are in ``airflow.providers.alibaba`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-alibaba``
 
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
 
+2.4.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+
+Misc
+~~~~
+
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 2.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/apache_airflow_providers_alibaba.egg-info/SOURCES.txt` & `apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/pyproject.toml` & `apache-airflow-providers-alibaba-2.4.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/setup.cfg` & `apache-airflow-providers-alibaba-2.4.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.1/
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
 	oss2>=2.14.0
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.alibaba.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.alibaba
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-alibaba-2.4.0rc2/setup.py` & `apache-airflow-providers-alibaba-2.4.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-alibaba package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "2.4.0"
+version = "2.4.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-alibaba setup."""
     setup(
         version=version,
         extras_require={},
```

