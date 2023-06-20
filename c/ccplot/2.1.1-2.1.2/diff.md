# Comparing `tmp/ccplot-2.1.1.tar.gz` & `tmp/ccplot-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccplot-2.1.1.tar", last modified: Sun Jan 23 17:39:01 2022, max compression
+gzip compressed data, was "ccplot-2.1.2.tar", last modified: Tue Jun 20 12:56:06 2023, max compression
```

## Comparing `ccplot-2.1.1.tar` & `ccplot-2.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-01-23 17:39:01.497893 ccplot-2.1.1/
--rw-r--r--   0 peter     (1000) peter     (1000)     1345 2022-01-23 17:31:03.000000 ccplot-2.1.1/LICENSE
--rw-r--r--   0 peter     (1000) peter     (1000)      201 2022-01-23 17:31:03.000000 ccplot-2.1.1/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)     5166 2022-01-23 17:31:03.000000 ccplot-2.1.1/NEWS
--rw-r--r--   0 peter     (1000) peter     (1000)     1021 2022-01-23 17:39:01.497893 ccplot-2.1.1/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     1416 2022-01-23 17:31:03.000000 ccplot-2.1.1/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-01-23 17:39:01.497893 ccplot-2.1.1/bin/
--rwxr-xr-x   0 peter     (1000) peter     (1000)    80826 2022-01-23 17:31:03.000000 ccplot-2.1.1/bin/ccplot
--rw-r--r--   0 peter     (1000) peter     (1000)       33 2022-01-23 17:31:03.000000 ccplot-2.1.1/bin/ccplot.bat
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-01-23 17:39:01.497893 ccplot-2.1.1/ccplot/
--rw-r--r--   0 peter     (1000) peter     (1000)        0 2022-01-23 17:31:03.000000 ccplot-2.1.1/ccplot/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2161 2022-01-23 17:31:03.000000 ccplot-2.1.1/ccplot/algorithms.pyx
--rw-r--r--   0 peter     (1000) peter     (1000)     1552 2022-01-23 17:31:03.000000 ccplot-2.1.1/ccplot/autostr.py
--rw-r--r--   0 peter     (1000) peter     (1000)    12928 2022-01-23 17:31:03.000000 ccplot-2.1.1/ccplot/cctk.c
--rw-r--r--   0 peter     (1000) peter     (1000)      430 2022-01-23 17:31:03.000000 ccplot-2.1.1/ccplot/config.py
--rw-r--r--   0 peter     (1000) peter     (1000)    16756 2022-01-23 17:31:03.000000 ccplot-2.1.1/ccplot/hdf.pyx
--rw-r--r--   0 peter     (1000) peter     (1000)    15343 2022-01-23 17:31:03.000000 ccplot-2.1.1/ccplot/hdfeos.pyx
--rw-r--r--   0 peter     (1000) peter     (1000)     4865 2022-01-23 17:31:03.000000 ccplot-2.1.1/ccplot/utils.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-01-23 17:39:01.497893 ccplot-2.1.1/ccplot.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     1021 2022-01-23 17:39:01.000000 ccplot-2.1.1/ccplot.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      649 2022-01-23 17:39:01.000000 ccplot-2.1.1/ccplot.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2022-01-23 17:39:01.000000 ccplot-2.1.1/ccplot.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       68 2022-01-23 17:39:01.000000 ccplot-2.1.1/ccplot.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        7 2022-01-23 17:39:01.000000 ccplot-2.1.1/ccplot.egg-info/top_level.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-01-23 17:39:01.497893 ccplot-2.1.1/cmap/
--rw-r--r--   0 peter     (1000) peter     (1000)      556 2022-01-23 17:31:03.000000 ccplot-2.1.1/cmap/calipso-backscatter.cmap
--rw-r--r--   0 peter     (1000) peter     (1000)      261 2022-01-23 17:31:03.000000 ccplot-2.1.1/cmap/calipso-cratio.cmap
--rw-r--r--   0 peter     (1000) peter     (1000)      193 2022-01-23 17:31:03.000000 ccplot-2.1.1/cmap/calipso-dratio.cmap
--rw-r--r--   0 peter     (1000) peter     (1000)     2588 2022-01-23 17:31:03.000000 ccplot-2.1.1/cmap/calipso-temperature.cmap
--rw-r--r--   0 peter     (1000) peter     (1000)      442 2022-01-23 17:31:03.000000 ccplot-2.1.1/cmap/cloudsat-reflectivity.cmap
--rw-r--r--   0 peter     (1000) peter     (1000)      800 2022-01-23 17:31:03.000000 ccplot-2.1.1/cmap/modis-reflectance.cmap
--rw-r--r--   0 peter     (1000) peter     (1000)     2602 2022-01-23 17:31:03.000000 ccplot-2.1.1/cmap/modis-temperature.cmap
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-01-23 17:39:01.497893 ccplot-2.1.1/man/
--rw-r--r--   0 peter     (1000) peter     (1000)    11270 2022-01-23 17:31:03.000000 ccplot-2.1.1/man/ccplot.1
--rw-r--r--   0 peter     (1000) peter     (1000)    17173 2022-01-23 17:31:03.000000 ccplot-2.1.1/man/ccplot.1.html
--rw-r--r--   0 peter     (1000) peter     (1000)    10863 2022-01-23 17:31:03.000000 ccplot-2.1.1/man/ccplot.1.ronn
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2022-01-23 17:39:01.497893 ccplot-2.1.1/setup.cfg
--rwxr-xr-x   0 peter     (1000) peter     (1000)     4001 2022-01-23 17:31:03.000000 ccplot-2.1.1/setup.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-01-23 17:39:01.497893 ccplot-2.1.1/test/
--rwxr-xr-x   0 peter     (1000) peter     (1000)     2256 2022-01-23 17:31:03.000000 ccplot-2.1.1/test/imgcompare
--rw-r--r--   0 peter     (1000) peter     (1000)     2092 2022-01-23 17:31:03.000000 ccplot-2.1.1/test/libtest.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)     5275 2022-01-23 17:31:03.000000 ccplot-2.1.1/test/test.sh
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:56:06.726887 ccplot-2.1.2/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1345 2023-06-20 12:44:34.000000 ccplot-2.1.2/LICENSE
+-rw-r--r--   0 peter     (1000) peter     (1000)      201 2023-06-20 12:44:34.000000 ccplot-2.1.2/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)     5245 2023-06-20 12:44:34.000000 ccplot-2.1.2/NEWS
+-rw-r--r--   0 peter     (1000) peter     (1000)     1021 2023-06-20 12:56:06.726887 ccplot-2.1.2/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     1416 2023-06-20 12:44:34.000000 ccplot-2.1.2/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:56:06.726887 ccplot-2.1.2/bin/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)    80826 2023-06-20 12:44:34.000000 ccplot-2.1.2/bin/ccplot
+-rw-r--r--   0 peter     (1000) peter     (1000)       33 2023-06-20 12:44:34.000000 ccplot-2.1.2/bin/ccplot.bat
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:56:06.726887 ccplot-2.1.2/ccplot/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2023-06-20 12:44:34.000000 ccplot-2.1.2/ccplot/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2161 2023-06-20 12:44:34.000000 ccplot-2.1.2/ccplot/algorithms.pyx
+-rw-r--r--   0 peter     (1000) peter     (1000)     1552 2023-06-20 12:44:34.000000 ccplot-2.1.2/ccplot/autostr.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    12928 2023-06-20 12:44:34.000000 ccplot-2.1.2/ccplot/cctk.c
+-rw-r--r--   0 peter     (1000) peter     (1000)      430 2023-06-20 12:44:34.000000 ccplot-2.1.2/ccplot/config.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    16756 2023-06-20 12:44:34.000000 ccplot-2.1.2/ccplot/hdf.pyx
+-rw-r--r--   0 peter     (1000) peter     (1000)    15343 2023-06-20 12:44:34.000000 ccplot-2.1.2/ccplot/hdfeos.pyx
+-rw-r--r--   0 peter     (1000) peter     (1000)     4865 2023-06-20 12:44:34.000000 ccplot-2.1.2/ccplot/utils.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:56:06.726887 ccplot-2.1.2/ccplot.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1021 2023-06-20 12:56:06.000000 ccplot-2.1.2/ccplot.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      649 2023-06-20 12:56:06.000000 ccplot-2.1.2/ccplot.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-06-20 12:56:06.000000 ccplot-2.1.2/ccplot.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       68 2023-06-20 12:56:06.000000 ccplot-2.1.2/ccplot.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        7 2023-06-20 12:56:06.000000 ccplot-2.1.2/ccplot.egg-info/top_level.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:56:06.726887 ccplot-2.1.2/cmap/
+-rw-r--r--   0 peter     (1000) peter     (1000)      556 2023-06-20 12:44:34.000000 ccplot-2.1.2/cmap/calipso-backscatter.cmap
+-rw-r--r--   0 peter     (1000) peter     (1000)      261 2023-06-20 12:44:34.000000 ccplot-2.1.2/cmap/calipso-cratio.cmap
+-rw-r--r--   0 peter     (1000) peter     (1000)      193 2023-06-20 12:44:34.000000 ccplot-2.1.2/cmap/calipso-dratio.cmap
+-rw-r--r--   0 peter     (1000) peter     (1000)     2588 2023-06-20 12:44:34.000000 ccplot-2.1.2/cmap/calipso-temperature.cmap
+-rw-r--r--   0 peter     (1000) peter     (1000)      442 2023-06-20 12:44:34.000000 ccplot-2.1.2/cmap/cloudsat-reflectivity.cmap
+-rw-r--r--   0 peter     (1000) peter     (1000)      800 2023-06-20 12:44:34.000000 ccplot-2.1.2/cmap/modis-reflectance.cmap
+-rw-r--r--   0 peter     (1000) peter     (1000)     2602 2023-06-20 12:44:34.000000 ccplot-2.1.2/cmap/modis-temperature.cmap
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:56:06.726887 ccplot-2.1.2/man/
+-rw-r--r--   0 peter     (1000) peter     (1000)    11270 2023-06-20 12:44:34.000000 ccplot-2.1.2/man/ccplot.1
+-rw-r--r--   0 peter     (1000) peter     (1000)    17173 2023-06-20 12:44:34.000000 ccplot-2.1.2/man/ccplot.1.html
+-rw-r--r--   0 peter     (1000) peter     (1000)    10863 2023-06-20 12:44:34.000000 ccplot-2.1.2/man/ccplot.1.ronn
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-06-20 12:56:06.726887 ccplot-2.1.2/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     4008 2023-06-20 12:44:34.000000 ccplot-2.1.2/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-06-20 12:56:06.726887 ccplot-2.1.2/test/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     2256 2023-06-20 12:44:34.000000 ccplot-2.1.2/test/imgcompare
+-rw-r--r--   0 peter     (1000) peter     (1000)     2092 2023-06-20 12:44:34.000000 ccplot-2.1.2/test/libtest.sh
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     5275 2023-06-20 12:44:34.000000 ccplot-2.1.2/test/test.sh
```

### Comparing `ccplot-2.1.1/LICENSE` & `ccplot-2.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2009-2021 Peter Kuma
+Copyright (c) 2009-2023 Peter Kuma
 
 This software is provided under the terms of a 2-clause BSD licence:
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
   1. Redistributions of source code must retain the above copyright notice,
