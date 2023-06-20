# Comparing `tmp/apache-airflow-providers-dingding-3.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-dingding-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-dingding-3.2.0rc2.tar", last modified: Fri May 19 17:52:15 2023, max compression
+gzip compressed data, was "apache-airflow-providers-dingding-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:52 2023, max compression
```

## Comparing `apache-airflow-providers-dingding-3.2.0rc2.tar` & `apache-airflow-providers-dingding-3.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-dingding-3.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:14.000000 apache-airflow-providers-dingding-3.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-dingding-3.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11511 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9957 2023-05-19 17:52:14.000000 apache-airflow-providers-dingding-3.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-19 12:05:20.000000 apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-05-19 17:52:14.000000 apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4985 2023-02-24 18:43:53.000000 apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/hooks/dingding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-02-24 18:43:53.000000 apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/operators/dingding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/apache_airflow_providers_dingding.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11511 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/apache_airflow_providers_dingding.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/apache_airflow_providers_dingding.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/apache_airflow_providers_dingding.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/apache_airflow_providers_dingding.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/apache_airflow_providers_dingding.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       95 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/apache_airflow_providers_dingding.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/apache_airflow_providers_dingding.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-dingding-3.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1871 2023-05-19 17:52:15.000000 apache-airflow-providers-dingding-3.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-19 17:52:14.000000 apache-airflow-providers-dingding-3.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.785783 apache-airflow-providers-dingding-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-dingding-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:51.000000 apache-airflow-providers-dingding-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-dingding-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11898 2023-06-20 11:41:52.786777 apache-airflow-providers-dingding-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10343 2023-06-20 11:41:51.000000 apache-airflow-providers-dingding-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.715311 apache-airflow-providers-dingding-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.716505 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.748701 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-06-20 11:41:51.000000 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.754309 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2023-06-05 12:50:36.000000 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/hooks/dingding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.760152 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-06-01 06:14:28.000000 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/operators/dingding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.783456 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11898 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-dingding-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-06-20 11:41:52.788740 apache-airflow-providers-dingding-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:41:51.000000 apache-airflow-providers-dingding-3.2.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/LICENSE` & `apache-airflow-providers-dingding-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/MANIFEST.in` & `apache-airflow-providers-dingding-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/PKG-INFO` & `apache-airflow-providers-dingding-3.2.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dingding
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dingding package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.1/
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
 
 
 Package ``apache-airflow-providers-dingding``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Dingding <https://oapi.dingtalk.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``dingding`` provider. All classes for this provider package
 are in ``airflow.providers.dingding`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-dingding``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -129,14 +129,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+
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
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/README.rst` & `apache-airflow-providers-dingding-3.2.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dingding``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Dingding <https://oapi.dingtalk.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``dingding`` provider. All classes for this provider package
 are in ``airflow.providers.dingding`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-dingding``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -95,14 +95,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+
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
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/__init__.py` & `apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/__init__.py`

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

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/get_provider_info.py` & `apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-dingding",
         "name": "Dingding",
         "description": "`Dingding <https://oapi.dingtalk.com/>`__\n",
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

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/hooks/__init__.py` & `apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/hooks/dingding.py` & `apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/hooks/dingding.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 from requests import Session
 
 from airflow.exceptions import AirflowException
 from airflow.providers.http.hooks.http import HttpHook
 
 
 class DingdingHook(HttpHook):
-    """
-    This hook allows you send Dingding message using Dingding custom bot.
-    Get Dingding token from conn_id.password. And prefer set domain to
-    conn_id.host, if not will use default ``https://oapi.dingtalk.com``.
+    """Send message using a custom Dingding bot.
+
+    Get Dingding token from the connection's ``password``. If ``host`` is not
+    set in the connection, the default ``https://oapi.dingtalk.com`` is used.
 
     For more detail message in
     `Dingding custom bot <https://open-doc.dingtalk.com/microapp/serverapi2/qf2nxq>`_
 
     :param dingding_conn_id: The name of the Dingding connection to use
     :param message_type: Message type you want to send to Dingding, support five type so far
         including text, link, markdown, actionCard, feedCard
@@ -71,45 +71,41 @@
         if not token:
             raise AirflowException(
                 "Dingding token is requests but get nothing, check you conn_id configuration."
             )
         return f"robot/send?access_token={token}"
 
     def _build_message(self) -> str:
-        """
-        Build different type of Dingding message
-        As most commonly used type, text message just need post message content
-        rather than a dict like ``{'content': 'message'}``
-        """
+        """Build different type of Dingding messages."""
         if self.message_type in ["text", "markdown"]:
             data = {
                 "msgtype": self.message_type,
                 self.message_type: {"content": self.message} if self.message_type == "text" else self.message,
                 "at": {"atMobiles": self.at_mobiles, "isAtAll": self.at_all},
             }
         else:
             data = {"msgtype": self.message_type, self.message_type: self.message}
         return json.dumps(data)
 
     def get_conn(self, headers: dict | None = None) -> Session:
-        """
-        Overwrite HttpHook get_conn because just need base_url and headers and
-        not don't need generic params
+        """Overwrite HttpHook get_conn.
+
+        We just need base_url and headers, and not don't need generic params.
 
         :param headers: additional headers to be passed through as a dictionary
         """
         conn = self.get_connection(self.http_conn_id)
         self.base_url = conn.host if conn.host else "https://oapi.dingtalk.com"
         session = requests.Session()
         if headers:
             session.headers.update(headers)
         return session
 
     def send(self) -> None:
-        """Send Dingding message"""
+        """Send Dingding message."""
         support_type = ["text", "link", "markdown", "actionCard", "feedCard"]
         if self.message_type not in support_type:
             raise ValueError(
                 f"DingdingWebhookHook only support {support_type} so far, but receive {self.message_type}"
             )
 
         data = self._build_message()
```

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/operators/__init__.py` & `apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/airflow/providers/dingding/operators/dingding.py` & `apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/operators/dingding.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/apache_airflow_providers_dingding.egg-info/PKG-INFO` & `apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dingding
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dingding package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.1/
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
 
 
 Package ``apache-airflow-providers-dingding``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Dingding <https://oapi.dingtalk.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``dingding`` provider. All classes for this provider package
 are in ``airflow.providers.dingding`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-dingding``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
@@ -129,14 +129,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+
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
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/apache_airflow_providers_dingding.egg-info/SOURCES.txt` & `apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/pyproject.toml` & `apache-airflow-providers-dingding-3.2.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/setup.cfg` & `apache-airflow-providers-dingding-3.2.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.1/
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
 	apache-airflow-providers-http
 	apache-airflow>=2.4.0.dev0
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.dingding.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.dingding
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-dingding-3.2.0rc2/setup.py` & `apache-airflow-providers-dingding-3.2.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-dingding package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.0"
+version = "3.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-dingding setup."""
     setup(
         version=version,
         extras_require={"http": ["apache-airflow-providers-http"]},
```

