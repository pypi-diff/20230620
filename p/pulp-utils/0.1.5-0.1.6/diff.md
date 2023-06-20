# Comparing `tmp/pulp_utils-0.1.5.tar.gz` & `tmp/pulp_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulp_utils-0.1.5.tar", last modified: Thu Oct 27 23:50:03 2022, max compression
+gzip compressed data, was "dist/pulp_utils-0.1.6.tar", last modified: Tue Jun 20 09:23:19 2023, max compression
```

## Comparing `pulp_utils-0.1.5.tar` & `pulp_utils-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2022-10-27 23:50:03.452405 pulp_utils-0.1.5/
--rw-r--r--   0 bmduser    (501) staff       (20)     1062 2022-10-20 04:41:37.000000 pulp_utils-0.1.5/LICENSE
--rw-r--r--   0 bmduser    (501) staff       (20)      922 2022-10-27 23:50:03.452520 pulp_utils-0.1.5/PKG-INFO
--rw-r--r--   0 bmduser    (501) staff       (20)      135 2022-10-20 04:25:16.000000 pulp_utils-0.1.5/README.md
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2022-10-27 23:50:03.450878 pulp_utils-0.1.5/pulp_utils/
--rw-r--r--   0 bmduser    (501) staff       (20)       94 2022-10-27 20:41:42.000000 pulp_utils-0.1.5/pulp_utils/__init__.py
--rw-r--r--   0 bmduser    (501) staff       (20)     1579 2022-10-27 20:49:33.000000 pulp_utils-0.1.5/pulp_utils/report.py
--rw-r--r--   0 bmduser    (501) staff       (20)     2416 2022-10-27 11:39:24.000000 pulp_utils-0.1.5/pulp_utils/transportation.py
--rw-r--r--   0 bmduser    (501) staff       (20)     3144 2022-10-27 20:50:50.000000 pulp_utils-0.1.5/pulp_utils/tsp.py
-drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2022-10-27 23:50:03.452180 pulp_utils-0.1.5/pulp_utils.egg-info/
--rw-r--r--   0 bmduser    (501) staff       (20)      922 2022-10-27 23:50:03.000000 pulp_utils-0.1.5/pulp_utils.egg-info/PKG-INFO
--rw-r--r--   0 bmduser    (501) staff       (20)      296 2022-10-27 23:50:03.000000 pulp_utils-0.1.5/pulp_utils.egg-info/SOURCES.txt
--rw-r--r--   0 bmduser    (501) staff       (20)        1 2022-10-27 23:50:03.000000 pulp_utils-0.1.5/pulp_utils.egg-info/dependency_links.txt
--rw-r--r--   0 bmduser    (501) staff       (20)       28 2022-10-27 23:50:03.000000 pulp_utils-0.1.5/pulp_utils.egg-info/requires.txt
--rw-r--r--   0 bmduser    (501) staff       (20)       11 2022-10-27 23:50:03.000000 pulp_utils-0.1.5/pulp_utils.egg-info/top_level.txt
--rw-r--r--   0 bmduser    (501) staff       (20)       67 2022-10-27 23:50:03.452907 pulp_utils-0.1.5/setup.cfg
--rw-r--r--   0 bmduser    (501) staff       (20)     1093 2022-10-27 22:23:10.000000 pulp_utils-0.1.5/setup.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-06-20 09:23:19.005350 pulp_utils-0.1.6/
+-rw-r--r--   0 bmduser    (501) staff       (20)     1062 2023-06-20 09:20:19.000000 pulp_utils-0.1.6/LICENSE
+-rw-r--r--   0 bmduser    (501) staff       (20)      973 2023-06-20 09:23:19.005464 pulp_utils-0.1.6/PKG-INFO
+-rw-r--r--   0 bmduser    (501) staff       (20)      135 2023-06-20 09:20:19.000000 pulp_utils-0.1.6/README.md
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-06-20 09:23:19.003705 pulp_utils-0.1.6/pulp_utils/
+-rw-r--r--   0 bmduser    (501) staff       (20)       94 2023-06-20 09:21:02.000000 pulp_utils-0.1.6/pulp_utils/__init__.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     1579 2023-06-20 09:20:19.000000 pulp_utils-0.1.6/pulp_utils/report.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     2416 2023-06-20 09:20:19.000000 pulp_utils-0.1.6/pulp_utils/transportation.py
+-rw-r--r--   0 bmduser    (501) staff       (20)     3144 2023-06-20 09:20:19.000000 pulp_utils-0.1.6/pulp_utils/tsp.py
+drwxr-xr-x   0 bmduser    (501) staff       (20)        0 2023-06-20 09:23:19.005120 pulp_utils-0.1.6/pulp_utils.egg-info/
+-rw-r--r--   0 bmduser    (501) staff       (20)      973 2023-06-20 09:23:18.000000 pulp_utils-0.1.6/pulp_utils.egg-info/PKG-INFO
+-rw-r--r--   0 bmduser    (501) staff       (20)      296 2023-06-20 09:23:18.000000 pulp_utils-0.1.6/pulp_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)        1 2023-06-20 09:23:18.000000 pulp_utils-0.1.6/pulp_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)       23 2023-06-20 09:23:18.000000 pulp_utils-0.1.6/pulp_utils.egg-info/requires.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)       11 2023-06-20 09:23:18.000000 pulp_utils-0.1.6/pulp_utils.egg-info/top_level.txt
+-rw-r--r--   0 bmduser    (501) staff       (20)       67 2023-06-20 09:23:19.005967 pulp_utils-0.1.6/setup.cfg
+-rw-r--r--   0 bmduser    (501) staff       (20)     1135 2023-06-20 09:20:41.000000 pulp_utils-0.1.6/setup.py
```

### Comparing `pulp_utils-0.1.5/LICENSE` & `pulp_utils-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp_utils-0.1.5/PKG-INFO` & `pulp_utils-0.1.6/pulp_utils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
-Name: pulp_utils
-Version: 0.1.5
+Name: pulp-utils
+Version: 0.1.6
 Summary: pulp_utils is a library with utility tools for PuLP
 Home-page: https://github.com/WiraDKP/pulp_utils
 Author: Wira Dharma Kencana Putra
 Author-email: wiradharma_kencanaputra@yahoo.com
 Keywords: linear programming operations research optimization jcop indonesia
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: Indonesian
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pulp_utils-0.1.5/pulp_utils/report.py` & `pulp_utils-0.1.6/pulp_utils/report.py`

 * *Files identical despite different names*

### Comparing `pulp_utils-0.1.5/pulp_utils/transportation.py` & `pulp_utils-0.1.6/pulp_utils/transportation.py`

 * *Files identical despite different names*

### Comparing `pulp_utils-0.1.5/pulp_utils/tsp.py` & `pulp_utils-0.1.6/pulp_utils/tsp.py`

 * *Files identical despite different names*

### Comparing `pulp_utils-0.1.5/pulp_utils.egg-info/PKG-INFO` & `pulp_utils-0.1.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
-Name: pulp-utils
-Version: 0.1.5
+Name: pulp_utils
+Version: 0.1.6
 Summary: pulp_utils is a library with utility tools for PuLP
 Home-page: https://github.com/WiraDKP/pulp_utils
 Author: Wira Dharma Kencana Putra
 Author-email: wiradharma_kencanaputra@yahoo.com
 Keywords: linear programming operations research optimization jcop indonesia
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: Indonesian
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pulp_utils-0.1.5/setup.py` & `pulp_utils-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,21 +9,22 @@
     version=pulp_utils.__version__,
     author="Wira Dharma Kencana Putra",
     author_email="wiradharma_kencanaputra@yahoo.com",
     description="pulp_utils is a library with utility tools for PuLP",
     long_description=description,
     long_description_content_type="text/markdown",
     python_requires=">=3.7",
-    install_requires=['pulp', 'numpy', 'scipy', 'matplotlib'],
+    install_requires=['numpy', 'scipy', 'matplotlib'],
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "Natural Language :: Indonesian",
         "Natural Language :: English"
     ],
     keywords="linear programming operations research optimization jcop indonesia",
     url="https://github.com/WiraDKP/pulp_utils"
```

