# Comparing `tmp/nselib-0.3.tar.gz` & `tmp/nselib-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nselib-0.3.tar", last modified: Mon Jun 19 16:51:16 2023, max compression
+gzip compressed data, was "nselib-0.4.tar", last modified: Tue Jun 20 01:41:41 2023, max compression
```

## Comparing `nselib-0.3.tar` & `nselib-0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 16:51:16.019899 nselib-0.3/
--rw-rw-rw-   0        0        0    11558 2023-06-18 02:00:39.000000 nselib-0.3/LICENSE
--rw-rw-rw-   0        0        0        0 2023-06-18 00:57:58.000000 nselib-0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3052 2023-06-19 16:51:16.020407 nselib-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2359 2023-06-19 16:47:39.000000 nselib-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 16:51:15.970229 nselib-0.3/nselib/
--rw-rw-rw-   0        0        0        0 2023-06-17 23:08:53.000000 nselib-0.3/nselib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:51:15.993213 nselib-0.3/nselib/capital_market/
--rw-rw-rw-   0        0        0      227 2023-06-19 16:40:39.000000 nselib-0.3/nselib/capital_market/__init__.py
--rw-rw-rw-   0        0        0    15217 2023-06-19 16:39:21.000000 nselib-0.3/nselib/capital_market/capital_market_data.py
--rw-rw-rw-   0        0        0     2115 2023-06-19 08:30:28.000000 nselib-0.3/nselib/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:51:15.999211 nselib-0.3/nselib/debt/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:50:56.000000 nselib-0.3/nselib/debt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:51:16.008366 nselib-0.3/nselib/derivatives/
--rw-rw-rw-   0        0        0      168 2023-06-19 13:36:13.000000 nselib-0.3/nselib/derivatives/__init__.py
--rw-rw-rw-   0        0        0     9022 2023-06-19 16:34:43.000000 nselib-0.3/nselib/derivatives/derivative_data.py
--rw-rw-rw-   0        0        0     3026 2023-06-19 15:56:00.000000 nselib-0.3/nselib/libutil.py
--rw-rw-rw-   0        0        0      438 2023-06-18 06:43:26.000000 nselib-0.3/nselib/logger.py
--rw-rw-rw-   0        0        0       17 2023-06-19 16:47:39.000000 nselib-0.3/nselib/version.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:51:15.984768 nselib-0.3/nselib.egg-info/
--rw-rw-rw-   0        0        0     3052 2023-06-19 16:51:15.000000 nselib-0.3/nselib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-06-19 16:51:15.000000 nselib-0.3/nselib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 16:51:15.000000 nselib-0.3/nselib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-19 16:51:15.000000 nselib-0.3/nselib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 16:51:15.000000 nselib-0.3/nselib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 16:51:16.024431 nselib-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1011 2023-06-19 16:49:37.000000 nselib-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:41:41.571295 nselib-0.4/
+-rw-rw-rw-   0        0        0    11558 2023-06-18 02:00:39.000000 nselib-0.4/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:57:58.000000 nselib-0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3856 2023-06-20 01:41:41.571295 nselib-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3163 2023-06-20 01:20:48.000000 nselib-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 01:41:41.549257 nselib-0.4/nselib/
+-rw-rw-rw-   0        0        0       68 2023-06-20 01:25:54.000000 nselib-0.4/nselib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:41:41.561293 nselib-0.4/nselib/capital_market/
+-rw-rw-rw-   0        0        0      286 2023-06-20 01:15:48.000000 nselib-0.4/nselib/capital_market/__init__.py
+-rw-rw-rw-   0        0        0    16203 2023-06-20 01:25:54.000000 nselib-0.4/nselib/capital_market/capital_market_data.py
+-rw-rw-rw-   0        0        0     2133 2023-06-19 17:43:08.000000 nselib-0.4/nselib/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:41:41.563257 nselib-0.4/nselib/debt/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:50:56.000000 nselib-0.4/nselib/debt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:41:41.568257 nselib-0.4/nselib/derivatives/
+-rw-rw-rw-   0        0        0      168 2023-06-19 13:36:13.000000 nselib-0.4/nselib/derivatives/__init__.py
+-rw-rw-rw-   0        0        0     9032 2023-06-20 01:08:27.000000 nselib-0.4/nselib/derivatives/derivative_data.py
+-rw-rw-rw-   0        0        0     4495 2023-06-20 01:00:15.000000 nselib-0.4/nselib/libutil.py
+-rw-rw-rw-   0        0        0      438 2023-06-18 06:43:26.000000 nselib-0.4/nselib/logger.py
+-rw-rw-rw-   0        0        0       15 2023-06-20 01:25:54.000000 nselib-0.4/nselib/version.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:41:41.557257 nselib-0.4/nselib.egg-info/
+-rw-rw-rw-   0        0        0     3856 2023-06-20 01:41:41.000000 nselib-0.4/nselib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-06-20 01:41:41.000000 nselib-0.4/nselib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 01:41:41.000000 nselib-0.4/nselib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-20 01:41:41.000000 nselib-0.4/nselib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-20 01:41:41.000000 nselib-0.4/nselib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-20 01:41:41.572296 nselib-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2023-06-20 01:40:52.000000 nselib-0.4/setup.py
```

### Comparing `nselib-0.3/LICENSE` & `nselib-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nselib-0.3/PKG-INFO` & `nselib-0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nselib
-Version: 0.3
+Version: 0.4
 Summary: library to get NSE India data
 Home-page: https://github.com/RuchiTanmay/nselib
 Author: RuchiTanmay
 Author-email: ruchitanmay@gmail.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# NSElib 0.3
