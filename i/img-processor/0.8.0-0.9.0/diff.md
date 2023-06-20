# Comparing `tmp/img_processor-0.8.0.tar.gz` & `tmp/img_processor-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img_processor-0.8.0.tar", last modified: Fri Jan 29 22:29:02 2021, max compression
+gzip compressed data, was "img_processor-0.9.0.tar", last modified: Mon Feb  8 21:31:55 2021, max compression
```

## Comparing `img_processor-0.8.0.tar` & `img_processor-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-01-29 22:29:02.403211 img_processor-0.8.0/
--rw-r--r--   0 justin    (1000) justin    (1000)      166 2020-09-22 15:15:55.000000 img_processor-0.8.0/AUTHORS.rst
--rw-r--r--   0 justin    (1000) justin    (1000)     3592 2020-09-22 15:15:55.000000 img_processor-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 justin    (1000) justin    (1000)      398 2021-01-29 22:24:02.000000 img_processor-0.8.0/HISTORY.rst
--rw-r--r--   0 justin    (1000) justin    (1000)     1072 2020-09-22 15:15:55.000000 img_processor-0.8.0/LICENSE
--rw-r--r--   0 justin    (1000) justin    (1000)      262 2020-09-22 15:15:55.000000 img_processor-0.8.0/MANIFEST.in
--rw-r--r--   0 justin    (1000) justin    (1000)     2667 2021-01-29 22:29:02.403211 img_processor-0.8.0/PKG-INFO
--rw-r--r--   0 justin    (1000) justin    (1000)      936 2020-09-22 15:15:55.000000 img_processor-0.8.0/README.rst
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-01-29 22:29:02.403211 img_processor-0.8.0/docs/
--rw-r--r--   0 justin    (1000) justin    (1000)      614 2020-09-22 15:15:55.000000 img_processor-0.8.0/docs/Makefile
--rw-r--r--   0 justin    (1000) justin    (1000)       28 2020-09-22 15:15:55.000000 img_processor-0.8.0/docs/authors.rst
--rwxr-xr-x   0 justin    (1000) justin    (1000)     4913 2020-09-22 20:19:51.000000 img_processor-0.8.0/docs/conf.py
--rw-r--r--   0 justin    (1000) justin    (1000)       33 2020-09-22 15:15:55.000000 img_processor-0.8.0/docs/contributing.rst
--rw-r--r--   0 justin    (1000) justin    (1000)       28 2020-09-22 15:15:55.000000 img_processor-0.8.0/docs/history.rst
--rw-r--r--   0 justin    (1000) justin    (1000)      310 2020-09-22 15:15:55.000000 img_processor-0.8.0/docs/index.rst
--rw-r--r--   0 justin    (1000) justin    (1000)     1178 2020-09-22 15:15:55.000000 img_processor-0.8.0/docs/installation.rst
--rw-r--r--   0 justin    (1000) justin    (1000)      775 2020-09-22 15:15:55.000000 img_processor-0.8.0/docs/make.bat
--rw-r--r--   0 justin    (1000) justin    (1000)       27 2020-09-22 15:15:55.000000 img_processor-0.8.0/docs/readme.rst
--rw-r--r--   0 justin    (1000) justin    (1000)       81 2020-09-22 15:15:55.000000 img_processor-0.8.0/docs/usage.rst
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-01-29 22:29:02.403211 img_processor-0.8.0/img_processor/
--rw-r--r--   0 justin    (1000) justin    (1000)      209 2021-01-29 22:24:18.000000 img_processor-0.8.0/img_processor/__init__.py
--rw-r--r--   0 justin    (1000) justin    (1000)      363 2020-09-28 16:50:53.000000 img_processor-0.8.0/img_processor/cli.py
--rw-r--r--   0 justin    (1000) justin    (1000)     6104 2021-01-29 20:38:23.000000 img_processor-0.8.0/img_processor/img_processor.py
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-01-29 22:29:02.403211 img_processor-0.8.0/img_processor.egg-info/
--rw-r--r--   0 justin    (1000) justin    (1000)     2667 2021-01-29 22:29:02.000000 img_processor-0.8.0/img_processor.egg-info/PKG-INFO
--rw-r--r--   0 justin    (1000) justin    (1000)      639 2021-01-29 22:29:02.000000 img_processor-0.8.0/img_processor.egg-info/SOURCES.txt
--rw-r--r--   0 justin    (1000) justin    (1000)        1 2021-01-29 22:29:02.000000 img_processor-0.8.0/img_processor.egg-info/dependency_links.txt
--rw-r--r--   0 justin    (1000) justin    (1000)       58 2021-01-29 22:29:02.000000 img_processor-0.8.0/img_processor.egg-info/entry_points.txt
--rw-r--r--   0 justin    (1000) justin    (1000)        1 2020-09-22 20:41:11.000000 img_processor-0.8.0/img_processor.egg-info/not-zip-safe
--rw-r--r--   0 justin    (1000) justin    (1000)       40 2021-01-29 22:29:02.000000 img_processor-0.8.0/img_processor.egg-info/requires.txt
--rw-r--r--   0 justin    (1000) justin    (1000)       14 2021-01-29 22:29:02.000000 img_processor-0.8.0/img_processor.egg-info/top_level.txt
--rw-r--r--   0 justin    (1000) justin    (1000)      455 2021-01-29 22:29:02.403211 img_processor-0.8.0/setup.cfg
--rw-r--r--   0 justin    (1000) justin    (1000)     1604 2021-01-29 22:28:59.000000 img_processor-0.8.0/setup.py
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-01-29 22:29:02.403211 img_processor-0.8.0/tests/
--rw-r--r--   0 justin    (1000) justin    (1000)       43 2020-09-22 15:15:55.000000 img_processor-0.8.0/tests/__init__.py
--rw-r--r--   0 justin    (1000) justin    (1000)     1011 2020-09-22 20:19:51.000000 img_processor-0.8.0/tests/test_img_processor.py
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-02-08 21:31:55.704553 img_processor-0.9.0/
+-rw-r--r--   0 justin    (1000) justin    (1000)      166 2020-09-22 15:15:55.000000 img_processor-0.9.0/AUTHORS.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)     3592 2020-09-22 15:15:55.000000 img_processor-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)      398 2021-01-29 22:24:02.000000 img_processor-0.9.0/HISTORY.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)     1072 2020-09-22 15:15:55.000000 img_processor-0.9.0/LICENSE
+-rw-r--r--   0 justin    (1000) justin    (1000)      262 2020-09-22 15:15:55.000000 img_processor-0.9.0/MANIFEST.in
+-rw-r--r--   0 justin    (1000) justin    (1000)     2667 2021-02-08 21:31:55.704553 img_processor-0.9.0/PKG-INFO
+-rw-r--r--   0 justin    (1000) justin    (1000)      936 2020-09-22 15:15:55.000000 img_processor-0.9.0/README.rst
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-02-08 21:31:55.704553 img_processor-0.9.0/docs/
+-rw-r--r--   0 justin    (1000) justin    (1000)      614 2020-09-22 15:15:55.000000 img_processor-0.9.0/docs/Makefile
+-rw-r--r--   0 justin    (1000) justin    (1000)       28 2020-09-22 15:15:55.000000 img_processor-0.9.0/docs/authors.rst
+-rwxr-xr-x   0 justin    (1000) justin    (1000)     4913 2020-09-22 20:19:51.000000 img_processor-0.9.0/docs/conf.py
+-rw-r--r--   0 justin    (1000) justin    (1000)       33 2020-09-22 15:15:55.000000 img_processor-0.9.0/docs/contributing.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)       28 2020-09-22 15:15:55.000000 img_processor-0.9.0/docs/history.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)      310 2020-09-22 15:15:55.000000 img_processor-0.9.0/docs/index.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)     1178 2020-09-22 15:15:55.000000 img_processor-0.9.0/docs/installation.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)      775 2020-09-22 15:15:55.000000 img_processor-0.9.0/docs/make.bat
+-rw-r--r--   0 justin    (1000) justin    (1000)       27 2020-09-22 15:15:55.000000 img_processor-0.9.0/docs/readme.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)       81 2020-09-22 15:15:55.000000 img_processor-0.9.0/docs/usage.rst
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-02-08 21:31:55.704553 img_processor-0.9.0/img_processor/
+-rw-r--r--   0 justin    (1000) justin    (1000)      193 2021-02-08 21:30:00.000000 img_processor-0.9.0/img_processor/__init__.py
+-rw-r--r--   0 justin    (1000) justin    (1000)      363 2020-09-28 16:50:53.000000 img_processor-0.9.0/img_processor/cli.py
+-rw-r--r--   0 justin    (1000) justin    (1000)     8260 2021-02-08 19:50:21.000000 img_processor-0.9.0/img_processor/img_processor.py
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-02-08 21:31:55.704553 img_processor-0.9.0/img_processor.egg-info/
+-rw-r--r--   0 justin    (1000) justin    (1000)     2667 2021-02-08 21:31:55.000000 img_processor-0.9.0/img_processor.egg-info/PKG-INFO
+-rw-r--r--   0 justin    (1000) justin    (1000)      639 2021-02-08 21:31:55.000000 img_processor-0.9.0/img_processor.egg-info/SOURCES.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)        1 2021-02-08 21:31:55.000000 img_processor-0.9.0/img_processor.egg-info/dependency_links.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)       58 2021-02-08 21:31:55.000000 img_processor-0.9.0/img_processor.egg-info/entry_points.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)        1 2020-09-22 20:41:11.000000 img_processor-0.9.0/img_processor.egg-info/not-zip-safe
+-rw-r--r--   0 justin    (1000) justin    (1000)       68 2021-02-08 21:31:55.000000 img_processor-0.9.0/img_processor.egg-info/requires.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)       14 2021-02-08 21:31:55.000000 img_processor-0.9.0/img_processor.egg-info/top_level.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)      439 2021-02-08 21:31:55.704553 img_processor-0.9.0/setup.cfg
+-rw-r--r--   0 justin    (1000) justin    (1000)     1689 2021-02-08 21:30:00.000000 img_processor-0.9.0/setup.py
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-02-08 21:31:55.704553 img_processor-0.9.0/tests/
+-rw-r--r--   0 justin    (1000) justin    (1000)       43 2020-09-22 15:15:55.000000 img_processor-0.9.0/tests/__init__.py
+-rw-r--r--   0 justin    (1000) justin    (1000)     1011 2020-09-22 20:19:51.000000 img_processor-0.9.0/tests/test_img_processor.py
```

### Comparing `img_processor-0.8.0/CONTRIBUTING.rst` & `img_processor-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `img_processor-0.8.0/LICENSE` & `img_processor-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `img_processor-0.8.0/PKG-INFO` & `img_processor-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: img_processor
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python package for taking an image and doing a thing
 Home-page: https://github.com/kellerjustin/img_processor
 Author: Justin Keller
 Author-email: kellerjustin@protonmail.com
 License: MIT license
 Description: =============
         img_processor
