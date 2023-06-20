# Comparing `tmp/social-blade-scraper-0.0.3.tar.gz` & `tmp/social-blade-scraper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social-blade-scraper-0.0.3.tar", last modified: Tue Jun 20 08:42:27 2023, max compression
+gzip compressed data, was "social-blade-scraper-0.0.4.tar", last modified: Tue Jun 20 09:03:39 2023, max compression
```

## Comparing `social-blade-scraper-0.0.3.tar` & `social-blade-scraper-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 08:42:27.462986 social-blade-scraper-0.0.3/
--rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-20 08:42:27.458986 social-blade-scraper-0.0.3/PKG-INFO
--rw-rw-r--   0 tej       (1000) tej       (1000)       23 2023-06-20 07:41:43.000000 social-blade-scraper-0.0.3/README.md
--rw-rw-r--   0 tej       (1000) tej       (1000)       38 2023-06-20 08:42:27.462986 social-blade-scraper-0.0.3/setup.cfg
--rw-rw-r--   0 tej       (1000) tej       (1000)      787 2023-06-20 08:41:33.000000 social-blade-scraper-0.0.3/setup.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 08:42:27.450986 social-blade-scraper-0.0.3/src/
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 08:42:27.454986 social-blade-scraper-0.0.3/src/social_blade_scraper/
--rw-rw-r--   0 tej       (1000) tej       (1000)       20 2023-06-20 08:41:12.000000 social-blade-scraper-0.0.3/src/social_blade_scraper/__init__.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 08:42:27.458986 social-blade-scraper-0.0.3/src/social_blade_scraper.egg-info/
--rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-20 08:42:27.000000 social-blade-scraper-0.0.3/src/social_blade_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 tej       (1000) tej       (1000)      316 2023-06-20 08:42:27.000000 social-blade-scraper-0.0.3/src/social_blade_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)        1 2023-06-20 08:42:27.000000 social-blade-scraper-0.0.3/src/social_blade_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)       39 2023-06-20 08:42:27.000000 social-blade-scraper-0.0.3/src/social_blade_scraper.egg-info/requires.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)       21 2023-06-20 08:42:27.000000 social-blade-scraper-0.0.3/src/social_blade_scraper.egg-info/top_level.txt
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 08:42:27.458986 social-blade-scraper-0.0.3/tests/
--rw-rw-r--   0 tej       (1000) tej       (1000)      205 2023-06-20 08:29:08.000000 social-blade-scraper-0.0.3/tests/test_youtube.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 09:03:39.774721 social-blade-scraper-0.0.4/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-20 09:03:39.774721 social-blade-scraper-0.0.4/PKG-INFO
+-rw-rw-r--   0 tej       (1000) tej       (1000)       23 2023-06-20 07:41:43.000000 social-blade-scraper-0.0.4/README.md
+-rw-rw-r--   0 tej       (1000) tej       (1000)       38 2023-06-20 09:03:39.774721 social-blade-scraper-0.0.4/setup.cfg
+-rw-rw-r--   0 tej       (1000) tej       (1000)      720 2023-06-20 09:00:58.000000 social-blade-scraper-0.0.4/setup.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 09:03:39.762722 social-blade-scraper-0.0.4/src/
+-rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 05:17:33.000000 social-blade-scraper-0.0.4/src/__init__.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 09:03:39.762722 social-blade-scraper-0.0.4/src/social_blade_scraper/
+-rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 08:55:41.000000 social-blade-scraper-0.0.4/src/social_blade_scraper/__init__.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 09:03:39.770721 social-blade-scraper-0.0.4/src/social_blade_scraper/stats/
+-rw-rw-r--   0 tej       (1000) tej       (1000)     6943 2023-06-20 02:29:40.000000 social-blade-scraper-0.0.4/src/social_blade_scraper/stats/youtube.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 09:03:39.770721 social-blade-scraper-0.0.4/src/social_blade_scraper.egg-info/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-20 09:03:39.000000 social-blade-scraper-0.0.4/src/social_blade_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 tej       (1000) tej       (1000)      374 2023-06-20 09:03:39.000000 social-blade-scraper-0.0.4/src/social_blade_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)        1 2023-06-20 09:03:39.000000 social-blade-scraper-0.0.4/src/social_blade_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)       39 2023-06-20 09:03:39.000000 social-blade-scraper-0.0.4/src/social_blade_scraper.egg-info/requires.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)       30 2023-06-20 09:03:39.000000 social-blade-scraper-0.0.4/src/social_blade_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-20 09:03:39.770721 social-blade-scraper-0.0.4/tests/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      205 2023-06-20 08:29:08.000000 social-blade-scraper-0.0.4/tests/test_youtube.py
```

### Comparing `social-blade-scraper-0.0.3/setup.py` & `social-blade-scraper-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,29 +2,26 @@
 from setuptools import setup
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="social-blade-scraper",
-    version="0.0.3",
+    version="0.0.4",
     description="Social blade scraper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/tejmagar/social-blade-scraper",
     install_requires=[
         "beautifulsoup4",
         "requests",
         "fake-useragent"
     ],
-    package_dir={"": "src"},
-    packages=setuptools.find_packages(
-        where='src',
-    ),
+    package_dir={'': 'src'},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
```

