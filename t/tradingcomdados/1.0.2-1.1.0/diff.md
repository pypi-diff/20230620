# Comparing `tmp/tradingcomdados-1.0.2.tar.gz` & `tmp/tradingcomdados-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingcomdados-1.0.2.tar", last modified: Wed May 24 11:28:49 2023, max compression
+gzip compressed data, was "tradingcomdados-1.1.0.tar", last modified: Tue Jun 20 01:26:24 2023, max compression
```

## Comparing `tradingcomdados-1.0.2.tar` & `tradingcomdados-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 11:28:49.105525 tradingcomdados-1.0.2/
--rw-rw-rw-   0        0        0      992 2023-05-24 11:28:49.105525 tradingcomdados-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      790 2023-05-23 23:43:04.000000 tradingcomdados-1.0.2/README.md
--rw-rw-rw-   0        0        0      301 2023-05-24 11:28:42.000000 tradingcomdados-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 11:28:49.105525 tradingcomdados-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 11:28:49.096503 tradingcomdados-1.0.2/tradingcomdados/
--rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.0.2/tradingcomdados/__init__.py
--rw-rw-rw-   0        0        0     7742 2023-05-23 23:32:14.000000 tradingcomdados-1.0.2/tradingcomdados/data_provider.py
-drwxrwxrwx   0        0        0        0 2023-05-24 11:28:49.104517 tradingcomdados-1.0.2/tradingcomdados.egg-info/
--rw-rw-rw-   0        0        0      992 2023-05-24 11:28:48.000000 tradingcomdados-1.0.2/tradingcomdados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-05-24 11:28:49.000000 tradingcomdados-1.0.2/tradingcomdados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 11:28:48.000000 tradingcomdados-1.0.2/tradingcomdados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-05-24 11:28:48.000000 tradingcomdados-1.0.2/tradingcomdados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-24 11:28:48.000000 tradingcomdados-1.0.2/tradingcomdados.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 01:26:24.009292 tradingcomdados-1.1.0/
+-rw-rw-rw-   0        0        0     1173 2023-06-20 01:26:24.008288 tradingcomdados-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-06-20 00:24:03.000000 tradingcomdados-1.1.0/README.md
+-rw-rw-rw-   0        0        0      301 2023-06-20 01:23:45.000000 tradingcomdados-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 01:26:24.009292 tradingcomdados-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:26:23.997772 tradingcomdados-1.1.0/tradingcomdados/
+-rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.1.0/tradingcomdados/__init__.py
+-rw-rw-rw-   0        0        0     7732 2023-06-20 00:37:56.000000 tradingcomdados-1.1.0/tradingcomdados/data_provider.py
+-rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.1.0/tradingcomdados/unsupervised_learning.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:26:24.007774 tradingcomdados-1.1.0/tradingcomdados.egg-info/
+-rw-rw-rw-   0        0        0     1173 2023-06-20 01:26:22.000000 tradingcomdados-1.1.0/tradingcomdados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-06-20 01:26:23.000000 tradingcomdados-1.1.0/tradingcomdados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 01:26:22.000000 tradingcomdados-1.1.0/tradingcomdados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-06-20 01:26:22.000000 tradingcomdados-1.1.0/tradingcomdados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-20 01:26:22.000000 tradingcomdados-1.1.0/tradingcomdados.egg-info/top_level.txt
```

### Comparing `tradingcomdados-1.0.2/PKG-INFO` & `tradingcomdados-1.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1
-Name: tradingcomdados
-Version: 1.0.2
-Summary: tradingcomdados
-Author: Lucas Roberto Correa
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # tradingcomdados
 
+## Introduction
 *Trading com Dados Library for quantitative finance*
 
 The library consists of a collection of methods that can be used in order to help Data Scientists, Quantitative Analysts and data professionals during the development of quantitative finance applications. One of the main objectives of the library is to provide methods to connect to Trading com dados' data provider services.
 
 ## Library Motivation and Description
 Trading com dados is an Edtech that provides educational content for people who want to know quantitative finance and in order to obtain that knowlegde, we need quality data, thus this library and our API service was created to solve that.
 
 ## API methods
 -> get_data
+
 -> get_data_tickers
 
 
 ## How to install
+```python 
 pip install tradingcomdados
+```
 
-
+## Importing and fetching data
+```python
+import tradingcomdados as tcd
+
+# Fetching data
+tcd.get_data('PETR4', start = '01/01/2019')
+```
```

### Comparing `tradingcomdados-1.0.2/setup.py` & `tradingcomdados-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.0.2/tradingcomdados/data_provider.py` & `tradingcomdados-1.1.0/tradingcomdados/data_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             "An error occured during the process of gathering data, please check the ticker and dates used and also remember to use a valid api key"
         )
 
 
 def _request_type_validation(data_type, request_type, ticker):
 
     try:
-        url_base = "https://api.tradingcomdados.com.br"
+        url_base = "https://api.fintz.com.br"
 
         if data_type == "stock":
 
             def _check_request_type_stock(request_type):
 
                 if request_type == "historical_data_stock":
                     endpoint = url_base + "/bolsa/b3/avista/cotacoes/historico"
```

### Comparing `tradingcomdados-1.0.2/tradingcomdados.egg-info/PKG-INFO` & `tradingcomdados-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.0.2
+Version: 1.1.0
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # tradingcomdados
 
+## Introduction
 *Trading com Dados Library for quantitative finance*
 
 The library consists of a collection of methods that can be used in order to help Data Scientists, Quantitative Analysts and data professionals during the development of quantitative finance applications. One of the main objectives of the library is to provide methods to connect to Trading com dados' data provider services.
 
 ## Library Motivation and Description
 Trading com dados is an Edtech that provides educational content for people who want to know quantitative finance and in order to obtain that knowlegde, we need quality data, thus this library and our API service was created to solve that.
 
 ## API methods
 -> get_data
+
 -> get_data_tickers
 
 
 ## How to install
+```python 
 pip install tradingcomdados
+```
+
+## Importing and fetching data
+```python
+import tradingcomdados as tcd
+
+# Fetching data
+tcd.get_data('PETR4', start = '01/01/2019')
+```
```

