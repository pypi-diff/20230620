# Comparing `tmp/haberpy-0.0.2.tar.gz` & `tmp/haberpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haberpy-0.0.2.tar", last modified: Thu Jan 19 20:33:10 2023, max compression
+gzip compressed data, was "haberpy-0.0.3.tar", last modified: Tue Jun 20 10:25:23 2023, max compression
```

## Comparing `haberpy-0.0.2.tar` & `haberpy-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-01-19 20:33:10.247462 haberpy-0.0.2/
--rw-rw-rw-   0        0        0    35149 2022-12-02 14:26:43.000000 haberpy-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1583 2023-01-19 20:33:10.245987 haberpy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-01-18 18:28:00.000000 haberpy-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-19 20:33:10.233073 haberpy-0.0.2/haberpy/
--rw-rw-rw-   0        0        0     1983 2023-01-18 18:20:50.000000 haberpy-0.0.2/haberpy/__init__.py
--rw-rw-rw-   0        0        0     1898 2023-01-18 17:56:43.000000 haberpy-0.0.2/haberpy/sport.py
-drwxrwxrwx   0        0        0        0 2023-01-19 20:33:10.243972 haberpy-0.0.2/haberpy.egg-info/
--rw-rw-rw-   0        0        0     1583 2023-01-19 20:33:10.000000 haberpy-0.0.2/haberpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-01-19 20:33:10.000000 haberpy-0.0.2/haberpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-19 20:33:10.000000 haberpy-0.0.2/haberpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-01-19 20:33:10.000000 haberpy-0.0.2/haberpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-19 20:33:10.247462 haberpy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      706 2023-01-19 20:31:00.000000 haberpy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:25:23.828973 haberpy-0.0.3/
+-rw-rw-rw-   0        0        0    35149 2022-12-02 14:26:43.000000 haberpy-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0    15042 2023-06-20 10:25:23.827969 haberpy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    14582 2023-06-20 10:22:53.000000 haberpy-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 10:25:23.799467 haberpy-0.0.3/haberpy/
+-rw-rw-rw-   0        0        0      331 2023-06-19 06:38:29.000000 haberpy-0.0.3/haberpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:25:23.824445 haberpy-0.0.3/haberpy/sondakika/
+-rw-rw-rw-   0        0        0     2565 2023-06-20 08:44:32.000000 haberpy-0.0.3/haberpy/sondakika/__init__.py
+-rw-rw-rw-   0        0        0     1292 2023-06-19 06:47:43.000000 haberpy-0.0.3/haberpy/sondakika/economy.py
+-rw-rw-rw-   0        0        0     1293 2023-06-20 08:43:03.000000 haberpy-0.0.3/haberpy/sondakika/magazine.py
+-rw-rw-rw-   0        0        0     1292 2023-06-20 08:41:47.000000 haberpy-0.0.3/haberpy/sondakika/policy.py
+-rw-rw-rw-   0        0        0     3216 2023-06-19 06:38:50.000000 haberpy-0.0.3/haberpy/sondakika/sport.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:25:23.808324 haberpy-0.0.3/haberpy.egg-info/
+-rw-rw-rw-   0        0        0    15042 2023-06-20 10:25:23.000000 haberpy-0.0.3/haberpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-06-20 10:25:23.000000 haberpy-0.0.3/haberpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:25:23.000000 haberpy-0.0.3/haberpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-20 10:25:23.000000 haberpy-0.0.3/haberpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 10:25:23.829980 haberpy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      806 2023-06-20 10:25:19.000000 haberpy-0.0.3/setup.py
```

### Comparing `haberpy-0.0.2/LICENSE` & `haberpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `haberpy-0.0.2/setup.py` & `haberpy-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="haberpy",
-    version="0.0.2",
-    description="Son dakika haberleri çekebilmenize yarar.",
-    long_description=open("README.md").read(),
+    version="0.0.3",
+    description="Haber sitelerinden bildirimleri kolay sekilde alabilmeniz icin tasarlanmis bir Python API",
+    long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
-    url="",
+    url="https://github.com/Meinos10/haberpy",
     author="Emre",
     author_email="rewoxirewo@gmail.com",
     license="MIT",
     #classifiers = [
     #"Programming Language :: Python :: 3",
     #"License :: OSI Approved :: MIT License",
     #"Operating System :: OS Independent",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

