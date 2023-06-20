# Comparing `tmp/apache-airflow-providers-apache-hdfs-4.0.0rc2.tar.gz` & `tmp/apache-airflow-providers-apache-hdfs-4.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-hdfs-4.0.0rc2.tar", last modified: Fri May 19 17:51:39 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-hdfs-4.1.0rc1.tar", last modified: Tue Jun 20 11:41:15 2023, max compression
```

## Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2.tar` & `apache-airflow-providers-apache-hdfs-4.1.0rc1.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:38.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11610 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10068 2023-05-19 17:51:38.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-19 12:00:54.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-05-19 17:51:38.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/hooks/hdfs.py
--rw-r--r--   0 root         (0) root         (0)     6104 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/hooks/webhdfs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/sensors/hdfs.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/sensors/web_hdfs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/apache_airflow_providers_apache_hdfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11610 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/apache_airflow_providers_apache_hdfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      870 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/apache_airflow_providers_apache_hdfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/apache_airflow_providers_apache_hdfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/apache_airflow_providers_apache_hdfs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/apache_airflow_providers_apache_hdfs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/apache_airflow_providers_apache_hdfs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/apache_airflow_providers_apache_hdfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1896 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1668 2023-05-19 17:51:38.000000 apache-airflow-providers-apache-hdfs-4.0.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.593816 apache-airflow-providers-apache-hdfs-4.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:14.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13210 2023-06-20 11:41:15.594917 apache-airflow-providers-apache-hdfs-4.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11667 2023-06-20 11:41:14.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.498277 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.499678 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.501081 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.537689 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 07:01:17.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2023-06-20 11:41:14.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.547725 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     6439 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/webhdfs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.554462 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5604 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/log/hdfs_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.565499 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/web_hdfs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.591094 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13210 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      971 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-06-20 11:41:15.597161 apache-airflow-providers-apache-hdfs-4.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-06-20 11:41:14.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/LICENSE` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/MANIFEST.in` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/PKG-INFO` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hdfs
-Version: 4.0.0rc2
+Version: 4.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hdfs package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.1.0/
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
@@ -48,39 +48,39 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hdfs``
 
-Release: ``4.0.0rc2``
+Release: ``4.1.0rc1``
 
 
 `Hadoop Distributed File System (HDFS) <https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html>`__
 and `WebHDFS <https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/WebHDFS.html>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.hdfs`` provider. All classes for this provider package
 are in ``airflow.providers.apache.hdfs`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-hdfs``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -110,14 +110,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.0
