# Comparing `tmp/dwclib-2023.6.20.tar.gz` & `tmp/dwclib-2023.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwclib-2023.6.20.tar", max compression
+gzip compressed data, was "dwclib-2023.6.7.tar", max compression
```

## Comparing `dwclib-2023.6.20.tar` & `dwclib-2023.6.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      753 2022-06-09 12:54:18.472933 dwclib-2023.6.20/LICENSE
--rw-r--r--   0        0        0     1396 2023-06-19 11:43:33.517768 dwclib-2023.6.20/README.md
--rw-r--r--   0        0        0      808 2023-06-20 11:01:24.005748 dwclib-2023.6.20/pyproject.toml
--rw-r--r--   0        0        0      433 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/__init__.py
--rw-r--r--   0        0        0       59 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/alerts/__init__.py
--rw-r--r--   0        0        0     2672 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/alerts/alerts.py
--rw-r--r--   0        0        0        0 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/assets/__init__.py
--rw-r--r--   0        0        0   173360 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/assets/alert_ref.csv
--rw-r--r--   0        0        0     1346 2023-06-20 11:00:59.901656 dwclib-2023.6.20/src/dwclib/common/db.py
--rw-r--r--   0        0        0     1178 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/common/meta.py
--rw-r--r--   0        0        0     2399 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/common/numerics.py
--rw-r--r--   0        0        0     1407 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/common/wave_unfold.py
--rw-r--r--   0        0        0     2179 2023-06-20 10:59:11.813240 dwclib-2023.6.20/src/dwclib/common/waves.py
--rw-r--r--   0        0        0      153 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/dask/__init__.py
--rw-r--r--   0        0        0      917 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/dask/generic.py
--rw-r--r--   0        0        0      820 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/dask/numerics.py
--rw-r--r--   0        0        0      817 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/dask/waves.py
--rw-r--r--   0        0        0     1419 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/dask/waves_convert.py
--rw-r--r--   0        0        0       65 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/numerics/__init__.py
--rw-r--r--   0        0        0     1551 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/numerics/numerics.py
--rw-r--r--   0        0        0       95 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/patients/__init__.py
--rw-r--r--   0        0        0     4141 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/patients/patients.py
--rw-r--r--   0        0        0       56 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/waves/__init__.py
--rw-r--r--   0        0        0     1334 2023-06-19 11:43:33.517768 dwclib-2023.6.20/src/dwclib/waves/waves.py
--rw-r--r--   0        0        0     2203 1970-01-01 00:00:00.000000 dwclib-2023.6.20/PKG-INFO
+-rw-r--r--   0        0        0      753 2022-06-09 12:54:18.472933 dwclib-2023.6.7/LICENSE
+-rw-r--r--   0        0        0     1263 2022-09-14 11:01:06.119049 dwclib-2023.6.7/README.md
+-rw-r--r--   0        0        0      823 2023-06-07 10:28:17.376535 dwclib-2023.6.7/pyproject.toml
+-rw-r--r--   0        0        0      433 2023-02-28 15:26:04.174955 dwclib-2023.6.7/src/dwclib/__init__.py
+-rw-r--r--   0        0        0       59 2023-02-28 15:26:04.174955 dwclib-2023.6.7/src/dwclib/alerts/__init__.py
+-rw-r--r--   0        0        0     2672 2023-03-03 15:13:00.467651 dwclib-2023.6.7/src/dwclib/alerts/alerts.py
+-rw-r--r--   0        0        0        0 2023-02-28 15:26:04.174955 dwclib-2023.6.7/src/dwclib/assets/__init__.py
+-rw-r--r--   0        0        0   173360 2023-03-03 14:48:35.668082 dwclib-2023.6.7/src/dwclib/assets/alert_ref.csv
+-rw-r--r--   0        0        0     1451 2023-02-28 15:26:04.178968 dwclib-2023.6.7/src/dwclib/common/db.py
+-rw-r--r--   0        0        0     1178 2023-02-28 15:26:04.178968 dwclib-2023.6.7/src/dwclib/common/meta.py
+-rw-r--r--   0        0        0     2398 2023-02-28 15:26:04.178968 dwclib-2023.6.7/src/dwclib/common/numerics.py
+-rw-r--r--   0        0        0     1397 2023-02-28 15:26:04.178968 dwclib-2023.6.7/src/dwclib/common/wave_unfold.py
+-rw-r--r--   0        0        0     2178 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/common/waves.py
+-rw-r--r--   0        0        0      153 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/__init__.py
+-rw-r--r--   0        0        0      917 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/generic.py
+-rw-r--r--   0        0        0      820 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/numerics.py
+-rw-r--r--   0        0        0      817 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/waves.py
+-rw-r--r--   0        0        0     1419 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/dask/waves_convert.py
+-rw-r--r--   0        0        0       65 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/numerics/__init__.py
+-rw-r--r--   0        0        0     1551 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/numerics/numerics.py
+-rw-r--r--   0        0        0       95 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/patients/__init__.py
+-rw-r--r--   0        0        0     4141 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/patients/patients.py
+-rw-r--r--   0        0        0       56 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/waves/__init__.py
+-rw-r--r--   0        0        0     1334 2023-02-28 15:26:04.182980 dwclib-2023.6.7/src/dwclib/waves/waves.py
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 dwclib-2023.6.7/PKG-INFO
```

### Comparing `dwclib-2023.6.20/LICENSE` & `dwclib-2023.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.20/README.md` & `dwclib-2023.6.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 Installation through conda greatly simplifies dependency management.
 
 Additionally, Microsoft SQL Server drivers are needed and will need to be installed seperately.
 See here for more information: https://github.com/mkleehammer/pyodbc/wiki
 
 
 ## Changelog
