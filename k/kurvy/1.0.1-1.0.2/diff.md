# Comparing `tmp/kurvy-1.0.1.tar.gz` & `tmp/kurvy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kurvy-1.0.1.tar", last modified: Tue Jun 20 08:44:25 2023, max compression
+gzip compressed data, was "kurvy-1.0.2.tar", last modified: Tue Jun 20 08:50:57 2023, max compression
```

## Comparing `kurvy-1.0.1.tar` & `kurvy-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 08:44:25.328637 kurvy-1.0.1/
--rw-r--r--   0 lucbatty   (501) staff       (20)     1069 2023-05-19 09:22:17.000000 kurvy-1.0.1/LICENSE
--rw-r--r--   0 lucbatty   (501) staff       (20)      727 2023-06-20 08:44:25.328112 kurvy-1.0.1/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)      338 2023-06-20 08:31:42.000000 kurvy-1.0.1/README.md
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 08:44:25.324926 kurvy-1.0.1/kurvy/
--rw-r--r--   0 lucbatty   (501) staff       (20)       71 2023-05-19 09:51:28.000000 kurvy-1.0.1/kurvy/__init__.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    12401 2023-05-23 12:33:36.000000 kurvy-1.0.1/kurvy/plots.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    17670 2023-05-23 12:33:36.000000 kurvy-1.0.1/kurvy/trig.py
--rw-r--r--   0 lucbatty   (501) staff       (20)     4475 2023-05-23 12:32:06.000000 kurvy-1.0.1/kurvy/utils.py
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 08:44:25.327336 kurvy-1.0.1/kurvy.egg-info/
--rw-r--r--   0 lucbatty   (501) staff       (20)      727 2023-06-20 08:44:25.000000 kurvy-1.0.1/kurvy.egg-info/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)      219 2023-06-20 08:44:25.000000 kurvy-1.0.1/kurvy.egg-info/SOURCES.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-20 08:44:25.000000 kurvy-1.0.1/kurvy.egg-info/dependency_links.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        6 2023-06-20 08:44:25.000000 kurvy-1.0.1/kurvy.egg-info/top_level.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)      380 2023-06-20 08:41:26.000000 kurvy-1.0.1/pyproject.toml
--rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-20 08:44:25.328849 kurvy-1.0.1/setup.cfg
--rw-r--r--   0 lucbatty   (501) staff       (20)      598 2023-06-20 08:43:58.000000 kurvy-1.0.1/setup.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 08:50:57.336665 kurvy-1.0.2/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1069 2023-05-19 09:22:17.000000 kurvy-1.0.2/LICENSE
+-rw-r--r--   0 lucbatty   (501) staff       (20)      831 2023-06-20 08:50:57.336287 kurvy-1.0.2/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)      338 2023-06-20 08:31:42.000000 kurvy-1.0.2/README.md
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 08:50:57.332279 kurvy-1.0.2/kurvy/
+-rw-r--r--   0 lucbatty   (501) staff       (20)       71 2023-05-19 09:51:28.000000 kurvy-1.0.2/kurvy/__init__.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    12401 2023-05-23 12:33:36.000000 kurvy-1.0.2/kurvy/plots.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    17670 2023-05-23 12:33:36.000000 kurvy-1.0.2/kurvy/trig.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)     4475 2023-05-23 12:32:06.000000 kurvy-1.0.2/kurvy/utils.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 08:50:57.335725 kurvy-1.0.2/kurvy.egg-info/
+-rw-r--r--   0 lucbatty   (501) staff       (20)      831 2023-06-20 08:50:57.000000 kurvy-1.0.2/kurvy.egg-info/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)      219 2023-06-20 08:50:57.000000 kurvy-1.0.2/kurvy.egg-info/SOURCES.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-20 08:50:57.000000 kurvy-1.0.2/kurvy.egg-info/dependency_links.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        6 2023-06-20 08:50:57.000000 kurvy-1.0.2/kurvy.egg-info/top_level.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)      231 2023-06-20 08:47:52.000000 kurvy-1.0.2/pyproject.toml
+-rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-20 08:50:57.336833 kurvy-1.0.2/setup.cfg
+-rw-r--r--   0 lucbatty   (501) staff       (20)      702 2023-06-20 08:50:22.000000 kurvy-1.0.2/setup.py
```

### Comparing `kurvy-1.0.1/LICENSE` & `kurvy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kurvy-1.0.1/PKG-INFO` & `kurvy-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: kurvy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Curve approximation toolkit
 Home-page: https://github.com/celerygemini/kurvy
 Author: celerygemini
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # kurvy
```

### Comparing `kurvy-1.0.1/kurvy/plots.py` & `kurvy-1.0.2/kurvy/plots.py`

 * *Files identical despite different names*

### Comparing `kurvy-1.0.1/kurvy/trig.py` & `kurvy-1.0.2/kurvy/trig.py`

 * *Files identical despite different names*

### Comparing `kurvy-1.0.1/kurvy/utils.py` & `kurvy-1.0.2/kurvy/utils.py`

 * *Files identical despite different names*

### Comparing `kurvy-1.0.1/kurvy.egg-info/PKG-INFO` & `kurvy-1.0.2/kurvy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: kurvy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Curve approximation toolkit
 Home-page: https://github.com/celerygemini/kurvy
 Author: celerygemini
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # kurvy
```

### Comparing `kurvy-1.0.1/setup.py` & `kurvy-1.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kurvy",
-    version="1.0.1",
+    version="1.0.2",
     author="celerygemini",
     description="Curve approximation toolkit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/celerygemini/kurvy",
     packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
+    classifiers = [
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
 )
```

