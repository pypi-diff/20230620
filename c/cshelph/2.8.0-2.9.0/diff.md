# Comparing `tmp/cshelph-2.8.0.tar.gz` & `tmp/cshelph-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshelph-2.8.0.tar", last modified: Sun May 14 00:02:48 2023, max compression
+gzip compressed data, was "cshelph-2.9.0.tar", last modified: Mon Jun 19 22:50:27 2023, max compression
```

## Comparing `cshelph-2.8.0.tar` & `cshelph-2.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-14 00:02:48.693502 cshelph-2.8.0/
--rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.8.0/LICENSE.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)     3098 2023-05-14 00:02:48.693375 cshelph-2.8.0/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)     2590 2023-05-13 23:59:02.000000 cshelph-2.8.0/README.md
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-14 00:02:48.693188 cshelph-2.8.0/cshelph.egg-info/
--rw-r--r--   0 nmthoma1   (503) staff       (20)     3098 2023-05-14 00:02:48.000000 cshelph-2.8.0/cshelph.egg-info/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)      165 2023-05-14 00:02:48.000000 cshelph-2.8.0/cshelph.egg-info/SOURCES.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-14 00:02:48.000000 cshelph-2.8.0/cshelph.egg-info/dependency_links.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-05-14 00:02:48.000000 cshelph-2.8.0/cshelph.egg-info/top_level.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)    16694 2023-05-13 22:41:28.000000 cshelph-2.8.0/cshelph.py
--rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-14 00:02:48.693543 cshelph-2.8.0/setup.cfg
--rw-r--r--   0 nmthoma1   (503) staff       (20)     1669 2023-05-14 00:00:44.000000 cshelph-2.8.0/setup.py
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-06-19 22:50:27.353794 cshelph-2.9.0/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.9.0/LICENSE.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     3103 2023-06-19 22:50:27.353654 cshelph-2.9.0/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     2595 2023-06-19 22:50:01.000000 cshelph-2.9.0/README.md
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-06-19 22:50:27.353461 cshelph-2.9.0/cshelph.egg-info/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     3103 2023-06-19 22:50:27.000000 cshelph-2.9.0/cshelph.egg-info/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      165 2023-06-19 22:50:27.000000 cshelph-2.9.0/cshelph.egg-info/SOURCES.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-06-19 22:50:27.000000 cshelph-2.9.0/cshelph.egg-info/dependency_links.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-06-19 22:50:27.000000 cshelph-2.9.0/cshelph.egg-info/top_level.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    16777 2023-06-19 22:25:46.000000 cshelph-2.9.0/cshelph.py
+-rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-06-19 22:50:27.353838 cshelph-2.9.0/setup.cfg
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     1669 2023-06-19 22:48:42.000000 cshelph-2.9.0/setup.py
```

### Comparing `cshelph-2.8.0/LICENSE.txt` & `cshelph-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cshelph-2.8.0/PKG-INFO` & `cshelph-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cshelph
-Version: 2.8.0
+Version: 2.9.0
 Summary: Classification of Sub-aquatic Height Extracted Photons
 Home-page: https://github.com/nmt28/C-SHELPh
 Author: Nathan Thomas and Brian Lee
 Author-email: nmthomas28@gmail.com
 License: LICENSE.txt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -19,15 +19,15 @@
 
 ### C-SHELPh is the Classification of Sub-aquatic Height Extracted Photons. It is designed to isolate bathymetric photons in ICESat2 ATL03 files.
 
 ## Installation
 
 ### It is recommended that the dependancies are installed via:
 ```
-conda install -c conda-forge geopandas utm numpy matplotlib s3fs xarray zarr pyproj proj-data h5py earthaccess h5netcdf dask
+conda install -c conda-forge geopandas utm numpy matplotlib s3fs xarray zarr pyproj proj-data h5py earthaccess h5netcdf dask tqdm
 
 pip install cshelph
 
 ```
 
 ## Using C-SHELPh
```

### Comparing `cshelph-2.8.0/README.md` & `cshelph-2.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ### C-SHELPh is the Classification of Sub-aquatic Height Extracted Photons. It is designed to isolate bathymetric photons in ICESat2 ATL03 files.
 
 ## Installation
 
 ### It is recommended that the dependancies are installed via:
 ```
-conda install -c conda-forge geopandas utm numpy matplotlib s3fs xarray zarr pyproj proj-data h5py earthaccess h5netcdf dask
+conda install -c conda-forge geopandas utm numpy matplotlib s3fs xarray zarr pyproj proj-data h5py earthaccess h5netcdf dask tqdm
 
 pip install cshelph
 
 ```
 
 ## Using C-SHELPh
