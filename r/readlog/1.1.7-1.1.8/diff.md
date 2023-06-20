# Comparing `tmp/readlog-1.1.7.tar.gz` & `tmp/readlog-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readlog-1.1.7.tar", last modified: Wed Jun  7 06:46:39 2023, max compression
+gzip compressed data, was "readlog-1.1.8.tar", last modified: Tue Jun 20 07:40:45 2023, max compression
```

## Comparing `readlog-1.1.7.tar` & `readlog-1.1.8.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 06:46:39.228189 readlog-1.1.7/
--rw-rw-rw-   0        0        0      128 2023-06-02 08:43:49.000000 readlog-1.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      849 2023-06-07 06:46:39.227189 readlog-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-06-07 06:46:18.000000 readlog-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 06:46:39.204596 readlog-1.1.7/demo/
--rw-rw-rw-   0        0        0   235181 2023-06-07 06:29:27.000000 readlog-1.1.7/demo/1_hydrate_dissociation_log.lammps
-drwxrwxrwx   0        0        0        0 2023-06-07 06:46:39.206597 readlog-1.1.7/demo/__pycache__/
--rw-rw-rw-   0        0        0     5413 2023-06-07 06:40:50.000000 readlog-1.1.7/demo/__pycache__/readlog.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2023-06-07 06:46:39.211597 readlog-1.1.7/demo/imgs/
--rw-rw-rw-   0        0        0   220194 2023-06-07 06:41:45.000000 readlog-1.1.7/demo/imgs/PotEng.png
--rw-rw-rw-   0        0        0   222242 2023-06-07 06:35:07.000000 readlog-1.1.7/demo/imgs/PotEng_incomplete.png
--rw-rw-rw-   0        0        0    80925 2023-06-02 08:38:09.000000 readlog-1.1.7/demo/log.lammps
--rw-rw-rw-   0        0        0    28861 2023-06-07 06:32:27.000000 readlog-1.1.7/demo/log_incomplete.lammps
--rw-rw-rw-   0        0        0     1272 2023-06-07 06:41:43.000000 readlog-1.1.7/demo/plot_themo.py
--rw-rw-rw-   0        0        0     3060 2023-06-07 06:40:48.000000 readlog-1.1.7/demo/readlog.py
--rw-rw-rw-   0        0        0       49 2023-05-30 13:49:56.000000 readlog-1.1.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 06:46:39.228189 readlog-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-06-07 06:42:10.000000 readlog-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:46:39.213597 readlog-1.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 06:46:39.223648 readlog-1.1.7/src/readlog.egg-info/
--rw-rw-rw-   0        0        0      849 2023-06-07 06:46:38.000000 readlog-1.1.7/src/readlog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-07 06:46:39.000000 readlog-1.1.7/src/readlog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 06:46:38.000000 readlog-1.1.7/src/readlog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-07 06:46:38.000000 readlog-1.1.7/src/readlog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 06:46:38.000000 readlog-1.1.7/src/readlog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3060 2023-06-07 06:40:48.000000 readlog-1.1.7/src/readlog.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:40:45.936527 readlog-1.1.8/
+-rw-rw-rw-   0        0        0      128 2023-06-02 08:43:49.000000 readlog-1.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      849 2023-06-20 07:40:45.935530 readlog-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-06-07 06:46:18.000000 readlog-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 07:40:45.909854 readlog-1.1.8/demo/
+-rw-rw-rw-   0        0        0   235181 2023-06-07 06:29:27.000000 readlog-1.1.8/demo/1_hydrate_dissociation_log.lammps
+drwxrwxrwx   0        0        0        0 2023-06-20 07:40:45.911620 readlog-1.1.8/demo/__pycache__/
+-rw-rw-rw-   0        0        0     5413 2023-06-07 06:40:50.000000 readlog-1.1.8/demo/__pycache__/readlog.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2023-06-20 07:40:45.920528 readlog-1.1.8/demo/imgs/
+-rw-rw-rw-   0        0        0   220194 2023-06-07 06:41:45.000000 readlog-1.1.8/demo/imgs/PotEng.png
+-rw-rw-rw-   0        0        0   222242 2023-06-07 06:35:07.000000 readlog-1.1.8/demo/imgs/PotEng_incomplete.png
+-rw-rw-rw-   0        0        0    28861 2023-06-07 06:32:27.000000 readlog-1.1.8/demo/log_incomplete.lammps
+-rw-rw-rw-   0        0        0     1272 2023-06-07 06:41:43.000000 readlog-1.1.8/demo/plot_themo.py
+-rw-rw-rw-   0        0        0     3060 2023-06-07 06:40:48.000000 readlog-1.1.8/demo/readlog.py
+-rw-rw-rw-   0        0        0       27 2023-06-20 07:38:09.000000 readlog-1.1.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:40:45.936527 readlog-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-06-20 07:40:37.000000 readlog-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:40:45.922526 readlog-1.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 07:40:45.933530 readlog-1.1.8/src/readlog.egg-info/
+-rw-rw-rw-   0        0        0      849 2023-06-20 07:40:45.000000 readlog-1.1.8/src/readlog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2023-06-20 07:40:45.000000 readlog-1.1.8/src/readlog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:40:45.000000 readlog-1.1.8/src/readlog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-20 07:40:45.000000 readlog-1.1.8/src/readlog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-20 07:40:45.000000 readlog-1.1.8/src/readlog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3060 2023-06-07 06:40:48.000000 readlog-1.1.8/src/readlog.py
```

### Comparing `readlog-1.1.7/PKG-INFO` & `readlog-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readlog
-Version: 1.1.7
+Version: 1.1.8
 Summary: Read themo info from lammps output file or log file
 Home-page: https://github.com/eastsheng/readlog
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 
 ## ReadLog