-- 2023.6.7
-    - Support for querying alerts using the read_alerts call
-    - Use the platformdirs package for config file location
-
 - 2022.9.14
     - Support numeric labels and sublabels in read_patients and read_numerics
     - Support to query for multiple patients at once in read_numerics
 
 - 2022.6.23
     - Convert packaging from flit to poetry
     - Add linting and testing with nox, flake8 and safety
```

### Comparing `dwclib-2023.6.20/pyproject.toml` & `dwclib-2023.6.7/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dwclib"
-version = "2023.6.20"
+version = "2023.6.7"
 description = "Python wrapper to DataWarehouse Connect"
 authors = ["Jona Joachim <jona@joachim.cc>"]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/larib-data/dwclib"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 numpy = "^1"
 pandas = ">=1.4,<3"
+numba = "~0.57"
 dask = ">=2022"
 SQLAlchemy = "~1.4"
 platformdirs = "^3.0.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 flake8-bandit = "^3.0.0"
```

### Comparing `dwclib-2023.6.20/src/dwclib/alerts/alerts.py` & `dwclib-2023.6.7/src/dwclib/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.20/src/dwclib/assets/alert_ref.csv` & `dwclib-2023.6.7/src/dwclib/assets/alert_ref.csv`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.20/src/dwclib/common/db.py` & `dwclib-2023.6.7/src/dwclib/common/db.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,41 +10,42 @@
     pyodbc.pooling = False
     odbcdriver = pyodbc.drivers()[0]
 except (ImportError, IndexError):
     odbcdriver = None
 
 from sqlalchemy.engine import URL
 
-config_dir = Path(user_config_dir(appname="larib-data", appauthor="larib-data"))
+config_dir = Path(user_config_dir(appname="dwclib", appauthor="larib-data"))
+config_dir.mkdir(parents=True, exist_ok=True)
 configfile = config_dir / "config.ini"
 
 
 if configfile.exists():
     config = ConfigParser()
     config.read(configfile)
-    dwcdriver = config.get('dwc', 'driver', fallback=odbcdriver)
+    dwcdriver = config.get('dwclib', 'dwc_driver', fallback=odbcdriver)
     if dwcdriver is None:
         warn('No ODBC driver found for DWC', RuntimeWarning)
 
     dwcuri = URL.create(
         'mssql+pyodbc',
-        username=config.get('dwc', 'user'),
-        password=config.get('dwc', 'pass'),
-        host=config.get('dwc', 'host'),
-        database=config.get('dwc', 'dbname'),
+        username=config.get('dwclib', 'dwc_user'),
+        password=config.get('dwclib', 'dwc_pass'),
+        host=config.get('dwclib', 'dwc_host'),
+        database=config.get('dwclib', 'dwc_dbname'),
         query={
             "driver": dwcdriver,
             "Encrypt": "no",
         },
     )
 
     pguri = URL.create(
         'postgresql',
-        username=config.get('dwcmeta', 'user'),
-        password=config.get('dwcmeta', 'pass'),
-        host=config.get('dwcmeta', 'host'),
-        database=config.get('dwcmeta', 'dbname'),
+        username=config.get('dwclib', 'dwcmeta_user'),
+        password=config.get('dwclib', 'dwcmeta_pass'),
+        host=config.get('dwclib', 'dwcmeta_host'),
+        database=config.get('dwclib', 'dwcmeta_dbname'),
     )
 else:
     warn(f"Configuration file {configfile} does not exist.", RuntimeWarning)
     dwcuri = None
     pguri = None
```

### Comparing `dwclib-2023.6.20/src/dwclib/common/meta.py` & `dwclib-2023.6.7/src/dwclib/common/meta.py`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.20/src/dwclib/common/numerics.py` & `dwclib-2023.6.7/src/dwclib/common/numerics.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         nn = nn.where(nnt.c.SubLabel.in_(sublabels))
     nn = nn.cte('Numeric')
 
     nv = select(nvt.c.TimeStamp, nvt.c.NumericId, nvt.c.Value, nvt.c.PatientId)
     nv = nv.with_hint(nvt, 'WITH (NOLOCK)')
     nv = nv.where(nvt.c.TimeStamp >= dtbegin)
     nv = nv.where(nvt.c.TimeStamp < dtend)
