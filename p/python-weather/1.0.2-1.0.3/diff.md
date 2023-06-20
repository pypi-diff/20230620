# Comparing `tmp/python-weather-1.0.2.tar.gz` & `tmp/python-weather-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-weather-1.0.2.tar", last modified: Thu May 18 11:48:31 2023, max compression
+gzip compressed data, was "python-weather-1.0.3.tar", last modified: Tue Jun 20 14:31:57 2023, max compression
```

## Comparing `python-weather-1.0.2.tar` & `python-weather-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 11:48:31.217005 python-weather-1.0.2/
--rw-rw-rw-   0        0        0     1106 2023-04-07 14:23:45.000000 python-weather-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      107 2023-04-25 12:21:36.000000 python-weather-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3760 2023-05-18 11:48:31.213070 python-weather-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2176 2023-04-29 06:26:46.000000 python-weather-1.0.2/README.md
--rw-rw-rw-   0        0        0     1437 2023-05-18 11:41:38.000000 python-weather-1.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-18 11:48:31.094670 python-weather-1.0.2/python_weather/
--rw-rw-rw-   0        0        0     1503 2023-05-18 11:41:38.000000 python-weather-1.0.2/python_weather/__init__.py
--rw-rw-rw-   0        0        0     5663 2023-04-29 06:25:45.000000 python-weather-1.0.2/python_weather/base.py
--rw-rw-rw-   0        0        0     5683 2023-04-29 06:25:45.000000 python-weather-1.0.2/python_weather/client.py
--rw-rw-rw-   0        0        0     1295 2023-04-29 06:25:45.000000 python-weather-1.0.2/python_weather/constants.py
--rw-rw-rw-   0        0        0    10130 2023-05-18 11:37:15.000000 python-weather-1.0.2/python_weather/enums.py
--rw-rw-rw-   0        0        0     1262 2023-04-29 06:25:45.000000 python-weather-1.0.2/python_weather/errors.py
--rw-rw-rw-   0        0        0    12867 2023-05-18 11:37:15.000000 python-weather-1.0.2/python_weather/forecast.py
-drwxrwxrwx   0        0        0        0 2023-05-18 11:48:31.191871 python-weather-1.0.2/python_weather.egg-info/
--rw-rw-rw-   0        0        0     3760 2023-05-18 11:48:30.000000 python-weather-1.0.2/python_weather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-05-18 11:48:30.000000 python-weather-1.0.2/python_weather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 11:48:30.000000 python-weather-1.0.2/python_weather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-18 11:48:30.000000 python-weather-1.0.2/python_weather.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-18 11:48:30.000000 python-weather-1.0.2/python_weather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 11:48:31.217615 python-weather-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 14:31:57.385029 python-weather-1.0.3/
+-rw-rw-rw-   0        0        0     1106 2023-06-20 11:11:09.000000 python-weather-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      107 2023-06-20 11:11:10.000000 python-weather-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3760 2023-06-20 14:31:57.285037 python-weather-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2176 2023-06-20 11:11:10.000000 python-weather-1.0.3/README.md
+-rw-rw-rw-   0        0        0     1437 2023-06-20 11:29:39.000000 python-weather-1.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-20 14:31:57.045030 python-weather-1.0.3/python_weather/
+-rw-rw-rw-   0        0        0     1503 2023-06-20 11:29:01.000000 python-weather-1.0.3/python_weather/__init__.py
+-rw-rw-rw-   0        0        0     5668 2023-06-20 11:28:22.000000 python-weather-1.0.3/python_weather/base.py
+-rw-rw-rw-   0        0        0     5683 2023-06-20 11:11:10.000000 python-weather-1.0.3/python_weather/client.py
+-rw-rw-rw-   0        0        0     1295 2023-06-20 11:11:10.000000 python-weather-1.0.3/python_weather/constants.py
+-rw-rw-rw-   0        0        0    13170 2023-06-20 14:18:24.000000 python-weather-1.0.3/python_weather/enums.py
+-rw-rw-rw-   0        0        0     1262 2023-06-20 11:11:10.000000 python-weather-1.0.3/python_weather/errors.py
+-rw-rw-rw-   0        0        0    12794 2023-06-20 12:25:08.000000 python-weather-1.0.3/python_weather/forecast.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:31:57.285037 python-weather-1.0.3/python_weather.egg-info/
+-rw-rw-rw-   0        0        0     3760 2023-06-20 14:31:56.000000 python-weather-1.0.3/python_weather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-06-20 14:31:56.000000 python-weather-1.0.3/python_weather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:31:56.000000 python-weather-1.0.3/python_weather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-20 14:31:56.000000 python-weather-1.0.3/python_weather.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-20 14:31:56.000000 python-weather-1.0.3/python_weather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:31:57.385029 python-weather-1.0.3/setup.cfg
```

### Comparing `python-weather-1.0.2/LICENSE` & `python-weather-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.2/PKG-INFO` & `python-weather-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: python-weather
-Version: 1.0.2
+Version: 1.0.3
 Summary: A free and asynchronous weather API wrapper made in Python, for Python.
 Author: null8626
 License: MIT
 Project-URL: repository, https://github.com/null8626/python-weather
