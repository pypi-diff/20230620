# Comparing `tmp/openstef_dbc-3.6.8a7.tar.gz` & `tmp/openstef_dbc-3.6.8a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstef_dbc-3.6.8a7.tar", last modified: Wed May 24 07:35:18 2023, max compression
+gzip compressed data, was "openstef_dbc-3.6.8a8.tar", last modified: Tue Jun 20 12:19:24 2023, max compression
```

## Comparing `openstef_dbc-3.6.8a7.tar` & `openstef_dbc-3.6.8a8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:35:18.325897 openstef_dbc-3.6.8a7/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-24 07:35:18.325897 openstef_dbc-3.6.8a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:35:18.321897 openstef_dbc-3.6.8a7/openstef_dbc/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/data_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/ktp_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:35:18.321897 openstef_dbc-3.6.8a7/openstef_dbc/log/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/log/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/log/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:35:18.321897 openstef_dbc-3.6.8a7/openstef_dbc/models/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/models/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/models/switch_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:35:18.325897 openstef_dbc-3.6.8a7/openstef_dbc/services/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/services/ems.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/services/model_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/services/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/services/predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/services/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/services/splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/services/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/services/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/services/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/openstef_dbc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:35:18.321897 openstef_dbc-3.6.8a7/openstef_dbc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-24 07:35:18.000000 openstef_dbc-3.6.8a7/openstef_dbc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-24 07:35:18.000000 openstef_dbc-3.6.8a7/openstef_dbc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:35:18.000000 openstef_dbc-3.6.8a7/openstef_dbc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-24 07:35:18.000000 openstef_dbc-3.6.8a7/openstef_dbc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 07:35:18.000000 openstef_dbc-3.6.8a7/openstef_dbc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-24 07:35:18.325897 openstef_dbc-3.6.8a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-24 07:35:04.000000 openstef_dbc-3.6.8a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:19:24.741753 openstef_dbc-3.6.8a8/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-20 12:19:24.741753 openstef_dbc-3.6.8a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:19:24.741753 openstef_dbc-3.6.8a8/openstef_dbc/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/data_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/ktp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:19:24.741753 openstef_dbc-3.6.8a8/openstef_dbc/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/log/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/log/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:19:24.741753 openstef_dbc-3.6.8a8/openstef_dbc/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/models/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/models/switch_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:19:24.741753 openstef_dbc-3.6.8a8/openstef_dbc/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/services/ems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/services/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/services/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/services/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/services/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/services/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/services/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/services/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18312 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/services/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/openstef_dbc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:19:24.741753 openstef_dbc-3.6.8a8/openstef_dbc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-20 12:19:24.000000 openstef_dbc-3.6.8a8/openstef_dbc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-20 12:19:24.000000 openstef_dbc-3.6.8a8/openstef_dbc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:19:24.000000 openstef_dbc-3.6.8a8/openstef_dbc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-20 12:19:24.000000 openstef_dbc-3.6.8a8/openstef_dbc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 12:19:24.000000 openstef_dbc-3.6.8a8/openstef_dbc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-20 12:19:24.741753 openstef_dbc-3.6.8a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-20 12:19:14.000000 openstef_dbc-3.6.8a8/setup.py
```

### Comparing `openstef_dbc-3.6.8a7/LICENSE` & `openstef_dbc-3.6.8a8/LICENSE`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/PKG-INFO` & `openstef_dbc-3.6.8a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.6.8a7
+Version: 3.6.8a8
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.8a7/README.md` & `openstef_dbc-3.6.8a8/README.md`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/__init__.py` & `openstef_dbc-3.6.8a8/openstef_dbc/__init__.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/data_interface.py` & `openstef_dbc-3.6.8a8/openstef_dbc/data_interface.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/database.py` & `openstef_dbc-3.6.8a8/openstef_dbc/database.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/ktp_api.py` & `openstef_dbc-3.6.8a8/openstef_dbc/ktp_api.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/log/logging.py` & `openstef_dbc-3.6.8a8/openstef_dbc/log/logging.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/log/processors.py` & `openstef_dbc-3.6.8a8/openstef_dbc/log/processors.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/models/measurement.py` & `openstef_dbc-3.6.8a8/openstef_dbc/models/measurement.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/services/ems.py` & `openstef_dbc-3.6.8a8/openstef_dbc/services/ems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/services/model_input.py` & `openstef_dbc-3.6.8a8/openstef_dbc/services/model_input.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/services/prediction_job.py` & `openstef_dbc-3.6.8a8/openstef_dbc/services/prediction_job.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/services/predictions.py` & `openstef_dbc-3.6.8a8/openstef_dbc/services/predictions.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/services/predictor.py` & `openstef_dbc-3.6.8a8/openstef_dbc/services/predictor.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/services/splitting.py` & `openstef_dbc-3.6.8a8/openstef_dbc/services/splitting.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/services/systems.py` & `openstef_dbc-3.6.8a8/openstef_dbc/services/systems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/services/weather.py` & `openstef_dbc-3.6.8a8/openstef_dbc/services/weather.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/services/write.py` & `openstef_dbc-3.6.8a8/openstef_dbc/services/write.py`

 * *Files 6% similar despite different names*

```diff
@@ -267,14 +267,56 @@
 
         field_columns = [
             x
             for x in list(influx_df.columns)
             if x not in tag_columns + forbidden_fields
         ]
 
