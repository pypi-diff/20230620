# Comparing `tmp/apache-airflow-providers-dbt-cloud-3.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-dbt-cloud-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-dbt-cloud-3.2.0rc2.tar", last modified: Fri May 19 17:52:13 2023, max compression
+gzip compressed data, was "apache-airflow-providers-dbt-cloud-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:51 2023, max compression
```

## Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2.tar` & `apache-airflow-providers-dbt-cloud-3.2.1rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:12.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11230 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9673 2023-05-19 17:52:12.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-05-19 12:05:02.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2990 2023-05-19 17:52:12.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24269 2023-03-10 19:31:58.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/hooks/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13638 2023-05-16 07:40:59.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5508 2023-05-03 19:47:07.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/sensors/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4839 2023-04-24 21:04:25.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/triggers/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11230 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      933 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1895 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1697 2023-05-19 17:52:12.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:51.021236 apache-airflow-providers-dbt-cloud-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:49.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11728 2023-06-20 11:41:51.022307 apache-airflow-providers-dbt-cloud-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10170 2023-06-20 11:41:49.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.931297 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.932461 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.933570 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.970994 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-06-20 11:41:49.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.976859 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24235 2023-06-02 11:31:21.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.983054 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13638 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.988790 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5614 2023-06-05 12:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.994693 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4649 2023-06-05 12:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:51.018368 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11728 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      933 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-06-20 11:41:51.024226 apache-airflow-providers-dbt-cloud-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-06-20 11:41:49.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/LICENSE` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/MANIFEST.in` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.1/
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
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``dbt.cloud`` provider. All classes for this provider package
 are in ``airflow.providers.dbt.cloud`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-dbt-cloud``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -131,14 +131,32 @@
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
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/README.rst` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``dbt.cloud`` provider. All classes for this provider package
 are in ``airflow.providers.dbt.cloud`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-dbt-cloud``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -97,14 +97,32 @@
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
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/__init__.py`

 * *Files 0% similar despite different names*

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

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/get_provider_info.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/get_provider_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-dbt-cloud",
         "name": "dbt Cloud",
         "description": "`dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__\n",
         "suspended": False,
         "versions": [
+            "3.2.1",
             "3.2.0",
             "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.3.1",
             "2.3.0",
             "2.2.0",
@@ -58,18 +59,15 @@
         "sensors": [
             {"integration-name": "dbt Cloud", "python-modules": ["airflow.providers.dbt.cloud.sensors.dbt"]}
         ],
         "hooks": [
             {"integration-name": "dbt Cloud", "python-modules": ["airflow.providers.dbt.cloud.hooks.dbt"]}
         ],
         "triggers": [
-            {
-                "integration-name": "dbt Cloud",
-                "class-names": ["airflow.providers.dbt.cloud.triggers.dbt.DbtCloudRunJobTrigger"],
-            }
+            {"integration-name": "dbt Cloud", "python-modules": ["airflow.providers.dbt.cloud.triggers.dbt"]}
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.dbt.cloud.hooks.dbt.DbtCloudHook",
                 "connection-type": "dbt_cloud",
             }
         ],
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/hooks/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/hooks/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/dbt.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import json
 import time
 from enum import Enum
-from functools import wraps
+from functools import cached_property, wraps
 from inspect import signature
 from typing import TYPE_CHECKING, Any, Callable, Sequence, Set, TypeVar, cast
 
 import aiohttp
 from aiohttp import ClientResponseError
 from asgiref.sync import sync_to_async
 from requests.auth import AuthBase
 from requests.sessions import Session
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException
 from airflow.providers.http.hooks.http import HttpHook
 from airflow.typing_compat import TypedDict
 
 if TYPE_CHECKING:
     from requests.models import PreparedRequest, Response
 
@@ -188,29 +187,29 @@
         return conn.host or "cloud.getdbt.com"
 
     @staticmethod
     def get_request_url_params(
         tenant: str, endpoint: str, include_related: list[str] | None = None
     ) -> tuple[str, dict[str, Any]]:
         """
-        Form URL from base url and endpoint url
+        Form URL from base url and endpoint url.
 
         :param tenant: The tenant domain name which is need to be replaced in base url.
         :param endpoint: Endpoint url to be requested.
         :param include_related: Optional. List of related fields to pull with the run.
             Valid values are "trigger", "job", "repository", and "environment".
         """
         data: dict[str, Any] = {}
         if include_related:
             data = {"include_related": include_related}
         url = f"https://{tenant}/api/v2/accounts/{endpoint or ''}"
         return url, data
 
     async def get_headers_tenants_from_connection(self) -> tuple[dict[str, Any], str]:
-        """Get Headers, tenants from the connection details"""
+        """Get Headers, tenants from the connection details."""
         headers: dict[str, Any] = {}
         connection: Connection = await sync_to_async(self.get_connection)(self.dbt_cloud_conn_id)
         tenant = self._get_tenant_domain(connection)
         package_name, provider_version = _get_provider_info()
         headers["User-Agent"] = f"{package_name}-v{provider_version}"
         headers["Content-Type"] = "application/json"
         headers["Authorization"] = f"Token {connection.password}"
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/operators/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/operators/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/sensors/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/sensors/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/dbt.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class DbtCloudJobRunSensor(BaseSensorOperator):
-    """
-    Checks the status of a dbt Cloud job run.
+    """Checks the status of a dbt Cloud job run.
 
     .. seealso::
         For more information on how to use this sensor, take a look at the guide:
         :ref:`howto/operator:DbtCloudJobRunSensor`
 
     :param dbt_cloud_conn_id: The connection identifier for connecting to dbt Cloud.
     :param run_id: The job run identifier.
