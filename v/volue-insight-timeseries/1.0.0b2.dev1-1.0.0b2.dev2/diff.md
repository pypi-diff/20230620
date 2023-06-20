# Comparing `tmp/volue-insight-timeseries-1.0.0b2.dev1.tar.gz` & `tmp/volue-insight-timeseries-1.0.0b2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volue-insight-timeseries-1.0.0b2.dev1.tar", last modified: Tue Jun 20 08:47:16 2023, max compression
+gzip compressed data, was "volue-insight-timeseries-1.0.0b2.dev2.tar", last modified: Tue Jun 20 08:54:47 2023, max compression
```

## Comparing `volue-insight-timeseries-1.0.0b2.dev1.tar` & `volue-insight-timeseries-1.0.0b2.dev2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:47:16.315821 volue-insight-timeseries-1.0.0b2.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-20 08:47:16.315821 volue-insight-timeseries-1.0.0b2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 08:47:16.315821 volue-insight-timeseries-1.0.0b2.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:47:16.315821 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    65949 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:47:16.315821 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-20 08:47:16.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-20 08:47:16.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:47:16.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 08:47:16.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 08:47:16.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:54:47.688860 volue-insight-timeseries-1.0.0b2.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 08:54:36.000000 volue-insight-timeseries-1.0.0b2.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 08:54:36.000000 volue-insight-timeseries-1.0.0b2.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-20 08:54:47.688860 volue-insight-timeseries-1.0.0b2.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-20 08:54:36.000000 volue-insight-timeseries-1.0.0b2.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 08:54:47.688860 volue-insight-timeseries-1.0.0b2.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-20 08:54:36.000000 volue-insight-timeseries-1.0.0b2.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:54:47.688860 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 08:54:45.000000 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-20 08:54:36.000000 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-20 08:54:36.000000 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65949 2023-06-20 08:54:36.000000 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-20 08:54:36.000000 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-06-20 08:54:36.000000 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-20 08:54:36.000000 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:54:47.688860 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-20 08:54:47.000000 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-20 08:54:47.000000 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:54:47.000000 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 08:54:47.000000 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 08:54:47.000000 volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries.egg-info/top_level.txt
```

### Comparing `volue-insight-timeseries-1.0.0b2.dev1/LICENSE` & `volue-insight-timeseries-1.0.0b2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.0b2.dev1/README.md` & `volue-insight-timeseries-1.0.0b2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.0b2.dev1/setup.py` & `volue-insight-timeseries-1.0.0b2.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,12 +34,12 @@
         'pytest',
         'pytest-cov >= 2.5',
         'requests-mock >= 1.3',
     ],
     version=version,
     description='Volue Insight API python library',
     long_description='This library is meant as a simple toolkit for working with data from https://api.volueinsight.com/ (or equivalent services).  Note that access is based on some sort of login credentials, this library is not all that useful unless you have a valid Volue Insight account.',
-    package_data={'volue_inisight_timeseries': ['VERSION']},
+    package_data={'volue_insight_timeseries': ['VERSION']},
     author='Volue Insight',
     author_email='support.insight@volue.com',
     url='https://www.volueinsight.com'
 )
```

### Comparing `volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/auth.py` & `volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/auth.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/curves.py` & `volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/curves.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/events.py` & `volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/events.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/session.py` & `volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/session.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/util.py` & `volue-insight-timeseries-1.0.0b2.dev2/volue_insight_timeseries/util.py`

 * *Files identical despite different names*