```

### Comparing `ccplot-2.1.1/NEWS` & `ccplot-2.1.2/NEWS`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 CCPLOT NEWS
 
+New in 2.1.2 (2023-06-20)
+
+    * Support for Anaconda Python 3.10 on Windows.
+
 New in 2.1.1 (2021-01-23)
 
     * Fix building of Python wheel on Windows (missing DLLs).
 
 New in 2.1.0 (2021-11-28)
 
     * Support for text encoding in the API.
```

### Comparing `ccplot-2.1.1/PKG-INFO` & `ccplot-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ccplot
-Version: 2.1.1
+Version: 2.1.2
 Summary: CloudSat and CALIPSO plotting tool
 Home-page: http://www.ccplot.org/
 Author: Peter Kuma
 Author-email: peter@peterkuma.net
 License: BSD
 Description: ccplot is an open source command-line program for
             plotting profile, layer and earth view data sets from CloudSat, CALIPSO
```

### Comparing `ccplot-2.1.1/README.md` & `ccplot-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/bin/ccplot` & `ccplot-2.1.2/bin/ccplot`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 #
 # ccplot
 # This file is a part of ccplot: CloudSat and CALIPSO plotting tool.
 #
-# Copyright (c) 2009-2021 Peter Kuma
+# Copyright (c) 2009-2023 Peter Kuma
 #
 # This software is provided under the terms of a 2-clause BSD licence:
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 #   1. Redistributions of source code must retain the above copyright notice,
@@ -68,15 +68,15 @@
 
 import ccplot.algorithms
 import ccplot.utils
 
 
 # Early global variables.
 program_name = os.path.basename(sys.argv[0])
-__version__ = "2.1.1"
+__version__ = "2.1.2"
 CCPLOT_CMAP_PATH = os.path.join(ccplot.config.sharepath, 'cmap') \
                  + ":/usr/share/ccplot/cmap:/usr/local/share/ccplot/cmap"
 
 # Early functions.
 def fail(s):
     global program_name
     sys.stderr.write("%s: %s\n" % (program_name, s))
```

