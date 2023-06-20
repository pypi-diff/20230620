# Comparing `tmp/cfr-0.6.0.tar.gz` & `tmp/cfr-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-0.6.0.tar", last modified: Mon Jun 19 02:43:55 2023, max compression
+gzip compressed data, was "cfr-0.6.1.tar", last modified: Tue Jun 20 03:58:37 2023, max compression
```

## Comparing `cfr-0.6.0.tar` & `cfr-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-19 02:43:55.064572 cfr-0.6.0/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.6.0/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-19 02:43:55.064401 cfr-0.6.0/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.6.0/README.md
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-19 02:43:55.056204 cfr-0.6.0/bin/
--rw-r--r--   0 fengzhu    (502) staff       (20)     5163 2023-06-19 02:34:42.000000 cfr-0.6.0/bin/cfr
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-19 02:43:55.060887 cfr-0.6.0/cfr/
--rw-r--r--   0 fengzhu    (502) staff       (20)      640 2023-03-24 23:03:50.000000 cfr-0.6.0/cfr/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-0.6.0/cfr/climate.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-19 02:43:55.064046 cfr-0.6.0/cfr/da/
--rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.6.0/cfr/da/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.6.0/cfr/da/enkf.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.6.0/cfr/gcm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.6.0/cfr/ml.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    63286 2023-06-17 21:42:44.000000 cfr-0.6.0/cfr/proxy.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    44993 2023-05-29 21:16:00.000000 cfr-0.6.0/cfr/psm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    54926 2023-06-19 02:39:39.000000 cfr-0.6.0/cfr/reconjob.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.6.0/cfr/reconres.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.6.0/cfr/ts.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    26581 2023-05-29 21:16:00.000000 cfr-0.6.0/cfr/utils.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.6.0/cfr/visual.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-19 02:43:55.063376 cfr-0.6.0/cfr.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-19 02:43:55.000000 cfr-0.6.0/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-19 02:43:55.000000 cfr-0.6.0/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-19 02:43:55.000000 cfr-0.6.0/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.6.0/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)      203 2023-06-19 02:43:55.000000 cfr-0.6.0/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-19 02:43:55.000000 cfr-0.6.0/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-19 02:43:55.064622 cfr-0.6.0/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1413 2023-06-17 21:43:24.000000 cfr-0.6.0/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-20 03:58:37.591813 cfr-0.6.1/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.6.1/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-20 03:58:37.591608 cfr-0.6.1/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.6.1/README.md
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-20 03:58:37.583348 cfr-0.6.1/bin/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     5163 2023-06-19 02:34:42.000000 cfr-0.6.1/bin/cfr
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-20 03:58:37.588061 cfr-0.6.1/cfr/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      640 2023-03-24 23:03:50.000000 cfr-0.6.1/cfr/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-0.6.1/cfr/climate.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-20 03:58:37.591269 cfr-0.6.1/cfr/da/
+-rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.6.1/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.6.1/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.6.1/cfr/gcm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.6.1/cfr/ml.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    64507 2023-06-20 03:20:00.000000 cfr-0.6.1/cfr/proxy.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-0.6.1/cfr/psm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    54926 2023-06-19 02:39:39.000000 cfr-0.6.1/cfr/reconjob.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.6.1/cfr/reconres.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.6.1/cfr/ts.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    26720 2023-06-20 03:27:33.000000 cfr-0.6.1/cfr/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.6.1/cfr/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-20 03:58:37.590533 cfr-0.6.1/cfr.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-20 03:58:37.000000 cfr-0.6.1/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-20 03:58:37.000000 cfr-0.6.1/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-20 03:58:37.000000 cfr-0.6.1/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.6.1/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)      203 2023-06-20 03:58:37.000000 cfr-0.6.1/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-20 03:58:37.000000 cfr-0.6.1/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-20 03:58:37.591869 cfr-0.6.1/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1413 2023-06-20 03:56:33.000000 cfr-0.6.1/setup.py
```

### Comparing `cfr-0.6.0/LICENSE` & `cfr-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-0.6.0/PKG-INFO` & `cfr-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.6.0
+Version: 0.6.1
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.6.0/README.md` & `cfr-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `cfr-0.6.0/bin/cfr` & `cfr-0.6.1/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-0.6.0/cfr/__init__.py` & `cfr-0.6.1/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.0/cfr/climate.py` & `cfr-0.6.1/cfr/climate.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.0/cfr/da/enkf.py` & `cfr-0.6.1/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.0/cfr/gcm.py` & `cfr-0.6.1/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.0/cfr/ml.py` & `cfr-0.6.1/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.0/cfr/proxy.py` & `cfr-0.6.1/cfr/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         ''' Centering the proxy timeseries regarding a reference period.
 
         Args:
             ref_period (tuple or list): the reference time period in the form or (start_yr, end_yr)
         '''
         new = self.copy()
         ref = self.slice(ref_period)
-        new.value -= np.mean(ref.value)
+        new.value -= np.nanmean(ref.value)
         return new
 
     def slice(self, timespan):
         ''' Slicing the timeseries with a timespan (tuple or list)
 
         Args:
             timespan (tuple or list):
@@ -256,18 +256,18 @@
             self.value, dims=['time'], coords={'time': dates}, name=self.pid,
             attrs={
                 'lat': self.lat,
                 'lon': self.lon,
                 'elev': np.nan if self.elev is None else self.elev,
                 'ptype': self.ptype,
                 'dt': self.dt,
-                'time_name': self.time_name,
-                'time_unit': self.time_unit,
-                'value_name': self.value_name,
-                'value_unit': self.value_unit,
+                'time_name': 'time' if self.time_name is None else self.time_name,
+                'time_unit': 'none' if self.time_unit is None else self.time_unit,
+                'value_name': 'value' if self.value_name is None else self.value_name,
+                'value_unit': 'none' if self.value_unit is None else self.value_unit,
             }
         )
         return da
 
     def from_da(self, da):
         ''' Get the time and value axis from the given Xarray.DataArray
         '''
@@ -307,15 +307,15 @@
             
 
     def standardize(self):
         new = self.copy()
         if self.value.std() == 0:
             new.value = np.zeros(np.size(self.value))
         else:
-            new.value = (self.value - self.value.mean()) / self.value.std()
+            new.value = (self.value - np.nanmean(self.value)) / np.nanstd(self.value)
         return new
 
     def __getitem__(self, key):
         ''' This makes the object subscriptable. '''
         new = self.copy()
         if type(key) is int or type(key) is list:
             new.value = new.value[key]
@@ -861,23 +861,50 @@
         ''' Make a deepcopy of the object. '''
         return copy.deepcopy(self)
 
     def center(self, ref_period):
         ''' Center the proxy timeseries against a reference time period.
 
         Args:
+        ----    
             ref_period (tuple or list): the reference time period in the form or (start_yr, end_yr)
+            
+        Returns
+        -------
+        new : cfr.ProxyDatabase object
+        
         '''
         new = self.copy()
         for pid, pobj in tqdm(self.records.items(), total=self.nrec, desc='Centering each of the ProxyRecord'):
             ref = pobj.slice(ref_period)
             if np.size(ref.time) == 0:
                 new -= pobj
             else:
-                new.records[pid].value -= np.mean(ref.value)
+                new.records[pid].value -= np.nanmean(ref.value)
+
+        return new
+    
+    def standardize(self, ref_period):
+        ''' Standardize elements of a proxy database against a reference time period.
+            Elements that have no values over the reference period are dropped 
+
+        Args:
+            ref_period (tuple or list): the reference time period in the form or (start_yr, end_yr)
+            
+        Returns
+        -------
+        new : cfr.ProxyDatabase object
+        '''
+        new = self.copy()
+        for pid, pobj in tqdm(self.records.items(), total=self.nrec, desc='Standardizing each of the ProxyRecords'):
+            ref = pobj.slice(ref_period)
+            if len(ref.time) < 5:
+                new -= pobj
+            else:
+                new.records[pid].value = (pobj.value - np.nanmean(ref.value)) / np.nanstd(ref.value)
 
         return new
 
     def refresh(self):
         ''' Refresh a bunch of attributes. '''
         self.nrec = len(self.records)
         self.pids = [pobj.pid for pid, pobj in self.records.items()]
@@ -935,15 +962,15 @@
         else:
             raise ValueError('Wrong file extention based on the given URL!')
 
         return pdb
 
     def from_df(self, df, pid_column='paleoData_pages2kID', lat_column='geo_meanLat', lon_column='geo_meanLon', elev_column='geo_meanElev',
                 time_column='year', value_column='paleoData_values', proxy_type_column='paleoData_proxy', archive_type_column='archiveType',
-                value_name_column='paleoData_variableName', value_unit_column='paleoData_units',
+                ptype_column='ptype', value_name_column='paleoData_variableName', value_unit_column='paleoData_units',
                 verbose=False):
         ''' Load database from a Pandas DataFrame
 
         Args:
             df (pandas.DataFrame): a Pandas DataFrame include at least lat, lon, time, value, proxy_type
             ptype_psm (dict): a mapping from ptype to psm
             verbose (bool, optional): print verbose information. Defaults to False.
@@ -954,17 +981,20 @@
             if verbose:
                 utils.p_fail(f'ProxyDatabase.from_df() >>> {err_msg}')
             raise TypeError(err_msg)
 
         records = OrderedDict()
 
         for idx, row in df.iterrows():
-            proxy_type = row[proxy_type_column]
-            archive_type = row[archive_type_column]
-            ptype = get_ptype(archive_type, proxy_type)
+            if ptype_column not in row:
+                proxy_type = row[proxy_type_column]
+                archive_type = row[archive_type_column]
+                ptype = get_ptype(archive_type, proxy_type)
+            else:
+                ptype = row[ptype_column]
             pid = row[pid_column]
             lat = row[lat_column]
             lon = np.mod(row[lon_column], 360)
             elev = row[elev_column]
             time = row[time_column]
             if type(time) is str:
                 time = utils.arr_str2np(time)
```

