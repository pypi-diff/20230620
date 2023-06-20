# Comparing `tmp/ahoy_dtu_webthing-0.0.8.tar.gz` & `tmp/ahoy_dtu_webthing-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahoy_dtu_webthing-0.0.8.tar", last modified: Mon Jun 19 20:31:18 2023, max compression
+gzip compressed data, was "ahoy_dtu_webthing-0.0.9.tar", last modified: Mon Jun 19 20:37:29 2023, max compression
```

## Comparing `ahoy_dtu_webthing-0.0.8.tar` & `ahoy_dtu_webthing-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:31:18.796286 ahoy_dtu_webthing-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:31:18.796286 ahoy_dtu_webthing-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:31:18.796286 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/dtu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/dtu_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:31:18.796286 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:31:18.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 20:31:18.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:31:18.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 20:31:18.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 20:31:18.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 20:31:18.000000 ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 20:31:07.000000 ahoy_dtu_webthing-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 20:31:18.800286 ahoy_dtu_webthing-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:37:29.864478 ahoy_dtu_webthing-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:37:29.864478 ahoy_dtu_webthing-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:37:29.864478 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/dtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/dtu_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:37:29.864478 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 20:37:29.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-19 20:37:29.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:37:29.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-19 20:37:29.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 20:37:29.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 20:37:29.000000 ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-19 20:37:18.000000 ahoy_dtu_webthing-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-19 20:37:29.864478 ahoy_dtu_webthing-0.0.9/setup.cfg
```

### Comparing `ahoy_dtu_webthing-0.0.8/LICENSE` & `ahoy_dtu_webthing-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.8/PKG-INFO` & `ahoy_dtu_webthing-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy_dtu_webthing
-Version: 0.0.8
+Version: 0.0.9
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ahoy_dtu_webthing-0.0.8/README.md` & `ahoy_dtu_webthing-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/app.py` & `ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/app.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/dtu.py` & `ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/dtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.p_ac = 0
         self.u_ac = 0
         self.i_ac = 0
         self.temp = 0
         self.efficiency = 0
         self.power_max = 0
         self.power_limit = 0
-        self.last_update = datetime.now()
+        self.last_update = datetime.fromtimestamp(0)
         self.is_available = False
         self.is_producing = False
         self.listener = None
         self.refresh()
         self.set_power_limit(self.power_max)
 
     def refresh(self):
```

### Comparing `ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing/dtu_webthing.py` & `ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing/dtu_webthing.py`

 * *Files identical despite different names*

### Comparing `ahoy_dtu_webthing-0.0.8/ahoy_dtu_webthing.egg-info/PKG-INFO` & `ahoy_dtu_webthing-0.0.9/ahoy_dtu_webthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahoy-dtu-webthing
-Version: 0.0.8
+Version: 0.0.9
 Summary: Ahoy DTU webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