@@ -87,17 +86,19 @@
 
         if job_run_status == DbtCloudJobRunStatus.CANCELLED.value:
             raise DbtCloudJobRunException(f"Job run {self.run_id} has been cancelled.")
 
         return job_run_status == DbtCloudJobRunStatus.SUCCESS.value
 
     def execute(self, context: Context) -> None:
-        """
-        Defers to Trigger class to poll for state of the job run until
-        it reaches a failure state or success state
+        """Run the sensor.
+
+        Depending on whether ``deferrable`` is set, this would either defer to
+        the triggerer or poll for states of the job run, until the job reaches a
+        failure state or success state.
         """
         if not self.deferrable:
             super().execute(context)
         else:
             end_time = time.time() + self.timeout
             if not self.poke(context=context):
                 self.defer(
@@ -109,30 +110,30 @@
                         poll_interval=self.poke_interval,
                         end_time=end_time,
                     ),
                     method_name="execute_complete",
                 )
 
     def execute_complete(self, context: Context, event: dict[str, Any]) -> int:
-        """
-        Callback for when the trigger fires - returns immediately.
-        Relies on trigger to throw an exception, otherwise it assumes execution was
-        successful.
+        """Callback for when the trigger fires - returns immediately.
+
+        This relies on trigger to throw an exception, otherwise it assumes
+        execution was successful.
         """
         if event["status"] in ["error", "cancelled"]:
             raise AirflowException("Error in dbt: " + event["message"])
         self.log.info(event["message"])
         return int(event["run_id"])
 
 
 class DbtCloudJobRunAsyncSensor(DbtCloudJobRunSensor):
-    """
-    This class is deprecated.
-    Please use
-    :class:`airflow.providers.dbt.cloud.sensor.dbt.DbtCloudJobRunSensor`.
+    """This class is deprecated.
+
+    Please use :class:`airflow.providers.dbt.cloud.sensor.dbt.DbtCloudJobRunSensor`
+    with ``deferrable=True``.
     """
 
     def __init__(self, **kwargs: Any) -> None:
         warnings.warn(
             "Class `DbtCloudJobRunAsyncSensor` is deprecated and will be removed in a future release. "
             "Please use `DbtCloudJobRunSensor` and set `deferrable` attribute to `True` instead",
             AirflowProviderDeprecationWarning,
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/triggers/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/triggers/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/dbt.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 from typing import Any, AsyncIterator
 
 from airflow.providers.dbt.cloud.hooks.dbt import DbtCloudHook, DbtCloudJobRunStatus
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
 class DbtCloudRunJobTrigger(BaseTrigger):
-    """
-    DbtCloudRunJobTrigger is triggered with run id and account id, makes async Http call to dbt and
-    get the status for the submitted job with run id in polling interval of time.
+    """Trigger to make an HTTP call to dbt and get the status for the job.
+
+    This is done with run id in polling interval of time.
 
     :param conn_id: The connection identifier for connecting to Dbt.
     :param run_id: The ID of a dbt Cloud job.
     :param end_time: Time in seconds to wait for a job run to reach a terminal status. Defaults to 7 days.
     :param account_id: The ID of a dbt Cloud account.
     :param poll_interval:  polling period in seconds to check for the status.
     """
@@ -61,15 +61,15 @@
                 "conn_id": self.conn_id,
                 "end_time": self.end_time,
                 "poll_interval": self.poll_interval,
             },
         )
 
     async def run(self) -> AsyncIterator[TriggerEvent]:
-        """Make async connection to Dbt, polls for the pipeline run status"""
+        """Make async connection to Dbt, polls for the pipeline run status."""
         hook = DbtCloudHook(self.conn_id)
         try:
             while await self.is_still_running(hook):
                 if self.end_time < time.time():
                     yield TriggerEvent(
                         {
                             "status": "error",
@@ -104,16 +104,12 @@
                         "run_id": self.run_id,
                     }
                 )
         except Exception as e:
             yield TriggerEvent({"status": "error", "message": str(e), "run_id": self.run_id})
 
     async def is_still_running(self, hook: DbtCloudHook) -> bool:
-        """
-        Async function to check whether the job is submitted via async API is in
-        running state and returns True if it is still running else
-        return False
-        """
+        """Check whether the submitted job is running."""
         job_run_status = await hook.get_job_status(self.run_id, self.account_id)
         if not DbtCloudJobRunStatus.is_terminal(job_run_status):
             return True
         return False
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.1/
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
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``dbt.cloud`` provider. All classes for this provider package
 are in ``airflow.providers.dbt.cloud`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-dbt-cloud``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -131,14 +131,32 @@
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
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/pyproject.toml` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/setup.cfg` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.1/
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
 	aiohttp
 	apache-airflow-providers-http
@@ -55,10 +55,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.dbt.cloud.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.dbt.cloud
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc2/setup.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-dbt-cloud package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.0"
+version = "3.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-dbt-cloud setup."""
     setup(
         version=version,
         extras_require={"http": ["apache-airflow-providers-http"]},
```

