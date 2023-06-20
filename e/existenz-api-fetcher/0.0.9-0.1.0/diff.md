# Comparing `tmp/existenz_api_fetcher-0.0.9.tar.gz` & `tmp/existenz_api_fetcher-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "existenz_api_fetcher-0.0.9.tar", last modified: Sun Apr 30 20:03:22 2023, max compression
+gzip compressed data, was "existenz_api_fetcher-0.1.0.tar", last modified: Tue Jun 20 15:23:25 2023, max compression
```

## Comparing `existenz_api_fetcher-0.0.9.tar` & `existenz_api_fetcher-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-04-30 20:03:29.470936 existenz_api_fetcher-0.0.9/
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1073 2022-10-03 16:15:39.000000 existenz_api_fetcher-0.0.9/LICENSE.txt
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1481 2023-04-30 20:03:29.468681 existenz_api_fetcher-0.0.9/PKG-INFO
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)      918 2023-03-10 14:08:16.000000 existenz_api_fetcher-0.0.9/README.md
-drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-04-30 20:03:29.331307 existenz_api_fetcher-0.0.9/existenz_api_fetcher/
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2022-09-21 17:33:00.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher/__init__.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     3752 2022-10-19 10:50:04.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher/hydro.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1863 2023-04-29 11:39:56.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher/locations.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)    13936 2023-03-13 14:45:01.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher/meteo.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1695 2023-03-09 20:16:31.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher/pipelines.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)       80 2023-04-29 20:55:39.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher/test.py
-drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-04-30 20:03:29.388149 existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1481 2023-04-30 20:03:29.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/PKG-INFO
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)      536 2023-04-30 20:03:29.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/SOURCES.txt
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)        1 2023-04-30 20:03:29.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/dependency_links.txt
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)       69 2023-04-30 20:03:29.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/requires.txt
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)       27 2023-04-30 20:03:29.000000 existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/top_level.txt
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)      565 2023-04-29 21:08:06.000000 existenz_api_fetcher-0.0.9/pyproject.toml
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)       38 2023-04-30 20:03:29.471681 existenz_api_fetcher-0.0.9/setup.cfg
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)      872 2023-04-30 18:14:06.000000 existenz_api_fetcher-0.0.9/setup.py
-drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-04-30 20:03:29.453176 existenz_api_fetcher-0.0.9/tests/
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2022-09-25 11:55:02.000000 existenz_api_fetcher-0.0.9/tests/__init__.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)      345 2022-10-17 08:25:28.000000 existenz_api_fetcher-0.0.9/tests/test_hydro.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1037 2022-10-17 08:25:28.000000 existenz_api_fetcher-0.0.9/tests/test_meteo.py
--rwxrwxrwx   0 lilian    (1000) lilian    (1000)      305 2022-10-17 08:25:28.000000 existenz_api_fetcher-0.0.9/tests/test_pipelines.py
+drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-06-20 15:23:25.042977 existenz_api_fetcher-0.1.0/
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1073 2022-10-03 16:15:39.000000 existenz_api_fetcher-0.1.0/LICENSE.txt
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1466 2023-06-20 15:23:25.039977 existenz_api_fetcher-0.1.0/PKG-INFO
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)      904 2023-06-20 15:19:55.000000 existenz_api_fetcher-0.1.0/README.md
+drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-06-20 15:23:24.920459 existenz_api_fetcher-0.1.0/existenz_api_fetcher/
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2022-09-21 17:33:00.000000 existenz_api_fetcher-0.1.0/existenz_api_fetcher/__init__.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     3854 2023-06-20 14:36:02.000000 existenz_api_fetcher-0.1.0/existenz_api_fetcher/hydro.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     2990 2023-06-20 14:11:48.000000 existenz_api_fetcher-0.1.0/existenz_api_fetcher/locations.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)    14298 2023-06-20 15:06:03.000000 existenz_api_fetcher-0.1.0/existenz_api_fetcher/meteo.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1834 2023-06-20 14:14:13.000000 existenz_api_fetcher-0.1.0/existenz_api_fetcher/pipelines.py
+drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-06-20 15:23:24.980555 existenz_api_fetcher-0.1.0/existenz_api_fetcher.egg-info/
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1466 2023-06-20 15:23:24.000000 existenz_api_fetcher-0.1.0/existenz_api_fetcher.egg-info/PKG-INFO
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)      507 2023-06-20 15:23:24.000000 existenz_api_fetcher-0.1.0/existenz_api_fetcher.egg-info/SOURCES.txt
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)        1 2023-06-20 15:23:24.000000 existenz_api_fetcher-0.1.0/existenz_api_fetcher.egg-info/dependency_links.txt
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)       84 2023-06-20 15:23:24.000000 existenz_api_fetcher-0.1.0/existenz_api_fetcher.egg-info/requires.txt
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)       27 2023-06-20 15:23:24.000000 existenz_api_fetcher-0.1.0/existenz_api_fetcher.egg-info/top_level.txt
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)      565 2023-06-20 15:22:54.000000 existenz_api_fetcher-0.1.0/pyproject.toml
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)       38 2023-06-20 15:23:25.043985 existenz_api_fetcher-0.1.0/setup.cfg
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)      898 2023-06-20 15:21:27.000000 existenz_api_fetcher-0.1.0/setup.py
+drwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2023-06-20 15:23:25.026464 existenz_api_fetcher-0.1.0/tests/
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)        0 2022-09-25 11:55:02.000000 existenz_api_fetcher-0.1.0/tests/__init__.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)      345 2022-10-17 08:25:28.000000 existenz_api_fetcher-0.1.0/tests/test_hydro.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)     1037 2022-10-17 08:25:28.000000 existenz_api_fetcher-0.1.0/tests/test_meteo.py
+-rwxrwxrwx   0 lilian    (1000) lilian    (1000)      305 2022-10-17 08:25:28.000000 existenz_api_fetcher-0.1.0/tests/test_pipelines.py
```

### Comparing `existenz_api_fetcher-0.0.9/LICENSE.txt` & `existenz_api_fetcher-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `existenz_api_fetcher-0.0.9/PKG-INFO` & `existenz_api_fetcher-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: existenz_api_fetcher
-Version: 0.0.9
+Version: 0.1.0
 Summary: Easily fetch swiss weather and hydrological data from the Existenz API
 Home-page: https://github.com/Lilian1510/ExistenzAPIFetcher/
 Author: Lilian Lonla
 Author-email: Lilian Lonla <lilianlonla15@gmail.com>
 Project-URL: Homepage, https://github.com/Lilian1510/ExistenzAPIFetcher/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,17 +20,18 @@
 
 Data is obtained by querying a two-year, daily time series from the InfluxDB database and is returned as a `pandas` dataframe.
 Functions to compute potential evapotranspiration using the `pyet` module have been implemented.
 Take a look at the Jupyter Notebooks tutorials in the examples directory to learn how to use the various functionalities of this package.
 
 ## Requirements
 ```
