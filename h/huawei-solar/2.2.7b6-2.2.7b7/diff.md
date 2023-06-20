# Comparing `tmp/huawei-solar-2.2.7b6.tar.gz` & `tmp/huawei-solar-2.2.7b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huawei-solar-2.2.7b6.tar", last modified: Tue Apr 11 06:47:43 2023, max compression
+gzip compressed data, was "huawei-solar-2.2.7b7.tar", last modified: Tue Jun 20 09:56:04 2023, max compression
```

## Comparing `huawei-solar-2.2.7b6.tar` & `huawei-solar-2.2.7b7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:47:43.770935 huawei-solar-2.2.7b6/
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/.codecov.yml
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/.yamllint
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     7718 2023-04-11 06:47:43.770935 huawei-solar-2.2.7b6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7163 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/bridge_tst.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/requirements_test.txt
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-04-11 06:47:43.771935 huawei-solar-2.2.7b6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:47:43.755933 huawei-solar-2.2.7b6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:47:43.766934 huawei-solar-2.2.7b6/src/huawei_solar/
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/bridge.py
--rw-rw-rw-   0 root         (0) root         (0)     1764 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    11325 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/files.py
--rw-rw-rw-   0 root         (0) root         (0)    24953 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     6590 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/modbus.py
--rw-rw-rw-   0 root         (0) root         (0)    18080 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/register_names.py
--rw-rw-rw-   0 root         (0) root         (0)    22487 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/register_values.py
--rw-rw-rw-   0 root         (0) root         (0)    42679 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/registers.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/src/huawei_solar/utils.py
--rw-r--r--   0 root         (0) root         (0)      148 2023-04-11 06:47:43.000000 huawei-solar-2.2.7b6/src/huawei_solar/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:47:43.768935 huawei-solar-2.2.7b6/src/huawei_solar.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7718 2023-04-11 06:47:43.000000 huawei-solar-2.2.7b6/src/huawei_solar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      891 2023-04-11 06:47:43.000000 huawei-solar-2.2.7b6/src/huawei_solar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 06:47:43.000000 huawei-solar-2.2.7b6/src/huawei_solar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-04-11 06:47:43.000000 huawei-solar-2.2.7b6/src/huawei_solar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 06:47:43.000000 huawei-solar-2.2.7b6/src/huawei_solar.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3578 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:47:43.770935 huawei-solar-2.2.7b6/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2611 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tests/mock_huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     3531 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tests/test__registers__peak_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     6245 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tests/test__registers__time_of_use.py
--rw-rw-rw-   0 root         (0) root         (0)    16324 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tests/test_huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tests/test_registers.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-04-11 06:47:20.000000 huawei-solar-2.2.7b6/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:04.019492 huawei-solar-2.2.7b7/
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/.codecov.yml
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/.yamllint
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     7719 2023-06-20 09:56:04.019492 huawei-solar-2.2.7b7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7163 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/bridge_tst.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/requirements_test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-06-20 09:56:04.019492 huawei-solar-2.2.7b7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:04.010492 huawei-solar-2.2.7b7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:04.016492 huawei-solar-2.2.7b7/src/huawei_solar/
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11325 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/files.py
+-rw-rw-rw-   0 root         (0) root         (0)    24953 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     7019 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/modbus.py
+-rw-rw-rw-   0 root         (0) root         (0)    18080 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/register_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    22487 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/register_values.py
+-rw-rw-rw-   0 root         (0) root         (0)    42679 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/registers.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/src/huawei_solar/utils.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-20 09:56:03.000000 huawei-solar-2.2.7b7/src/huawei_solar/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:04.017492 huawei-solar-2.2.7b7/src/huawei_solar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7719 2023-06-20 09:56:03.000000 huawei-solar-2.2.7b7/src/huawei_solar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      891 2023-06-20 09:56:04.000000 huawei-solar-2.2.7b7/src/huawei_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 09:56:03.000000 huawei-solar-2.2.7b7/src/huawei_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-20 09:56:03.000000 huawei-solar-2.2.7b7/src/huawei_solar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 09:56:03.000000 huawei-solar-2.2.7b7/src/huawei_solar.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:04.018492 huawei-solar-2.2.7b7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2611 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tests/mock_huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     3531 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tests/test__registers__peak_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tests/test__registers__time_of_use.py
+-rw-rw-rw-   0 root         (0) root         (0)    16324 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tests/test_huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tests/test_registers.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-20 09:55:50.000000 huawei-solar-2.2.7b7/tox.ini
```

### Comparing `huawei-solar-2.2.7b6/.gitignore` & `huawei-solar-2.2.7b7/.gitignore`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/.gitlab-ci.yml` & `huawei-solar-2.2.7b7/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 # Official language image. Look for the different tagged releases at:
 # https://hub.docker.com/r/library/python/tags/
-image: python:3.10
+image: python:3.11
 
 # Change pip's cache directory to be inside the project directory since we can
 # only cache local items.
 variables:
   PIP_CACHE_DIR: "$CI_PROJECT_DIR/.cache/pip"
 
 # Pip's cache doesn't store the python packages
@@ -53,14 +53,15 @@
     - twine upload dist/*
   only:
     - tags
   artifacts:
     paths:
       - dist/
 
-python39:
-  stage: test
-  script: tox -e py39
-
 python310:
   stage: test
+  image: python:3.10
   script: tox -e py310
+
+python311:
+  stage: test
+  script: tox -e py311
```