+# NSElib 0.4
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
@@ -39,33 +39,66 @@
 ```$pip install nselib```
 
 Upgrade
 
 ```$pip install nselib --upgrade```
 
 ## Function list
+
+### nselib
+* trading_holiday_calendar
+
+Example :
+
+import nselib
+
+data = nselib.trading_holiday_calendar()
+
 ### Capital Market
 * price_volume_and_deliverable_position_data 
 * price_volume_data
 * deliverable_position_data
 * bulk_deal_data
 * block_deals_data
 * short_selling_data
 * bhav_copy_with_delivery
 * bhav_copy
+* equity_list
+* fno_equity_list
+* nifty50_equity_list
+
+Example : 
+
+from nselib import capital_market 
+
+data = capital_market.price_volume_and_deliverable_position_data(symbol='SBIN', from_date='01-06-2023', to_date='10-06-2023')
+                                            
+OR
+
+data = capital_market.price_volume_and_deliverable_position_data(symbol='SBIN', period='1M')
 
 More functions will be available in future releases...
 
 ### Derivative
 * future_price_volume_data
 * option_price_volume_data
 * fno_bhav_copy
 * participant_wise_open_interest
 * participant_wise_trading_volume
 
+Example : 
+
+from nselib import derivatives
+
+data = derivatives.future_price_volume_data(symbol='SBIN', instrument='FUTSTK', from_date='01-06-2023', to_date='10-06-2023')
+
+OR
+
+data = derivatives.price_volume_and_deliverable_position_data(symbol='BANKNIFTY', instrument='FUTIDX', period='1M')
+
 More functions will be available in future releases...
 
 ### Debt
 
 More functions will be available in future releases...
```

### Comparing `nselib-0.3/README.md` & `nselib-0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# NSElib 0.3
+# NSElib 0.4
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
@@ -21,33 +21,66 @@
 ```$pip install nselib```
 
 Upgrade
 
 ```$pip install nselib --upgrade```
 
 ## Function list
+
+### nselib
+* trading_holiday_calendar
+
+Example :
+
+import nselib
+
+data = nselib.trading_holiday_calendar()
+
 ### Capital Market
 * price_volume_and_deliverable_position_data 
 * price_volume_data
 * deliverable_position_data
 * bulk_deal_data
 * block_deals_data
 * short_selling_data
 * bhav_copy_with_delivery
 * bhav_copy
