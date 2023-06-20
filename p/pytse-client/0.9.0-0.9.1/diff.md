# Comparing `tmp/pytse-client-0.9.0.tar.gz` & `tmp/pytse-client-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytse-client-0.9.0.tar", max compression
+gzip compressed data, was "pytse-client-0.9.1.tar", max compression
```

## Comparing `pytse-client-0.9.0.tar` & `pytse-client-0.9.1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0    35149 2021-09-02 07:18:47.772581 pytse-client-0.9.0/LICENSE
--rw-r--r--   0        0        0    18874 2021-09-02 07:18:47.772581 pytse-client-0.9.0/README.md
--rw-r--r--   0        0        0      498 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        6 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/.gitignore
--rw-r--r--   0        0        0      148 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/__init__.py
--rw-r--r--   0        0        0      202 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/config.py
--rw-r--r--   0        0        0        0 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/data/__init__.py
--rw-r--r--   0        0        0   161413 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/data/symbols_name.json
--rw-r--r--   0        0        0     7481 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/download.py
--rw-r--r--   0        0        0        0 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/examples/__init__.py
--rw-r--r--   0        0        0      866 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/examples/client_types.py
--rw-r--r--   0        0        0      169 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/examples/download_all.py
--rw-r--r--   0        0        0      435 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/examples/download_shareholders_history.py
--rw-r--r--   0        0        0     1292 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/examples/download_shareholders_history_aync.py
--rw-r--r--   0        0        0      376 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/examples/sma.py
--rw-r--r--   0        0        0     1008 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/examples/ticker.py
--rw-r--r--   0        0        0        0 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/scraper/__init__.py
--rw-r--r--   0        0        0     2775 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/scraper/symbol_scraper.py
--rw-r--r--   0        0        0     1226 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/scraper/tsetmc_scraper.py
--rw-r--r--   0        0        0     1152 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/scripts/update_symbols_json.py
--rw-r--r--   0        0        0     1250 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/symbols_data.py
--rw-r--r--   0        0        0       27 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/ticker/__init__.py
--rw-r--r--   0        0        0     1000 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/ticker/api_extractors.py
--rw-r--r--   0        0        0    10892 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/ticker/ticker.py
--rw-r--r--   0        0        0      439 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/translations.py
--rw-r--r--   0        0        0     1084 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/tse_settings.py
--rw-r--r--   0        0        0      305 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/utils/__init__.py
--rw-r--r--   0        0        0      839 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/utils/async_utils.py
--rw-r--r--   0        0        0      183 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/utils/date.py
--rw-r--r--   0        0        0      100 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/utils/persian.py
--rw-r--r--   0        0        0      616 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/utils/request_session.py
--rw-r--r--   0        0        0     1388 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/utils/scrape.py
--rw-r--r--   0        0        0      131 2021-09-02 07:18:47.772581 pytse-client-0.9.0/pytse_client/utils/string.py
--rw-r--r--   0        0        0    20263 2021-09-02 07:19:01.515392 pytse-client-0.9.0/setup.py
--rw-r--r--   0        0        0    19607 2021-09-02 07:19:01.516762 pytse-client-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-09-04 14:52:55.232059 pytse-client-0.9.1/LICENSE
+-rw-r--r--   0        0        0    19235 2021-09-04 14:52:55.236059 pytse-client-0.9.1/README.md
+-rw-r--r--   0        0        0      498 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        6 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/.gitignore
+-rw-r--r--   0        0        0      148 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/__init__.py
+-rw-r--r--   0        0        0      202 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/config.py
+-rw-r--r--   0        0        0        0 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/data/__init__.py
+-rw-r--r--   0        0        0   161413 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/data/symbols_name.json
+-rw-r--r--   0        0        0     7481 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/download.py
+-rw-r--r--   0        0        0        0 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/examples/__init__.py
+-rw-r--r--   0        0        0      866 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/examples/client_types.py
+-rw-r--r--   0        0        0      169 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/examples/download_all.py
+-rw-r--r--   0        0        0      435 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/examples/download_shareholders_history.py
+-rw-r--r--   0        0        0     1292 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/examples/download_shareholders_history_aync.py
+-rw-r--r--   0        0        0      376 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/examples/sma.py
+-rw-r--r--   0        0        0     1008 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/examples/ticker.py
+-rw-r--r--   0        0        0      207 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/proxy/dto.py
+-rw-r--r--   0        0        0     1986 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/proxy/tsetmc.py
+-rw-r--r--   0        0        0        0 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/scraper/__init__.py
+-rw-r--r--   0        0        0     2775 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/scraper/symbol_scraper.py
+-rw-r--r--   0        0        0      289 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/scraper/tsetmc_scraper.py
+-rw-r--r--   0        0        0     1152 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/scripts/update_symbols_json.py
+-rw-r--r--   0        0        0     1250 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/symbols_data.py
+-rw-r--r--   0        0        0       27 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/ticker/__init__.py
+-rw-r--r--   0        0        0     1000 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/ticker/api_extractors.py
+-rw-r--r--   0        0        0    10969 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/ticker/ticker.py
+-rw-r--r--   0        0        0      439 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/translations.py
+-rw-r--r--   0        0        0     1212 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/tse_settings.py
+-rw-r--r--   0        0        0      305 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/utils/__init__.py
+-rw-r--r--   0        0        0      839 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/utils/async_utils.py
+-rw-r--r--   0        0        0      258 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/utils/date.py
+-rw-r--r--   0        0        0      100 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/utils/persian.py
+-rw-r--r--   0        0        0      616 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/utils/request_session.py
+-rw-r--r--   0        0        0     1388 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/utils/scrape.py
+-rw-r--r--   0        0        0      131 2021-09-04 14:52:55.236059 pytse-client-0.9.1/pytse_client/utils/string.py
+-rw-r--r--   0        0        0    20648 2021-09-04 14:53:09.554829 pytse-client-0.9.1/setup.py
+-rw-r--r--   0        0        0    19968 2021-09-04 14:53:09.556360 pytse-client-0.9.1/PKG-INFO
```

### Comparing `pytse-client-0.9.0/LICENSE` & `pytse-client-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/README.md` & `pytse-client-0.9.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -311,30 +311,31 @@
 to_when=datetime.datetime.now(), تا چه تاریخی اطلاعات گرفته شود پیشفرض امروز هست
 only_trade_days=True, فقط روز‌های معاملاتی پیش فرض بله
 ```
 خروجی این تابع یک دیتا فریم به شکل زیر هست که به صورت csv 
 <div dir="ltr">
 
 ```
