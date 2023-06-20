# Comparing `tmp/apache-airflow-providers-common-sql-1.5.1.tar.gz` & `tmp/apache-airflow-providers-common-sql-1.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-common-sql-1.5.1.tar", last modified: Wed May 24 07:14:14 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-common-sql-1.5.1rc1.tar", last modified: Wed May 24 07:20:32 2023, max compression
```

## Comparing `apache-airflow-providers-common-sql-1.5.1.tar` & `apache-airflow-providers-common-sql-1.5.1rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:14.000000 apache-airflow-providers-common-sql-1.5.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-common-sql-1.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:14:11.000000 apache-airflow-providers-common-sql-1.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-common-sql-1.5.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10581 2023-05-24 07:14:14.000000 apache-airflow-providers-common-sql-1.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8971 2023-05-24 07:14:11.000000 apache-airflow-providers-common-sql-1.5.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-05-24 07:09:22.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2557 2023-05-24 07:14:11.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21739 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/hooks/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44516 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/operators/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4691 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/sensors/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:14:14.000000 apache-airflow-providers-common-sql-1.5.1/apache_airflow_providers_common_sql.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10581 2023-05-24 07:14:13.000000 apache-airflow-providers-common-sql-1.5.1/apache_airflow_providers_common_sql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-24 07:14:13.000000 apache-airflow-providers-common-sql-1.5.1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:14:13.000000 apache-airflow-providers-common-sql-1.5.1/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-24 07:14:13.000000 apache-airflow-providers-common-sql-1.5.1/apache_airflow_providers_common_sql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:14:13.000000 apache-airflow-providers-common-sql-1.5.1/apache_airflow_providers_common_sql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-24 07:14:13.000000 apache-airflow-providers-common-sql-1.5.1/apache_airflow_providers_common_sql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:14:13.000000 apache-airflow-providers-common-sql-1.5.1/apache_airflow_providers_common_sql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-common-sql-1.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1901 2023-05-24 07:14:14.000000 apache-airflow-providers-common-sql-1.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1690 2023-05-24 07:14:11.000000 apache-airflow-providers-common-sql-1.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-common-sql-1.5.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:20:31.000000 apache-airflow-providers-common-sql-1.5.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-common-sql-1.5.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10587 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8974 2023-05-24 07:20:31.000000 apache-airflow-providers-common-sql-1.5.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-05-24 07:09:22.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2557 2023-05-24 07:20:31.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21739 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/hooks/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44516 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/operators/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-05-23 11:35:14.000000 apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/sensors/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10587 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-common-sql-1.5.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-05-24 07:20:32.000000 apache-airflow-providers-common-sql-1.5.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-05-24 07:20:31.000000 apache-airflow-providers-common-sql-1.5.1rc1/setup.py
```

### Comparing `apache-airflow-providers-common-sql-1.5.1/LICENSE` & `apache-airflow-providers-common-sql-1.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.1/MANIFEST.in` & `apache-airflow-providers-common-sql-1.5.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.1/PKG-INFO` & `apache-airflow-providers-common-sql-1.5.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.5.1
+Version: 1.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.1/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.5.1``
+Release: ``1.5.1rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-common-sql-1.5.1/README.rst` & `apache-airflow-providers-common-sql-1.5.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.5.1``
+Release: ``1.5.1rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/__init__.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/get_provider_info.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/hooks/__init__.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/hooks/sql.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/hooks/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/operators/__init__.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/operators/sql.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/operators/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/sensors/__init__.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.1/airflow/providers/common/sql/sensors/sql.py` & `apache-airflow-providers-common-sql-1.5.1rc1/airflow/providers/common/sql/sensors/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.1/apache_airflow_providers_common_sql.egg-info/PKG-INFO` & `apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.5.1
+Version: 1.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.1/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.5.1``
+Release: ``1.5.1rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-common-sql-1.5.1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt` & `apache-airflow-providers-common-sql-1.5.1rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.1/pyproject.toml` & `apache-airflow-providers-common-sql-1.5.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.5.1/setup.cfg` & `apache-airflow-providers-common-sql-1.5.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,21 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	sqlparse>=0.4.2
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.common.sql.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.common.sql
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-common-sql-1.5.1/setup.py` & `apache-airflow-providers-common-sql-1.5.1rc1/setup.py`

 * *Files identical despite different names*

