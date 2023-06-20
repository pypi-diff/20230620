# Comparing `tmp/apache-airflow-providers-apache-kafka-1.1.0rc2.tar.gz` & `tmp/apache-airflow-providers-apache-kafka-1.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-kafka-1.1.0rc2.tar", last modified: Fri May 19 17:51:44 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-kafka-1.1.1rc1.tar", last modified: Tue Jun 20 11:41:21 2023, max compression
```

## Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2.tar` & `apache-airflow-providers-apache-kafka-1.1.1rc1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:43.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5154 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3609 2023-05-19 17:51:43.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-19 12:01:36.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3047 2023-05-19 17:51:43.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2746 2023-04-24 21:04:25.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/base.py
--rw-r--r--   0 root         (0) root         (0)     2351 2023-04-24 21:04:25.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/client.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/consume.py
--rw-r--r--   0 root         (0) root         (0)     1549 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/produce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8020 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/consume.py
--rw-r--r--   0 root         (0) root         (0)     4950 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/produce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8272 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/sensors/kafka.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/triggers/await_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5154 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1196 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1897 2023-05-19 17:51:44.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-19 17:51:43.000000 apache-airflow-providers-apache-kafka-1.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.234331 apache-airflow-providers-apache-kafka-1.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:20.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5937 2023-06-20 11:41:21.234885 apache-airflow-providers-apache-kafka-1.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-20 11:41:20.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.137110 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.138409 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.139745 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.174605 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-06-20 11:41:20.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.188594 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/base.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/client.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/consume.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/produce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.197120 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8020 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/consume.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/produce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.202842 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8272 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/kafka.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.208920 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4914 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/await_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.232008 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5937 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-06-20 11:41:21.236883 apache-airflow-providers-apache-kafka-1.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:41:20.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/LICENSE` & `apache-airflow-providers-apache-kafka-1.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/MANIFEST.in` & `apache-airflow-providers-apache-kafka-1.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/PKG-INFO` & `apache-airflow-providers-apache-kafka-1.1.1rc1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kafka
-Version: 1.1.0rc2
+Version: 1.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-kafka package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.1/
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
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.1.0rc2``
+Release: ``1.1.1rc1``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.kafka`` provider. All classes for this provider package
 are in ``airflow.providers.apache.kafka`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-kafka``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
@@ -101,18 +101,39 @@
  .. Unless required by applicable law or agreed to in writing,
     software distributed under the License is distributed on an
     "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