```

### Comparing `img_processor-0.8.0/README.rst` & `img_processor-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `img_processor-0.8.0/docs/Makefile` & `img_processor-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `img_processor-0.8.0/docs/conf.py` & `img_processor-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `img_processor-0.8.0/docs/installation.rst` & `img_processor-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `img_processor-0.8.0/docs/make.bat` & `img_processor-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `img_processor-0.8.0/img_processor.egg-info/PKG-INFO` & `img_processor-0.9.0/img_processor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: img-processor
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python package for taking an image and doing a thing
 Home-page: https://github.com/kellerjustin/img_processor
 Author: Justin Keller
 Author-email: kellerjustin@protonmail.com
 License: MIT license
 Description: =============
         img_processor
```

### Comparing `img_processor-0.8.0/img_processor.egg-info/SOURCES.txt` & `img_processor-0.9.0/img_processor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `img_processor-0.8.0/setup.py` & `img_processor-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
 requirements = [
+    "numpy",
     "Click>=7.0",
     "pytesseract",
     "pdf2image",
     "PyPDF2",
+    "libtiff",
+    "opencv-python",
 ]
 
 setup_requirements = [
     "pytest-runner",
 ]
 
 test_requirements = [
@@ -37,22 +40,26 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
     description="Python package for taking an image and doing a thing",
-    entry_points={"console_scripts": ["img_processor=img_processor.cli:main",],},
+    entry_points={
+        "console_scripts": [
+            "img_processor=img_processor.cli:main",
+        ],
+    },
     install_requires=requirements,
     license="MIT license",
     long_description=readme + "\n\n" + history,
     include_package_data=True,
     keywords="img_processor",
     name="img_processor",
     packages=find_packages(include=["img_processor", "img_processor.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/kellerjustin/img_processor",
-    version="0.8.0",
+    version="0.9.0",
     zip_safe=False,
 )
```

### Comparing `img_processor-0.8.0/tests/test_img_processor.py` & `img_processor-0.9.0/tests/test_img_processor.py`

 * *Files identical despite different names*

