# Comparing `tmp/FlowAnalyzer-0.1.0.tar.gz` & `tmp/FlowAnalyzer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowAnalyzer-0.1.0.tar", last modified: Sat Jun 17 15:35:37 2023, max compression
+gzip compressed data, was "FlowAnalyzer-0.1.1.tar", last modified: Tue Jun 20 05:21:10 2023, max compression
```

## Comparing `FlowAnalyzer-0.1.0.tar` & `FlowAnalyzer-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 15:35:37.354898 FlowAnalyzer-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-17 15:35:37.351897 FlowAnalyzer-0.1.0/FlowAnalyzer/
--rw-rw-rw-   0        0        0     5170 2023-06-17 14:16:52.000000 FlowAnalyzer-0.1.0/FlowAnalyzer/FlowAnalyzer.py
--rw-rw-rw-   0        0        0       70 2023-06-16 14:40:24.000000 FlowAnalyzer-0.1.0/FlowAnalyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 15:35:37.353897 FlowAnalyzer-0.1.0/FlowAnalyzer.egg-info/
--rw-rw-rw-   0        0        0     6271 2023-06-17 15:35:37.000000 FlowAnalyzer-0.1.0/FlowAnalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-17 15:35:37.000000 FlowAnalyzer-0.1.0/FlowAnalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 15:35:37.000000 FlowAnalyzer-0.1.0/FlowAnalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-17 15:35:37.000000 FlowAnalyzer-0.1.0/FlowAnalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-06-17 13:51:39.000000 FlowAnalyzer-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     6271 2023-06-17 15:35:37.354898 FlowAnalyzer-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5236 2023-06-17 15:05:24.000000 FlowAnalyzer-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 15:35:37.354898 FlowAnalyzer-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1144 2023-06-17 15:28:04.000000 FlowAnalyzer-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:21:10.792611 FlowAnalyzer-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-20 05:21:10.789611 FlowAnalyzer-0.1.1/FlowAnalyzer/
+-rw-rw-rw-   0        0        0     6803 2023-06-20 05:17:17.000000 FlowAnalyzer-0.1.1/FlowAnalyzer/FlowAnalyzer.py
+-rw-rw-rw-   0        0        0       70 2023-06-16 14:40:24.000000 FlowAnalyzer-0.1.1/FlowAnalyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:21:10.791611 FlowAnalyzer-0.1.1/FlowAnalyzer.egg-info/
+-rw-rw-rw-   0        0        0     6271 2023-06-20 05:21:10.000000 FlowAnalyzer-0.1.1/FlowAnalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-20 05:21:10.000000 FlowAnalyzer-0.1.1/FlowAnalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 05:21:10.000000 FlowAnalyzer-0.1.1/FlowAnalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 05:21:10.000000 FlowAnalyzer-0.1.1/FlowAnalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-06-17 13:51:39.000000 FlowAnalyzer-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6271 2023-06-20 05:21:10.791611 FlowAnalyzer-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5236 2023-06-20 05:17:46.000000 FlowAnalyzer-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 05:21:10.792611 FlowAnalyzer-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1144 2023-06-20 05:18:00.000000 FlowAnalyzer-0.1.1/setup.py
```

### Comparing `FlowAnalyzer-0.1.0/FlowAnalyzer.egg-info/PKG-INFO` & `FlowAnalyzer-0.1.1/FlowAnalyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: FlowAnalyzer
-Version: 0.1.0
+Version: 0.1.1
 Summary: FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件
 Home-page: https://github.com/Byxs20/FlowAnalyzer
 Author: Byxs20
 Author-email: 97766819@qq.com
 License: UNKNOWN
 Description: # FlowAnalyzer
         
         # Installation
         
         Install the package using pip:
         
         ```
-        pip3 insatll FlowAnalyzer
+        pip3 install FlowAnalyzer
         ```
         
         # Usage
         
         ```
         $ git clone https://github.com/Byxs20/FlowAnalyzer.git
         $ cd ./FlowAnalyzer/
```

### Comparing `FlowAnalyzer-0.1.0/LICENSE` & `FlowAnalyzer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowAnalyzer-0.1.0/PKG-INFO` & `FlowAnalyzer-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: FlowAnalyzer
-Version: 0.1.0
+Version: 0.1.1
 Summary: FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件
 Home-page: https://github.com/Byxs20/FlowAnalyzer
 Author: Byxs20
 Author-email: 97766819@qq.com
 License: UNKNOWN
 Description: # FlowAnalyzer
         
         # Installation
         
         Install the package using pip:
         
         ```
-        pip3 insatll FlowAnalyzer
+        pip3 install FlowAnalyzer
         ```
         
         # Usage
         
         ```
         $ git clone https://github.com/Byxs20/FlowAnalyzer.git
         $ cd ./FlowAnalyzer/
```

### Comparing `FlowAnalyzer-0.1.0/README.md` & `FlowAnalyzer-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # FlowAnalyzer
 
 # Installation
 
 Install the package using pip:
 
 ```
-pip3 insatll FlowAnalyzer
+pip3 install FlowAnalyzer
 ```
 
 # Usage
 
 ```
 $ git clone https://github.com/Byxs20/FlowAnalyzer.git
 $ cd ./FlowAnalyzer/
```

### Comparing `FlowAnalyzer-0.1.0/setup.py` & `FlowAnalyzer-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="FlowAnalyzer",
-    version="0.1.0",
+    version="0.1.1",
     description="FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件",
     author="Byxs20",
     author_email="97766819@qq.com",
     packages=find_packages(exclude=["tests", "*.egg-info"]),
     package_data={
         '': ['LICENSE', 'README.md', 'setup.py'],
     },
```