### Comparing `cfr-0.6.0/cfr/psm.py` & `cfr-0.6.1/cfr/psm.py`

 * *Files 0% similar despite different names*

```diff
@@ -659,17 +659,18 @@
         # run the model
 
         # annualize the data
         tas_ann = self.pobj.clim[self.tas_name].annualize()
         pr_ann = self.pobj.clim[self.pr_name].annualize()
         psl_ann = self.pobj.clim[self.psl_name].annualize()
 
+        year_in_float = utils.datetime2year_float(self.pobj.clim[self.pr_name].da.time.values)
         # sensor model
         d18O_ice = ice_sensor(
-            self.pobj.clim[self.pr_name].da.time.values,
+            year_in_float,
             self.pobj.clim[self.d18O_name].da.values,
             self.pobj.clim[self.pr_name].da.values,
             alt_diff=alt_diff,
         )
 
         # diffuse model
         if nproc is None: nproc = cpu_count()
```

### Comparing `cfr-0.6.0/cfr/reconjob.py` & `cfr-0.6.1/cfr/reconjob.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.0/cfr/reconres.py` & `cfr-0.6.1/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.0/cfr/ts.py` & `cfr-0.6.1/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.0/cfr/utils.py` & `cfr-0.6.1/cfr/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -726,12 +726,13 @@
     'iCESM_past1000/psl': 'https://atmos.washington.edu/~rtardif/LMR/prior/psl_sfc_Amon_iCESM_past1000_085001-184912.nc',
     'gistemp1200_ERSSTv4': 'https://github.com/fzhu2e/cfr-data/raw/main/gistemp1200_ERSSTv4.nc.gz',
     'gistemp1200_GHCNv4_ERSSTv5': 'https://data.giss.nasa.gov/pub/gistemp/gistemp1200_GHCNv4_ERSSTv5.nc.gz',
     'CRUTSv4.07/tas': 'https://crudata.uea.ac.uk/cru/data/hrg/cru_ts_4.07/cruts.2304141047.v4.07/tmp/cru_ts4.07.1901.2022.tmp.dat.nc.gz',
     'CRUTSv4.07/pr': 'https://crudata.uea.ac.uk/cru/data/hrg/cru_ts_4.07/cruts.2304141047.v4.07/pre/cru_ts4.07.1901.2022.pre.dat.nc.gz',
     '20CRv3/tas': 'https://downloads.psl.noaa.gov/Datasets/20thC_ReanV3/Monthlies/2mSI-MO/air.2m.mon.mean.nc',
     '20CRv3/pr': 'https://downloads.psl.noaa.gov/Datasets/20thC_ReanV3/Monthlies/sfcSI-MO/prate.mon.mean.nc',
+    'HadCRUTv5': 'https://www.metoffice.gov.uk/hadobs/hadcrut5/data/current/analysis/HadCRUT.5.0.1.0.analysis.anomalies.ensemble_mean.nc',
 }
 
 ensts_url_dict = {
     'BC09_NINO34': 'https://github.com/fzhu2e/cfr-data/raw/main/BC09_NINO34.csv',
 }
```

### Comparing `cfr-0.6.0/cfr/visual.py` & `cfr-0.6.1/cfr/visual.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.0/cfr.egg-info/PKG-INFO` & `cfr-0.6.1/cfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.6.0
+Version: 0.6.1
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.6.0/setup.py` & `cfr-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='0.6.0',
+    version='0.6.1',
     description='cfr: a Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

