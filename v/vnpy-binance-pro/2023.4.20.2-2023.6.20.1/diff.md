# Comparing `tmp/vnpy_binance_pro-2023.4.20.2.tar.gz` & `tmp/vnpy_binance_pro-2023.6.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_binance_pro-2023.4.20.2.tar", last modified: Thu Apr 20 09:50:55 2023, max compression
+gzip compressed data, was "vnpy_binance_pro-2023.6.20.1.tar", last modified: Tue Jun 20 09:45:30 2023, max compression
```

## Comparing `vnpy_binance_pro-2023.4.20.2.tar` & `vnpy_binance_pro-2023.6.20.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-20 09:50:55.869765 vnpy_binance_pro-2023.4.20.2/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1066 2023-04-20 08:16:53.000000 vnpy_binance_pro-2023.4.20.2/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2126 2023-04-20 09:50:55.869866 vnpy_binance_pro-2023.4.20.2/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1165 2023-04-20 08:16:53.000000 vnpy_binance_pro-2023.4.20.2/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1028 2023-04-20 09:50:55.870413 vnpy_binance_pro-2023.4.20.2/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-04-20 08:16:53.000000 vnpy_binance_pro-2023.4.20.2/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-20 09:50:55.867519 vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1460 2023-04-20 08:16:53.000000 vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    31285 2023-04-20 08:16:53.000000 vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro/binance_inverse_gateway.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    29183 2023-04-20 09:27:23.000000 vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro/binance_spot_gateway.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    31907 2023-04-20 09:43:38.000000 vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro/binance_usdt_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-04-20 09:50:55.869565 vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2126 2023-04-20 09:50:55.000000 vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      429 2023-04-20 09:50:55.000000 vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-20 09:50:55.000000 vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-04-20 08:47:50.000000 vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-04-20 09:50:55.000000 vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       17 2023-04-20 09:50:55.000000 vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-20 09:45:30.567106 vnpy_binance_pro-2023.6.20.1/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1066 2023-06-20 09:41:43.000000 vnpy_binance_pro-2023.6.20.1/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2126 2023-06-20 09:45:30.567204 vnpy_binance_pro-2023.6.20.1/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1165 2023-06-20 09:41:43.000000 vnpy_binance_pro-2023.6.20.1/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1028 2023-06-20 09:45:30.567668 vnpy_binance_pro-2023.6.20.1/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-06-20 09:41:43.000000 vnpy_binance_pro-2023.6.20.1/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-20 09:45:30.565253 vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1460 2023-06-20 09:41:43.000000 vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    31283 2023-06-20 09:43:04.000000 vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro/binance_inverse_gateway.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    29183 2023-06-20 09:41:43.000000 vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro/binance_spot_gateway.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    31905 2023-06-20 09:43:04.000000 vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro/binance_usdt_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-20 09:45:30.566916 vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     2126 2023-06-20 09:45:30.000000 vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      429 2023-06-20 09:45:30.000000 vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-20 09:45:30.000000 vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-20 09:45:30.000000 vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-20 09:45:30.000000 vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       17 2023-06-20 09:45:30.000000 vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro.egg-info/top_level.txt
```

### Comparing `vnpy_binance_pro-2023.4.20.2/LICENSE` & `vnpy_binance_pro-2023.6.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_binance_pro-2023.4.20.2/PKG-INFO` & `vnpy_binance_pro-2023.6.20.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_binance_pro
-Version: 2023.4.20.2
+Version: 2023.6.20.1
 Summary: BINANCE gateway for vn.py quant trading framework.
 Home-page: https://github.com/monk-after-90s/vnpy-binance-pro
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy_binance_pro-2023.4.20.2/README.md` & `vnpy_binance_pro-2023.6.20.1/README.md`

 * *Files identical despite different names*

### Comparing `vnpy_binance_pro-2023.4.20.2/setup.cfg` & `vnpy_binance_pro-2023.6.20.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy_binance_pro
-version = 2023.4.20.2
+version = 2023.6.20.1
 url = https://github.com/monk-after-90s/vnpy-binance-pro
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = BINANCE gateway for vn.py quant trading framework.
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro/__init__.py` & `vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro/binance_inverse_gateway.py` & `vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro/binance_inverse_gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 DIRECTION_VT2BINANCES: Dict[Direction, str] = {
     Direction.LONG: "BUY",
     Direction.SHORT: "SELL"
 }
 DIRECTION_BINANCES2VT: Dict[str, Direction] = {v: k for k, v in DIRECTION_VT2BINANCES.items()}
 
 # 数据频率映射
-INTERVAL_VT2BINANCES: Dict[Interval, str] = {
+INTERVAL_VT2BINANCE: Dict[Interval, str] = {
     Interval.MINUTE: "1m",
     Interval.HOUR: "1h",
     Interval.DAILY: "1d",
 }
 
 # 时间间隔映射
 TIMEDELTA_MAP: Dict[Interval, timedelta] = {
@@ -667,15 +667,15 @@
         limit: int = 1500
         end_time: int = int(datetime.timestamp(req.end))
 
         while True:
             # 创建查询参数
             params: dict = {
                 "symbol": req.symbol,
-                "interval": INTERVAL_VT2BINANCES[req.interval],
+                "interval": INTERVAL_VT2BINANCE[req.interval],
                 "limit": limit
             }
 
             params["endTime"] = end_time * 1000
             path: str = "/dapi/v1/klines"
             if req.start:
                 start_time = int(datetime.timestamp(req.start))
```

### Comparing `vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro/binance_spot_gateway.py` & `vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro/binance_spot_gateway.py`

 * *Files identical despite different names*

### Comparing `vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro/binance_usdt_gateway.py` & `vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro/binance_usdt_gateway.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 DIRECTION_VT2BINANCES: Dict[Direction, str] = {
     Direction.LONG: "BUY",
     Direction.SHORT: "SELL"
 }
 DIRECTION_BINANCES2VT: Dict[str, Direction] = {v: k for k, v in DIRECTION_VT2BINANCES.items()}
 
 # 数据频率映射
-INTERVAL_VT2BINANCES: Dict[Interval, str] = {
+INTERVAL_VT2BINANCE: Dict[Interval, str] = {
     Interval.MINUTE: "1m",
     Interval.HOUR: "1h",
     Interval.DAILY: "1d",
 }
 
 # 时间间隔映射
 TIMEDELTA_MAP: Dict[Interval, timedelta] = {
@@ -672,15 +672,15 @@
         start_time: int = int(datetime.timestamp(req.start))
 
         sleep_seconds = 0.5
         while True:
             # 创建查询参数
             params: dict = {
                 "symbol": req.symbol,
-                "interval": INTERVAL_VT2BINANCES[req.interval],
+                "interval": INTERVAL_VT2BINANCE[req.interval],
                 "limit": limit
             }
 
             params["startTime"] = start_time * 1000
             path: str = "/fapi/v1/klines"
             if req.end:
                 end_time: int = int(datetime.timestamp(req.end))
```

### Comparing `vnpy_binance_pro-2023.4.20.2/vnpy_binance_pro.egg-info/PKG-INFO` & `vnpy_binance_pro-2023.6.20.1/vnpy_binance_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-binance-pro
-Version: 2023.4.20.2
+Version: 2023.6.20.1
 Summary: BINANCE gateway for vn.py quant trading framework.
 Home-page: https://github.com/monk-after-90s/vnpy-binance-pro
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