### Comparing `huawei-solar-2.2.7b6/.pre-commit-config.yaml` & `huawei-solar-2.2.7b7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/LICENSE.md` & `huawei-solar-2.2.7b7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/PKG-INFO` & `huawei-solar-2.2.7b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: huawei-solar
-Version: 2.2.7b6
+Version: 2.2.7b7
 Summary: A Python wrapper for the Huawei Inverter modbus TCP API
 Home-page: https://gitlab.com/EmilV2/huawei-solar
 Author: Emil Vanherp
 Author-email: emil@vanherp.me
 License: MIT License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `huawei-solar-2.2.7b6/README.md` & `huawei-solar-2.2.7b7/README.md`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/bridge_tst.py` & `huawei-solar-2.2.7b7/bridge_tst.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/pyproject.toml` & `huawei-solar-2.2.7b7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/setup.cfg` & `huawei-solar-2.2.7b7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 long_description_content_type = text/markdown
 url = https://gitlab.com/EmilV2/huawei-solar
 author = Emil Vanherp
 author_email = emil@vanherp.me
 license = MIT License
 license_file = LICENSE.md
 classifiers = 
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	=src
 packages = find:
```

### Comparing `huawei-solar-2.2.7b6/src/huawei_solar/__init__.py` & `huawei-solar-2.2.7b7/src/huawei_solar/__init__.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/src/huawei_solar/bridge.py` & `huawei-solar-2.2.7b7/src/huawei_solar/bridge.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/src/huawei_solar/exceptions.py` & `huawei-solar-2.2.7b7/src/huawei_solar/exceptions.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/src/huawei_solar/files.py` & `huawei-solar-2.2.7b7/src/huawei_solar/files.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/src/huawei_solar/huawei_solar.py` & `huawei-solar-2.2.7b7/src/huawei_solar/huawei_solar.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/src/huawei_solar/modbus.py` & `huawei-solar-2.2.7b7/src/huawei_solar/modbus.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,46 +10,55 @@
 
 RECONNECT_DELAY = 1000  # in milliseconds
 WAIT_ON_CONNECT = 1500  # in milliseconds
 
 LOGGER = logging.getLogger(__name__)
 
 
-class AsyncHuaweiSolarModbusSerialClient(AsyncModbusSerialClient):
-    """Custom SerialClient with support for custom Huawei modbus messages"""
-
-    def __init__(self, port, baudrate, timeout: int, **serial_kwargs):
-        super().__init__(port, **serial_kwargs, baudrate=baudrate, reconnect_delay=RECONNECT_DELAY, timeout=timeout)
-        self.register(PrivateHuaweiModbusResponse)
-
-
-class AsyncHuaweiSolarModbusTcpClient(AsyncModbusTcpClient):
-    """Custom TcpClient that supports wait after connect and custom Huawei modbus messages"""
+class ModbusConnectionMixin:
+    """Mixin that adds support for custom Huawei modbus messages and delays upon reconnect"""
 
     connected_event = asyncio.Event()
 
