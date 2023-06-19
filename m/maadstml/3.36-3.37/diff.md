# Comparing `tmp/maadstml-3.36.tar.gz` & `tmp/maadstml-3.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadstml-3.36.tar", last modified: Mon Jun 19 21:22:21 2023, max compression
+gzip compressed data, was "maadstml-3.37.tar", last modified: Mon Jun 19 23:47:42 2023, max compression
```

## Comparing `maadstml-3.36.tar` & `maadstml-3.37.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 21:22:21.749509 maadstml-3.36/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.36/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.36/MANIFEST.in
--rw-rw-rw-   0        0        0   174408 2023-06-19 21:22:21.748946 maadstml-3.36/PKG-INFO
--rw-rw-rw-   0        0        0   173811 2023-06-13 18:28:52.000000 maadstml-3.36/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 21:22:21.696196 maadstml-3.36/maadstml/
--rw-rw-rw-   0        0        0     2387 2023-06-13 18:19:41.000000 maadstml-3.36/maadstml/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.36/maadstml/readpdf.py
--rw-rw-rw-   0        0        0    81649 2023-06-13 19:45:36.000000 maadstml-3.36/maadstml/sendfiles.py
--rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.36/maadstml/tmltextsummary.py
-drwxrwxrwx   0        0        0        0 2023-06-19 21:22:21.739827 maadstml-3.36/maadstml.egg-info/
--rw-rw-rw-   0        0        0   174408 2023-06-19 21:22:21.000000 maadstml-3.36/maadstml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-06-19 21:22:21.000000 maadstml-3.36/maadstml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 21:22:21.000000 maadstml-3.36/maadstml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2023-06-19 21:22:21.000000 maadstml-3.36/maadstml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-19 21:22:21.000000 maadstml-3.36/maadstml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      234 2023-06-19 21:15:50.000000 maadstml-3.36/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 21:22:21.749509 maadstml-3.36/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-06-19 21:21:21.000000 maadstml-3.36/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:47:41.997992 maadstml-3.37/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.37/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.37/MANIFEST.in
+-rw-rw-rw-   0        0        0   174408 2023-06-19 23:47:41.997992 maadstml-3.37/PKG-INFO
+-rw-rw-rw-   0        0        0   173811 2023-06-13 18:28:52.000000 maadstml-3.37/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 23:47:41.984117 maadstml-3.37/maadstml/
+-rw-rw-rw-   0        0        0     2387 2023-06-13 18:19:41.000000 maadstml-3.37/maadstml/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.37/maadstml/readpdf.py
+-rw-rw-rw-   0        0        0    81649 2023-06-13 19:45:36.000000 maadstml-3.37/maadstml/sendfiles.py
+-rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.37/maadstml/tmltextsummary.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:47:41.997992 maadstml-3.37/maadstml.egg-info/
+-rw-rw-rw-   0        0        0   174408 2023-06-19 23:47:41.000000 maadstml-3.37/maadstml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-19 23:47:41.000000 maadstml-3.37/maadstml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 23:47:41.000000 maadstml-3.37/maadstml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      223 2023-06-19 23:47:41.000000 maadstml-3.37/maadstml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-19 23:47:41.000000 maadstml-3.37/maadstml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      239 2023-06-19 23:47:07.000000 maadstml-3.37/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 23:47:41.997992 maadstml-3.37/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-06-19 23:47:36.000000 maadstml-3.37/setup.py
```

### Comparing `maadstml-3.36/LICENSE.txt` & `maadstml-3.37/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstml-3.36/PKG-INFO` & `maadstml-3.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.36
+Version: 3.37
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadstml-3.36/README.md` & `maadstml-3.37/README.md`

 * *Files identical despite different names*

### Comparing `maadstml-3.36/maadstml/__init__.py` & `maadstml-3.37/maadstml/__init__.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.36/maadstml/readpdf.py` & `maadstml-3.37/maadstml/readpdf.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.36/maadstml/sendfiles.py` & `maadstml-3.37/maadstml/sendfiles.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.36/maadstml/tmltextsummary.py` & `maadstml-3.37/maadstml/tmltextsummary.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.36/maadstml.egg-info/PKG-INFO` & `maadstml-3.37/maadstml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.36
+Version: 3.37
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadstml-3.36/setup.py` & `maadstml-3.37/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstml',
-    version='3.36',
+    version='3.37',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

