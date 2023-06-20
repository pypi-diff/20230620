# Comparing `tmp/apache-airflow-providers-celery-3.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-celery-3.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-celery-3.2.0rc1.tar", last modified: Tue May 16 15:53:26 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-celery-3.2.0rc2.tar", last modified: Fri May 19 17:52:02 2023, max compression
```

## Comparing `apache-airflow-providers-celery-3.2.0rc1.tar` & `apache-airflow-providers-celery-3.2.0rc2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-celery-3.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:25.000000 apache-airflow-providers-celery-3.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-celery-3.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9156 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7629 2023-05-16 15:53:25.000000 apache-airflow-providers-celery-3.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/airflow/providers/celery/
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-16 15:39:21.000000 apache-airflow-providers-celery-3.2.0rc1/airflow/providers/celery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-05-16 15:53:25.000000 apache-airflow-providers-celery-3.2.0rc1/airflow/providers/celery/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/airflow/providers/celery/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-celery-3.2.0rc1/airflow/providers/celery/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-02-24 18:43:53.000000 apache-airflow-providers-celery-3.2.0rc1/airflow/providers/celery/sensors/celery_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/apache_airflow_providers_celery.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9156 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/apache_airflow_providers_celery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/apache_airflow_providers_celery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/apache_airflow_providers_celery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/apache_airflow_providers_celery.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/apache_airflow_providers_celery.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/apache_airflow_providers_celery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-celery-3.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1861 2023-05-16 15:53:26.000000 apache-airflow-providers-celery-3.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1638 2023-05-16 15:53:25.000000 apache-airflow-providers-celery-3.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-celery-3.2.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:01.000000 apache-airflow-providers-celery-3.2.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-celery-3.2.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9373 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7846 2023-05-19 17:52:01.000000 apache-airflow-providers-celery-3.2.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/airflow/providers/celery/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-05-19 12:03:57.000000 apache-airflow-providers-celery-3.2.0rc2/airflow/providers/celery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-05-19 17:52:01.000000 apache-airflow-providers-celery-3.2.0rc2/airflow/providers/celery/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/airflow/providers/celery/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-celery-3.2.0rc2/airflow/providers/celery/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-02-24 18:43:53.000000 apache-airflow-providers-celery-3.2.0rc2/airflow/providers/celery/sensors/celery_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/apache_airflow_providers_celery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9373 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/apache_airflow_providers_celery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/apache_airflow_providers_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/apache_airflow_providers_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/apache_airflow_providers_celery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/apache_airflow_providers_celery.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/apache_airflow_providers_celery.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/apache_airflow_providers_celery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-celery-3.2.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-05-19 17:52:02.000000 apache-airflow-providers-celery-3.2.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-05-19 17:52:01.000000 apache-airflow-providers-celery-3.2.0rc2/setup.py
```

### Comparing `apache-airflow-providers-celery-3.2.0rc1/LICENSE` & `apache-airflow-providers-celery-3.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.0rc1/MANIFEST.in` & `apache-airflow-providers-celery-3.2.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.0rc1/PKG-INFO` & `apache-airflow-providers-celery-3.2.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-celery
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-celery package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.2.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-celery``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `Celery <http://www.celeryproject.org/>`__
 
 
 Provider package
 ----------------
@@ -126,14 +126,17 @@
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.3+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-celery-3.2.0rc1/README.rst` & `apache-airflow-providers-celery-3.2.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-celery``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `Celery <http://www.celeryproject.org/>`__
 
 
 Provider package
 ----------------
@@ -93,14 +93,17 @@
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.3+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-celery-3.2.0rc1/airflow/providers/celery/__init__.py` & `apache-airflow-providers-celery-3.2.0rc2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,28 +11,39 @@
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
+"""Setup.py for the apache-airflow-providers-celery package."""
 
-__all__ = ["version"]
+from setuptools import find_namespace_packages, setup
 
 version = "3.2.0"
 
-if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
-    raise RuntimeError(
-        f"The package `apache-airflow-providers-celery:{version}` requires Apache Airflow 2.4.0+"
+
+def do_setup():
+    """Perform the package apache-airflow-providers-celery setup."""
+    setup(
+        version=version,
+        extras_require={},
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.celery",
+                "airflow.providers.celery.*",
+                "airflow.providers.celery_vendor",
+                "airflow.providers.celery_vendor.*",
+            ],
+        ),
     )
+
+
+if __name__ == "__main__":
+    do_setup()
```

### Comparing `apache-airflow-providers-celery-3.2.0rc1/airflow/providers/celery/get_provider_info.py` & `apache-airflow-providers-celery-3.2.0rc2/airflow/providers/celery/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.0rc1/airflow/providers/celery/sensors/__init__.py` & `apache-airflow-providers-celery-3.2.0rc2/airflow/providers/celery/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.0rc1/airflow/providers/celery/sensors/celery_queue.py` & `apache-airflow-providers-celery-3.2.0rc2/airflow/providers/celery/sensors/celery_queue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.0rc1/apache_airflow_providers_celery.egg-info/PKG-INFO` & `apache-airflow-providers-celery-3.2.0rc2/apache_airflow_providers_celery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-celery
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-celery package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.2.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-celery``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `Celery <http://www.celeryproject.org/>`__
 
 
 Provider package
 ----------------
@@ -126,14 +126,17 @@
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.3+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-celery-3.2.0rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt` & `apache-airflow-providers-celery-3.2.0rc2/apache_airflow_providers_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.0rc1/pyproject.toml` & `apache-airflow-providers-celery-3.2.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-celery-3.2.0rc1/setup.cfg` & `apache-airflow-providers-celery-3.2.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.celery.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.celery
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

