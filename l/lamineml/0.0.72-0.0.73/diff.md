# Comparing `tmp/lamineml-0.0.72.tar.gz` & `tmp/lamineml-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamineml-0.0.72.tar", last modified: Sat May 27 10:38:45 2023, max compression
+gzip compressed data, was "lamineml-0.0.73.tar", last modified: Tue Jun 20 07:49:30 2023, max compression
```

## Comparing `lamineml-0.0.72.tar` & `lamineml-0.0.73.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-27 10:38:45.093236 lamineml-0.0.72/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.72/LICENSE
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-27 10:38:45.093236 lamineml-0.0.72/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.72/README.md
--rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-05-18 14:20:16.000000 lamineml-0.0.72/pyproject.toml
--rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-27 10:38:45.093236 lamineml-0.0.72/setup.cfg
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-27 10:38:45.089236 lamineml-0.0.72/src/
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-27 10:38:45.089236 lamineml-0.0.72/src/lamine/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.72/src/lamine/__init__.py
--rw-rw-r--   0 hello     (1000) hello     (1000)     5568 2023-05-27 10:37:30.000000 lamineml-0.0.72/src/lamine/tools.py
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-27 10:38:45.093236 lamineml-0.0.72/src/lamineml.egg-info/
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-27 10:38:45.000000 lamineml-0.0.72/src/lamineml.egg-info/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-27 10:38:45.000000 lamineml-0.0.72/src/lamineml.egg-info/SOURCES.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-27 10:38:45.000000 lamineml-0.0.72/src/lamineml.egg-info/dependency_links.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-27 10:38:45.000000 lamineml-0.0.72/src/lamineml.egg-info/top_level.txt
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-06-20 07:49:30.811950 lamineml-0.0.73/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.73/LICENSE
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-06-20 07:49:30.811950 lamineml-0.0.73/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.73/README.md
+-rw-rw-r--   0 hello     (1000) hello     (1000)      133 2023-06-20 06:47:59.000000 lamineml-0.0.73/pyproject.toml
+-rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-06-20 07:49:30.811950 lamineml-0.0.73/setup.cfg
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-06-20 07:49:30.807950 lamineml-0.0.73/src/
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-06-20 07:49:30.811950 lamineml-0.0.73/src/lamine/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.73/src/lamine/__init__.py
+-rw-rw-r--   0 hello     (1000) hello     (1000)     5566 2023-05-27 11:16:19.000000 lamineml-0.0.73/src/lamine/tools.py
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-06-20 07:49:30.811950 lamineml-0.0.73/src/lamineml.egg-info/
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-06-20 07:49:30.000000 lamineml-0.0.73/src/lamineml.egg-info/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-06-20 07:49:30.000000 lamineml-0.0.73/src/lamineml.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-06-20 07:49:30.000000 lamineml-0.0.73/src/lamineml.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-06-20 07:49:30.000000 lamineml-0.0.73/src/lamineml.egg-info/top_level.txt
```

### Comparing `lamineml-0.0.72/PKG-INFO` & `lamineml-0.0.73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.72
+Version: 0.0.73
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lamineml-0.0.72/README.md` & `lamineml-0.0.73/README.md`

 * *Files identical despite different names*

### Comparing `lamineml-0.0.72/setup.cfg` & `lamineml-0.0.73/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lamineml
-version = 0.0.72
+version = 0.0.73
 author = Lamine ML
 author_email = lamineml128@gmail.com
 description = use this library in kivy android
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `lamineml-0.0.72/src/lamine/tools.py` & `lamineml-0.0.73/src/lamine/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     installedPackages =PackageManager.getInstalledPackages(0);
     for i in installedPackages:
         a= i.packageName
         al.append(a.replace(",","\n"))
     return al
 @run_on_ui_thread
 def KEEP_SCREEN_ON():
-    activity.getWindow(). addFlags (window.FLAG_KEEP_SCREEN_ON)
+    activity.getWindow().addFlags(window.FLAG_KEEP_SCREEN_ON)
 def open_browser(url):
     intent = Intent()
     intent.setAction(Intent.ACTION_VIEW)
     intent.setData(uri.parse(url))
     activity.startActivity(intent)
 
 def copy_text(text):
```

### Comparing `lamineml-0.0.72/src/lamineml.egg-info/PKG-INFO` & `lamineml-0.0.73/src/lamineml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.72
+Version: 0.0.73
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

