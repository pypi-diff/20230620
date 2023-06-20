# Comparing `tmp/mogutda-0.3.4.tar.gz` & `tmp/mogutda-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mogutda-0.3.4.tar", last modified: Sat Sep 10 01:18:46 2022, max compression
+gzip compressed data, was "dist/mogutda-0.3.5.tar", last modified: Tue Jun 20 16:05:34 2023, max compression
```

## Comparing `mogutda-0.3.4.tar` & `mogutda-0.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-10 01:18:46.304768 mogutda-0.3.4/
--rw-r--r--   0 stephenhky   (501) staff       (20)     1055 2020-08-15 03:48:18.000000 mogutda-0.3.4/LICENSE
--rw-r--r--   0 stephenhky   (501) staff       (20)       59 2020-10-02 20:25:37.000000 mogutda-0.3.4/MANIFEST.in
--rw-r--r--   0 stephenhky   (501) staff       (20)     8814 2022-09-10 01:18:46.304486 mogutda-0.3.4/PKG-INFO
--rw-r--r--   0 stephenhky   (501) staff       (20)     7886 2022-09-10 01:18:09.000000 mogutda-0.3.4/README.md
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-10 01:18:46.299813 mogutda-0.3.4/mogutda/
--rw-r--r--   0 stephenhky   (501) staff       (20)      149 2021-04-10 21:46:39.000000 mogutda-0.3.4/mogutda/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     4857 2021-04-10 21:46:39.000000 mogutda-0.3.4/mogutda/abssimcomplex.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     2293 2021-04-10 21:46:39.000000 mogutda-0.3.4/mogutda/alphacomplex.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      606 2021-04-10 21:46:39.000000 mogutda-0.3.4/mogutda/utils.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1219 2021-04-10 21:46:39.000000 mogutda-0.3.4/mogutda/vrcomplex.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-10 01:18:46.302679 mogutda-0.3.4/mogutda.egg-info/
--rw-r--r--   0 stephenhky   (501) staff       (20)     8814 2022-09-10 01:18:46.000000 mogutda-0.3.4/mogutda.egg-info/PKG-INFO
--rw-r--r--   0 stephenhky   (501) staff       (20)      370 2022-09-10 01:18:46.000000 mogutda-0.3.4/mogutda.egg-info/SOURCES.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2022-09-10 01:18:46.000000 mogutda-0.3.4/mogutda.egg-info/dependency_links.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2020-08-16 15:28:14.000000 mogutda-0.3.4/mogutda.egg-info/not-zip-safe
--rw-r--r--   0 stephenhky   (501) staff       (20)       59 2022-09-10 01:18:46.000000 mogutda-0.3.4/mogutda.egg-info/requires.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        8 2022-09-10 01:18:46.000000 mogutda-0.3.4/mogutda.egg-info/top_level.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       59 2020-08-16 15:21:12.000000 mogutda-0.3.4/requirements.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       38 2022-09-10 01:18:46.304931 mogutda-0.3.4/setup.cfg
--rw-r--r--   0 stephenhky   (501) staff       (20)     1648 2022-09-10 01:18:09.000000 mogutda-0.3.4/setup.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-10 01:18:46.303104 mogutda-0.3.4/test/
--rw-r--r--   0 stephenhky   (501) staff       (20)     3529 2020-08-16 15:21:12.000000 mogutda-0.3.4/test/test_simcomplex.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 16:05:34.924451 mogutda-0.3.5/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1055 2020-08-15 03:48:18.000000 mogutda-0.3.5/LICENSE
+-rw-r--r--   0 stephenhky   (501) staff       (20)       59 2020-10-02 20:25:37.000000 mogutda-0.3.5/MANIFEST.in
+-rw-r--r--   0 stephenhky   (501) staff       (20)     8913 2023-06-20 16:05:34.923947 mogutda-0.3.5/PKG-INFO
+-rw-r--r--   0 stephenhky   (501) staff       (20)     7926 2023-06-20 16:04:14.000000 mogutda-0.3.5/README.md
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 16:05:34.917443 mogutda-0.3.5/mogutda/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      149 2021-04-10 21:46:39.000000 mogutda-0.3.5/mogutda/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4857 2021-04-10 21:46:39.000000 mogutda-0.3.5/mogutda/abssimcomplex.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2293 2021-04-10 21:46:39.000000 mogutda-0.3.5/mogutda/alphacomplex.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      606 2021-04-10 21:46:39.000000 mogutda-0.3.5/mogutda/utils.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1219 2021-04-10 21:46:39.000000 mogutda-0.3.5/mogutda/vrcomplex.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 16:05:34.922151 mogutda-0.3.5/mogutda.egg-info/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     8913 2023-06-20 16:05:34.000000 mogutda-0.3.5/mogutda.egg-info/PKG-INFO
+-rw-r--r--   0 stephenhky   (501) staff       (20)      370 2023-06-20 16:05:34.000000 mogutda-0.3.5/mogutda.egg-info/SOURCES.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2023-06-20 16:05:34.000000 mogutda-0.3.5/mogutda.egg-info/dependency_links.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2020-08-16 15:28:14.000000 mogutda-0.3.5/mogutda.egg-info/not-zip-safe
+-rw-r--r--   0 stephenhky   (501) staff       (20)       59 2023-06-20 16:05:34.000000 mogutda-0.3.5/mogutda.egg-info/requires.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        8 2023-06-20 16:05:34.000000 mogutda-0.3.5/mogutda.egg-info/top_level.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       59 2020-08-16 15:21:12.000000 mogutda-0.3.5/requirements.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       38 2023-06-20 16:05:34.924642 mogutda-0.3.5/setup.cfg
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1700 2023-06-20 16:04:14.000000 mogutda-0.3.5/setup.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 16:05:34.922704 mogutda-0.3.5/test/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3529 2020-08-16 15:21:12.000000 mogutda-0.3.5/test/test_simcomplex.py
```

### Comparing `mogutda-0.3.4/LICENSE` & `mogutda-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mogutda-0.3.4/PKG-INFO` & `mogutda-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mogutda
-Version: 0.3.4
+Version: 0.3.5
 Summary: Topological Data Analysis in Python
 Home-page: https://github.com/stephenhky/MoguTDA
 Author: Kwan-Yuet Ho
 Author-email: stephenhky@yahoo.com.hk
 License: MIT
 Description: ## Introduction
         
