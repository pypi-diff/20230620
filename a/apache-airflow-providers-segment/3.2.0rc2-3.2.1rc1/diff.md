# Comparing `tmp/apache-airflow-providers-segment-3.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-segment-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-segment-3.2.0rc2.tar", last modified: Fri May 19 17:53:25 2023, max compression
+gzip compressed data, was "apache-airflow-providers-segment-3.2.1rc1.tar", last modified: Tue Jun 20 11:43:05 2023, max compression
```

## Comparing `apache-airflow-providers-segment-3.2.0rc2.tar` & `apache-airflow-providers-segment-3.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:25.000000 apache-airflow-providers-segment-3.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-segment-3.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:24.000000 apache-airflow-providers-segment-3.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-segment-3.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9646 2023-05-19 17:53:25.000000 apache-airflow-providers-segment-3.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8116 2023-05-19 17:53:24.000000 apache-airflow-providers-segment-3.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:24.000000 apache-airflow-providers-segment-3.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:24.000000 apache-airflow-providers-segment-3.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:25.000000 apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-05-19 12:21:07.000000 apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2392 2023-05-19 17:53:24.000000 apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:25.000000 apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3487 2023-02-24 18:43:53.000000 apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/hooks/segment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:25.000000 apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-02-24 18:43:53.000000 apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/operators/segment_track_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:25.000000 apache-airflow-providers-segment-3.2.0rc2/apache_airflow_providers_segment.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9646 2023-05-19 17:53:24.000000 apache-airflow-providers-segment-3.2.0rc2/apache_airflow_providers_segment.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-19 17:53:24.000000 apache-airflow-providers-segment-3.2.0rc2/apache_airflow_providers_segment.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:24.000000 apache-airflow-providers-segment-3.2.0rc2/apache_airflow_providers_segment.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-19 17:53:24.000000 apache-airflow-providers-segment-3.2.0rc2/apache_airflow_providers_segment.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:24.000000 apache-airflow-providers-segment-3.2.0rc2/apache_airflow_providers_segment.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-19 17:53:24.000000 apache-airflow-providers-segment-3.2.0rc2/apache_airflow_providers_segment.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:24.000000 apache-airflow-providers-segment-3.2.0rc2/apache_airflow_providers_segment.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-segment-3.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1859 2023-05-19 17:53:25.000000 apache-airflow-providers-segment-3.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-05-19 17:53:23.000000 apache-airflow-providers-segment-3.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:05.007316 apache-airflow-providers-segment-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-segment-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:03.000000 apache-airflow-providers-segment-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-segment-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9982 2023-06-20 11:43:05.008371 apache-airflow-providers-segment-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8451 2023-06-20 11:43:03.000000 apache-airflow-providers-segment-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:04.928049 apache-airflow-providers-segment-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:04.929448 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:04.964288 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-06-20 11:43:03.000000 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:04.971002 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-06-02 11:31:21.000000 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/hooks/segment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:04.977768 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2646 2023-06-02 11:31:21.000000 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/operators/segment_track_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:05.004501 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9982 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-segment-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-06-20 11:43:05.010340 apache-airflow-providers-segment-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:43:03.000000 apache-airflow-providers-segment-3.2.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-segment-3.2.0rc2/LICENSE` & `apache-airflow-providers-segment-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.0rc2/MANIFEST.in` & `apache-airflow-providers-segment-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.0rc2/PKG-INFO` & `apache-airflow-providers-segment-3.2.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-segment
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-segment package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.1/
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
 
 
 Package ``apache-airflow-providers-segment``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Segment <https://segment.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``segment`` provider. All classes for this provider package
 are in ``airflow.providers.segment`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-segment``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ====================  ==================
 PIP package           Version required
 ====================  ==================
@@ -109,14 +109,29 @@
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
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-segment-3.2.0rc2/README.rst` & `apache-airflow-providers-segment-3.2.1rc1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-segment``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Segment <https://segment.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``segment`` provider. All classes for this provider package
 are in ``airflow.providers.segment`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-segment``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ====================  ==================
 PIP package           Version required
 ====================  ==================
@@ -76,14 +76,29 @@
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
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/__init__.py` & `apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/__init__.py`

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

### Comparing `apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/get_provider_info.py` & `apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-segment",
         "name": "Segment",
         "description": "`Segment <https://segment.com/>`__\n",
         "suspended": False,
         "versions": [
+            "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.0.4",
             "2.0.3",
             "2.0.2",
             "2.0.1",
```

### Comparing `apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/hooks/__init__.py` & `apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/hooks/segment.py` & `apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/hooks/segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,10 +79,10 @@
         if self.segment_debug_mode:
             self.log.info("Setting Segment analytics connection to debug mode")
         analytics.on_error = self.on_error
         analytics.write_key = self.write_key
         return analytics
 
     def on_error(self, error: str, items: str) -> None:
-        """Handles error callbacks when using Segment with segment_debug_mode set to True"""
+        """Handles error callbacks when using Segment with segment_debug_mode set to True."""
         self.log.error("Encountered Segment error: %s with items: %s", error, items)
         raise AirflowException(f"Segment error: {error}")
```

### Comparing `apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/operators/__init__.py` & `apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.0rc2/airflow/providers/segment/operators/segment_track_event.py` & `apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/operators/segment_track_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SegmentTrackEventOperator(BaseOperator):
     """
-    Send Track Event to Segment for a specified user_id and event
+    Send Track Event to Segment for a specified user_id and event.
 
     :param user_id: The ID for this user in your database. (templated)
     :param event: The name of the event you're tracking. (templated)
     :param properties: A dictionary of properties for the event. (templated)
     :param segment_conn_id: The connection ID to use when connecting to Segment.
     :param segment_debug_mode: Determines whether Segment should run in debug mode.
         Defaults to False
```

### Comparing `apache-airflow-providers-segment-3.2.0rc2/apache_airflow_providers_segment.egg-info/PKG-INFO` & `apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-segment
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-segment package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.1/
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
 
 
 Package ``apache-airflow-providers-segment``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Segment <https://segment.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``segment`` provider. All classes for this provider package
 are in ``airflow.providers.segment`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-segment``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ====================  ==================
 PIP package           Version required
 ====================  ==================
@@ -109,14 +109,29 @@
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
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-segment-3.2.0rc2/apache_airflow_providers_segment.egg-info/SOURCES.txt` & `apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.0rc2/pyproject.toml` & `apache-airflow-providers-segment-3.2.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-segment-3.2.0rc2/setup.cfg` & `apache-airflow-providers-segment-3.2.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.1/
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
 	analytics-python>=1.2.9
 	apache-airflow>=2.4.0.dev0
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.segment.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.segment
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-segment-3.2.0rc2/setup.py` & `apache-airflow-providers-segment-3.2.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-segment package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.0"
+version = "3.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-segment setup."""
     setup(
         version=version,
         extras_require={},
```