-,date,shares,percentage,instrument_id,shareholder
-0,2021-01-23,3280482041,56.56,IRO1BRKT0003,شركت كارانديش دوران معاصر-سهامي خاص-
-1,2021-01-23,486240253,8.38,IRO1BRKT0003,شركت گروه سرمايه گذاري تدبير-سهامي خاص-
-2,2021-01-23,209066245,3.6,IRO1BRKT0003,شركت سرمايه گذاري پويا-سهامي عام-
-3,2021-01-23,121523528,2.09,IRO1BRKT0003,شركت پالايش پارسيان سپهر-سهامي خاص-
-4,2021-01-23,64873196,1.11,IRO1BRKT0003,BFMصندوق سرمايه گذاري.ا.ب.تدبيرگران فردا
-5,2021-01-24,3280482041,56.56,IRO1BRKT0003,شركت كارانديش دوران معاصر-سهامي خاص-
-6,2021-01-24,486240253,8.38,IRO1BRKT0003,شركت گروه سرمايه گذاري تدبير-سهامي خاص-
-7,2021-01-24,209066245,3.6,IRO1BRKT0003,شركت سرمايه گذاري پويا-سهامي عام-
-8,2021-01-24,121523528,2.09,IRO1BRKT0003,شركت پالايش پارسيان سپهر-سهامي خاص-
-9,2021-01-24,65213196,1.12,IRO1BRKT0003,BFMصندوق سرمايه گذاري.ا.ب.تدبيرگران فردا
-10,2021-01-25,3280482041,56.56,IRO1BRKT0003,شركت كارانديش دوران معاصر-سهامي خاص-
-11,2021-01-25,486240253,8.38,IRO1BRKT0003,شركت گروه سرمايه گذاري تدبير-سهامي خاص-
-12,2021-01-25,209066245,3.6,IRO1BRKT0003,شركت سرمايه گذاري پويا-سهامي عام-
-13,2021-01-25,121523528,2.09,IRO1BRKT0003,شركت پالايش پارسيان سپهر-سهامي خاص-
-14,2021-01-25,68453196,1.18,IRO1BRKT0003,BFMصندوق سرمايه گذاري.ا.ب.تدبيرگران فردا
+,date,shareholder_id,shareholder_shares,shareholder_percentage,shareholder_instrument_id,shareholder_name,change
+0,2021-08-30 17:01:23.037957,273,2910355428.0,32.19,IRO1RSAP0000,شركت ايراني توليداتومبيل-سايپا-,1
+1,2021-08-30 17:01:23.037957,406,975144471.0,10.78,IRO1RSAP0000,شركت سايپا,1
+2,2021-08-30 17:01:23.037957,50264,454000000.0,5.02,IRO1RSAP0000,شركت ايراني توليداتومبيل سايپا-سهامي عام-,1
+3,2021-08-30 17:01:23.037957,42636,409843922.0,4.53,IRO1RSAP0000,شركت سرمايه گذاري وتوسعه صنعتي نيوان ابتكارس.ع,1
+4,2021-08-30 17:01:23.037957,46966,116002189.0,1.28,IRO1RSAP0000,BFMصندوق.س.ا.بازارگرداني سهم آشنايكم,1
+5,2021-08-31 17:01:23.037957,273,2910355428.0,32.19,IRO1RSAP0000,شركت ايراني توليداتومبيل-سايپا-,1
+6,2021-08-31 17:01:23.037957,406,975144471.0,10.78,IRO1RSAP0000,شركت سايپا,1
+7,2021-08-31 17:01:23.037957,50264,454000000.0,5.02,IRO1RSAP0000,شركت ايراني توليداتومبيل سايپا-سهامي عام-,1
+8,2021-08-31 17:01:23.037957,42636,409843922.0,4.53,IRO1RSAP0000,شركت سرمايه گذاري وتوسعه صنعتي نيوان ابتكارس.ع,1
+9,2021-08-31 17:01:23.037957,46966,116002189.0,1.28,IRO1RSAP0000,BFMصندوق.س.ا.بازارگرداني سهم آشنايكم,1
+10,2021-09-01 17:01:23.037957,273,2910355428.0,32.19,IRO1RSAP0000,شركت ايراني توليداتومبيل-سايپا-,1
+11,2021-09-01 17:01:23.037957,406,975144471.0,10.78,IRO1RSAP0000,شركت سايپا,1
+12,2021-09-01 17:01:23.037957,50264,454000000.0,5.02,IRO1RSAP0000,شركت ايراني توليداتومبيل سايپا-سهامي عام-,1
+13,2021-09-01 17:01:23.037957,42636,409843922.0,4.53,IRO1RSAP0000,شركت سرمايه گذاري وتوسعه صنعتي نيوان ابتكارس.ع,1
+14,2021-09-01 17:01:23.037957,46966,116002189.0,1.28,IRO1RSAP0000,BFMصندوق.س.ا.بازارگرداني سهم آشنايكم,1
+
 ```
 </div>
 
 <div id="qa" />
 گرفتن این دیتا کار زمان بری هست(با توجه به تعداد روزی که لازم دارید) و سریع کردن کار با کد به راحتی امکان پذیر نیست. سعی نکنید با همزمان اجرا کردن این تابع برای سهم‌های مختلف روند رو سریع‌تر کنید چون سایت ip رو بلاک میکنه.
 اگر موقع اجرای کد پیغام زیر را به تعداد زیاد گرفتید (مثلا هر ثانیه این پیغام اومد) یعنی آیپی شما توسط سایت بورس بلاک شده و چند دقیقه صبر کنید و دوباره ادامه بدید.
 <div dir="ltr">
```

### Comparing `pytse-client-0.9.0/pytse_client/data/symbols_name.json` & `pytse-client-0.9.1/pytse_client/data/symbols_name.json`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/pytse_client/download.py` & `pytse-client-0.9.1/pytse_client/download.py`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/pytse_client/examples/client_types.py` & `pytse-client-0.9.1/pytse_client/examples/client_types.py`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/pytse_client/examples/download_shareholders_history_aync.py` & `pytse-client-0.9.1/pytse_client/examples/download_shareholders_history_aync.py`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/pytse_client/examples/ticker.py` & `pytse-client-0.9.1/pytse_client/examples/ticker.py`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/pytse_client/scraper/symbol_scraper.py` & `pytse-client-0.9.1/pytse_client/scraper/symbol_scraper.py`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/pytse_client/scripts/update_symbols_json.py` & `pytse-client-0.9.1/pytse_client/scripts/update_symbols_json.py`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/pytse_client/symbols_data.py` & `pytse-client-0.9.1/pytse_client/symbols_data.py`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/pytse_client/ticker/api_extractors.py` & `pytse-client-0.9.1/pytse_client/ticker/api_extractors.py`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/pytse_client/ticker/ticker.py` & `pytse-client-0.9.1/pytse_client/ticker/ticker.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     config,
     symbols_data,
     translations,
     tse_settings,
     utils,
 )
 from pytse_client.download import download, download_ticker_client_types_record
-from pytse_client.scraper import tsetmc_scraper
+from pytse_client.proxy.dto import ShareholderData
+from pytse_client.proxy.tsetmc import get_day_shareholders_history
 from pytse_client.ticker.api_extractors import Order, get_orders
 from pytse_client.tse_settings import TSE_CLIENT_TYPE_DATA_URL
-from pytse_client.utils import async_utils
 from tenacity import retry, wait_random
 from tenacity.before_sleep import before_sleep_log
 
 logger = logging.getLogger(config.LOGGER_NAME)
 logger.addHandler(logging.NullHandler())
 
 
@@ -201,57 +201,59 @@
         only_trade_days=True,
         session=None,
     ) -> pd.DataFrame:
         requested_dates = utils.datetime_range(to_when - from_when, to_when)
         session_created = False
         if not session:
             session_created = True
-            conn = aiohttp.TCPConnector(limit=3)
+            conn = aiohttp.TCPConnector(limit=25)
             session = aiohttp.ClientSession(connector=conn)
         tasks = []
-        for date in requested_dates:
-            if only_trade_days and date.date() not in self.trade_dates:
-                continue
+        filtered_dates = list(
+            filter(
+                lambda date: not only_trade_days or
+                (only_trade_days and date.date() in self.trade_dates),
+                requested_dates,
+            )
+        )
+        for date in filtered_dates:
             tasks.append(
-                self._get_ticker_daily_info_page_response(
-                    session, date.strftime(tse_settings.DATE_FORMAT)
-                )
+                get_day_shareholders_history(self._index, date, session)
             )
-        pages = await async_utils.run_tasks_with_wait(tasks, 30, 10)
+        all_tickers_shareholders: List[List[ShareholderData]
+                                       ] = await asyncio.gather(*tasks)
         if session_created is True:
             await session.close()
+
         rows = []
-        for page in pages:
-            page_date = tsetmc_scraper.scrape_daily_info_page_for_date(page)
-            shareholders_data = (
-                tsetmc_scraper.
-                scrape_daily_info_page_for_shareholder_data(page)
-            )
-            for shareholder_data in shareholders_data:
+        for ticker_shareholders, info_date in zip(
+            all_tickers_shareholders, filtered_dates
+        ):
+            for shareholder_data in ticker_shareholders:
                 rows.append(
                     [
-                        datetime.datetime.strptime(
-                            page_date,
-                            tse_settings.DATE_FORMAT,
-                        ),
+                        info_date,
+                        shareholder_data.id,
                         shareholder_data.shares,
                         shareholder_data.percentage,
                         shareholder_data.instrument_id,
                         shareholder_data.name,
+                        shareholder_data.change,
                     ]
                 )
-
         return pd.DataFrame(
             data=rows,
             columns=[
                 'date',
-                'shares',
-                'percentage',
-                'instrument_id',
-                'shareholder',
+                'shareholder_id',
+                'shareholder_shares',
+                'shareholder_percentage',
+                'shareholder_instrument_id',
+                'shareholder_name',
+                'change',
             ]
         )
 
     @property
     def last_price(self):
         return self.get_ticker_real_time_info_response().last_price