@@ -85,14 +85,15 @@
         Richard Hennigan put a nice Wolfram Demonstration online explaining what
         the simplicial complexes are, and how homologies are defined:
         
         * [Simplicial Homology of the Alpha Complex](http://demonstrations.wolfram.com/SimplicialHomologyOfTheAlphaComplex/)
         
         ## News
         
+        * 06/20/2023: `mogutda` 0.3.5 released.
         * 09/09/2022: `mogutda` 0.3.4 released.
         * 07/15/2021: `mogutda` 0.3.3 released.
         * 04/10/2021: `mogutda` 0.3.2 released.
         * 11/28/2020: `mogutda` 0.3.1 released.
         * 08/16/2020: `mogutda` 0.3.0 released.
         * 04/28/2020: `mogutda` 0.2.1 released.
         * 01/16/2020: `mogutda` 0.2.0 released.
@@ -148,13 +149,14 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
```

### Comparing `mogutda-0.3.4/README.md` & `mogutda-0.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 Richard Hennigan put a nice Wolfram Demonstration online explaining what
 the simplicial complexes are, and how homologies are defined:
 
 * [Simplicial Homology of the Alpha Complex](http://demonstrations.wolfram.com/SimplicialHomologyOfTheAlphaComplex/)
 
 ## News
 
+* 06/20/2023: `mogutda` 0.3.5 released.
 * 09/09/2022: `mogutda` 0.3.4 released.
 * 07/15/2021: `mogutda` 0.3.3 released.
 * 04/10/2021: `mogutda` 0.3.2 released.
 * 11/28/2020: `mogutda` 0.3.1 released.
 * 08/16/2020: `mogutda` 0.3.0 released.
 * 04/28/2020: `mogutda` 0.2.1 released.
 * 01/16/2020: `mogutda` 0.2.0 released.
```

### Comparing `mogutda-0.3.4/mogutda/abssimcomplex.py` & `mogutda-0.3.5/mogutda/abssimcomplex.py`

 * *Files identical despite different names*

### Comparing `mogutda-0.3.4/mogutda/alphacomplex.py` & `mogutda-0.3.5/mogutda/alphacomplex.py`

 * *Files identical despite different names*

### Comparing `mogutda-0.3.4/mogutda/utils.py` & `mogutda-0.3.5/mogutda/utils.py`

 * *Files identical despite different names*

### Comparing `mogutda-0.3.4/mogutda/vrcomplex.py` & `mogutda-0.3.5/mogutda/vrcomplex.py`

 * *Files identical despite different names*

### Comparing `mogutda-0.3.4/mogutda.egg-info/PKG-INFO` & `mogutda-0.3.5/mogutda.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mogutda
-Version: 0.3.4
+Version: 0.3.5
 Summary: Topological Data Analysis in Python
 Home-page: https://github.com/stephenhky/MoguTDA
 Author: Kwan-Yuet Ho
 Author-email: stephenhky@yahoo.com.hk
 License: MIT
 Description: ## Introduction
         
@@ -85,14 +85,15 @@
         Richard Hennigan put a nice Wolfram Demonstration online explaining what
         the simplicial complexes are, and how homologies are defined:
         
         * [Simplicial Homology of the Alpha Complex](http://demonstrations.wolfram.com/SimplicialHomologyOfTheAlphaComplex/)
         
         ## News
         
+        * 06/20/2023: `mogutda` 0.3.5 released.
         * 09/09/2022: `mogutda` 0.3.4 released.
         * 07/15/2021: `mogutda` 0.3.3 released.
         * 04/10/2021: `mogutda` 0.3.2 released.
         * 11/28/2020: `mogutda` 0.3.1 released.
         * 08/16/2020: `mogutda` 0.3.0 released.
         * 04/28/2020: `mogutda` 0.2.1 released.
         * 01/16/2020: `mogutda` 0.2.0 released.
@@ -148,13 +149,14 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
```

### Comparing `mogutda-0.3.4/setup.py` & `mogutda-0.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,26 +17,27 @@
     return [
         package_string.strip()
         for package_string in open('requirements.txt', 'r', encoding="utf-8")
     ]
 
 
 setup(name='mogutda',
-      version="0.3.4",
+      version="0.3.5",
       description="Topological Data Analysis in Python",
       long_description=package_description(),
       long_description_content_type='text/markdown',
       classifiers=[
           "Topic :: Scientific/Engineering :: Mathematics",
           "Topic :: Scientific/Engineering :: Physics",
           "Programming Language :: Python :: 3.6",
           "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
+          "Programming Language :: Python :: 3.11",
           "License :: OSI Approved :: MIT License",
           "Intended Audience :: Developers",
           "Intended Audience :: Education",
           "Intended Audience :: Information Technology",
           "Intended Audience :: Science/Research"
       ],
       keywords="mogutda numerics topology data",
```

### Comparing `mogutda-0.3.4/test/test_simcomplex.py` & `mogutda-0.3.5/test/test_simcomplex.py`

 * *Files identical despite different names*

