# Comparing `tmp/ghga_transpiler-1.0.1.tar.gz` & `tmp/ghga_transpiler-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_transpiler-1.0.1.tar", last modified: Tue Jun 20 19:25:27 2023, max compression
+gzip compressed data, was "ghga_transpiler-1.0.2.tar", last modified: Tue Jun 20 19:36:04 2023, max compression
```

## Comparing `ghga_transpiler-1.0.1.tar` & `ghga_transpiler-1.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:25:27.477549 ghga_transpiler-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-20 19:25:27.481550 ghga_transpiler-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:25:27.473549 ghga_transpiler-1.0.1/ghga_transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/ghga_transpiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/ghga_transpiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/ghga_transpiler/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:25:27.477549 ghga_transpiler-1.0.1/ghga_transpiler/config/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/ghga_transpiler/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/ghga_transpiler/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/ghga_transpiler/config/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:25:27.477549 ghga_transpiler-1.0.1/ghga_transpiler/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/ghga_transpiler/configs/0.10.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/ghga_transpiler/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/ghga_transpiler/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/ghga_transpiler/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/ghga_transpiler/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:25:27.477549 ghga_transpiler-1.0.1/ghga_transpiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-20 19:25:27.000000 ghga_transpiler-1.0.1/ghga_transpiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-20 19:25:27.000000 ghga_transpiler-1.0.1/ghga_transpiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:25:27.000000 ghga_transpiler-1.0.1/ghga_transpiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 19:25:27.000000 ghga_transpiler-1.0.1/ghga_transpiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:25:27.000000 ghga_transpiler-1.0.1/ghga_transpiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-20 19:25:27.000000 ghga_transpiler-1.0.1/ghga_transpiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 19:25:27.000000 ghga_transpiler-1.0.1/ghga_transpiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-20 19:25:27.481550 ghga_transpiler-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:25:27.477549 ghga_transpiler-1.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:25:27.477549 ghga_transpiler-1.0.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:25:27.477549 ghga_transpiler-1.0.1/tests/fixtures/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/tests/fixtures/configs/0.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/tests/fixtures/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:25:27.477549 ghga_transpiler-1.0.1/tests/fixtures/test_data_objects/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/tests/fixtures/test_data_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/tests/fixtures/test_data_objects/conversion_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/tests/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/tests/test_convert_workbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/tests/test_create_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-20 19:25:16.000000 ghga_transpiler-1.0.1/tests/test_process_workbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:36:04.058660 ghga_transpiler-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-20 19:36:04.058660 ghga_transpiler-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:36:04.046660 ghga_transpiler-1.0.2/ghga_transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/ghga_transpiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/ghga_transpiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/ghga_transpiler/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:36:04.054660 ghga_transpiler-1.0.2/ghga_transpiler/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/ghga_transpiler/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/ghga_transpiler/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/ghga_transpiler/config/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:36:04.054660 ghga_transpiler-1.0.2/ghga_transpiler/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/ghga_transpiler/configs/0.10.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/ghga_transpiler/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/ghga_transpiler/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/ghga_transpiler/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/ghga_transpiler/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:36:04.050660 ghga_transpiler-1.0.2/ghga_transpiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-20 19:36:04.000000 ghga_transpiler-1.0.2/ghga_transpiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-20 19:36:04.000000 ghga_transpiler-1.0.2/ghga_transpiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:36:04.000000 ghga_transpiler-1.0.2/ghga_transpiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 19:36:04.000000 ghga_transpiler-1.0.2/ghga_transpiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:36:03.000000 ghga_transpiler-1.0.2/ghga_transpiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 19:36:04.000000 ghga_transpiler-1.0.2/ghga_transpiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 19:36:04.000000 ghga_transpiler-1.0.2/ghga_transpiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 19:36:04.058660 ghga_transpiler-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:36:04.054660 ghga_transpiler-1.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:36:04.054660 ghga_transpiler-1.0.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:36:04.054660 ghga_transpiler-1.0.2/tests/fixtures/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/tests/fixtures/configs/0.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/tests/fixtures/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:36:04.058660 ghga_transpiler-1.0.2/tests/fixtures/test_data_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/tests/fixtures/test_data_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/tests/fixtures/test_data_objects/conversion_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/tests/test_convert_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/tests/test_create_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-20 19:35:53.000000 ghga_transpiler-1.0.2/tests/test_process_workbook.py
```

### Comparing `ghga_transpiler-1.0.1/LICENSE` & `ghga_transpiler-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/PKG-INFO` & `ghga_transpiler-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_transpiler
-Version: 1.0.1
+Version: 1.0.2
 Summary: GHGA-Transpiler - GHGA metadata XLSX to JSON transpilation
 Home-page: https://github.com/ghga-de/ghga-transpiler
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_transpiler-1.0.1/README.md` & `ghga_transpiler-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler/__init__.py` & `ghga_transpiler-1.0.2/ghga_transpiler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Short description of package"""  # Please adapt to package
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
```

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler/__main__.py` & `ghga_transpiler-1.0.2/ghga_transpiler/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler/cli.py` & `ghga_transpiler-1.0.2/ghga_transpiler/cli.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler/config/__init__.py` & `ghga_transpiler-1.0.2/ghga_transpiler/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler/config/config.py` & `ghga_transpiler-1.0.2/ghga_transpiler/config/config.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler/config/exceptions.py` & `ghga_transpiler-1.0.2/ghga_transpiler/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler/configs/0.10.0.yaml` & `ghga_transpiler-1.0.2/ghga_transpiler/configs/0.10.0.yaml`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler/configs/__init__.py` & `ghga_transpiler-1.0.2/ghga_transpiler/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler/core.py` & `ghga_transpiler-1.0.2/ghga_transpiler/core.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler/io.py` & `ghga_transpiler-1.0.2/ghga_transpiler/io.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler/transformations.py` & `ghga_transpiler-1.0.2/ghga_transpiler/transformations.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler.egg-info/PKG-INFO` & `ghga_transpiler-1.0.2/ghga_transpiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-transpiler
-Version: 1.0.1
+Version: 1.0.2
 Summary: GHGA-Transpiler - GHGA metadata XLSX to JSON transpilation
 Home-page: https://github.com/ghga-de/ghga-transpiler
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_transpiler-1.0.1/ghga_transpiler.egg-info/SOURCES.txt` & `ghga_transpiler-1.0.2/ghga_transpiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/setup.py` & `ghga_transpiler-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/tests/fixtures/__init__.py` & `ghga_transpiler-1.0.2/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/tests/fixtures/configs/__init__.py` & `ghga_transpiler-1.0.2/tests/fixtures/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/tests/fixtures/test_data_objects/__init__.py` & `ghga_transpiler-1.0.2/tests/fixtures/test_data_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/tests/fixtures/test_data_objects/conversion_data.py` & `ghga_transpiler-1.0.2/tests/fixtures/test_data_objects/conversion_data.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/tests/fixtures/utils.py` & `ghga_transpiler-1.0.2/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/tests/test_convert_workbook.py` & `ghga_transpiler-1.0.2/tests/test_convert_workbook.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/tests/test_create_config.py` & `ghga_transpiler-1.0.2/tests/test_create_config.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/tests/test_io.py` & `ghga_transpiler-1.0.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `ghga_transpiler-1.0.1/tests/test_process_workbook.py` & `ghga_transpiler-1.0.2/tests/test_process_workbook.py`

 * *Files identical despite different names*

