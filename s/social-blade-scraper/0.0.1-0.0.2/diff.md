# Comparing `tmp/social-blade-scraper-0.0.1.tar.gz` & `tmp/social-blade-scraper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social-blade-scraper-0.0.1.tar", last modified: Tue Jun 20 07:35:13 2023, max compression
+gzip compressed data, was "social-blade-scraper-0.0.2.tar", last modified: Tue Jun 20 08:30:09 2023, max compression
```

## Comparing `social-blade-scraper-0.0.1.tar` & `social-blade-scraper-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 07:35:13.665252 social-blade-scraper-0.0.1/
--rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-20 07:35:13.661251 social-blade-scraper-0.0.1/PKG-INFO
--rw-rw-r--   0 tej       (1000) tej       (1000)       22 2023-06-20 05:12:10.000000 social-blade-scraper-0.0.1/README.md
--rw-rw-r--   0 tej       (1000) tej       (1000)       38 2023-06-20 07:35:13.665252 social-blade-scraper-0.0.1/setup.cfg
--rw-rw-r--   0 tej       (1000) tej       (1000)      787 2023-06-20 07:35:04.000000 social-blade-scraper-0.0.1/setup.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 07:35:13.661251 social-blade-scraper-0.0.1/src/
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 07:35:13.661251 social-blade-scraper-0.0.1/src/social_blade_scraper.egg-info/
--rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-20 07:35:13.000000 social-blade-scraper-0.0.1/src/social_blade_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 tej       (1000) tej       (1000)      315 2023-06-20 07:35:13.000000 social-blade-scraper-0.0.1/src/social_blade_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)        1 2023-06-20 07:35:13.000000 social-blade-scraper-0.0.1/src/social_blade_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)       39 2023-06-20 07:35:13.000000 social-blade-scraper-0.0.1/src/social_blade_scraper.egg-info/requires.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)       20 2023-06-20 07:35:13.000000 social-blade-scraper-0.0.1/src/social_blade_scraper.egg-info/top_level.txt
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 07:35:13.661251 social-blade-scraper-0.0.1/src/socialblade_scraper/
--rw-rw-r--   0 tej       (1000) tej       (1000)       35 2023-06-20 06:23:35.000000 social-blade-scraper-0.0.1/src/socialblade_scraper/__init__.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 07:35:13.661251 social-blade-scraper-0.0.1/tests/
--rw-rw-r--   0 tej       (1000) tej       (1000)      133 2023-06-20 05:06:21.000000 social-blade-scraper-0.0.1/tests/test_youtube.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 08:30:09.452353 social-blade-scraper-0.0.2/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-20 08:30:09.452353 social-blade-scraper-0.0.2/PKG-INFO
+-rw-rw-r--   0 tej       (1000) tej       (1000)       23 2023-06-20 07:41:43.000000 social-blade-scraper-0.0.2/README.md
+-rw-rw-r--   0 tej       (1000) tej       (1000)       38 2023-06-20 08:30:09.452353 social-blade-scraper-0.0.2/setup.cfg
+-rw-rw-r--   0 tej       (1000) tej       (1000)      787 2023-06-20 08:24:44.000000 social-blade-scraper-0.0.2/setup.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 08:30:09.452353 social-blade-scraper-0.0.2/src/
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 08:30:09.452353 social-blade-scraper-0.0.2/src/social_blade_scraper/
+-rw-rw-r--   0 tej       (1000) tej       (1000)       16 2023-06-20 08:24:12.000000 social-blade-scraper-0.0.2/src/social_blade_scraper/__init__.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 08:30:09.452353 social-blade-scraper-0.0.2/src/social_blade_scraper.egg-info/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-20 08:30:09.000000 social-blade-scraper-0.0.2/src/social_blade_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 tej       (1000) tej       (1000)      316 2023-06-20 08:30:09.000000 social-blade-scraper-0.0.2/src/social_blade_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)        1 2023-06-20 08:30:09.000000 social-blade-scraper-0.0.2/src/social_blade_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)       39 2023-06-20 08:30:09.000000 social-blade-scraper-0.0.2/src/social_blade_scraper.egg-info/requires.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)       21 2023-06-20 08:30:09.000000 social-blade-scraper-0.0.2/src/social_blade_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 08:30:09.452353 social-blade-scraper-0.0.2/tests/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      205 2023-06-20 08:29:08.000000 social-blade-scraper-0.0.2/tests/test_youtube.py
```

### Comparing `social-blade-scraper-0.0.1/setup.py` & `social-blade-scraper-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="social-blade-scraper",
-    version="0.0.1",
+    version="0.0.2",
     description="Social blade scraper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/tejmagar/social-blade-scraper",
     install_requires=[
         "beautifulsoup4",
```

