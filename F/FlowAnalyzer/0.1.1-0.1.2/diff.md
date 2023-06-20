# Comparing `tmp/FlowAnalyzer-0.1.1.tar.gz` & `tmp/FlowAnalyzer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowAnalyzer-0.1.1.tar", last modified: Tue Jun 20 05:21:10 2023, max compression
+gzip compressed data, was "FlowAnalyzer-0.1.2.tar", last modified: Tue Jun 20 05:45:56 2023, max compression
```

## Comparing `FlowAnalyzer-0.1.1.tar` & `FlowAnalyzer-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 05:21:10.792611 FlowAnalyzer-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-20 05:21:10.789611 FlowAnalyzer-0.1.1/FlowAnalyzer/
--rw-rw-rw-   0        0        0     6803 2023-06-20 05:17:17.000000 FlowAnalyzer-0.1.1/FlowAnalyzer/FlowAnalyzer.py
--rw-rw-rw-   0        0        0       70 2023-06-16 14:40:24.000000 FlowAnalyzer-0.1.1/FlowAnalyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:21:10.791611 FlowAnalyzer-0.1.1/FlowAnalyzer.egg-info/
--rw-rw-rw-   0        0        0     6271 2023-06-20 05:21:10.000000 FlowAnalyzer-0.1.1/FlowAnalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-20 05:21:10.000000 FlowAnalyzer-0.1.1/FlowAnalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 05:21:10.000000 FlowAnalyzer-0.1.1/FlowAnalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-20 05:21:10.000000 FlowAnalyzer-0.1.1/FlowAnalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-06-17 13:51:39.000000 FlowAnalyzer-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6271 2023-06-20 05:21:10.791611 FlowAnalyzer-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5236 2023-06-20 05:17:46.000000 FlowAnalyzer-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 05:21:10.792611 FlowAnalyzer-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1144 2023-06-20 05:18:00.000000 FlowAnalyzer-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:45:56.948942 FlowAnalyzer-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-20 05:45:56.944941 FlowAnalyzer-0.1.2/FlowAnalyzer/
+-rw-rw-rw-   0        0        0     6796 2023-06-20 05:45:06.000000 FlowAnalyzer-0.1.2/FlowAnalyzer/FlowAnalyzer.py
+-rw-rw-rw-   0        0        0       70 2023-06-16 14:40:24.000000 FlowAnalyzer-0.1.2/FlowAnalyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:45:56.947441 FlowAnalyzer-0.1.2/FlowAnalyzer.egg-info/
+-rw-rw-rw-   0        0        0     6271 2023-06-20 05:45:56.000000 FlowAnalyzer-0.1.2/FlowAnalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-20 05:45:56.000000 FlowAnalyzer-0.1.2/FlowAnalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 05:45:56.000000 FlowAnalyzer-0.1.2/FlowAnalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 05:45:56.000000 FlowAnalyzer-0.1.2/FlowAnalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-06-17 13:51:39.000000 FlowAnalyzer-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6271 2023-06-20 05:45:56.948441 FlowAnalyzer-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5236 2023-06-20 05:17:46.000000 FlowAnalyzer-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 05:45:56.948942 FlowAnalyzer-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1144 2023-06-20 05:45:55.000000 FlowAnalyzer-0.1.2/setup.py
```

### Comparing `FlowAnalyzer-0.1.1/FlowAnalyzer/FlowAnalyzer.py` & `FlowAnalyzer-0.1.2/FlowAnalyzer/FlowAnalyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,10 +147,10 @@
             if not save_http_header:
                 num = full_request.find(b"\r\n\r\n")
                 full_request = re.findall(b'^\r\n\r\n.*?\r\n(.*)\r\n.*?\r\n\r\n$', full_request[num:], flags=re.DOTALL)[0]
             full_request = re.sub(b"\r\n.{4}\r\n", b"", full_request) # 由于是多个tcp所以需要去除应该是长度的字节 不确定是不是4个字节 后期可能出现bug
             
         try:
             return gzip.decompress(full_request)
-        except gzip.BadGzipFile:
+        except Exception:
             return full_request
```

### Comparing `FlowAnalyzer-0.1.1/FlowAnalyzer.egg-info/PKG-INFO` & `FlowAnalyzer-0.1.2/FlowAnalyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowAnalyzer
-Version: 0.1.1
+Version: 0.1.2
 Summary: FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件
 Home-page: https://github.com/Byxs20/FlowAnalyzer
 Author: Byxs20
 Author-email: 97766819@qq.com
 License: UNKNOWN
 Description: # FlowAnalyzer
```

### Comparing `FlowAnalyzer-0.1.1/LICENSE` & `FlowAnalyzer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowAnalyzer-0.1.1/PKG-INFO` & `FlowAnalyzer-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowAnalyzer
-Version: 0.1.1
+Version: 0.1.2
 Summary: FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件
 Home-page: https://github.com/Byxs20/FlowAnalyzer
 Author: Byxs20
 Author-email: 97766819@qq.com
 License: UNKNOWN
 Description: # FlowAnalyzer
```

### Comparing `FlowAnalyzer-0.1.1/README.md` & `FlowAnalyzer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `FlowAnalyzer-0.1.1/setup.py` & `FlowAnalyzer-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="FlowAnalyzer",
-    version="0.1.1",
+    version="0.1.2",
     description="FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件",
     author="Byxs20",
     author_email="97766819@qq.com",
     packages=find_packages(exclude=["tests", "*.egg-info"]),
     package_data={
         '': ['LICENSE', 'README.md', 'setup.py'],
     },
```

