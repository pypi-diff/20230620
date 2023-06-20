# Comparing `tmp/apache-airflow-providers-apache-druid-3.4.0rc2.tar.gz` & `tmp/apache-airflow-providers-apache-druid-3.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-druid-3.4.0rc2.tar", last modified: Fri May 19 17:51:35 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-druid-3.4.1rc1.tar", last modified: Tue Jun 20 11:41:12 2023, max compression
```

## Comparing `apache-airflow-providers-apache-druid-3.4.0rc2.tar` & `apache-airflow-providers-apache-druid-3.4.1rc1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-druid-3.4.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:34.000000 apache-airflow-providers-apache-druid-3.4.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-druid-3.4.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13525 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11925 2023-05-19 17:51:34.000000 apache-airflow-providers-apache-druid-3.4.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-19 12:00:16.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3224 2023-05-19 17:51:34.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6899 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/hooks/druid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2525 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/operators/druid.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-03 19:47:07.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/operators/druid_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10085 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/transfers/hive_to_druid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/apache_airflow_providers_apache_druid.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13525 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/apache_airflow_providers_apache_druid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      959 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/apache_airflow_providers_apache_druid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/apache_airflow_providers_apache_druid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/apache_airflow_providers_apache_druid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/apache_airflow_providers_apache_druid.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/apache_airflow_providers_apache_druid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/apache_airflow_providers_apache_druid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-apache-druid-3.4.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1929 2023-05-19 17:51:35.000000 apache-airflow-providers-apache-druid-3.4.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1819 2023-05-19 17:51:34.000000 apache-airflow-providers-apache-druid-3.4.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:12.041424 apache-airflow-providers-apache-druid-3.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-druid-3.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-druid-3.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-druid-3.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13930 2023-06-20 11:41:12.042636 apache-airflow-providers-apache-druid-3.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12329 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-druid-3.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:11.950450 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:11.951673 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:11.954599 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:11.988713 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3245 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:11.994512 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6903 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/hooks/druid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:12.002986 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/druid.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/druid_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:12.008772 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10081 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/transfers/hive_to_druid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:12.038030 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13930 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      959 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      192 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-druid-3.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-06-20 11:41:12.045048 apache-airflow-providers-apache-druid-3.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-druid-3.4.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/LICENSE` & `apache-airflow-providers-apache-druid-3.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/MANIFEST.in` & `apache-airflow-providers-apache-druid-3.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/PKG-INFO` & `apache-airflow-providers-apache-druid-3.4.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-druid
-Version: 3.4.0rc2
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-druid package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.1/
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
 Provides-Extra: apache.hive
 Provides-Extra: common.sql
 License-File: LICENSE
 License-File: NOTICE
 
 
@@ -50,38 +50,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-druid``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `Apache Druid <https://druid.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.druid`` provider. All classes for this provider package
 are in ``airflow.providers.apache.druid`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-druid``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -132,14 +132,30 @@
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
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/README.rst` & `apache-airflow-providers-apache-druid-3.4.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-druid``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `Apache Druid <https://druid.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.druid`` provider. All classes for this provider package
 are in ``airflow.providers.apache.druid`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-druid``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -97,14 +97,30 @@
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
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/__init__.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/__init__.py`

 * *Files 1% similar despite different names*

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

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/get_provider_info.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-druid",
         "name": "Apache Druid",
         "description": "`Apache Druid <https://druid.apache.org/>`__.\n",
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

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/hooks/__init__.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/hooks/druid.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/hooks/druid.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
 
 class DruidHook(BaseHook):
     """
-    Connection to Druid overlord for ingestion
+    Connection to Druid overlord for ingestion.
 
     To connect to a Druid cluster that is secured with the druid-basic-security
     extension, add the username and password to the druid ingestion connection.
 
     :param druid_ingest_conn_id: The connection id to the Druid overlord machine
                                  which accepts index jobs
     :param timeout: The interval between polling
@@ -56,15 +56,15 @@
         self.max_ingestion_time = max_ingestion_time
         self.header = {"content-type": "application/json"}
 
         if self.timeout < 1:
             raise ValueError("Druid timeout should be equal or greater than 1")
 
     def get_conn_url(self) -> str:
-        """Get Druid connection url"""
+        """Get Druid connection url."""
         conn = self.get_connection(self.druid_ingest_conn_id)
         host = conn.host
         port = conn.port
         conn_type = conn.conn_type or "http"
         endpoint = conn.extra_dejson.get("endpoint", "")
         return f"{conn_type}://{host}:{port}/{endpoint}"
 
@@ -79,15 +79,15 @@
         password = conn.password
         if user is not None and password is not None:
             return requests.auth.HTTPBasicAuth(user, password)
         else:
             return None
 
     def submit_indexing_job(self, json_index_spec: dict[str, Any] | str) -> None:
-        """Submit Druid ingestion job"""
+        """Submit Druid ingestion job."""
         url = self.get_conn_url()
 
         self.log.info("Druid ingestion spec: %s", json_index_spec)
         req_index = requests.post(url, data=json_index_spec, headers=self.header, auth=self.get_auth())
 
         code = req_index.status_code
         if code != 200:
@@ -127,15 +127,15 @@
                 raise AirflowException(f"Could not get status of the job, got {status}")
 
         self.log.info("Successful index")
 
 
 class DruidDbApiHook(DbApiHook):
     """
