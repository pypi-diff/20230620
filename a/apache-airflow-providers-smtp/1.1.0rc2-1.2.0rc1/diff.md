# Comparing `tmp/apache-airflow-providers-smtp-1.1.0rc2.tar.gz` & `tmp/apache-airflow-providers-smtp-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-smtp-1.1.0rc2.tar", last modified: Fri May 19 17:53:33 2023, max compression
+gzip compressed data, was "apache-airflow-providers-smtp-1.2.0rc1.tar", last modified: Tue Jun 20 11:43:14 2023, max compression
```

## Comparing `apache-airflow-providers-smtp-1.1.0rc2.tar` & `apache-airflow-providers-smtp-1.2.0rc1.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.1.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:32.000000 apache-airflow-providers-smtp-1.1.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.1.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5663 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4142 2023-05-19 17:53:32.000000 apache-airflow-providers-smtp-1.1.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-05-19 12:21:49.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-05-19 17:53:32.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13824 2023-04-07 21:10:19.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/hooks/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-04-13 08:25:20.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/operators/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5663 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-smtp-1.1.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1816 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-05-19 17:53:32.000000 apache-airflow-providers-smtp-1.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:14.048896 apache-airflow-providers-smtp-1.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:12.000000 apache-airflow-providers-smtp-1.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6088 2023-06-20 11:43:14.049613 apache-airflow-providers-smtp-1.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4566 2023-06-20 11:43:12.000000 apache-airflow-providers-smtp-1.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:13.965372 apache-airflow-providers-smtp-1.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:13.966540 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:14.001773 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2391 2023-06-20 11:43:12.000000 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:14.007479 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13827 2023-06-02 11:31:21.000000 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/hooks/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:14.013293 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-08 05:42:54.000000 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-06-08 05:42:54.000000 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/notifications/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:14.018845 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-06-01 06:14:29.000000 apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/operators/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:14.045800 apache-airflow-providers-smtp-1.2.0rc1/apache_airflow_providers_smtp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6088 2023-06-20 11:43:13.000000 apache-airflow-providers-smtp-1.2.0rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-20 11:43:13.000000 apache-airflow-providers-smtp-1.2.0rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:13.000000 apache-airflow-providers-smtp-1.2.0rc1/apache_airflow_providers_smtp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:43:13.000000 apache-airflow-providers-smtp-1.2.0rc1/apache_airflow_providers_smtp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:13.000000 apache-airflow-providers-smtp-1.2.0rc1/apache_airflow_providers_smtp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:43:13.000000 apache-airflow-providers-smtp-1.2.0rc1/apache_airflow_providers_smtp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:13.000000 apache-airflow-providers-smtp-1.2.0rc1/apache_airflow_providers_smtp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-smtp-1.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-06-20 11:43:14.051705 apache-airflow-providers-smtp-1.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-20 11:43:12.000000 apache-airflow-providers-smtp-1.2.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/LICENSE` & `apache-airflow-providers-smtp-1.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/MANIFEST.in` & `apache-airflow-providers-smtp-1.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/PKG-INFO` & `apache-airflow-providers-smtp-1.2.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.1.0rc2
+Version: 1.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-smtp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.2.0/
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
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.1.0rc2``
+Release: ``1.2.0rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``smtp`` provider. All classes for this provider package
 are in ``airflow.providers.smtp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-smtp``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -108,14 +108,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+1.2.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* ``Add notifier for Smtp (#31359)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Fix ruff static check (#31762)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 1.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/README.rst` & `apache-airflow-providers-smtp-1.2.0rc1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.1.0rc2``
+Release: ``1.2.0rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``smtp`` provider. All classes for this provider package
 are in ``airflow.providers.smtp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-smtp``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -75,14 +75,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+1.2.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* ``Add notifier for Smtp (#31359)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Fix ruff static check (#31762)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 1.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/__init__.py` & `apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/get_provider_info.py` & `apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-smtp",
         "name": "Simple Mail Transfer Protocol (SMTP)",
         "description": "`Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__\n",
         "suspended": False,
-        "versions": ["1.1.0", "1.0.1", "1.0.0"],
+        "versions": ["1.2.0", "1.1.0", "1.0.1", "1.0.0"],
         "dependencies": ["apache-airflow>=2.4.0"],
         "integrations": [
             {
                 "integration-name": "Simple Mail Transfer Protocol (SMTP)",
                 "external-doc-url": "https://tools.ietf.org/html/rfc5321",
                 "logo": "/integration-logos/smtp/SMTP.png",
                 "tags": ["protocol"],
@@ -49,8 +49,9 @@
                 "integration-name": "Simple Mail Transfer Protocol (SMTP)",
                 "python-modules": ["airflow.providers.smtp.hooks.smtp"],
             }
         ],
         "connection-types": [
             {"hook-class-name": "airflow.providers.smtp.hooks.smtp.SmtpHook", "connection-type": "smtp"}
         ],
+        "notifications": ["airflow.providers.smtp.notifications.smtp.SmtpNotifier"],
     }
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/hooks/__init__.py` & `apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/hooks/smtp.py` & `apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/hooks/smtp.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             smtp_kwargs["port"] = self.port
         smtp_kwargs["timeout"] = self.timeout
 
         return SMTP(**smtp_kwargs)
 
     @classmethod
     def get_connection_form_widgets(cls) -> dict[str, Any]:
-        """Returns connection widgets to add to connection form"""
+        """Returns connection widgets to add to connection form."""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import BooleanField, IntegerField, StringField
         from wtforms.validators import NumberRange
 
         return {
             "from_email": StringField(lazy_gettext("From email"), widget=BS3TextFieldWidget()),
@@ -134,15 +134,15 @@
                 default=5,
             ),
             "disable_tls": BooleanField(lazy_gettext("Disable TLS"), default=False),
             "disable_ssl": BooleanField(lazy_gettext("Disable SSL"), default=False),
         }
 
     def test_connection(self) -> tuple[bool, str]:
