# Comparing `tmp/tencentcloud-sdk-python-rp-3.0.917.tar.gz` & `tmp/tencentcloud-sdk-python-rp-3.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-rp-3.0.917.tar", last modified: Mon Jun 19 00:31:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-rp-3.0.918.tar", last modified: Tue Jun 20 02:46:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-rp-3.0.917.tar` & `tencentcloud-sdk-python-rp-3.0.918.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud_sdk_python_rp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud_sdk_python_rp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      435 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud_sdk_python_rp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud_sdk_python_rp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud_sdk_python_rp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud/rp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud/rp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud/rp/v20200224/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud/rp/v20200224/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9659 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud/rp/v20200224/models.py
--rw-r--r--   0 root         (0) root         (0)     2220 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud/rp/v20200224/rp_client.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/tencentcloud/rp/v20200224/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/README.rst
--rw-r--r--   0 root         (0) root         (0)     1654 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1004 2023-06-19 00:31:20.000000 tencentcloud-sdk-python-rp-3.0.917/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud_sdk_python_rp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud_sdk_python_rp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud_sdk_python_rp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud_sdk_python_rp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud_sdk_python_rp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud/rp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud/rp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud/rp/v20200224/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud/rp/v20200224/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9659 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud/rp/v20200224/models.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud/rp/v20200224/rp_client.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/tencentcloud/rp/v20200224/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-06-20 02:46:30.000000 tencentcloud-sdk-python-rp-3.0.918/setup.py
```

### Comparing `tencentcloud-sdk-python-rp-3.0.917/tencentcloud_sdk_python_rp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-rp-3.0.918/tencentcloud_sdk_python_rp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rp
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Rp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rp-3.0.917/tencentcloud/__init__.py` & `tencentcloud-sdk-python-rp-3.0.918/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-rp-3.0.917/tencentcloud/rp/v20200224/models.py` & `tencentcloud-sdk-python-rp-3.0.918/tencentcloud/rp/v20200224/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rp-3.0.917/tencentcloud/rp/v20200224/rp_client.py` & `tencentcloud-sdk-python-rp-3.0.918/tencentcloud/rp/v20200224/rp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rp-3.0.917/tencentcloud/rp/v20200224/errorcodes.py` & `tencentcloud-sdk-python-rp-3.0.918/tencentcloud/rp/v20200224/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rp-3.0.917/README.rst` & `tencentcloud-sdk-python-rp-3.0.918/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rp-3.0.917/PKG-INFO` & `tencentcloud-sdk-python-rp-3.0.918/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rp
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Rp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rp-3.0.917/setup.py` & `tencentcloud-sdk-python-rp-3.0.918/setup.py`

 * *Files identical despite different names*

