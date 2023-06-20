# Comparing `tmp/dearwatson-0.7.7.tar.gz` & `tmp/dearwatson-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dearwatson-0.7.7.tar", last modified: Tue Jun 13 19:21:05 2023, max compression
+gzip compressed data, was "dearwatson-0.7.8.tar", last modified: Tue Jun 20 09:37:04 2023, max compression
```

## Comparing `dearwatson-0.7.7.tar` & `dearwatson-0.7.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:21:05.992714 dearwatson-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 19:20:53.000000 dearwatson-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 19:20:53.000000 dearwatson-0.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-13 19:21:05.988714 dearwatson-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-13 19:20:53.000000 dearwatson-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:21:05.988714 dearwatson-0.7.7/dearwatson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-13 19:21:05.000000 dearwatson-0.7.7/dearwatson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-13 19:21:05.000000 dearwatson-0.7.7/dearwatson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:21:05.000000 dearwatson-0.7.7/dearwatson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-13 19:21:05.000000 dearwatson-0.7.7/dearwatson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 19:21:05.000000 dearwatson-0.7.7/dearwatson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:21:05.992714 dearwatson-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-13 19:20:53.000000 dearwatson-0.7.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 19:20:53.000000 dearwatson-0.7.7/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:21:05.988714 dearwatson-0.7.7/watson/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 19:20:53.000000 dearwatson-0.7.7/watson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 19:20:53.000000 dearwatson-0.7.7/watson/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:21:05.988714 dearwatson-0.7.7/watson/data_validation_report/
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-13 19:20:53.000000 dearwatson-0.7.7/watson/data_validation_report/DvrPreparer.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-13 19:20:53.000000 dearwatson-0.7.7/watson/data_validation_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-13 19:20:53.000000 dearwatson-0.7.7/watson/neighbours.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-06-13 19:20:53.000000 dearwatson-0.7.7/watson/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:21:05.984714 dearwatson-0.7.7/watson/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:21:05.988714 dearwatson-0.7.7/watson/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-06-13 19:20:53.000000 dearwatson-0.7.7/watson/resources/images/sherlock3.png
--rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-06-13 19:20:53.000000 dearwatson-0.7.7/watson/resources/images/watson.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:21:05.988714 dearwatson-0.7.7/watson/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:20:54.000000 dearwatson-0.7.7/watson/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-13 19:20:54.000000 dearwatson-0.7.7/watson/tests/test_watson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:21:05.988714 dearwatson-0.7.7/watson/tpfplotterSub/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:20:54.000000 dearwatson-0.7.7/watson/tpfplotterSub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-06-13 19:20:55.000000 dearwatson-0.7.7/watson/tpfplotterSub/tpfplotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-06-13 19:20:55.000000 dearwatson-0.7.7/watson/tpfplotterSub/tpfplotter_py2.py
--rw-r--r--   0 runner    (1001) docker     (123)   107124 2023-06-13 19:20:54.000000 dearwatson-0.7.7/watson/watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.547575 dearwatson-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 09:36:50.000000 dearwatson-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 09:36:50.000000 dearwatson-0.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-20 09:37:04.547575 dearwatson-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-06-20 09:36:50.000000 dearwatson-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.543575 dearwatson-0.7.8/dearwatson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-20 09:37:04.000000 dearwatson-0.7.8/dearwatson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 09:37:04.000000 dearwatson-0.7.8/dearwatson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:37:04.000000 dearwatson-0.7.8/dearwatson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-20 09:37:04.000000 dearwatson-0.7.8/dearwatson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 09:37:04.000000 dearwatson-0.7.8/dearwatson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:37:04.547575 dearwatson-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-20 09:36:51.000000 dearwatson-0.7.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-20 09:36:51.000000 dearwatson-0.7.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.543575 dearwatson-0.7.8/watson/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.543575 dearwatson-0.7.8/watson/data_validation_report/
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/data_validation_report/DvrPreparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/data_validation_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.543575 dearwatson-0.7.8/watson/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.547575 dearwatson-0.7.8/watson/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/resources/images/sherlock3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/resources/images/watson.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.547575 dearwatson-0.7.8/watson/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/tests/test_watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:37:04.547575 dearwatson-0.7.8/watson/tpfplotterSub/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:36:52.000000 dearwatson-0.7.8/watson/tpfplotterSub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-06-20 09:36:52.000000 dearwatson-0.7.8/watson/tpfplotterSub/tpfplotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-06-20 09:36:52.000000 dearwatson-0.7.8/watson/tpfplotterSub/tpfplotter_py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107007 2023-06-20 09:36:51.000000 dearwatson-0.7.8/watson/watson.py
```

### Comparing `dearwatson-0.7.7/LICENSE` & `dearwatson-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.7/PKG-INFO` & `dearwatson-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.7.7
+Version: 0.7.8
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.7.7/README.md` & `dearwatson-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.7/dearwatson.egg-info/PKG-INFO` & `dearwatson-0.7.8/dearwatson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.7.7
+Version: 0.7.8
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.7.7/dearwatson.egg-info/SOURCES.txt` & `dearwatson-0.7.8/dearwatson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.7/setup.py` & `dearwatson-0.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-version = "0.7.7"
+version = "0.7.8"
 setuptools.setup(
     name="dearwatson", # Replace with your own username
     version=version,
     author="M. Dévora-Pajares",
     author_email="mdevorapajares@protonmail.com",
     description="Visual Vetting and Analysis of Transits from Space ObservatioNs",
     long_description=long_description,
```

### Comparing `dearwatson-0.7.7/watson/data_validation_report/DvrPreparer.py` & `dearwatson-0.7.8/watson/data_validation_report/DvrPreparer.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.7/watson/neighbours.py` & `dearwatson-0.7.8/watson/neighbours.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.7/watson/report.py` & `dearwatson-0.7.8/watson/report.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.7/watson/resources/images/sherlock3.png` & `dearwatson-0.7.8/watson/resources/images/sherlock3.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.7/watson/resources/images/watson.png` & `dearwatson-0.7.8/watson/resources/images/watson.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.7/watson/tests/test_watson.py` & `dearwatson-0.7.8/watson/tests/test_watson.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,79 +10,80 @@
 
 from watson.watson import Watson
 
 
 class TestsWatson(unittest.TestCase):
     def test_vetting_by_params(self):
         object_dir = TestsWatson.get_path("TIC25155310_[1,_2]")
-        vetting_dir = object_dir + "/vetting_0"
+        vetting_dir = object_dir + "/vetting_0/"
         try:
-            Watson(object_dir).vetting("TIC 25155310", 3.2899, 1327.51, 199, 6.082, [1, 2], 0.07571,
+            Watson(object_dir, vetting_dir).vetting("TIC 25155310", 3.2899, 1327.51, 199, 6.082, [1, 2], 0.07571,
                                        cadence=120, cpus=multiprocessing.cpu_count() // 2, clean=False)
             files_in_dir = os.listdir(vetting_dir)
-            assert len(files_in_dir) == 25
+            assert len(files_in_dir) == 34
         finally:
             if os.path.exists(vetting_dir):
                 shutil.rmtree(vetting_dir, ignore_errors=False)
 
     def test_vetting_by_files(self):
         object_dir = TestsWatson.get_path("TIC25155310_[1,_2]")
-        vetting_dir = object_dir + "/vetting_0"
+        vetting_dir = object_dir + "/vetting_0/"
         try:
-            Watson(object_dir).vetting("TIC 25155310", 3.2899, 1327.51, 199, 6.082, [1, 2], 0.07571,
+            Watson(object_dir, vetting_dir).vetting("TIC 25155310", 3.2899, 1327.51, 199, 6.082, [1, 2], 0.07571,
                                        a_rstar=20, cadence=120, lc_file=object_dir + "/lc.csv",
                                        lc_data_file=object_dir + "/lc_data.csv",
                                        tpfs_dir=object_dir + "/tpfs",
                                        apertures_file=object_dir + "/apertures.yaml",
                                        cpus=multiprocessing.cpu_count() // 2, clean=False)
             files_in_dir = os.listdir(vetting_dir)
             assert len(files_in_dir) == 25
         finally:
             if os.path.exists(vetting_dir):
                 shutil.rmtree(vetting_dir, ignore_errors=False)
 
     def test_fov_plots(self):
         object_dir = TestsWatson.get_path("TIC25155310_[1,_2]")
+        vetting_dir = object_dir + "/vetting_0/"
         fov_dir = object_dir + "/fov"
         os.mkdir(fov_dir)
         try:
             apertures = yaml.load(open(object_dir + "/apertures.yaml"), yaml.SafeLoader)
             apertures = apertures["sectors"]
-            Watson(object_dir).vetting_field_of_view(fov_dir, "TESS", "25155310", 120, 63.374706, -69.226593, [1, 2],
+            Watson(object_dir, vetting_dir).vetting_field_of_view(fov_dir, "TESS", "25155310", 120, 63.374706, -69.226593, [1, 2],
                                                      "tpf", apertures, multiprocessing.cpu_count() // 2)
             files_in_dir = os.listdir(fov_dir)
             assert len(files_in_dir) == 6
         finally:
             if os.path.exists(fov_dir):
                 shutil.rmtree(fov_dir, ignore_errors=False)
 
     def test_vetting_by_files_with_fov(self):
         object_dir = TestsWatson.get_path("TIC25155310_[1,_2]")
-        vetting_dir = object_dir + "/vetting_0"
+        vetting_dir = object_dir + "/vetting_0/"
         try:
-            Watson(object_dir).vetting("TIC 25155310", 3.2899, 1327.51, 199, 6.082, [1, 2], 0.07571,
+            Watson(object_dir, vetting_dir).vetting("TIC 25155310", 3.2899, 1327.51, 199, 6.082, [1, 2], 0.07571,
                                        a_rstar=20, cadence=120, lc_file=object_dir + "/lc.csv",
                                        lc_data_file=object_dir + "/lc_data.csv",
                                        tpfs_dir=object_dir + "/tpfs",
                                        apertures_file=object_dir + "/apertures.yaml",
                                        cpus=multiprocessing.cpu_count() // 2, create_fov_plots=True,
                                        cadence_fov=120, ra=63.3739396231274, dec=-69.226822697583, clean=False)
             files_in_dir = os.listdir(vetting_dir)
             assert len(files_in_dir) == 37
         finally:
             if os.path.exists(vetting_dir):
                 shutil.rmtree(vetting_dir, ignore_errors=False)
 
     def test_vetting_by_files_with_transits_list(self):
         object_dir = TestsWatson.get_path("TIC25155310_[1,_2]")
-        vetting_dir = object_dir + "/vetting_0"
+        vetting_dir = object_dir + "/vetting_0/"
         try:
             transits_list_df = pd.read_csv(object_dir + "/transits_stats.csv")
             transits_list_df = transits_list_df[transits_list_df["candidate"] == 0]
-            Watson(object_dir).vetting("TIC 25155310", 3.2899, 1327.51, 199, 6.082, [1, 2], 0.07571,
+            Watson(object_dir, vetting_dir).vetting("TIC 25155310", 3.2899, 1327.51, 199, 6.082, [1, 2], 0.07571,
                                        a_rstar=20, cadence=120, lc_file=object_dir + "/lc.csv",
                                        lc_data_file=object_dir + "/lc_data.csv",
                                        tpfs_dir=object_dir + "/tpfs",
                                        apertures_file=object_dir + "/apertures.yaml",
                                        cpus=multiprocessing.cpu_count() // 2,
                                        transits_list=transits_list_df.to_dict("list"), ra=63.3739396231274,
                                        dec=-69.226822697583, clean=False)
@@ -90,22 +91,22 @@
             assert len(files_in_dir) == 32
         finally:
             if os.path.exists(vetting_dir):
                 shutil.rmtree(vetting_dir, ignore_errors=False)
 
     def test_create_report(self):
         object_dir = TestsWatson.get_path("TIC25155310_[1,_2]")
-        vetting_dir = TestsWatson.get_path("vetting_test")
+        vetting_dir = TestsWatson.get_path("vetting_test/")
         transits_list_df = pd.read_csv(object_dir + "/transits_stats.csv")
         transits_list_df = transits_list_df[transits_list_df["candidate"] == 0]
         transits_list_df = transits_list_df[transits_list_df["depth"].notnull()]
         transits_list_df = transits_list_df[transits_list_df["t0"].notnull()]
         transits_list = numpy.array(transits_list_df.to_dict("list")["t0"])
         transits_list = transits_list[~numpy.isnan(transits_list)]
-        Watson(vetting_dir).report("TIC 25155310", 63.3739396231274, -69.226822697583, 1327.51, 3.2899, 199, 6.082,
+        Watson(vetting_dir, vetting_dir).report("TIC 25155310", 63.3739396231274, -69.226822697583, 1327.51, 3.2899, 199, 6.082,
                                    transits_list, [2, 5, 7], None, None, None, None)
         files_in_dir = os.listdir(vetting_dir)
         assert len(files_in_dir) == 20
 
     @staticmethod
     def get_path(path):
         """
```

### Comparing `dearwatson-0.7.7/watson/tpfplotterSub/tpfplotter.py` & `dearwatson-0.7.8/watson/tpfplotterSub/tpfplotter.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.7/watson/tpfplotterSub/tpfplotter_py2.py` & `dearwatson-0.7.8/watson/tpfplotterSub/tpfplotter_py2.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.7.7/watson/watson.py` & `dearwatson-0.7.8/watson/watson.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # from __future__ import print_function, absolute_import, division
 
 import logging
 import multiprocessing
+import shutil
 import traceback
-import sys
 
 from watson.data_validation_report.DvrPreparer import DvrPreparer
 
 import warnings
 from itertools import chain
 import PIL
 import batman
@@ -53,17 +53,17 @@
 
 
 class Watson:
     """
     Provides transiting candidate vetting information like centroids and spaceship motion, momentum dumps, neighbours
     curves inspection and more to give a deeper insight on the quality of the candidate signal.
     """
-    def __init__(self, object_dir):
+    def __init__(self, object_dir, output_dir):
         self.object_dir = os.getcwd() if object_dir is None else object_dir
-        self.data_dir = self.object_dir + "/"
+        self.data_dir = output_dir
 
     def vetting(self, id, period, t0, duration, depth, sectors, rp_rstar=None, a_rstar=None, cpus=None,
                 cadence=None, lc_file=None, lc_data_file=None, tpfs_dir=None, apertures_file=None,
                 create_fov_plots=False, cadence_fov=None, ra=None, dec=None, transits_list=None,
                 v=None, j=None, h=None, k=None, clean=True, transits_mask=None):
         """
         Launches the whole vetting procedure that ends up with a validation report
@@ -100,44 +100,40 @@
         logging.info("Period (d): %.2f", period)
         logging.info("Epoch (d): %.2f", t0)
         logging.info("Duration (min): %.2f", duration)
         logging.info("Depth (ppt): %.2f", depth)
         logging.info("Rp_Rstar: %.4f", rp_rstar)
         logging.info("a_Rstar: %.2f", a_rstar)
         logging.info("Sectors: %s", sectors)
+        if self.data_dir != self.object_dir and os.path.exists(self.data_dir) or os.path.isdir(self.data_dir):
+            shutil.rmtree(self.data_dir)
+        os.mkdir(self.data_dir)
         lc_builder = LcBuilder()
         if transits_mask is None:
             transits_mask = []
         if rp_rstar is None:
             rp_rstar = np.sqrt(depth / 1000)
         lc_build = None
         if lc_file is None or lc_data_file is None:
             lc_build = lc_builder.build(MissionObjectInfo(sectors, id, cadence=cadence,
                                                           initial_transit_mask=transits_mask), self.data_dir)
-            lc_build.lc_data.to_csv(self.data_dir + "/lc_data.csv")
-            lc_file = self.data_dir + "/lc.csv"
-            lc_data_file = self.data_dir + "/lc_data.csv"
+            lc_build.lc_data.to_csv(self.object_dir + "/lc_data.csv")
+            lc_file = self.object_dir + "/lc.csv"
+            lc_data_file = self.object_dir + "/lc_data.csv"
         if a_rstar is None and lc_build is None:
             raise ValueError("You need to define a_rstar if you are providing the lc_file and lc_data_file")
         if a_rstar is None:
             a_rstar = HabitabilityCalculator().calculate_semi_major_axis(period, lc_build.star_info.mass)
         if tpfs_dir is None:
-            tpfs_dir = self.data_dir + "/tpfs/"
+            tpfs_dir = self.object_dir + "/tpfs/"
         if apertures_file is None:
-            apertures_file = self.data_dir + "/apertures.yaml"
-        index = 0
-        vetting_dir = self.data_dir + "/vetting_" + str(index)
-        while os.path.exists(vetting_dir) or os.path.isdir(vetting_dir):
-            vetting_dir = self.data_dir + "/vetting_" + str(index)
-            index = index + 1
-        os.mkdir(vetting_dir)
-        self.data_dir = vetting_dir
+            apertures_file = self.object_dir + "/apertures.yaml"
         try:
             if sectors is not None:
-                DvrPreparer().retrieve(id, sectors, vetting_dir)
+                DvrPreparer().retrieve(id, sectors, self.data_dir)
             transits_list_t0s, summary_list_t0s_indexes = self.__process(id, period, t0, duration, depth, rp_rstar, a_rstar,
                                                                  cpus, lc_file, lc_data_file, tpfs_dir,
                                                                  apertures_file, create_fov_plots, cadence_fov, ra,
                                                                  dec, transits_list, transits_mask)
             self.report(id, ra, dec, t0, period, duration, depth, transits_list_t0s, summary_list_t0s_indexes,
                         v, j, h, k, os.path.exists(tpfs_dir))
             if clean:
```