+* equity_list
+* fno_equity_list
+* nifty50_equity_list
+
+Example : 
+
+from nselib import capital_market 
+
+data = capital_market.price_volume_and_deliverable_position_data(symbol='SBIN', from_date='01-06-2023', to_date='10-06-2023')
+                                            
+OR
+
+data = capital_market.price_volume_and_deliverable_position_data(symbol='SBIN', period='1M')
 
 More functions will be available in future releases...
 
 ### Derivative
 * future_price_volume_data
 * option_price_volume_data
 * fno_bhav_copy
 * participant_wise_open_interest
 * participant_wise_trading_volume
 
+Example : 
+
+from nselib import derivatives
+
+data = derivatives.future_price_volume_data(symbol='SBIN', instrument='FUTSTK', from_date='01-06-2023', to_date='10-06-2023')
+
+OR
+
+data = derivatives.price_volume_and_deliverable_position_data(symbol='BANKNIFTY', instrument='FUTIDX', period='1M')
+
 More functions will be available in future releases...
 
 ### Debt
 
 More functions will be available in future releases...
```

### Comparing `nselib-0.3/nselib/capital_market/capital_market_data.py` & `nselib-0.4/nselib/capital_market/capital_market_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import time
 import zipfile
 from io import BytesIO, StringIO
 from nselib.libutil import *
 from nselib.constants import *
 
 
-def price_volume_and_deliverable_position_data(symbol:str, from_date:str = None, to_date:str = None, period:str = None):
+def price_volume_and_deliverable_position_data(symbol: str, from_date: str = None, to_date: str = None,
+                                               period: str = None):
     """
     get Security wise price volume & Deliverable position data set. use get_nse_symbols() to get all symbols
     :param symbol: symbol eg: 'SBIN'
     :param from_date: '17-03-2022' ('dd-mm-YYYY')
     :param to_date: '17-06-2023' ('dd-mm-YYYY')
     :param period: use one {'1D': last day data,'1W': for last 7 days data,
                             '1M': from last month same date, '6M': last 6 month data, '1Y': from last year same date)
@@ -34,30 +35,30 @@
         data_df = get_price_volume_and_deliverable_position_data(symbol=symbol, from_date=start_date, to_date=end_date)
         from_date = from_date + dt.timedelta(365)
         load_days = (to_date - from_date).days
         nse_df = pd.concat([nse_df, data_df], ignore_index=True)
     return nse_df
 
 
-def get_price_volume_and_deliverable_position_data(symbol:str, from_date:str, to_date:str):
+def get_price_volume_and_deliverable_position_data(symbol: str, from_date: str, to_date: str):
     # print(from_date, to_date)
     data_df = pd.DataFrame()
     url = "https://www.nseindia.com/api/historical/securityArchives?"
     payload = f"from={from_date}&to={to_date}&symbol={symbol}&dataType=priceVolumeDeliverable&series=ALL&csv=true"
-    data_text = nse_urlfetch(url+payload).text
-    data_text = data_text.replace('\x82','').replace('â¹', 'In Rs')
+    data_text = nse_urlfetch(url + payload).text
+    data_text = data_text.replace('\x82', '').replace('â¹', 'In Rs')
     with open('file.csv', 'w') as f:
         f.write(data_text)
     f.close()
     data_df = pd.read_csv('file.csv')
-    data_df.columns = [name.replace(' ','') for name in data_df.columns]
+    data_df.columns = [name.replace(' ', '') for name in data_df.columns]
     return data_df
 
 
-def price_volume_data(symbol:str, from_date:str = None, to_date:str = None, period:str = None):
+def price_volume_data(symbol: str, from_date: str = None, to_date: str = None, period: str = None):
     """
     get Security wise price volume data set.
     :param symbol: symbol eg: 'SBIN'
     :param from_date: '17-03-2022' ('dd-mm-YYYY')
     :param to_date: '17-06-2023' ('dd-mm-YYYY')
     :param period: use one {'1D': last day data,'1W': for last 7 days data,
                             '1M': from last month same date, '6M': last 6 month data, '1Y': from last year same date)
