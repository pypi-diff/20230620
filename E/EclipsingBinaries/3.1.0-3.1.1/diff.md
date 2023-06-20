# Comparing `tmp/EclipsingBinaries-3.1.0.tar.gz` & `tmp/EclipsingBinaries-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-3.1.0.tar", last modified: Sun Jun 18 20:32:29 2023, max compression
+gzip compressed data, was "EclipsingBinaries-3.1.1.tar", last modified: Tue Jun 20 18:59:32 2023, max compression
```

## Comparing `EclipsingBinaries-3.1.0.tar` & `EclipsingBinaries-3.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:32:29.411487 EclipsingBinaries-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:32:29.407487 EclipsingBinaries-3.1.0/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    24369 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:32:29.411487 EclipsingBinaries-3.1.0/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/multi_aperture_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:32:29.411487 EclipsingBinaries-3.1.0/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:32:29.411487 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-06-18 20:32:29.000000 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-18 20:32:29.000000 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:32:29.000000 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-18 20:32:29.000000 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-18 20:32:29.000000 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-18 20:32:29.000000 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-06-18 20:32:29.411487 EclipsingBinaries-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 20:32:29.411487 EclipsingBinaries-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:59:32.184738 EclipsingBinaries-3.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:59:32.176737 EclipsingBinaries-3.1.1/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    24369 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:59:32.180737 EclipsingBinaries-3.1.1/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:59:32.180737 EclipsingBinaries-3.1.1/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:59:32.180737 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-20 18:59:32.000000 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-20 18:59:32.000000 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:59:32.000000 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 18:59:32.000000 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 18:59:32.000000 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 18:59:32.000000 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-20 18:59:32.184738 EclipsingBinaries-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:59:32.184738 EclipsingBinaries-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/setup.py
```

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/IRAF_Reduction.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/apass.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/apass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Combines all APASS programs that were originally separate on GitHub for an easy editing and less to load per file.
 
 Author: Kyle Koeller
 Created: 12/26/2022
-Last Updated: 06/17/2023
+Last Updated: 06/20/2023
 """
 
 from astroquery.vizier import Vizier
 import numpy as np
 import pandas as pd
 
 import astropy.units as u
@@ -29,15 +29,15 @@
 
 
 # turn off this warning that just tells the user,
 # "The warning raised when the contents of the FITS header have been modified to be standards compliant."
 warnings.filterwarnings("ignore", category=wcs.FITSFixedWarning)
 
 
-def comparison_selector(ra, dec, pipeline, folder_path, obj_name):
+def comparison_selector(ra="", dec="", pipeline=False, folder_path="", obj_name=""):
     """
     This code compares AIJ found stars (given an RA and DEC) to APASS stars to get their respective Johnson B, V, and
     Cousins R values and their respective errors.
 
     This code is not 100% accurate and will still need the human eye to compare the final list to the AIJ given list. As
     this code can only get down to such an accuracy to be effective in gathering stars to be usable.
 
@@ -45,31 +45,39 @@
     :param dec: The declination of the target
     :param pipeline: The pipeline that is being used
     :param folder_path: The path of the folder where the images are going to
     :param obj_name: The name of the target object
 
     :return: A list of stars that are the most likely to be on the AIJ list of stars
     """
-
-    apass_file, input_ra, input_dec, T_list = cousins_r(ra, dec, pipeline, folder_path, obj_name)
-    df = pd.read_csv(apass_file, header=None, skiprows=[0], sep="\t")
-
-    print("Finished Saving\n\n")
-    print("The output file you have entered has RA and DEC for stars and their B, V, Cousins R, and TESS T magnitudes "
-          "with their respective errors.\n")
-
-    create_radec(df, input_ra, input_dec, T_list, pipeline, folder_path, obj_name)
-
+    
     if not pipeline:
+        apass_file, input_ra, input_dec, T_list = cousins_r()
+        df = pd.read_csv(apass_file, header=None, skiprows=[0], sep="\t")
+    
+        print("Finished Saving\n\n")
+        print("The output file you have entered has RA and DEC for stars and their B, V, Cousins R, and TESS T magnitudes "
+              "with their respective errors.\n")
+    
+        create_radec(df, input_ra, input_dec, T_list, pipeline, folder_path, obj_name)
+
         overlay(df, input_ra, input_dec)
     else:
-        pass
+        apass_file, input_ra, input_dec, T_list = cousins_r(ra, dec, pipeline, folder_path, obj_name)
+        df = pd.read_csv(apass_file, header=None, skiprows=[0], sep="\t")
 
+        print("Finished Saving\n\n")
+        print(
+            "The output file you have entered has RA and DEC for stars and their B, V, Cousins R, and TESS T magnitudes "
+            "with their respective errors.\n")
 
-def cousins_r(ra, dec, pipeline, folder_path, obj_name):
+        create_radec(df, input_ra, input_dec, T_list, pipeline, folder_path, obj_name)
+
+
+def cousins_r(ra="", dec="", pipeline=False, folder_path="", obj_name=""):
     """
     Calculates the Cousins R_c value for a given B, V, g', and r' from APASS
 
     :param ra: The right ascension of the target
     :param dec: The declination of the target
     :param pipeline: The pipeline that is being used
     :param folder_path: The path of the folder where the images are going to
@@ -79,16 +87,19 @@
     """
     # predefined values DO NOT change
     alpha = 0.278
     e_alpha = 0.016
     beta = 1.321
     e_beta = 0.03
     gamma = 0.219
-
-    input_file, input_ra, input_dec = catalog_finder(ra, dec, pipeline, folder_path, obj_name)
+    
+    if not pipeline:
+        input_file, input_ra, input_dec = catalog_finder(ra, dec, pipeline, folder_path, obj_name)
+    else:
+        input_file, input_ra, input_dec = catalog_finder()
     df = pd.read_csv(input_file, header=None, skiprows=[0], sep=",")
 
     # writes the columns from the input file
     try:
         # this try except function checks whether there are just enough columns in the file being loaded and tells
         # the user what they need to do in order to get the correct columns
         ra = df[0]
@@ -157,15 +168,15 @@
     # noinspection PyTypeChecker
     final.to_csv(output_file, index=True, sep="\t")
     print("\nCompleted Save.\n")
 
     return output_file, input_ra, input_dec, T_list
 
 
-def catalog_finder(ra, dec, pipeline, folder_path, obj_name):
+def catalog_finder(ra="", dec="", pipeline=False, folder_path="", obj_name=""):
     """
     This looks at a region of the sky at the decimal coordinates of an object and gathers the "column" data with
     "column filters"
     You can change the columns or the column filters to whatever you like, I have these set as they are because of the
     telescope that was used (Rooftop)
 
     I also set the width of the search radius to larger than what you would actually see in the field of view of any
```

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_B.txt` & `EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_R.txt` & `EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_V.txt` & `EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_minimums.txt` & `EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/find_min.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/gaia.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/menu.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/multi_aperture_photometry.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/multi_aperture_photometry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Analyze images using aperture photometry within Python and not with Astro ImageJ (AIJ)
 
 Author: Kyle Koeller
 Created: 05/07/2023
