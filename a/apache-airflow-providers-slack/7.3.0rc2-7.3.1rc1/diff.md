# Comparing `tmp/apache-airflow-providers-slack-7.3.0rc2.tar.gz` & `tmp/apache-airflow-providers-slack-7.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-slack-7.3.0rc2.tar", last modified: Fri May 19 17:53:32 2023, max compression
+gzip compressed data, was "apache-airflow-providers-slack-7.3.1rc1.tar", last modified: Tue Jun 20 11:43:12 2023, max compression
```

## Comparing `apache-airflow-providers-slack-7.3.0rc2.tar` & `apache-airflow-providers-slack-7.3.1rc1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:32.000000 apache-airflow-providers-slack-7.3.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-slack-7.3.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:30.000000 apache-airflow-providers-slack-7.3.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-slack-7.3.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15516 2023-05-19 17:53:32.000000 apache-airflow-providers-slack-7.3.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13965 2023-05-19 17:53:30.000000 apache-airflow-providers-slack-7.3.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-05-19 12:21:41.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3592 2023-05-19 17:53:30.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14518 2023-05-03 19:47:07.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/hooks/slack.py
--rw-r--r--   0 root         (0) root         (0)    21257 2023-05-03 19:47:07.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/hooks/slack_webhook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/notifications/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3214 2023-05-12 14:26:38.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/notifications/slack.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-05-12 14:26:38.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/notifications/slack_notifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8439 2023-05-03 19:47:07.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/operators/slack.py
--rw-r--r--   0 root         (0) root         (0)     7416 2023-05-03 19:47:07.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/operators/slack_webhook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12879 2023-02-24 18:43:53.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/transfers/sql_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/utils/
--rw-r--r--   0 root         (0) root         (0)     5131 2023-04-30 16:55:11.000000 apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:32.000000 apache-airflow-providers-slack-7.3.0rc2/apache_airflow_providers_slack.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15516 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/apache_airflow_providers_slack.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1090 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/apache_airflow_providers_slack.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/apache_airflow_providers_slack.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/apache_airflow_providers_slack.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/apache_airflow_providers_slack.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      142 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/apache_airflow_providers_slack.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:31.000000 apache-airflow-providers-slack-7.3.0rc2/apache_airflow_providers_slack.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-slack-7.3.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1889 2023-05-19 17:53:32.000000 apache-airflow-providers-slack-7.3.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1685 2023-05-19 17:53:30.000000 apache-airflow-providers-slack-7.3.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.173391 apache-airflow-providers-slack-7.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:11.000000 apache-airflow-providers-slack-7.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-06-20 11:43:12.174477 apache-airflow-providers-slack-7.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14394 2023-06-20 11:43:11.000000 apache-airflow-providers-slack-7.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.072082 apache-airflow-providers-slack-7.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.073303 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.111497 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3613 2023-06-20 11:43:11.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.120174 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14482 2023-06-01 07:44:14.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/slack.py
+-rw-r--r--   0 root         (0) root         (0)    21221 2023-06-01 07:44:14.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/slack_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.128994 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/slack.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/slack_notifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.137516 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-06-05 12:50:36.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/slack.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/slack_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.143280 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12879 2023-06-01 06:14:29.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/transfers/sql_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.146227 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/utils/
+-rw-r--r--   0 root         (0) root         (0)     5132 2023-06-02 11:31:21.000000 apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:12.170761 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      142 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:12.000000 apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-slack-7.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-06-20 11:43:12.176409 apache-airflow-providers-slack-7.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-06-20 11:43:11.000000 apache-airflow-providers-slack-7.3.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/LICENSE` & `apache-airflow-providers-slack-7.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.0rc2/MANIFEST.in` & `apache-airflow-providers-slack-7.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.0rc2/PKG-INFO` & `apache-airflow-providers-slack-7.3.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-slack
-Version: 7.3.0rc2
+Version: 7.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-slack package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.1/
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
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``7.3.0rc2``
+Release: ``7.3.1rc1``
 
 
 `Slack <https://slack.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``slack`` provider. All classes for this provider package
 are in ``airflow.providers.slack`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-slack``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -130,14 +130,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+7.3.1
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
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 7.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/README.rst` & `apache-airflow-providers-slack-7.3.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``7.3.0rc2``
+Release: ``7.3.1rc1``
 
 
 `Slack <https://slack.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``slack`` provider. All classes for this provider package
 are in ``airflow.providers.slack`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-slack``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -96,14 +96,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+7.3.1
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
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 7.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/__init__.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "7.3.0"
+__version__ = "7.3.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/get_provider_info.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-slack",
         "name": "Slack",
         "description": "`Slack <https://slack.com/>`__\n",
         "suspended": False,
         "versions": [
+            "7.3.1",
             "7.3.0",
             "7.2.0",
             "7.1.1",
             "7.1.0",
             "7.0.0",
             "6.0.0",
             "5.1.0",
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/hooks/__init__.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/hooks/slack.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/slack.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import json
 import warnings
-from functools import wraps
+from functools import cached_property, wraps
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Sequence
 
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackApiError
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowNotFoundException, AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 from airflow.providers.slack.utils import ConnectionExtraConfig
 from airflow.utils.helpers import exactly_one
 from airflow.utils.log.secrets_masker import mask_secret
 
 if TYPE_CHECKING:
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/hooks/slack_webhook.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/hooks/slack_webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import json
 import warnings
-from functools import wraps
+from functools import cached_property, wraps
 from typing import TYPE_CHECKING, Any, Callable
 from urllib.parse import urlsplit
 
 from slack_sdk import WebhookClient
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 from airflow.models import Connection
 from airflow.providers.slack.utils import ConnectionExtraConfig
 from airflow.utils.log.secrets_masker import mask_secret
 
 if TYPE_CHECKING:
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/notifications/__init__.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/notifications/slack.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from __future__ import annotations
 
 import json
+from functools import cached_property
 from typing import Sequence
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowOptionalProviderFeatureException
 
 try:
     from airflow.notifications.basenotifier import BaseNotifier
 except ImportError:
     raise AirflowOptionalProviderFeatureException(
         "Failed to import BaseNotifier. This feature is only available in Airflow versions >= 2.6.0"
@@ -33,15 +33,15 @@
 from airflow.providers.slack.hooks.slack import SlackHook
 
 ICON_URL: str = "https://raw.githubusercontent.com/apache/airflow/2.5.0/airflow/www/static/pin_100.png"
 
 
 class SlackNotifier(BaseNotifier):
     """
-    Slack BaseNotifier
+    Slack BaseNotifier.
 
     :param slack_conn_id: Slack API token (https://api.slack.com/web).
     :param text: The content of the message
     :param channel: The channel to send the message to. Optional
     :param username: The username to send the message as. Optional
     :param icon_url: The icon to use for the message. Optional
     :param attachments: A list of attachments to send with the message. Optional
@@ -72,15 +72,15 @@
 
     @cached_property
     def hook(self) -> SlackHook:
         """Slack Hook."""
         return SlackHook(slack_conn_id=self.slack_conn_id)
 
     def notify(self, context):
-        """Send a message to a Slack Channel"""
+        """Send a message to a Slack Channel."""
         api_call_params = {
             "channel": self.channel,
             "username": self.username,
             "text": self.text,
             "icon_url": self.icon_url,
             "attachments": json.dumps(self.attachments),
             "blocks": json.dumps(self.blocks),
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/notifications/slack_notifier.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/notifications/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/operators/__init__.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/operators/slack.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/slack.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import json
 import warnings
+from functools import cached_property
 from typing import Any, Sequence
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.slack.hooks.slack import SlackHook
 from airflow.utils.log.secrets_masker import mask_secret
 
 
 class SlackAPIOperator(BaseOperator):
-    """
-    Base Slack Operator
-    The SlackAPIPostOperator is derived from this operator.
-    In the future additional Slack API Operators will be derived from this class as well.
-    Only one of `slack_conn_id` and `token` is required.
+    """Base Slack Operator class.
+
+    Only one of ``slack_conn_id`` or ``token`` is required.
 
     :param slack_conn_id: :ref:`Slack API Connection <howto/connection:slack>`
         which its password is Slack API token. Optional
     :param token: Slack API token (https://api.slack.com/web). Optional
     :param method: The Slack API Method to Call (https://api.slack.com/methods). Optional
     :param api_params: API Method call parameters (https://api.slack.com/methods). Optional
     :param client_args: Slack Hook parameters. Optional. Check airflow.providers.slack.hooks.SlackHook
@@ -63,72 +61,72 @@
 
     @cached_property
     def hook(self) -> SlackHook:
         """Slack Hook."""
         return SlackHook(token=self.token, slack_conn_id=self.slack_conn_id)
 
     def construct_api_call_params(self) -> Any:
-        """
-        Used by the execute function. Allows templating on the source fields
-        of the api_call_params dict before construction
+        """API call parameters used by the execute function.
 
-        Override in child classes.
-        Each SlackAPIOperator child class is responsible for
-        having a construct_api_call_params function
-        which sets self.api_call_params with a dict of
-        API call parameters (https://api.slack.com/methods)
+        Allows templating on the source fields of the ``api_call_params`` dict
+        before construction.
+
+        Child classes should override this. Each SlackAPIOperator child class is
+        responsible for having function set ``self.api_call_params`` with a dict
+        of API call parameters (https://api.slack.com/methods)
         """
         raise NotImplementedError(
             "SlackAPIOperator should not be used directly. Chose one of the subclasses instead"
         )
 
     def execute(self, **kwargs):
         if not self.api_params:
             self.construct_api_call_params()
         self.hook.call(self.method, json=self.api_params)
 
 
 class SlackAPIPostOperator(SlackAPIOperator):
-    """
-    Posts messages to a slack channel
-    Examples:
+    """Post messages to a Slack channel.
 
     .. code-block:: python
 
         slack = SlackAPIPostOperator(
             task_id="post_hello",
             dag=dag,
-            token="XXX",
+            token="...",
             text="hello there!",
             channel="#random",
         )
 
     :param channel: channel in which to post message on slack name (#general) or
         ID (C12318391). (templated)
     :param username: Username that airflow will be posting to Slack as. (templated)
     :param text: message to send to slack. (templated)
-    :param icon_url: url to icon used for this message
+    :param icon_url: URL to icon used for this message
     :param attachments: extra formatting details. (templated)
-        - see https://api.slack.com/docs/attachments.
+        See https://api.slack.com/docs/attachments
     :param blocks: extra block layouts. (templated)
-        - see https://api.slack.com/reference/block-kit/blocks.
+        See https://api.slack.com/reference/block-kit/blocks
     """
 
     template_fields: Sequence[str] = ("username", "text", "attachments", "blocks", "channel")
     ui_color = "#FFBA40"
 
     def __init__(
         self,
         channel: str = "#general",
         username: str = "Airflow",
-        text: str = "No message has been set.\n"
-        "Here is a cat video instead\n"
-        "https://www.youtube.com/watch?v=J---aiyznGQ",
-        icon_url: str = "https://raw.githubusercontent.com/apache/"
-        "airflow/main/airflow/www/static/pin_100.png",
+        text: str = (
+            "No message has been set.\n"
+            "Here is a cat video instead\n"
+            "https://www.youtube.com/watch?v=J---aiyznGQ"
+        ),
+        icon_url: str = (
+            "https://raw.githubusercontent.com/apache/airflow/main/airflow/www/static/pin_100.png"
+        ),
         attachments: list | None = None,
         blocks: list | None = None,
         **kwargs,
     ) -> None:
         self.method = "chat.postMessage"
         self.channel = channel
         self.username = username
@@ -146,17 +144,15 @@
             "icon_url": self.icon_url,
             "attachments": json.dumps(self.attachments),
             "blocks": json.dumps(self.blocks),
         }
 
 
 class SlackAPIFileOperator(SlackAPIOperator):
-    """
-    Send a file to a slack channels
-    Examples:
+    """Send a file to a Slack channel.
 
     .. code-block:: python
 
         # Send file with filename and filetype
         slack_operator_file = SlackAPIFileOperator(
             task_id="slack_file_upload_1",
             dag=dag,
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/operators/slack_webhook.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/operators/slack_webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import warnings
+from functools import cached_property
 from typing import TYPE_CHECKING, Sequence
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.slack.hooks.slack_webhook import SlackWebhookHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -154,15 +154,15 @@
             slack_webhook_conn_id=self.slack_webhook_conn_id,
             proxy=self.proxy,
             # Deprecated. SlackWebhookHook will notify user if user provide non-empty ``webhook_token``.
             webhook_token=self.webhook_token,
         )
 
     def execute(self, context: Context) -> None:
-        """Call the SlackWebhookHook to post the provided Slack message"""
+        """Call the SlackWebhookHook to post the provided Slack message."""
         self.hook.send(
             text=self.message,
             attachments=self.attachments,
             blocks=self.blocks,
             # Parameters below use for compatibility with previous version of Operator and warn user if it set
             # Legacy Integration Parameters
             channel=self.channel,
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/transfers/__init__.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/transfers/sql_to_slack.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/transfers/sql_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.0rc2/airflow/providers/slack/utils/__init__.py` & `apache-airflow-providers-slack-7.3.1rc1/airflow/providers/slack/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
 
 def parse_filename(
     filename: str, supported_file_formats: Sequence[str], fallback: str | None = None
 ) -> tuple[str, str | None]:
     """
     Parse filetype and compression from given filename.
+
     :param filename: filename to parse.
     :param supported_file_formats: list of supported file extensions.
     :param fallback: fallback to given file format.
     :returns: filetype and compression (if specified)
     """
     if not filename:
         raise ValueError("Expected 'filename' parameter is missing.")
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/apache_airflow_providers_slack.egg-info/PKG-INFO` & `apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-slack
-Version: 7.3.0rc2
+Version: 7.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-slack package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.1/
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
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``7.3.0rc2``
+Release: ``7.3.1rc1``
 
 
 `Slack <https://slack.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``slack`` provider. All classes for this provider package
 are in ``airflow.providers.slack`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-slack``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -130,14 +130,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+7.3.1
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
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 7.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/apache_airflow_providers_slack.egg-info/SOURCES.txt` & `apache-airflow-providers-slack-7.3.1rc1/apache_airflow_providers_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.3.0rc2/pyproject.toml` & `apache-airflow-providers-slack-7.3.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-slack-7.3.0rc2/setup.cfg` & `apache-airflow-providers-slack-7.3.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.1/
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
 	provider_info=airflow.providers.slack.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.slack
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-slack-7.3.0rc2/setup.py` & `apache-airflow-providers-slack-7.3.1rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-slack package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "7.3.0"
+version = "7.3.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-slack setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

