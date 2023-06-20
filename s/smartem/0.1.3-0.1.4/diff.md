# Comparing `tmp/smartem-0.1.3.tar.gz` & `tmp/smartem-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartem-0.1.3.tar", last modified: Fri Jun  9 09:19:16 2023, max compression
+gzip compressed data, was "smartem-0.1.4.tar", last modified: Tue Jun 20 14:05:38 2023, max compression
```

## Comparing `smartem-0.1.3.tar` & `smartem-0.1.4.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.288080 smartem-0.1.3/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1486 2022-06-01 11:07:25.000000 smartem-0.1.3/LICENSE
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1248 2023-06-09 09:19:16.288080 smartem-0.1.3/PKG-INFO
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1046 2022-06-01 12:11:08.000000 smartem-0.1.3/README.rst
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      130 2022-06-01 11:44:37.000000 smartem-0.1.3/pyproject.toml
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1218 2023-06-09 09:19:16.289080 smartem-0.1.3/setup.cfg
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      154 2022-06-01 11:07:25.000000 smartem-0.1.3/setup.py
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.266080 smartem-0.1.3/src/
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.269080 smartem-0.1.3/src/smartem/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      212 2023-06-09 09:16:37.000000 smartem-0.1.3/src/smartem/__init__.py
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.276080 smartem-0.1.3/src/smartem/cli/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        0 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/cli/__init__.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      808 2022-06-01 15:51:48.000000 smartem-0.1.3/src/smartem/cli/change_epu_directory.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1143 2022-09-28 11:51:20.000000 smartem-0.1.3/src/smartem/cli/export.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2864 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/cli/initialise.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      158 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/cli/launch.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2105 2022-06-07 15:03:21.000000 smartem-0.1.3/src/smartem/cli/missing.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      717 2023-06-09 09:16:23.000000 smartem-0.1.3/src/smartem/cli/quick_epu_viewer.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1253 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/cli/start.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      883 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/cli/stop.py
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.279080 smartem-0.1.3/src/smartem/data_model/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     7130 2022-10-05 09:04:05.000000 smartem-0.1.3/src/smartem/data_model/__init__.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2375 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/data_model/construct.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    35995 2022-07-14 14:09:47.000000 smartem-0.1.3/src/smartem/data_model/extract.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    11757 2022-06-24 14:10:56.000000 smartem-0.1.3/src/smartem/data_model/structure.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    14708 2023-06-09 09:16:14.000000 smartem-0.1.3/src/smartem/data_model/torch.py
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.279080 smartem-0.1.3/src/smartem/gui/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        0 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/gui/__init__.py
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.284079 smartem-0.1.3/src/smartem/gui/qt/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    10881 2022-08-08 10:49:51.000000 smartem-0.1.3/src/smartem/gui/qt/__init__.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2164 2022-06-20 16:22:21.000000 smartem-0.1.3/src/smartem/gui/qt/component_tab.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    38827 2022-10-24 11:47:57.000000 smartem-0.1.3/src/smartem/gui/qt/display.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    12229 2022-09-28 11:51:20.000000 smartem-0.1.3/src/smartem/gui/qt/image_utils.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    24920 2022-06-27 16:06:26.000000 smartem-0.1.3/src/smartem/gui/qt/loader.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     5086 2022-06-23 16:20:23.000000 smartem-0.1.3/src/smartem/gui/qt/loader_csv.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1419 2022-06-24 11:19:21.000000 smartem-0.1.3/src/smartem/gui/qt/plotting_utils.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1289 2022-08-08 11:23:01.000000 smartem-0.1.3/src/smartem/gui/qt/qt_style.css
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.287079 smartem-0.1.3/src/smartem/parsing/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        0 2022-06-01 11:07:25.000000 smartem-0.1.3/src/smartem/parsing/__init__.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    19542 2023-06-09 09:16:23.000000 smartem-0.1.3/src/smartem/parsing/epu.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    12274 2023-06-09 09:16:23.000000 smartem-0.1.3/src/smartem/parsing/epu_vis.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    13637 2022-10-24 11:27:26.000000 smartem-0.1.3/src/smartem/parsing/export.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     5608 2022-08-05 15:49:38.000000 smartem-0.1.3/src/smartem/parsing/relion_default.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)    12683 2022-06-27 16:06:15.000000 smartem-0.1.3/src/smartem/parsing/star.py
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     2434 2022-08-05 10:46:09.000000 smartem-0.1.3/src/smartem/stage_model.py
-drwxrwxr-x   0 kif41228 (1218358) kif41228 (1218358)        0 2023-06-09 09:19:16.272080 smartem-0.1.3/src/smartem.egg-info/
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1248 2023-06-09 09:19:16.000000 smartem-0.1.3/src/smartem.egg-info/PKG-INFO
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)     1260 2023-06-09 09:19:16.000000 smartem-0.1.3/src/smartem.egg-info/SOURCES.txt
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        1 2023-06-09 09:19:16.000000 smartem-0.1.3/src/smartem.egg-info/dependency_links.txt
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)      372 2023-06-09 09:19:16.000000 smartem-0.1.3/src/smartem.egg-info/entry_points.txt
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        1 2022-06-01 11:46:31.000000 smartem-0.1.3/src/smartem.egg-info/not-zip-safe
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)       91 2023-06-09 09:19:16.000000 smartem-0.1.3/src/smartem.egg-info/requires.txt
--rw-rw-r--   0 kif41228 (1218358) kif41228 (1218358)        8 2023-06-09 09:19:16.000000 smartem-0.1.3/src/smartem.egg-info/top_level.txt
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.868933 smartem-0.1.4/
+-rw-r--r--   0 kif41228   (504) staff       (20)     1486 2022-12-08 11:26:40.000000 smartem-0.1.4/LICENSE
+-rw-r--r--   0 kif41228   (504) staff       (20)     1248 2023-06-20 14:05:38.869018 smartem-0.1.4/PKG-INFO
+-rw-r--r--   0 kif41228   (504) staff       (20)     1046 2022-12-08 11:26:40.000000 smartem-0.1.4/README.rst
+-rw-r--r--   0 kif41228   (504) staff       (20)      130 2022-12-08 11:26:40.000000 smartem-0.1.4/pyproject.toml
+-rw-r--r--   0 kif41228   (504) staff       (20)     1224 2023-06-20 14:05:38.869428 smartem-0.1.4/setup.cfg
+-rw-r--r--   0 kif41228   (504) staff       (20)      154 2022-12-08 11:26:40.000000 smartem-0.1.4/setup.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.859585 smartem-0.1.4/src/
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.861520 smartem-0.1.4/src/smartem/
+-rw-r--r--   0 kif41228   (504) staff       (20)      212 2023-06-20 14:04:04.000000 smartem-0.1.4/src/smartem/__init__.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.864482 smartem-0.1.4/src/smartem/cli/
+-rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)      808 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/change_epu_directory.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1143 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/export.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2864 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/initialise.py
+-rw-r--r--   0 kif41228   (504) staff       (20)      158 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/launch.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2105 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/missing.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1136 2023-06-15 15:34:04.000000 smartem-0.1.4/src/smartem/cli/quick_epu_viewer.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1253 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/start.py
+-rw-r--r--   0 kif41228   (504) staff       (20)      883 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/cli/stop.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.865413 smartem-0.1.4/src/smartem/data_model/
+-rw-r--r--   0 kif41228   (504) staff       (20)     7130 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/data_model/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2375 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/data_model/construct.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    35995 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/data_model/extract.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    11757 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/data_model/structure.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    14708 2023-06-15 09:29:29.000000 smartem-0.1.4/src/smartem/data_model/torch.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.865676 smartem-0.1.4/src/smartem/gui/
+-rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/__init__.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.867248 smartem-0.1.4/src/smartem/gui/qt/
+-rw-r--r--   0 kif41228   (504) staff       (20)    10881 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2164 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/component_tab.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    38827 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/display.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    12229 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/image_utils.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    24920 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/loader.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     5086 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/loader_csv.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1419 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/plotting_utils.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     1289 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/gui/qt/qt_style.css
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.868486 smartem-0.1.4/src/smartem/parsing/
+-rw-r--r--   0 kif41228   (504) staff       (20)        0 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/parsing/__init__.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    19542 2023-06-15 09:29:29.000000 smartem-0.1.4/src/smartem/parsing/epu.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    12550 2023-06-20 14:03:27.000000 smartem-0.1.4/src/smartem/parsing/epu_vis.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    13637 2023-05-15 12:06:59.000000 smartem-0.1.4/src/smartem/parsing/export.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     5608 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/parsing/relion_default.py
+-rw-r--r--   0 kif41228   (504) staff       (20)    12683 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/parsing/star.py
+-rw-r--r--   0 kif41228   (504) staff       (20)     2434 2022-12-08 11:26:40.000000 smartem-0.1.4/src/smartem/stage_model.py
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.862825 smartem-0.1.4/src/smartem.egg-info/
+-rw-r--r--   0 kif41228   (504) staff       (20)     1248 2023-06-20 14:05:38.000000 smartem-0.1.4/src/smartem.egg-info/PKG-INFO
+-rw-r--r--   0 kif41228   (504) staff       (20)     1286 2023-06-20 14:05:38.000000 smartem-0.1.4/src/smartem.egg-info/SOURCES.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)        1 2023-06-20 14:05:38.000000 smartem-0.1.4/src/smartem.egg-info/dependency_links.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)      372 2023-06-20 14:05:38.000000 smartem-0.1.4/src/smartem.egg-info/entry_points.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)        1 2023-05-15 12:40:38.000000 smartem-0.1.4/src/smartem.egg-info/not-zip-safe
+-rw-r--r--   0 kif41228   (504) staff       (20)       95 2023-06-20 14:05:38.000000 smartem-0.1.4/src/smartem.egg-info/requires.txt
+-rw-r--r--   0 kif41228   (504) staff       (20)        8 2023-06-20 14:05:38.000000 smartem-0.1.4/src/smartem.egg-info/top_level.txt
+drwxr-xr-x   0 kif41228   (504) staff       (20)        0 2023-06-20 14:05:38.868706 smartem-0.1.4/tests/
+-rw-r--r--   0 kif41228   (504) staff       (20)     1958 2023-06-15 09:29:29.000000 smartem-0.1.4/tests/test_stage_model.py
```

### Comparing `smartem-0.1.3/LICENSE` & `smartem-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/PKG-INFO` & `smartem-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartem
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 Requires-Python: >=3.8
 License-File: LICENSE
 
 ===============================================================
 Tools to trace cryoEM SPA processing results through EPU output
 ===============================================================
