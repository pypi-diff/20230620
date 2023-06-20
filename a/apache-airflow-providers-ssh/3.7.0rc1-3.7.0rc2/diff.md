# Comparing `tmp/apache-airflow-providers-ssh-3.7.0rc1.tar.gz` & `tmp/apache-airflow-providers-ssh-3.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-ssh-3.7.0rc1.tar", last modified: Tue May 16 15:55:22 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-ssh-3.7.0rc2.tar", last modified: Fri May 19 17:53:39 2023, max compression
```

## Comparing `apache-airflow-providers-ssh-3.7.0rc1.tar` & `apache-airflow-providers-ssh-3.7.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-ssh-3.7.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:55:21.000000 apache-airflow-providers-ssh-3.7.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-ssh-3.7.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13431 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11913 2023-05-16 15:55:21.000000 apache-airflow-providers-ssh-3.7.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/
--rw-r--r--   0 root         (0) root         (0)     1372 2023-05-16 15:39:21.000000 apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2619 2023-05-16 15:55:21.000000 apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22534 2023-05-03 19:47:07.000000 apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/hooks/ssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7717 2023-05-03 19:47:07.000000 apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/operators/ssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/apache_airflow_providers_ssh.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13431 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/apache_airflow_providers_ssh.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      671 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/apache_airflow_providers_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/apache_airflow_providers_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/apache_airflow_providers_ssh.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/apache_airflow_providers_ssh.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/apache_airflow_providers_ssh.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/apache_airflow_providers_ssh.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-ssh-3.7.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1845 2023-05-16 15:55:22.000000 apache-airflow-providers-ssh-3.7.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1620 2023-05-16 15:55:21.000000 apache-airflow-providers-ssh-3.7.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-ssh-3.7.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:38.000000 apache-airflow-providers-ssh-3.7.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-ssh-3.7.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13648 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12130 2023-05-19 17:53:38.000000 apache-airflow-providers-ssh-3.7.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-05-19 12:22:17.000000 apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-05-19 17:53:38.000000 apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22534 2023-05-03 19:47:07.000000 apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/hooks/ssh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7717 2023-05-03 19:47:07.000000 apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/operators/ssh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/apache_airflow_providers_ssh.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13648 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/apache_airflow_providers_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      671 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/apache_airflow_providers_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/apache_airflow_providers_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/apache_airflow_providers_ssh.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/apache_airflow_providers_ssh.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/apache_airflow_providers_ssh.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/apache_airflow_providers_ssh.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-ssh-3.7.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-05-19 17:53:39.000000 apache-airflow-providers-ssh-3.7.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-19 17:53:38.000000 apache-airflow-providers-ssh-3.7.0rc2/setup.py
```

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/LICENSE` & `apache-airflow-providers-ssh-3.7.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/MANIFEST.in` & `apache-airflow-providers-ssh-3.7.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/PKG-INFO` & `apache-airflow-providers-ssh-3.7.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ssh
-Version: 3.7.0rc1
+Version: 3.7.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ssh package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ssh/3.7.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ssh``
 
-Release: ``3.7.0rc1``
+Release: ``3.7.0rc2``
 
 
 `Secure Shell (SSH) <https://tools.ietf.org/html/rfc4251>`__
 
 
 Provider package
 ----------------
@@ -127,14 +127,17 @@
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.6.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/README.rst` & `apache-airflow-providers-ssh-3.7.0rc2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ssh``
 
-Release: ``3.7.0rc1``
+Release: ``3.7.0rc2``
 
 
 `Secure Shell (SSH) <https://tools.ietf.org/html/rfc4251>`__
 
 
 Provider package
 ----------------
@@ -94,14 +94,17 @@
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.6.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/__init__.py` & `apache-airflow-providers-ssh-3.7.0rc2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,26 +11,39 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-#
+
 # NOTE! THIS FILE IS AUTOMATICALLY GENERATED AND WILL BE