+        # Cast columns to correct type, as influx is extremely picky
+        casting_dict = {
+            "source_run": np.int64,
+            "input_city": str,
+            "temp": np.float64,
+            "windspeed_100m": np.float64,
+            "windspeed": np.float64,
+            "winddeg": np.float64,
+            "clouds": np.float64,
+            "mxlD": np.float64,
+            "snowDepth": np.float64,
+            "pressure": np.float64,
+            "humidity": np.float64,
+            "clearSky_ulf": np.float64,
+            "clearSky_dlf": np.float64,
+            "radiation": np.float64,
+            "windspeed_100m_ensemble": np.float64,
+            "windspeed_ensemble": np.float64,
+            "winddeg_ensemble": np.float64,
+            "clouds_ensemble": np.float64,
+            "radiation_ensemble": np.float64,
+            "ensemble_run": str,
+            "source": str,
+            "created": np.int64,
+        }
+
+        # Check if we have all columns and not some extra
+        casting_dict_columns = list(casting_dict.keys())
+        for k in casting_dict_columns:
+            # Remove any casting dict entries that are not in the dataframe
+            if k not in influx_df.columns:
+                casting_dict.pop(k, None)
+
+        if set(casting_dict.keys()) != set(
+            influx_df.columns.to_list()
+        ):  # Check if we have a type description for every column, if not raise an error
+            raise ValueError(
+                "Got unexpected columns, unable to cast these columns in the correct datatype."
+            )
+
+        influx_df = influx_df.astype(casting_dict)
+
         # Write DataFrame to influx database
         result = _DataInterface.get_instance().exec_influx_write(
             influx_df.copy(),
             database=dbname,
             measurement=table,
             tag_columns=tag_columns,
             field_columns=field_columns,
```

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc/utils.py` & `openstef_dbc-3.6.8a8/openstef_dbc/utils.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc.egg-info/PKG-INFO` & `openstef_dbc-3.6.8a8/openstef_dbc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef-dbc
-Version: 3.6.8a7
+Version: 3.6.8a8
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openstef_dbc-3.6.8a7/openstef_dbc.egg-info/SOURCES.txt` & `openstef_dbc-3.6.8a8/openstef_dbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.6.8a7/setup.py` & `openstef_dbc-3.6.8a8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def read_long_description_from_readme():
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name="openstef_dbc",
-    version="3.6.8a7",
+    version="3.6.8a8",
     packages=find_packages(include=["openstef_dbc", "openstef_dbc.*"]),
     description="Database Connection for OpenSTEF",
     long_description=read_long_description_from_readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/openstef/openstef-dbc",
     author="Alliander N.V",
     author_email="korte.termijn.prognoses@alliander.com",
```

