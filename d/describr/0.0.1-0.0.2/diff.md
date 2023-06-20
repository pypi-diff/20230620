# Comparing `tmp/describr-0.0.1.tar.gz` & `tmp/describr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "describr-0.0.1.tar", last modified: Tue Jun 20 16:23:53 2023, max compression
+gzip compressed data, was "describr-0.0.2.tar", last modified: Tue Jun 20 16:47:25 2023, max compression
```

## Comparing `describr-0.0.1.tar` & `describr-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 16:23:53.505435 describr-0.0.1/
--rw-rw-rw-   0        0        0     1099 2023-06-20 15:03:20.000000 describr-0.0.1/LICENSE
--rw-rw-rw-   0        0        0   214601 2023-06-20 16:23:53.505435 describr-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3740 2023-06-20 15:28:09.000000 describr-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 16:23:53.461438 describr-0.0.1/describr/
--rw-rw-rw-   0        0        0      129 2023-06-20 14:56:12.000000 describr-0.0.1/describr/__init__.py
--rw-rw-rw-   0        0        0    16616 2023-06-20 14:40:14.000000 describr-0.0.1/describr/describr.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:23:53.503434 describr-0.0.1/describr.egg-info/
--rw-rw-rw-   0        0        0   214601 2023-06-20 16:23:53.000000 describr-0.0.1/describr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-20 16:23:53.000000 describr-0.0.1/describr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 16:23:53.000000 describr-0.0.1/describr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-20 16:23:53.000000 describr-0.0.1/describr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 16:23:53.000000 describr-0.0.1/describr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 16:23:53.506439 describr-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1577 2023-06-20 16:23:46.000000 describr-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:47:25.585224 describr-0.0.2/
+-rw-rw-rw-   0        0        0     1099 2023-06-20 15:03:20.000000 describr-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4995 2023-06-20 16:47:25.585224 describr-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3740 2023-06-20 15:28:09.000000 describr-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 16:47:25.568150 describr-0.0.2/describr/
+-rw-rw-rw-   0        0        0      129 2023-06-20 16:29:45.000000 describr-0.0.2/describr/__init__.py
+-rw-rw-rw-   0        0        0    16616 2023-06-20 14:40:14.000000 describr-0.0.2/describr/describr.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:47:25.583223 describr-0.0.2/describr.egg-info/
+-rw-rw-rw-   0        0        0     4995 2023-06-20 16:47:25.000000 describr-0.0.2/describr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-20 16:47:25.000000 describr-0.0.2/describr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 16:47:25.000000 describr-0.0.2/describr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-20 16:47:25.000000 describr-0.0.2/describr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 16:47:25.000000 describr-0.0.2/describr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 16:47:25.585224 describr-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1613 2023-06-20 16:47:09.000000 describr-0.0.2/setup.py
```

### Comparing `describr-0.0.1/LICENSE` & `describr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `describr-0.0.1/README.md` & `describr-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `describr-0.0.1/describr/describr.py` & `describr-0.0.2/describr/describr.py`

 * *Files identical despite different names*

### Comparing `describr-0.0.1/setup.py` & `describr-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import setuptools
 from setuptools import setup, find_packages
 import os
-import requests
 
-response = requests.get("https://github.com/famutimine/describr/blob/main/README.md")
-long_description = response.text
+from urllib.request import urlopen
+
+with urlopen("https://raw.githubusercontent.com/famutimine/describr/main/README.md") as fh:
+    long_description = fh.read().decode()
 
 setuptools.setup(
     name='describr',
-    version='0.0.1',
+    version='0.0.2',
     description='Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/famutimine/describr',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
```