```

### Comparing `cshelph-2.8.0/cshelph.egg-info/PKG-INFO` & `cshelph-2.9.0/cshelph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cshelph
-Version: 2.8.0
+Version: 2.9.0
 Summary: Classification of Sub-aquatic Height Extracted Photons
 Home-page: https://github.com/nmt28/C-SHELPh
 Author: Nathan Thomas and Brian Lee
 Author-email: nmthomas28@gmail.com
 License: LICENSE.txt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -19,15 +19,15 @@
 
 ### C-SHELPh is the Classification of Sub-aquatic Height Extracted Photons. It is designed to isolate bathymetric photons in ICESat2 ATL03 files.
 
 ## Installation
 
 ### It is recommended that the dependancies are installed via:
 ```
-conda install -c conda-forge geopandas utm numpy matplotlib s3fs xarray zarr pyproj proj-data h5py earthaccess h5netcdf dask
+conda install -c conda-forge geopandas utm numpy matplotlib s3fs xarray zarr pyproj proj-data h5py earthaccess h5netcdf dask tqdm
 
 pip install cshelph
 
 ```
 
 ## Using C-SHELPh
```

### Comparing `cshelph-2.8.0/cshelph.py` & `cshelph-2.9.0/cshelph.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 import geopandas
 #import netCDF4
 from datetime import datetime
 import utm
 import xarray as xr
 import fsspec
 import earthaccess
-import geopandas
-
 # need s3fs installed
 
 def read_atl03(h5_file, laser_num):
     # Read File
     f = h5.File(h5_file,'r')
     
     # Select a laser
@@ -148,15 +146,15 @@
     
     # Add height bins to dataframe
     dataset1['height_bins'] = height_bins
     dataset1 = dataset1.reset_index(drop=True)
 
     return dataset1
 
-def get_sea_height(binned_data, surface_buffer):
+def get_sea_height(binned_data, surface_buffer=-0.5):
     '''Calculate mean sea height for easier calculation of depth and cleaner figures'''
     
     # Create sea height list
     sea_height = []
     
     # Group data by latitude
     binned_data_sea = binned_data[(binned_data['photon_height'] > surface_buffer)] # Filter out subsurface data
@@ -201,36 +199,31 @@
     
     date_range = file_date[0:4] + '-' + file_date[4:6] + '-' + file_date[6:]
     
     location_df = pd.DataFrame({'longitude':longitude,'latitude':latitude})
     
     location_df = location_df.dropna(axis=0)
     
-    med_lon = np.nanmedian(location_df['longitude'])
-    med_lat = np.nanmedian(location_df['latitude'])
+    minx, miny, maxx, maxy = np.min(location_df['longitude']), np.min(location_df['latitude']), np.max(location_df['longitude']), np.max(location_df['latitude'])
     
-    minx, miny, maxx, maxy = list(location_df.total_bounds)
+    lat_med = np.median(location_df['latitude'])
+    lon_med = np.median(location_df['longitude'])
 
     Query = earthaccess.collection_query()
 
     # Use chain methods to customize our query
-    Query.keyword('GHRSST Level 4 CMC0.1deg Global Foundation Sea Surface Temperature Analysis').bounding_box(minx,miny,maxx,maxy).temporal(date_range,date_range)
-
+    collections = Query.keyword('GHRSST Level 4 CMC0.1deg Global Foundation Sea Surface Temperature Analysis').bounding_box(minx,miny,maxx,maxy).temporal(date_range,date_range).get(10)
+    
     short_name = collections[0]["umm"]["ShortName"]
     
     Query = earthaccess.granule_query().short_name(short_name).version("3.0").bounding_box(minx,miny,maxx,maxy).temporal("2020-01-01","2020-01-01")
     
     granules = Query.get(10)
     
-    ds_L3 = xr.open_mfdataset(
-    earthaccess.open(granules),
-    combine='nested',
-    concat_dim='time',
-    coords='minimal',
-    )
+    ds_L3 = xr.open_mfdataset(earthaccess.open(granules),combine='nested',concat_dim='time',coords='minimal')
     
     sea_temp = ds_L3['analysed_sst'].sel(lat=lat_med,lon=lon_med,method='nearest').load()
     
     sst = round(np.nanmedian(sea_temp.values)-273,2)
     
     return sst
```

### Comparing `cshelph-2.8.0/setup.py` & `cshelph-2.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 #
 #
 # Purpose:  Installation of the C-SHELPh software
 #
 # Author: Nathan Thomas
 # Email: nmthomas28@gmail.com
 # Date: 05/05/2023
-# Version: 2.8.0
+# Version: 2.9.0
 #
 # History:
 # Version 2.7.0
 
 from distutils.core import setup
 import os
 
 setup(name='cshelph',
-    version='2.8.0',
+    version='2.9.0',
     description='Classification of Sub-aquatic Height Extracted Photons',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Nathan Thomas and Brian Lee',
     author_email='nmthomas28@gmail.com',
     scripts=['cshelph.py'],
     package_dir={},
```