### Comparing `ccplot-2.1.1/ccplot/algorithms.pyx` & `ccplot-2.1.2/ccplot/algorithms.pyx`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/ccplot/autostr.py` & `ccplot-2.1.2/ccplot/autostr.py`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/ccplot/cctk.c` & `ccplot-2.1.2/ccplot/cctk.c`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/ccplot/hdf.pyx` & `ccplot-2.1.2/ccplot/hdf.pyx`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/ccplot/hdfeos.pyx` & `ccplot-2.1.2/ccplot/hdfeos.pyx`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/ccplot/utils.py` & `ccplot-2.1.2/ccplot/utils.py`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/ccplot.egg-info/PKG-INFO` & `ccplot-2.1.2/ccplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ccplot
-Version: 2.1.1
+Version: 2.1.2
 Summary: CloudSat and CALIPSO plotting tool
 Home-page: http://www.ccplot.org/
 Author: Peter Kuma
 Author-email: peter@peterkuma.net
 License: BSD
 Description: ccplot is an open source command-line program for
             plotting profile, layer and earth view data sets from CloudSat, CALIPSO
```

### Comparing `ccplot-2.1.1/ccplot.egg-info/SOURCES.txt` & `ccplot-2.1.2/ccplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/cmap/calipso-backscatter.cmap` & `ccplot-2.1.2/cmap/calipso-backscatter.cmap`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/cmap/calipso-temperature.cmap` & `ccplot-2.1.2/cmap/calipso-temperature.cmap`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/cmap/modis-reflectance.cmap` & `ccplot-2.1.2/cmap/modis-reflectance.cmap`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/cmap/modis-temperature.cmap` & `ccplot-2.1.2/cmap/modis-temperature.cmap`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/man/ccplot.1` & `ccplot-2.1.2/man/ccplot.1`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/man/ccplot.1.html` & `ccplot-2.1.2/man/ccplot.1.html`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/man/ccplot.1.ronn` & `ccplot-2.1.2/man/ccplot.1.ronn`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/setup.py` & `ccplot-2.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from glob import glob
 import shutil
 import sys
 import os
 import numpy
 
 # Windows build: modify to point to HDF4 and HDF-EOS2 libraries.
-WIN_HDF_DIR=r'C:\Program Files\HDF_Group\HDF\4.2.15'
+WIN_HDF_DIR=r'C:\Program Files\HDF_Group\HDF\4.2.16'
 WIN_HDFEOS_DIR=r'C:\Program Files\hdf-eos2-3.0'
 
 
 if sys.platform == 'win32':
     HDF_DIR = os.environ.get('HDF_DIR', WIN_HDF_DIR)
     HDFEOS_DIR = os.environ.get('HDFEOS_DIR', WIN_HDFEOS_DIR)
     scripts = ['bin/ccplot', 'bin/ccplot.bat']
-    hdf_libraries = ['hdf', 'mfhdf', 'libjpeg', 'libzlib', 'libszip', 'xdr', 'Ws2_32']
+    hdf_libraries = ['hdf', 'mfhdf', 'libjpeg', 'libzlib', 'libszaec', 'xdr', 'Ws2_32']
     hdf_include_dirs = [os.path.join(HDF_DIR, 'include')]
     hdf_library_dirs = [os.path.join(HDF_DIR, 'lib')]
     hdfeos_libraries = ['hdf-eos2']
     hdfeos_include_dirs = [os.path.join(HDFEOS_DIR, r'include')]
     hdfeos_library_dirs = [os.path.join(HDFEOS_DIR, r'vs2019\HDF-EOS2\x64\Release')]
     dlls = [
         os.path.join(HDF_DIR, 'bin', x)
@@ -48,15 +48,15 @@
 
 if sys.platform == 'darwin':
     hdfeos_libraries += ['Gctp']
 
 
 setup(
     name='ccplot',
-    version='2.1.1',
+    version='2.1.2',
     description='CloudSat and CALIPSO plotting tool',
     long_description="""ccplot is an open source command-line program for
     plotting profile, layer and earth view data sets from CloudSat, CALIPSO
     and Aqua MODIS products.""",
     platforms='any',
     author='Peter Kuma',
     author_email='peter@peterkuma.net',
@@ -90,15 +90,15 @@
     ],
     setup_requires=[
         'cython'
     ],
     include_dirs=[numpy.get_include()],
     data_files=[('share/doc/ccplot', ['NEWS']),
                 ('share/ccplot/cmap', glob('cmap/*')),
-                ('man/man1', ['man/ccplot.1'])],
+                ('share/man/man1', ['man/ccplot.1'])],
     include_package_data=True,
     package_data=package_data,
     cmdclass={
         'build_ext': build_ext,
     },
     ext_modules=[
         Extension(
```

### Comparing `ccplot-2.1.1/test/imgcompare` & `ccplot-2.1.2/test/imgcompare`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/test/libtest.sh` & `ccplot-2.1.2/test/libtest.sh`

 * *Files identical despite different names*

### Comparing `ccplot-2.1.1/test/test.sh` & `ccplot-2.1.2/test/test.sh`

 * *Files identical despite different names*