+.. NOTE TO CONTRIBUTORS:
+   Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
+   and you want to add an explanation to the users on how they are supposed to deal with them.
+   The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+1.1.1
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
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Add note about dropping Python 3.7 for kafka and impala (#32017)``
+
 1.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/README.rst` & `apache-airflow-providers-apache-kafka-1.1.1rc1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.1.0rc2``
+Release: ``1.1.1rc1``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.kafka`` provider. All classes for this provider package
 are in ``airflow.providers.apache.kafka`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-kafka``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
@@ -68,18 +68,39 @@
  .. Unless required by applicable law or agreed to in writing,
     software distributed under the License is distributed on an
     "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
+.. NOTE TO CONTRIBUTORS:
+   Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
+   and you want to add an explanation to the users on how they are supposed to deal with them.
+   The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+1.1.1
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
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Add note about dropping Python 3.7 for kafka and impala (#32017)``
+
 1.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/get_provider_info.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-kafka",
         "name": "Apache Kafka",
         "suspended": False,
         "description": "`Apache Kafka  <https://kafka.apache.org/>`__\n",
-        "versions": ["1.1.0", "1.0.0"],
+        "versions": ["1.1.1", "1.1.0", "1.0.0"],
         "dependencies": ["apache-airflow>=2.4.0", "asgiref", "confluent-kafka>=1.8.2"],
         "integrations": [
             {
                 "integration-name": "Apache Kafka",
                 "external-doc-url": "https://kafka.apache.org/",
                 "logo": "/integration-logos/apache/kafka.svg",
                 "tags": ["apache"],
@@ -63,15 +63,15 @@
                 "integration-name": "Apache Kafka",
                 "python-modules": ["airflow.providers.apache.kafka.sensors.kafka"],
             }
         ],
         "triggers": [
             {
                 "integration-name": "Apache Kafka",
-                "class-names": ["airflow.providers.apache.kafka.triggers.await_message.AwaitMessageTrigger"],
+                "python-modules": ["airflow.providers.apache.kafka.triggers.await_message"],
             }
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.apache.kafka.hooks.base.KafkaBaseHook",
                 "connection-type": "kafka",
             }
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/base.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,66 +12,66 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+from functools import cached_property
 from typing import Any
 
 from confluent_kafka.admin import AdminClient
 
-from airflow.compat.functools import cached_property
 from airflow.hooks.base import BaseHook
 
 
 class KafkaBaseHook(BaseHook):
     """
-    A base hook for interacting with Apache Kafka
+    A base hook for interacting with Apache Kafka.
 
     :param kafka_config_id: The connection object to use, defaults to "kafka_default"
     """
 
     conn_name_attr = "kafka_config_id"
     default_conn_name = "kafka_default"
     conn_type = "kafka"
     hook_name = "Apache Kafka"
 
     def __init__(self, kafka_config_id=default_conn_name, *args, **kwargs):
-        """Initialize our Base"""
+        """Initialize our Base."""
         super().__init__()
         self.kafka_config_id = kafka_config_id
         self.get_conn
 
     @staticmethod
     def get_ui_field_behaviour() -> dict[str, Any]:
-        """Returns custom field behaviour"""
+        """Returns custom field behaviour."""
         return {
             "hidden_fields": ["schema", "login", "password", "port", "host"],
             "relabeling": {"extra": "Config Dict"},
             "placeholders": {
                 "extra": '{"bootstrap.servers": "localhost:9092"}',
             },
         }
 
     def _get_client(self, config):
         raise NotImplementedError
 
     @cached_property
     def get_conn(self) -> Any:
-        """Get the configuration object"""
+        """Get the configuration object."""
         config = self.get_connection(self.kafka_config_id).extra_dejson
 
         if not (config.get("bootstrap.servers", None)):
             raise ValueError("config['bootstrap.servers'] must be provided.")
 
         return self._get_client(config)
 
     def test_connection(self) -> tuple[bool, str]:
-        """Test Connectivity from the UI"""
+        """Test Connectivity from the UI."""
         try:
             config = self.get_connection(self.kafka_config_id).extra_dejson
             t = AdminClient(config, timeout=10).list_topics()
             if t:
                 return True, "Connection successful."
         except Exception as e:
             False, str(e)
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/client.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,30 +22,30 @@
 from confluent_kafka.admin import AdminClient, NewTopic
 
 from airflow.providers.apache.kafka.hooks.base import KafkaBaseHook
 
 
 class KafkaAdminClientHook(KafkaBaseHook):
     """
-    A hook for interacting with the Kafka Cluster
+    A hook for interacting with the Kafka Cluster.
 
     :param kafka_config_id: The connection object to use, defaults to "kafka_default"
     """
 
     def __init__(self, kafka_config_id=KafkaBaseHook.default_conn_name) -> None:
         super().__init__(kafka_config_id=kafka_config_id)
 
     def _get_client(self, config) -> AdminClient:
         return AdminClient(config)
 
     def create_topic(
         self,
         topics: Sequence[Sequence[Any]],
     ) -> None:
-        """Creates a topic
+        """Creates a topic.
 
         :param topics: a list of topics to create including the number of partitions for the topic
           and the replication factor. Format: [ ("topic_name", number of partitions, replication factor)]
         """
         admin_client = self.get_conn
 
         new_topics = [NewTopic(t[0], num_partitions=t[1], replication_factor=t[2]) for t in topics]
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/consume.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/consume.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from confluent_kafka import Consumer
 
 from airflow.providers.apache.kafka.hooks.base import KafkaBaseHook
 
 
 class KafkaConsumerHook(KafkaBaseHook):
     """
-    A hook for creating a Kafka Consumer
+    A hook for creating a Kafka Consumer.
 
     :param kafka_config_id: The connection object to use, defaults to "kafka_default"
     :param topics: A list of topics to subscribe to.
     """
 
     def __init__(self, topics: Sequence[str], kafka_config_id=KafkaBaseHook.default_conn_name) -> None:
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/hooks/produce.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/produce.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 from confluent_kafka import Producer
 
 from airflow.providers.apache.kafka.hooks.base import KafkaBaseHook
 
 
 class KafkaProducerHook(KafkaBaseHook):
     """
-    A hook for creating a Kafka Producer
+    A hook for creating a Kafka Producer.
 
     :param kafka_config_id: The connection object to use, defaults to "kafka_default"
     """
 
     def __init__(self, kafka_config_id=KafkaBaseHook.default_conn_name) -> None:
         super().__init__(kafka_config_id=kafka_config_id)
 
     def _get_client(self, config) -> Producer:
         return Producer(config)
 
     def get_producer(self) -> Producer:
-        """Returns a producer object for sending messages to Kafka"""
+        """Returns a producer object for sending messages to Kafka."""
         producer = self.get_conn
 
         self.log.info("Producer %s", producer)
         return producer
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/consume.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/consume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/operators/produce.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/produce.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     else:
         local_logger.info(
             f"Produced record to topic {msg.topic()} partition [{msg.partition()}] @ offset {msg.offset()}"
         )
 
 
 class ProduceToTopicOperator(BaseOperator):
-    """An operator that produces messages to a Kafka topic
+    """An operator that produces messages to a Kafka topic.
 
     Registers a producer to a kafka topic and publishes messages to the log.
 
     :param kafka_config_id: The connection object to use, defaults to "kafka_default"
     :param topic: The topic the producer should produce to, defaults to None
     :param producer_function: The function that generates key/value pairs as messages for production,
         defaults to None
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/sensors/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/sensors/kafka.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/kafka.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/triggers/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/airflow/providers/apache/kafka/triggers/await_message.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/await_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from airflow import AirflowException
 from airflow.providers.apache.kafka.hooks.consume import KafkaConsumerHook
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 from airflow.utils.module_loading import import_string
 
 
 class AwaitMessageTrigger(BaseTrigger):
-    """A trigger that waits for a message matching specific criteria to arrive in Kafka
+    """A trigger that waits for a message matching specific criteria to arrive in Kafka.
 
     The behavior of the consumer of this trigger is as follows:
     - poll the Kafka topics for a message, if no message returned, sleep
     - process the message with provided callable and commit the message offset:
 
         - if callable returns any data, raise a TriggerEvent with the return data
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO` & `apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kafka
-Version: 1.1.0rc2
+Version: 1.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-kafka package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.1/
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
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.1.0rc2``
+Release: ``1.1.1rc1``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.kafka`` provider. All classes for this provider package
 are in ``airflow.providers.apache.kafka`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-kafka``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
@@ -101,18 +101,39 @@
  .. Unless required by applicable law or agreed to in writing,
     software distributed under the License is distributed on an
     "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
+.. NOTE TO CONTRIBUTORS:
+   Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
+   and you want to add an explanation to the users on how they are supposed to deal with them.
+   The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+1.1.1
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
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Add note about dropping Python 3.7 for kafka and impala (#32017)``
+
 1.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/pyproject.toml` & `apache-airflow-providers-apache-kafka-1.1.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/setup.cfg` & `apache-airflow-providers-apache-kafka-1.1.1rc1/setup.cfg`

 * *Files 9% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.1/
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
 	asgiref
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.kafka.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.kafka
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.0rc2/setup.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-kafka package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.1.0"
+version = "1.1.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-kafka setup."""
     setup(
         version=version,
         extras_require={},
```

