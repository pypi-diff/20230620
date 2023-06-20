# Comparing `tmp/CallingGPT-0.0.0.6.tar.gz` & `tmp/CallingGPT-0.0.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CallingGPT-0.0.0.6.tar", last modified: Tue Jun 20 13:58:56 2023, max compression
+gzip compressed data, was "CallingGPT-0.0.0.6.1.tar", last modified: Tue Jun 20 14:04:40 2023, max compression
```

## Comparing `CallingGPT-0.0.0.6.tar` & `CallingGPT-0.0.0.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 13:58:56.182616 CallingGPT-0.0.0.6/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4492 2023-06-20 13:58:56.182616 CallingGPT-0.0.0.6/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4088 2023-06-20 11:59:45.000000 CallingGPT-0.0.0.6/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-20 13:58:56.182616 CallingGPT-0.0.0.6/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      734 2023-06-20 13:58:32.000000 CallingGPT-0.0.0.6/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 13:58:56.158616 CallingGPT-0.0.0.6/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 13:58:56.162616 CallingGPT-0.0.0.6/src/CallingGPT/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:05:39.000000 CallingGPT-0.0.0.6/src/CallingGPT/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 13:58:56.178616 CallingGPT-0.0.0.6/src/CallingGPT/cli/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1887 2023-06-20 11:59:49.000000 CallingGPT-0.0.0.6/src/CallingGPT/cli/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 13:58:56.178616 CallingGPT-0.0.0.6/src/CallingGPT/entities/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:09:28.000000 CallingGPT-0.0.0.6/src/CallingGPT/entities/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6805 2023-06-20 12:29:42.000000 CallingGPT-0.0.0.6/src/CallingGPT/entities/namespace.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 13:58:56.182616 CallingGPT-0.0.0.6/src/CallingGPT/session/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 07:58:52.000000 CallingGPT-0.0.0.6/src/CallingGPT/session/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1913 2023-06-20 12:29:42.000000 CallingGPT-0.0.0.6/src/CallingGPT/session/session.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 13:58:56.174616 CallingGPT-0.0.0.6/src/CallingGPT.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4492 2023-06-20 13:58:56.000000 CallingGPT-0.0.0.6/src/CallingGPT.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      407 2023-06-20 13:58:56.000000 CallingGPT-0.0.0.6/src/CallingGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-20 13:58:56.000000 CallingGPT-0.0.0.6/src/CallingGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-20 13:58:56.000000 CallingGPT-0.0.0.6/src/CallingGPT.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       11 2023-06-20 13:58:56.000000 CallingGPT-0.0.0.6/src/CallingGPT.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 14:04:40.282616 CallingGPT-0.0.0.6.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4494 2023-06-20 14:04:40.282616 CallingGPT-0.0.0.6.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4088 2023-06-20 11:59:45.000000 CallingGPT-0.0.0.6.1/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-20 14:04:40.282616 CallingGPT-0.0.0.6.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      787 2023-06-20 14:04:30.000000 CallingGPT-0.0.0.6.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 14:04:40.270616 CallingGPT-0.0.0.6.1/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 14:04:40.274616 CallingGPT-0.0.0.6.1/src/CallingGPT/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:05:39.000000 CallingGPT-0.0.0.6.1/src/CallingGPT/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 14:04:40.278616 CallingGPT-0.0.0.6.1/src/CallingGPT/cli/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1887 2023-06-20 11:59:49.000000 CallingGPT-0.0.0.6.1/src/CallingGPT/cli/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 14:04:40.278616 CallingGPT-0.0.0.6.1/src/CallingGPT/entities/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:09:28.000000 CallingGPT-0.0.0.6.1/src/CallingGPT/entities/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6805 2023-06-20 12:29:42.000000 CallingGPT-0.0.0.6.1/src/CallingGPT/entities/namespace.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 14:04:40.282616 CallingGPT-0.0.0.6.1/src/CallingGPT/session/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 07:58:52.000000 CallingGPT-0.0.0.6.1/src/CallingGPT/session/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1913 2023-06-20 12:29:42.000000 CallingGPT-0.0.0.6.1/src/CallingGPT/session/session.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-20 14:04:40.278616 CallingGPT-0.0.0.6.1/src/CallingGPT.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4494 2023-06-20 14:04:40.000000 CallingGPT-0.0.0.6.1/src/CallingGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      407 2023-06-20 14:04:40.000000 CallingGPT-0.0.0.6.1/src/CallingGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-20 14:04:40.000000 CallingGPT-0.0.0.6.1/src/CallingGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-20 14:04:40.000000 CallingGPT-0.0.0.6.1/src/CallingGPT.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       11 2023-06-20 14:04:40.000000 CallingGPT-0.0.0.6.1/src/CallingGPT.egg-info/top_level.txt
```

### Comparing `CallingGPT-0.0.0.6/PKG-INFO` & `CallingGPT-0.0.0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CallingGPT
-Version: 0.0.0.6
+Version: 0.0.0.6.1
 Summary: GPT's function calling feature wrapper
 Home-page: https://github.com/RockChinQ/CallingGPT
 Author: RockChinQ
 Author-email: 1010553892@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `CallingGPT-0.0.0.6/README.md` & `CallingGPT-0.0.0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `CallingGPT-0.0.0.6/src/CallingGPT/cli/__init__.py` & `CallingGPT-0.0.0.6.1/src/CallingGPT/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `CallingGPT-0.0.0.6/src/CallingGPT/entities/namespace.py` & `CallingGPT-0.0.0.6.1/src/CallingGPT/entities/namespace.py`

 * *Files identical despite different names*

### Comparing `CallingGPT-0.0.0.6/src/CallingGPT/session/session.py` & `CallingGPT-0.0.0.6.1/src/CallingGPT/session/session.py`

 * *Files identical despite different names*

### Comparing `CallingGPT-0.0.0.6/src/CallingGPT.egg-info/PKG-INFO` & `CallingGPT-0.0.0.6.1/src/CallingGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CallingGPT
-Version: 0.0.0.6
+Version: 0.0.0.6.1
 Summary: GPT's function calling feature wrapper
 Home-page: https://github.com/RockChinQ/CallingGPT
 Author: RockChinQ
 Author-email: 1010553892@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

