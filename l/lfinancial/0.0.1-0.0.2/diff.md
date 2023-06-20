# Comparing `tmp/lfinancial-0.0.1.tar.gz` & `tmp/lfinancial-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.0.1.tar", last modified: Tue Jun 20 16:21:58 2023, max compression
+gzip compressed data, was "lfinancial-0.0.2.tar", last modified: Tue Jun 20 16:59:06 2023, max compression
```

## Comparing `lfinancial-0.0.1.tar` & `lfinancial-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-20 16:21:58.281653 lfinancial-0.0.1/
--rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-20 16:21:58.281557 lfinancial-0.0.1/PKG-INFO
--rw-r--r--   0 lzy        (501) staff       (20)       76 2023-06-20 15:54:53.000000 lfinancial-0.0.1/README.md
-drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-20 16:21:58.281004 lfinancial-0.0.1/lfinancial/
--rw-r--r--   0 lzy        (501) staff       (20)       33 2023-06-20 16:21:35.000000 lfinancial-0.0.1/lfinancial/__init__.py
--rw-r--r--   0 lzy        (501) staff       (20)      182 2023-06-20 16:21:28.000000 lfinancial-0.0.1/lfinancial/financial.py
-drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-20 16:21:58.281414 lfinancial-0.0.1/lfinancial.egg-info/
--rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-20 16:21:58.000000 lfinancial-0.0.1/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 lzy        (501) staff       (20)      201 2023-06-20 16:21:58.000000 lfinancial-0.0.1/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 lzy        (501) staff       (20)        1 2023-06-20 16:21:58.000000 lfinancial-0.0.1/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 lzy        (501) staff       (20)       11 2023-06-20 16:21:58.000000 lfinancial-0.0.1/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 lzy        (501) staff       (20)       38 2023-06-20 16:21:58.281682 lfinancial-0.0.1/setup.cfg
--rw-r--r--   0 lzy        (501) staff       (20)      568 2023-06-20 16:20:59.000000 lfinancial-0.0.1/setup.py
+drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-20 16:59:06.642574 lfinancial-0.0.2/
+-rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-20 16:59:06.642483 lfinancial-0.0.2/PKG-INFO
+-rw-r--r--   0 lzy        (501) staff       (20)       68 2023-06-20 16:50:45.000000 lfinancial-0.0.2/README.md
+drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-20 16:59:06.641989 lfinancial-0.0.2/lfinancial/
+-rw-r--r--   0 lzy        (501) staff       (20)       33 2023-06-20 16:21:35.000000 lfinancial-0.0.2/lfinancial/__init__.py
+-rw-r--r--   0 lzy        (501) staff       (20)      155 2023-06-20 16:56:11.000000 lfinancial-0.0.2/lfinancial/financial.py
+-rw-r--r--   0 lzy        (501) staff       (20)      741 2023-06-20 16:56:11.000000 lfinancial-0.0.2/lfinancial/generators.py
+drwxr-xr-x   0 lzy        (501) staff       (20)        0 2023-06-20 16:59:06.642335 lfinancial-0.0.2/lfinancial.egg-info/
+-rw-r--r--   0 lzy        (501) staff       (20)      289 2023-06-20 16:59:06.000000 lfinancial-0.0.2/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 lzy        (501) staff       (20)      226 2023-06-20 16:59:06.000000 lfinancial-0.0.2/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 lzy        (501) staff       (20)        1 2023-06-20 16:59:06.000000 lfinancial-0.0.2/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 lzy        (501) staff       (20)       11 2023-06-20 16:59:06.000000 lfinancial-0.0.2/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 lzy        (501) staff       (20)       38 2023-06-20 16:59:06.642603 lfinancial-0.0.2/setup.cfg
+-rw-r--r--   0 lzy        (501) staff       (20)      568 2023-06-20 16:58:21.000000 lfinancial-0.0.2/setup.py
```

### Comparing `lfinancial-0.0.1/setup.py` & `lfinancial-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 excluded_packages = ["docs", "tests", "tests.*"]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lfinancial',
-    version='0.0.1',
+    version='0.0.2',
     author='zaneliu',
     author_email='lzy291980138@163.com',
     description='Generate financial test data',
     packages=['lfinancial'],
     install_requires=[],
     classifiers=[
         'Programming Language :: Python :: 3',
```