@@ -80,28 +81,28 @@
         data_df = get_price_volume_data(symbol=symbol, from_date=start_date, to_date=end_date)
         from_date = from_date + dt.timedelta(365)
         load_days = (to_date - from_date).days
         nse_df = pd.concat([nse_df, data_df], ignore_index=True)
     return nse_df
 
 
-def get_price_volume_data(symbol:str, from_date:str, to_date:str):
+def get_price_volume_data(symbol: str, from_date: str, to_date: str):
     # print(from_date, to_date)
     url = "https://www.nseindia.com/api/historical/securityArchives?"
     payload = f"from={from_date}&to={to_date}&symbol={symbol}&dataType=priceVolume&series=ALL&csv=true"
-    data_text = nse_urlfetch(url+payload).text
+    data_text = nse_urlfetch(url + payload).text
     with open('file.csv', 'w') as f:
         f.write(data_text)
     f.close()
     data_df = pd.read_csv('file.csv')
-    data_df.columns = [name.replace(' ','') for name in data_df.columns]
+    data_df.columns = [name.replace(' ', '') for name in data_df.columns]
     return data_df
 
 
-def deliverable_position_data(symbol:str, from_date:str = None, to_date:str = None, period:str = None):
+def deliverable_position_data(symbol: str, from_date: str = None, to_date: str = None, period: str = None):
     """
     get Security wise deliverable position data set.
     :param symbol: symbol eg: 'SBIN'
     :param from_date: '17-03-2022' ('dd-mm-YYYY')
     :param to_date: '17-06-2023' ('dd-mm-YYYY')
     :param period: use one {'1D': last day data,
                             '1W': for last 7 days data,
@@ -127,29 +128,29 @@
         data_df = get_price_volume_data(symbol=symbol, from_date=start_date, to_date=end_date)
         from_date = from_date + dt.timedelta(365)
         load_days = (to_date - from_date).days
         nse_df = pd.concat([nse_df, data_df], ignore_index=True)
     return nse_df
 
 
-def get_deliverable_position_data(symbol:str, from_date:str, to_date:str):
+def get_deliverable_position_data(symbol: str, from_date: str, to_date: str):
     # print(from_date, to_date)
     url = "https://www.nseindia.com/api/historical/securityArchives?"
     payload = f"from={from_date}&to={to_date}&symbol={symbol}&dataType=deliverable&series=ALL&csv=true"
-    data_text = nse_urlfetch(url+payload).text
+    data_text = nse_urlfetch(url + payload).text
     # data_text = data_text.replace('\x82','').replace('â¹', 'In Rs')
     with open('file.csv', 'w') as f:
         f.write(data_text)
     f.close()
     data_df = pd.read_csv('file.csv')
-    data_df.columns = [name.replace(' ','') for name in data_df.columns]
+    data_df.columns = [name.replace(' ', '') for name in data_df.columns]
     return data_df
 
 
-def bulk_deal_data(from_date:str = None, to_date:str = None, period:str = None):
+def bulk_deal_data(from_date: str = None, to_date: str = None, period: str = None):
     """
     get bulk deal data set.
     :param from_date: '17-03-2022' ('dd-mm-YYYY')
     :param to_date: '17-06-2023' ('dd-mm-YYYY')
     :param period: use one {'1D': last day data,
                             '1W': for last 7 days data,
                             '1M': from last month same date,
@@ -174,29 +175,29 @@
         data_df = get_bulk_deal_data(from_date=start_date, to_date=end_date)
         from_date = from_date + dt.timedelta(365)
         load_days = (to_date - from_date).days
         nse_df = pd.concat([nse_df, data_df], ignore_index=True)
     return nse_df
 
 
-def get_bulk_deal_data(from_date:str, to_date:str):
+def get_bulk_deal_data(from_date: str, to_date: str):
     # print(from_date, to_date)
     url = "https://www.nseindia.com/api/historical/bulk-deals?"
     payload = f"from={from_date}&to={to_date}&csv=true"
-    data_text = nse_urlfetch(url+payload).text
+    data_text = nse_urlfetch(url + payload).text
     # data_text = data_text.replace('\x82','').replace('â¹', 'In Rs')
     with open('file.csv', 'w') as f:
         f.write(data_text)
     f.close()
     data_df = pd.read_csv('file.csv')
-    data_df.columns = [name.replace(' ','') for name in data_df.columns]
+    data_df.columns = [name.replace(' ', '') for name in data_df.columns]
     return data_df
 
 
-def block_deals_data(from_date:str = None, to_date:str = None, period:str = None):
+def block_deals_data(from_date: str = None, to_date: str = None, period: str = None):
     """
     get block deals data set.
     :param from_date: '17-03-2022' ('dd-mm-YYYY')
     :param to_date: '17-06-2023' ('dd-mm-YYYY')
     :param period: use one {'1D': last day data,
                             '1W': for last 7 days data,
                             '1M': from last month same date,
@@ -221,29 +222,29 @@
         data_df = get_block_deals_data(from_date=start_date, to_date=end_date)
         from_date = from_date + dt.timedelta(365)
         load_days = (to_date - from_date).days
         nse_df = pd.concat([nse_df, data_df], ignore_index=True)
     return nse_df
 
 
-def get_block_deals_data(from_date:str, to_date:str):
+def get_block_deals_data(from_date: str, to_date: str):
     # print(from_date, to_date)
     url = "https://www.nseindia.com/api/historical/block-deals?"
     payload = f"from={from_date}&to={to_date}&csv=true"
-    data_text = nse_urlfetch(url+payload).text
+    data_text = nse_urlfetch(url + payload).text
     # data_text = data_text.replace('\x82','').replace('â¹', 'In Rs')
     with open('file.csv', 'w') as f:
         f.write(data_text)
     f.close()
     data_df = pd.read_csv('file.csv')
-    data_df.columns = [name.replace(' ','') for name in data_df.columns]
+    data_df.columns = [name.replace(' ', '') for name in data_df.columns]
     return data_df
 
 
-def short_selling_data(from_date:str = None, to_date:str = None, period:str = None):
+def short_selling_data(from_date: str = None, to_date: str = None, period: str = None):
     """
     get short selling data set.
     :param from_date: '17-03-2022' ('dd-mm-YYYY')
     :param to_date: '17-06-2023' ('dd-mm-YYYY')
     :param period: use one {'1D': last day data,
                             '1W': for last 7 days data,
                             '1M': from last month same date,
@@ -268,61 +269,81 @@
         data_df = get_short_selling_data(from_date=start_date, to_date=end_date)
         from_date = from_date + dt.timedelta(365)
         load_days = (to_date - from_date).days
         nse_df = pd.concat([nse_df, data_df], ignore_index=True)
     return nse_df
 
 
-def get_short_selling_data(from_date:str, to_date:str):
+def get_short_selling_data(from_date: str, to_date: str):
     # print(from_date, to_date)
     url = "https://www.nseindia.com/api/historical/short-selling?"
     payload = f"from={from_date}&to={to_date}&csv=true"
-    data_text = nse_urlfetch(url+payload).text
+    data_text = nse_urlfetch(url + payload).text
     # data_text = data_text.replace('\x82','').replace('â¹', 'In Rs')
     with open('file.csv', 'w') as f:
         f.write(data_text)
     f.close()
     data_df = pd.read_csv('file.csv')
-    data_df.columns = [name.replace(' ','') for name in data_df.columns]
+    data_df.columns = [name.replace(' ', '') for name in data_df.columns]
     return data_df
 
 
-def bhav_copy_with_delivery(trade_date:str):
+def bhav_copy_with_delivery(trade_date: str):
     trade_date = datetime.strptime(trade_date, dd_mm_yyyy)
     use_date = trade_date.strftime(ddmmyyyy)
-    url = 'https://archives.nseindia.com/products/content/sec_bhavdata_full_'
-    payload = f'{trade_date}.csv'
+    url = f'https://archives.nseindia.com/products/content/sec_bhavdata_full_{use_date}.csv'
     request_bhav = nse_urlfetch(url)
     bhav_df = pd.DataFrame()
     if request_bhav.status_code == 200:
         bhav_df = pd.read_csv(StringIO(request_bhav.text), sep=', ', engine='python')
     elif request_bhav.status_code == 403:
         raise FileNotFoundError(f' Data not found, change the date...')
     return bhav_df[['SYMBOL', 'SERIES', 'OPEN_PRICE', 'HIGH_PRICE', 'LOW_PRICE', 'CLOSE_PRICE',
-                                   'PREV_CLOSE', 'TTL_TRD_QNTY', 'TURNOVER_LACS', 'NO_OF_TRADES', 'DELIV_QTY',
-                                   'DELIV_PER', 'DATE1']]
+                    'PREV_CLOSE', 'TTL_TRD_QNTY', 'TURNOVER_LACS', 'NO_OF_TRADES', 'DELIV_QTY',
+                    'DELIV_PER', 'DATE1']]
 
 
-def bhav_copy(trade_date:str):
+def bhav_copy(trade_date: str):
     trade_date = datetime.strptime(trade_date, dd_mm_yyyy)
     url = 'https://archives.nseindia.com/content/historical/EQUITIES/'
     payload = f"{str(trade_date.strftime('%Y'))}/{str(trade_date.strftime('%b').upper())}/" \
               f"cm{str(trade_date.strftime('%d%b%Y').upper())}bhav.csv.zip"