```

### Comparing `smartem-0.1.3/README.rst` & `smartem-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/setup.cfg` & `smartem-0.1.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [metadata]
 name = smartem
-version = 0.1.3
+version = 0.1.4
 description = Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 long_description = file: README.rst
 license_file = LICENSE
 
 [options]
 include_package_data = True
 install_requires = 
 	gemmi
 	matplotlib
 	xmltodict
 	mrcfile
 	pyyaml
 	psycopg2
-	sqlalchemy
+	sqlalchemy < 2.0
 	PyQt5
 	pandas
 	plotly
 	tifffile
 packages = find:
 package_dir = 
 	=src
```

### Comparing `smartem-0.1.3/src/smartem/cli/change_epu_directory.py` & `smartem-0.1.4/src/smartem/cli/change_epu_directory.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/cli/export.py` & `smartem-0.1.4/src/smartem/cli/export.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/cli/initialise.py` & `smartem-0.1.4/src/smartem/cli/initialise.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/cli/missing.py` & `smartem-0.1.4/src/smartem/cli/missing.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/cli/start.py` & `smartem-0.1.4/src/smartem/cli/start.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/cli/stop.py` & `smartem-0.1.4/src/smartem/cli/stop.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/data_model/__init__.py` & `smartem-0.1.4/src/smartem/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/data_model/construct.py` & `smartem-0.1.4/src/smartem/data_model/construct.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/data_model/extract.py` & `smartem-0.1.4/src/smartem/data_model/extract.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/data_model/structure.py` & `smartem-0.1.4/src/smartem/data_model/structure.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/data_model/torch.py` & `smartem-0.1.4/src/smartem/data_model/torch.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/gui/qt/__init__.py` & `smartem-0.1.4/src/smartem/gui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/gui/qt/component_tab.py` & `smartem-0.1.4/src/smartem/gui/qt/component_tab.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/gui/qt/display.py` & `smartem-0.1.4/src/smartem/gui/qt/display.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/gui/qt/image_utils.py` & `smartem-0.1.4/src/smartem/gui/qt/image_utils.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/gui/qt/loader.py` & `smartem-0.1.4/src/smartem/gui/qt/loader.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/gui/qt/loader_csv.py` & `smartem-0.1.4/src/smartem/gui/qt/loader_csv.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/gui/qt/plotting_utils.py` & `smartem-0.1.4/src/smartem/gui/qt/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/gui/qt/qt_style.css` & `smartem-0.1.4/src/smartem/gui/qt/qt_style.css`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/parsing/epu.py` & `smartem-0.1.4/src/smartem/parsing/epu.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/parsing/epu_vis.py` & `smartem-0.1.4/src/smartem/parsing/epu_vis.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,24 +16,31 @@
 class Atlas:
     def __init__(
         self, atlas_epu_dir: Path, sample: int, epu_data_dir: Path | None = None
     ):
         atlas_epu_dir = Path(atlas_epu_dir)
         self._epu_data_dir = epu_data_dir
         self._atlas_location = atlas_epu_dir / f"Sample{sample}" / "Atlas"
-        epu_data = parse_epu_xml(self._atlas_location / "Atlas_1.xml")
+        if (self._atlas_location / "Atlas_1.xml").is_file():
+            epu_data = parse_epu_xml(self._atlas_location / "Atlas_1.xml")
+        else:
+            epu_data = parse_epu_xml(list(self._atlas_location.glob("Atlas_*.xml"))[0])
         self._pixel_size = epu_data["pixel_size"]
         self._readout_area = epu_data["readout_area"]
         self._grid_square_positions = metadata_grid_square_positions(
             self._atlas_location / "Atlas.dm"
         )
 
     @property
     def image(self) -> np.array:
-        with mrcfile.open(self._atlas_location / "Atlas_1.mrc") as mrc:
+        if (self._atlas_location / "Atlas_1.mrc").is_file():
+            atlasf = self._atlas_location / "Atlas_1.mrc"
+        else:
+            atlasf = list(self._atlas_location.glob("Atlas_*.mrc"))[0]
+        with mrcfile.open(atlasf) as mrc:
             data = mrc.data
         return data
 
     @property
     def _grid_square_stage_locations(self) -> dict:
         return metadata_grid_square_stage(self._atlas_location / "Atlas.dm")
 
@@ -175,17 +182,15 @@
         leg = ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
         for legline, origline in zip(leg.legendHandles, lines_list):
             legline.set_picker(True)
             lines[legline] = origline
         fig.canvas.mpl_connect("motion_notify_event", hover)
         fig.canvas.mpl_connect("button_press_event", click)
         fig.canvas.mpl_connect("pick_event", on_pick)
-        fig.show()
         plt.show()
-        plt.close(fig)
 
 
 class GridSquare:
     def __init__(self, epu_dir: Path, grid_square: int, images_disc: int = 1):
         epu_dir = Path(epu_dir)
         self._id = grid_square
         self._epu_location = (
@@ -330,8 +335,7 @@
         leg = ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
         for legline, origline in zip(leg.legendHandles, lines_list):
             legline.set_picker(True)
             lines[legline] = origline
         fig.canvas.mpl_connect("motion_notify_event", hover)
         fig.canvas.mpl_connect("pick_event", on_pick)
         plt.show()
-        plt.close(fig)
```