```

### Comparing `pytse-client-0.9.0/pytse_client/tse_settings.py` & `pytse-client-0.9.1/pytse_client/tse_settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,9 +25,14 @@
 SYMBOLS_LIST_URL = ("http://www.tsetmc.com/Loader.aspx?ParTree=111C1417")
 
 # market watch init, has initial data for market watch like symbols name etc.
 MARKET_WATCH_INIT_URL = (
     "http://www.tsetmc.com/tsev2/data/MarketWatchInit.aspx?h=0&r=0"
 )
 
+# get day share holder data
+SYMBOL_DAY_INFO_SHAREHOLDERS_DATA = (
+    "http://cdn.tsetmc.com/api/Shareholder/{index}/{date}"
+)
+
 DATE_FORMAT = "%Y%m%d"
 MIN_DATE = 20010321
```

### Comparing `pytse-client-0.9.0/pytse_client/utils/async_utils.py` & `pytse-client-0.9.1/pytse_client/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/pytse_client/utils/request_session.py` & `pytse-client-0.9.1/pytse_client/utils/request_session.py`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/pytse_client/utils/scrape.py` & `pytse-client-0.9.1/pytse_client/utils/scrape.py`

 * *Files identical despite different names*

### Comparing `pytse-client-0.9.0/setup.py` & `pytse-client-0.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['pytse_client',
  'pytse_client.data',
  'pytse_client.examples',
+ 'pytse_client.proxy',
  'pytse_client.scraper',
  'pytse_client.scripts',
  'pytse_client.ticker',
  'pytse_client.utils']
 
 package_data = \
 {'': ['*']}
