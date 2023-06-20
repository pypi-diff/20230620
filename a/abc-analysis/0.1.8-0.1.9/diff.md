# Comparing `tmp/abc_analysis-0.1.8.tar.gz` & `tmp/abc_analysis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\abc_analysis-0.1.8.tar", last modified: Fri Mar  8 09:13:17 2019, max compression
+gzip compressed data, was "dist\abc_analysis-0.1.9.tar", last modified: Mon Mar 11 09:09:56 2019, max compression
```

## Comparing `abc_analysis-0.1.8.tar` & `abc_analysis-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2019-03-08 09:13:17.000000 abc_analysis-0.1.8/
-drwxrwxrwx   0        0        0        0 2019-03-08 09:13:17.000000 abc_analysis-0.1.8/abc_analysis/
--rw-rw-rw-   0        0        0    12195 2019-03-06 13:52:17.000000 abc_analysis-0.1.8/abc_analysis/abc_analysis.py
--rw-rw-rw-   0        0        0       73 2019-03-08 09:03:59.000000 abc_analysis-0.1.8/abc_analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2019-03-08 09:13:17.000000 abc_analysis-0.1.8/abc_analysis.egg-info/
--rw-rw-rw-   0        0        0        1 2019-03-08 09:13:16.000000 abc_analysis-0.1.8/abc_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-03-08 07:36:49.000000 abc_analysis-0.1.8/abc_analysis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      871 2019-03-08 09:13:16.000000 abc_analysis-0.1.8/abc_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       56 2019-03-08 09:13:16.000000 abc_analysis-0.1.8/abc_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      286 2019-03-08 09:13:16.000000 abc_analysis-0.1.8/abc_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       13 2019-03-08 09:13:16.000000 abc_analysis-0.1.8/abc_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      871 2019-03-08 09:13:17.000000 abc_analysis-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1106 2019-03-06 14:47:49.000000 abc_analysis-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2019-03-08 09:13:17.000000 abc_analysis-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1181 2019-03-08 09:03:49.000000 abc_analysis-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2019-03-11 09:09:56.000000 abc_analysis-0.1.9/
+drwxrwxrwx   0        0        0        0 2019-03-11 09:09:56.000000 abc_analysis-0.1.9/abc_analysis/
+-rw-rw-rw-   0        0        0    12195 2019-03-06 13:52:17.000000 abc_analysis-0.1.9/abc_analysis/abc_analysis.py
+-rw-rw-rw-   0        0        0       73 2019-03-11 09:09:42.000000 abc_analysis-0.1.9/abc_analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2019-03-11 09:09:56.000000 abc_analysis-0.1.9/abc_analysis.egg-info/
+-rw-rw-rw-   0        0        0        1 2019-03-11 09:09:56.000000 abc_analysis-0.1.9/abc_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-03-08 07:36:49.000000 abc_analysis-0.1.9/abc_analysis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      950 2019-03-11 09:09:56.000000 abc_analysis-0.1.9/abc_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2019-03-11 09:09:56.000000 abc_analysis-0.1.9/abc_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      286 2019-03-11 09:09:56.000000 abc_analysis-0.1.9/abc_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       13 2019-03-11 09:09:56.000000 abc_analysis-0.1.9/abc_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      950 2019-03-11 09:09:56.000000 abc_analysis-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1106 2019-03-06 14:47:49.000000 abc_analysis-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2019-03-11 09:09:56.000000 abc_analysis-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1273 2019-03-11 09:09:20.000000 abc_analysis-0.1.9/setup.py
```

### Comparing `abc_analysis-0.1.8/abc_analysis/abc_analysis.py` & `abc_analysis-0.1.9/abc_analysis/abc_analysis.py`

 * *Files identical despite different names*

### Comparing `abc_analysis-0.1.8/abc_analysis.egg-info/PKG-INFO` & `abc_analysis-0.1.9/abc_analysis.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 1.1
 Name: abc-analysis
-Version: 0.1.8
+Version: 0.1.9
 Summary: ABC analysis with automated limit detection
 Home-page: https://github.com/viessmann/abc_analysis
 Author: Tino Gehlert
 Author-email: ghlt@viessmann.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/viessmann/abc_analysis/archive/v0.1.8.tar.gz
+Download-URL: https://github.com/viessmann/abc_analysis/archive/v0.1.9.tar.gz
+Project-URL: Viessmann, https://www.linkedin.com/company/viessmann/
 Description: 
         Performs and visualizes an ABC analysis with automated limit detection.
         
         This package is a Python implementation of the R package `ABCanalysis <https://CRAN.R-project.org/package=ABCanalysis>`__
         
-Keywords: abc-analysis abc_analysis
+Keywords: abc-analysis abc_analysis Viessmann
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `abc_analysis-0.1.8/PKG-INFO` & `abc_analysis-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 1.1
 Name: abc_analysis
-Version: 0.1.8
+Version: 0.1.9
 Summary: ABC analysis with automated limit detection
 Home-page: https://github.com/viessmann/abc_analysis
 Author: Tino Gehlert
 Author-email: ghlt@viessmann.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/viessmann/abc_analysis/archive/v0.1.8.tar.gz
+Download-URL: https://github.com/viessmann/abc_analysis/archive/v0.1.9.tar.gz
+Project-URL: Viessmann, https://www.linkedin.com/company/viessmann/
 Description: 
         Performs and visualizes an ABC analysis with automated limit detection.
         
         This package is a Python implementation of the R package `ABCanalysis <https://CRAN.R-project.org/package=ABCanalysis>`__
         
-Keywords: abc-analysis abc_analysis
+Keywords: abc-analysis abc_analysis Viessmann
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `abc_analysis-0.1.8/README.md` & `abc_analysis-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `abc_analysis-0.1.8/setup.py` & `abc_analysis-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 
 setup(name='abc_analysis',
-      version='0.1.8',
+      version='0.1.9',
       description='ABC analysis with automated limit detection',
       long_description="""
 Performs and visualizes an ABC analysis with automated limit detection.
 
 This package is a Python implementation of the R package `ABCanalysis <https://CRAN.R-project.org/package=ABCanalysis>`__
 """,
-      download_url='https://github.com/viessmann/abc_analysis/archive/v0.1.8.tar.gz',
+      download_url='https://github.com/viessmann/abc_analysis/archive/v0.1.9.tar.gz',
       classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.6',
         'Topic :: Scientific/Engineering',
       ],
-      keywords='abc-analysis abc_analysis',
+      keywords='abc-analysis abc_analysis Viessmann',
       url='https://github.com/viessmann/abc_analysis',
+      project_urls={'Viessmann': 'https://www.linkedin.com/company/viessmann/'},
       author='Tino Gehlert',
       author_email='ghlt@viessmann.com',
       license='GNU General Public License v3 (GPLv3)',
       packages=find_packages(),
       install_requires=[
          'pandas>=0.22',
 		  'numpy>=1.14',
```

