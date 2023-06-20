# Comparing `tmp/volue-insight-timeseries-1.0.0b1.tar.gz` & `tmp/volue-insight-timeseries-1.0.0b2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volue-insight-timeseries-1.0.0b1.tar", last modified: Mon Feb 13 11:37:55 2023, max compression
+gzip compressed data, was "volue-insight-timeseries-1.0.0b2.dev1.tar", last modified: Tue Jun 20 08:47:16 2023, max compression
```

## Comparing `volue-insight-timeseries-1.0.0b1.tar` & `volue-insight-timeseries-1.0.0b2.dev1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0     1000 root         (0)        0 2023-02-13 11:37:55.622990 volue-insight-timeseries-1.0.0b1/
--rw-r--r--   0     1000 root         (0)     1069 2023-02-13 11:37:15.000000 volue-insight-timeseries-1.0.0b1/LICENSE
--rw-r--r--   0     1000 root         (0)       34 2023-02-13 11:37:15.000000 volue-insight-timeseries-1.0.0b1/MANIFEST.in
--rw-r--r--   0     1000 root         (0)      575 2023-02-13 11:37:55.622990 volue-insight-timeseries-1.0.0b1/PKG-INFO
--rw-r--r--   0     1000 root         (0)     3214 2023-02-13 11:37:15.000000 volue-insight-timeseries-1.0.0b1/README.md
--rw-r--r--   0     1000 root         (0)        8 2023-02-13 11:37:15.000000 volue-insight-timeseries-1.0.0b1/VERSION
--rw-r--r--   0     1000 root         (0)      148 2023-02-13 11:37:55.624990 volue-insight-timeseries-1.0.0b1/setup.cfg
--rw-r--r--   0     1000 root         (0)     1101 2023-02-13 11:37:15.000000 volue-insight-timeseries-1.0.0b1/setup.py
-drwxr-xr-x   0     1000 root         (0)        0 2023-02-13 11:37:55.619989 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries/
--rw-r--r--   0     1000 root         (0)      154 2023-02-13 11:37:15.000000 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries/__init__.py
--rw-r--r--   0     1000 root         (0)     2117 2023-02-13 11:37:15.000000 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries/auth.py
--rw-r--r--   0     1000 root         (0)    65949 2023-02-13 11:37:15.000000 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries/curves.py
--rw-r--r--   0     1000 root         (0)     4194 2023-02-13 11:37:15.000000 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries/events.py
--rw-r--r--   0     1000 root         (0)    20115 2023-02-13 11:37:15.000000 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries/session.py
--rw-r--r--   0     1000 root         (0)     9284 2023-02-13 11:37:15.000000 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries/util.py
-drwxr-xr-x   0     1000 root         (0)        0 2023-02-13 11:37:55.622990 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries.egg-info/
--rw-r--r--   0     1000 root         (0)      575 2023-02-13 11:37:55.000000 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries.egg-info/PKG-INFO
--rw-r--r--   0     1000 root         (0)      504 2023-02-13 11:37:55.000000 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries.egg-info/SOURCES.txt
--rw-r--r--   0     1000 root         (0)        1 2023-02-13 11:37:55.000000 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries.egg-info/dependency_links.txt
--rw-r--r--   0     1000 root         (0)       60 2023-02-13 11:37:55.000000 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries.egg-info/requires.txt
--rw-r--r--   0     1000 root         (0)       25 2023-02-13 11:37:55.000000 volue-insight-timeseries-1.0.0b1/volue_insight_timeseries.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:47:16.315821 volue-insight-timeseries-1.0.0b2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-20 08:47:16.315821 volue-insight-timeseries-1.0.0b2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 08:47:16.315821 volue-insight-timeseries-1.0.0b2.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:47:16.315821 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65949 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-20 08:47:06.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:47:16.315821 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-20 08:47:16.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-20 08:47:16.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:47:16.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 08:47:16.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 08:47:16.000000 volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/top_level.txt
```

### Comparing `volue-insight-timeseries-1.0.0b1/LICENSE` & `volue-insight-timeseries-1.0.0b2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.0b1/PKG-INFO` & `volue-insight-timeseries-1.0.0b2.dev1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 Metadata-Version: 2.1
 Name: volue-insight-timeseries
-Version: 1.0.0b1
+Version: 1.0.0b2.dev1
 Summary: Volue Insight API python library
 Home-page: https://www.volueinsight.com
 Author: Volue Insight
 Author-email: support.insight@volue.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.9, <3.11a0
+Requires-Python: >=3.9, <3.12a0
 License-File: LICENSE
 
 This library is meant as a simple toolkit for working with data from https://api.volueinsight.com/ (or equivalent services).  Note that access is based on some sort of login credentials, this library is not all that useful unless you have a valid Volue Insight account.
-
```

### Comparing `volue-insight-timeseries-1.0.0b1/README.md` & `volue-insight-timeseries-1.0.0b2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.0b1/volue_insight_timeseries/auth.py` & `volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/auth.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.0b1/volue_insight_timeseries/curves.py` & `volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/curves.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.0b1/volue_insight_timeseries/events.py` & `volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/events.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.0b1/volue_insight_timeseries/session.py` & `volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/session.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.0.0b1/volue_insight_timeseries/util.py` & `volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     def fullname(self):
         attrs = []
         if self.name:
             attrs.append(self.name)
         else:
             if self.id:
                 attrs.append(str(self.id))
-            attrs.extend([self.curve_type, self.tz.zone, self.frequency])
+            attrs.extend([self.curve_type, str(self.tz), self.frequency])
         if self.tag:
             attrs.append(self.tag)
         if self.issue_date:
             attrs.append(str(self.issue_date))
         return ' '.join(attrs)
 
     def to_pandas(self, name=None):
```

### Comparing `volue-insight-timeseries-1.0.0b1/volue_insight_timeseries.egg-info/PKG-INFO` & `volue-insight-timeseries-1.0.0b2.dev1/volue_insight_timeseries.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 Metadata-Version: 2.1
 Name: volue-insight-timeseries
-Version: 1.0.0b1
+Version: 1.0.0b2.dev1
 Summary: Volue Insight API python library
 Home-page: https://www.volueinsight.com
 Author: Volue Insight
 Author-email: support.insight@volue.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.9, <3.11a0
+Requires-Python: >=3.9, <3.12a0
 License-File: LICENSE
 
 This library is meant as a simple toolkit for working with data from https://api.volueinsight.com/ (or equivalent services).  Note that access is based on some sort of login credentials, this library is not all that useful unless you have a valid Volue Insight account.
-
```