@@ -19,17 +20,17 @@
  'jdatetime>=3.6.2,<4.0.0',
  'pandas',
  'requests>=2.23.0,<3.0.0',
  'tenacity>=7.0.0,<8.0.0']
 
 setup_kwargs = {
     'name': 'pytse-client',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'tehran stock exchange(TSE) client in python',
-    'long_description': '<div dir="rtl">\n\n# دریافت اطلاعات بازار بورس تهران\n\n![Python application](https://github.com/Glyphack/pytse-client/workflows/Python%20application/badge.svg)\n[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Glyphack/pytse-client.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Glyphack/pytse-client/context:python)\n[![Discord Chat](https://img.shields.io/discord/730808323808559106?label=discord)](https://discord.gg/ampPDKHpVv)\n\nبا استفاده از pytse client میتونید به دیتای بازار بورس تهران در پایتون دسترسی داشته باشید.\nهدف حل مشکلات گرفتن اطلاعات بروز از سایت بازار بورس تهران هست.\n\n## میخواید مشارکت کنید؟\nلطفا [این صفحه](https://github.com/Glyphack/pytse-client/blob/master/CONTRIBUTING.md) رو مطالعه کنید\n\n- [دریافت اطلاعات بازار بورس تهران](#دریافت-اطلاعات-بازار-بورس-تهران)\n  - [میخواید مشارکت کنید؟](#میخواید-مشارکت-کنید)\n  - [قابلیت ها](#قابلیت-ها)\n  - [نصب](#نصب)\n  - [نحوه استفاده](#نحوه-استفاده)\n    - [دانلود سابقه سهم\u200cها](#دانلود-سابقه-سهمها)\n    - [دانلود سابقه معاملات حقیقی و حقوقی به صورت مجزا](#دانلود-سابقه-معاملات-حقیقی-و-حقوقی-به-صورت-مجزا)\n    - [ماژول Ticker](#ماژول-ticker)\n        - [۱نکته](#۱نکته)\n        - [نکته۲](#نکته۲)\n      - [اطلاعات نماد\u200cهای حذف شده](#اطلاعات-نمادهای-حذف-شده)\n      - [اطلاعات حقیقی و حقوقی](#اطلاعات-حقیقی-و-حقوقی)\n      - [سهامداران عمده](#سهامداران-عمده)\n        - [شناور سهم](#شناور-سهم)\n        - [تاریخچه\u200cی سهام داران عمده](#تاریخچهی-سهام-داران-عمده)\n        - [اطلاعات لحظه\u200cای سهام](#اطلاعات-لحظهای-سهام)\n      - [کامیونیتی](#کامیونیتی)\n      - [پکیج های مورد نیاز:](#پکیج-های-مورد-نیاز)\n      - [الهام گرفته از:](#الهام-گرفته-از)\n\n## قابلیت ها\n\n- دریافت اطلاعات روز های معاملاتی هر سهم و قابلیت ذخیره سازی\n- قابلیت گرفتن اطلاعات یک سهام مانند گروه سهام و اطلاعات معاملات حقیقی و حقوقی\n- دریافت اطلاعات فاندامنتال یک نماد شامل(eps, p/e ,حجم مبنا)\n\n## نصب\n\n<div dir="ltr">\n\n```bash\npip install pytse-client\n```\n\n</div>\n\n## نحوه استفاده\n\n### دانلود سابقه سهم\u200cها\n\nبا استفاده از این تابع میتوان سابقه سهام هارو دریافت کرد و هم اون رو ذخیره و هم توی کد استفاده کرد\n\n<div dir="ltr">\n\n```python\nimport pytse_client as tse\ntickers = tse.download(symbols="all", write_to_csv=True)\ntickers["ولملت"] # history\n\n            date     open     high  ...     volume  count    close\n0     2009-02-18   1050.0   1050.0  ...  330851245    800   1050.0\n1     2009-02-21   1051.0   1076.0  ...  335334212   6457   1057.0\n2     2009-02-22   1065.0   1074.0  ...    8435464    603   1055.0\n3     2009-02-23   1066.0   1067.0  ...    8570222    937   1060.0\n4     2009-02-25   1061.0   1064.0  ...    7434309    616   1060.0\n...          ...      ...      ...  ...        ...    ...      ...\n2323  2020-04-14   9322.0   9551.0  ...  105551315  13536   9400.0\n2324  2020-04-15   9410.0   9815.0  ...  201457026  11322   9815.0\n2325  2020-04-18  10283.0  10283.0  ...  142377245   8929  10283.0\n2326  2020-04-19  10797.0  10797.0  ...  292985635  22208  10380.0\n2327  2020-04-20  10600.0  11268.0  ...  295590437  16313  11268.0\n```\n\n</div>\n\nبرای دانلود سابقه یک یا چند سهم کافی هست اسم اون ها به تابع داده بشه:\n\n<div dir="rtl">\n\nهمچنین با گذاشتن\n`write_to_csv=True`\nسابقه سهم توی فایلی با اسم سهم نوشته میشه\n\nسابقه سهم در قالب `Dataframe` است\n\nدرصورتی که می خواهید تاریخ شمسی به خروجی اضافه شود می توانید با گذاشتن\n`include_jdate=True`\nاین امکان را فراهم کنید\n\n</div>\n\n<div dir="ltr">\n\n```python\nimport pytse_client as tse\ntse.download(symbols="وبملت", write_to_csv=True)\ntse.download(symbols="وبملت", write_to_csv=True, include_jdate=True)\ntse.download(symbols=["وبملت", "ولملت"], write_to_csv=True)\n```\n\n</div>\n\n### دانلود سابقه معاملات حقیقی و حقوقی به صورت مجزا\n\nبرای دانلود سابقه معاملات حقیقی و حقوقی برای تمامی نمادها میتوان از تابع زیر استفاده کرد\n\n<div dir="ltr">\n\n```python\nfrom pytse_client import download_client_types_records\n\nif __name__ == \'__main__\':\n\n  records_dict = download_client_types_records("all")\n  print(records_dict["فولاد"])\n  #Output\ndate         individual_buy_count  ... individual_ownership_change\n\n2020-09-01                36298  ...                   -691857.0\n2020-08-31                58185  ...                  83789408.0\n2020-08-26                  461  ...                  21647730.0\n2020-08-25                 1248  ...                  14716846.0\n2020-08-24                38291  ...                -238454702.0\n...                         ...  ...                         ...\n2008-12-02                    7  ...                    -10000.0\n2008-12-01                    8  ...                         0.0\n2008-11-30                   10  ...                    -12781.0\n2008-11-29                  116  ...                   4596856.0\n2008-11-26                   14  ...                    -20000.0\n\n[2518 rows x 17 columns]\n\n```\n\n</div>\n\nمشابه تابع قبلی میتوان نتایج را ذخیره کرد\n\n<div dir="ltr">\n\n```python\nfrom pytse_client import download_client_types_records\nif __name__ == \'__main__\':\n\n  #Records are saved as a .csv file with the same name of ticer\'s\n  records = download_client_types_records("فولاد", write_to_csv=True)\n```\n\n</div>\n\n### ماژول Ticker\n\nاین ماژول برای کار با دیتای یک سهم خاص هست و با گرفتن نماد اطلاعات موجود رو میده\n\nبرای مثال:\n\n<div dir="ltr">\n\n```python\nimport pytse_client as tse\n\ntse.download(symbols="وبملت", write_to_csv=True)  # optional\nticker = tse.Ticker("وبملت")\nprint(ticker.history)  # سابقه قیمت سهم\nprint(ticker.client_types)  # حقیقی حقوقی\nprint(ticker.title)  # نام شرکت\nبانك ملت (وبملت)\nprint(ticker.url)  # آدرس صفحه سهم\nhttp://tsetmc.com/Loader.aspx?ParTree=151311&i=778253364357513\nprint(ticker.group_name)  # نام گروه\nبانكها و موسسات اعتباري\nprint(ticker.eps)  # eps\n2725.0\nprint(ticker.p_e_ratio)  # P/E\n6.1478899082568805\nprint(ticker.group_p_e_ratio)  # group P/E\n18.0\nprint(ticker.base_volume)  # حجم مبنا\n7322431.0\nprint(ticker.last_price)  # آخرین معامله\n17316\nprint(ticker.adj_close)  # قیمت پایانی\n16753\nprint(ticker.best_supply_price)  # قیمت بهترین تقاضا\n26700\nprint(ticker.best_supply_vol)  # حجم بهترین تقاضا\n357062\nprint(ticker.best_demand_price)  # قیمت بهترین عرضه\n26700\nprint(ticker.best_demand_vol)  # حجم بهترین عرضه\n576608\nprint(ticker.shareholders)  # اطلاعات سهام داران عمده\n\nprint(ticker.get_shareholders_history())) # تاریخچه\u200cی سهام داران عمده\nprint(ticker.get_ticker_real_time_info_response()) # اطلاعات لحظه\u200cای مانند قیمت و پیشنهادات خرید و فروش\n\n\n```\n\n</div>\n\nبرای استفاده لازم نیست حتما تابع دانلود صدا زده بشه.\nاگر این کد رو بدون دانلود کردن سهم استفاده کنید خودش اطلاعات سهم رو از سایت میگیره،\nاما اگر قبل از اون از دانلود استفاده کرده باشید\nبه جای گرفتن از اینترنت اطلاعات رو از روی فایل میخونه که سریع تر هست\n\n##### ۱نکته\n\nطبق تجربه\u200c ای که داشتم چون گاهی اوقات سایت بورس مدت زیادی طول میکشه تا اطلاعات رو بفرسته یا بعضی مواقع نمیفرسته بهتر هست که اول تابع دانلود رو استفاده کنید برای سهم\u200cهایی که لازم هست و بعد با دیتای اون ها کار کنید.\n\n##### نکته۲\n\nبعضی از ویژگی\u200cها برای همه\u200cی سهم ها در دسترس نیست. برای مثال بعضی از سهم ها دارای آخرین قیمت یا پی به ای یا ای پی اس نیستند. مقدار این ویژگی\u200cها در صورت نبودن برابر با `None` خواهد بود. پس باید در برنامه خود اینکه این مقادیر وجود دارند را بررسی کنید.\n\n#### اطلاعات نماد\u200cهای حذف شده\nتعدادی از نماد\u200cها توی سایت به شکل حذف شده هستند. برای گرفتن دیتای این نماد\u200cها از ماژول تیکر به شکل زیر استفاده کنید:\nبرای مثال در سهام \nhttp://www.tsetmc.com/Loader.aspx?ParTree=151311&i=25165947991415904\n\n<div dir="ltr">\n\n```python\nimport pytse_client as tse\n\nticker = tse.Ticker("", index="25165947991415904")\n```\n\n</div>\n\nمقدار  \u200d`index` را با مقدار جلوی `i=` جایگزین میکنیم.\n#### اطلاعات حقیقی و حقوقی\n\nاطلاعات خرید و فروش حقیقی و حقوقی سهام رو میشه از طریق `ticker.client_types` گرفت این اطلاعات یه DataFrame شامل اطلاعات موجود در تب حقیقی حقوقی(تب بنفشی که در این [صفحه](http://www.tsetmc.com/Loader.aspx?ParTree=151311&i=778253364357513) هست) سهم هست:\n\n<div dir="ltr">\n\n```\ndate : تاریخ\nindividual_buy_count : تعداد معاملات خرید حقیقی\ncorporate_buy_count : تعداد معلاملات خرید حقوقی\nindividual_sell_count : تعداد معاملات فروش حقیقی\ncorporate_sell_count : تعداد معلاملات فروش حقوقی\nindividual_buy_vol : حجم خرید حقیقی\ncorporate_buy_vol : حجم خرید حقوقی\nindividual_sell_vol : حجم فروش حقیقی\ncorporate_sell_value : حجم فروش حقوقی\nindividual_buy_mean_price : قیمت میانگین خرید حقیقی\nindividual_sell_mean_price : قیمت میانگین فروش حقیقی\ncorporate_buy_mean_price : قیمت میانگین خرید حقوقی\ncorporate_sell_mean_price : قیمت میانگین فروش حقوقی\nindividual_ownership_change : تغییر مالکیت حقوقی به حقیقی\n```\n\n</div>\n\n#### سهامداران عمده\n\nسهام داران عمده اطلاعات داخل این [صفحه](http://tsetmc.com/Loader.aspx?Partree=15131T&c=IRO1BMLT0007) هست.\nاین اطلاعات رو میشه با `shareholders` گرفت که یک DataFrame هست.\n\n\n<div dir="ltr">\n\n```\nticker = Ticker("وبملت")\nprint(ticker.shareholders) # اطلاعات سهام داران عمده\n\n change   percentage       share                                 shareholder  \n0   دولت جمهوري اسلامي ايران                    23,114,768,760  11.160     0     \n1   صندوق تامين آتيه كاركنان بانك ملت           13,353,035,330  6.440      0      \n2   صندوق سرمايه گذاري واسطه گري مالي يكم       11,748,764,647  5.670      0      \n3   شركت پتروشيمي فن آوران-سهامي عام-           9,253,327,080   4.460      0      \n4   شركت گروه مالي ملت-سهام عام-                8,933,698,834   4.310      0      \n5   صندوق سرمايه گذاري.ا.بازارگرداني ملت     8,395,500,914   4.050      0   \n6   شركت سرمايه گذاري صباتامين-سهامي عام-       7,659,597,269   3.690      0      \n7   شركت تعاوني معين آتيه خواهان                4,561,801,327   2.200      0      \n8   شركت س اتهران س.خ-م ك م ف ع-                4,278,903,677   2.060      0      \n9   شركت گروه توسعه مالي مهرآيندگان-سهامي عام-  4,161,561,525   2.000      0      \n10  شركت س اخراسان رضوي س.خ-م ك م ف ع-          3,442,236,423   1.660      0      \n11  شركت س افارس س.خ-م ك م ف ع-                 2,593,956,288   1.250      0      \n12  شركت س اخوزستان س.خ-م ك م ف ع-              2,526,080,803   1.220      0      \n13  شركت شيرين عسل-سهامي خاص-                   2,496,936,881   1.200      0      \n14  شركت سرمايه گذاري ملي ايران-سهامي عام-      2,423,674,676   1.170      0      \n15  شركت س ااصفهان س.خ-م ك م ف ع-               2,274,221,331   1.090      0      \n```\n</div>\n\n##### شناور سهم\nبرای مثال میشه با استفاده از سهامداران عمده شناور سهم رو حساب کرد:\n\n<div dir="ltr">\n\n```\nticker.shareholders.percentage.sum() # جمع سهام داران\n53.63\n\n100 - ticker.shareholders.percentage.sum() # شناور سهم \n46.37\n```\n</div>\n\n##### تاریخچه\u200cی سهام داران عمده\nبا استفاده از تابع get_shareholders_history میشه اطلاعات سهام داران عمده رو گرفت\nورودی\u200cهای تابع:\n```python\nfrom_when=datetime.timedelta(days=90), تعداد روز\u200cهای گذشته پیشفرض ۹۰ روز گذشته است\nto_when=datetime.datetime.now(), تا چه تاریخی اطلاعات گرفته شود پیشفرض امروز هست\nonly_trade_days=True, فقط روز\u200cهای معاملاتی پیش فرض بله\n```\nخروجی این تابع یک دیتا فریم به شکل زیر هست که به صورت csv \n<div dir="ltr">\n\n```\n,date,shares,percentage,instrument_id,shareholder\n0,2021-01-23,3280482041,56.56,IRO1BRKT0003,شركت كارانديش دوران معاصر-سهامي خاص-\n1,2021-01-23,486240253,8.38,IRO1BRKT0003,شركت گروه سرمايه گذاري تدبير-سهامي خاص-\n2,2021-01-23,209066245,3.6,IRO1BRKT0003,شركت سرمايه گذاري پويا-سهامي عام-\n3,2021-01-23,121523528,2.09,IRO1BRKT0003,شركت پالايش پارسيان سپهر-سهامي خاص-\n4,2021-01-23,64873196,1.11,IRO1BRKT0003,BFMصندوق سرمايه گذاري.ا.ب.تدبيرگران فردا\n5,2021-01-24,3280482041,56.56,IRO1BRKT0003,شركت كارانديش دوران معاصر-سهامي خاص-\n6,2021-01-24,486240253,8.38,IRO1BRKT0003,شركت گروه سرمايه گذاري تدبير-سهامي خاص-\n7,2021-01-24,209066245,3.6,IRO1BRKT0003,شركت سرمايه گذاري پويا-سهامي عام-\n8,2021-01-24,121523528,2.09,IRO1BRKT0003,شركت پالايش پارسيان سپهر-سهامي خاص-\n9,2021-01-24,65213196,1.12,IRO1BRKT0003,BFMصندوق سرمايه گذاري.ا.ب.تدبيرگران فردا\n10,2021-01-25,3280482041,56.56,IRO1BRKT0003,شركت كارانديش دوران معاصر-سهامي خاص-\n11,2021-01-25,486240253,8.38,IRO1BRKT0003,شركت گروه سرمايه گذاري تدبير-سهامي خاص-\n12,2021-01-25,209066245,3.6,IRO1BRKT0003,شركت سرمايه گذاري پويا-سهامي عام-\n13,2021-01-25,121523528,2.09,IRO1BRKT0003,شركت پالايش پارسيان سپهر-سهامي خاص-\n14,2021-01-25,68453196,1.18,IRO1BRKT0003,BFMصندوق سرمايه گذاري.ا.ب.تدبيرگران فردا\n```\n</div>\n\n<div id="qa" />\nگرفتن این دیتا کار زمان بری هست(با توجه به تعداد روزی که لازم دارید) و سریع کردن کار با کد به راحتی امکان پذیر نیست. سعی نکنید با همزمان اجرا کردن این تابع برای سهم\u200cهای مختلف روند رو سریع\u200cتر کنید چون سایت ip رو بلاک میکنه.\nاگر موقع اجرای کد پیغام زیر را به تعداد زیاد گرفتید (مثلا هر ثانیه این پیغام اومد) یعنی آیپی شما توسط سایت بورس بلاک شده و چند دقیقه صبر کنید و دوباره ادامه بدید.\n<div dir="ltr">\n\n```\nRetrying pytse_client.ticker.ticker.Ticker._get_ticker_daily_info_page_response in 1.3127419515957892 seconds as it raised ClientResponseError: 500, message=\'Internal Server Error\', url=URL(\'http://cdn.tsetmc.com/Loader.aspx?ParTree=15131P&i=56574323121551263&d=20210220\').\n```\n</div>\n\n##### اطلاعات لحظه\u200cای سهام\nاز طریق تابع `get_ticker_real_time_info_response` میشه اطلاعات لحظه\u200cای سهام رو گرفت.\nنمونه\u200cی استفاده\n\n<div dir="ltr">\n\n```python\nreal_time_data = ticker.get_ticker_real_time_info_response()\n\nprint(real_time_data.buy_orders) # پیشنهادات خرید\nprint(real_time_data.sell_orders) # پیشنهادات فروش\nprint(real_time_data.best_supply_price)  # قیمت بهترین تقاضا\nprint(real_time_data.best_supply_vol)  # حجم بهترین تقاضا\nprint(real_time_data.best_demand_price)  # قیمت بهترین عرضه\nprint(real_time_data.best_demand_vol)  # حجم بهترین عرضه\nprint(real_time_data.adj_close) # آخرین معامله\nprint(real_time_data.last_price) # قیمت پایانی\n\nfor sell_order in real_time_data.sell_orders:\n    print(sell_order.volume, sell_order.count, sell_order.price)\n\nfor buy_order in real_time_data.buy_orders:\n    print(buy_order.volume, buy_order.count, buy_order.price)\n```\n</div>\n\n#### کامیونیتی\n\nاگر درباره پکیج یا استفاده از اون سوالی دارید میتونید توی سرور دیسکورد بپرسید.\n\nhttps://discord.gg/ampPDKHpVv\n\n<div id="required-packages" />\n\n#### پکیج های مورد نیاز:\n\n- [Pandas](https://github.com/pydata/pandas)\n- [Requests](http://docs.python-requests.org/en/master/)\n- [jdatetime](https://github.com/slashmili/python-jalali)\n- [beautifulsoup4](https://pypi.org/project/beautifulsoup4)\n\n<div id="credits" />\n\n#### الهام گرفته از:\n\n- [tehran_stocks](https://github.com/ghodsizadeh/tehran-stocks)\n- [yfinance](https://github.com/ranaroussi/yfinance)\n\n</div>\n',
+    'long_description': '<div dir="rtl">\n\n# دریافت اطلاعات بازار بورس تهران\n\n![Python application](https://github.com/Glyphack/pytse-client/workflows/Python%20application/badge.svg)\n[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Glyphack/pytse-client.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/Glyphack/pytse-client/context:python)\n[![Discord Chat](https://img.shields.io/discord/730808323808559106?label=discord)](https://discord.gg/ampPDKHpVv)\n\nبا استفاده از pytse client میتونید به دیتای بازار بورس تهران در پایتون دسترسی داشته باشید.\nهدف حل مشکلات گرفتن اطلاعات بروز از سایت بازار بورس تهران هست.\n\n## میخواید مشارکت کنید؟\nلطفا [این صفحه](https://github.com/Glyphack/pytse-client/blob/master/CONTRIBUTING.md) رو مطالعه کنید\n\n- [دریافت اطلاعات بازار بورس تهران](#دریافت-اطلاعات-بازار-بورس-تهران)\n  - [میخواید مشارکت کنید؟](#میخواید-مشارکت-کنید)\n  - [قابلیت ها](#قابلیت-ها)\n  - [نصب](#نصب)\n  - [نحوه استفاده](#نحوه-استفاده)\n    - [دانلود سابقه سهم\u200cها](#دانلود-سابقه-سهمها)\n    - [دانلود سابقه معاملات حقیقی و حقوقی به صورت مجزا](#دانلود-سابقه-معاملات-حقیقی-و-حقوقی-به-صورت-مجزا)\n    - [ماژول Ticker](#ماژول-ticker)\n        - [۱نکته](#۱نکته)\n        - [نکته۲](#نکته۲)\n      - [اطلاعات نماد\u200cهای حذف شده](#اطلاعات-نمادهای-حذف-شده)\n      - [اطلاعات حقیقی و حقوقی](#اطلاعات-حقیقی-و-حقوقی)\n      - [سهامداران عمده](#سهامداران-عمده)\n        - [شناور سهم](#شناور-سهم)\n        - [تاریخچه\u200cی سهام داران عمده](#تاریخچهی-سهام-داران-عمده)\n        - [اطلاعات لحظه\u200cای سهام](#اطلاعات-لحظهای-سهام)\n      - [کامیونیتی](#کامیونیتی)\n      - [پکیج های مورد نیاز:](#پکیج-های-مورد-نیاز)\n      - [الهام گرفته از:](#الهام-گرفته-از)\n\n## قابلیت ها\n\n- دریافت اطلاعات روز های معاملاتی هر سهم و قابلیت ذخیره سازی\n- قابلیت گرفتن اطلاعات یک سهام مانند گروه سهام و اطلاعات معاملات حقیقی و حقوقی\n- دریافت اطلاعات فاندامنتال یک نماد شامل(eps, p/e ,حجم مبنا)\n\n## نصب\n\n<div dir="ltr">\n\n```bash\npip install pytse-client\n```\n\n</div>\n\n## نحوه استفاده\n\n### دانلود سابقه سهم\u200cها\n\nبا استفاده از این تابع میتوان سابقه سهام هارو دریافت کرد و هم اون رو ذخیره و هم توی کد استفاده کرد\n\n<div dir="ltr">\n\n```python\nimport pytse_client as tse\ntickers = tse.download(symbols="all", write_to_csv=True)\ntickers["ولملت"] # history\n\n            date     open     high  ...     volume  count    close\n0     2009-02-18   1050.0   1050.0  ...  330851245    800   1050.0\n1     2009-02-21   1051.0   1076.0  ...  335334212   6457   1057.0\n2     2009-02-22   1065.0   1074.0  ...    8435464    603   1055.0\n3     2009-02-23   1066.0   1067.0  ...    8570222    937   1060.0\n4     2009-02-25   1061.0   1064.0  ...    7434309    616   1060.0\n...          ...      ...      ...  ...        ...    ...      ...\n2323  2020-04-14   9322.0   9551.0  ...  105551315  13536   9400.0\n2324  2020-04-15   9410.0   9815.0  ...  201457026  11322   9815.0\n2325  2020-04-18  10283.0  10283.0  ...  142377245   8929  10283.0\n2326  2020-04-19  10797.0  10797.0  ...  292985635  22208  10380.0\n2327  2020-04-20  10600.0  11268.0  ...  295590437  16313  11268.0\n```\n\n</div>\n\nبرای دانلود سابقه یک یا چند سهم کافی هست اسم اون ها به تابع داده بشه:\n\n<div dir="rtl">\n\nهمچنین با گذاشتن\n`write_to_csv=True`\nسابقه سهم توی فایلی با اسم سهم نوشته میشه\n\nسابقه سهم در قالب `Dataframe` است\n\nدرصورتی که می خواهید تاریخ شمسی به خروجی اضافه شود می توانید با گذاشتن\n`include_jdate=True`\nاین امکان را فراهم کنید\n\n</div>\n\n<div dir="ltr">\n\n```python\nimport pytse_client as tse\ntse.download(symbols="وبملت", write_to_csv=True)\ntse.download(symbols="وبملت", write_to_csv=True, include_jdate=True)\ntse.download(symbols=["وبملت", "ولملت"], write_to_csv=True)\n```\n\n</div>\n\n### دانلود سابقه معاملات حقیقی و حقوقی به صورت مجزا\n\nبرای دانلود سابقه معاملات حقیقی و حقوقی برای تمامی نمادها میتوان از تابع زیر استفاده کرد\n\n<div dir="ltr">\n\n```python\nfrom pytse_client import download_client_types_records\n\nif __name__ == \'__main__\':\n\n  records_dict = download_client_types_records("all")\n  print(records_dict["فولاد"])\n  #Output\ndate         individual_buy_count  ... individual_ownership_change\n\n2020-09-01                36298  ...                   -691857.0\n2020-08-31                58185  ...                  83789408.0\n2020-08-26                  461  ...                  21647730.0\n2020-08-25                 1248  ...                  14716846.0\n2020-08-24                38291  ...                -238454702.0\n...                         ...  ...                         ...\n2008-12-02                    7  ...                    -10000.0\n2008-12-01                    8  ...                         0.0\n2008-11-30                   10  ...                    -12781.0\n2008-11-29                  116  ...                   4596856.0\n2008-11-26                   14  ...                    -20000.0\n\n[2518 rows x 17 columns]\n\n```\n\n</div>\n\nمشابه تابع قبلی میتوان نتایج را ذخیره کرد\n\n<div dir="ltr">\n\n```python\nfrom pytse_client import download_client_types_records\nif __name__ == \'__main__\':\n\n  #Records are saved as a .csv file with the same name of ticer\'s\n  records = download_client_types_records("فولاد", write_to_csv=True)\n```\n\n</div>\n\n### ماژول Ticker\n\nاین ماژول برای کار با دیتای یک سهم خاص هست و با گرفتن نماد اطلاعات موجود رو میده\n\nبرای مثال:\n\n<div dir="ltr">\n\n```python\nimport pytse_client as tse\n\ntse.download(symbols="وبملت", write_to_csv=True)  # optional\nticker = tse.Ticker("وبملت")\nprint(ticker.history)  # سابقه قیمت سهم\nprint(ticker.client_types)  # حقیقی حقوقی\nprint(ticker.title)  # نام شرکت\nبانك ملت (وبملت)\nprint(ticker.url)  # آدرس صفحه سهم\nhttp://tsetmc.com/Loader.aspx?ParTree=151311&i=778253364357513\nprint(ticker.group_name)  # نام گروه\nبانكها و موسسات اعتباري\nprint(ticker.eps)  # eps\n2725.0\nprint(ticker.p_e_ratio)  # P/E\n6.1478899082568805\nprint(ticker.group_p_e_ratio)  # group P/E\n18.0\nprint(ticker.base_volume)  # حجم مبنا\n7322431.0\nprint(ticker.last_price)  # آخرین معامله\n17316\nprint(ticker.adj_close)  # قیمت پایانی\n16753\nprint(ticker.best_supply_price)  # قیمت بهترین تقاضا\n26700\nprint(ticker.best_supply_vol)  # حجم بهترین تقاضا\n357062\nprint(ticker.best_demand_price)  # قیمت بهترین عرضه\n26700\nprint(ticker.best_demand_vol)  # حجم بهترین عرضه\n576608\nprint(ticker.shareholders)  # اطلاعات سهام داران عمده\n\nprint(ticker.get_shareholders_history())) # تاریخچه\u200cی سهام داران عمده\nprint(ticker.get_ticker_real_time_info_response()) # اطلاعات لحظه\u200cای مانند قیمت و پیشنهادات خرید و فروش\n\n\n```\n\n</div>\n\nبرای استفاده لازم نیست حتما تابع دانلود صدا زده بشه.\nاگر این کد رو بدون دانلود کردن سهم استفاده کنید خودش اطلاعات سهم رو از سایت میگیره،\nاما اگر قبل از اون از دانلود استفاده کرده باشید\nبه جای گرفتن از اینترنت اطلاعات رو از روی فایل میخونه که سریع تر هست\n\n##### ۱نکته\n\nطبق تجربه\u200c ای که داشتم چون گاهی اوقات سایت بورس مدت زیادی طول میکشه تا اطلاعات رو بفرسته یا بعضی مواقع نمیفرسته بهتر هست که اول تابع دانلود رو استفاده کنید برای سهم\u200cهایی که لازم هست و بعد با دیتای اون ها کار کنید.\n\n##### نکته۲\n\nبعضی از ویژگی\u200cها برای همه\u200cی سهم ها در دسترس نیست. برای مثال بعضی از سهم ها دارای آخرین قیمت یا پی به ای یا ای پی اس نیستند. مقدار این ویژگی\u200cها در صورت نبودن برابر با `None` خواهد بود. پس باید در برنامه خود اینکه این مقادیر وجود دارند را بررسی کنید.\n\n#### اطلاعات نماد\u200cهای حذف شده\nتعدادی از نماد\u200cها توی سایت به شکل حذف شده هستند. برای گرفتن دیتای این نماد\u200cها از ماژول تیکر به شکل زیر استفاده کنید:\nبرای مثال در سهام \nhttp://www.tsetmc.com/Loader.aspx?ParTree=151311&i=25165947991415904\n\n<div dir="ltr">\n\n```python\nimport pytse_client as tse\n\nticker = tse.Ticker("", index="25165947991415904")\n```\n\n</div>\n\nمقدار  \u200d`index` را با مقدار جلوی `i=` جایگزین میکنیم.\n#### اطلاعات حقیقی و حقوقی\n\nاطلاعات خرید و فروش حقیقی و حقوقی سهام رو میشه از طریق `ticker.client_types` گرفت این اطلاعات یه DataFrame شامل اطلاعات موجود در تب حقیقی حقوقی(تب بنفشی که در این [صفحه](http://www.tsetmc.com/Loader.aspx?ParTree=151311&i=778253364357513) هست) سهم هست:\n\n<div dir="ltr">\n\n```\ndate : تاریخ\nindividual_buy_count : تعداد معاملات خرید حقیقی\ncorporate_buy_count : تعداد معلاملات خرید حقوقی\nindividual_sell_count : تعداد معاملات فروش حقیقی\ncorporate_sell_count : تعداد معلاملات فروش حقوقی\nindividual_buy_vol : حجم خرید حقیقی\ncorporate_buy_vol : حجم خرید حقوقی\nindividual_sell_vol : حجم فروش حقیقی\ncorporate_sell_value : حجم فروش حقوقی\nindividual_buy_mean_price : قیمت میانگین خرید حقیقی\nindividual_sell_mean_price : قیمت میانگین فروش حقیقی\ncorporate_buy_mean_price : قیمت میانگین خرید حقوقی\ncorporate_sell_mean_price : قیمت میانگین فروش حقوقی\nindividual_ownership_change : تغییر مالکیت حقوقی به حقیقی\n```\n\n</div>\n\n#### سهامداران عمده\n\nسهام داران عمده اطلاعات داخل این [صفحه](http://tsetmc.com/Loader.aspx?Partree=15131T&c=IRO1BMLT0007) هست.\nاین اطلاعات رو میشه با `shareholders` گرفت که یک DataFrame هست.\n\n\n<div dir="ltr">\n\n```\nticker = Ticker("وبملت")\nprint(ticker.shareholders) # اطلاعات سهام داران عمده\n\n change   percentage       share                                 shareholder  \n0   دولت جمهوري اسلامي ايران                    23,114,768,760  11.160     0     \n1   صندوق تامين آتيه كاركنان بانك ملت           13,353,035,330  6.440      0      \n2   صندوق سرمايه گذاري واسطه گري مالي يكم       11,748,764,647  5.670      0      \n3   شركت پتروشيمي فن آوران-سهامي عام-           9,253,327,080   4.460      0      \n4   شركت گروه مالي ملت-سهام عام-                8,933,698,834   4.310      0      \n5   صندوق سرمايه گذاري.ا.بازارگرداني ملت     8,395,500,914   4.050      0   \n6   شركت سرمايه گذاري صباتامين-سهامي عام-       7,659,597,269   3.690      0      \n7   شركت تعاوني معين آتيه خواهان                4,561,801,327   2.200      0      \n8   شركت س اتهران س.خ-م ك م ف ع-                4,278,903,677   2.060      0      \n9   شركت گروه توسعه مالي مهرآيندگان-سهامي عام-  4,161,561,525   2.000      0      \n10  شركت س اخراسان رضوي س.خ-م ك م ف ع-          3,442,236,423   1.660      0      \n11  شركت س افارس س.خ-م ك م ف ع-                 2,593,956,288   1.250      0      \n12  شركت س اخوزستان س.خ-م ك م ف ع-              2,526,080,803   1.220      0      \n13  شركت شيرين عسل-سهامي خاص-                   2,496,936,881   1.200      0      \n14  شركت سرمايه گذاري ملي ايران-سهامي عام-      2,423,674,676   1.170      0      \n15  شركت س ااصفهان س.خ-م ك م ف ع-               2,274,221,331   1.090      0      \n```\n</div>\n\n##### شناور سهم\nبرای مثال میشه با استفاده از سهامداران عمده شناور سهم رو حساب کرد:\n\n<div dir="ltr">\n\n```\nticker.shareholders.percentage.sum() # جمع سهام داران\n53.63\n\n100 - ticker.shareholders.percentage.sum() # شناور سهم \n46.37\n```\n</div>\n\n##### تاریخچه\u200cی سهام داران عمده\nبا استفاده از تابع get_shareholders_history میشه اطلاعات سهام داران عمده رو گرفت\nورودی\u200cهای تابع:\n```python\nfrom_when=datetime.timedelta(days=90), تعداد روز\u200cهای گذشته پیشفرض ۹۰ روز گذشته است\nto_when=datetime.datetime.now(), تا چه تاریخی اطلاعات گرفته شود پیشفرض امروز هست\nonly_trade_days=True, فقط روز\u200cهای معاملاتی پیش فرض بله\n```\nخروجی این تابع یک دیتا فریم به شکل زیر هست که به صورت csv \n<div dir="ltr">\n\n```\n,date,shareholder_id,shareholder_shares,shareholder_percentage,shareholder_instrument_id,shareholder_name,change\n0,2021-08-30 17:01:23.037957,273,2910355428.0,32.19,IRO1RSAP0000,شركت ايراني توليداتومبيل-سايپا-,1\n1,2021-08-30 17:01:23.037957,406,975144471.0,10.78,IRO1RSAP0000,شركت سايپا,1\n2,2021-08-30 17:01:23.037957,50264,454000000.0,5.02,IRO1RSAP0000,شركت ايراني توليداتومبيل سايپا-سهامي عام-,1\n3,2021-08-30 17:01:23.037957,42636,409843922.0,4.53,IRO1RSAP0000,شركت سرمايه گذاري وتوسعه صنعتي نيوان ابتكارس.ع,1\n4,2021-08-30 17:01:23.037957,46966,116002189.0,1.28,IRO1RSAP0000,BFMصندوق.س.ا.بازارگرداني سهم آشنايكم,1\n5,2021-08-31 17:01:23.037957,273,2910355428.0,32.19,IRO1RSAP0000,شركت ايراني توليداتومبيل-سايپا-,1\n6,2021-08-31 17:01:23.037957,406,975144471.0,10.78,IRO1RSAP0000,شركت سايپا,1\n7,2021-08-31 17:01:23.037957,50264,454000000.0,5.02,IRO1RSAP0000,شركت ايراني توليداتومبيل سايپا-سهامي عام-,1\n8,2021-08-31 17:01:23.037957,42636,409843922.0,4.53,IRO1RSAP0000,شركت سرمايه گذاري وتوسعه صنعتي نيوان ابتكارس.ع,1\n9,2021-08-31 17:01:23.037957,46966,116002189.0,1.28,IRO1RSAP0000,BFMصندوق.س.ا.بازارگرداني سهم آشنايكم,1\n10,2021-09-01 17:01:23.037957,273,2910355428.0,32.19,IRO1RSAP0000,شركت ايراني توليداتومبيل-سايپا-,1\n11,2021-09-01 17:01:23.037957,406,975144471.0,10.78,IRO1RSAP0000,شركت سايپا,1\n12,2021-09-01 17:01:23.037957,50264,454000000.0,5.02,IRO1RSAP0000,شركت ايراني توليداتومبيل سايپا-سهامي عام-,1\n13,2021-09-01 17:01:23.037957,42636,409843922.0,4.53,IRO1RSAP0000,شركت سرمايه گذاري وتوسعه صنعتي نيوان ابتكارس.ع,1\n14,2021-09-01 17:01:23.037957,46966,116002189.0,1.28,IRO1RSAP0000,BFMصندوق.س.ا.بازارگرداني سهم آشنايكم,1\n\n```\n</div>\n\n<div id="qa" />\nگرفتن این دیتا کار زمان بری هست(با توجه به تعداد روزی که لازم دارید) و سریع کردن کار با کد به راحتی امکان پذیر نیست. سعی نکنید با همزمان اجرا کردن این تابع برای سهم\u200cهای مختلف روند رو سریع\u200cتر کنید چون سایت ip رو بلاک میکنه.\nاگر موقع اجرای کد پیغام زیر را به تعداد زیاد گرفتید (مثلا هر ثانیه این پیغام اومد) یعنی آیپی شما توسط سایت بورس بلاک شده و چند دقیقه صبر کنید و دوباره ادامه بدید.\n<div dir="ltr">\n\n```\nRetrying pytse_client.ticker.ticker.Ticker._get_ticker_daily_info_page_response in 1.3127419515957892 seconds as it raised ClientResponseError: 500, message=\'Internal Server Error\', url=URL(\'http://cdn.tsetmc.com/Loader.aspx?ParTree=15131P&i=56574323121551263&d=20210220\').\n```\n</div>\n\n##### اطلاعات لحظه\u200cای سهام\nاز طریق تابع `get_ticker_real_time_info_response` میشه اطلاعات لحظه\u200cای سهام رو گرفت.\nنمونه\u200cی استفاده\n\n<div dir="ltr">\n\n```python\nreal_time_data = ticker.get_ticker_real_time_info_response()\n\nprint(real_time_data.buy_orders) # پیشنهادات خرید\nprint(real_time_data.sell_orders) # پیشنهادات فروش\nprint(real_time_data.best_supply_price)  # قیمت بهترین تقاضا\nprint(real_time_data.best_supply_vol)  # حجم بهترین تقاضا\nprint(real_time_data.best_demand_price)  # قیمت بهترین عرضه\nprint(real_time_data.best_demand_vol)  # حجم بهترین عرضه\nprint(real_time_data.adj_close) # آخرین معامله\nprint(real_time_data.last_price) # قیمت پایانی\n\nfor sell_order in real_time_data.sell_orders:\n    print(sell_order.volume, sell_order.count, sell_order.price)\n\nfor buy_order in real_time_data.buy_orders:\n    print(buy_order.volume, buy_order.count, buy_order.price)\n```\n</div>\n\n#### کامیونیتی\n\nاگر درباره پکیج یا استفاده از اون سوالی دارید میتونید توی سرور دیسکورد بپرسید.\n\nhttps://discord.gg/ampPDKHpVv\n\n<div id="required-packages" />\n\n#### پکیج های مورد نیاز:\n\n- [Pandas](https://github.com/pydata/pandas)\n- [Requests](http://docs.python-requests.org/en/master/)\n- [jdatetime](https://github.com/slashmili/python-jalali)\n- [beautifulsoup4](https://pypi.org/project/beautifulsoup4)\n\n<div id="credits" />\n\n#### الهام گرفته از:\n\n- [tehran_stocks](https://github.com/ghodsizadeh/tehran-stocks)\n- [yfinance](https://github.com/ranaroussi/yfinance)\n\n</div>\n',
     'author': 'glyphack',
     'author_email': 'sh.hooshyari@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pytse-client-0.9.0/PKG-INFO` & `pytse-client-0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytse-client
-Version: 0.9.0
+Version: 0.9.1
 Summary: tehran stock exchange(TSE) client in python
 License: GPLv3
 Author: glyphack
 Author-email: sh.hooshyari@gmail.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -332,30 +332,31 @@
 to_when=datetime.datetime.now(), تا چه تاریخی اطلاعات گرفته شود پیشفرض امروز هست
 only_trade_days=True, فقط روز‌های معاملاتی پیش فرض بله
 ```
 خروجی این تابع یک دیتا فریم به شکل زیر هست که به صورت csv 
 <div dir="ltr">
 
 ```
-,date,shares,percentage,instrument_id,shareholder
-0,2021-01-23,3280482041,56.56,IRO1BRKT0003,شركت كارانديش دوران معاصر-سهامي خاص-
-1,2021-01-23,486240253,8.38,IRO1BRKT0003,شركت گروه سرمايه گذاري تدبير-سهامي خاص-
-2,2021-01-23,209066245,3.6,IRO1BRKT0003,شركت سرمايه گذاري پويا-سهامي عام-
-3,2021-01-23,121523528,2.09,IRO1BRKT0003,شركت پالايش پارسيان سپهر-سهامي خاص-
-4,2021-01-23,64873196,1.11,IRO1BRKT0003,BFMصندوق سرمايه گذاري.ا.ب.تدبيرگران فردا
-5,2021-01-24,3280482041,56.56,IRO1BRKT0003,شركت كارانديش دوران معاصر-سهامي خاص-
-6,2021-01-24,486240253,8.38,IRO1BRKT0003,شركت گروه سرمايه گذاري تدبير-سهامي خاص-
-7,2021-01-24,209066245,3.6,IRO1BRKT0003,شركت سرمايه گذاري پويا-سهامي عام-
-8,2021-01-24,121523528,2.09,IRO1BRKT0003,شركت پالايش پارسيان سپهر-سهامي خاص-
-9,2021-01-24,65213196,1.12,IRO1BRKT0003,BFMصندوق سرمايه گذاري.ا.ب.تدبيرگران فردا
-10,2021-01-25,3280482041,56.56,IRO1BRKT0003,شركت كارانديش دوران معاصر-سهامي خاص-
-11,2021-01-25,486240253,8.38,IRO1BRKT0003,شركت گروه سرمايه گذاري تدبير-سهامي خاص-
-12,2021-01-25,209066245,3.6,IRO1BRKT0003,شركت سرمايه گذاري پويا-سهامي عام-
-13,2021-01-25,121523528,2.09,IRO1BRKT0003,شركت پالايش پارسيان سپهر-سهامي خاص-
-14,2021-01-25,68453196,1.18,IRO1BRKT0003,BFMصندوق سرمايه گذاري.ا.ب.تدبيرگران فردا
+,date,shareholder_id,shareholder_shares,shareholder_percentage,shareholder_instrument_id,shareholder_name,change
+0,2021-08-30 17:01:23.037957,273,2910355428.0,32.19,IRO1RSAP0000,شركت ايراني توليداتومبيل-سايپا-,1
+1,2021-08-30 17:01:23.037957,406,975144471.0,10.78,IRO1RSAP0000,شركت سايپا,1
+2,2021-08-30 17:01:23.037957,50264,454000000.0,5.02,IRO1RSAP0000,شركت ايراني توليداتومبيل سايپا-سهامي عام-,1
+3,2021-08-30 17:01:23.037957,42636,409843922.0,4.53,IRO1RSAP0000,شركت سرمايه گذاري وتوسعه صنعتي نيوان ابتكارس.ع,1
+4,2021-08-30 17:01:23.037957,46966,116002189.0,1.28,IRO1RSAP0000,BFMصندوق.س.ا.بازارگرداني سهم آشنايكم,1
+5,2021-08-31 17:01:23.037957,273,2910355428.0,32.19,IRO1RSAP0000,شركت ايراني توليداتومبيل-سايپا-,1
+6,2021-08-31 17:01:23.037957,406,975144471.0,10.78,IRO1RSAP0000,شركت سايپا,1
+7,2021-08-31 17:01:23.037957,50264,454000000.0,5.02,IRO1RSAP0000,شركت ايراني توليداتومبيل سايپا-سهامي عام-,1
+8,2021-08-31 17:01:23.037957,42636,409843922.0,4.53,IRO1RSAP0000,شركت سرمايه گذاري وتوسعه صنعتي نيوان ابتكارس.ع,1
+9,2021-08-31 17:01:23.037957,46966,116002189.0,1.28,IRO1RSAP0000,BFMصندوق.س.ا.بازارگرداني سهم آشنايكم,1
+10,2021-09-01 17:01:23.037957,273,2910355428.0,32.19,IRO1RSAP0000,شركت ايراني توليداتومبيل-سايپا-,1
+11,2021-09-01 17:01:23.037957,406,975144471.0,10.78,IRO1RSAP0000,شركت سايپا,1
+12,2021-09-01 17:01:23.037957,50264,454000000.0,5.02,IRO1RSAP0000,شركت ايراني توليداتومبيل سايپا-سهامي عام-,1
+13,2021-09-01 17:01:23.037957,42636,409843922.0,4.53,IRO1RSAP0000,شركت سرمايه گذاري وتوسعه صنعتي نيوان ابتكارس.ع,1
+14,2021-09-01 17:01:23.037957,46966,116002189.0,1.28,IRO1RSAP0000,BFMصندوق.س.ا.بازارگرداني سهم آشنايكم,1
+
 ```
 </div>
 
 <div id="qa" />
 گرفتن این دیتا کار زمان بری هست(با توجه به تعداد روزی که لازم دارید) و سریع کردن کار با کد به راحتی امکان پذیر نیست. سعی نکنید با همزمان اجرا کردن این تابع برای سهم‌های مختلف روند رو سریع‌تر کنید چون سایت ip رو بلاک میکنه.
 اگر موقع اجرای کد پیغام زیر را به تعداد زیاد گرفتید (مثلا هر ثانیه این پیغام اومد) یعنی آیپی شما توسط سایت بورس بلاک شده و چند دقیقه صبر کنید و دوباره ادامه بدید.
 <div dir="ltr">
```

