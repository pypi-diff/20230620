# Comparing `tmp/autodistill-detic-0.0.1.tar.gz` & `tmp/autodistill_detic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-detic-0.0.1.tar", last modified: Wed Jun  7 11:06:40 2023, max compression
+gzip compressed data, was "autodistill_detic-0.1.2.tar", last modified: Thu Jun  8 13:58:17 2023, max compression
```

## Comparing `autodistill-detic-0.0.1.tar` & `autodistill_detic-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:40.133344 autodistill-detic-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)      361 2023-06-07 11:06:40.133217 autodistill-detic-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)       18 2023-06-07 11:06:38.000000 autodistill-detic-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:40.132098 autodistill-detic-0.0.1/autodistill_detic/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-06-07 11:06:38.000000 autodistill-detic-0.0.1/autodistill_detic/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:40.133038 autodistill-detic-0.0.1/autodistill_detic.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      361 2023-06-07 11:06:40.000000 autodistill-detic-0.0.1/autodistill_detic.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      252 2023-06-07 11:06:40.000000 autodistill-detic-0.0.1/autodistill_detic.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 11:06:40.000000 autodistill-detic-0.0.1/autodistill_detic.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       53 2023-06-07 11:06:40.000000 autodistill-detic-0.0.1/autodistill_detic.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       18 2023-06-07 11:06:40.000000 autodistill-detic-0.0.1/autodistill_detic.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-07 11:06:40.133385 autodistill-detic-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      979 2023-06-07 11:06:38.000000 autodistill-detic-0.0.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 13:58:17.212259 autodistill_detic-0.1.2/
+-rw-r--r--   0 james      (501) staff       (20)     1055 2023-06-06 11:14:33.000000 autodistill_detic-0.1.2/LICENSE.md
+-rw-r--r--   0 james      (501) staff       (20)     2297 2023-06-08 13:58:17.212114 autodistill_detic-0.1.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1821 2023-06-06 11:15:52.000000 autodistill_detic-0.1.2/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 13:58:17.210645 autodistill_detic-0.1.2/autodistill_detic/
+-rw-r--r--   0 james      (501) staff       (20)       71 2023-06-08 13:58:14.000000 autodistill_detic-0.1.2/autodistill_detic/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     4802 2023-06-07 14:22:07.000000 autodistill_detic-0.1.2/autodistill_detic/detic_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 13:58:17.211565 autodistill_detic-0.1.2/autodistill_detic.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2297 2023-06-08 13:58:17.000000 autodistill_detic-0.1.2/autodistill_detic.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      315 2023-06-08 13:58:17.000000 autodistill_detic-0.1.2/autodistill_detic.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-08 13:58:17.000000 autodistill_detic-0.1.2/autodistill_detic.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       53 2023-06-08 13:58:17.000000 autodistill_detic-0.1.2/autodistill_detic.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       18 2023-06-08 13:58:17.000000 autodistill_detic-0.1.2/autodistill_detic.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-08 13:58:17.212307 autodistill_detic-0.1.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1161 2023-06-07 14:22:41.000000 autodistill_detic-0.1.2/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 13:58:17.211720 autodistill_detic-0.1.2/test/
+-rw-r--r--   0 james      (501) staff       (20)       91 2023-06-06 09:39:29.000000 autodistill_detic-0.1.2/test/test_hello.py
```

### Comparing `autodistill-detic-0.0.1/setup.py` & `autodistill_detic-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-
 import setuptools
 from setuptools import find_packages
 import re
 
 with open("./autodistill_detic/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="autodistill-detic",
+    name="autodistill_detic",
     version=version,
     author="Roboflow",
     author_email="support@roboflow.com",
-    description="",
+    description="DETIC module for use with Autodistill",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=[],
+    url="https://github.com/autodistill/autodistill-detic",
+    nstall_requires=[
+        "torch",
+        "supervision==0.9.0",
+        "numpy",
+        "autodistill"
+    ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
-
```

