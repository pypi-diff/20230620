# Comparing `tmp/metlo-0.0.8.tar.gz` & `tmp/metlo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metlo-0.0.8.tar", last modified: Mon Sep 27 20:01:57 2021, max compression
+gzip compressed data, was "metlo-0.0.9.tar", last modified: Fri Oct  1 04:50:35 2021, max compression
```

## Comparing `metlo-0.0.8.tar` & `metlo-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2021-09-27 20:01:57.366656 metlo-0.0.8/
--rw-r--r--   0 akshay     (501) staff       (20)      638 2021-09-27 20:01:57.366453 metlo-0.0.8/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)       79 2021-09-16 23:45:35.000000 metlo-0.0.8/README.md
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2021-09-27 20:01:57.363460 metlo-0.0.8/metlo/
--rw-r--r--   0 akshay     (501) staff       (20)      159 2021-09-27 20:00:50.000000 metlo-0.0.8/metlo/__init__.py
--rw-r--r--   0 akshay     (501) staff       (20)     2497 2021-09-27 19:43:54.000000 metlo-0.0.8/metlo/api.py
--rw-r--r--   0 akshay     (501) staff       (20)     1591 2021-09-19 00:42:54.000000 metlo-0.0.8/metlo/command_line.py
--rw-r--r--   0 akshay     (501) staff       (20)     1346 2021-09-19 06:20:48.000000 metlo-0.0.8/metlo/config.py
--rw-r--r--   0 akshay     (501) staff       (20)      544 2021-09-19 00:21:50.000000 metlo-0.0.8/metlo/load_definitions.py
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2021-09-27 20:01:57.364371 metlo-0.0.8/metlo/types/
--rw-r--r--   0 akshay     (501) staff       (20)        0 2021-09-18 22:57:57.000000 metlo-0.0.8/metlo/types/__init__.py
--rw-r--r--   0 akshay     (501) staff       (20)     1771 2021-09-20 01:05:19.000000 metlo-0.0.8/metlo/types/definition.py
--rw-r--r--   0 akshay     (501) staff       (20)      938 2021-09-18 22:57:41.000000 metlo-0.0.8/metlo/types/enums.py
--rw-r--r--   0 akshay     (501) staff       (20)      444 2021-09-18 22:58:23.000000 metlo-0.0.8/metlo/types/query.py
--rw-r--r--   0 akshay     (501) staff       (20)      243 2021-09-17 00:36:52.000000 metlo-0.0.8/metlo/utils.py
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2021-09-27 20:01:57.366088 metlo-0.0.8/metlo.egg-info/
--rw-r--r--   0 akshay     (501) staff       (20)      638 2021-09-27 20:01:57.000000 metlo-0.0.8/metlo.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)      416 2021-09-27 20:01:57.000000 metlo-0.0.8/metlo.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (501) staff       (20)        1 2021-09-27 20:01:57.000000 metlo-0.0.8/metlo.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (501) staff       (20)       51 2021-09-27 20:01:57.000000 metlo-0.0.8/metlo.egg-info/entry_points.txt
--rw-r--r--   0 akshay     (501) staff       (20)      109 2021-09-27 20:01:57.000000 metlo-0.0.8/metlo.egg-info/requires.txt
--rw-r--r--   0 akshay     (501) staff       (20)        6 2021-09-27 20:01:57.000000 metlo-0.0.8/metlo.egg-info/top_level.txt
--rw-r--r--   0 akshay     (501) staff       (20)       38 2021-09-27 20:01:57.366717 metlo-0.0.8/setup.cfg
--rw-r--r--   0 akshay     (501) staff       (20)     1120 2021-09-27 20:00:40.000000 metlo-0.0.8/setup.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2021-10-01 04:50:35.694925 metlo-0.0.9/
+-rw-r--r--   0 akshay     (501) staff       (20)      638 2021-10-01 04:50:35.694662 metlo-0.0.9/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)       79 2021-09-16 23:45:35.000000 metlo-0.0.9/README.md
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2021-10-01 04:50:35.690190 metlo-0.0.9/metlo/
+-rw-r--r--   0 akshay     (501) staff       (20)      159 2021-10-01 04:29:39.000000 metlo-0.0.9/metlo/__init__.py
+-rw-r--r--   0 akshay     (501) staff       (20)     2554 2021-10-01 02:57:00.000000 metlo-0.0.9/metlo/api.py
+-rw-r--r--   0 akshay     (501) staff       (20)     1591 2021-09-19 00:42:54.000000 metlo-0.0.9/metlo/command_line.py
+-rw-r--r--   0 akshay     (501) staff       (20)     1346 2021-09-19 06:20:48.000000 metlo-0.0.9/metlo/config.py
+-rw-r--r--   0 akshay     (501) staff       (20)      544 2021-09-19 00:21:50.000000 metlo-0.0.9/metlo/load_definitions.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2021-10-01 04:50:35.692829 metlo-0.0.9/metlo/types/
+-rw-r--r--   0 akshay     (501) staff       (20)        0 2021-09-18 22:57:57.000000 metlo-0.0.9/metlo/types/__init__.py
+-rw-r--r--   0 akshay     (501) staff       (20)     1771 2021-09-20 01:05:19.000000 metlo-0.0.9/metlo/types/definition.py
+-rw-r--r--   0 akshay     (501) staff       (20)      938 2021-09-18 22:57:41.000000 metlo-0.0.9/metlo/types/enums.py
+-rw-r--r--   0 akshay     (501) staff       (20)      444 2021-09-18 22:58:23.000000 metlo-0.0.9/metlo/types/query.py
+-rw-r--r--   0 akshay     (501) staff       (20)      243 2021-09-17 00:36:52.000000 metlo-0.0.9/metlo/utils.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2021-10-01 04:50:35.694324 metlo-0.0.9/metlo.egg-info/
+-rw-r--r--   0 akshay     (501) staff       (20)      638 2021-10-01 04:50:35.000000 metlo-0.0.9/metlo.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)      416 2021-10-01 04:50:35.000000 metlo-0.0.9/metlo.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        1 2021-10-01 04:50:35.000000 metlo-0.0.9/metlo.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       51 2021-10-01 04:50:35.000000 metlo-0.0.9/metlo.egg-info/entry_points.txt
+-rw-r--r--   0 akshay     (501) staff       (20)      109 2021-10-01 04:50:35.000000 metlo-0.0.9/metlo.egg-info/requires.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        6 2021-10-01 04:50:35.000000 metlo-0.0.9/metlo.egg-info/top_level.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       38 2021-10-01 04:50:35.695007 metlo-0.0.9/setup.cfg
+-rw-r--r--   0 akshay     (501) staff       (20)     1120 2021-10-01 04:29:34.000000 metlo-0.0.9/setup.py
```

### Comparing `metlo-0.0.8/PKG-INFO` & `metlo-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metlo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Metlo's Python SDK
 Home-page: UNKNOWN
 Author: S2 Labs Inc.
 Author-email: akshay@metlo.com
 License: MIT
 Project-URL: Homepage, https://www.metlo.com
 Project-URL: Documentation, https://docs.metlo.com