-    request_bhav = nse_urlfetch(url+payload)
+    request_bhav = nse_urlfetch(url + payload)
     bhav_df = pd.DataFrame()
     if request_bhav.status_code == 200:
         zip_bhav = zipfile.ZipFile(BytesIO(request_bhav.content), 'r')
         for file_name in zip_bhav.filelist:
             if file_name:
                 bhav_df = pd.read_csv(zip_bhav.open(file_name))
     elif request_bhav.status_code == 403:
         raise FileNotFoundError(f' Data not found, change the date...')
     bhav_df = bhav_df[['SYMBOL', 'SERIES', 'OPEN', 'HIGH', 'LOW', 'CLOSE', 'LAST', 'PREVCLOSE', 'TOTTRDQTY',
                        'TOTTRDVAL', 'TIMESTAMP', 'TOTALTRADES']]
     return bhav_df
 
 
-if __name__ == '__main__':
-    df = bhav_copy(trade_date='01-06-2022')
-    print(df)
-    print(df.columns)
+def equity_list():
+    data_df = pd.read_csv("https://archives.nseindia.com/content/equities/EQUITY_L.csv")
+    data_df = data_df[['SYMBOL', 'NAME OF COMPANY', ' SERIES', ' DATE OF LISTING', ' FACE VALUE']]
+    return data_df
+
+
+def fno_equity_list():
+    data_df = pd.read_csv("https://archives.nseindia.com/content/fo/fo_mktlots.csv", skiprows=5)
+    today = dt.date.today()
+    MMM_YY = today.strftime(mmm_yy).upper()
+    data_df.rename(columns={'Derivatives on Individual Securities': 'Company_Name'}, inplace=True)
+    data_df.columns = [name.replace('    ', '').replace(' ', '') for name in data_df.columns]
+    data_df = data_df[['Company_Name', 'Symbol', f'{MMM_YY}']]
+    return data_df
+
+
+def nifty50_equity_list():
+    data_df = pd.read_csv("https://archives.nseindia.com/content/indices/ind_nifty50list.csv")
+    data_df = data_df[['Company Name', 'Industry', 'Symbol']]
+    return data_df
+
 