-    def __init__(self, host, port, timeout) -> AsyncModbusTcpClient:
-        super().__init__(host, port, timeout=timeout, reconnect_delay=RECONNECT_DELAY)
-        self.register(PrivateHuaweiModbusResponse)
+    def __init__(self, *args, **kwargs) -> None:
+        """Add support for the custom Huawei modbus messages"""
+        super().__init__(*args, **kwargs)
+        super().register(PrivateHuaweiModbusResponse)
 
     def client_made_connection(self, protocol):
+        """Register that a connection has been made in an asyncio Event"""
         super().client_made_connection(protocol)
 
         async def _made_connection_task():
             LOGGER.debug("Waiting for %d milliseconds after connection before performing operations", WAIT_ON_CONNECT)
             await asyncio.sleep(WAIT_ON_CONNECT / 1000)
             self.connected_event.set()
 
         asyncio.create_task(_made_connection_task())
 
     def client_lost_connection(self, protocol):
+        """Register that a connection has been lost in an asyncio Event"""
         super().client_lost_connection(protocol)
         self.connected_event.clear()
 
 
+class AsyncHuaweiSolarModbusSerialClient(ModbusConnectionMixin, AsyncModbusSerialClient):
+    """Custom SerialClient with support for custom Huawei modbus messages"""
+
+    def __init__(self, port, baudrate, timeout: int, **serial_kwargs):
+        super().__init__(port, **serial_kwargs, baudrate=baudrate, reconnect_delay=RECONNECT_DELAY, timeout=timeout)
+
+
+class AsyncHuaweiSolarModbusTcpClient(ModbusConnectionMixin, AsyncModbusTcpClient):
+    """Custom TcpClient that supports wait after connect and custom Huawei modbus messages"""
+
+    def __init__(self, host, port, timeout) -> AsyncModbusTcpClient:
+        super().__init__(host, port, timeout=timeout, reconnect_delay=RECONNECT_DELAY)
+
+
 class PrivateHuaweiModbusResponse(ModbusResponse):
     """Response with the private Huawei Solar function code"""
 
     function_code = 0x41
     _rtu_byte_count_pos = 3
 
     def __init__(self, **kwargs):
```

### Comparing `huawei-solar-2.2.7b6/src/huawei_solar/register_names.py` & `huawei-solar-2.2.7b7/src/huawei_solar/register_names.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/src/huawei_solar/register_values.py` & `huawei-solar-2.2.7b7/src/huawei_solar/register_values.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/src/huawei_solar/registers.py` & `huawei-solar-2.2.7b7/src/huawei_solar/registers.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/src/huawei_solar.egg-info/PKG-INFO` & `huawei-solar-2.2.7b7/src/huawei_solar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: huawei-solar
-Version: 2.2.7b6
+Version: 2.2.7b7
 Summary: A Python wrapper for the Huawei Inverter modbus TCP API
 Home-page: https://gitlab.com/EmilV2/huawei-solar
 Author: Emil Vanherp
 Author-email: emil@vanherp.me
 License: MIT License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `huawei-solar-2.2.7b6/src/huawei_solar.egg-info/SOURCES.txt` & `huawei-solar-2.2.7b7/src/huawei_solar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/test.py` & `huawei-solar-2.2.7b7/test.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/tests/conftest.py` & `huawei-solar-2.2.7b7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/tests/mock_huawei_solar.py` & `huawei-solar-2.2.7b7/tests/mock_huawei_solar.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/tests/test__registers__peak_periods.py` & `huawei-solar-2.2.7b7/tests/test__registers__peak_periods.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/tests/test__registers__time_of_use.py` & `huawei-solar-2.2.7b7/tests/test__registers__time_of_use.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/tests/test_huawei_solar.py` & `huawei-solar-2.2.7b7/tests/test_huawei_solar.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/tests/test_registers.py` & `huawei-solar-2.2.7b7/tests/test_registers.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.7b6/tox.ini` & `huawei-solar-2.2.7b7/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # content of: tox.ini , put in same dir as setup.py
 [tox]
-envlist = py39, py310, py311, flake8, pylint, codecov, yamllint
+envlist = py310, py311, flake8, pylint, codecov, yamllint
 skip_missing_interpreters = True
 
 [testenv]
 # install the test-dependencies mentioned in pyproject.toml
 extras = test
 
 #changedir = tests
```

