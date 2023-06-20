# Comparing `tmp/apache-airflow-providers-salesforce-5.4.0rc2.tar.gz` & `tmp/apache-airflow-providers-salesforce-5.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-salesforce-5.4.0rc2.tar", last modified: Fri May 19 17:53:21 2023, max compression
+gzip compressed data, was "apache-airflow-providers-salesforce-5.4.1rc1.tar", last modified: Tue Jun 20 11:43:01 2023, max compression
```

## Comparing `apache-airflow-providers-salesforce-5.4.0rc2.tar` & `apache-airflow-providers-salesforce-5.4.1rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-salesforce-5.4.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:20.000000 apache-airflow-providers-salesforce-5.4.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-salesforce-5.4.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11814 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10275 2023-05-19 17:53:20.000000 apache-airflow-providers-salesforce-5.4.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-05-19 12:20:52.000000 apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3024 2023-05-19 17:53:20.000000 apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18074 2023-02-24 18:43:53.000000 apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/hooks/salesforce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4762 2023-02-24 18:43:53.000000 apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/operators/bulk.py
--rw-r--r--   0 root         (0) root         (0)     2553 2023-02-24 18:43:53.000000 apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/operators/salesforce_apex_rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/apache_airflow_providers_salesforce.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11814 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/apache_airflow_providers_salesforce.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      833 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/apache_airflow_providers_salesforce.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/apache_airflow_providers_salesforce.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/apache_airflow_providers_salesforce.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/apache_airflow_providers_salesforce.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/apache_airflow_providers_salesforce.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/apache_airflow_providers_salesforce.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-salesforce-5.4.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1894 2023-05-19 17:53:21.000000 apache-airflow-providers-salesforce-5.4.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1662 2023-05-19 17:53:20.000000 apache-airflow-providers-salesforce-5.4.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.535191 apache-airflow-providers-salesforce-5.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-salesforce-5.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:00.000000 apache-airflow-providers-salesforce-5.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-salesforce-5.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12194 2023-06-20 11:43:01.536272 apache-airflow-providers-salesforce-5.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10654 2023-06-20 11:43:00.000000 apache-airflow-providers-salesforce-5.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.462015 apache-airflow-providers-salesforce-5.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.463123 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.494400 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-20 11:01:09.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3045 2023-06-20 11:43:00.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.500139 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18065 2023-06-02 11:31:21.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/hooks/salesforce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.508943 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4762 2023-06-01 06:14:28.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/bulk.py
+-rw-r--r--   0 root         (0) root         (0)     2555 2023-06-02 11:31:21.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/salesforce_apex_rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.532527 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12194 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      833 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-salesforce-5.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-06-20 11:43:01.538296 apache-airflow-providers-salesforce-5.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-06-20 11:43:00.000000 apache-airflow-providers-salesforce-5.4.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/LICENSE` & `apache-airflow-providers-salesforce-5.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/MANIFEST.in` & `apache-airflow-providers-salesforce-5.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/PKG-INFO` & `apache-airflow-providers-salesforce-5.4.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-salesforce
-Version: 5.4.0rc2
+Version: 5.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-salesforce package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.1/
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
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.4.0rc2``
+Release: ``5.4.1rc1``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``salesforce`` provider. All classes for this provider package
 are in ``airflow.providers.salesforce`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-salesforce``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
@@ -110,14 +110,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.4.1
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
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 5.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/README.rst` & `apache-airflow-providers-salesforce-5.4.1rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.4.0rc2``
+Release: ``5.4.1rc1``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``salesforce`` provider. All classes for this provider package
 are in ``airflow.providers.salesforce`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-salesforce``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