-influxdb_client>=1.32.0
-pandas>=1.4.3
-pyet>=1.1.0
+influxdb_client
+pandas
+pyet
+folium
 ```
 
 ## :gear: Installation
 To install the package from the PypI index:
 
 `pip install existenz_api_fetcher`
```

### Comparing `existenz_api_fetcher-0.0.9/README.md` & `existenz_api_fetcher-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 Data is obtained by querying a two-year, daily time series from the InfluxDB database and is returned as a `pandas` dataframe.
 Functions to compute potential evapotranspiration using the `pyet` module have been implemented.
 Take a look at the Jupyter Notebooks tutorials in the examples directory to learn how to use the various functionalities of this package.
 
 ## Requirements
 ```
-influxdb_client>=1.32.0
-pandas>=1.4.3
-pyet>=1.1.0
+influxdb_client
+pandas
+pyet
+folium
 ```
 
 ## :gear: Installation
 To install the package from the PypI index:
 
 `pip install existenz_api_fetcher`
```

### Comparing `existenz_api_fetcher-0.0.9/existenz_api_fetcher/hydro.py` & `existenz_api_fetcher-0.1.0/existenz_api_fetcher/hydro.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import warnings
-
+from typing import Union
+import pandas as pd
 from influxdb_client import InfluxDBClient
 from influxdb_client.client.warnings import MissingPivotFunction
 
 from existenz_api_fetcher import pipelines
 
 warnings.simplefilter("ignore", MissingPivotFunction)
 
@@ -12,15 +13,15 @@
 org = "api.existenz.ch"
 bucket = "existenzApi"
 token = "0yLbh-D7RMe1sX1iIudFel8CcqCI8sVfuRTaliUp56MgE6kub8-nSd05_EJ4zTTKt0lUzw8zcO73zL9QhC3jtA=="
 client = InfluxDBClient(url=url, token=token, org=org)
 query_api = client.query_api()
 
 
