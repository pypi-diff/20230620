# Comparing `tmp/apache-airflow-providers-http-4.4.1.tar.gz` & `tmp/apache-airflow-providers-http-4.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-http-4.4.1.tar", last modified: Wed May 24 07:14:18 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-http-4.4.1rc1.tar", last modified: Wed May 24 07:20:34 2023, max compression
```

## Comparing `apache-airflow-providers-http-4.4.1.tar` & `apache-airflow-providers-http-4.4.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:18.000000 apache-airflow-providers-http-4.4.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-http-4.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:14:15.000000 apache-airflow-providers-http-4.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-http-4.4.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12421 2023-05-24 07:14:18.000000 apache-airflow-providers-http-4.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10852 2023-05-24 07:14:15.000000 apache-airflow-providers-http-4.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:17.000000 apache-airflow-providers-http-4.4.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:17.000000 apache-airflow-providers-http-4.4.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:17.000000 apache-airflow-providers-http-4.4.1/airflow/providers/http/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-05-24 07:09:22.000000 apache-airflow-providers-http-4.4.1/airflow/providers/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3067 2023-05-24 07:14:15.000000 apache-airflow-providers-http-4.4.1/airflow/providers/http/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:18.000000 apache-airflow-providers-http-4.4.1/airflow/providers/http/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1/airflow/providers/http/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16287 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1/airflow/providers/http/hooks/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:18.000000 apache-airflow-providers-http-4.4.1/airflow/providers/http/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1/airflow/providers/http/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5828 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1/airflow/providers/http/operators/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:18.000000 apache-airflow-providers-http-4.4.1/airflow/providers/http/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1/airflow/providers/http/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5885 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1/airflow/providers/http/sensors/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:18.000000 apache-airflow-providers-http-4.4.1/apache_airflow_providers_http.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12421 2023-05-24 07:14:17.000000 apache-airflow-providers-http-4.4.1/apache_airflow_providers_http.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      768 2023-05-24 07:14:17.000000 apache-airflow-providers-http-4.4.1/apache_airflow_providers_http.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:14:17.000000 apache-airflow-providers-http-4.4.1/apache_airflow_providers_http.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-24 07:14:17.000000 apache-airflow-providers-http-4.4.1/apache_airflow_providers_http.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:14:17.000000 apache-airflow-providers-http-4.4.1/apache_airflow_providers_http.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-24 07:14:17.000000 apache-airflow-providers-http-4.4.1/apache_airflow_providers_http.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:14:17.000000 apache-airflow-providers-http-4.4.1/apache_airflow_providers_http.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-http-4.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1903 2023-05-24 07:14:18.000000 apache-airflow-providers-http-4.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-05-24 07:14:15.000000 apache-airflow-providers-http-4.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-http-4.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:20:33.000000 apache-airflow-providers-http-4.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-http-4.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12427 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10855 2023-05-24 07:20:33.000000 apache-airflow-providers-http-4.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-05-24 07:09:22.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-05-24 07:20:33.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16287 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/hooks/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5828 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/operators/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5885 2023-05-23 11:35:14.000000 apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/sensors/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12427 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      768 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-http-4.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-05-24 07:20:34.000000 apache-airflow-providers-http-4.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-24 07:20:33.000000 apache-airflow-providers-http-4.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-http-4.4.1/LICENSE` & `apache-airflow-providers-http-4.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.1/MANIFEST.in` & `apache-airflow-providers-http-4.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.1/PKG-INFO` & `apache-airflow-providers-http-4.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-http
-Version: 4.4.1
+Version: 4.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-http package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.4.1``
+Release: ``4.4.1rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-http-4.4.1/README.rst` & `apache-airflow-providers-http-4.4.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.4.1``
+Release: ``4.4.1rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-http-4.4.1/airflow/providers/http/__init__.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.1/airflow/providers/http/get_provider_info.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.1/airflow/providers/http/hooks/__init__.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.1/airflow/providers/http/hooks/http.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/hooks/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.1/airflow/providers/http/operators/__init__.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.1/airflow/providers/http/operators/http.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/operators/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.1/airflow/providers/http/sensors/__init__.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.1/airflow/providers/http/sensors/http.py` & `apache-airflow-providers-http-4.4.1rc1/airflow/providers/http/sensors/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.1/apache_airflow_providers_http.egg-info/PKG-INFO` & `apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-http
-Version: 4.4.1
+Version: 4.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-http package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.4.1``
+Release: ``4.4.1rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-http-4.4.1/apache_airflow_providers_http.egg-info/SOURCES.txt` & `apache-airflow-providers-http-4.4.1rc1/apache_airflow_providers_http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.1/pyproject.toml` & `apache-airflow-providers-http-4.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.1/setup.cfg` & `apache-airflow-providers-http-4.4.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	aiohttp
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	asgiref
 	requests>=2.26.0
 	requests_toolbelt
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.http.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.http
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-http-4.4.1/setup.py` & `apache-airflow-providers-http-4.4.1rc1/setup.py`

 * *Files identical despite different names*

