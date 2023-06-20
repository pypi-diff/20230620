# Comparing `tmp/solo_epd_loader-0.2.6.tar.gz` & `tmp/solo_epd_loader-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-2t8k6eda/solo_epd_loader-0.2.6.tar", last modified: Mon Jun 19 16:38:58 2023, max compression
+gzip compressed data, was "/home/gieseler/uni/solo/solo-epd-loader/dist/.tmp-lwq7isme/solo_epd_loader-0.2.7.tar", last modified: Tue Jun 20 12:50:57 2023, max compression
```

## Comparing `solo_epd_loader-0.2.6.tar` & `solo_epd_loader-0.2.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.250460 solo_epd_loader-0.2.6/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.6/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.6/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-19 16:38:58.250460 solo_epd_loader-0.2.6/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15847 2023-06-19 08:20:58.000000 solo_epd_loader-0.2.6/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.6/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.242460 solo_epd_loader-0.2.6/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.6/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.6/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.6/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.6/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.242460 solo_epd_loader-0.2.6/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.6/examples/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.6/examples/ws2021_fig_2d.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.6/gh2021_fig_2.png
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.6/gh2021_fig_2a.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.246460 solo_epd_loader-0.2.6/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.6/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.6/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.6/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2306 2023-06-19 16:38:58.250460 solo_epd_loader-0.2.6/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.6/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.246460 solo_epd_loader-0.2.6/solo_epd_loader/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    54968 2023-06-19 12:20:19.000000 solo_epd_loader-0.2.6/solo_epd_loader/__init__.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.246460 solo_epd_loader-0.2.6/solo_epd_loader/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.6/solo_epd_loader/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-19 16:38:58.000000 solo_epd_loader-0.2.6/solo_epd_loader/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-19 16:38:58.246460 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-19 16:38:58.000000 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      611 2023-06-19 16:38:58.000000 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-19 16:38:58.000000 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      192 2023-06-19 16:38:58.000000 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-06-19 16:38:58.000000 solo_epd_loader-0.2.6/solo_epd_loader.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.6/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.909556 solo_epd_loader-0.2.7/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.7/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.7/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-20 12:50:57.909556 solo_epd_loader-0.2.7/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    15847 2023-06-19 08:20:58.000000 solo_epd_loader-0.2.7/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:49:33.000000 solo_epd_loader-0.2.7/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.905557 solo_epd_loader-0.2.7/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.7/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2312 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.7/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      379 2022-01-11 15:35:29.000000 solo_epd_loader-0.2.7/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.7/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.905557 solo_epd_loader-0.2.7/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-01-18 13:16:32.000000 solo_epd_loader-0.2.7/examples/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    72237 2021-05-19 13:25:57.000000 solo_epd_loader-0.2.7/examples/ws2021_fig_2d.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-28 12:32:34.000000 solo_epd_loader-0.2.7/gh2021_fig_2.png
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   530502 2022-03-25 16:10:07.000000 solo_epd_loader-0.2.7/gh2021_fig_2a.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.905557 solo_epd_loader-0.2.7/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1483 2022-01-10 16:29:51.000000 solo_epd_loader-0.2.7/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.7/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.7/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2306 2023-06-20 12:50:57.909556 solo_epd_loader-0.2.7/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      666 2022-03-01 17:04:02.000000 solo_epd_loader-0.2.7/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.909556 solo_epd_loader-0.2.7/solo_epd_loader/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    55969 2023-06-20 12:40:19.000000 solo_epd_loader-0.2.7/solo_epd_loader/__init__.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.909556 solo_epd_loader-0.2.7/solo_epd_loader/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solo_epd_loader-0.2.7/solo_epd_loader/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-06-20 12:50:57.000000 solo_epd_loader-0.2.7/solo_epd_loader/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-06-20 12:50:57.909556 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    16795 2023-06-20 12:50:57.000000 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      611 2023-06-20 12:50:57.000000 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-06-20 12:50:57.000000 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-01-12 15:20:36.000000 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      192 2023-06-20 12:50:57.000000 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       16 2023-06-20 12:50:57.000000 solo_epd_loader-0.2.7/solo_epd_loader.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1308 2022-06-28 13:22:42.000000 solo_epd_loader-0.2.7/tox.ini
```

### Comparing `solo_epd_loader-0.2.6/LICENSE.rst` & `solo_epd_loader-0.2.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/PKG-INFO` & `solo_epd_loader-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo_epd_loader
-Version: 0.2.6
+Version: 0.2.7
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.2.6/README.rst` & `solo_epd_loader-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/code_of_conduct.md` & `solo_epd_loader-0.2.7/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/docs/Makefile` & `solo_epd_loader-0.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/docs/conf.py` & `solo_epd_loader-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/docs/make.bat` & `solo_epd_loader-0.2.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/examples/gh2021_fig_2.png` & `solo_epd_loader-0.2.7/examples/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/examples/ws2021_fig_2d.png` & `solo_epd_loader-0.2.7/examples/ws2021_fig_2d.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/gh2021_fig_2.png` & `solo_epd_loader-0.2.7/gh2021_fig_2.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/gh2021_fig_2a.png` & `solo_epd_loader-0.2.7/gh2021_fig_2a.png`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/licenses/LICENSE.rst` & `solo_epd_loader-0.2.7/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/licenses/TEMPLATE_LICENSE.rst` & `solo_epd_loader-0.2.7/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/setup.cfg` & `solo_epd_loader-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/setup.py` & `solo_epd_loader-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/solo_epd_loader/__init__.py` & `solo_epd_loader-0.2.7/solo_epd_loader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,15 +439,15 @@
             if level.lower() == 'l2':
                 _ = _epd_l2_download(date=tdate, path=path, sensor=sensor,
                                      viewing=tview)
     return
 
 
 def epd_load(sensor, startdate, enddate=None, level='l2', viewing=None, path=None,
-             autodownload=False, only_averages=False, contamination_threshold=2):
+             autodownload=False, only_averages=False):
     """
     Load SolO/EPD data
 
     Load-in data for Solar Orbiter/EPD energetic charged particle sensors EPT,
     HET, and STEP. Supports level 2 and low latency data provided by ESA's
     Solar Orbiter Archive. Optionally downloads missing data directly. Returns
     data as Pandas dataframe.
@@ -479,21 +479,14 @@
     autodownload : bool, optional
         If True, will try to download missing data files from SOAR, by default
         False.
     only_averages : bool, optional
         If True, will for STEP only return the averaged fluxes, and not the data
         of each of the 15 Pixels. This will reduce the memory consumption. By
         default False.
-    contamination_threshold : int or False, optional
-        >> NOT IN USE AS OF VERSION 0.2.4 <<
-        If int, mask electron data that probably is contaminated (i.e., set it
-        to nan) using an integer contamination threshold following the equation:
-        Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty
-        If False, don't alter the data at all. Only implemented for new STEP
-        data (after Oct 2021) so far. By default 2.
 
     Returns
     -------
     For EPT & HET:
         1. Pandas dataframe with proton fluxes and errors (for EPT also alpha particles) in 'particles / (s cm^2 sr MeV)'
         2. Pandas dataframe with electron fluxes and errors in 'particles / (s cm^2 sr MeV)'
         3. Dictionary with energy information for all particles:
@@ -828,24 +821,28 @@
     dependencies and cannot easily be put in the same dataframe!
     '''
 
     return df_epd_p, df_epd_e, energies_dict
 
 
 def _read_step_cdf(level, startdate, enddate=None, path=None, autodownload=False,
-                   only_averages=False, contamination_threshold=2):
+                   only_averages=False):
     """
     INPUT:
         level: 'll' or 'l2' (string)
         startdate,
         enddate:    YYYYMMDD, e.g., 20210415 (integer)
                     (if no enddate is given, 'enddate = startdate' will be set)
         path: directory in which Solar Orbiter data is/should be organized;
               e.g. '/home/userxyz/uni/solo/data/' (string)
         autodownload: if True will try to download missing data files from SOAR
+        only_averages : bool, optional
+            If True, will for STEP only return the averaged fluxes, and not the data
+            of each of the 15 Pixels. This will reduce the memory consumption. By
+            default False.
     RETURNS:
         1. Pandas dataframe with fluxes and errors in
            'particles / (s cm^2 sr MeV)'
         2. Dictionary with energy information for all particles:
             - String with energy channel info
             - Value of lower energy bin edge in MeV
             - Value of energy bin width in MeV
@@ -950,29 +947,29 @@
 
             # transform the index of the dataframe into pd_datetime
             datetimes = cdflib.cdfepoch.encode(datadf.index.values)
             datadf.index = pd.to_datetime(datetimes)
 
             datadf.index.names = ['Time']
 
-            if type(contamination_threshold) == int:
-                print("'contamination_threshold' not yet included for old STEP data (before Oct 22, 2021)!")
+            # if type(contamination_threshold) == int:
+            #     print("'contamination_threshold' not yet included for old STEP data (before Oct 22, 2021)!")
 
         elif product == 'main':
             datadf, energies_dict = _read_new_step_cdf(filelist, only_averages, contamination_threshold)
 
     '''
     Careful if adding more species - they might have different EPOCH
     dependencies and cannot easily be put in the same dataframe!
     '''
 
     return datadf, energies_dict
 
 
-def _read_new_step_cdf(files, only_averages=False, contamination_threshold=2):
+def _read_new_step_cdf(files, only_averages=False):
     """
     Function that reads in new format (since Oct 2021) STEP CDF 'files'.
     EPOCH_X dependent data is obtained as Pandas Dataframe via sunpy.
     Time-independent meta data is read in from the first cdf file via cdflib.
     """
     # read electron correction factors and meta data via cdflib
     cdf = cdflib.CDF(files[0])
@@ -1051,14 +1048,44 @@
     # df3['QUALITY_BITMASK'] = df['QUALITY_BITMASK']
     # df3['SMALL_PIXELS_FLAG'] = df['SMALL_PIXELS_FLAG']
 
     return df, meta
 
 
 def calc_electrons(df, meta, contamination_threshold=2, only_averages=False, resample=False):
+    """
+    Calulate STEP electron data from Integral and Magnet observations.
+
+    Parameters
+    ----------
+    df : Pandas DataFrame
+        DataFrame containing the original STEP data read-in with epd_load
+        (containing Integral_Fluxes and Magnet_Fluxes).
+    meta : dict
+        Dictionary of meta data like energy information provided as second output
+        of epd_load.
+    contamination_threshold : int or False/None, optional
+        If int, mask electron data that probably is contaminated (i.e., set it
+        to nan) using an integer contamination threshold following the equation:
+        Integral_Flux - Magnet_Flux > contamination_threshold * Integral_Uncertainty
+        If False, don't alter the data at all. Only implemented for new STEP
+        data (after Oct 2021) so far. By default 2.
+    only_averages : bool, optional
+        If True, will for STEP only return the averaged fluxes, and not the data
+        of each of the 15 Pixels. This will reduce the memory consumption. By
+        default False.
+    resample : str
+        Pandas-readable resampling time, e.g. '1min'
+
+    Returns
+    -------
+    df : Pandas DataFrame
+        DataFrame sutrucuted as the input DataFrame, but with additional Electron columns
+        (Flux and Uncertainity) and possibly resampled.
+    """
     df = df.copy()
 
     Electron_Flux_Mult = meta['Electron_Flux_Mult']
 
     if resample:
         # for all Integral and Magnet Uncertainties:
         col_uncertainties = df.filter(like=f'_Uncertainty_').columns.tolist()
@@ -1115,15 +1142,15 @@
                     df[f'Electron_{pix}_Flux_{i}'] = df[f'Electron_{pix}_Flux_{i}'].mask(~clean)
                     df[f'Electron_{pix}_Uncertainty_{i}'] = df[f'Electron_{pix}_Uncertainty_{i}'].mask(~clean)
 
     if contamination_threshold == 0:
         print("contamination_threshold has been set to 0. Ignoring the contamination_threshold (i.e., NOT calculating it for 0)!")
 
     if type(contamination_threshold) != int:
-        print("conatmination_threshold will only be applied if it is an integer. Otherwise only negative fluxes are removed.")
+        print("Info: contamination_threshold will only be applied if it is an integer. Otherwise only negative fluxes are removed.")
 
     # remove negative fluxes (probably not needed for masked data, but for contamination_threshold=None)
     df = df.mask(df < 0)
 
     return df
```

### Comparing `solo_epd_loader-0.2.6/solo_epd_loader.egg-info/PKG-INFO` & `solo_epd_loader-0.2.7/solo_epd_loader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solo-epd-loader
-Version: 0.2.6
+Version: 0.2.7
 Summary: Data loader for Solar Orbiter/EPD energetic charged particle sensors EPT, HET, and STEP.
 Home-page: https://github.com/jgieseler/solo-epd-loader
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solo_epd_loader-0.2.6/solo_epd_loader.egg-info/SOURCES.txt` & `solo_epd_loader-0.2.7/solo_epd_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solo_epd_loader-0.2.6/tox.ini` & `solo_epd_loader-0.2.7/tox.ini`

 * *Files identical despite different names*

