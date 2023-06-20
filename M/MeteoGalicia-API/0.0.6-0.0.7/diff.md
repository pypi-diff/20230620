# Comparing `tmp/MeteoGalicia-API-0.0.6.tar.gz` & `tmp/MeteoGalicia-API-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeteoGalicia-API-0.0.6.tar", last modified: Fri Dec 30 21:33:39 2022, max compression
+gzip compressed data, was "MeteoGalicia-API-0.0.7.tar", last modified: Tue Jun 20 21:13:15 2023, max compression
```

## Comparing `MeteoGalicia-API-0.0.6.tar` & `MeteoGalicia-API-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2022-12-30 21:33:39.115541 MeteoGalicia-API-0.0.6/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2022-12-30 21:13:33.000000 MeteoGalicia-API-0.0.6/LICENSE.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       61 2022-12-30 21:13:33.000000 MeteoGalicia-API-0.0.6/MANIFEST.in
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2022-12-30 21:33:39.115541 MeteoGalicia-API-0.0.6/MeteoGalicia_API.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2111 2022-12-30 21:33:39.000000 MeteoGalicia-API-0.0.6/MeteoGalicia_API.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      391 2022-12-30 21:33:39.000000 MeteoGalicia-API-0.0.6/MeteoGalicia_API.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2022-12-30 21:33:39.000000 MeteoGalicia-API-0.0.6/MeteoGalicia_API.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2022-12-30 21:33:39.000000 MeteoGalicia-API-0.0.6/MeteoGalicia_API.egg-info/not-zip-safe
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2022-12-30 21:33:39.000000 MeteoGalicia-API-0.0.6/MeteoGalicia_API.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2022-12-30 21:33:39.000000 MeteoGalicia-API-0.0.6/MeteoGalicia_API.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     2111 2022-12-30 21:33:39.115541 MeteoGalicia-API-0.0.6/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1145 2022-12-30 21:13:33.000000 MeteoGalicia-API-0.0.6/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2022-12-30 21:33:39.115541 MeteoGalicia-API-0.0.6/meteogalicia_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       29 2022-12-30 21:13:33.000000 MeteoGalicia-API-0.0.6/meteogalicia_api/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       36 2022-12-30 21:13:33.000000 MeteoGalicia-API-0.0.6/meteogalicia_api/const.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1639 2022-12-30 21:32:04.000000 MeteoGalicia-API-0.0.6/meteogalicia_api/interface.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2022-12-30 21:13:33.000000 MeteoGalicia-API-0.0.6/requirements.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       54 2022-12-30 21:33:39.115541 MeteoGalicia-API-0.0.6/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1788 2022-12-30 21:32:41.000000 MeteoGalicia-API-0.0.6/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 21:13:15.171267 MeteoGalicia-API-0.0.7/
+-rw-r--r--   0 pi        (1000) pi        (1000)    35149 2023-06-20 17:56:00.000000 MeteoGalicia-API-0.0.7/LICENSE.md
+-rw-r--r--   0 pi        (1000) pi        (1000)       61 2023-06-20 17:56:00.000000 MeteoGalicia-API-0.0.7/MANIFEST.in
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 21:13:15.163267 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2388 2023-06-20 21:13:14.000000 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      391 2023-06-20 21:13:15.000000 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-20 21:13:14.000000 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-20 21:13:14.000000 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/not-zip-safe
+-rw-r--r--   0 pi        (1000) pi        (1000)        9 2023-06-20 21:13:14.000000 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       17 2023-06-20 21:13:14.000000 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)     2388 2023-06-20 21:13:15.171267 MeteoGalicia-API-0.0.7/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     1145 2023-06-20 17:56:00.000000 MeteoGalicia-API-0.0.7/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 21:13:15.167267 MeteoGalicia-API-0.0.7/meteogalicia_api/
+-rw-r--r--   0 pi        (1000) pi        (1000)       29 2023-06-20 17:56:00.000000 MeteoGalicia-API-0.0.7/meteogalicia_api/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       36 2023-06-20 17:56:00.000000 MeteoGalicia-API-0.0.7/meteogalicia_api/const.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1595 2023-06-20 21:10:50.000000 MeteoGalicia-API-0.0.7/meteogalicia_api/interface.py
+-rw-r--r--   0 pi        (1000) pi        (1000)        8 2023-06-20 17:56:00.000000 MeteoGalicia-API-0.0.7/requirements.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       54 2023-06-20 21:13:15.175267 MeteoGalicia-API-0.0.7/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)     1838 2023-06-20 21:12:37.000000 MeteoGalicia-API-0.0.7/setup.py
```

### Comparing `MeteoGalicia-API-0.0.6/LICENSE.md` & `MeteoGalicia-API-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MeteoGalicia-API-0.0.6/README.md` & `MeteoGalicia-API-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `MeteoGalicia-API-0.0.6/meteogalicia_api/interface.py` & `MeteoGalicia-API-0.0.7/meteogalicia_api/interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 """Client for the Meteogalicia REST API."""
 import logging
 from datetime import datetime, timedelta
-
 import requests
+
 URL_FORECAST = "https://servizos.meteogalicia.gal/mgrss/predicion/jsonPredConcellos.action?idConc={}"
 URL_OBSERVATION = "https://servizos.meteogalicia.gal/mgrss/observacion/observacionConcellos.action?idConcello={}"
 
 
-_LOGGER = logging.getLogger(__name__)
 
 class MeteoGalicia:
     """Class to interact with the MeteoGalicia web service."""
     def __init__( self,  log_level=logging.WARNING):
-        logging.getLogger().setLevel(log_level)
+        self.logger = logging.getLogger(__name__)
+        self.logger.setLevel(log_level)
         self._session = requests.Session()
     
     def _do_get(self, url, id):
         result = None
         r = self._session.get(url.format(id),timeout=15)
         if r.status_code == 200:
-                _LOGGER.debug("data received for %s", id)
+                self.logger.debug(f"Data received for {id}")
                 
                 result = r.json()
         else:
-                _LOGGER.error("error code %s for %s - returned: %s",  r.status_code,
-                    id,
-                    r.text,
-                    
-                )
+                self.logger.error(f"error code {r.status_code} for code: {id} - returned: {r.text}")
         return result
 
     def get_forecast_data(self,id):
         r = self._do_get(URL_FORECAST,id)
         if (r==None ):
-            _LOGGER.error("No data for %s", id)
+            self.logger.error(f"No data for code: {id}")
         elif ((r['predConcello'])==None):
-                _LOGGER.debug("No forecast data for %s", id)
+                self.logger.debug(f"No forecast data for {id}")
         return r
     
     def get_observation_data(self,id):
         r = self._do_get(URL_OBSERVATION,id)
         if (r==None):
-            _LOGGER.error("No data for %s", id)
+            self.logger.error(f"No data for code: {id}")
         elif (len(r['listaObservacionConcellos'])==0):
-             _LOGGER.debug("No observation data for %s", id)
+             self.logger.debug(f"No observation data for {id}")
         return r
```

### Comparing `MeteoGalicia-API-0.0.6/setup.py` & `MeteoGalicia-API-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 NAME = "MeteoGalicia-API"
 DESCRIPTION = (
     "Python library for get info from MeteoGalicia web service. MeteoGalicia is the meteorological agency for Galicia, Spain"
 )
 URL = "https://github.com/danieldiazi/meteogalicia-api"
 EMAIL = "dandiazde@gmail.com"
 AUTHOR = "danieldiazi"
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 
 here = lambda *a: os.path.join(os.path.dirname(__file__), *a)
 requirements = [x.strip() for x in open(here('requirements.txt')).readlines()]
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 try:
@@ -50,10 +50,11 @@
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.11'
       ],
 )
```

