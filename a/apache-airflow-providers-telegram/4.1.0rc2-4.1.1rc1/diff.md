# Comparing `tmp/apache-airflow-providers-telegram-4.1.0rc2.tar.gz` & `tmp/apache-airflow-providers-telegram-4.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-telegram-4.1.0rc2.tar", last modified: Fri May 19 17:53:44 2023, max compression
+gzip compressed data, was "apache-airflow-providers-telegram-4.1.1rc1.tar", last modified: Tue Jun 20 11:43:25 2023, max compression
```

## Comparing `apache-airflow-providers-telegram-4.1.0rc2.tar` & `apache-airflow-providers-telegram-4.1.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-telegram-4.1.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:43.000000 apache-airflow-providers-telegram-4.1.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-telegram-4.1.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10665 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9132 2023-05-19 17:53:43.000000 apache-airflow-providers-telegram-4.1.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-19 12:22:43.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-05-19 17:53:43.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-02-24 18:43:53.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/hooks/telegram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3011 2023-02-24 18:43:53.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/operators/telegram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10665 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-telegram-4.1.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1650 2023-05-19 17:53:43.000000 apache-airflow-providers-telegram-4.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:25.100860 apache-airflow-providers-telegram-4.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-telegram-4.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-telegram-4.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11001 2023-06-20 11:43:25.102572 apache-airflow-providers-telegram-4.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9467 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:24.991067 apache-airflow-providers-telegram-4.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:24.992534 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:25.044391 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:25.051577 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5241 2023-06-02 11:31:21.000000 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/hooks/telegram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:25.060847 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2023-06-02 11:31:21.000000 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/operators/telegram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:25.096735 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11001 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-telegram-4.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-06-20 11:43:25.105507 apache-airflow-providers-telegram-4.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/LICENSE` & `apache-airflow-providers-telegram-4.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/MANIFEST.in` & `apache-airflow-providers-telegram-4.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/PKG-INFO` & `apache-airflow-providers-telegram-4.1.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-telegram
-Version: 4.1.0rc2
+Version: 4.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-telegram package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.1/
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
 
 
 Package ``apache-airflow-providers-telegram``
 
-Release: ``4.1.0rc2``
+Release: ``4.1.1rc1``
 
 
 `Telegram <https://telegram.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``telegram`` provider. All classes for this provider package
 are in ``airflow.providers.telegram`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-telegram``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================  ==================
 PIP package              Version required
 =======================  ==================
@@ -109,14 +109,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.1
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
 4.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/README.rst` & `apache-airflow-providers-telegram-4.1.1rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-telegram``
 
-Release: ``4.1.0rc2``
+Release: ``4.1.1rc1``
 
 
 `Telegram <https://telegram.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``telegram`` provider. All classes for this provider package
 are in ``airflow.providers.telegram`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-telegram``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================  ==================
 PIP package              Version required
 =======================  ==================
@@ -76,14 +76,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.1
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
 4.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/__init__.py` & `apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.1.0"
+__version__ = "4.1.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/get_provider_info.py` & `apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-telegram",
         "name": "Telegram",
         "description": "`Telegram <https://telegram.org/>`__\n",
         "suspended": False,
         "versions": [
+            "4.1.1",
             "4.1.0",
             "4.0.0",
             "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.0.4",
             "2.0.3",
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/hooks/__init__.py` & `apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/hooks/telegram.py` & `apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/hooks/telegram.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Hook for Telegram"""
+"""Hook for Telegram."""
 from __future__ import annotations
 
 import asyncio
 
 import telegram
 import tenacity
 
@@ -67,23 +67,23 @@
         super().__init__()
         self.token = self.__get_token(token, telegram_conn_id)
         self.chat_id = self.__get_chat_id(chat_id, telegram_conn_id)
         self.connection = self.get_conn()
 
     def get_conn(self) -> telegram.Bot:
         """
-        Returns the telegram bot client
+        Returns the telegram bot client.
 
         :return: telegram bot client
         """
         return telegram.Bot(self.token)
 
     def __get_token(self, token: str | None, telegram_conn_id: str | None) -> str:
         """
-        Returns the telegram API token
+        Returns the telegram API token.
 
         :param token: telegram API token
         :param telegram_conn_id: telegram connection name
         :return: telegram API token
         """
         if token is not None:
             return token
@@ -96,15 +96,15 @@
 
             return conn.password
 
         raise AirflowException("Cannot get token: No valid Telegram connection supplied.")
 
     def __get_chat_id(self, chat_id: str | None, telegram_conn_id: str | None) -> str | None:
         """
-        Returns the telegram chat ID for a chat/channel/group
+        Returns the telegram chat ID for a chat/channel/group.
 
         :param chat_id: optional chat ID
         :param telegram_conn_id: telegram connection name
         :return: telegram chat ID
         """
         if chat_id is not None:
             return chat_id
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/operators/__init__.py` & `apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/operators/telegram.py` & `apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/operators/telegram.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Operator for Telegram"""
+"""Operator for Telegram."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Sequence
 
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.providers.telegram.hooks.telegram import TelegramHook
@@ -67,15 +67,15 @@
             raise AirflowException("No valid Telegram connection id supplied.")
 
         self.telegram_conn_id = telegram_conn_id
 
         super().__init__(**kwargs)
 
     def execute(self, context: Context) -> None:
-        """Calls the TelegramHook to post the provided Telegram message"""
+        """Calls the TelegramHook to post the provided Telegram message."""
         if self.text:
             self.telegram_kwargs["text"] = self.text
 
         telegram_hook = TelegramHook(
             telegram_conn_id=self.telegram_conn_id,
             token=self.token,
             chat_id=self.chat_id,
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/PKG-INFO` & `apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-telegram
-Version: 4.1.0rc2
+Version: 4.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-telegram package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.1/
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
 
 
 Package ``apache-airflow-providers-telegram``
 
-Release: ``4.1.0rc2``
+Release: ``4.1.1rc1``
 
 
 `Telegram <https://telegram.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``telegram`` provider. All classes for this provider package
 are in ``airflow.providers.telegram`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-telegram``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================  ==================
 PIP package              Version required
 =======================  ==================
@@ -109,14 +109,29 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.1
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
 4.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/SOURCES.txt` & `apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/pyproject.toml` & `apache-airflow-providers-telegram-4.1.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/setup.cfg` & `apache-airflow-providers-telegram-4.1.1rc1/setup.cfg`

 * *Files 4% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.1/
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
 	python-telegram-bot>=20.0.0
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.telegram.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.telegram
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc2/setup.py` & `apache-airflow-providers-telegram-4.1.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-telegram package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.1.0"
+version = "4.1.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-telegram setup."""
     setup(
         version=version,
         extras_require={},
```