-def flow(station: str) -> object:
+def flow(station: str) -> Union[None, pd.DataFrame]:
     """
     Returns 2 years of streamflow [m3/s] data in the form of a pandas dataframe. Note that not all stations measure streamflow.
     Args: FOEN station code (str). Use the locations.maps() function to open a map with all the stations for more info
     Returns: DataFrame with a datetime index
     """
     flow_df = query_api.query_data_frame('from(bucket:"existenzApi") '
                                          '|> range(start: -2y)'
@@ -30,15 +31,15 @@
                                          '|> aggregateWindow(every: 1d, fn: mean, createEmpty: false)'
                                          '|> yield(name: "mean")'
                                          )
     flow_df = pipelines.preprocess(flow_df)
     return flow_df
 
 
-def temperature(station: str) -> object:
+def temperature(station: str) -> Union[None, pd.DataFrame]:
     """
     Returns 2 years of water temperature [°C] data in the form of a pandas dataframe. Note that not all stations measure water temperature.
     Args: FOEN station code (str). Use the locations.maps() function to open a map with all the stations for more info
     Returns: DataFrame with a datetime index
     """
     t_df = query_api.query_data_frame('from(bucket:"existenzApi") '
                                       '|> range(start: -2y)'
@@ -52,15 +53,15 @@
         t_df = pipelines.preprocess(t_df)
         return t_df
     else:
         print(f"Station {station} does not measure water temperature...")
         return None
 
 
-def height(station: str) -> object:
+def height(station: str) -> Union[None, pd.DataFrame]:
     """
     Returns 2 years of River or lake height [m over sea level] data in the form of a pandas dataframe.
     Args: FOEN station code (str). Use the locations.maps() function to open a map with all the stations for more info
     Returns: DataFrame with a datetime index
     """
     h_df = query_api.query_data_frame('from(bucket:"existenzApi") '
                                       '|> range(start: -2y)'
```

### Comparing `existenz_api_fetcher-0.0.9/existenz_api_fetcher/meteo.py` & `existenz_api_fetcher-0.1.0/existenz_api_fetcher/meteo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import warnings
-
+from typing import Union
+import pandas as pd
 from influxdb_client import InfluxDBClient
 from influxdb_client.client.warnings import MissingPivotFunction
-from pyet import penman, pm, pm_fao56
+from pyet import penman, pm, pm_fao56, deg_to_rad
 
 from existenz_api_fetcher import pipelines
 
 warnings.simplefilter("ignore", MissingPivotFunction)
 
 # Influx DB client configuration
 url = "https://influx.konzept.space/"
 org = "api.existenz.ch"
 bucket = "existenzApi"
 token = "0yLbh-D7RMe1sX1iIudFel8CcqCI8sVfuRTaliUp56MgE6kub8-nSd05_EJ4zTTKt0lUzw8zcO73zL9QhC3jtA=="
 client = InfluxDBClient(url=url, token=token, org=org)
 query_api = client.query_api()
 
 
-def rainfall(station: str):
+def rainfall(station: str) -> pd.DataFrame:
     """
     Returns 2 years of rainfall [mm/day] data in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
     Returns: DataFrame with a datetime index
     """
     rr_df = query_api.query_data_frame('from(bucket: "existenzApi")'
                                        '|> range(start: -2y)'
@@ -31,15 +32,15 @@
                                        '|> aggregateWindow(every: 1d, fn: sum, createEmpty: true)'
                                        '|> yield(name: "cumulative_sum")'
                                        )
     rr_df = pipelines.preprocess(rr_df)
     return rr_df
 
 
-def temperature(station: str):
+def temperature(station: str) -> pd.DataFrame:
     """
     Returns 2 years of mean temperature [°C] data in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
     Returns: DataFrame with a datetime index
     """
     tt_df = query_api.query_data_frame('from(bucket: "existenzApi")'
                                        '|> range(start: -2y)'
@@ -49,15 +50,15 @@
                                        '|> aggregateWindow(every: 1d, fn: mean, createEmpty: true)'
                                        '|> yield(name: "mean")'
                                        )
     tt_df = pipelines.preprocess(tt_df)
     return tt_df
 
 
-def min_temperature(station: str):
+def min_temperature(station: str) -> pd.DataFrame:
     """
     Returns 2 years of minimum temperature [°C] data in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
     Returns: DataFrame with a datetime index
     """
     mintt_df = query_api.query_data_frame('from(bucket: "existenzApi")'
                                           '|> range(start: -2y)'
@@ -67,15 +68,15 @@
                                           '|> aggregateWindow(every: 1d, fn: min, createEmpty: true)'
                                           '|> yield(name: "mean")'
                                           )
     mintt_df = pipelines.preprocess(mintt_df)
     return mintt_df
 
 
-def max_temperature(station: str):
+def max_temperature(station: str) -> pd.DataFrame:
     """
     Returns 2 years of maximum temperature [°C] data in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
     Returns: DataFrame with a datetime index
     """
     # Maximum temperature[°C]
     maxtt_df = query_api.query_data_frame('from(bucket: "existenzApi")'
@@ -86,15 +87,15 @@
                                           '|> aggregateWindow(every: 1d, fn: max, createEmpty: true)'
                                           '|> yield(name: "mean")'
                                           )
     maxtt_df = pipelines.preprocess(maxtt_df)
     return maxtt_df
 
 
-def humidity(station: str):
+def humidity(station: str) -> pd.DataFrame:
     """
     Returns 2 years of relative humidity [%] data in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
     Returns: DataFrame with a datetime index
     """
     rh_df = query_api.query_data_frame('from(bucket: "existenzApi")'
                                        '|> range(start: -2y)'
@@ -103,15 +104,15 @@
                                        '|> filter(fn: (r) => r["_field"] == "rh")'
                                        '|> aggregateWindow(every: 1d, fn: mean, createEmpty: true)'
                                        '|> yield(name: "mean")')
     rh_df = pipelines.preprocess(rh_df)
     return rh_df
 
 
-def wind_speed(station: str):
+def wind_speed(station: str) -> pd.DataFrame:
     """
     Returns 2 years of wind speed [km/h] data in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
     Returns: DataFrame with a datetime index
     """
     ff_df = query_api.query_data_frame('from(bucket: "existenzApi")'
                                        '|> range(start: -2y) '
@@ -121,35 +122,35 @@
                                        '|> aggregateWindow(every: 1d, fn: mean, createEmpty: true)'
                                        '|> yield(name: "mean")'
                                        )
     ff_df = pipelines.preprocess(ff_df)
     return ff_df
 
 
-def radiation(station: str):
+def radiation(station: str) -> pd.DataFrame:
     """
-    Returns 2 years of radiation intensity [W/m2] data in the form of a pandas dataframe.
+    Returns 2 years of radiation intensity [W/m2] (ten minutes mean) data in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
     Returns: DataFrame with a datetime index
     """
     rad_df = query_api.query_data_frame('from(bucket: "existenzApi")'
                                         '|> range(start: -2y) '
                                         '|> filter(fn: (r) => r["_measurement"] == "smn")'
                                         f'|> filter(fn: (r) => r["loc"] == "{station}")'
                                         '|> filter(fn: (r) => r["_field"] == "rad")'
                                         '|> aggregateWindow(every: 1d, fn: mean, createEmpty: true)'
                                         '|> yield(name: "mean")'
                                         )
     rad_df = pipelines.preprocess(rad_df)
     # Convert from W/m2 to MJ/m2/d
-    rad_df['_value'] = rad_df['_value'] * 10e-6 * 60*60*24
+    rad_df['_value'] = rad_df['_value'] * 10/60/24 * 10e-6
     return rad_df
 
 
-def pressure(station: str):
+def pressure(station: str) -> pd.DataFrame:
     """
     Returns 2 years of pressure at station level [hPa] data in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
     Returns: DataFrame with a datetime index
     """
     qfe_df = query_api.query_data_frame('from(bucket: "existenzApi")'
                                         '|> range(start: -2y) '
@@ -159,15 +160,15 @@
                                         '|> aggregateWindow(every: 1d, fn: mean, createEmpty: true)'
                                         '|> yield(name: "mean")'
                                         )
     qfe_df = pipelines.preprocess(qfe_df)
     return qfe_df
 
 
-def sunshine_duration(station: str):
+def sunshine_duration(station: str) -> pd.DataFrame:
     """
     Returns 2 years of sunshine duration [min] data in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
     Returns: DataFrame with a datetime index
     """
     ss_df = query_api.query_data_frame('from(bucket: "existenzApi")'
                                        '|> range(start: -2y) '
@@ -177,15 +178,15 @@
                                        '|> aggregateWindow(every: 1d, fn: mean, createEmpty: true)'
                                        '|> yield(name: "mean")'
                                        )
     ss_df = pipelines.preprocess(ss_df)
     return ss_df
 
 
-def dew_point(station: str):
+def dew_point(station: str) -> pd.DataFrame:
     """
     Returns 2 years of dew point (2 m above ground) data in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
     Returns: DataFrame with a datetime index
     """
     td_df = query_api.query_data_frame('from(bucket: "existenzApi")'
                                        '|> range(start: -2y) '
@@ -195,68 +196,68 @@
                                        '|> aggregateWindow(every: 1d, fn: mean, createEmpty: true)'
                                        '|> yield(name: "mean")'
                                        )
     td_df = pipelines.preprocess(td_df)
     return td_df
 
 
-def ev_penman(station: str, elevation: int, lat: float):
+def ev_penman(station: str, elevation: int, lat: float) -> Union[None, pd.DataFrame]:
     """
     Returns 2 years of potential evapotranspiration data (computed according to Penman (1948)) in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
           Station elevation (int), station latitude (float). Use the locations.geolocate() function to find these parameters.
     Returns: DataFrame with a datetime index
     """
     penman_df = pipelines.compute(radiation(station))
     if penman_df is None:
         return None
     else:
         # Compute potential evaporation with Penman equation
         ev = penman(tmean=temperature(station)['_value'], wind=wind_speed(station)['_value'],
                     rs=radiation(station)['_value'], elevation=elevation,
-                    lat=lat, tmax=max_temperature(station)['_value'], tmin=min_temperature(station)['_value'],
+                    lat=deg_to_rad(lat), tmax=max_temperature(station)['_value'], tmin=min_temperature(station)['_value'],
                     rh=humidity(station)['_value'])
         # Interpolate missing data
         penman_df['_value'] = ev.interpolate()
         return penman_df
 
 
-def ev_penman_monteith(station: str, elevation: int, lat: float):
+def ev_penman_monteith(station: str, elevation: int, lat: float) -> Union[None, pd.DataFrame]:
     """
     Returns 2 years of potential evapotranspiration data (computed according to Monteith (1965)) in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
           Station elevation (int), station latitude (float). Use the locations.geolocate() function to find these parameters.
     Returns: DataFrame with a datetime index
     """
     pm_df = pipelines.compute(radiation(station))
     if pm_df is None:
         return None
     else:
         # Compute potential evaporation with Penman-Monteith equation
         ev = pm(tmean=temperature(station)['_value'], wind=wind_speed(station)['_value'],
                 rs=radiation(station)['_value'], elevation=elevation,
-                lat=lat, tmax=max_temperature(station)['_value'], tmin=min_temperature(station)['_value'],
+                lat=deg_to_rad(lat), tmax=max_temperature(station)['_value'], tmin=min_temperature(station)['_value'],
                 rh=humidity(station)['_value'])
         # Interpolate missing data
         pm_df['_value'] = ev.interpolate()
         return pm_df
 
 
-def ev_fao56(station: str, elevation: int, lat: float):
+def ev_fao56(station: str, elevation: int, lat: float) ->  Union[None, pd.DataFrame]:
     """
     Returns 2 years of potential evapotranspiration data (computed according to Allen et al. (1998)) in the form of a pandas dataframe.
     Args: MeteoSwiss station code (str). Use the locations.map() function to open a map with all the stations for more info.
           Station elevation (int), station latitude (float). Use the locations.geolocate() function to find these parameters.
     Returns: DataFrame with a datetime index
     """
     fao_df = pipelines.compute(radiation(station))
     if fao_df is None:
         return None
     else:
         # Compute potential evaporation with Fao56 equation
         ev = pm_fao56(tmean=temperature(station)['_value'], wind=wind_speed(station)['_value'],
                       rs=radiation(station)['_value'], elevation=elevation,
-                      lat=lat, tmax=max_temperature(station)['_value'], tmin=min_temperature(station)['_value'],
+                      lat=deg_to_rad(lat), tmax=max_temperature(station)['_value'], tmin=min_temperature(station)['_value'],
                       rh=humidity(station)['_value'])
         # Interpolate missing data
         fao_df['_value'] = ev.interpolate()
-        return fao_df
+        return fao_df
```

### Comparing `existenz_api_fetcher-0.0.9/existenz_api_fetcher/pipelines.py` & `existenz_api_fetcher-0.1.0/existenz_api_fetcher/pipelines.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import reduce
-
+from typing import Union
 import pandas as pd
 
 
-def preprocess(df):
+def preprocess(df: pd.DataFrame) -> Union[None, pd.DataFrame]:
     """
     Batch processes a DataFrame to make it easier to use.
     Args: DataFrame
     Return: Processed Dataframe
     """
     if df.empty:
         return None
@@ -18,15 +18,15 @@
         df['_value'] = df['_value'].interpolate(method="time")  # Interpolate missing data
         df.index = df.index.to_series().apply(lambda x: x.date()) # Removes unnecessary time
         # Converting the index as date
         df.index = pd.to_datetime(df.index)
         return df
 
 
-def compute(df):
+def compute(df: pd.DataFrame) -> Union[None, pd.DataFrame]:
     """
     Generates a dataframe from an existing one.
     Args: DataFrame
     Return: New Dataframe
     """
     if df is None:
         return None
@@ -34,15 +34,15 @@
         new_df = df.filter(['_value'], axis=1)
         new_df.index = df.index
         new_df['_field'] = 'pet'
         new_df = new_df[["_value"]]
         return new_df
 
 
-def merge(*args):
+def merge(*args) -> Union[None, pd.DataFrame]:
     """
     Function to merge DataFrames.
     *Args: Dataframes
     Returns: DataFrame with DateTime index and all parameters as columns
     """
     if len(args) == 1:
         return args[0]
```

### Comparing `existenz_api_fetcher-0.0.9/existenz_api_fetcher.egg-info/PKG-INFO` & `existenz_api_fetcher-0.1.0/existenz_api_fetcher.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: existenz-api-fetcher
-Version: 0.0.9
+Version: 0.1.0
 Summary: Easily fetch swiss weather and hydrological data from the Existenz API
 Home-page: https://github.com/Lilian1510/ExistenzAPIFetcher/
 Author: Lilian Lonla
 Author-email: Lilian Lonla <lilianlonla15@gmail.com>
 Project-URL: Homepage, https://github.com/Lilian1510/ExistenzAPIFetcher/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,17 +20,18 @@
 
 Data is obtained by querying a two-year, daily time series from the InfluxDB database and is returned as a `pandas` dataframe.
 Functions to compute potential evapotranspiration using the `pyet` module have been implemented.
 Take a look at the Jupyter Notebooks tutorials in the examples directory to learn how to use the various functionalities of this package.
 
 ## Requirements
 ```
-influxdb_client>=1.32.0
-pandas>=1.4.3
-pyet>=1.1.0
+influxdb_client
+pandas
+pyet
+folium
 ```
 
 ## :gear: Installation
 To install the package from the PypI index:
 
 `pip install existenz_api_fetcher`
```

### Comparing `existenz_api_fetcher-0.0.9/pyproject.toml` & `existenz_api_fetcher-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "existenz_api_fetcher"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
 	{name="Lilian Lonla", email="lilianlonla15@gmail.com"}
 ]
 description = "Easily fetch swiss weather and hydrological data from the Existenz API"
 readme = "README.md"
 classifiers = [
 	"Programming Language :: Python :: 3",
```

### Comparing `existenz_api_fetcher-0.0.9/setup.py` & `existenz_api_fetcher-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='existenz_api_fetcher',
-    version='0.0.9',
+    version='0.1.0',
     author='Lilian Lonla',
     author_email='lilianlonla15@gmail.com',
     description='Easily fetch swiss weather and hydrological data from the Existenz API',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Lilian1510/ExistenzAPIFetcher/',
     packages=setuptools.find_packages(),
     install_requires=[
         'influxdb_client>=1.32.0',
-        'pandas>=1.4.3',
+        'pandas==2.0.2',
         'pyet>=1.1.0',
-        'setuptools==67.7.2'
+        'folium>=0.14.0',
+        'setuptools==68.0.0'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
```

### Comparing `existenz_api_fetcher-0.0.9/tests/test_meteo.py` & `existenz_api_fetcher-0.1.0/tests/test_meteo.py`

 * *Files identical despite different names*