+# if __name__ == '__main__':
+#     import nselib
+#     data = nselib.trading_holiday_calendar()
+#     print(data)
```

### Comparing `nselib-0.3/nselib/constants.py` & `nselib-0.4/nselib/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 dd_mm_yyyy = '%d-%m-%Y'
 dd_mmm_yyyy = '%d-%b-%Y'
 ddmmyyyy = '%d%m%Y'
+mmm_yy = '%b-%y'
 
 equity_periods = ['1D', '1W', '1M', '3M', '6M', '1Y']
 
 # ---------- column lists-----------------
 
 price_volume_and_deliverable_position_data_columns = \
     ['Symbol', 'Series', 'Date', 'PrevClose', 'OpenPrice', 'HighPrice',
```

### Comparing `nselib-0.3/nselib/derivatives/derivative_data.py` & `nselib-0.4/nselib/derivatives/derivative_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,12 +176,12 @@
     except Exception:
         data_df = pd.read_csv(url, engine='c', sep=',', quotechar='"', on_bad_lines='skip', skiprows=1)
         data_df.drop(data_df.tail(1).index, inplace=True)
         data_df.columns = [name.replace('\t', '') for name in data_df.columns]
     return data_df
 
 
-if __name__ == '__main__':
-    df = future_price_volume_data("BANKNIFTY", "FUTIDX", from_date='17-06-2023', to_date='19-06-2023', period='1D')
-    # df = participant_wise_trading_volume(trade_date='03-04-2023')
-    print(df)
-    print(df[df['EXPIRY_DT']=='27-Jul-2023'])
+# if __name__ == '__main__':
+#     df = future_price_volume_data("BANKNIFTY", "FUTIDX", from_date='17-06-2023', to_date='19-06-2023', period='1D')
+#     # df = participant_wise_trading_volume(trade_date='03-04-2023')
+#     print(df)
+#     print(df[df['EXPIRY_DT']=='27-Jul-2023'])
```

### Comparing `nselib-0.3/nselib.egg-info/PKG-INFO` & `nselib-0.4/nselib.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nselib
-Version: 0.3
+Version: 0.4
 Summary: library to get NSE India data
 Home-page: https://github.com/RuchiTanmay/nselib
 Author: RuchiTanmay
 Author-email: ruchitanmay@gmail.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# NSElib 0.3
+# NSElib 0.4
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
@@ -39,33 +39,66 @@
 ```$pip install nselib```
 
 Upgrade
 
 ```$pip install nselib --upgrade```
 
 ## Function list
+
+### nselib
+* trading_holiday_calendar
+
+Example :
+
+import nselib
+
+data = nselib.trading_holiday_calendar()
+
 ### Capital Market
 * price_volume_and_deliverable_position_data 
 * price_volume_data
 * deliverable_position_data
 * bulk_deal_data
 * block_deals_data
 * short_selling_data
 * bhav_copy_with_delivery
 * bhav_copy
+* equity_list
+* fno_equity_list
+* nifty50_equity_list
+
+Example : 
+
+from nselib import capital_market 
+
+data = capital_market.price_volume_and_deliverable_position_data(symbol='SBIN', from_date='01-06-2023', to_date='10-06-2023')
+                                            
+OR
+
+data = capital_market.price_volume_and_deliverable_position_data(symbol='SBIN', period='1M')
 
 More functions will be available in future releases...
 
 ### Derivative
 * future_price_volume_data
 * option_price_volume_data
 * fno_bhav_copy
 * participant_wise_open_interest
 * participant_wise_trading_volume
 
+Example : 
+
+from nselib import derivatives
+
+data = derivatives.future_price_volume_data(symbol='SBIN', instrument='FUTSTK', from_date='01-06-2023', to_date='10-06-2023')
+
+OR
+
+data = derivatives.price_volume_and_deliverable_position_data(symbol='BANKNIFTY', instrument='FUTIDX', period='1M')
+
 More functions will be available in future releases...
 
 ### Debt
 
 More functions will be available in future releases...
```

### Comparing `nselib-0.3/setup.py` & `nselib-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='nselib',
     packages=setuptools.find_packages(),
-    version='0.3',
+    version='0.4',
     include_package_data=True,
     description='library to get NSE India data',
     long_description=long_description,
     long_description_content_type="text/markdown", author='RuchiTanmay',
     author_email='ruchitanmay@gmail.com',
     url='https://github.com/RuchiTanmay/nselib',
     install_requires=['requests', 'pandas', 'scipy'],
```

