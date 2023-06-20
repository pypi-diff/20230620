# Comparing `tmp/tencentcloud-sdk-python-apcas-3.0.917.tar.gz` & `tmp/tencentcloud-sdk-python-apcas-3.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apcas-3.0.917.tar", last modified: Mon Jun 19 00:17:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apcas-3.0.918.tar", last modified: Tue Jun 20 02:32:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apcas-3.0.917.tar` & `tencentcloud-sdk-python-apcas-3.0.918.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud_sdk_python_apcas.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud_sdk_python_apcas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud_sdk_python_apcas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud_sdk_python_apcas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud_sdk_python_apcas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/apcas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/apcas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/apcas/v20201127/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/apcas/v20201127/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23599 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/apcas/v20201127/models.py
--rw-r--r--   0 root         (0) root         (0)     7186 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/apcas/v20201127/apcas_client.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/apcas/v20201127/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/README.rst
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-19 00:17:21.000000 tencentcloud-sdk-python-apcas-3.0.917/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud_sdk_python_apcas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud_sdk_python_apcas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud_sdk_python_apcas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud_sdk_python_apcas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud_sdk_python_apcas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/apcas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/apcas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/apcas/v20201127/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/apcas/v20201127/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23599 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/apcas/v20201127/models.py
+-rw-r--r--   0 root         (0) root         (0)     7186 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/apcas/v20201127/apcas_client.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/apcas/v20201127/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-20 02:32:29.000000 tencentcloud-sdk-python-apcas-3.0.918/setup.py
```

### Comparing `tencentcloud-sdk-python-apcas-3.0.917/tencentcloud_sdk_python_apcas.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apcas-3.0.918/tencentcloud_sdk_python_apcas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apcas
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Apcas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.917'
+__version__ = '3.0.918'
```

### Comparing `tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/apcas/v20201127/models.py` & `tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/apcas/v20201127/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/apcas/v20201127/apcas_client.py` & `tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/apcas/v20201127/apcas_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apcas-3.0.917/tencentcloud/apcas/v20201127/errorcodes.py` & `tencentcloud-sdk-python-apcas-3.0.918/tencentcloud/apcas/v20201127/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apcas-3.0.917/README.rst` & `tencentcloud-sdk-python-apcas-3.0.918/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apcas-3.0.917/PKG-INFO` & `tencentcloud-sdk-python-apcas-3.0.918/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apcas
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Apcas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apcas-3.0.917/setup.py` & `tencentcloud-sdk-python-apcas-3.0.918/setup.py`

 * *Files identical despite different names*