-# OVERWRITTEN WHEN PREPARING DOCUMENTATION FOR THE PACKAGES.
+# OVERWRITTEN WHEN PREPARING PACKAGES.
 #
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
-# `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
-#
-from __future__ import annotations
-
-import packaging.version
+# `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
-import airflow
+"""Setup.py for the apache-airflow-providers-ssh package."""
 
-__all__ = ["version"]
+from setuptools import find_namespace_packages, setup
 
 version = "3.7.0"
 
-if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
-    raise RuntimeError(f"The package `apache-airflow-providers-ssh:{version}` requires Apache Airflow 2.4.0+")
+
+def do_setup():
+    """Perform the package apache-airflow-providers-ssh setup."""
+    setup(
+        version=version,
+        extras_require={},
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.ssh",
+                "airflow.providers.ssh.*",
+                "airflow.providers.ssh_vendor",
+                "airflow.providers.ssh_vendor.*",
+            ],
+        ),
+    )
+
+
+if __name__ == "__main__":
+    do_setup()
```

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/get_provider_info.py` & `apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/hooks/__init__.py` & `apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/hooks/ssh.py` & `apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/hooks/ssh.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/operators/__init__.py` & `apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/airflow/providers/ssh/operators/ssh.py` & `apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/operators/ssh.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/apache_airflow_providers_ssh.egg-info/PKG-INFO` & `apache-airflow-providers-ssh-3.7.0rc2/apache_airflow_providers_ssh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ssh
-Version: 3.7.0rc1
+Version: 3.7.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ssh package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ssh/3.7.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ssh``
 
-Release: ``3.7.0rc1``
+Release: ``3.7.0rc2``
 
 
 `Secure Shell (SSH) <https://tools.ietf.org/html/rfc4251>`__
 
 
 Provider package
 ----------------
@@ -127,14 +127,17 @@
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.6.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/apache_airflow_providers_ssh.egg-info/SOURCES.txt` & `apache-airflow-providers-ssh-3.7.0rc2/apache_airflow_providers_ssh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/pyproject.toml` & `apache-airflow-providers-ssh-3.7.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     # implicit single-line string concatenation
     "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
+    # "D400", WIP: see #31135
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
     "D403",
     "D412",
     "D419"
 ]
 extend-ignore = [
```

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/setup.cfg` & `apache-airflow-providers-ssh-3.7.0rc2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.ssh.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.ssh
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-ssh-3.7.0rc1/setup.py` & `apache-airflow-providers-ssh-3.7.0rc2/airflow/providers/ssh/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,39 +11,31 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-
+#
 # NOTE! THIS FILE IS AUTOMATICALLY GENERATED AND WILL BE
-# OVERWRITTEN WHEN PREPARING PACKAGES.
+# OVERWRITTEN WHEN PREPARING DOCUMENTATION FOR THE PACKAGES.
 #
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
-# `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
+# `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
+#
+from __future__ import annotations
 
-"""Setup.py for the apache-airflow-providers-ssh package."""
+import packaging.version
 
-from setuptools import find_namespace_packages, setup
+__all__ = ["__version__"]
 
-version = "3.7.0"
+__version__ = "3.7.0"
 
+try:
+    from airflow import __version__ as airflow_version
+except ImportError:
+    from airflow.version import version as airflow_version
 
-def do_setup():
-    """Perform the package apache-airflow-providers-ssh setup."""
-    setup(
-        version=version,
-        extras_require={},
-        packages=find_namespace_packages(
-            include=[
-                "airflow.providers.ssh",
-                "airflow.providers.ssh.*",
-                "airflow.providers.ssh_vendor",
-                "airflow.providers.ssh_vendor.*",
-            ],
-        ),
+if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+    raise RuntimeError(
+        f"The package `apache-airflow-providers-ssh:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
-
-
-if __name__ == "__main__":
-    do_setup()
```

