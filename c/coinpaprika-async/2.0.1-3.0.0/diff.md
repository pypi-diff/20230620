# Comparing `tmp/coinpaprika_async-2.0.1.tar.gz` & `tmp/coinpaprika_async-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinpaprika_async-2.0.1.tar", last modified: Sun May 21 18:02:35 2023, max compression
+gzip compressed data, was "coinpaprika_async-3.0.0.tar", last modified: Tue Jun 20 21:14:57 2023, max compression
```

## Comparing `coinpaprika_async-2.0.1.tar` & `coinpaprika_async-3.0.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 18:02:35.158793 coinpaprika_async-2.0.1/
--rw-rw-rw-   0        0        0     1084 2023-05-21 17:45:15.000000 coinpaprika_async-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     2075 2023-05-21 18:02:35.159792 coinpaprika_async-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-05-21 17:45:15.000000 coinpaprika_async-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 18:02:35.123797 coinpaprika_async-2.0.1/coinpaprika_async/
--rw-rw-rw-   0        0        0      228 2023-05-21 17:51:17.000000 coinpaprika_async-2.0.1/coinpaprika_async/__init__.py
--rw-rw-rw-   0        0        0      125 2023-05-21 17:49:59.000000 coinpaprika_async-2.0.1/coinpaprika_async/_version__.py
--rw-rw-rw-   0        0        0      647 2023-05-21 17:45:15.000000 coinpaprika_async-2.0.1/coinpaprika_async/api_exception.py
--rw-rw-rw-   0        0        0     4573 2023-05-21 17:55:39.000000 coinpaprika_async-2.0.1/coinpaprika_async/client.py
--rw-rw-rw-   0        0        0      740 2023-05-21 17:45:15.000000 coinpaprika_async-2.0.1/coinpaprika_async/response_object.py
-drwxrwxrwx   0        0        0        0 2023-05-21 18:02:35.146794 coinpaprika_async-2.0.1/coinpaprika_async.egg-info/
--rw-rw-rw-   0        0        0     2075 2023-05-21 18:02:34.000000 coinpaprika_async-2.0.1/coinpaprika_async.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2023-05-21 18:02:35.000000 coinpaprika_async-2.0.1/coinpaprika_async.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 18:02:34.000000 coinpaprika_async-2.0.1/coinpaprika_async.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-21 18:02:34.000000 coinpaprika_async-2.0.1/coinpaprika_async.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-21 18:02:34.000000 coinpaprika_async-2.0.1/coinpaprika_async.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      209 2023-05-21 17:49:30.000000 coinpaprika_async-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      139 2023-05-21 18:02:35.163810 coinpaprika_async-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-05-21 18:02:12.000000 coinpaprika_async-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 18:02:35.156795 coinpaprika_async-2.0.1/tests/
--rw-rw-rw-   0        0        0     1239 2023-05-21 17:45:15.000000 coinpaprika_async-2.0.1/tests/test_client.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:14:57.926778 coinpaprika_async-3.0.0/
+-rw-rw-rw-   0        0        0     1084 2023-05-21 17:45:15.000000 coinpaprika_async-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2169 2023-06-20 21:14:57.927779 coinpaprika_async-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1400 2023-06-20 20:27:13.000000 coinpaprika_async-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 21:14:57.907777 coinpaprika_async-3.0.0/coinpaprika_async/
+-rw-rw-rw-   0        0        0      147 2023-06-17 19:38:46.000000 coinpaprika_async-3.0.0/coinpaprika_async/__init__.py
+-rw-rw-rw-   0        0        0      125 2023-06-20 20:16:17.000000 coinpaprika_async-3.0.0/coinpaprika_async/_version__.py
+-rw-rw-rw-   0        0        0     1315 2023-06-20 18:32:49.000000 coinpaprika_async-3.0.0/coinpaprika_async/coinpaprika_async_client.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:14:57.920778 coinpaprika_async-3.0.0/coinpaprika_async.egg-info/
+-rw-rw-rw-   0        0        0     2169 2023-06-20 21:14:57.000000 coinpaprika_async-3.0.0/coinpaprika_async.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-06-20 21:14:57.000000 coinpaprika_async-3.0.0/coinpaprika_async.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 21:14:57.000000 coinpaprika_async-3.0.0/coinpaprika_async.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 21:14:57.000000 coinpaprika_async-3.0.0/coinpaprika_async.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-20 21:14:57.000000 coinpaprika_async-3.0.0/coinpaprika_async.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      209 2023-05-21 17:49:30.000000 coinpaprika_async-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      139 2023-06-20 21:14:57.934795 coinpaprika_async-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-06-20 20:16:11.000000 coinpaprika_async-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:14:57.924779 coinpaprika_async-3.0.0/tests/
+-rw-rw-rw-   0        0        0     1893 2023-06-20 18:16:17.000000 coinpaprika_async-3.0.0/tests/test_client.py
```

### Comparing `coinpaprika_async-2.0.1/LICENSE` & `coinpaprika_async-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-2.0.1/PKG-INFO` & `coinpaprika_async-3.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: coinpaprika_async
-Version: 2.0.1
+Version: 3.0.0
 Summary: An asynchronous client for the coinpaprika API.
 Home-page: https://github.com/DroidZed/coinpaprika-async-client.git
 Author: DroidZed
 Author-email: droid.zed77@outlook.com
 License: MIT
 Keywords: coinpaprika_async api cryptocurrency async httpx client
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <h1 style="font-size:50px;">Coinpaprika Async Client</h1>
-  
+
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/coinpaprika-async)
-[![Actions Status](https://github.com/DroidZed/coinpaprika-async-client/workflows/Python%20package/badge.svg)](https://github.com/DroidZed/coinpaprika-async-client/actions)
-  
+
 </div>
 
 ## 1. Usage
 
 This library provides convenient and modern way to use [coinpaprika.com](https://api.coinpaprika.com/) API in Python.
 
 [Coinpaprika](https://coinpaprika.com/) delivers full market data to the world of crypto: coin prices, volumes, market caps, ATHs, return rates and more.
@@ -43,19 +41,26 @@
 
 ```sh
 pipenv install coinpaprika_async
 ```
 
 ## 3. Getting started
 
-```py
-from coinpaprika_async import Client
+Each top-level path has their own endpoint class now:
+
+
+- `GET` /coins `->` `CoinsEndpoint`
+- `GET` /exchanges `->` `ExchangesEndpoint`
+- `GET` /key `->` `KeyEndpoint`
+- `GET` /global `->` `MarketEndpoint`
+- `GET` /search + /price-converter `->` `MiscelanousEndpoints`
+- `GET` /people `->` `PeopleEndpoint`
+- `GET` /tags `->` `TagsEndpoint`
+- `GET` /tickers `->` `TickersEndpoint`
 
-client = Client()
-```
 
 ## 4 Examples:
 
 Check out the [examples](./examples) directory.
 
 ## 5. Tests
```

### Comparing `coinpaprika_async-2.0.1/coinpaprika_async.egg-info/PKG-INFO` & `coinpaprika_async-3.0.0/coinpaprika_async.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: coinpaprika-async
-Version: 2.0.1
+Version: 3.0.0
 Summary: An asynchronous client for the coinpaprika API.
 Home-page: https://github.com/DroidZed/coinpaprika-async-client.git
 Author: DroidZed
 Author-email: droid.zed77@outlook.com
 License: MIT
 Keywords: coinpaprika_async api cryptocurrency async httpx client
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 <h1 style="font-size:50px;">Coinpaprika Async Client</h1>
-  
+
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/coinpaprika-async)
-[![Actions Status](https://github.com/DroidZed/coinpaprika-async-client/workflows/Python%20package/badge.svg)](https://github.com/DroidZed/coinpaprika-async-client/actions)
-  
+
 </div>
 
 ## 1. Usage
 
 This library provides convenient and modern way to use [coinpaprika.com](https://api.coinpaprika.com/) API in Python.
 
 [Coinpaprika](https://coinpaprika.com/) delivers full market data to the world of crypto: coin prices, volumes, market caps, ATHs, return rates and more.
@@ -43,19 +41,26 @@
 
 ```sh
 pipenv install coinpaprika_async
 ```
 
 ## 3. Getting started
 
-```py
-from coinpaprika_async import Client
+Each top-level path has their own endpoint class now:
+
+
+- `GET` /coins `->` `CoinsEndpoint`
+- `GET` /exchanges `->` `ExchangesEndpoint`
+- `GET` /key `->` `KeyEndpoint`
+- `GET` /global `->` `MarketEndpoint`
+- `GET` /search + /price-converter `->` `MiscelanousEndpoints`
+- `GET` /people `->` `PeopleEndpoint`
+- `GET` /tags `->` `TagsEndpoint`
+- `GET` /tickers `->` `TickersEndpoint`
 
-client = Client()
-```
 
 ## 4 Examples:
 
 Check out the [examples](./examples) directory.
 
 ## 5. Tests
```

### Comparing `coinpaprika_async-2.0.1/setup.py` & `coinpaprika_async-3.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import setup
 
 setup(
     name="coinpaprika_async",
-    version="2.0.1",
+    version="3.0.0",
     author="DroidZed",
     author_email="droid.zed77@outlook.com",
     description="An asynchronous client for the coinpaprika API.",
     packages=["coinpaprika_async"],
     url="https://github.com/DroidZed/coinpaprika-async-client.git",
     license="MIT",
     install_requires=["httpx"],
     keywords="coinpaprika_async api cryptocurrency async httpx client",
     classifiers=[
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

