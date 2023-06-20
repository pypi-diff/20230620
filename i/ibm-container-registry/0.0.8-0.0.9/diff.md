# Comparing `tmp/ibm-container-registry-0.0.8.tar.gz` & `tmp/ibm-container-registry-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ibm-container-registry-0.0.8.tar", last modified: Thu Aug 11 13:55:24 2022, max compression
+gzip compressed data, was "dist/ibm-container-registry-0.0.9.tar", last modified: Tue Jun 20 15:32:56 2023, max compression
```

## Comparing `ibm-container-registry-0.0.8.tar` & `ibm-container-registry-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-11 13:55:24.000000 ibm-container-registry-0.0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2022-08-11 13:54:05.000000 ibm-container-registry-0.0.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2022-08-11 13:54:05.000000 ibm-container-registry-0.0.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4209 2022-08-11 13:55:24.000000 ibm-container-registry-0.0.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3262 2022-08-11 13:54:05.000000 ibm-container-registry-0.0.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-11 13:55:24.000000 ibm-container-registry-0.0.8/ibm_container_registry/
--rw-rw-r--   0 travis    (2000) travis    (2000)      872 2022-08-11 13:54:05.000000 ibm-container-registry-0.0.8/ibm_container_registry/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2425 2022-08-11 13:54:05.000000 ibm-container-registry-0.0.8/ibm_container_registry/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   126420 2022-08-11 13:54:05.000000 ibm-container-registry-0.0.8/ibm_container_registry/container_registry_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      667 2022-08-11 13:54:05.000000 ibm-container-registry-0.0.8/ibm_container_registry/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92021 2022-08-11 13:54:05.000000 ibm-container-registry-0.0.8/ibm_container_registry/vulnerability_advisor_v3.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-08-11 13:55:24.000000 ibm-container-registry-0.0.8/ibm_container_registry.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4209 2022-08-11 13:55:24.000000 ibm-container-registry-0.0.8/ibm_container_registry.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      547 2022-08-11 13:55:24.000000 ibm-container-registry-0.0.8/ibm_container_registry.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-08-11 13:55:24.000000 ibm-container-registry-0.0.8/ibm_container_registry.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2022-08-11 13:55:24.000000 ibm-container-registry-0.0.8/ibm_container_registry.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2022-08-11 13:55:24.000000 ibm-container-registry-0.0.8/ibm_container_registry.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-08-11 13:54:32.000000 ibm-container-registry-0.0.8/ibm_container_registry.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      173 2022-08-11 13:54:05.000000 ibm-container-registry-0.0.8/requirements-dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2022-08-11 13:54:05.000000 ibm-container-registry-0.0.8/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-08-11 13:55:24.000000 ibm-container-registry-0.0.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2609 2022-08-11 13:54:05.000000 ibm-container-registry-0.0.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-20 15:32:56.000000 ibm-container-registry-0.0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-06-20 15:29:58.000000 ibm-container-registry-0.0.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2023-06-20 15:29:58.000000 ibm-container-registry-0.0.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4209 2023-06-20 15:32:56.000000 ibm-container-registry-0.0.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3262 2023-06-20 15:29:58.000000 ibm-container-registry-0.0.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-20 15:32:56.000000 ibm-container-registry-0.0.9/ibm_container_registry/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      872 2023-06-20 15:29:58.000000 ibm-container-registry-0.0.9/ibm_container_registry/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2425 2023-06-20 15:29:58.000000 ibm-container-registry-0.0.9/ibm_container_registry/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   126419 2023-06-20 15:29:58.000000 ibm-container-registry-0.0.9/ibm_container_registry/container_registry_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      667 2023-06-20 15:29:58.000000 ibm-container-registry-0.0.9/ibm_container_registry/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92020 2023-06-20 15:29:58.000000 ibm-container-registry-0.0.9/ibm_container_registry/vulnerability_advisor_v3.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-20 15:32:56.000000 ibm-container-registry-0.0.9/ibm_container_registry.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4209 2023-06-20 15:32:56.000000 ibm-container-registry-0.0.9/ibm_container_registry.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      547 2023-06-20 15:32:56.000000 ibm-container-registry-0.0.9/ibm_container_registry.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-20 15:32:56.000000 ibm-container-registry-0.0.9/ibm_container_registry.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2023-06-20 15:32:56.000000 ibm-container-registry-0.0.9/ibm_container_registry.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2023-06-20 15:32:56.000000 ibm-container-registry-0.0.9/ibm_container_registry.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-20 15:30:39.000000 ibm-container-registry-0.0.9/ibm_container_registry.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      173 2023-06-20 15:29:58.000000 ibm-container-registry-0.0.9/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2023-06-20 15:29:58.000000 ibm-container-registry-0.0.9/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-20 15:32:56.000000 ibm-container-registry-0.0.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2609 2023-06-20 15:29:58.000000 ibm-container-registry-0.0.9/setup.py
```

### Comparing `ibm-container-registry-0.0.8/LICENSE` & `ibm-container-registry-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-container-registry-0.0.8/PKG-INFO` & `ibm-container-registry-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-container-registry
-Version: 0.0.8
+Version: 0.0.9
 Summary: IBM Cloud Container Registry Python SDK
 Home-page: https://github.com/IBM/container-registry-python-sdk
 Author: IBM
 Author-email: alchemy.registry.squad@uk.ibm.com
 License: Apache 2.0
 Keywords: ibm_container_registry
 Classifier: Programming Language :: Python