-Project-URL: download_url, https://github.com/null8626/python-weather/archive/1.0.2.tar.gz
+Project-URL: download_url, https://github.com/null8626/python-weather/archive/1.0.3.tar.gz
 Keywords: weather,forecast,weather-api,weather-forecast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: aiohttp
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-weather-1.0.2/README.md` & `python-weather-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.2/pyproject.toml` & `python-weather-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "python-weather"
-version = "1.0.2"
+version = "1.0.3"
 description = "A free and asynchronous weather API wrapper made in Python, for Python."
 readme = "README.md"
 license = { text = "MIT" }
 authors = [{ name = "null8626" }]
 keywords = ["weather", "forecast", "weather-api", "weather-forecast"]
 dependencies = ["aiohttp==3.8.4"]
 classifiers = [
@@ -34,8 +34,8 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12"
 ]
 requires-python = ">=3.7"
 
 [project.urls]
 repository = "https://github.com/null8626/python-weather"
-download_url = "https://github.com/null8626/python-weather/archive/1.0.2.tar.gz"
+download_url = "https://github.com/null8626/python-weather/archive/1.0.3.tar.gz"
```

### Comparing `python-weather-1.0.2/python_weather/__init__.py` & `python-weather-1.0.3/python_weather/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,12 +26,12 @@
 """
 
 from .enums import Kind, Locale, Phase, Ultraviolet, WindDirection
 from .constants import METRIC, IMPERIAL
 from .client import Client
 from .errors import Error
 
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 __all__ = (
   'METRIC', 'IMPERIAL', 'Client', 'Error', 'Kind', 'Locale', 'Phase',
   'Ultraviolet', 'WindDirection'
 )
```

### Comparing `python-weather-1.0.2/python_weather/base.py` & `python-weather-1.0.3/python_weather/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     
     super().__init__(unit, locale)
   
   @property
   def ultraviolet(self) -> Ultraviolet:
     """:class:`Ultraviolet`: The UV (:term:`ultraviolet`) index."""
     
-    return Ultraviolet(int(self.__inner['uvIndex']))
+    return Ultraviolet._new(int(self.__inner['uvIndex']))
   
   @property
   def feels_like(self) -> int:
     """:class:`int`: What it felt like, in Celcius or Fahrenheit."""
     
     return int(
       self.__inner[
```

### Comparing `python-weather-1.0.2/python_weather/client.py` & `python-weather-1.0.3/python_weather/client.py`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.2/python_weather/constants.py` & `python-weather-1.0.3/python_weather/constants.py`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.2/python_weather/errors.py` & `python-weather-1.0.3/python_weather/errors.py`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.2/python_weather/forecast.py` & `python-weather-1.0.3/python_weather/forecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,17 @@
 SOFTWARE.
 """
 
 from typing import Iterable, Optional, Tuple
 from datetime import datetime, date, time
 from enum import auto
 
-from .enums import Kind, Phase, WindDirection, Locale, Ultraviolet
-from .constants import VALID_UNITS, LATLON_REGEX, METRIC
+from .enums import Phase, Locale
+from .constants import LATLON_REGEX, METRIC
 from .base import BaseForecast, CustomizableBase
-from .errors import Error
 
 class Area:
   """Represents the location of the weather forecast."""
   
   __slots__ = ('__inner',)
   
   def __init__(self, json: dict):
```

### Comparing `python-weather-1.0.2/python_weather.egg-info/PKG-INFO` & `python-weather-1.0.3/python_weather.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: python-weather
-Version: 1.0.2
+Version: 1.0.3
 Summary: A free and asynchronous weather API wrapper made in Python, for Python.
 Author: null8626
 License: MIT
 Project-URL: repository, https://github.com/null8626/python-weather
-Project-URL: download_url, https://github.com/null8626/python-weather/archive/1.0.2.tar.gz
+Project-URL: download_url, https://github.com/null8626/python-weather/archive/1.0.3.tar.gz
 Keywords: weather,forecast,weather-api,weather-forecast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: aiohttp
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

