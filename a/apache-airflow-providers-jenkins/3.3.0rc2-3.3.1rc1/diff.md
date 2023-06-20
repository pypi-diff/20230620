# Comparing `tmp/apache-airflow-providers-jenkins-3.3.0rc2.tar.gz` & `tmp/apache-airflow-providers-jenkins-3.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-jenkins-3.3.0rc2.tar", last modified: Fri May 19 17:52:47 2023, max compression
+gzip compressed data, was "apache-airflow-providers-jenkins-3.3.1rc1.tar", last modified: Tue Jun 20 11:42:25 2023, max compression
```

## Comparing `apache-airflow-providers-jenkins-3.3.0rc2.tar` & `apache-airflow-providers-jenkins-3.3.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-jenkins-3.3.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:46.000000 apache-airflow-providers-jenkins-3.3.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-jenkins-3.3.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11325 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9795 2023-05-19 17:52:46.000000 apache-airflow-providers-jenkins-3.3.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-05-19 12:13:06.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-05-19 17:52:46.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-03-27 08:32:49.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/hooks/jenkins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10552 2023-02-24 18:43:53.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/operators/jenkins_job_trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2852 2023-02-24 18:43:53.000000 apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/sensors/jenkins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/apache_airflow_providers_jenkins.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11325 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/apache_airflow_providers_jenkins.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      834 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/apache_airflow_providers_jenkins.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/apache_airflow_providers_jenkins.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/apache_airflow_providers_jenkins.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/apache_airflow_providers_jenkins.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/apache_airflow_providers_jenkins.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/apache_airflow_providers_jenkins.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-jenkins-3.3.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1857 2023-05-19 17:52:47.000000 apache-airflow-providers-jenkins-3.3.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-05-19 17:52:46.000000 apache-airflow-providers-jenkins-3.3.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.776960 apache-airflow-providers-jenkins-3.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-jenkins-3.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:24.000000 apache-airflow-providers-jenkins-3.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-jenkins-3.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11712 2023-06-20 11:42:25.779160 apache-airflow-providers-jenkins-3.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10181 2023-06-20 11:42:24.000000 apache-airflow-providers-jenkins-3.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.687090 apache-airflow-providers-jenkins-3.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.688352 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.723106 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2023-06-20 11:42:24.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.729694 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-06-02 11:31:21.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/hooks/jenkins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.737257 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10539 2023-06-05 12:50:36.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/operators/jenkins_job_trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.745170 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2023-06-05 12:50:36.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/sensors/jenkins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.774296 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11712 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      834 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-jenkins-3.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-06-20 11:42:25.781616 apache-airflow-providers-jenkins-3.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:42:24.000000 apache-airflow-providers-jenkins-3.3.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/LICENSE` & `apache-airflow-providers-jenkins-3.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/MANIFEST.in` & `apache-airflow-providers-jenkins-3.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/PKG-INFO` & `apache-airflow-providers-jenkins-3.3.1rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jenkins
-Version: 3.3.0rc2
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-jenkins package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.1/
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
 
 
 Package ``apache-airflow-providers-jenkins``
 
-Release: ``3.3.0rc2``
+Release: ``3.3.1rc1``
 
 
 `Jenkins <https://jenkins.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``jenkins`` provider. All classes for this provider package
 are in ``airflow.providers.jenkins`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-jenkins``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -109,14 +109,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 3.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/README.rst` & `apache-airflow-providers-jenkins-3.3.1rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-jenkins``
 
-Release: ``3.3.0rc2``
+Release: ``3.3.1rc1``
 
 
 `Jenkins <https://jenkins.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``jenkins`` provider. All classes for this provider package
 are in ``airflow.providers.jenkins`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-jenkins``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -76,14 +76,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 3.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/__init__.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.3.0"