-        """Test SMTP connectivity from UI"""
+        """Test SMTP connectivity from UI."""
         try:
             smtp_client = self.get_conn().smtp_client
             if smtp_client:
                 status = smtp_client.noop()[0]
                 if status == 250:
                     return True, "Connection successfully tested"
         except Exception as e:
@@ -352,12 +352,12 @@
 
     @property
     def use_ssl(self) -> bool:
         return not bool(self.conn.extra_dejson.get("disable_ssl", False))
 
     @staticmethod
     def get_ui_field_behaviour() -> dict[str, Any]:
-        """Returns custom field behaviour"""
+        """Returns custom field behaviour."""
         return {
             "hidden_fields": ["schema", "extra"],
             "relabeling": {},
         }
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/operators/__init__.py` & `apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/operators/smtp.py` & `apache-airflow-providers-smtp-1.2.0rc1/airflow/providers/smtp/operators/smtp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/PKG-INFO` & `apache-airflow-providers-smtp-1.2.0rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.1.0rc2
+Version: 1.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-smtp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.2.0/
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
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.1.0rc2``
+Release: ``1.2.0rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``smtp`` provider. All classes for this provider package
 are in ``airflow.providers.smtp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-smtp``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -108,14 +108,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+1.2.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Features
+~~~~~~~~
+
+* ``Add notifier for Smtp (#31359)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Fix ruff static check (#31762)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 1.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/SOURCES.txt` & `apache-airflow-providers-smtp-1.2.0rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 pyproject.toml
 setup.cfg
 setup.py
 airflow/providers/smtp/__init__.py
 airflow/providers/smtp/get_provider_info.py
 airflow/providers/smtp/hooks/__init__.py
 airflow/providers/smtp/hooks/smtp.py
+airflow/providers/smtp/notifications/__init__.py
+airflow/providers/smtp/notifications/smtp.py
 airflow/providers/smtp/operators/__init__.py
 airflow/providers/smtp/operators/smtp.py
 apache_airflow_providers_smtp.egg-info/PKG-INFO
 apache_airflow_providers_smtp.egg-info/SOURCES.txt
 apache_airflow_providers_smtp.egg-info/dependency_links.txt
 apache_airflow_providers_smtp.egg-info/entry_points.txt
 apache_airflow_providers_smtp.egg-info/not-zip-safe
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/pyproject.toml` & `apache-airflow-providers-smtp-1.2.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/setup.cfg` & `apache-airflow-providers-smtp-1.2.0rc1/setup.cfg`

 * *Files 21% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.2.0/
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
 
@@ -52,10 +52,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.smtp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.smtp
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc2/setup.py` & `apache-airflow-providers-smtp-1.2.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-smtp package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.1.0"
+version = "1.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-smtp setup."""
     setup(
         version=version,
         extras_require={},
```

