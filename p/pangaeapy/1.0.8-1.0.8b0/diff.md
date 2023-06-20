# Comparing `tmp/pangaeapy-1.0.8.tar.gz` & `tmp/pangaeapy-1.0.8b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pangaeapy-1.0.8.tar", last modified: Mon Nov  7 11:42:00 2022, max compression
+gzip compressed data, was "dist\pangaeapy-1.0.8b0.tar", last modified: Mon Nov  7 12:03:07 2022, max compression
```

## Comparing `pangaeapy-1.0.8.tar` & `pangaeapy-1.0.8b0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/
--rw-rw-rw-   0        0        0    35819 2020-07-06 11:59:36.000000 pangaeapy-1.0.8/LICENSE.md
--rw-rw-rw-   0        0        0      755 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      261 2021-12-27 13:22:58.000000 pangaeapy-1.0.8/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/data/
--rw-rw-rw-   0        0        0    39424 2021-12-30 14:14:28.000000 pangaeapy-1.0.8/data/parameter_mapping.csv
-drwxrwxrwx   0        0        0        0 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/export/
--rw-rw-rw-   0        0        0       37 2021-12-23 10:48:23.000000 pangaeapy-1.0.8/export/read.me
-drwxrwxrwx   0        0        0        0 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/exporter/
--rw-rw-rw-   0        0        0        0 2021-06-23 12:35:36.000000 pangaeapy-1.0.8/exporter/__init__.py
--rw-rw-rw-   0        0        0    17409 2022-11-04 14:07:08.000000 pangaeapy-1.0.8/exporter/pan_dwca_exporter.py
--rw-rw-rw-   0        0        0      999 2022-01-07 09:34:34.000000 pangaeapy-1.0.8/exporter/pan_exporter.py
--rw-rw-rw-   0        0        0     4141 2022-11-01 14:03:30.000000 pangaeapy-1.0.8/exporter/pan_frictionless_exporter.py
--rw-rw-rw-   0        0        0    24907 2022-01-07 10:08:04.000000 pangaeapy-1.0.8/exporter/pan_netcdf_exporter.py
--rw-rw-rw-   0        0        0     2435 2022-11-01 14:03:30.000000 pangaeapy-1.0.8/exporter/pan_panimport_exporter.py
-drwxrwxrwx   0        0        0        0 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/exporter/xslt/
--rw-rw-rw-   0        0        0     4250 2022-02-04 13:16:24.000000 pangaeapy-1.0.8/exporter/xslt/panmd2eml.xslt
-drwxrwxrwx   0        0        0        0 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/mappings/
--rw-rw-rw-   0        0        0        0 2021-06-23 12:35:28.000000 pangaeapy-1.0.8/mappings/__init__.py
--rw-rw-rw-   0        0        0      213 2021-04-23 09:40:05.000000 pangaeapy-1.0.8/mappings/mapping_helper.py
--rw-rw-rw-   0        0        0    65684 2021-12-30 14:08:44.000000 pangaeapy-1.0.8/mappings/pan_mappings.json
--rw-rw-rw-   0        0        0    65102 2022-11-04 11:35:30.000000 pangaeapy-1.0.8/pandataset.py
-drwxrwxrwx   0        0        0        0 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/pangaeapy.egg-info/
--rw-rw-rw-   0        0        0      755 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/pangaeapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      565 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/pangaeapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/pangaeapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/pangaeapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/pangaeapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2887 2021-02-18 14:04:28.000000 pangaeapy-1.0.8/panquery.py
--rw-rw-rw-   0        0        0       97 2022-11-02 09:48:17.000000 pangaeapy-1.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-11-07 11:42:00.000000 pangaeapy-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1120 2022-11-07 11:38:18.000000 pangaeapy-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/
+-rw-rw-rw-   0        0        0    35819 2020-07-06 11:59:36.000000 pangaeapy-1.0.8b0/LICENSE.md
+-rw-rw-rw-   0        0        0      757 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2021-12-27 13:22:58.000000 pangaeapy-1.0.8b0/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/data/
+-rw-rw-rw-   0        0        0    39424 2021-12-30 14:14:28.000000 pangaeapy-1.0.8b0/data/parameter_mapping.csv
+drwxrwxrwx   0        0        0        0 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/export/
+-rw-rw-rw-   0        0        0       37 2021-12-23 10:48:23.000000 pangaeapy-1.0.8b0/export/read.me
+drwxrwxrwx   0        0        0        0 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/exporter/
+-rw-rw-rw-   0        0        0        0 2021-06-23 12:35:36.000000 pangaeapy-1.0.8b0/exporter/__init__.py
+-rw-rw-rw-   0        0        0    17472 2022-11-07 12:02:04.000000 pangaeapy-1.0.8b0/exporter/pan_dwca_exporter.py
+-rw-rw-rw-   0        0        0      999 2022-01-07 09:34:34.000000 pangaeapy-1.0.8b0/exporter/pan_exporter.py
+-rw-rw-rw-   0        0        0     4141 2022-11-01 14:03:30.000000 pangaeapy-1.0.8b0/exporter/pan_frictionless_exporter.py
+-rw-rw-rw-   0        0        0    24907 2022-01-07 10:08:04.000000 pangaeapy-1.0.8b0/exporter/pan_netcdf_exporter.py
+-rw-rw-rw-   0        0        0     2435 2022-11-01 14:03:30.000000 pangaeapy-1.0.8b0/exporter/pan_panimport_exporter.py
+drwxrwxrwx   0        0        0        0 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/exporter/xslt/
+-rw-rw-rw-   0        0        0     4250 2022-02-04 13:16:24.000000 pangaeapy-1.0.8b0/exporter/xslt/panmd2eml.xslt
+drwxrwxrwx   0        0        0        0 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/mappings/
+-rw-rw-rw-   0        0        0        0 2021-06-23 12:35:28.000000 pangaeapy-1.0.8b0/mappings/__init__.py
+-rw-rw-rw-   0        0        0      213 2021-04-23 09:40:05.000000 pangaeapy-1.0.8b0/mappings/mapping_helper.py
+-rw-rw-rw-   0        0        0    65684 2021-12-30 14:08:44.000000 pangaeapy-1.0.8b0/mappings/pan_mappings.json
+-rw-rw-rw-   0        0        0    65102 2022-11-04 11:35:30.000000 pangaeapy-1.0.8b0/pandataset.py
+drwxrwxrwx   0        0        0        0 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/pangaeapy.egg-info/
+-rw-rw-rw-   0        0        0      757 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/pangaeapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/pangaeapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/pangaeapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/pangaeapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/pangaeapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2887 2021-02-18 14:04:28.000000 pangaeapy-1.0.8b0/panquery.py
+-rw-rw-rw-   0        0        0       97 2022-11-02 09:48:17.000000 pangaeapy-1.0.8b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-11-07 12:03:07.000000 pangaeapy-1.0.8b0/setup.cfg
+-rw-rw-rw-   0        0        0     1121 2022-11-07 12:02:26.000000 pangaeapy-1.0.8b0/setup.py
```

### Comparing `pangaeapy-1.0.8/LICENSE.md` & `pangaeapy-1.0.8b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pangaeapy-1.0.8/PKG-INFO` & `pangaeapy-1.0.8b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangaeapy
-Version: 1.0.8
+Version: 1.0.8b0
 Summary: This module allows to download and analyse metadata as well as data from tabular PANGAEA (https://www.pangaea.de) datasets.                  Usage:         import pangaeapy.pandataset as pd         ds= pd.PanDataSet(787140)         print(ds.title)         print(ds.data.head())                  Please visit the github project page to see more documentation and some examples:         https://github.com/pangaea-data-publisher/pangaeapy
 Home-page: https://github.com/pangaea-data-publisher/pangaeapy
 Author: Robert Huber
 Author-email: rhuber@uni-bremen.de
 License: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 License-File: LICENSE.md
```

### Comparing `pangaeapy-1.0.8/data/parameter_mapping.csv` & `pangaeapy-1.0.8b0/data/parameter_mapping.csv`

 * *Files identical despite different names*

### Comparing `pangaeapy-1.0.8/exporter/pan_dwca_exporter.py` & `pangaeapy-1.0.8b0/exporter/pan_dwca_exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             taxonframe['institutionCode'] = 'Pangaea'
             doimatch = re.search('(10\.1594/PANGAEA\.[0-9]+)', self.pandataset.doi)
             taxonframe['CollectionCode'] = 'doi:' + str(doimatch[1])
             taxonframe['datasetID'] = self.pandataset.doi
             taxonframe['basisOfRecord'] = basisofrecord
             taxonframe['catalogNumber'] = taxonframe['Colname'].apply(
                 lambda x: taxoncolumns.get(x).get('series')).astype(str) + '_' + taxonframe['index'].astype(str)
-            taxonframe['recordedBy'] = taxonframe['Colname'].apply(lambda x: taxoncolumns.get(x).get('author'))
+            taxonframe['recordedBy'] = taxonframe['Colname'].apply(lambda x: None if not taxoncolumns.get(x).get('author') else taxoncolumns.get(x).get('author').get('name'))
             taxonframe['scientificName'] = taxonframe['Colname'].apply(lambda x: taxoncolumns.get(x).get('taxon'))
             taxonframe['geodeticDatum'] = 'WGS84'
             taxonframe['kingdom'] = taxonframe['Colname'].apply(lambda x: taxoncolumns.get(x).get('kingdom'))
             #taxonframe['organismQuantityType'] = 'individuals (' + taxonframe['Colname'].apply(
             #    lambda x: taxoncolumns.get(x).get('unit')).astype(str) + ')'
             taxonframe['organismQuantityType'] = taxonframe['Colname'].apply(lambda x: taxoncolumns.get(x).get('dimension'))
             try:
```

### Comparing `pangaeapy-1.0.8/exporter/pan_exporter.py` & `pangaeapy-1.0.8b0/exporter/pan_exporter.py`

 * *Files identical despite different names*

### Comparing `pangaeapy-1.0.8/exporter/pan_frictionless_exporter.py` & `pangaeapy-1.0.8b0/exporter/pan_frictionless_exporter.py`

 * *Files identical despite different names*

### Comparing `pangaeapy-1.0.8/exporter/pan_netcdf_exporter.py` & `pangaeapy-1.0.8b0/exporter/pan_netcdf_exporter.py`

 * *Files identical despite different names*

### Comparing `pangaeapy-1.0.8/exporter/pan_panimport_exporter.py` & `pangaeapy-1.0.8b0/exporter/pan_panimport_exporter.py`

 * *Files identical despite different names*

### Comparing `pangaeapy-1.0.8/exporter/xslt/panmd2eml.xslt` & `pangaeapy-1.0.8b0/exporter/xslt/panmd2eml.xslt`

 * *Files identical despite different names*

### Comparing `pangaeapy-1.0.8/mappings/pan_mappings.json` & `pangaeapy-1.0.8b0/mappings/pan_mappings.json`

 * *Files identical despite different names*

### Comparing `pangaeapy-1.0.8/pandataset.py` & `pangaeapy-1.0.8b0/pandataset.py`

 * *Files identical despite different names*

### Comparing `pangaeapy-1.0.8/pangaeapy.egg-info/PKG-INFO` & `pangaeapy-1.0.8b0/pangaeapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangaeapy
-Version: 1.0.8
+Version: 1.0.8b0
 Summary: This module allows to download and analyse metadata as well as data from tabular PANGAEA (https://www.pangaea.de) datasets.                  Usage:         import pangaeapy.pandataset as pd         ds= pd.PanDataSet(787140)         print(ds.title)         print(ds.data.head())                  Please visit the github project page to see more documentation and some examples:         https://github.com/pangaea-data-publisher/pangaeapy
 Home-page: https://github.com/pangaea-data-publisher/pangaeapy
 Author: Robert Huber
 Author-email: rhuber@uni-bremen.de
 License: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 License-File: LICENSE.md
```

### Comparing `pangaeapy-1.0.8/pangaeapy.egg-info/SOURCES.txt` & `pangaeapy-1.0.8b0/pangaeapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pangaeapy-1.0.8/panquery.py` & `pangaeapy-1.0.8b0/panquery.py`

 * *Files identical despite different names*

### Comparing `pangaeapy-1.0.8/setup.py` & `pangaeapy-1.0.8b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pangaeapy',
-    version='1.0.8',
+    version='1.0.8b',
     install_requires=['lxml>=4.9.1','requests~=2.26.0','pandas~=1.3.5','numpy>=1.21.0','netcdf4~=1.5.6'],
     packages=['pangaeapy','pangaeapy.exporter'],
     package_dir={'pangaeapy': ''},
     #package_data={'mypkg': ['data/*.dat']},
     package_data={'pangaeapy': ['mappings/*.json','data/*.csv','export/*.*']},
     include_package_data=True,
     url='https://github.com/pangaea-data-publisher/pangaeapy',
```

