# Comparing `tmp/apache-airflow-providers-github-2.3.0rc2.tar.gz` & `tmp/apache-airflow-providers-github-2.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-github-2.3.0rc2.tar", last modified: Fri May 19 17:52:27 2023, max compression
+gzip compressed data, was "apache-airflow-providers-github-2.3.1rc1.tar", last modified: Tue Jun 20 11:42:05 2023, max compression
```

## Comparing `apache-airflow-providers-github-2.3.0rc2.tar` & `apache-airflow-providers-github-2.3.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-github-2.3.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:26.000000 apache-airflow-providers-github-2.3.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-github-2.3.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7895 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6368 2023-05-19 17:52:26.000000 apache-airflow-providers-github-2.3.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-05-19 12:06:38.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2244 2023-05-19 17:52:26.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3349 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/hooks/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3025 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/operators/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5277 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/sensors/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/apache_airflow_providers_github.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7895 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/apache_airflow_providers_github.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/apache_airflow_providers_github.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/apache_airflow_providers_github.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/apache_airflow_providers_github.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/apache_airflow_providers_github.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/apache_airflow_providers_github.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/apache_airflow_providers_github.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-github-2.3.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1844 2023-05-19 17:52:27.000000 apache-airflow-providers-github-2.3.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1638 2023-05-19 17:52:26.000000 apache-airflow-providers-github-2.3.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.409521 apache-airflow-providers-github-2.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-github-2.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:04.000000 apache-airflow-providers-github-2.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-github-2.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8598 2023-06-20 11:42:05.410709 apache-airflow-providers-github-2.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7070 2023-06-20 11:42:04.000000 apache-airflow-providers-github-2.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.321707 apache-airflow-providers-github-2.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.322761 apache-airflow-providers-github-2.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.356383 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-06-20 11:42:04.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.362590 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2023-06-02 11:31:21.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/hooks/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.369395 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-06-05 12:50:36.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/operators/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.375929 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5278 2023-06-02 11:31:21.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/sensors/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.407186 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8598 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-github-2.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-06-20 11:42:05.412712 apache-airflow-providers-github-2.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-06-20 11:42:04.000000 apache-airflow-providers-github-2.3.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-github-2.3.0rc2/LICENSE` & `apache-airflow-providers-github-2.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.0rc2/MANIFEST.in` & `apache-airflow-providers-github-2.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.0rc2/PKG-INFO` & `apache-airflow-providers-github-2.3.1rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-github
-Version: 2.3.0rc2
+Version: 2.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-github package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.1/
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
 
 
 Package ``apache-airflow-providers-github``
 
-Release: ``2.3.0rc2``
+Release: ``2.3.1rc1``
 
 
 `GitHub <https://www.github.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``github`` provider. All classes for this provider package
 are in ``airflow.providers.github`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-github``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -102,17 +102,38 @@
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
+
 Changelog
 ---------
 
+2.3.1
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
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 2.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-github-2.3.0rc2/README.rst` & `apache-airflow-providers-github-2.3.1rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-github``
 
-Release: ``2.3.0rc2``
+Release: ``2.3.1rc1``
 
 
 `GitHub <https://www.github.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``github`` provider. All classes for this provider package
 are in ``airflow.providers.github`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-github``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -69,17 +69,38 @@
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
+
 Changelog
 ---------
 
+2.3.1
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
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 2.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/__init__.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "2.3.0"
+__version__ = "2.3.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/get_provider_info.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/get_provider_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,26 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-github",
         "name": "Github",
         "description": "`GitHub <https://www.github.com/>`__\n",
         "dependencies": ["apache-airflow>=2.4.0", "PyGithub!=1.58"],
         "suspended": False,
-        "versions": ["2.3.0", "2.2.1", "2.2.0", "2.1.0", "2.0.0", "1.0.3", "1.0.2", "1.0.1", "1.0.0"],
+        "versions": [
+            "2.3.1",
+            "2.3.0",
+            "2.2.1",
+            "2.2.0",
+            "2.1.0",
+            "2.0.0",
+            "1.0.3",
+            "1.0.2",
+            "1.0.1",
+            "1.0.0",
+        ],
         "integrations": [
             {
                 "integration-name": "Github",
                 "external-doc-url": "https://www.github.com/",
                 "tags": ["software"],
             }
         ],
```

### Comparing `apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/hooks/__init__.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/hooks/github.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/hooks/github.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         else:
             self.client = GithubClient(login_or_token=access_token, base_url=host)
 
         return self.client
 
     @staticmethod
     def get_ui_field_behaviour() -> dict:
-        """Returns custom field behaviour"""
+        """Returns custom field behaviour."""
         return {
             "hidden_fields": ["schema", "port", "login", "extra"],
             "relabeling": {"host": "GitHub Enterprise URL (Optional)", "password": "GitHub Access Token"},
             "placeholders": {"host": "https://{hostname}/api/v3 (for GitHub Enterprise)"},
         }
 
     def test_connection(self) -> tuple[bool, str]:
```

### Comparing `apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/operators/__init__.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/operators/github.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/operators/github.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 from airflow.providers.github.hooks.github import GithubHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class GithubOperator(BaseOperator):
-    """
-    GithubOperator to interact and perform action on GitHub API.
-    This operator is designed to use GitHub Python SDK: https://github.com/PyGithub/PyGithub
+    """Interact and perform actions on GitHub API.
+
+    This operator is designed to use GitHub's Python SDK: https://github.com/PyGithub/PyGithub
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:GithubOperator`
 
     :param github_conn_id: Reference to a pre-defined GitHub Connection
     :param github_method: Method name from GitHub Python SDK to be called
```

### Comparing `apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/sensors/__init__.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.0rc2/airflow/providers/github/sensors/github.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/sensors/github.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         )
 
     def poke(self, context: Context) -> bool:
         self.log.info("Poking for tag: %s in repository: %s", self.tag_name, self.repository_name)
         return GithubSensor.poke(self, context=context)
 
     def tag_checker(self, repo: Any) -> bool | None:
-        """Checking existence of Tag in a Repository"""
+        """Checking existence of Tag in a Repository."""
         result = None
         try:
             if repo is not None and self.tag_name is not None:
                 all_tags = [x.name for x in repo.get_tags()]
                 result = self.tag_name in all_tags
 
         except GithubException as github_error:  # type: ignore[misc]
```

### Comparing `apache-airflow-providers-github-2.3.0rc2/apache_airflow_providers_github.egg-info/PKG-INFO` & `apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-github
-Version: 2.3.0rc2
+Version: 2.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-github package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.1/
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
 
 
 Package ``apache-airflow-providers-github``
 
-Release: ``2.3.0rc2``
+Release: ``2.3.1rc1``
 
 
 `GitHub <https://www.github.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``github`` provider. All classes for this provider package
 are in ``airflow.providers.github`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-github``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -102,17 +102,38 @@
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
+
 Changelog
 ---------
 
+2.3.1
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
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 2.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-github-2.3.0rc2/apache_airflow_providers_github.egg-info/SOURCES.txt` & `apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.0rc2/pyproject.toml` & `apache-airflow-providers-github-2.3.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-github-2.3.0rc2/setup.cfg` & `apache-airflow-providers-github-2.3.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.1/
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
 	PyGithub!=1.58
 	apache-airflow>=2.4.0.dev0
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.github.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.github
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-github-2.3.0rc2/setup.py` & `apache-airflow-providers-github-2.3.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-github package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "2.3.0"
+version = "2.3.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-github setup."""
     setup(
         version=version,
         extras_require={},
```