### Comparing `smartem-0.1.3/src/smartem/parsing/export.py` & `smartem-0.1.4/src/smartem/parsing/export.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/parsing/relion_default.py` & `smartem-0.1.4/src/smartem/parsing/relion_default.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/parsing/star.py` & `smartem-0.1.4/src/smartem/parsing/star.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem/stage_model.py` & `smartem-0.1.4/src/smartem/stage_model.py`

 * *Files identical despite different names*

### Comparing `smartem-0.1.3/src/smartem.egg-info/PKG-INFO` & `smartem-0.1.4/src/smartem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartem
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tool to trace cryoEM SPA processing results through the magnification hierarchy provided by EPU
 Requires-Python: >=3.8
 License-File: LICENSE
 
 ===============================================================
 Tools to trace cryoEM SPA processing results through EPU output
 ===============================================================
```

### Comparing `smartem-0.1.3/src/smartem.egg-info/SOURCES.txt` & `smartem-0.1.4/src/smartem.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 src/smartem/gui/qt/plotting_utils.py
 src/smartem/gui/qt/qt_style.css
 src/smartem/parsing/__init__.py
 src/smartem/parsing/epu.py
 src/smartem/parsing/epu_vis.py
 src/smartem/parsing/export.py
 src/smartem/parsing/relion_default.py
-src/smartem/parsing/star.py
+src/smartem/parsing/star.py
+tests/test_stage_model.py
```

