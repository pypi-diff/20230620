# Comparing `tmp/apache-airflow-providers-grpc-3.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-grpc-3.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-grpc-3.2.0rc1.tar", last modified: Tue May 16 15:54:18 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-grpc-3.2.0rc2.tar", last modified: Fri May 19 17:52:36 2023, max compression
```

## Comparing `apache-airflow-providers-grpc-3.2.0rc1.tar` & `apache-airflow-providers-grpc-3.2.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-grpc-3.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:16.000000 apache-airflow-providers-grpc-3.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-grpc-3.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10113 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8592 2023-05-16 15:54:16.000000 apache-airflow-providers-grpc-3.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/
--rw-r--r--   0 root         (0) root         (0)     1387 2023-05-16 15:39:21.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-05-16 15:54:16.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6850 2023-02-24 18:43:53.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/hooks/grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3799 2023-02-24 18:43:53.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/operators/grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10113 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       96 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-grpc-3.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1889 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-05-16 15:54:16.000000 apache-airflow-providers-grpc-3.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-grpc-3.2.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:35.000000 apache-airflow-providers-grpc-3.2.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-grpc-3.2.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10330 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8809 2023-05-19 17:52:35.000000 apache-airflow-providers-grpc-3.2.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-05-19 12:12:13.000000 apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-05-19 17:52:35.000000 apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6850 2023-02-24 18:43:53.000000 apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/hooks/grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3799 2023-02-24 18:43:53.000000 apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/operators/grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/apache_airflow_providers_grpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10330 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/apache_airflow_providers_grpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/apache_airflow_providers_grpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/apache_airflow_providers_grpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/apache_airflow_providers_grpc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/apache_airflow_providers_grpc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/apache_airflow_providers_grpc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/apache_airflow_providers_grpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-grpc-3.2.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-05-19 17:52:36.000000 apache-airflow-providers-grpc-3.2.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-19 17:52:35.000000 apache-airflow-providers-grpc-3.2.0rc2/setup.py
```

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/LICENSE` & `apache-airflow-providers-grpc-3.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/MANIFEST.in` & `apache-airflow-providers-grpc-3.2.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/PKG-INFO` & `apache-airflow-providers-grpc-3.2.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-grpc
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-grpc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.2.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-grpc``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `gRPC <https://grpc.io/>`__
 
 
 Provider package
 ----------------
@@ -130,14 +130,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare docs for Jan 2023 wave of Providers (#28651)``
    * ``Updated docs for RC3 wave of providers (#27937)``
    * ``Prepare for follow-up relase for November providers (#27774)``
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

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/README.rst` & `apache-airflow-providers-grpc-3.2.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-grpc``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `gRPC <https://grpc.io/>`__
 
 
 Provider package
 ----------------
@@ -97,14 +97,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare docs for Jan 2023 wave of Providers (#28651)``
    * ``Updated docs for RC3 wave of providers (#27937)``
    * ``Prepare for follow-up relase for November providers (#27774)``
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

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/get_provider_info.py` & `apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/hooks/__init__.py` & `apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/hooks/grpc.py` & `apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/hooks/grpc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/operators/__init__.py` & `apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/operators/grpc.py` & `apache-airflow-providers-grpc-3.2.0rc2/airflow/providers/grpc/operators/grpc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/PKG-INFO` & `apache-airflow-providers-grpc-3.2.0rc2/apache_airflow_providers_grpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-grpc
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-grpc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.2.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-grpc``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `gRPC <https://grpc.io/>`__
 
 
 Provider package
 ----------------
@@ -130,14 +130,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare docs for Jan 2023 wave of Providers (#28651)``
    * ``Updated docs for RC3 wave of providers (#27937)``
    * ``Prepare for follow-up relase for November providers (#27774)``
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

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/SOURCES.txt` & `apache-airflow-providers-grpc-3.2.0rc2/apache_airflow_providers_grpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/pyproject.toml` & `apache-airflow-providers-grpc-3.2.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/setup.cfg` & `apache-airflow-providers-grpc-3.2.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -55,10 +55,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.grpc.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.grpc
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-grpc-3.2.0rc1/setup.py` & `apache-airflow-providers-grpc-3.2.0rc2/setup.py`

 * *Files identical despite different names*