-    Interact with Druid broker
+    Interact with Druid broker.
 
     This hook is purely for users to query druid broker.
     For ingestion, please use druidHook.
     """
 
     conn_name_attr = "druid_broker_conn_id"
     default_conn_name = "druid_broker_default"
```

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/operators/__init__.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/operators/druid.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/druid.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class DruidOperator(BaseOperator):
     """
-    Allows to submit a task directly to druid
+    Allows to submit a task directly to druid.
 
     :param json_index_file: The filepath to the druid index specification
     :param druid_ingest_conn_id: The connection id of the Druid overlord which
         accepts index jobs
     :param timeout: The interval (in seconds) between polling the Druid job for the status
         of the ingestion job. Must be greater than or equal to 1
     :param max_ingestion_time: The maximum ingestion time before assuming the job failed
```

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/operators/druid_check.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/druid_check.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/transfers/__init__.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/airflow/providers/apache/druid/transfers/hive_to_druid.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/transfers/hive_to_druid.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
     from airflow.utils.context import Context
 
 LOAD_CHECK_INTERVAL = 5
 DEFAULT_TARGET_PARTITION_SIZE = 5000000
 
 
 class HiveToDruidOperator(BaseOperator):
-    """
-    Moves data from Hive to Druid, [del]note that for now the data is loaded
-    into memory before being pushed to Druid, so this operator should
-    be used for smallish amount of data.[/del]
+    """Moves data from Hive to Druid.
+
+    [del]note that for now the data is loaded into memory before being pushed to
+    Druid, so this operator should be used for smallish amount of data.[/del]
 
     :param sql: SQL query to execute against the Druid database. (templated)
     :param druid_datasource: the datasource you want to ingest into in druid
     :param ts_dim: the timestamp dimension
     :param metric_spec: the metrics you want to define for your data
     :param hive_cli_conn_id: the hive connection id
     :param druid_ingest_conn_id: the druid ingest connection id
```

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/apache_airflow_providers_apache_druid.egg-info/PKG-INFO` & `apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-druid
-Version: 3.4.0rc2
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-druid package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.1/
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
 Provides-Extra: apache.hive
 Provides-Extra: common.sql
 License-File: LICENSE
 License-File: NOTICE
 
 
@@ -50,38 +50,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-druid``
 
-Release: ``3.4.0rc2``
+Release: ``3.4.1rc1``
 
 
 `Apache Druid <https://druid.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.druid`` provider. All classes for this provider package
 are in ``airflow.providers.apache.druid`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-druid``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -132,14 +132,30 @@
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
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+
 3.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/apache_airflow_providers_apache_druid.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/pyproject.toml` & `apache-airflow-providers-apache-druid-3.4.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/setup.cfg` & `apache-airflow-providers-apache-druid-3.4.1rc1/setup.cfg`

 * *Files 16% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.1/
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
 	provider_info=airflow.providers.apache.druid.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.druid
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-druid-3.4.0rc2/setup.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-druid package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.0"
+version = "3.4.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-druid setup."""
     setup(
         version=version,
         extras_require={
```

