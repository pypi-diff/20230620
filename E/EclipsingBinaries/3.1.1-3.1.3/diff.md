# Comparing `tmp/EclipsingBinaries-3.1.1.tar.gz` & `tmp/EclipsingBinaries-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-3.1.1.tar", last modified: Tue Jun 20 18:59:32 2023, max compression
+gzip compressed data, was "EclipsingBinaries-3.1.3.tar", last modified: Tue Jun 20 20:39:02 2023, max compression
```

## Comparing `EclipsingBinaries-3.1.1.tar` & `EclipsingBinaries-3.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:59:32.184738 EclipsingBinaries-3.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:59:32.176737 EclipsingBinaries-3.1.1/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    24369 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-20 18:59:10.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:59:32.180737 EclipsingBinaries-3.1.1/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/multi_aperture_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:59:32.180737 EclipsingBinaries-3.1.1/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:59:32.180737 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-20 18:59:32.000000 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-20 18:59:32.000000 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:59:32.000000 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 18:59:32.000000 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 18:59:32.000000 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 18:59:32.000000 EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-20 18:59:32.184738 EclipsingBinaries-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:59:32.184738 EclipsingBinaries-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-20 18:59:16.000000 EclipsingBinaries-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    24369 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19854 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-20 20:38:32.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-20 20:39:02.000000 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-20 20:39:02.000000 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:39:02.000000 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 20:39:02.000000 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 20:39:02.000000 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 20:39:02.000000 EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 20:39:02.220020 EclipsingBinaries-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-20 20:38:38.000000 EclipsingBinaries-3.1.3/setup.py
```

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/IRAF_Reduction.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/apass.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/apass.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
     :param pipeline: True if pipeline, False if not
     :param folder_path: folder path for saving RADEC files
     :param obj_name: object name for saving RADEC files
 
     :return: None but saves the RADEC files to user specified locations
     """
     filters = ["B", "V", "R", "T"]
-    header = "#RA in decimal or sexagesimal HOURS\n " \
+    header = "#RA in decimal or sexagesimal HOURS\n" \
              "#Dec in decimal or sexagesimal DEGREES\n" \
              "#Ref Star=0,1,missing (0=target star, 1=ref star, missing->first ap=target, others=ref)\n" \
              "#Centroid=0,1,missing (0=do not centroid, 1=centroid, missing=centroid)\n" \
              "#Apparent Magnitude or missing (value = apparent magnitude, or value > 99 or missing = no mag info)\n" \
              "#Add one comma separated line per aperture in the following format:\n"
     header += "#RA, Dec, Ref Star, Centroid, Magnitude\n"
     header += str(conversion([ra])[0]) + ", " + str(conversion([dec])[0]) + ", 0, 1, 99.999\n"
```

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_B.txt` & `EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_R.txt` & `EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_V.txt` & `EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/examples/test_minimums.txt` & `EclipsingBinaries-3.1.3/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/find_min.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/gaia.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/menu.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/multi_aperture_photometry.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/multi_aperture_photometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Analyze images using aperture photometry within Python and not with Astro ImageJ (AIJ)
 
 Author: Kyle Koeller
 Created: 05/07/2023
-Last Updated: 06/18/2023
+Last Updated: 06/20/2023
 """
 
 # Python imports
 import numpy as np
 import pandas as pd
 from pathlib import Path
 import matplotlib.pyplot as plt
@@ -278,28 +278,34 @@
         # find the number of pixels used to estimate the sky background
         n_b_mask_comp = comparison_annulus.to_mask(method="center")
         n_b_comp = np.sum(n_b_mask_comp)
 
         n_b_mask_tar = target_annulus.to_mask(method="center")
         n_b_tar = np.sum(n_b_mask_tar.data)
 
-        # find the number of pixels used in the aperture
-        n_pix_mask_comp = comparison_aperture.to_mask(method="center")
-        n_pix_comp = np.sum(n_pix_mask_comp)
+        """
+        # find the number of pixels used in the aperture if the radius of the apertures is in arcseconds not pixels
+        focal_length = 4114  # mm
+        pixel_size = 9  # microns
+        pixel_size = pixel_size * 10 ** -3  # mm
+        ap_area = np.pi * aperture_radius.area**2  # area of the aperture in mm^2
+        plate_scale = 1/focal_length  # rad/mm
+        plate_scale = plate_scale * 206265  # arcsec/mm
+        n_pix = ap_area / (plate_scale * pixel_size)**2  # number of pixels in the aperture
+        """
 
-        n_pix_tar = target_aperture.to_mask(method="center")
-        n_pix_tar = np.sum(n_pix_tar)
+        n_pix = np.pi * aperture_radius**2  # number of pixels in the aperture
 
         # Calculate the total noise
         sigma_f = 0.289  # quoted from Collins 2017 https://iopscience.iop.org/article/10.3847/1538-3881/153/2/77/pdf
         F_s = 0.01  # number of sky background counts per pixel in ADU
 
-        N_comp = np.sqrt(gain * comparison_flx + n_pix_comp * (1 + (n_pix_comp / n_b_comp)) *
+        N_comp = np.sqrt(gain * comparison_flx + n_pix * (1 + (n_pix_comp / n_b_comp)) *
                          (gain * F_s + F_dark + read_noise ** 2 + gain ** 2 + sigma_f ** 2)) / gain
-        N_tar = np.sqrt(gain * target_flx + n_pix_tar * (1 + (n_pix_tar / n_b_tar)) *
+        N_tar = np.sqrt(gain * target_flx + n_pix * (1 + (n_pix_tar / n_b_tar)) *
                         (gain * F_s + F_dark + read_noise ** 2 + gain ** 2 + sigma_f ** 2)) / gain
 
         # calculate the total comparison ensemble noise
         N_e_comp = np.sqrt(np.sum(N_comp ** 2))
 
         rel_flux_err = (rel_flx_T1/rel_flux_comp)*np.sqrt((N_tar**2/target_flx**2) +
                                                           (N_e_comp**2/sum(comparison_flx)**2))
```

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/pipeline.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/pipeline.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/tests/test_OC_plot.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-3.1.3/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 3.1.1
+Version: 3.1.3
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-3.1.1/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-3.1.3/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/LICENSE` & `EclipsingBinaries-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/PKG-INFO` & `EclipsingBinaries-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 3.1.1
+Version: 3.1.3
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-3.1.1/README.md` & `EclipsingBinaries-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.1.1/setup.py` & `EclipsingBinaries-3.1.3/setup.py`

 * *Files identical despite different names*