@@ -75,21 +75,21 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibm-container-registry>=0.0.8"
+pip install --upgrade "ibm-container-registry>=0.0.9"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibm-container-registry>=0.0.8"
+easy_install --upgrade "ibm-container-registry>=0.0.9"
 ```
 
 ## Using the SDK
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/main/README.md)
 
 ## Questions
```

### Comparing `ibm-container-registry-0.0.8/README.md` & `ibm-container-registry-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,21 +52,21 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibm-container-registry>=0.0.8"
+pip install --upgrade "ibm-container-registry>=0.0.9"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibm-container-registry>=0.0.8"
+easy_install --upgrade "ibm-container-registry>=0.0.9"
 ```
 
 ## Using the SDK
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/main/README.md)
 
 ## Questions
```

### Comparing `ibm-container-registry-0.0.8/ibm_container_registry/__init__.py` & `ibm-container-registry-0.0.9/ibm_container_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-container-registry-0.0.8/ibm_container_registry/common.py` & `ibm-container-registry-0.0.9/ibm_container_registry/common.py`

 * *Files identical despite different names*

### Comparing `ibm-container-registry-0.0.8/ibm_container_registry/container_registry_v1.py` & `ibm-container-registry-0.0.9/ibm_container_registry/container_registry_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # IBM OpenAPI SDK Code Generator Version: 3.29.1-b338fb38-20210313-010605
- 
+
 """
 Management interface for IBM Cloud Container Registry
 """
 
 from typing import Dict, List
 import json
```

### Comparing `ibm-container-registry-0.0.8/ibm_container_registry/version.py` & `ibm-container-registry-0.0.9/ibm_container_registry/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of ibm_container_registry
 """
-__version__ = '0.0.8'
+__version__ = '0.0.9'
```

### Comparing `ibm-container-registry-0.0.8/ibm_container_registry/vulnerability_advisor_v3.py` & `ibm-container-registry-0.0.9/ibm_container_registry/vulnerability_advisor_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # IBM OpenAPI SDK Code Generator Version: 3.29.1-b338fb38-20210313-010605
- 
+
 """
 Management interface of Vulnerability Advisor for IBM Cloud Container Registry
 """
 
 from typing import Dict, List
 import json
```

### Comparing `ibm-container-registry-0.0.8/ibm_container_registry.egg-info/PKG-INFO` & `ibm-container-registry-0.0.9/ibm_container_registry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-container-registry
-Version: 0.0.8
+Version: 0.0.9
 Summary: IBM Cloud Container Registry Python SDK
 Home-page: https://github.com/IBM/container-registry-python-sdk
 Author: IBM
 Author-email: alchemy.registry.squad@uk.ibm.com
 License: Apache 2.0
 Keywords: ibm_container_registry
 Classifier: Programming Language :: Python
@@ -75,21 +75,21 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip` or `easy_install`:
 
 ```bash
-pip install --upgrade "ibm-container-registry>=0.0.8"
+pip install --upgrade "ibm-container-registry>=0.0.9"
 ```
 
 or
 
 ```bash
-easy_install --upgrade "ibm-container-registry>=0.0.8"
+easy_install --upgrade "ibm-container-registry>=0.0.9"
 ```
 
 ## Using the SDK
 For general SDK usage information, please see [this link](https://github.com/IBM/ibm-cloud-sdk-common/blob/main/README.md)
 
 ## Questions
```

### Comparing `ibm-container-registry-0.0.8/ibm_container_registry.egg-info/SOURCES.txt` & `ibm-container-registry-0.0.9/ibm_container_registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-container-registry-0.0.8/setup.py` & `ibm-container-registry-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 PACKAGE_NAME = 'ibm_container_registry'
 PACKAGE_DESC = 'IBM Cloud Container Registry Python SDK'
 
 with open('requirements.txt') as f:
     install_requires = [
         str(req) for req in pkg_resources.parse_requirements(f)
     ]
```