```

### Comparing `readlog-1.1.7/README.md` & `readlog-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `readlog-1.1.7/demo/1_hydrate_dissociation_log.lammps` & `readlog-1.1.8/demo/1_hydrate_dissociation_log.lammps`

 * *Files identical despite different names*

### Comparing `readlog-1.1.7/demo/__pycache__/readlog.cpython-311.pyc` & `readlog-1.1.8/demo/__pycache__/readlog.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `readlog-1.1.7/demo/imgs/PotEng.png` & `readlog-1.1.8/demo/imgs/PotEng.png`

 * *Files identical despite different names*

### Comparing `readlog-1.1.7/demo/imgs/PotEng_incomplete.png` & `readlog-1.1.8/demo/imgs/PotEng_incomplete.png`

 * *Files identical despite different names*

### Comparing `readlog-1.1.7/demo/log_incomplete.lammps` & `readlog-1.1.8/demo/log_incomplete.lammps`

 * *Files identical despite different names*

### Comparing `readlog-1.1.7/demo/plot_themo.py` & `readlog-1.1.8/demo/plot_themo.py`

 * *Files identical despite different names*

### Comparing `readlog-1.1.7/demo/readlog.py` & `readlog-1.1.8/demo/readlog.py`

 * *Files identical despite different names*

### Comparing `readlog-1.1.7/setup.py` & `readlog-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
 
 
 setup(
 name         = 'readlog',
-version      = '1.1.7',
+version      = '1.1.8',
 py_modules   = ['readlog'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
 install_requires=required,
 url          = 'https://github.com/eastsheng/readlog',
```

### Comparing `readlog-1.1.7/src/readlog.egg-info/PKG-INFO` & `readlog-1.1.8/src/readlog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readlog
-Version: 1.1.7
+Version: 1.1.8
 Summary: Read themo info from lammps output file or log file
 Home-page: https://github.com/eastsheng/readlog
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 
 ## ReadLog
```

### Comparing `readlog-1.1.7/src/readlog.py` & `readlog-1.1.8/src/readlog.py`

 * *Files identical despite different names*