```

### Comparing `metlo-0.0.8/metlo/api.py` & `metlo-0.0.9/metlo/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 
 def query(
     metrics: Union[str, List[str]],
     filters: List[Filter] = [],
     groups: List[str] = [],
     time_dimensions: List[TimeDimension] = [],
+    limit: Optional[int] = None,
     streaming = False,
 ) -> Optional[pd.DataFrame]:
     colorama_init()
     if not isinstance(metrics, list):
         metrics = [metrics]
 
     conf = get_config()
@@ -31,14 +32,15 @@
         return
 
     query_data = {
         'metrics': metrics,
         'filters': [asdict(e) for e in filters],
         'groups': groups,
         'time_dimensions': [asdict(e) for e in time_dimensions],
+        'limit': limit,
         'streaming': streaming,
     }
 
     if conf.definition_dir:
         request_data = {
             'query': query_data,
             'definitions': [
```

### Comparing `metlo-0.0.8/metlo/command_line.py` & `metlo-0.0.9/metlo/command_line.py`

 * *Files identical despite different names*

### Comparing `metlo-0.0.8/metlo/config.py` & `metlo-0.0.9/metlo/config.py`

 * *Files identical despite different names*

### Comparing `metlo-0.0.8/metlo/load_definitions.py` & `metlo-0.0.9/metlo/load_definitions.py`

 * *Files identical despite different names*

### Comparing `metlo-0.0.8/metlo/types/definition.py` & `metlo-0.0.9/metlo/types/definition.py`

 * *Files identical despite different names*

### Comparing `metlo-0.0.8/metlo/types/enums.py` & `metlo-0.0.9/metlo/types/enums.py`

 * *Files identical despite different names*

### Comparing `metlo-0.0.8/metlo.egg-info/PKG-INFO` & `metlo-0.0.9/metlo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metlo
-Version: 0.0.8
+Version: 0.0.9
 Summary: Metlo's Python SDK
 Home-page: UNKNOWN
 Author: S2 Labs Inc.
 Author-email: akshay@metlo.com
 License: MIT
 Project-URL: Homepage, https://www.metlo.com
 Project-URL: Documentation, https://docs.metlo.com
```

### Comparing `metlo-0.0.8/setup.py` & `metlo-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / 'README.md').read_text()
 
 with open(this_directory / 'requirements.in') as f:
     required = f.read().strip().splitlines()
 
 setuptools.setup(
     name='metlo',
-    version='0.0.8',
+    version='0.0.9',
     author='S2 Labs Inc.',
     author_email='akshay@metlo.com',
     description='Metlo\'s Python SDK',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     python_requires='>=3.0',
```