-Last Updated: 06/12/2023
+Last Updated: 06/18/2023
 """
 
 # Python imports
 import numpy as np
 import pandas as pd
 from pathlib import Path
 import matplotlib.pyplot as plt
@@ -20,40 +20,58 @@
 from astropy.io import fits
 # from astropy.nddata import CCDData
 # from astropy.stats import sigma_clipped_stats
 from photutils.aperture import CircularAperture, CircularAnnulus, aperture_photometry, ApertureStats
 from astropy.wcs import WCS
 import astropy.units as u
 from astropy import wcs
+
 # from astropy.visualization import ZScaleInterval
 
 # turn off this warning that just tells the user,
 # "The warning raised when the contents of the FITS header have been modified to be standards compliant."
 warnings.filterwarnings("ignore", category=wcs.FITSFixedWarning)
 
 
-def main():
-    # path = input("Please enter a file pathway (i.e. C:\\folder1\\folder2\\[raw]) to where the reduced images are or type "
-    #             "the word 'Close' to leave: ")
+def main(path="", pipeline=False):
+    """
+    Main function for aperture photometry
 
-    path = "D:\\BSUO data\\2022.09.29-reduced"  # For testing purposes
+    Parameters
+    ----------
+    path : str
+        Path to the folder containing the images.
 