+__version__ = "3.3.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/get_provider_info.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-jenkins",
         "name": "Jenkins",
         "description": "`Jenkins <https://jenkins.io/>`__\n",
         "suspended": False,
         "versions": [
+            "3.3.1",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.1.0",
             "2.0.7",
```

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/hooks/__init__.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/hooks/jenkins.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/hooks/jenkins.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,38 +50,38 @@
 
         return inner
 
     return dec
 
 
 class JenkinsHook(BaseHook):
-    """Hook to manage connection to jenkins server"""
+    """Hook to manage connection to jenkins server."""
 
     conn_name_attr = "conn_id"
     default_conn_name = "jenkins_default"
     conn_type = "jenkins"
     hook_name = "Jenkins"
 
     @staticmethod
     def get_connection_form_widgets() -> dict[str, Any]:
-        """Returns connection widgets to add to connection form"""
+        """Returns connection widgets to add to connection form."""
         from flask_babel import lazy_gettext
         from wtforms import BooleanField
 
         return {
             "use_https": BooleanField(
                 label=lazy_gettext("Use Https"),
                 description="Specifies whether to use https scheme. Defaults to http",
             ),
         }
 
     @staticmethod
     @_ensure_prefixes(conn_type="jenkins")
     def get_ui_field_behaviour() -> dict[str, Any]:
-        """Returns custom field behaviour"""
+        """Returns custom field behaviour."""
         return {
             "hidden_fields": ["schema", "extra"],
             "relabeling": {},
             "placeholders": {
                 "login": "Login for the Jenkins service you would like to connect to",
                 "password": "Password for the Jenkins service you would like to connect too",
                 "host": "Host for your Jenkins server. Should NOT contain scheme (http:// or https://)",
@@ -98,15 +98,15 @@
         if connection.extra_dejson.get("use_https"):
             connection_prefix = "https"
         url = f"{connection_prefix}://{connection.host}:{connection.port}/{connection.schema}"
         self.log.info("Trying to connect to %s", url)
         self.jenkins_server = jenkins.Jenkins(url, connection.login, connection.password)
 
     def get_jenkins_server(self) -> jenkins.Jenkins:
-        """Get jenkins server"""
+        """Get jenkins server."""
         return self.jenkins_server
 
     def get_latest_build_number(self, job_name) -> int:
         self.log.info("Build number not specified, getting latest build info from Jenkins")
         job_info = self.jenkins_server.get_job_info(job_name)
         return job_info["lastBuild"]["number"]
```

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/operators/__init__.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/operators/jenkins_job_trigger.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/operators/jenkins_job_trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 from airflow.providers.jenkins.hooks.jenkins import JenkinsHook
 
 JenkinsRequest = Mapping[str, Any]
 ParamType = Union[str, dict, List, None]
 
 
 def jenkins_request_with_headers(jenkins_server: Jenkins, req: Request) -> JenkinsRequest | None:
-    """
-    We need to get the headers in addition to the body answer
-    to get the location from them
-    This function uses jenkins_request method from python-jenkins library
-    with just the return call changed
+    """Create a Jenkins request from a raw request.
+
+    We need to get the headers in addition to the body answer to get the
+    location from them. This function uses ``jenkins_request`` from
+    python-jenkins with just the return call changed.
 
     :param jenkins_server: The server to query
     :param req: The request to execute
     :return: Dict containing the response body (key body)
         and the headers coming along (headers)
     """
     try:
@@ -69,19 +69,19 @@
         raise jenkins.TimeoutException(f"Error in request: {e}")
     except URLError as e:
         raise JenkinsException(f"Error in request: {e.reason}")
     return None
 
 
 class JenkinsJobTriggerOperator(BaseOperator):
-    """
-    Trigger a Jenkins Job and monitor it's execution.
-    This operator depend on python-jenkins library,
-    version >= 0.4.15 to communicate with jenkins server.
-    You'll also need to configure a Jenkins connection in the connections screen.
+    """Trigger a Jenkins Job and monitor its execution.
+
+    This operator depend on the python-jenkins library version >= 0.4.15 to
+    communicate with the Jenkins server. You'll also need to configure a Jenkins
+    connection in the connections screen.
 
     :param jenkins_connection_id: The jenkins connection to use for this job
     :param job_name: The name of the job to trigger
     :param parameters: The parameters block provided to jenkins for use in
         the API call when triggering a build. (templated)
     :param sleep_time: How long will the operator sleep between each status
         request for the job (min 1, default 10)
@@ -110,19 +110,19 @@
         self.parameters = parameters
         self.sleep_time = max(sleep_time, 1)
         self.jenkins_connection_id = jenkins_connection_id
         self.max_try_before_job_appears = max_try_before_job_appears
         self.allowed_jenkins_states = list(allowed_jenkins_states) if allowed_jenkins_states else ["SUCCESS"]
 
     def build_job(self, jenkins_server: Jenkins, params: ParamType = None) -> JenkinsRequest | None:
-        """
-        This function makes an API call to Jenkins to trigger a build for 'job_name'
-        It returned a dict with 2 keys : body and headers.
-        headers contains also a dict-like object which can be queried to get
-        the location to poll in the queue.
+        """Trigger a build job.
+
+        This returns a dict with 2 keys ``body`` and ``headers``. ``headers``
+        contains also a dict-like object which can be queried to get the
+        location to poll in the queue.
 
         :param jenkins_server: The jenkins server where the job should be triggered
         :param params: The parameters block to provide to jenkins API call.
         :return: Dict containing the response body (key body)
             and the headers coming along (headers)
         """
         # Since params can be either JSON string, dictionary, or list,
@@ -130,23 +130,24 @@
         if params and isinstance(params, str):
             params = ast.literal_eval(params)
 
         request = Request(method="POST", url=jenkins_server.build_job_url(self.job_name, params, None))
         return jenkins_request_with_headers(jenkins_server, request)
 
     def poll_job_in_queue(self, location: str, jenkins_server: Jenkins) -> int:
-        """
-        This method poll the jenkins queue until the job is executed.
-        When we trigger a job through an API call,
-        the job is first put in the queue without having a build number assigned.
-        Thus we have to wait the job exit the queue to know its build number.
-        To do so, we have to add /api/json (or /api/xml) to the location
-        returned by the build_job call and poll this file.
-        When a 'executable' block appears in the json, it means the job execution started
-        and the field 'number' then contains the build number.
+        """Poll the jenkins queue until the job is executed.
+
+        When we trigger a job through an API call, the job is first put in the
+        queue without having a build number assigned. We have to wait until the
+        job exits the queue to know its build number.
+
+        To do so, we add ``/api/json`` (or ``/api/xml``) to the location
+        returned by the ``build_job`` call, and poll this file. When an
+        ``executable`` block appears in the response, the job execution would
+        have started, and the field ``number`` would contains the build number.
 
         :param location: Location to poll, returned in the header of the build_job call
         :param jenkins_server: The jenkins server to poll
         :return: The build_number corresponding to the triggered job
         """
         try_count = 0
         location += "/api/json"
@@ -180,15 +181,15 @@
             time.sleep(self.sleep_time)
 
         raise AirflowException(
             f"The job hasn't been executed after polling the queue {self.max_try_before_job_appears} times"
         )
 
     def get_hook(self) -> JenkinsHook:
-        """Instantiate jenkins hook"""
+        """Instantiate the Jenkins hook."""
         return JenkinsHook(self.jenkins_connection_id)
 
     def execute(self, context: Mapping[Any, Any]) -> str | None:
         self.log.info(
             "Triggering the job %s on the jenkins : %s with the parameters : %s",
             self.job_name,
             self.jenkins_connection_id,
```

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/sensors/__init__.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/airflow/providers/jenkins/sensors/jenkins.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/sensors/jenkins.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class JenkinsBuildSensor(BaseSensorOperator):
-    """
-    Monitor a jenkins job and pass when it is finished building. This is regardless of the build outcome.
-    This sensor depend on python-jenkins library,
+    """Monitor a Jenkins job and pass when it is finished building.
+
+    This is regardless of the build outcome.
 
     :param jenkins_connection_id: The jenkins connection to use for this job
     :param job_name: The name of the job to check
     :param build_number: Build number to check - if None, the latest build will be used
     """
 
     def __init__(
```

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/apache_airflow_providers_jenkins.egg-info/PKG-INFO` & `apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jenkins
-Version: 3.3.0rc2
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-jenkins package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.1/
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
 
 
 Package ``apache-airflow-providers-jenkins``
 
-Release: ``3.3.0rc2``
+Release: ``3.3.1rc1``
 
 
 `Jenkins <https://jenkins.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``jenkins`` provider. All classes for this provider package
 are in ``airflow.providers.jenkins`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-jenkins``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -109,14 +109,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 3.3.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/apache_airflow_providers_jenkins.egg-info/SOURCES.txt` & `apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/pyproject.toml` & `apache-airflow-providers-jenkins-3.3.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/setup.cfg` & `apache-airflow-providers-jenkins-3.3.1rc1/setup.cfg`

 * *Files 3% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.1/
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
 	python-jenkins>=1.0.0
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.jenkins.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.jenkins
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-jenkins-3.3.0rc2/setup.py` & `apache-airflow-providers-jenkins-3.3.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-jenkins package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.3.0"
+version = "3.3.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-jenkins setup."""
     setup(
         version=version,
         extras_require={},
```