+-----
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* Add ability to read/write task instance logs from HDFS (#31512)
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Updates release notes for snakebite-py3 incompatibility with protobuf (#31756)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 4.0.0
 -----
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
@@ -135,14 +152,33 @@
 this provider and they are not available any more. If you want to continue using them,
 you can use 3.* version of the provider, but the recommendation is to switch to the new
 ``WebHDFSHook`` and ``WebHDFSSensor`` that use the ``WebHDFS`` API.
 
 
 * ``Remove snakebite-py3 based HDFS hooks and sensors (#31262)``
 
+
+.. note::
+
+   Protobuf 3 required by the snakebite-py3 library has ended its life in June 2023 and Airflow and it's
+   providers stopped supporting it. If you would like to continue using HDFS hooks and sensors
+   based on snakebite-py3 library when you have protobuf library 4.+ you can install the 3.* version
+   of the provider but due to Protobuf incompatibility, you need to do one of the the two things:
+
+   * set ``PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=python`` variable in your environment.
+   * downgrade protobuf to latest 3.* version (3.20.3 at this time)
+
+   Setting ``PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=python`` will make many libraries using protobuf
+   much slower - including multiple Google client libraries and Kubernetes. Downgrading protobuf to
+   (already End-Of-Life) 3.* version will make some of the latest versions of the new providers
+   incompatible (for example google and grpc) and you will have to downgrade those providers as well.
+   Both should be treated as a temporary workaround only, and you should migrate to WebHDFS
+   as soon as possible.
+
+
 Misc
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
```

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/README.rst` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,39 +15,39 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hdfs``
 
-Release: ``4.0.0rc2``
+Release: ``4.1.0rc1``
 
 
 `Hadoop Distributed File System (HDFS) <https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html>`__
 and `WebHDFS <https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/WebHDFS.html>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.hdfs`` provider. All classes for this provider package
 are in ``airflow.providers.apache.hdfs`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-hdfs``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -77,14 +77,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.0
+-----
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* Add ability to read/write task instance logs from HDFS (#31512)
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Updates release notes for snakebite-py3 incompatibility with protobuf (#31756)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 4.0.0
 -----
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
@@ -102,14 +119,33 @@
 this provider and they are not available any more. If you want to continue using them,
 you can use 3.* version of the provider, but the recommendation is to switch to the new
 ``WebHDFSHook`` and ``WebHDFSSensor`` that use the ``WebHDFS`` API.
 
 
 * ``Remove snakebite-py3 based HDFS hooks and sensors (#31262)``
 
+
+.. note::
+
+   Protobuf 3 required by the snakebite-py3 library has ended its life in June 2023 and Airflow and it's
+   providers stopped supporting it. If you would like to continue using HDFS hooks and sensors
+   based on snakebite-py3 library when you have protobuf library 4.+ you can install the 3.* version
+   of the provider but due to Protobuf incompatibility, you need to do one of the the two things:
+
+   * set ``PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=python`` variable in your environment.
+   * downgrade protobuf to latest 3.* version (3.20.3 at this time)
+
+   Setting ``PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=python`` will make many libraries using protobuf
+   much slower - including multiple Google client libraries and Kubernetes. Downgrading protobuf to
+   (already End-Of-Life) 3.* version will make some of the latest versions of the new providers
+   incompatible (for example google and grpc) and you will have to downgrade those providers as well.
+   Both should be treated as a temporary workaround only, and you should migrate to WebHDFS
+   as soon as possible.
+
+
 Misc
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
```

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/__init__.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.0.0"
+__version__ = "4.1.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/get_provider_info.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-hdfs",
         "name": "Apache HDFS",
         "description": "`Hadoop Distributed File System (HDFS) <https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html>`__\nand `WebHDFS <https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/WebHDFS.html>`__.\n",
         "suspended": False,
         "versions": [
+            "4.1.0",
             "4.0.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.1",
             "3.0.0",
             "2.2.3",
```

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/hooks/__init__.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/hooks/hdfs.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/hdfs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/hooks/webhdfs.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/webhdfs.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Hook for Web HDFS"""
+"""Hook for Web HDFS."""
 from __future__ import annotations
 
 import logging
 import socket
 from typing import Any
 
 import requests
@@ -37,15 +37,15 @@
         from hdfs.ext.kerberos import KerberosClient
     except ImportError:
         log.error("Could not load the Kerberos extension for the WebHDFSHook.")
         raise
 
 
 class AirflowWebHDFSHookException(AirflowException):
-    """Exception specific for WebHDFS hook"""
+    """Exception specific for WebHDFS hook."""
 
 
 class WebHDFSHook(BaseHook):
     """
     Interact with HDFS. This class is a wrapper around the hdfscli library.
 
     :param webhdfs_conn_id: The connection id for the webhdfs client to connect to.
@@ -149,7 +149,19 @@
         """
         conn = self.get_conn()
 
         conn.upload(
             hdfs_path=destination, local_path=source, overwrite=overwrite, n_threads=parallelism, **kwargs
         )
         self.log.debug("Uploaded file %s to %s", source, destination)
+
+    def read_file(self, filename: str) -> bytes:
+        """Read a file from HDFS.
+
+        :param filename: The path of the file to read.
+        :return: File content as a raw string
+        """
+        conn = self.get_conn()
+
+        with conn.read(filename) as reader:
+            content = reader.read()
+        return content
```

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/sensors/__init__.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/sensors/hdfs.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/hdfs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/airflow/providers/apache/hdfs/sensors/web_hdfs.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/web_hdfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class WebHdfsSensor(BaseSensorOperator):
-    """Waits for a file or folder to land in HDFS"""
+    """Waits for a file or folder to land in HDFS."""
 
     template_fields: Sequence[str] = ("filepath",)
 
     def __init__(self, *, filepath: str, webhdfs_conn_id: str = "webhdfs_default", **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self.filepath = filepath
         self.webhdfs_conn_id = webhdfs_conn_id
```

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/apache_airflow_providers_apache_hdfs.egg-info/PKG-INFO` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hdfs
-Version: 4.0.0rc2
+Version: 4.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hdfs package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.1.0/
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
@@ -48,39 +48,39 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hdfs``
 
-Release: ``4.0.0rc2``
+Release: ``4.1.0rc1``
 
 
 `Hadoop Distributed File System (HDFS) <https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html>`__
 and `WebHDFS <https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/WebHDFS.html>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.hdfs`` provider. All classes for this provider package
 are in ``airflow.providers.apache.hdfs`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-hdfs``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -110,14 +110,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.0
+-----
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* Add ability to read/write task instance logs from HDFS (#31512)
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Updates release notes for snakebite-py3 incompatibility with protobuf (#31756)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 4.0.0
 -----
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
@@ -135,14 +152,33 @@
 this provider and they are not available any more. If you want to continue using them,
 you can use 3.* version of the provider, but the recommendation is to switch to the new
 ``WebHDFSHook`` and ``WebHDFSSensor`` that use the ``WebHDFS`` API.
 
 
 * ``Remove snakebite-py3 based HDFS hooks and sensors (#31262)``
 
+
+.. note::
+
+   Protobuf 3 required by the snakebite-py3 library has ended its life in June 2023 and Airflow and it's
+   providers stopped supporting it. If you would like to continue using HDFS hooks and sensors
+   based on snakebite-py3 library when you have protobuf library 4.+ you can install the 3.* version
+   of the provider but due to Protobuf incompatibility, you need to do one of the the two things:
+
+   * set ``PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=python`` variable in your environment.
+   * downgrade protobuf to latest 3.* version (3.20.3 at this time)
+
+   Setting ``PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=python`` will make many libraries using protobuf
+   much slower - including multiple Google client libraries and Kubernetes. Downgrading protobuf to
+   (already End-Of-Life) 3.* version will make some of the latest versions of the new providers
+   incompatible (for example google and grpc) and you will have to downgrade those providers as well.
+   Both should be treated as a temporary workaround only, and you should migrate to WebHDFS
+   as soon as possible.
+
+
 Misc
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
```

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/apache_airflow_providers_apache_hdfs.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 setup.cfg
 setup.py
 airflow/providers/apache/hdfs/__init__.py
 airflow/providers/apache/hdfs/get_provider_info.py
 airflow/providers/apache/hdfs/hooks/__init__.py
 airflow/providers/apache/hdfs/hooks/hdfs.py
 airflow/providers/apache/hdfs/hooks/webhdfs.py
+airflow/providers/apache/hdfs/log/__init__.py
+airflow/providers/apache/hdfs/log/hdfs_task_handler.py
 airflow/providers/apache/hdfs/sensors/__init__.py
 airflow/providers/apache/hdfs/sensors/hdfs.py
 airflow/providers/apache/hdfs/sensors/web_hdfs.py
 apache_airflow_providers_apache_hdfs.egg-info/PKG-INFO
 apache_airflow_providers_apache_hdfs.egg-info/SOURCES.txt
 apache_airflow_providers_apache_hdfs.egg-info/dependency_links.txt
 apache_airflow_providers_apache_hdfs.egg-info/entry_points.txt
```

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/pyproject.toml` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/setup.cfg` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.0.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.1.0/
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
 	hdfs[avro,dataframe,kerberos]>=2.0.4
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.hdfs.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.hdfs
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-hdfs-4.0.0rc2/setup.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-hdfs package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.0.0"
+version = "4.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-hdfs setup."""
     setup(
         version=version,
         extras_require={},
```