-    if path.lower() == "close":
-        exit()
+    pipeline : bool
+        If True, then the program is being run from the pipeline and will not ask for user input.
+    Returns
+    -------
+    N/A
+    """
+    if not pipeline:
+        path = input("Please enter a file pathway (i.e. C:\\folder1\\folder2\\[raw]) to where the reduced images are or type "
+                     "the word 'Close' to leave: ")
+
+        # path = "D:\\BSUO data\\2022.09.29-reduced"  # For testing purposes
+
+        if path.lower() == "close":
+            exit()
+    else:
+        pass
 
     science_imagetyp = 'LIGHT'
 
     images_path = Path(path)
     files = ccdp.ImageFileCollection(images_path)
     image_list = files.files_filtered(imagetyp=science_imagetyp, filter="Empty/V")
 
-    single_MAP(image_list, images_path)
+    multiple_AP(image_list, images_path)
 
 
-def single_MAP(image_list, path):
+def single_AP(image_list, path):
     """
     Perform multi-aperture photometry on a list of images for a single target
 
     Parameters
     ----------
     path : path
         Path to the folder containing the images.
@@ -126,16 +144,16 @@
         target_bkg = ApertureStats(image_data, target_aperture, local_bkg=target_bkg_mean).sum
 
         # Calculate the background subtracted counts
         target_flx = target_phot_table['aperture_sum'] - target_bkg
 
         target_flx_err = np.sqrt(target_phot_table['aperture_sum'])
 
-        target_magnitude = 25 - 2.5*np.log10(target_flx)
-        target_magnitude_error = (2.5/np.log(10)) * (target_flx_err/target_flx)
+        target_magnitude = 25 - 2.5 * np.log10(target_flx)
+        target_magnitude_error = (2.5 / np.log(10)) * (target_flx_err / target_flx)
 
         # Append the calculated magnitude and error to the lists
         magnitudes.append(target_magnitude[0])
         mag_err.append(target_magnitude_error[0])
 
         # Clear the axis
         ax.clear()
@@ -155,41 +173,29 @@
         time.sleep(0.1)
         plt.pause(0.0001)
 
     # Disable interactive mode
     plt.ioff()
 
 
-def multiple_MAP(image_list, path):
+def multiple_AP(image_list, path):
     """
-    Perform multi-aperture photometry on a list of images for multiple targets
+    Perform multi-aperture photometry on a list of images for a single target
+
     Parameters
     ----------
-    image_list
-    path
+    path : path
+        Path to the folder containing the images.
+    image_list : table
+        Table of images to perform aperture photometry on.
 
     Returns
     -------
-
-    """
-
+    None
     """
-        Perform multi-aperture photometry on a list of images for a single target
-
-        Parameters
-        ----------
-        path : path
-            Path to the folder containing the images.
-        image_list : table
-            Table of images to perform aperture photometry on.
-
-        Returns
-        -------
-        None
-        """
 
     # Define the aperture parameters
     # Define the aperture and annulus radii
     aperture_radius = 20
     annulus_radii = (30, 50)
 
     read_noise = 10.83  # * u.electron  # gathered from fits headers manually
@@ -253,51 +259,60 @@
             comparison_bkg_mean = 0
 
         target_bkg = ApertureStats(image_data, target_aperture, local_bkg=target_bkg_mean).sum
         comparison_bkg = ApertureStats(image_data, comparison_aperture, local_bkg=comparison_bkg_mean).sum
 
         # Calculate the background subtracted counts
         target_flx = target_phot_table['aperture_sum'] - target_bkg
+        target_flux_err = np.sqrt(target_phot_table['aperture_sum'] + target_aperture.area * read_noise**2)
         comparison_flx = comparison_phot_table['aperture_sum'] - comparison_bkg
+        comp_flux_err = np.sqrt(comparison_phot_table['aperture_sum'] + comparison_aperture.area * read_noise ** 2)
 
-        # calculate the relative flux for each comparison star
+        # calculate the relative flux for each comparison star and the target star
         rel_flx_T1 = target_flx / sum(comparison_flx)
         count = 0
         for i in comparison_flx:
             if i == comparison_flx[count]:
                 rel_flux_comp = i / (sum(comparison_flx) - i)
             count += 1
 
         # find the number of pixels used to estimate the sky background
         n_b_mask_comp = comparison_annulus.to_mask(method="center")
         n_b_comp = np.sum(n_b_mask_comp)
 
         n_b_mask_tar = target_annulus.to_mask(method="center")
