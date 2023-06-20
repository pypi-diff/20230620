# Comparing `tmp/eons-2.6.3.tar.gz` & `tmp/eons-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.6.3.tar", last modified: Tue Jun 20 01:44:00 2023, max compression
+gzip compressed data, was "eons-2.6.4.tar", last modified: Tue Jun 20 04:20:16 2023, max compression
```

## Comparing `eons-2.6.3.tar` & `eons-2.6.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:44:00.892161 eons-2.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-20 01:44:00.892161 eons-2.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-20 01:43:44.000000 eons-2.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:44:00.888161 eons-2.6.3/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:44:00.888161 eons-2.6.3/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 01:43:52.000000 eons-2.6.3/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92293 2023-06-20 01:43:52.000000 eons-2.6.3/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:44:00.888161 eons-2.6.3/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-20 01:43:36.000000 eons-2.6.3/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:43:52.000000 eons-2.6.3/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:44:00.892161 eons-2.6.3/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:43:52.000000 eons-2.6.3/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-20 01:43:36.000000 eons-2.6.3/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-20 01:43:36.000000 eons-2.6.3/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-20 01:43:36.000000 eons-2.6.3/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-20 01:43:36.000000 eons-2.6.3/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 01:43:36.000000 eons-2.6.3/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:44:00.888161 eons-2.6.3/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-20 01:44:00.000000 eons-2.6.3/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-20 01:44:00.000000 eons-2.6.3/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:44:00.000000 eons-2.6.3/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 01:44:00.000000 eons-2.6.3/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 01:44:00.000000 eons-2.6.3/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 01:43:52.000000 eons-2.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-20 01:44:00.892161 eons-2.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:20:16.226518 eons-2.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-20 04:20:16.226518 eons-2.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-20 04:19:57.000000 eons-2.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:20:16.218517 eons-2.6.4/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:20:16.222517 eons-2.6.4/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 04:20:06.000000 eons-2.6.4/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92334 2023-06-20 04:20:06.000000 eons-2.6.4/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:20:16.222517 eons-2.6.4/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-20 04:19:47.000000 eons-2.6.4/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:20:06.000000 eons-2.6.4/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:20:16.226518 eons-2.6.4/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:20:06.000000 eons-2.6.4/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-20 04:19:47.000000 eons-2.6.4/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-20 04:19:47.000000 eons-2.6.4/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-20 04:19:47.000000 eons-2.6.4/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-20 04:19:47.000000 eons-2.6.4/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 04:19:47.000000 eons-2.6.4/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:20:16.222517 eons-2.6.4/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-20 04:20:16.000000 eons-2.6.4/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-20 04:20:16.000000 eons-2.6.4/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:20:16.000000 eons-2.6.4/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 04:20:16.000000 eons-2.6.4/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 04:20:16.000000 eons-2.6.4/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 04:20:06.000000 eons-2.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-20 04:20:16.226518 eons-2.6.4/setup.cfg
```

### Comparing `eons-2.6.3/PKG-INFO` & `eons-2.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.6.3
+Version: 2.6.4
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.6.3/README.md` & `eons-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.6.3/pkg/eons/eons.py` & `eons-2.6.4/pkg/eons/eons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1646,15 +1646,15 @@
 
 	# End the current placement session (if any)
 	def ResetPlacementSession(this):
 		this.placement.session.active = False
 		this.placement.session.level = this.placement.max
 		this.placement.session.hierarchy = {}
 		this.placement.session.current = []
-		logging.debug(f"Dependency placement session ended; level is now {this.placement.session.level}")
+		# logging.debug(f"Dependency placement session ended; level is now {this.placement.session.level}")
 
 	# Track to the current location in the placement hierarchy.
 	def GetPlacementSessionCurrentPosition(this):
 		if (not this.placement.session.active):
 			return None
 		ret = this.placement.session.hierarchy
 		for place in this.placement.session.hierarchy:
@@ -1664,30 +1664,30 @@
 	def BeginPlacing(this, toPlace):
 		if (not this.placement.session.active):
 			this.placement.session.active = True
 		hierarchy = this.GetPlacementSessionCurrentPosition()
 		hierarchy[toPlace] = {}
 		this.placement.session.current.append(toPlace)
 		this.placement.session.level -= 1
-		logging.debug(f"Placing {toPlace}; level is now {this.placement.session.level}")
+		logging.debug(f"Prepared to place dependencies for {toPlace}; level is now {this.placement.session.level}")
 
 	# Once the proper location of a Functor has been derived, remove it from the hierarchy.
 	# Additionally, if we're the last ones to play with the current session, reset it.
 	def ResolvePlacementOf(this, placed):
 		if (not this.placement.session.active):
 			return
 		try:
 			this.placement.session.current.remove(placed)
 			hierarchy = this.GetPlacementSessionCurrentPosition()
 			if (not len(this.placement.session.current)):
 				this.ResetPlacementSession()
 			elif (hierarchy and placed in hierarchy.keys()):
 				del hierarchy[placed]
 				this.placement.session.level += 1
-			logging.debug(f"Resolved placement of {placed}; level is now {this.placement.session.level}")
+			logging.debug(f"Finished placing dependencies for {placed}; level is now {this.placement.session.level}")
 		except:
 			pass # key errors when getting an existing Functor...
 		
 
 	# Create any sub-class necessary for child-operations
 	# Does not RETURN anything.
 	def InitData(this):
```

### Comparing `eons-2.6.3/pkg/eons/method/External.py` & `eons-2.6.4/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.3/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.6.4/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.3/pkg/eons/resolve/resolve_import_module.py` & `eons-2.6.4/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.3/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.6.4/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.3/pkg/eons.egg-info/PKG-INFO` & `eons-2.6.4/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.6.3
+Version: 2.6.4
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.6.3/pkg/eons.egg-info/SOURCES.txt` & `eons-2.6.4/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.6.3/setup.cfg` & `eons-2.6.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.6.3
+version = 2.6.4
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -19,18 +19,18 @@
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	jsonpickle
-	pyyaml
+	eot
 	requests
+	pyyaml
 	tqdm
-	eot
 	requests_futures
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build =
```

