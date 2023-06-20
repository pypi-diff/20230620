# Comparing `tmp/element-calcium-imaging-0.7.3.tar.gz` & `tmp/element-calcium-imaging-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-calcium-imaging-0.7.3.tar", last modified: Fri Jun  9 05:30:34 2023, max compression
+gzip compressed data, was "element-calcium-imaging-0.7.4.tar", last modified: Tue Jun 20 15:35:16 2023, max compression
```

## Comparing `element-calcium-imaging-0.7.3.tar` & `element-calcium-imaging-0.7.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:30:34.661798 element-calcium-imaging-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 05:30:27.000000 element-calcium-imaging-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-09 05:30:34.661798 element-calcium-imaging-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-09 05:30:27.000000 element-calcium-imaging-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:30:34.657798 element-calcium-imaging-0.7.3/element_calcium_imaging/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    66523 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    63721 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/imaging_no_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    74252 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/imaging_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/imaging_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:30:34.661798 element-calcium-imaging-0.7.3/element_calcium_imaging/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/plotting/cell_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/plotting/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    25849 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/element_calcium_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:30:34.661798 element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-09 05:30:34.000000 element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-09 05:30:34.000000 element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:30:34.000000 element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-09 05:30:34.000000 element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-09 05:30:34.000000 element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 05:30:34.661798 element-calcium-imaging-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-09 05:30:28.000000 element-calcium-imaging-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:35:16.163175 element-calcium-imaging-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-20 15:35:16.163175 element-calcium-imaging-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:35:16.163175 element-calcium-imaging-0.7.4/element_calcium_imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/element_calcium_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/element_calcium_imaging/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66523 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/element_calcium_imaging/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63721 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/element_calcium_imaging/imaging_no_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74252 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/element_calcium_imaging/imaging_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/element_calcium_imaging/imaging_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:35:16.163175 element-calcium-imaging-0.7.4/element_calcium_imaging/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/element_calcium_imaging/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/element_calcium_imaging/plotting/cell_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/element_calcium_imaging/plotting/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25849 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/element_calcium_imaging/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/element_calcium_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:35:16.163175 element-calcium-imaging-0.7.4/element_calcium_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-20 15:35:15.000000 element-calcium-imaging-0.7.4/element_calcium_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-20 15:35:15.000000 element-calcium-imaging-0.7.4/element_calcium_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:35:15.000000 element-calcium-imaging-0.7.4/element_calcium_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-20 15:35:15.000000 element-calcium-imaging-0.7.4/element_calcium_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 15:35:15.000000 element-calcium-imaging-0.7.4/element_calcium_imaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:35:16.163175 element-calcium-imaging-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-20 15:35:10.000000 element-calcium-imaging-0.7.4/setup.py
```

### Comparing `element-calcium-imaging-0.7.3/LICENSE` & `element-calcium-imaging-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.3/PKG-INFO` & `element-calcium-imaging-0.7.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-calcium-imaging
-Version: 0.7.3
+Version: 0.7.4
 Summary: Calcium Imaging DataJoint Element
 Home-page: https://github.com/datajoint/element-calcium-imaging
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
@@ -80,14 +80,19 @@
   - Install [VSCode](https://code.visualstudio.com/)
   - Install the VSCode [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
   - `git clone` the codebase repository and open it in VSCode
   - Use the `Dev Containers extension` to `Reopen in Container` (More info is in the `Getting started` included with the extension.)
 
 You will know your environment has finished loading once you either see a terminal open related to `Running postStartCommand` with a final message of `Done` or the `README.md` is opened in `Preview`.
 
+Once the environment has launched, please run the following command in the terminal:
+```
+MYSQL_VER=8.0 docker compose -f docker-compose-db.yaml up --build -d
+```
+
 ### Instructions
 
 1. We recommend you start by navigating to the `notebooks` directory on the left panel and go through the `tutorial.ipynb` Jupyter notebook. Execute the cells in the notebook to begin your walk through of the tutorial.
 
 1. Once you are done, see the options available to you in the menu in the bottom-left corner. For example, in Codespace you will have an option to `Stop Current Codespace` but when running Dev Container on your own machine the equivalent option is `Reopen folder locally`. By default, GitHub will also automatically stop the Codespace after 30 minutes of inactivity.  Once the Codespace is no longer being used, we recommend deleting the Codespace.
```

### Comparing `element-calcium-imaging-0.7.3/README.md` & `element-calcium-imaging-0.7.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,12 +62,17 @@
   - Install [VSCode](https://code.visualstudio.com/)
   - Install the VSCode [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
   - `git clone` the codebase repository and open it in VSCode
   - Use the `Dev Containers extension` to `Reopen in Container` (More info is in the `Getting started` included with the extension.)
 
 You will know your environment has finished loading once you either see a terminal open related to `Running postStartCommand` with a final message of `Done` or the `README.md` is opened in `Preview`.
 
+Once the environment has launched, please run the following command in the terminal:
+```
+MYSQL_VER=8.0 docker compose -f docker-compose-db.yaml up --build -d
+```
+
 ### Instructions
 
 1. We recommend you start by navigating to the `notebooks` directory on the left panel and go through the `tutorial.ipynb` Jupyter notebook. Execute the cells in the notebook to begin your walk through of the tutorial.
 
 1. Once you are done, see the options available to you in the menu in the bottom-left corner. For example, in Codespace you will have an option to `Stop Current Codespace` but when running Dev Container on your own machine the equivalent option is `Reopen folder locally`. By default, GitHub will also automatically stop the Codespace after 30 minutes of inactivity.  Once the Codespace is no longer being used, we recommend deleting the Codespace.
```

### Comparing `element-calcium-imaging-0.7.3/element_calcium_imaging/analysis.py` & `element-calcium-imaging-0.7.4/element_calcium_imaging/analysis.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.3/element_calcium_imaging/imaging.py` & `element-calcium-imaging-0.7.4/element_calcium_imaging/imaging.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.3/element_calcium_imaging/imaging_no_curation.py` & `element-calcium-imaging-0.7.4/element_calcium_imaging/imaging_no_curation.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.3/element_calcium_imaging/imaging_preprocess.py` & `element-calcium-imaging-0.7.4/element_calcium_imaging/imaging_preprocess.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.3/element_calcium_imaging/imaging_report.py` & `element-calcium-imaging-0.7.4/element_calcium_imaging/imaging_report.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.3/element_calcium_imaging/plotting/cell_plot.py` & `element-calcium-imaging-0.7.4/element_calcium_imaging/plotting/cell_plot.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.3/element_calcium_imaging/plotting/widget.py` & `element-calcium-imaging-0.7.4/element_calcium_imaging/plotting/widget.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.3/element_calcium_imaging/scan.py` & `element-calcium-imaging-0.7.4/element_calcium_imaging/scan.py`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/PKG-INFO` & `element-calcium-imaging-0.7.4/element_calcium_imaging.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-calcium-imaging
-Version: 0.7.3
+Version: 0.7.4
 Summary: Calcium Imaging DataJoint Element
 Home-page: https://github.com/datajoint/element-calcium-imaging
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
@@ -80,14 +80,19 @@
   - Install [VSCode](https://code.visualstudio.com/)
   - Install the VSCode [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
   - `git clone` the codebase repository and open it in VSCode
   - Use the `Dev Containers extension` to `Reopen in Container` (More info is in the `Getting started` included with the extension.)
 
 You will know your environment has finished loading once you either see a terminal open related to `Running postStartCommand` with a final message of `Done` or the `README.md` is opened in `Preview`.
 
+Once the environment has launched, please run the following command in the terminal:
+```
+MYSQL_VER=8.0 docker compose -f docker-compose-db.yaml up --build -d
+```
+
 ### Instructions
 
 1. We recommend you start by navigating to the `notebooks` directory on the left panel and go through the `tutorial.ipynb` Jupyter notebook. Execute the cells in the notebook to begin your walk through of the tutorial.
 
 1. Once you are done, see the options available to you in the menu in the bottom-left corner. For example, in Codespace you will have an option to `Stop Current Codespace` but when running Dev Container on your own machine the equivalent option is `Reopen folder locally`. By default, GitHub will also automatically stop the Codespace after 30 minutes of inactivity.  Once the Codespace is no longer being used, we recommend deleting the Codespace.
```

### Comparing `element-calcium-imaging-0.7.3/element_calcium_imaging.egg-info/SOURCES.txt` & `element-calcium-imaging-0.7.4/element_calcium_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `element-calcium-imaging-0.7.3/setup.py` & `element-calcium-imaging-0.7.4/setup.py`

 * *Files identical despite different names*