-    nv = nv.where(nvt.c.Value.is_not(None))
+    nv = nv.where(nvt.c.Value is not None)
     if patientids:
         if is_list_like(patientids):
             nv = nv.where(nvt.c.PatientId.in_(patientids))
         else:
             nv = nv.where(nvt.c.PatientId == patientids)
     nv = nv.cte('NumericValue')
```

### Comparing `dwclib-2023.6.20/src/dwclib/common/wave_unfold.py` & `dwclib-2023.6.7/src/dwclib/common/wave_unfold.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import pandas as pd
+from numba import njit
 
 
 def unfold_row(row: pd.Series, naive_datetime=True) -> pd.Series:
     # XXX unify following line once we use the same unfold_row function for pandas and dask
     begintime = row.name[0] if isinstance(row.name, tuple) else row.name
     basetime = 1000 * begintime.timestamp()
     msperiod = row['SamplePeriod']
@@ -19,20 +20,21 @@
     # Convert to datetime[64]
     timestamps = pd.to_datetime(timestamps, unit='ms', utc=True)
     if naive_datetime:
         timestamps = timestamps.to_numpy(dtype='datetime64[ns]')
     return pd.Series(realvals, index=timestamps)
 
 
+@njit
 def wave_unfold(indata: bytes, cau: float, cal: float, csu: int, csl: int):
     if len(indata) % 2:
         indata = indata[:-1]
     int16le = np.dtype('<i2')
     npindata = np.frombuffer(indata, dtype=int16le)
-    if any(np.isnan([cau, cal, csu, csl])) or (csu - csl) == 0:
-        m = 1
-        b = 0
-    else:
+    if (csu - csl) != 0:
         m = (cau - cal) / (csu - csl)
         b = cau - m * csu
+    else:
+        m = 1
+        b = 0
     outdata = m * npindata.astype(np.float32) + b
     return outdata
```

### Comparing `dwclib-2023.6.20/src/dwclib/common/waves.py` & `dwclib-2023.6.7/src/dwclib/common/waves.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         ww = ww.where(wwt.c.Label.in_(labels))
     ww = ww.cte('Wave')
 
     ws = select(wst.c.TimeStamp, wst.c.WaveId, wst.c.WaveSamples, wst.c.PatientId)
     ws = ws.with_hint(wst, 'WITH (NOLOCK)')
     ws = ws.where(wst.c.TimeStamp >= dtbegin)
     ws = ws.where(wst.c.TimeStamp < dtend)
-    ws = ws.where(wst.c.WaveSamples.is_not(None))
+    ws = ws.where(wst.c.WaveSamples is not None)
     if patientid:
         ws = ws.where(wst.c.PatientId == patientid)
     ws = ws.cte('WaveSample')
 
     j = join(ws, ww, ws.c.WaveId == ww.c.Id)
     q = select(
         ws.c.TimeStamp,
```

### Comparing `dwclib-2023.6.20/src/dwclib/dask/generic.py` & `dwclib-2023.6.7/src/dwclib/dask/generic.py`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.20/src/dwclib/dask/numerics.py` & `dwclib-2023.6.7/src/dwclib/dask/numerics.py`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.20/src/dwclib/dask/waves.py` & `dwclib-2023.6.7/src/dwclib/dask/waves.py`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.20/src/dwclib/dask/waves_convert.py` & `dwclib-2023.6.7/src/dwclib/dask/waves_convert.py`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.20/src/dwclib/numerics/numerics.py` & `dwclib-2023.6.7/src/dwclib/numerics/numerics.py`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.20/src/dwclib/patients/patients.py` & `dwclib-2023.6.7/src/dwclib/patients/patients.py`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.20/src/dwclib/waves/waves.py` & `dwclib-2023.6.7/src/dwclib/waves/waves.py`

 * *Files identical despite different names*

### Comparing `dwclib-2023.6.20/PKG-INFO` & `dwclib-2023.6.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dwclib
-Version: 2023.6.20
+Version: 2023.6.7
 Summary: Python wrapper to DataWarehouse Connect
 Home-page: https://github.com/larib-data/dwclib
 License: ISC
 Author: Jona Joachim
 Author-email: jona@joachim.cc
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=1.4,<1.5)
 Requires-Dist: dask (>=2022)
+Requires-Dist: numba (>=0.57,<0.58)
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: pandas (>=1.4,<3)
 Requires-Dist: platformdirs (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/larib-data/dwclib
 Description-Content-Type: text/markdown
 
 # Overview
@@ -33,18 +34,14 @@
 Installation through conda greatly simplifies dependency management.
 
 Additionally, Microsoft SQL Server drivers are needed and will need to be installed seperately.
 See here for more information: https://github.com/mkleehammer/pyodbc/wiki
 
 
 ## Changelog
-- 2023.6.7
-    - Support for querying alerts using the read_alerts call
-    - Use the platformdirs package for config file location
-
 - 2022.9.14
     - Support numeric labels and sublabels in read_patients and read_numerics
     - Support to query for multiple patients at once in read_numerics
 
 - 2022.6.23
     - Convert packaging from flit to poetry
     - Add linting and testing with nox, flake8 and safety
```