-        n_b_tar = np.sum(n_b_mask_tar)
+        n_b_tar = np.sum(n_b_mask_tar.data)
 
         # find the number of pixels used in the aperture
         n_pix_mask_comp = comparison_aperture.to_mask(method="center")
         n_pix_comp = np.sum(n_pix_mask_comp)
 
         n_pix_tar = target_aperture.to_mask(method="center")
         n_pix_tar = np.sum(n_pix_tar)
 
         # Calculate the total noise
         sigma_f = 0.289  # quoted from Collins 2017 https://iopscience.iop.org/article/10.3847/1538-3881/153/2/77/pdf
         F_s = 0.01  # number of sky background counts per pixel in ADU
 
-        N_comp = np.sqrt(gain*comparison_flx + n_pix_comp*(1 + (n_pix_comp/n_b_comp))*(gain*F_s + F_dark + read_noise**2 + gain**2 + sigma_f**2)) / gain
-        N_tar = np.sqrt(gain*target_flx + n_pix_tar*(1 + (n_pix_tar/n_b_tar))*(gain*F_s + F_dark + read_noise**2 + gain**2 + sigma_f**2)) / gain
+        N_comp = np.sqrt(gain * comparison_flx + n_pix_comp * (1 + (n_pix_comp / n_b_comp)) *
+                         (gain * F_s + F_dark + read_noise ** 2 + gain ** 2 + sigma_f ** 2)) / gain
+        N_tar = np.sqrt(gain * target_flx + n_pix_tar * (1 + (n_pix_tar / n_b_tar)) *
+                        (gain * F_s + F_dark + read_noise ** 2 + gain ** 2 + sigma_f ** 2)) / gain
 
         # calculate the total comparison ensemble noise
-        N_e_comp = np.sqrt(np.sum(N_comp**2))
-        
+        N_e_comp = np.sqrt(np.sum(N_comp ** 2))
+
+        rel_flux_err = (rel_flx_T1/rel_flux_comp)*np.sqrt((N_tar**2/target_flx**2) +
+                                                          (N_e_comp**2/sum(comparison_flx)**2))
+
         # calculate the total target magnitude and error
-        target_magnitude = [0]
-        target_magnitude_error = [0]
+        target_magnitude = -np.log(sum(2.512**(magnitudes_comp)))/np.log(2.512) - \
+                           (2.5*np.log10(target_bkg/sum(comparison_bkg)))
+        target_magnitude_error = 2.5*np.log10(1 + np.sqrt(target_flux_err**2/target_bkg**2) +
+                                              (sum(comp_flux_err)**2/sum(comparison_bkg)**2))
 
         # Append the calculated magnitude and error to the lists
         magnitudes.append(target_magnitude[0])
         mag_err.append(target_magnitude_error[0])
 
         # Clear the axis
         ax.clear()
```

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/pipeline.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/pipeline.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/tests/test_OC_plot.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-3.1.1/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 3.1.0
+Version: 3.1.1
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
-[![Python 3.8, 3.9, 3.10](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml/badge.svg)](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml)
+[![Python OS 3.8, 3.9, 3.10](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/ci_tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/eclipsingbinaries/badge/?version=latest)](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/EclipsingBinaries.svg)](https://badge.fury.io/py/EclipsingBinaries)
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
```

### Comparing `EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/LICENSE` & `EclipsingBinaries-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.0/PKG-INFO` & `EclipsingBinaries-3.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 3.1.0
+Version: 3.1.1
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
-[![Python 3.8, 3.9, 3.10](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml/badge.svg)](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml)
+[![Python OS 3.8, 3.9, 3.10](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/ci_tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/eclipsingbinaries/badge/?version=latest)](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/EclipsingBinaries.svg)](https://badge.fury.io/py/EclipsingBinaries)
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
```

### Comparing `EclipsingBinaries-3.1.0/README.md` & `EclipsingBinaries-3.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Python 3.8, 3.9, 3.10](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml/badge.svg)](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml)
+[![Python OS 3.8, 3.9, 3.10](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/ci_tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/eclipsingbinaries/badge/?version=latest)](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/EclipsingBinaries.svg)](https://badge.fury.io/py/EclipsingBinaries)
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
```

### Comparing `EclipsingBinaries-3.1.0/setup.py` & `EclipsingBinaries-3.1.1/setup.py`

 * *Files identical despite different names*