@@ -77,14 +77,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.4.1
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
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 5.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/__init__.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "5.4.0"
+__version__ = "5.4.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/get_provider_info.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-salesforce",
         "name": "Salesforce",
         "description": "`Salesforce <https://www.salesforce.com/>`__\n",
         "suspended": False,
         "versions": [
+            "5.4.1",
             "5.4.0",
             "5.3.0",
             "5.2.0",
             "5.1.0",
             "5.0.0",
             "4.0.0",
             "3.4.4",
```

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/hooks/__init__.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/hooks/salesforce.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/hooks/salesforce.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 .. note:: this hook also relies on the simple_salesforce package:
       https://github.com/simple-salesforce/simple-salesforce
 """
 from __future__ import annotations
 
 import logging
 import time
+from functools import cached_property
 from typing import Any, Iterable
 
 import pandas as pd
 from requests import Session
 from simple_salesforce import Salesforce, api
 
-from airflow.compat.functools import cached_property
 from airflow.hooks.base import BaseHook
 
 log = logging.getLogger(__name__)
 
 
 class SalesforceHook(BaseHook):
     """
@@ -88,15 +88,15 @@
         if field_name in extras:
             return extras[field_name] or None
         prefixed_name = f"{backcompat_prefix}{field_name}"
         return extras.get(prefixed_name) or None
 
     @staticmethod
     def get_connection_form_widgets() -> dict[str, Any]:
-        """Returns connection widgets to add to connection form"""
+        """Returns connection widgets to add to connection form."""
         from flask_appbuilder.fieldwidgets import BS3PasswordFieldWidget, BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import PasswordField, StringField
 
         return {
             "security_token": PasswordField(lazy_gettext("Security Token"), widget=BS3PasswordFieldWidget()),
             "domain": StringField(lazy_gettext("Domain"), widget=BS3TextFieldWidget()),
@@ -111,25 +111,25 @@
             "proxies": StringField(lazy_gettext("Proxies"), widget=BS3TextFieldWidget()),
             "version": StringField(lazy_gettext("API Version"), widget=BS3TextFieldWidget()),
             "client_id": StringField(lazy_gettext("Client ID"), widget=BS3TextFieldWidget()),
         }
 
     @staticmethod
     def get_ui_field_behaviour() -> dict[str, Any]:
-        """Returns custom field behaviour"""
+        """Returns custom field behaviour."""
         return {
             "hidden_fields": ["schema", "port", "extra", "host"],
             "relabeling": {
                 "login": "Username",
             },
         }
 
     @cached_property
     def conn(self) -> api.Salesforce:
-        """Returns a Salesforce instance. (cached)"""
+        """Returns a Salesforce instance. (cached)."""
         connection = self.get_connection(self.conn_id)
         extras = connection.extra_dejson
         # all extras below (besides the version one) are explicitly defaulted to None
         # because simple-salesforce has a built-in authentication-choosing method that
         # relies on which arguments are None and without "or None" setting this connection
         # in the UI will result in the blank extras being empty strings instead of None,
         # which would break the connection if "get" was used on its own.
@@ -149,15 +149,15 @@
             consumer_key=self._get_field(extras, "consumer_key") or None,
             privatekey_file=self._get_field(extras, "private_key_file_path") or None,
             privatekey=self._get_field(extras, "private_key") or None,
         )
         return conn
 
     def get_conn(self) -> api.Salesforce:
-        """Returns a Salesforce instance. (cached)"""
+        """Returns a Salesforce instance. (cached)."""
         return self.conn
 
     def make_query(self, query: str, include_deleted: bool = False, query_params: dict | None = None) -> dict:
         """
         Make a query to Salesforce.
 
         :param query: The query to make to Salesforce.
@@ -221,15 +221,15 @@
         )
 
         return self.make_query(query)
 
     @classmethod
     def _to_timestamp(cls, column: pd.Series) -> pd.Series:
         """
-        Convert a column of a dataframe to UNIX timestamps if applicable
+        Convert a column of a dataframe to UNIX timestamps if applicable.
 
         :param column: A Series object representing a column of a dataframe.
         :return: a new series that maintains the same index as the original
         """
         # try and convert the column to datetimes
         # the column MUST have a four digit year somewhere in the string
         # there should be a better way to do this,
@@ -389,15 +389,15 @@
         if record_time_added:
             fetched_time = time.time()
             df["time_fetched_from_salesforce"] = fetched_time
 
         return df
 
     def test_connection(self):
-        """Test the Salesforce connectivity"""
+        """Test the Salesforce connectivity."""
         try:
             self.describe_object("Account")
             status = True
             message = "Connection successfully tested"
         except Exception as e:
             status = False
             message = str(e)
```

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/operators/__init__.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/operators/bulk.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/bulk.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/airflow/providers/salesforce/operators/salesforce_apex_rest.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/salesforce_apex_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SalesforceApexRestOperator(BaseOperator):
     """
-    Execute a APEX Rest API action
+    Execute a APEX Rest API action.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SalesforceApexRestOperator`
 
     :param endpoint: The REST endpoint for the request.
     :param method: HTTP method for the request (default GET)
@@ -53,14 +53,15 @@
         self.method = method
         self.payload = payload
         self.salesforce_conn_id = salesforce_conn_id
 
     def execute(self, context: Context) -> dict:
         """
         Makes an HTTP request to an APEX REST endpoint and pushes results to xcom.
+
         :param context: The task context during execution.
         :return: Apex response
         """
         result: dict = {}
         sf_hook = SalesforceHook(salesforce_conn_id=self.salesforce_conn_id)
         conn = sf_hook.get_conn()
         execution_result = conn.apexecute(action=self.endpoint, method=self.method, data=self.payload)
```

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/apache_airflow_providers_salesforce.egg-info/PKG-INFO` & `apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-salesforce
-Version: 5.4.0rc2
+Version: 5.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-salesforce package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.1/
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
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.4.0rc2``
+Release: ``5.4.1rc1``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``salesforce`` provider. All classes for this provider package
 are in ``airflow.providers.salesforce`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-salesforce``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
@@ -110,14 +110,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.4.1
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
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 5.4.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/apache_airflow_providers_salesforce.egg-info/SOURCES.txt` & `apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/pyproject.toml` & `apache-airflow-providers-salesforce-5.4.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/setup.cfg` & `apache-airflow-providers-salesforce-5.4.1rc1/setup.cfg`

 * *Files 5% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.1/
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
 	pandas>=0.17.1
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.salesforce.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.salesforce
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-salesforce-5.4.0rc2/setup.py` & `apache-airflow-providers-salesforce-5.4.1rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-salesforce package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.4.0"
+version = "5.4.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-salesforce setup."""
     setup(
         version=version,
         extras_require={},
```

