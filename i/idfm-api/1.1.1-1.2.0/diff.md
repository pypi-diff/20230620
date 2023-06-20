# Comparing `tmp/idfm_api-1.1.1.tar.gz` & `tmp/idfm_api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idfm_api-1.1.1.tar", last modified: Sun Dec 18 15:43:58 2022, max compression
+gzip compressed data, was "idfm_api-1.2.0.tar", last modified: Tue Jun 20 17:19:08 2023, max compression
```

## Comparing `idfm_api-1.1.1.tar` & `idfm_api-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 15:43:58.195421 idfm_api-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2022-12-18 15:42:57.000000 idfm_api-1.1.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2022-12-18 15:43:58.195421 idfm_api-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2022-12-18 15:42:57.000000 idfm_api-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 15:43:58.187421 idfm_api-1.1.1/idfm_api/
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2022-12-18 15:42:57.000000 idfm_api-1.1.1/idfm_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2022-12-18 15:42:57.000000 idfm_api-1.1.1/idfm_api/attribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    68158 2022-12-18 15:43:42.000000 idfm_api-1.1.1/idfm_api/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2022-12-18 15:42:57.000000 idfm_api-1.1.1/idfm_api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)  7167700 2022-12-18 15:43:42.000000 idfm_api-1.1.1/idfm_api/stops.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 15:43:58.195421 idfm_api-1.1.1/idfm_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2022-12-18 15:43:58.000000 idfm_api-1.1.1/idfm_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2022-12-18 15:43:58.000000 idfm_api-1.1.1/idfm_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-18 15:43:58.000000 idfm_api-1.1.1/idfm_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-18 15:43:58.000000 idfm_api-1.1.1/idfm_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-18 15:43:58.000000 idfm_api-1.1.1/idfm_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-18 15:43:58.195421 idfm_api-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      977 2022-12-18 15:42:57.000000 idfm_api-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:19:08.637329 idfm_api-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-20 17:17:52.000000 idfm_api-1.2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-20 17:19:08.637329 idfm_api-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-20 17:17:52.000000 idfm_api-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:19:08.625329 idfm_api-1.2.0/idfm_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-06-20 17:17:52.000000 idfm_api-1.2.0/idfm_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-20 17:17:52.000000 idfm_api-1.2.0/idfm_api/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70382 2023-06-20 17:18:54.000000 idfm_api-1.2.0/idfm_api/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-20 17:17:52.000000 idfm_api-1.2.0/idfm_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123) 11821534 2023-06-20 17:18:55.000000 idfm_api-1.2.0/idfm_api/stops.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:19:08.637329 idfm_api-1.2.0/idfm_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-20 17:19:08.000000 idfm_api-1.2.0/idfm_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-20 17:19:08.000000 idfm_api-1.2.0/idfm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:19:08.000000 idfm_api-1.2.0/idfm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 17:19:08.000000 idfm_api-1.2.0/idfm_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 17:19:08.000000 idfm_api-1.2.0/idfm_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:19:08.637329 idfm_api-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-20 17:17:52.000000 idfm_api-1.2.0/setup.py
```

### Comparing `idfm_api-1.1.1/LICENCE` & `idfm_api-1.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `idfm_api-1.1.1/PKG-INFO` & `idfm_api-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idfm_api
-Version: 1.1.1
+Version: 1.2.0
 Summary: API for Ile de france mobilite
 Home-page: https://github.com/droso-hass/idfm-api
 Author: drosocode
 License: MIT
 Project-URL: Documentation, https://idfm-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/droso-hass/idfm-api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `idfm_api-1.1.1/idfm_api/__init__.py` & `idfm_api-1.2.0/idfm_api/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,23 +19,31 @@
     async def __request(self, url):
         """
         API request helper
         Args:
             url: the url to request
         Returns:
             A json object
+        Raises:
+            UnknownIdentifierException
         """
         try:
             async with async_timeout.timeout(self._timeout):
                 response = await self._session.get(url, headers={
                     "apiKey": self._apikey,
                     "Content-Type": "application/json",
                     "Accept-encoding": "gzip, deflate"
                 })
                 if response.status != 200:
+                    try:
+                        err = (await response.json())["Siri"]["ServiceDelivery"]["StopMonitoringDelivery"][0]["ErrorCondition"]["ErrorInformation"]["ErrorText"]
+                        if err == "Le couple MonitoringRef/LineRef n'existe pas" or err == "La requête contient des identifiants qui sont inconnus":
+                            raise UnknownIdentifierException()
+                    except KeyError:
+                        pass
                     _LOGGER.warn(
                         "Error while fetching information from %s - %s",
                         url,
                         response._body,
                     )
                 resp = (await response.json())["Siri"]["ServiceDelivery"]
                 if "GeneralMessageDelivery" in resp:
@@ -55,16 +63,14 @@
 
         except asyncio.TimeoutError as exception:
             _LOGGER.error(
                 "Timeout error fetching information from %s - %s",
                 url,
                 exception,
             )
-        except Exception as exception:  # pylint: disable=broad-except
-            _LOGGER.error("Something really wrong happened! - %s", exception)
 
     async def get_stops(self, line_id: str) -> List[StopData]:
         """
         Return a list of stop areas corresponding to the specified line
         Args:
             line_id: A string indicating id of a line
         Returns:
@@ -74,46 +80,60 @@
         with importlib.resources.open_text("idfm_api", "stops.json", encoding="utf8") as f:
             data = json.load(f)
             if line_id in data:
                 for i in data[line_id]:
                     ret.append(StopData.from_json(i))
         return ret
 
-    async def get_traffic(self, stop_id: str, destination_name: Optional[str] = None, direction_name: Optional[str] = None) -> List[TrafficData]:
+    async def get_traffic(self, stop_id: str, destination_name: Optional[str] = None, direction_name: Optional[str] = None, line_id: Optional[str] = None) -> List[TrafficData]:
         """
         Returns the next schedules in a line for a specified depart area to an optional destination
         
         Args:
             stop_id: A string indicating the id of the depart stop area
             destination_name: A string indicating the final destination (I.E. the station name returned by get_directions), the schedules for all the available destinations are returned if not specified
             direction_name: A boolean indicating the direction of a train, ignored if not specified
+            line_id: A string indicating id of a line (if not specified, all schedules for this stop/direction will be returned regardless of the line)
         Returns:
             A list of TrafficData objects
         """
-        d = f"https://prim.iledefrance-mobilites.fr/marketplace/stop-monitoring?MonitoringRef=STIF:StopPoint:Q:{stop_id.split(':')[-1]}:"
-        data = (await self.__request(d))["MonitoredStopVisit"]
+
+        # for backward compatibility where only the stoppoint id is specified
+        if stop_id[0:4] != "STIF":
+            stop_id = f"STIF:StopPoint:Q:{stop_id}:"
+        
+        line = f"&LineRef=STIF:Line::{line_id}:" if line_id is not None else ""
+        request = f"https://prim.iledefrance-mobilites.fr/marketplace/stop-monitoring?MonitoringRef={stop_id}"
+        try:
+            response = await self.__request(request+line)
+        except UnknownIdentifierException:
+            # if the MonitoringRef/LineRef couple does not exists, fallback to use only the MonitoringRef
+            _LOGGER.debug("unknown MonitoringRef/LineRef coupe, falling back to only MonitoringRef")
+            response = await self.__request(request)
+        
         ret = []
-        for i in data:
+        for i in response["MonitoredStopVisit"]:
             d = TrafficData.from_json(i)
             if d and (direction_name is None or d.direction == direction_name) and (destination_name is None or d.destination_name == destination_name):
                 ret.append(d)
         return sorted(ret)
 
-    async def get_destinations(self, stop_id: str, direction_name: Optional[str] = None) -> List[str]:
+    async def get_destinations(self, stop_id: str, direction_name: Optional[str] = None, line_id: Optional[str] = None) -> List[str]:
         """
         Returns the available destinations for a specified line
 
         Args:
             stop_id: A string indicating the id of the depart stop area
             direction_name: The direction of a train
+            line_id: A string indicating id of a line (if not specified, all schedules for this stop/direction will be returned regardless of the line)
         Returns:
             A list of string representing the stations names
         """
         ret = set()
-        for i in await self.get_traffic(stop_id, direction_name=direction_name):
+        for i in await self.get_traffic(stop_id, direction_name=direction_name, line_id=line_id):
             ret.add(i.destination_name)
         return list(ret)
 
     async def get_directions(self, stop_id: str) -> List[str]:
         """
         Returns the available directions for a specified line
 
@@ -155,7 +175,13 @@
         ret = []
         with importlib.resources.open_text("idfm_api", "lines.json", encoding="utf8") as f:
             data = json.load(f)
             if transport.value in data:
                 for name, id in data[transport.value].items():
                     ret.append(LineData(name=name, id=id, type=transport))
         return ret
+
+class UnknownIdentifierException(Exception):
+    """
+    Exception raised when the identifier (MonitoringRef/LineRef) is unknown
+    """
+    pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `idfm_api-1.1.1/idfm_api/attribution.py` & `idfm_api-1.2.0/idfm_api/attribution.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 IDFM_DB_LICENCE = "Licence ODbL Version Française"
 IDFM_DB_LICENCE_LINK = "http://vvlibri.org/fr/licence/odbl-10/legalcode/unofficial"
 IDFM_DB_SOURCES = {
     "Arrêts et lignes associées": "https://data.iledefrance-mobilites.fr/explore/dataset/arrets-lignes",
-    "Référentiel des lignes de transport en commun d’île-de-France": "https://data.iledefrance-mobilites.fr/explore/dataset/referentiel-des-lignes",
-    "Référentiel des arrêts : Relations": "https://data.iledefrance-mobilites.fr/explore/dataset/relations"
+    "Référentiel des lignes de transport en commun d'île-de-France": "https://data.iledefrance-mobilites.fr/explore/dataset/referentiel-des-lignes",
+    "Référentiel des arrêts : Relations": "https://data.iledefrance-mobilites.fr/explore/dataset/relations",
+    "Référentiel des arrêts : Zones de correspondance": "https://data.iledefrance-mobilites.fr/explore/dataset/zones-de-correspondance"
 }
 IDFM_API_LICENCE = "Licence Mobilité"
 IDFM_API_LICENCE_LINK = "https://cloud.fabmob.io/s/eYWWJBdM3fQiFNm"
 IDFM_API_LINK = "https://prim.iledefrance-mobilites.fr/fr/donnees-dynamiques/idfm-ivtr-requete_unitaire"
```

### Comparing `idfm_api-1.1.1/idfm_api/lines.json` & `idfm_api-1.2.0/idfm_api/lines.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9289942252165545%*

 * *Differences: {"'bus'": "{'6 / Keolis Seine et Oise Est': 'C02568', '13 / Keolis Seine et Oise Est': 'C02570', "*

 * *          "'33 / Keolis Seine et Oise Est': 'C00116', '7 / Keolis Seine et Oise Est': 'C02569', "*

 * *          "'10 / Keolis Seine et Oise Est': 'C00286', '51 / Keolis Seine et Oise Est': 'C02547', "*

 * *          "'20 / Keolis Seine et Oise Est': 'C00272', '1 / Transdev CEAT': 'C00552', '3 / Transdev "*

 * *          'CEAT\': \'C00554\', "A / Keolis Val d\'Yerres Val de Seine": \'C00580\', \'2 / Keolis '*

 * *          "Seine […]*

```diff
@@ -20,47 +20,45 @@
         "04 / Transdev Ile-de-France Rambouillet": "C00165",
         "04 / Transdev Marne-la-Vall\u00e9e": "C00622",
         "04 / Transdev Senart": "C00844",
         "05 / Transdev Ile-de-France Conflans": "C01475",
         "05 / Transdev Ile-de-France Rambouillet": "C00166",
         "05 / Transdev Senart": "C00842",
         "06 / Transdev Ile-de-France Nanterre": "C01489",
-        "06 / Transdev Ile-de-France St-Fargeau-Ponthierry": "C00803",
         "06 / Transdev Marne-la-Vall\u00e9e": "C00903",
         "07 / Transdev Marne-la-Vall\u00e9e": "C00619",
         "08 / Transdev Ile-de-France Rambouillet": "C00168",
         "09 / Transdev Ile-de-France St-Fargeau-Ponthierry": "C02156",
         "09A / Transdev Brie et 2 Morin": "C02116",
         "09B / Transdev Brie et 2 Morin": "C02117",
         "09C / Transdev Brie et 2 Morin": "C02118",
-        "1 / CIF": "C00189",
+        "1 (future 401) / RD Bi\u00e8vre": "C00339",
         "1 / Cars Moreau": "C01456",
         "1 / Francilit\u00e9 Ouest Essonne": "C00975",
         "1 / Keolis Argenteuil Boucles de Seine": "C00292",
-        "1 / Keolis Seine et Oise Est": "C00641",
+        "1 / Keolis Seine et Oise Est": "C02565",
         "1 / Keolis Versailles": "C00692",
         "1 / Mobicit\u00e9": "C01826",
-        "1 / RD Bi\u00e8vre": "C00339",
         "1 / RD Mantois": "C00725",
         "1 / RD Saclay": "C00074",
         "1 / STBC": "C01423",
-        "1 / Transdev CEAT": "C00086",
+        "1 / Transdev CEAT": "C00552",
         "1 / Transdev CSO": "C02313",
         "1 / Transdev Ile-de-France Nemours": "C00832",
         "1 / Transdev Ile-de-France Vulaines": "C00793",
+        "1 / Transdev Nord Seine-Saint-Denis": "C00189",
         "1-1 / ProCars": "C01501",
         "1-2 / ProCars": "C02432",
         "1-3 / ProCars": "C02433",
-        "10 / Cars Hourtoule": "C00403",
-        "10 / Keolis Seine et Oise Est": "C00269",
+        "10 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00403",
+        "10 / Keolis Portes et Val de Brie": "C00014",
+        "10 / Keolis Seine et Oise Est": "C00286",
         "10 / Keolis Versailles": "C00701",
-        "10 / N4 Mobilit\u00e9s": "C00014",
         "10 / ProCars": "C01724",
         "10 / RD Saclay": "C00490",
-        "10 / SETRA": "C02124",
         "10 / Transdev Boucle des Lys": "C00149",
         "10 / Transdev Brie et 2 Morin": "C01040",
         "10 / Transdev CEAT": "C00547",
         "10 / Transdev Ile-de-France Nemours": "C00823",
         "10 / Transdev Ile-de-France Rambouillet": "C00170",
         "10 / Transdev Marne-et-Ourcq": "C00908",
         "10 / Transdev Valmy": "C00299",
@@ -83,104 +81,101 @@
         "105A / Transdev CEAT": "C02418",
         "105B / Transdev CEAT": "C02419",
         "106 / Keolis Versailles": "C00709",
         "106 / RATP": "C01135",
         "107 / Keolis Versailles": "C00710",
         "107 / RATP": "C01136",
         "107 / Transdev CEAT": "C00090",
-        "108 (ex 36) / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00040",
+        "108 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00040",
         "108 / RATP": "C01137",
         "108 / Transdev CEAT": "C01810",
-        "109 (ex 39-40 A) / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01690",
+        "109 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01690",
         "109 / RATP": "C01138",
         "109 / RD Mantois": "C00751",
         "109 / Transdev CEAT": "C01663",
         "11 / CIF": "C00191",
         "11 / Cars Hourtoule": "C00408",
-        "11 / Keolis Seine et Oise Est": "C00270",
+        "11 / Keolis Portes et Val de Brie": "C00015",
+        "11 / Keolis Seine et Oise Est": "C00111",
         "11 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00702",
-        "11 / N4 Mobilit\u00e9s": "C00015",
         "11 / ProCars": "C01507",
         "11 / RD Saclay": "C00495",
         "11 / Transdev Ile-de-France Conflans": "C01477",
         "11 / Transdev Ile-de-France Rambouillet": "C00171",
         "11 / Transdev Marne-et-Ourcq": "C00909",
         "11 / Transdev Senart": "C00845",
-        "11 / Transdev Vall\u00e9e Sud": "C00347",
         "11 / Transdev Valmy": "C00304",
         "11.5 / CIF": "C02165",
-        "110 (ex 39-40 B) / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01691",
+        "110 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01691",
         "110 / RATP": "C01139",
         "110 / RD Mantois": "C00752",
-        "111 (ex 39-40 C) / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01692",
         "111 / Cars Hourtoule": "C00420",
+        "111 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01692",
         "111 / RATP": "C01140",
         "111 / Transdev Ile-de-France Vulaines": "C02202",
-        "112 (ex 39-40 D) / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01693",
+        "112 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01693",
         "112 / RATP": "C01141",
         "112 / Transdev Ile-de-France Vulaines": "C00797",
-        "113 (ex 39-39 A) / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00527",
+        "113 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00527",
         "113 / RATP": "C01142",
         "113 / Transdev Ile-de-France St-Fargeau-Ponthierry": "C02289",
-        "114 (ex 39-39 B) / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01689",
+        "114 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01689",
         "114 / RATP": "C01143",
         "114 / RD Saclay": "C00093",
         "114 / Transdev Ile-de-France St-Fargeau-Ponthierry": "C02290",
-        "115 (ex 22 scolaire) / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C02478",
+        "115 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C02478",
         "115 / RATP": "C01144",
         "115 / Transdev Ile-de-France St-Fargeau-Ponthierry": "C02287",
-        "116 (ex 35) / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00039",
         "116 / CIF": "C00225",
+        "116 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00039",
         "116 / RATP": "C01145",
         "116 / RD Saclay": "C01766",
-        "117 (ex 39.37 A) / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00525",
+        "117 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00525",
         "117 / RATP": "C01146",
-        "118 (ex 39-37 B) / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01688",
+        "118 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01688",
         "118 / RATP": "C01147",
         "119 / RATP": "C01148",
         "11A / Transdev Ile-de-France Nemours": "C00824",
         "11B / Transdev Ile-de-France Nemours": "C01965",
         "11C / Transdev Ile-de-France Nemours": "C01966",
         "11D / Transdev Ile-de-France Nemours": "C01967",
+        "12 (future 412) / RD Bi\u00e8vre": "C00348",
         "12 / CIF": "C00194",
         "12 / Cars Hourtoule": "C00409",
         "12 / Keolis Argenteuil Boucles de Seine": "C01478",
-        "12 / Keolis Seine et Oise Est": "C00654",
+        "12 / Keolis Seine et Oise Est": "C00274",
         "12 / Keolis Val d'Yerres Val de Seine": "C00369",
         "12 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00703",
         "12 / ProCars": "C01508",
-        "12 / RD Bi\u00e8vre": "C00348",
         "12 / RD Saclay": "C00503",
-        "12 / SETRA": "C00548",
         "12 / TVF": "C01777",
         "12 / Transdev Brie et 2 Morin": "C00910",
         "12 / Transdev Ile-de-France Nemours": "C02031",
         "12 / Transdev Ile-de-France Rambouillet": "C01951",
         "12 / Transdev Marne-la-Vall\u00e9e": "C00620",
         "12 / Transdev Senart": "C00846",
         "12 / Transdev Valmy": "C00301",
         "12.1 / CIF": "C02167",
         "120 / RATP": "C01149",
-        "121 / N4 Mobilit\u00e9s": "C00020",
+        "121 / Keolis Portes et Val de Brie": "C00020",
         "121 / RATP": "C01150",
         "122 / RATP": "C01151",
         "123 / RATP": "C01152",
         "124 / RATP": "C01153",
         "125 / RATP": "C01154",
         "126 / RATP": "C01155",
         "127 / RATP": "C01156",
         "128 / RATP": "C01157",
         "129 / RATP": "C01158",
         "12A / Transdev Brie et 2 Morin": "C02072",
         "12B / Transdev Brie et 2 Morin": "C02073",
         "12C / Transdev Brie et 2 Morin": "C02074",
         "12ZI / CIF": "C02166",
-        "13 / Keolis Seine et Oise Est": "C00111",
+        "13 / Keolis Seine et Oise Est": "C02570",
         "13 / Keolis Val d'Yerres Val de Seine": "C00370",
-        "13 / Keolis Versailles": "C00704",
         "13 / ProCars": "C01509",
         "13 / RD Saclay": "C00520",
         "13 / Transdev Ile-de-France Houdan": "C00060",
         "13 / Transdev Marne-la-Vall\u00e9e": "C00621",
         "13 / Transdev Senart": "C00847",
         "13 / Transdev Valmy": "C00302",
         "131 / RATP": "C01159",
@@ -193,18 +188,18 @@
         "13A / Transdev Ile-de-France Nemours": "C00826",
         "13B / Transdev Brie et 2 Morin": "C01716",
         "13B / Transdev Ile-de-France Nemours": "C01969",
         "13C / Transdev Ile-de-France Nemours": "C01970",
         "14 / CIF": "C00196",
         "14 / Cars Hourtoule": "C00410",
         "14 / Darche Gros": "C01043",
-        "14 / Keolis Seine et Oise Est": "C00271",
+        "14 / Keolis Portes et Val de Brie": "C00016",
+        "14 / Keolis Seine et Oise Est": "C02571",
         "14 / Keolis Val d'Yerres Val de Seine": "C00371",
         "14 / Keolis Versailles": "C02286",
-        "14 / N4 Mobilit\u00e9s": "C00016",
         "14 / ProCars": "C01510",
         "14 / RD Saclay": "C00075",
         "14 / Transdev Ile-de-France Conflans": "C01479",
         "14 / Transdev Ile-de-France Ecquevilly": "C00112",
         "14 / Transdev Ile-de-France St-Fargeau-Ponthierry": "C02277",
         "14 / Transdev Marne-la-Vall\u00e9e": "C00911",
         "14 / Transdev Vall\u00e9e Sud": "C00350",
@@ -216,62 +211,61 @@
         "144 / RATP": "C01169",
         "145 / RATP": "C01170",
         "146 / RATP": "C01171",
         "147 / RATP": "C01172",
         "148 / RATP": "C01173",
         "14A / Transdev Ile-de-France Nemours": "C00827",
         "14B / Transdev Ile-de-France Nemours": "C01971",
-        "15 / CIF": "C00197",
+        "15 (future 415) / RD Bi\u00e8vre": "C01658",
         "15 / Cars Hourtoule": "C00411",
+        "15 / Keolis Seine et Oise Est": "C02537",
         "15 / ProCars": "C01511",
-        "15 / RD Bi\u00e8vre": "C01658",
         "15 / RD Mantois": "C00733",
         "15 / RD Saclay": "C02155",
-        "15 / Transdev Boucle des Lys": "C00150",
         "15 / Transdev CEAT": "C00094",
         "15 / Transdev Ile-de-France Rambouillet": "C00172",
         "15 / Transdev Marne-la-Vall\u00e9e": "C00623",
+        "15 / Transdev Nord Seine-Saint-Denis": "C00197",
         "15 / Transdev Valmy": "C01804",
         "150 / RATP": "C01174",
         "151 / RATP": "C01175",
         "152 / RATP": "C01176",
         "153 / RATP": "C01177",
         "157 / RATP": "C01180",
         "158 / RATP": "C01181",
         "159 / RATP": "C01182",
         "16 / CIF": "C00198",
-        "16 / Keolis Seine et Oise Est": "C00272",
+        "16 / Keolis Seine et Oise Est": "C02539",
         "16 / Keolis Val d'Yerres Val de Seine": "C00376",
         "16 / ProCars": "C01512",
         "16 / RD Mantois": "C00734",
         "16 / RD Saclay": "C00078",
         "16 / Transdev Ile-de-France Rambouillet": "C01957",
-        "16 / Transdev Vall\u00e9e Sud": "C01655",
         "16 / Transdev Valmy": "C01802",
         "160 / RATP": "C01183",
         "162 / RATP": "C01184",
         "163 / RATP": "C01185",
         "164 / RATP": "C01186",
         "165 / RATP": "C01187",
         "166 / RATP": "C01188",
         "167 / RATP": "C01189",
         "168 / RATP": "C02007",
         "169 / RATP": "C01190",
         "17 / CIF": "C00199",
         "17 / Cars Hourtoule": "C00413",
         "17 / Keolis Argenteuil Boucles de Seine": "C01822",
+        "17 / Keolis Portes et Val de Brie": "C00624",
+        "17 / Keolis Seine et Oise Est": "C00649",
         "17 / Keolis Val d'Yerres Val de Seine": "C00378",
-        "17 / N4 Mobilit\u00e9s": "C00624",
         "17 / ProCars": "C01725",
         "17 / RD Mantois": "C00735",
         "17 / RD Saclay": "C00680",
         "17 / TVF": "C00658",
         "17 / Transdev Ile-de-France Ecquevilly": "C00113",
         "17 / Transdev Ile-de-France Houdan": "C01992",
-        "17 / Transdev Vall\u00e9e Sud": "C01656",
         "17 / Transdev Valmy": "C02462",
         "170 / RATP": "C01191",
         "170 / Transdev Ile-de-France Ecquevilly": "C00124",
         "171 / CIF": "C01779",
         "171 / RATP": "C01192",
         "171 / Transdev Ile-de-France Ecquevilly": "C00125",
         "172 / RATP": "C01193",
@@ -285,20 +279,20 @@
         "178 / RATP": "C01199",
         "179 / RATP": "C01200",
         "17A / Transdev Ile-de-France Conflans": "C01480",
         "17A / Transdev Ile-de-France Nemours": "C00830",
         "17B / Transdev Ile-de-France Conflans": "C02197",
         "17B / Transdev Ile-de-France Nemours": "C01973",
         "17S / Transdev Ile-de-France Ecquevilly": "C02446",
+        "18 (future 418) / RD Bi\u00e8vre": "C01657",
         "18 / CIF": "C00200",
         "18 / Keolis Argenteuil Boucles de Seine": "C00303",
-        "18 / Keolis Seine et Oise Est": "C02441",
+        "18 / Keolis Portes et Val de Brie": "C00017",
+        "18 / Keolis Seine et Oise Est": "C00651",
         "18 / Keolis Val d'Yerres Val de Seine": "C00372",
-        "18 / N4 Mobilit\u00e9s": "C00017",
-        "18 / RD Bi\u00e8vre": "C01657",
         "18 / RD Mantois": "C00736",
         "18 / RD Saclay": "C02355",
         "18 / TVF": "C00659",
         "18 / Transdev Brie et 2 Morin": "C00913",
         "18 / Transdev Ile-de-France Rambouillet": "C00173",
         "180 / RATP": "C01201",
         "181 / RATP": "C01202",
@@ -321,15 +315,15 @@
         "18A / Transdev Ile-de-France Nemours": "C00831",
         "18B / Transdev Ile-de-France Nemours": "C01974",
         "18C / Transdev Ile-de-France Nemours": "C02032",
         "18s / Transdev Boucle des Lys": "C00153",
         "19 / CIF": "C00201",
         "19 / Cars Hourtoule": "C00415",
         "19 / INTERVAL": "C01451",
-        "19 / Keolis Seine et Oise Est": "C00114",
+        "19 / Keolis Seine et Oise Est": "C02540",
         "19 / Keolis Val d'Yerres Val de Seine": "C00373",
         "19 / RD Mantois": "C00737",
         "19 / RD Saclay": "C00079",
         "19 / TVF": "C00660",
         "19 / Transdev Ile-de-France Rambouillet": "C00174",
         "19 / Transdev Marne-et-Ourcq": "C00914",
         "190 / RATP": "C01211",
@@ -337,45 +331,45 @@
         "192 / RATP": "C01213",
         "193 / RATP": "C02288",
         "194 / RATP": "C01214",
         "195 / RATP": "C01215",
         "196 / RATP": "C01216",
         "197 / RATP": "C01217",
         "199 / RATP": "C01218",
+        "2 (future 402) / RD Bi\u00e8vre": "C00340",
         "2 / Cars Moreau": "C01464",
         "2 / Francilit\u00e9 Ouest Essonne": "C00976",
-        "2 / Keolis Argenteuil Boucles de Seine": "C00294",
-        "2 / Keolis Seine et Oise Est": "C00132",
+        "2 / Keolis Argenteuil Boucles de Seine": "C01473",
+        "2 / Keolis Seine et Oise Est": "C02566",
         "2 / Keolis Val d'Oise": "C00603",
         "2 / Keolis Versailles": "C00693",
         "2 / Mobicit\u00e9": "C01827",
         "2 / ProCars": "C01722",
-        "2 / RD Bi\u00e8vre": "C00340",
         "2 / RD Saclay": "C00067",
         "2 / STBC": "C01426",
         "2 / Transdev CEAT": "C00087",
         "2 / Transdev CSO": "C02481",
         "2 / Transdev Ile-de-France Houdan": "C00054",
         "2 / Transdev Ile-de-France Nemours": "C00833",
         "2 / Transdev Ile-de-France Vulaines": "C00795",
-        "20 / Cars Hourtoule": "C00416",
-        "20 / Darche Gros": "C01044",
+        "20 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00416",
         "20 / Keolis Argenteuil Boucles de Seine": "C02264",
-        "20 / Keolis Seine et Oise Est": "C00274",
+        "20 / Keolis Portes et Val de Brie": "C01044",
+        "20 / Keolis Seine et Oise Est": "C00272",
         "20 / RATP": "C01072",
         "20 / RD Mantois": "C00738",
         "20 / RD Saclay": "C00066",
         "20 / Trans Val d'Oise": "C01867",
         "20 / Transdev Ile-de-France Rambouillet": "C00175",
         "20 / Transdev Ile-de-France St-Fargeau-Ponthierry": "C02278",
         "20 / Transdev Marne-la-Vall\u00e9e": "C02455",
-        "200 / N4 Mobilit\u00e9s": "C02311",
+        "200 / Keolis Portes et Val de Brie": "C02311",
         "201 / Cars Moreau": "C01461",
+        "201 / Keolis Portes et Val de Brie": "C00021",
         "201 / Keolis Val d'Essonne Deux Vall\u00e9es": "C00319",
-        "201 / N4 Mobilit\u00e9s": "C00021",
         "201 / RATP": "C01219",
         "202 / Cars Moreau": "C01462",
         "202 / Transdev CEAT": "C00323",
         "202 / Transdev Ile-de-France Nemours": "C00817",
         "203 / Cars Moreau": "C01463",
         "203 / INTERVAL": "C01450",
         "203 / Keolis Val d'Essonne Deux Vall\u00e9es": "C00322",
@@ -392,25 +386,24 @@
         "207 / RATP": "C01222",
         "207 / Transdev Ile-de-France Nemours": "C00828",
         "208 / INTERVAL": "C01444",
         "208 / Keolis Val d'Essonne Deux Vall\u00e9es": "C02021",
         "208A / RATP": "C01223",
         "208B / RATP": "C01818",
         "208S / RATP": "C01819",
+        "209 / Keolis Portes et Val de Brie": "C00024",
         "209 / Keolis Val d'Essonne Deux Vall\u00e9es": "C02221",
-        "209 / N4 Mobilit\u00e9s": "C00024",
         "209 / RATP": "C02437",
         "209 / Transdev Ile-de-France Vulaines": "C00799",
         "21 / CIF": "C00202",
-        "21 / Keolis Seine et Oise Est": "C00275",
-        "21 / N4 Mobilit\u00e9s": "C00018",
+        "21 / Keolis Portes et Val de Brie": "C00018",
+        "21 / Keolis Seine et Oise Est": "C00106",
         "21 / RATP": "C01073",
         "21 / RD Mantois": "C00739",
         "21 / RD Saclay": "C01697",
-        "21 / SETRA": "C00550",
         "21 / Transdev Boucle des Lys": "C00154",
         "21 / Transdev CEAT": "C02426",
         "21 / Transdev Ile-de-France Houdan": "C01980",
         "21 / Transdev Ile-de-France St-Fargeau-Ponthierry": "C02159",
         "21 / Transdev Marne-et-Ourcq": "C00916",
         "21 / Transdev Marne-la-Vall\u00e9e": "C00625",
         "21 / Transdev Senart": "C00862",
@@ -425,15 +418,15 @@
         "215 / RATP": "C01229",
         "216 / RATP": "C01230",
         "217 / RATP": "C01231",
         "21S / Transdev Marne-et-Ourcq": "C01994",
         "21s / Transdev Boucle des Lys": "C02307",
         "22 / CIF": "C00203",
         "22 / Francilit\u00e9 Ouest Essonne": "C00176",
-        "22 / Keolis Seine et Oise Est": "C00643",
+        "22 / Keolis Seine et Oise Est": "C00107",
         "22 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00052",
         "22 / RATP": "C01074",
         "22 / RD Mantois": "C00740",
         "22 / RD Saclay": "C01698",
         "22 / Trans Val d'Oise": "C00609",
         "22 / Transdev CEAT": "C02427",
         "22 / Transdev Ile-de-France Houdan": "C01981",
@@ -453,18 +446,18 @@
         "2272 / Orgebus": "C01950",
         "2273 / Orgebus": "C01498",
         "2274 / Orgebus": "C01497",
         "2276 / Orgebus": "C01496",
         "228 / Keolis Val d'Essonne Deux Vall\u00e9es": "C02023",
         "229 / Keolis Val d'Essonne Deux Vall\u00e9es": "C02024",
         "23 / CIF": "C00204",
+        "23 / Keolis Portes et Val de Brie": "C00551",
+        "23 / Keolis Seine et Oise Est": "C02441",
         "23 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00050",
-        "23 / N4 Mobilit\u00e9s": "C00019",
         "23 / RD Saclay": "C01699",
-        "23 / SETRA": "C00551",
         "23 / Trans Val d'Oise": "C00610",
         "23 / Transdev CSO": "C00276",
         "23 / Transdev Ile-de-France Rambouillet": "C00187",
         "23 / Transdev Ile-de-France St-Fargeau-Ponthierry": "C02279",
         "23 / Transdev Marne-et-Ourcq": "C00919",
         "23 / Transdev Marne-la-Vall\u00e9e": "C00627",
         "23 / Transdev Senart": "C00867",
@@ -473,31 +466,31 @@
         "232 / Keolis Val d'Essonne Deux Vall\u00e9es": "C02387",
         "234 / RATP": "C01234",
         "235 / RATP": "C01235",
         "237 / RATP": "C01236",
         "238 / RATP": "C01237",
         "239 / RATP": "C01238",
         "24 / CIF": "C01866",
-        "24 / Darche Gros": "C01045",
-        "24 / Keolis Seine et Oise Est": "C00277",
+        "24 / Keolis Portes et Val de Brie": "C01045",
+        "24 / Keolis Seine et Oise Est": "C00285",
         "24 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00043",
         "24 / RATP": "C01075",
         "24 / Trans Val d'Oise": "C00612",
         "24 / Transdev Ile-de-France Rambouillet": "C00177",
         "24 / Transdev Marne-la-Vall\u00e9e": "C00638",
         "24 / Transdev Senart": "C00865",
         "24 sco / Trans Val d'Oise": "C00613",
         "24-06 / Keolis Seine Essonne": "C00380",
         "24-10 / Keolis Val d'Essonne Deux Vall\u00e9es": "C00382",
         "241 / RATP": "C01239",
         "244 / RATP": "C01240",
         "247 / RATP": "C01695",
         "248 / RATP": "C01696",
         "249 / RATP": "C01241",
-        "25 / Keolis Seine et Oise Est": "C00278",
+        "25 / Keolis Seine et Oise Est": "C02541",
         "25 / RATP": "C02243",
         "25 / Trans Val d'Oise": "C00611",
         "25 / Transdev Brie et 2 Morin": "C01046",
         "25 / Transdev Ile-de-France Rambouillet": "C00178",
         "25 / Transdev Marne-la-Vall\u00e9e": "C00628",
         "25 / Transdev Senart": "C00864",
         "250 / RATP": "C01242",
@@ -505,15 +498,15 @@
         "252 / RATP": "C01244",
         "253 / RATP": "C01245",
         "254 / RATP": "C01808",
         "255 / RATP": "C01246",
         "256 / RATP": "C01247",
         "258 / RATP": "C01248",
         "259 / RATP": "C02000",
-        "26 / Keolis Seine et Oise Est": "C00644",
+        "26 / Keolis Seine et Oise Est": "C00117",
         "26 / RATP": "C01076",
         "26 / RD Mantois": "C00741",
         "26 / Transdev Brie et 2 Morin": "C01047",
         "26 / Transdev Ile-de-France Rambouillet": "C00179",
         "26 / Transdev Marne-la-Vall\u00e9e": "C00629",
         "26 / Transdev Senart": "C00866",
         "260 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01799",
@@ -524,46 +517,47 @@
         "262 / RATP": "C01250",
         "263 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00530",
         "263 / RATP": "C02314",
         "264 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01700",
         "268 / RATP": "C01251",
         "269 / RATP": "C01252",
         "27 / Keolis Mobilit\u00e9 Roissy": "C02059",
+        "27 / Keolis Seine et Oise Est": "C00641",
         "27 / RATP": "C01077",
         "27 / Transdev Brie et 2 Morin": "C01048",
         "27 / Transdev CSO": "C00279",
         "27 / Transdev Ile-de-France Nanterre": "C01482",
         "27 / Transdev Marne-la-Vall\u00e9e": "C02298",
         "27 / Transdev Senart": "C02458",
         "27 / Transdev Valmy": "C02463",
         "270 / RATP": "C01253",
         "272 / RATP": "C01254",
         "274 / RATP": "C01255",
         "275 / RATP": "C01256",
         "276 / RATP": "C01257",
         "278 / RATP": "C01258",
-        "28 / Keolis Seine et Oise Est": "C00280",
+        "28 / Keolis Seine et Oise Est": "C00642",
         "28 / RATP": "C01078",
         "28 / Transdev Ile-de-France Ecquevilly": "C02444",
         "28 / Transdev Ile-de-France Nanterre": "C01483",
         "281 / RATP": "C01260",
         "282 / Keolis Ouest Val-de-Marne": "C00007",
         "284-001 / Keolis Val d'Essonne Deux Vall\u00e9es": "C01013",
         "284-002 / Keolis Val d'Essonne Deux Vall\u00e9es": "C01014",
         "284-003 / Keolis Val d'Essonne Deux Vall\u00e9es": "C01015",
         "284-004 / Keolis Val d'Essonne Deux Vall\u00e9es": "C01016",
         "284-005 / Keolis Val d'Essonne Deux Vall\u00e9es": "C02393",
         "284-006 / Keolis Val d'Essonne Deux Vall\u00e9es": "C01017",
         "285 / RATP": "C01262",
         "286 / RATP": "C01263",
         "289 / RATP": "C01264",
-        "28A / Darche Gros": "C02089",
-        "28B / Darche Gros": "C02090",
-        "28C / Darche Gros": "C02091",
-        "29 / Keolis Seine et Oise Est": "C02222",
+        "28A / Keolis Portes et Val de Brie": "C02089",
+        "28B / Keolis Portes et Val de Brie": "C02090",
+        "28C / Keolis Portes et Val de Brie": "C02091",
+        "29 / Keolis Seine et Oise Est": "C02542",
         "29 / RATP": "C01079",
         "29 / Stivo": "C02141",
         "29 / Transdev Ile-de-France Nanterre": "C01484",
         "29 / Transdev Ile-de-France Rambouillet": "C00180",
         "29 / Transdev Marne-la-Vall\u00e9e": "C00630",
         "290 / RATP": "C01265",
         "291 / RATP": "C01266",
@@ -576,26 +570,26 @@
         "29M / Transdev Brie et 2 Morin": "C02196",
         "2A / RD Mantois": "C01797",
         "2B / RD Mantois": "C01796",
         "2C / RD Mantois": "C01798",
         "3 / Cars Moreau": "C01664",
         "3 / Francilit\u00e9 Ouest Essonne": "C00982",
         "3 / Keolis Argenteuil Boucles de Seine": "C01681",
-        "3 / Keolis Seine et Oise Est": "C00133",
+        "3 / Keolis Portes et Val de Brie": "C00009",
+        "3 / Keolis Seine et Oise Est": "C00281",
         "3 / Keolis Versailles": "C00694",
         "3 / Mobicit\u00e9": "C01828",
-        "3 / N4 Mobilit\u00e9s": "C00009",
         "3 / ProCars": "C01502",
         "3 / RD Saclay": "C00068",
         "3 / STBC": "C02129",
-        "3 / Transdev CEAT": "C00088",
+        "3 / Transdev CEAT": "C00554",
         "3 / Transdev Ile-de-France Nemours": "C00819",
         "3 / Transdev Ile-de-France Vulaines": "C00796",
         "3 / Transdev Vall\u00e9e Sud": "C00341",
-        "30 / Keolis Seine et Oise Est": "C00645",
+        "30 / Keolis Seine et Oise Est": "C01937",
         "30 / RATP": "C01080",
         "30 / Stivo": "C00762",
         "30 / Transdev Ile-de-France Nanterre": "C01772",
         "30 / Transdev Ile-de-France Rambouillet": "C00181",
         "30-03 / Cars Lacroix": "C02005",
         "30-04 Scolaire / Cars Lacroix": "C00436",
         "30-05 / Cars Lacroix": "C00437",
@@ -608,15 +602,14 @@
         "30-14 / Cars Lacroix": "C00447",
         "30-18 / Cars Lacroix": "C00448",
         "30-21 Est / Cars Lacroix": "C02389",
         "30-21 Ouest / Cars Lacroix": "C02049",
         "30-22 / Cars Lacroix": "C00451",
         "30-23 / Cars Lacroix": "C00452",
         "30-25 Scolaire / Cars Lacroix": "C00453",
-        "30-27 / Keolis Seine et Oise Est": "C00454",
         "30-28 Scolaire / Cars Lacroix": "C00455",
         "30-29 Scolaire / Cars Lacroix": "C00456",
         "30-31 Scolaire / Cars Lacroix": "C00458",
         "30-32 Scolaire / Cars Lacroix": "C00459",
         "30-33 Scolaire / Cars Lacroix": "C00460",
         "30-34 Scolaire / Cars Lacroix": "C00461",
         "30-36 / Cars Lacroix": "C00462",
@@ -639,50 +632,48 @@
         "304 / Keolis Seine Essonne": "C00390",
         "304 / RATP": "C01275",
         "305 / Keolis Seine Essonne": "C00392",
         "306 / RATP": "C01276",
         "306.04 / Francilit\u00e9 Ouest Essonne": "C00973",
         "306.12 / Francilit\u00e9 Ouest Essonne": "C00974",
         "308 / RATP": "C01277",
-        "309 / N4 Mobilit\u00e9s": "C00025",
-        "30A / Darche Gros": "C02121",
+        "309 / Keolis Portes et Val de Brie": "C00025",
+        "30A / Keolis Portes et Val de Brie": "C02121",
         "30B / CIF": "C00205",
-        "30B / Darche Gros": "C02120",
-        "30C / Darche Gros": "C02122",
+        "30B / Keolis Portes et Val de Brie": "C02120",
+        "30C / Keolis Portes et Val de Brie": "C02122",
         "30D / CIF": "C00206",
         "31 / CIF": "C00208",
-        "31 / Keolis Seine et Oise Est": "C00646",
+        "31 / Keolis Seine et Oise Est": "C00267",
         "31 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01687",
         "31 / RATP": "C01081",
         "31 / Transdev Brie et 2 Morin": "C00920",
         "31 / Transdev Ile-de-France Houdan": "C01982",
         "31 / Transdev Senart": "C01669",
         "310 / RATP": "C01278",
-        "311 / Keolis Seine et Oise Est": "C00128",
+        "311 / RATP": "C02538",
         "312 / Keolis Seine Essonne": "C00387",
-        "312 / Keolis Seine et Oise Est": "C00129",
         "312 / RATP": "C01279",
         "313 / Keolis Seine Essonne": "C00389",
-        "313 / Keolis Seine et Oise Est": "C00130",
         "314 / Keolis Val d'Essonne Deux Vall\u00e9es": "C00391",
         "316 / Francilit\u00e9 Ouest Essonne": "C02066",
         "317 / Francilit\u00e9 Ouest Essonne": "C02067",
         "317 / RATP": "C01280",
         "318 / Francilit\u00e9 Ouest Essonne": "C02068",
         "318 / RATP": "C01281",
         "319 / Francilit\u00e9 Ouest Essonne": "C00097",
         "319 / RATP": "C01282",
         "31A / Transdev Brie et 2 Morin": "C02077",
         "31B / Transdev Brie et 2 Morin": "C02078",
         "31C / Transdev Brie et 2 Morin": "C02079",
         "31S / Transdev Brie et 2 Morin": "C00921",
         "32 / CIF": "C00209",
-        "32 / Darche Gros": "C01052",
         "32 / Keolis Mobilit\u00e9 Roissy": "C02061",
-        "32 / Keolis Seine et Oise Est": "C00647",
+        "32 / Keolis Portes et Val de Brie": "C01052",
+        "32 / Keolis Seine et Oise Est": "C00280",
         "32 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00038",
         "32 / RATP": "C01082",
         "32 / Transdev Brie et 2 Morin": "C00922",
         "32 / Transdev Marne-la-Vall\u00e9e": "C00631",
         "32 / Transdev Senart": "C00868",
         "320 / Francilit\u00e9 Ouest Essonne": "C01975",
         "320 / RATP": "C01283",
@@ -695,84 +686,83 @@
         "324 / Francilit\u00e9 Ouest Essonne": "C02270",
         "325 / Francilit\u00e9 Ouest Essonne": "C02271",
         "325 / RATP": "C01288",
         "32A / CIF": "C00210",
         "32S / Transdev Brie et 2 Morin": "C02160",
         "32ZA / CIF": "C01815",
         "33 / CIF": "C00211",
-        "33 / Darche Gros": "C01053",
-        "33 / Keolis Seine et Oise Est": "C00117",
+        "33 / Keolis Portes et Val de Brie": "C01053",
+        "33 / Keolis Seine et Oise Est": "C00116",
         "33 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00042",
         "33 / Stivo": "C02085",
         "33 / Transdev Brie et 2 Morin": "C00923",
         "33 / Transdev Senart": "C00871",
         "33 SoisyBus / Transdev Valmy": "C00305",
         "330 / Francilit\u00e9 Ouest Essonne": "C00105",
         "330 / RATP": "C01289",
         "331 / Francilit\u00e9 Ouest Essonne": "C00098",
         "332 / Francilit\u00e9 Ouest Essonne": "C02431",
         "337 / RATP": "C01756",
         "34 / CIF": "C02164",
         "34 / Keolis Argenteuil Boucles de Seine": "C00306",
+        "34 / Keolis Seine et Oise Est": "C01773",
         "34 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C01805",
         "34 / RD Mantois": "C00118",
         "34 / Stivo": "C00763",
         "34 / Transdev Brie et 2 Morin": "C00924",
         "34 / Transdev Ile-de-France Nemours": "C00815",
         "34 / Transdev Marne-la-Vall\u00e9e": "C00632",
         "34 / Transdev Senart": "C00850",
         "340 / RATP": "C01292",
         "341 / RATP": "C01294",
         "346 / RATP": "C01295",
-        "349 / RATP": "C01297",
-        "34A / Darche Gros": "C02087",
-        "34B / Darche Gros": "C02088",
+        "349 / Transdev Nord Seine-Saint-Denis": "C01297",
+        "34A / Keolis Portes et Val de Brie": "C02087",
+        "34B / Keolis Portes et Val de Brie": "C02088",
         "34S1 / Transdev Brie et 2 Morin": "C00925",
         "34S2 / Transdev Brie et 2 Morin": "C02400",
         "34S3 / Transdev Brie et 2 Morin": "C02401",
-        "35 / Keolis Seine et Oise Est": "C00649",
         "35 / RATP": "C01680",
         "35 / Stivo": "C00764",
         "35 / Trans Val d'Oise": "C00615",
         "35 / Transdev Brie et 2 Morin": "C00926",
         "35 / Transdev Ile-de-France Houdan": "C01983",
         "35 / Transdev Marne-la-Vall\u00e9e": "C02015",
         "35 / Transdev Senart": "C00856",
         "350 / RATP": "C01298",
         "351 / RATP": "C01299",
         "353 / RATP": "C02008",
         "355 / RATP": "C01302",
         "356 / RATP": "C01303",
-        "35A / Darche Gros": "C02126",
-        "35B / Darche Gros": "C02125",
-        "35C / Darche Gros": "C02127",
-        "35D / Darche Gros": "C02128",
+        "35A / Keolis Portes et Val de Brie": "C02126",
+        "35B / Keolis Portes et Val de Brie": "C02125",
+        "35C / Keolis Portes et Val de Brie": "C02127",
+        "35D / Keolis Portes et Val de Brie": "C02128",
         "36 / Stivo": "C00765",
         "36 / Trans Val d'Oise": "C00616",
         "36 / Transdev Senart": "C00851",
-        "36-15 / Cars Perrier": "C00482",
+        "36-15 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00482",
         "360 / RATP": "C01304",
         "361 / RATP": "C01305",
         "366 / RATP": "C01306",
         "367 / RATP": "C01307",
         "368 / RATP": "C01308",
         "37 / Keolis Argenteuil Boucles de Seine": "C01491",
-        "37 / Keolis Seine et Oise Est": "C00650",
         "37 / Trans Val d'Oise": "C00617",
         "37 / Transdev Marne-la-Vall\u00e9e": "C00633",
         "37 / Transdev Senart": "C00852",
         "37 / Transdev Valmy": "C00307",
         "370 / RATP": "C01309",
         "372 / RATP": "C01310",
         "378 / RATP": "C01311",
         "379 / RATP": "C01312",
-        "37A / Darche Gros": "C02107",
-        "37B / Darche Gros": "C02108",
-        "37C / Darche Gros": "C02109",
-        "37RPI / Darche Gros": "C02110",
+        "37A / Keolis Portes et Val de Brie": "C02107",
+        "37B / Keolis Portes et Val de Brie": "C02108",
+        "37C / Keolis Portes et Val de Brie": "C02109",
+        "37R / Keolis Portes et Val de Brie": "C02110",
         "38 / CIF": "C00212",
         "38 / RATP": "C01083",
         "38 / Stivo": "C00766",
         "38 / Transdev Brie et 2 Morin": "C01057",
         "38 / Transdev Ile-de-France Ecquevilly": "C02443",
         "38 / Transdev Ile-de-France Houdan": "C01984",
         "38 / Transdev Ile-de-France Nanterre": "C01493",
@@ -781,20 +771,19 @@
         "380 / RATP": "C01809",
         "3801 / Cars Rose": "C00484",
         "3804 / Cars Rose": "C00487",
         "382 / RATP": "C02459",
         "385 / RATP": "C01313",
         "388 / RATP": "C01314",
         "389 / RATP": "C01315",
-        "39 / CIF": "C00213",
-        "39 / Darche Gros": "C01058",
-        "39 / Keolis Seine et Oise Est": "C00651",
+        "39 / Keolis Portes et Val de Brie": "C01058",
         "39 / RATP": "C01084",
         "39 / Stivo": "C00767",
         "39 / Transdev Ile-de-France Rambouillet": "C01952",
+        "39 / Transdev Nord Seine-Saint-Denis": "C00213",
         "39-003 / SAVAC": "C00489",
         "39-02 / SAVAC": "C00488",
         "39-07 / SAVAC": "C01721",
         "39-07 A / SAVAC": "C00494",
         "39-07 B / SAVAC": "C01718",
         "39-07 C / SAVAC": "C01719",
         "39-07 D / SAVAC": "C01720",
@@ -833,162 +822,167 @@
         "393 / RATP": "C01318",
         "394 / RATP": "C01319",
         "395 / RATP": "C01320",
         "396 / RATP": "C01321",
         "399 / RATP": "C01322",
         "3A / CIF": "C01801",
         "3s / STBC": "C02130",
+        "4 (future 412) / RD Bi\u00e8vre": "C00342",
         "4 / Keolis Argenteuil Boucles de Seine": "C00295",
-        "4 / Keolis Seine et Oise Est": "C00134",
+        "4 / Keolis Portes et Val de Brie": "C00010",
+        "4 / Keolis Seine et Oise Est": "C01784",
         "4 / Keolis Versailles": "C00695",
         "4 / Mobicit\u00e9": "C01829",
-        "4 / N4 Mobilit\u00e9s": "C00010",
-        "4 / RD Bi\u00e8vre": "C00342",
         "4 / RD Mantois": "C00728",
         "4 / RD Saclay": "C00069",
         "4 / STBC": "C02137",
-        "4 / Transdev CEAT": "C00555",
+        "4 / Transdev CEAT": "C00089",
         "4 / Transdev Ile-de-France Nemours": "C00834",
         "4 / Transdev Ile-de-France Vulaines": "C00794",
         "4 / Transdev Marne-et-Ourcq": "C00901",
-        "40 / CIF": "C02214",
         "40 / Keolis Argenteuil Boucles de Seine": "C01492",
+        "40 / Keolis Seine et Oise Est": "C00270",
         "40 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00048",
         "40 / RATP": "C02254",
         "40 / RD Mantois": "C01428",
         "40 / STAVO": "C01868",
         "40 / Stivo": "C00768",
         "40 / Transdev Brie et 2 Morin": "C01059",
         "40 / Transdev Ile-de-France Houdan": "C01985",
         "40 / Transdev Ile-de-France Vulaines": "C02258",
         "40 / Transdev Marne-et-Ourcq": "C00927",
-        "401 / SQYBUS": "C01521",
+        "40 / Transdev Nord Seine-Saint-Denis": "C02214",
+        "401 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01521",
         "401 / TICE": "C01616",
-        "402 / SQYBUS": "C01523",
+        "402 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01523",
         "402 / TICE": "C01617",
-        "403 / SQYBUS": "C02448",
+        "403 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C02448",
         "403 / TICE": "C01618",
         "404 / TICE": "C01619",
         "405 / TICE": "C01620",
         "406 / TICE": "C01621",
         "407 / TICE": "C01622",
         "408 / TICE": "C01623",
-        "409 / N4 Mobilit\u00e9s": "C00026",
+        "409 / Keolis Portes et Val de Brie": "C00026",
         "409 / TICE": "C01624",
         "41 / Cars Hourtoule": "C00425",
         "41 / Francilit\u00e9 Ouest Essonne": "C02449",
+        "41 / Keolis Seine et Oise Est": "C00654",
         "41 / RD Mantois": "C02480",
         "41 / Transdev CEAT": "C02111",
         "41 / Transdev Ile-de-France Ecquevilly": "C00119",
         "41 / Transdev Ile-de-France Houdan": "C01986",
         "41 / Transdev Ile-de-France Vulaines": "C00789",
         "41 / Transdev Marne-et-Ourcq": "C00928",
         "41 / Transdev Senart": "C00853",
         "412 / TICE": "C01625",
         "413 / TICE": "C01626",
-        "414 / SQYBUS": "C01527",
+        "414 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01527",
         "414 / TICE": "C01627",
-        "415 / SQYBUS": "C01528",
+        "415 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01528",
         "415 / TICE": "C01628",
         "416 / TICE": "C01672",
-        "417 / SQYBUS": "C01530",
-        "418 / SQYBUS": "C01531",
+        "417 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01530",
+        "418 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01531",
         "418 / TICE": "C01629",
-        "419 / SQYBUS": "C01532",
+        "419 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01532",
         "419 / TICE": "C01630",
         "41A / Transdev Brie et 2 Morin": "C01060",
         "41B / Transdev Brie et 2 Morin": "C02154",
         "42 / Francilit\u00e9 Ouest Essonne": "C02450",
+        "42 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00571",
+        "42 / Keolis Seine et Oise Est": "C00640",
         "42 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00049",
         "42 / RATP": "C01085",
         "42 / RD Mantois": "C00120",
-        "42 / STAVO": "C00571",
         "42 / Stivo": "C00769",
         "42 / Transdev CEAT": "C02112",
         "42 / Transdev Ile-de-France Vulaines": "C00790",
         "42 / Transdev Marne-et-Ourcq": "C00929",
         "42 / Transdev Marne-la-Vall\u00e9e": "C00634",
         "42 / Transdev Senart": "C00854",
-        "420 / SQYBUS": "C01524",
+        "420 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01524",
         "420 / TICE": "C01956",
         "421 / RATP": "C01323",
-        "422 / SQYBUS": "C01526",
-        "423 / SQYBUS": "C02216",
-        "424 / SQYBUS": "C02217",
+        "422 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01526",
+        "423 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C02216",
+        "424 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C02217",
         "426 / RATP": "C01481",
-        "43 / CIF": "C00214",
+        "43 / Keolis Seine et Oise Est": "C00644",
         "43 / RATP": "C01086",
         "43 / RD Mantois": "C00121",
         "43 / STAVO": "C01872",
         "43 / Stivo": "C00770",
         "43 / Transdev Ile-de-France Vulaines": "C00813",
         "43 / Transdev Marne-la-Vall\u00e9e": "C00635",
+        "43 / Transdev Nord Seine-Saint-Denis": "C00214",
         "43 / Transdev Senart": "C00855",
-        "430 / SQYBUS": "C01677",
-        "431 / SQYBUS": "C01676",
-        "439 / SQYBUS": "C00544",
+        "430 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01677",
+        "431 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01676",
+        "439 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00544",
         "43S / Francilit\u00e9 Ouest Essonne": "C02451",
-        "44 / CIF": "C00215",
+        "44 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01869",
+        "44 / Keolis Seine et Oise Est": "C00653",
         "44 / RD Mantois": "C00108",
-        "44 / STAVO": "C01869",
         "44 / Stivo": "C00771",
         "44 / Transdev Ile-de-France Vulaines": "C00791",
         "44 / Transdev Marne-la-Vall\u00e9e": "C00636",
-        "440 / SQYBUS": "C00545",
-        "441 / SQYBUS": "C01522",
-        "444 / SQYBUS": "C01533",
-        "448 / SQYBUS": "C00535",
-        "449 / SQYBUS": "C00536",
+        "44 / Transdev Nord Seine-Saint-Denis": "C00215",
+        "440 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00545",
+        "441 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01522",
+        "444 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01533",
+        "448 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00535",
+        "449 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00536",
         "44S / Francilit\u00e9 Ouest Essonne": "C02452",
-        "45 / CIF": "C00216",
+        "45 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01870",
         "45 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C00051",
         "45 / RATP": "C02244",
         "45 / RD Mantois": "C00109",
-        "45 / STAVO": "C01870",
         "45 / Stivo": "C00772",
         "45 / Transdev Ile-de-France Houdan": "C01987",
         "45 / Transdev Ile-de-France Vulaines": "C00792",
-        "450 / SQYBUS": "C00537",
-        "451 / SQYBUS": "C00538",
-        "452 / SQYBUS": "C00539",
-        "453 / SQYBUS": "C00540",
+        "45 / Transdev Nord Seine-Saint-Denis": "C00216",
+        "450 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00537",
+        "451 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00538",
+        "452 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00539",
+        "453 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00540",
         "453 / TICE": "C01631",
-        "454 / SQYBUS": "C00541",
-        "455 / SQYBUS": "C00542",
-        "456 / SQYBUS": "C00543",
-        "457 / SQYBUS": "C01668",
-        "458 / SQYBUS": "C01793",
+        "454 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00541",
+        "455 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00542",
+        "456 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00543",
+        "457 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01668",
+        "458 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01793",
+        "459 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C02218",
         "459 / RATP": "C01485",
-        "459 / SQYBUS": "C02218",
         "45S / Francilit\u00e9 Ouest Essonne": "C02453",
         "46 / CIF": "C00217",
         "46 / RATP": "C01087",
         "46 / Transdev Marne-et-Ourcq": "C00930",
         "46 / Transdev Marne-la-Vall\u00e9e": "C01713",
         "46-1 / ProCars": "C01513",
         "46-2 / ProCars": "C02435",
         "46-3 / ProCars": "C02436",
-        "460 / SQYBUS": "C01534",
+        "460 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01534",
         "460 / Transdev Ile-de-France Nanterre": "C02239",
-        "461 / SQYBUS": "C01535",
-        "463 / SQYBUS": "C01537",
-        "464 / SQYBUS": "C01538",
-        "465 / SQYBUS": "C01539",
-        "466 / SQYBUS": "C01540",
+        "461 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01535",
+        "463 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01537",
+        "464 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01538",
+        "465 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01539",
+        "466 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01540",
+        "467 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01541",
         "467 / RATP": "C01324",
-        "467 / SQYBUS": "C01541",
-        "468 / SQYBUS": "C01542",
+        "468 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01542",
         "469 / Mobicit\u00e9": "C02300",
         "47 / CIF": "C00218",
         "47 / RATP": "C01088",
         "47 / Stivo": "C00773",
         "47 / Transdev Marne-et-Ourcq": "C00931",
         "47 / Transdev Marne-la-Vall\u00e9e": "C02016",
         "471 / RATP": "C01488",
-        "475 / SQYBUS": "C01543",
+        "475 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01543",
         "48 / RATP": "C01089",
         "48 / Stivo": "C00774",
         "48 / Transdev Brie et 2 Morin": "C01993",
         "48 / Transdev Ile-de-France Houdan": "C01988",
         "480 / Keolis Ouest Val-de-Marne": "C00006",
         "482 / Keolis Ouest Val-de-Marne": "C00001",
         "483 / Keolis Ouest Val-de-Marne": "C00004",
@@ -1009,239 +1003,259 @@
         "4C / Cars Moreau": "C01454",
         "4D / Cars Moreau": "C01455",
         "4E / Cars Moreau": "C02056",
         "4s / STBC": "C02138",
         "5 / Cars Hourtoule": "C00401",
         "5 / Francilit\u00e9 Ouest Essonne": "C00983",
         "5 / Keolis Argenteuil Boucles de Seine": "C00296",
-        "5 / Keolis Seine et Oise Est": "C00136",
+        "5 / Keolis Portes et Val de Brie": "C00011",
+        "5 / Keolis Seine et Oise Est": "C02567",
         "5 / Keolis Versailles": "C00696",
-        "5 / N4 Mobilit\u00e9s": "C00011",
         "5 / ProCars": "C01503",
         "5 / RD Mantois": "C00727",
         "5 / RD Saclay": "C00070",
         "5 / STBC": "C01427",
         "5 / Transdev CEAT": "C00556",
         "5 / Transdev Ile-de-France Nemours": "C00835",
         "5 / Transdev Ile-de-France Vulaines": "C00787",
         "5 S / Transdev Ile-de-France Conflans": "C02225",
         "50 / CIF": "C00220",
-        "50 / Cars Hourtoule": "C01871",
-        "50 / Keolis Seine et Oise Est": "C00281",
+        "50 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C01871",
+        "50 / Keolis Seine et Oise Est": "C02546",
         "50 / Transdev Marne-et-Ourcq": "C00935",
         "50 / Transdev Senart": "C00836",
         "500 / N4 Mobilit\u00e9s": "C02240",
         "501 / Keolis Val d'Yerres Val de Seine": "C00364",
         "501 / N4 Mobilit\u00e9s": "C00028",
         "501 / Transdev Ile-de-France Houdan": "C00061",
         "501 Scolaire / Keolis Argenteuil Boucles de Seine": "C00309",
-        "502 / Keolis Seine et Oise Est": "C00653",
         "502 / N4 Mobilit\u00e9s": "C00029",
         "502 Scolaire / Keolis Argenteuil Boucles de Seine": "C00310",
         "503 / Transdev Ile-de-France Nanterre": "C01490",
         "503 Scolaire / Keolis Argenteuil Boucles de Seine": "C00311",
-        "51 / Keolis Seine et Oise Est": "C00282",
+        "51 / Keolis Seine et Oise Est": "C02547",
         "51 / STAVO": "C01873",
         "51 / Transdev CEAT": "C02351",
         "51 / Transdev Ile-de-France Houdan": "C01989",
         "51 / Transdev Senart": "C00837",
         "510 / TICE": "C01615",
         "511 / Transdev Ile-de-France Ecquevilly": "C00137",
         "512 / Transdev Ile-de-France Ecquevilly": "C00138",
-        "52 / Keolis Seine et Oise Est": "C00283",
+        "52 / Keolis Seine et Oise Est": "C02548",
         "52 / Keolis Yvelines": "C02219",
         "52 / RATP": "C01090",
         "52 / RD Mantois": "C00744",
         "52 / Transdev Marne-et-Ourcq": "C00937",
         "520 / RATP": "C01334",
-        "526 / Mobicit\u00e9": "C02301",
+        "53 / Keolis Seine et Oise Est": "C02549",
         "53 / Keolis Yvelines": "C02183",
         "53 / Transdev Marne-et-Ourcq": "C00938",
         "53 / Transdev Senart": "C00861",
-        "54 / Keolis Seine et Oise Est": "C00285",
+        "54 / Keolis Seine et Oise Est": "C02550",
         "54 / Keolis Yvelines": "C02184",
         "54 / RATP": "C01092",
         "54 / Transdev Ile-de-France Nanterre": "C00327",
         "54 / Transdev Marne-et-Ourcq": "C00939",
         "54 / Transdev Senart": "C00839",
         "545 / RATP": "C01341",
         "54B / Transdev Marne-et-Ourcq": "C00940",
-        "55 / Keolis Seine et Oise Est": "C01773",
+        "55 / Keolis Seine et Oise Est": "C02551",
         "55 / Stivo": "C02086",
         "55 / Transdev Ile-de-France Houdan": "C01990",
         "55 / Transdev Ile-de-France Nanterre": "C00328",
         "55 / Transdev Senart": "C00838",
         "559A / RATP": "C01345",
         "559B / RATP": "C02080",
         "559C / RATP": "C02081",
         "559D / RATP": "C02082",
         "56 / Keolis Argenteuil Boucles de Seine": "C02360",
+        "56 / Keolis Seine et Oise Est": "C02552",
         "56 / RATP": "C01093",
         "56 / Stivo": "C00781",
         "56 / Transdev Brie et 2 Morin": "C00941",
         "564 / RATP": "C01349",
         "565 / RATP": "C01350",
         "566 / RATP": "C01351",
         "56S / Transdev Brie et 2 Morin": "C00942",
         "57 / Keolis Argenteuil Boucles de Seine": "C02361",
+        "57 / Keolis Seine et Oise Est": "C02553",
         "57 / RATP": "C01094",
         "57 / Stivo": "C00782",
         "57 / Transdev Marne-la-Vall\u00e9e": "C00943",
+        "58 / Keolis Seine et Oise Est": "C02554",
         "58 / RATP": "C01095",
         "58 / Stivo": "C00783",
+        "59 / Keolis Seine et Oise Est": "C02555",
         "59 / RATP": "C02245",
         "59 / Stivo": "C00784",
         "59 / Transdev Brie et 2 Morin": "C00944",
         "59 / Transdev Ile-de-France Rambouillet": "C01954",
         "595 / RATP": "C01369",
-        "6 / Cars Hourtoule": "C02169",
         "6 / Francilit\u00e9 Ouest Essonne": "C02057",
-        "6 / Keolis Argenteuil Boucles de Seine": "C00308",
-        "6 / Keolis Seine et Oise Est": "C00135",
+        "6 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C02169",
+        "6 / Keolis Argenteuil Boucles de Seine": "C01476",
+        "6 / Keolis Portes et Val de Brie": "C00803",
+        "6 / Keolis Seine et Oise Est": "C02568",
         "6 / Keolis Versailles": "C00697",
         "6 / RD Saclay": "C02316",
         "6 / STBC": "C02131",
         "6 / Transdev CEAT": "C00557",
         "6 / Transdev Ile-de-France Vulaines": "C00788",
         "6 / Transdev Vall\u00e9e Sud": "C00343",
         "6-1 / ProCars": "C01504",
         "6-3 / ProCars": "C02434",
+        "60 / Keolis Seine et Oise Est": "C00128",
         "60 / RATP": "C01096",
         "60 / RD Saclay": "C00046",
         "60 / Stivo": "C00785",
         "60 / Transdev Marne-la-Vall\u00e9e": "C00945",
         "602 / TRA": "C01574",
         "603 / TRA": "C01575",
         "604 / TRA": "C01576",
         "605 / TRA": "C01577",
-        "607 / TRA": "C01578",
-        "609 / TRA": "C01579",
+        "607 / Transdev Nord Seine-Saint-Denis": "C01578",
+        "609 / Transdev Nord Seine-Saint-Denis": "C01579",
         "61 / Francilit\u00e9 Ouest Essonne": "C00167",
+        "61 / Keolis Seine et Oise Est": "C00129",
         "61 / RATP": "C01097",
         "61 / Transdev Ile-de-France Houdan": "C01991",
         "61 / Transdev Marne-et-Ourcq": "C00946",
-        "610 / TRA": "C01580",
-        "611 / TRA": "C01884",
+        "610 / Transdev Nord Seine-Saint-Denis": "C01580",
+        "611 / Transdev Nord Seine-Saint-Denis": "C01884",
         "613 / TRA": "C01581",
-        "615 / TRA": "C01583",
-        "616 / TRA": "C01584",
-        "617 / TRA": "C01585",
-        "618 / TRA": "C01586",
-        "619 / TRA": "C01587",
+        "615 / Transdev Nord Seine-Saint-Denis": "C01583",
+        "616 / Transdev Nord Seine-Saint-Denis": "C01584",
+        "617 / Transdev Nord Seine-Saint-Denis": "C01585",
+        "618 / Transdev Nord Seine-Saint-Denis": "C01586",
+        "619 / Transdev Nord Seine-Saint-Denis": "C01587",
         "61A / Transdev Senart": "C02194",
         "61B / Transdev Marne-et-Ourcq": "C02345",
         "61B / Transdev Senart": "C02187",
         "62 / Francilit\u00e9 Ouest Essonne": "C02185",
+        "62 / Keolis Seine et Oise Est": "C00130",
         "62 / RATP": "C01098",
-        "620 / TRA": "C01588",
+        "620 / Transdev Nord Seine-Saint-Denis": "C01588",
         "623 / TRA": "C01589",
-        "627 / TRA": "C01590",
+        "627 / Transdev Nord Seine-Saint-Denis": "C01590",
         "62A / Transdev Senart": "C02191",
         "62B / Transdev Senart": "C02192",
         "62C / Transdev Senart": "C02188",
         "63 / Francilit\u00e9 Ouest Essonne": "C02186",
+        "63 / Keolis Seine et Oise Est": "C02222",
         "63 / RATP": "C01099",
         "63 / Transdev Marne-et-Ourcq": "C00948",
         "63 / Transdev Senart": "C02193",
-        "637 / TRA": "C01591",
+        "637 / Transdev Nord Seine-Saint-Denis": "C01591",
+        "64 / Keolis Seine et Oise Est": "C02556",
         "64 / RATP": "C01100",
         "64 / Transdev Senart": "C00860",
-        "640 / TRA": "C01592",
-        "642 / TRA": "C01594",
+        "640 / Transdev Nord Seine-Saint-Denis": "C01592",
+        "642 / Transdev Nord Seine-Saint-Denis": "C01594",
         "643 / TRA": "C02092",
         "644 / TRA": "C01595",
+        "65 / Keolis Seine et Oise Est": "C02557",
         "65 / Transdev Ile-de-France Houdan": "C00063",
         "65 / Transdev Marne-et-Ourcq": "C00950",
+        "66 / Keolis Seine et Oise Est": "C02558",
         "66 / RATP": "C01102",
+        "67 / Keolis Seine et Oise Est": "C02559",
         "67 / RATP": "C01103",
+        "68 / Keolis Seine et Oise Est": "C02560",
         "68 / RATP": "C01104",
         "68-09 / Francilit\u00e9 Ouest Essonne": "C00967",
         "68-13A / Francilit\u00e9 Ouest Essonne": "C02296",
         "68-13B / Francilit\u00e9 Ouest Essonne": "C02297",
         "68-16 / Francilit\u00e9 Ouest Essonne": "C00970",
         "68.01 / Keolis Meyer": "C00962",
         "68.01S / Keolis Meyer": "C02065",
         "68.02 / Keolis Meyer": "C00963",
         "68.05 A / Keolis Meyer": "C00964",
         "68.05 B / Keolis Meyer": "C00972",
         "68.06 / Keolis Meyer": "C00965",
         "68.08 / Keolis Meyer": "C00966",
         "68.100 / Keolis Meyer": "C00971",
         "68.14 / Francilit\u00e9 Ouest Essonne": "C00969",
+        "69 / Keolis Seine et Oise Est": "C02561",
         "69 / RATP": "C01105",
         "7 / Cars Hourtoule": "C00402",
         "7 / Keolis Argenteuil Boucles de Seine": "C00312",
-        "7 / Keolis Seine et Oise Est": "C01783",
+        "7 / Keolis Portes et Val de Brie": "C00546",
+        "7 / Keolis Seine et Oise Est": "C02569",
         "7 / Keolis Versailles": "C00698",
-        "7 / N4 Mobilit\u00e9s": "C00012",
         "7 / RD Mantois": "C00730",
         "7 / RD Saclay": "C00072",
-        "7 / SETRA": "C00546",
         "7 / STBC": "C02136",
         "7 / Transdev CEAT": "C00084",
         "7 / Transdev Vall\u00e9e Sud": "C00344",
+        "70 / Keolis Seine et Oise Est": "C00275",
         "70 / RATP": "C01106",
         "70 / Transdev Brie et 2 Morin": "C00951",
         "7001 / Cars Soeur": "C00985",
         "7001 Scolaire / Cars Soeur": "C00986",
         "7002 / Cars Soeur": "C00987",
         "7002 Scolaire / Cars Soeur": "C02390",
         "7005 / Cars Soeur": "C00989",
         "7006 / Cars Soeur": "C00990",
         "701 / Autobus du Fort": "C01548",
         "701 / CIF": "C00245",
-        "702 / Autobus du Fort": "C01549",
         "702 / CIF": "C00246",
-        "703 / Autobus du Fort": "C01550",
+        "702 / Transdev Nord Seine-Saint-Denis": "C01549",
         "703 / CIF": "C00247",
+        "703 / Transdev Nord Seine-Saint-Denis": "C01550",
         "704 / CIF": "C00248",
         "705 / CIF": "C00249",
         "707 / CIF": "C00250",
         "708 / CIF": "C00251",
         "709 / CIF": "C00252",
         "71 / CIF": "C00221",
+        "71 / Keolis Seine et Oise Est": "C00643",
         "71 / RATP": "C02246",
         "71 / RD Mantois": "C02161",
         "71 / Transdev Brie et 2 Morin": "C02207",
         "71 / Transdev CEAT": "C02428",
         "71 / Transdev Ile-de-France Ecquevilly": "C00122",
         "710 / CIF": "C00253",
         "711 / CIF": "C00254",
         "714 / CIF": "C00255",
         "715 / CIF": "C00256",
+        "72 / Keolis Seine et Oise Est": "C02562",
         "72 / RATP": "C01107",
         "72 / RD Mantois": "C01036",
+        "73 / Keolis Seine et Oise Est": "C00110",
         "73 / RATP": "C01108",
         "73 / RD Mantois": "C01034",
         "73 / Transdev Brie et 2 Morin": "C00952",
+        "74 / Keolis Seine et Oise Est": "C02563",
         "74 / RATP": "C01109",
         "74 / RD Mantois": "C01035",
         "749 / CIF": "C01759",
+        "75 / Keolis Seine et Oise Est": "C02564",
         "75 / RATP": "C01110",
         "75 / RD Mantois": "C01033",
         "751 / CIF": "C00257",
         "753 / CIF": "C01813",
         "755 / CIF": "C00259",
         "756 / CIF": "C00260",
+        "76 / Keolis Seine et Oise Est": "C00454",
         "76 / RATP": "C01111",
         "76 / RD Mantois": "C02162",
         "76 / Transdev Ile-de-France Ecquevilly": "C02076",
         "77 / RATP": "C02251",
         "777 / Transdev Marne-et-Ourcq": "C00262",
         "79 / Transdev Ile-de-France Rambouillet": "C01955",
         "7A / Transdev Ile-de-France Nemours": "C00820",
         "7B / Transdev Ile-de-France Nemours": "C01958",
         "7C / Transdev Ile-de-France Nemours": "C01959",
         "7D / Transdev Ile-de-France Nemours": "C01960",
         "7s / STBC": "C02135",
-        "8 / Cars Hourtoule": "C00418",
+        "8 (future 408) / RD Bi\u00e8vre": "C00345",
+        "8 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C00418",
         "8 / Keolis Argenteuil Boucles de Seine": "C00297",
         "8 / Keolis Versailles": "C00699",
         "8 / ProCars": "C01506",
-        "8 / RD Bi\u00e8vre": "C00345",
         "8 / RD Saclay": "C00073",
         "8 / STBC": "C01717",
         "8 / TVF": "C00656",
         "8 / Transdev Boucle des Lys": "C00144",
         "8 / Transdev CEAT": "C00085",
         "8 / Transdev Ile-de-France Vulaines": "C01947",
         "80 / RATP": "C01112",
@@ -1267,42 +1281,47 @@
         "8A / Transdev Brie et 2 Morin": "C00905",
         "8A / Transdev Ile-de-France Nemours": "C00821",
         "8ASc / Transdev Brie et 2 Morin": "C02318",
         "8B / Transdev Brie et 2 Morin": "C00906",
         "8B / Transdev Ile-de-France Nemours": "C01961",
         "8C / Transdev Brie et 2 Morin": "C00907",
         "8s / STBC": "C02139",
-        "9 / Cars Hourtoule": "C02170",
+        "9 (future 409) / RD Bi\u00e8vre": "C00346",
+        "9 / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C02170",
         "9 / Keolis Argenteuil Boucles de Seine": "C00298",
-        "9 / Keolis Seine et Oise Est": "C00273",
         "9 / Keolis Versailles": "C00700",
-        "9 / RD Bi\u00e8vre": "C00346",
         "9 / RD Mantois": "C00731",
         "9 / RD Saclay": "C01561",
         "9 / STBC": "C02133",
         "9 / TVF": "C01776",
         "9 / Transdev CEAT": "C02456",
         "9 / Transdev Ile-de-France Houdan": "C00057",
         "9 / Transdev Ile-de-France Vulaines": "C00786",
+        "90 / Keolis Seine et Oise Est": "C02543",
         "90 / RD Mantois": "C00756",
+        "91 / Keolis Seine et Oise Est": "C00271",
         "91 / RATP": "C01122",
         "91 / RD Mantois": "C00760",
         "91-02 / Francilit\u00e9 Ouest Essonne": "C01563",
         "91-03 / Francilit\u00e9 Ouest Essonne": "C01564",
         "91-07 / Francilit\u00e9 Ouest Essonne": "C01568",
         "913.07 / Francilit\u00e9 Ouest Essonne": "C00977",
         "913.08 / Francilit\u00e9 Ouest Essonne": "C00978",
         "913.10 / Francilit\u00e9 Ouest Essonne": "C00979",
         "913.17A / Francilit\u00e9 Ouest Essonne": "C02470",
         "913.17B / Francilit\u00e9 Ouest Essonne": "C02472",
         "913.17C / Francilit\u00e9 Ouest Essonne": "C02473",
         "913.50 / Francilit\u00e9 Ouest Essonne": "C00984",
+        "92 / Keolis Seine et Oise Est": "C02544",
         "92 / RATP": "C01123",
+        "93 / Keolis Seine et Oise Est": "C00115",
         "93 / RATP": "C01124",
+        "94 / Keolis Seine et Oise Est": "C02545",
         "94 / RATP": "C01125",
+        "95 / Keolis Seine et Oise Est": "C02536",
         "95 / RATP": "C01126",
         "95-01 / CIF": "C00264",
         "95-02 / CIF": "C00265",
         "95-03A / Cars Lacroix": "C00471",
         "95-03B / Cars Lacroix": "C00472",
         "95-04 / Transdev Vexin": "C01552",
         "95-05 / Transdev Vexin": "C00393",
@@ -1338,98 +1357,88 @@
         "95-46 / Transdev Vexin": "C01559",
         "95-47 / Transdev Vexin": "C01560",
         "95-48 / Transdev Vexin": "C02206",
         "95-49 / Transdev Vexin": "C02414",
         "95-50 / Transdev Vexin": "C02413",
         "95-51 / Transdev Vexin": "C02415",
         "96 / RATP": "C01127",
-        "98 / Keolis Seine et Oise Est": "C00286",
         "9A / Transdev Boucle des Lys": "C00145",
         "9A / Transdev Ile-de-France Nemours": "C00822",
         "9AB / Transdev Boucle des Lys": "C00146",
         "9B / Transdev Boucle des Lys": "C00147",
         "9B / Transdev Ile-de-France Nemours": "C01962",
         "9C / Transdev Ile-de-France Nemours": "C01963",
         "9D / Transdev Boucle des Lys": "C00148",
         "9D / Transdev Ile-de-France Nemours": "C01964",
         "9s / STBC": "C02132",
         "A / Autocars Dominique": "C01830",
         "A / INTERVAL": "C01435",
         "A / Keolis Argenteuil Boucles de Seine": "C00330",
         "A / Keolis Val d'Oise": "C01659",
-        "A / Keolis Val d'Yerres Val de Seine": "C00354",
+        "A / Keolis Val d'Yerres Val de Seine": "C00580",
         "A / N4 Mobilit\u00e9s": "C00031",
         "A / RD Mantois": "C01949",
-        "A / SNCF": "C01849",
         "A / Transdev Brie et 2 Morin": "C02035",
         "A / Transdev Ile-de-France Rambouillet": "C00182",
         "A / Transdev Marne-et-Ourcq": "C00954",
         "A / Transdev Melun": "C00875",
         "A1 / Transdev Ile-de-France Conflans": "C01685",
         "A2 / Transdev Ile-de-France Conflans": "C01674",
-        "AQ / Cars Hourtoule": "C02171",
+        "AMIBUS / Transdev Vall\u00e9e Sud": "C01366",
+        "AQ / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C02171",
         "AS AUTOBUS SURESNOIS / RATP": "C01340",
+        "A\u00e9robus / A\u00e9roport Paris-Beauvais / SAGEB": "C02179",
         "B / Autocars Dominique": "C01831",
         "B / Cars Hourtoule": "C00421",
         "B / INTERVAL": "C01436",
         "B / Keolis Argenteuil Boucles de Seine": "C02149",
         "B / Keolis Val d'Oise": "C01660",
         "B / Keolis Val d'Yerres Val de Seine": "C00355",
         "B / N4 Mobilit\u00e9s": "C00033",
         "B / SNCF": "C01850",
         "B / STRAV": "C00581",
         "B / Transdev Brie et 2 Morin": "C02036",
         "B / Transdev Ile-de-France Rambouillet": "C00183",
         "B / Transdev Marne-et-Ourcq": "C00953",
         "B / Transdev Melun": "C00876",
-        "BALADOBUS / SAVAC": "C02123",
-        "BL / Cars Hourtoule": "C02172",
+        "BL / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C02172",
         "BM / Keolis Val d'Yerres Val de Seine": "C00356",
         "BRAY 11 / Cars Moreau": "C01471",
         "BRAY 3 / Cars Moreau": "C01468",
         "BRAY 9 / Cars Moreau": "C01467",
         "Brie Bus / SETRA": "C00549",
-        "Bus de substitution du RER A / SNCF": "C02442",
         "Bus de substitution du RER B / SNCF": "C02385",
+        "Bus de substitution du m\u00e9tro 11 / RATP": "C02531",
         "Bus de substitution du m\u00e9tro 14 / RATP": "C02494",
         "C / Autocars Dominique": "C01832",
         "C / INTERVAL": "C01437",
         "C / Keolis Argenteuil Boucles de Seine": "C00335",
         "C / Keolis Val d'Oise": "C00606",
-        "C / Keolis Val d'Yerres Val de Seine": "C00582",
+        "C / Keolis Val d'Yerres Val de Seine": "C00357",
         "C / N4 Mobilit\u00e9s": "C00034",
         "C / RD Mantois": "C01600",
         "C / SNCF": "C01851",
         "C / Transdev Ile-de-France Rambouillet": "C01678",
         "C / Transdev Marne-et-Ourcq": "C00902",
         "C / Transdev Melun": "C00877",
         "CHOISYBUS / RATP": "C01360",
         "CITALIEN / Transdev Senart": "C01806",
         "CPSF / Transdev Senart": "C00869",
-        "CSP / Cars Hourtoule": "C02173",
-        "Cam\u00e9l\u00e9on T2 / RATP": "C02405",
-        "Cam\u00e9l\u00e9on T3a / RATP": "C02406",
-        "Cam\u00e9l\u00e9on T3b / RATP": "C02407",
-        "Cam\u00e9l\u00e9on T5 / RATP": "C02408",
-        "Cam\u00e9l\u00e9on T7 / RATP": "C02410",
-        "Cam\u00e9l\u00e9on T8 / RATP": "C02411",
+        "CSP / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C02173",
         "Cd / Transdev Melun": "C00878",
-        "ChavilBus Nord / Mobicit\u00e9": "C02302",
-        "ChavilBus Sud / Mobicit\u00e9": "C02303",
-        "Chavilbus Unique / Mobicit\u00e9": "C02304",
+        "Chavilbus / SAVAC": "C02304",
         "Cit\u00e9Val Cormeilles-en-Parisis / Cars Lacroix": "C02040",
         "Cit\u00e9Val Ermont / Cars Lacroix": "C02517",
         "Cit\u00e9Val Franconville / Cars Lacroix": "C02041",
         "Cit\u00e9Val Nord Herblay / Cars Lacroix": "C00480",
         "Cit\u00e9Val Sud Herblay / Cars Lacroix": "C00481",
         "ClamiBus / Transdev Vall\u00e9e Sud": "C01357",
-        "Conflans Ste Honorine - Mantes / SNCF": "C02367",
         "Corbeil - La Fert\u00e9 Alais / SNCF": "C02363",
         "Corbeil - Melun / SNCF": "C02364",
-        "Coulommiers - La Fert\u00e9 Gaucher Centre / SNCF": "C02365",
+        "Coulommiers - La Fert\u00e9 Gaucher Centre / Transdev Brie et 2 Morin": "C02365",
         "D / Keolis Argenteuil Boucles de Seine": "C01755",
         "D / Keolis Val d'Yerres Val de Seine": "C00579",
         "D / N4 Mobilit\u00e9s": "C00032",
         "D / RD Mantois": "C01601",
         "D / SNCF": "C01852",
         "D / Transdev Ile-de-France Rambouillet": "C01824",
         "D / Transdev Marne-et-Ourcq": "C00958",
@@ -1471,26 +1480,28 @@
         "DM5S / Keolis Meyer": "C02398",
         "DM7S / Keolis Meyer": "C00669",
         "DM9 / Keolis Meyer": "C00671",
         "DM9S / Keolis Meyer": "C02399",
         "E / Autocars Dominique": "C02497",
         "E / Keolis Argenteuil Boucles de Seine": "C00332",
         "E / Keolis Val d'Oise": "C00604",
-        "E / Keolis Val d'Yerres Val de Seine": "C00599",
+        "E / Keolis Val d'Yerres Val de Seine": "C00359",
         "E / N4 Mobilit\u00e9s": "C00030",
         "E / RD Mantois": "C01602",
         "E / SNCF": "C01853",
         "E / Transdev Ile-de-France Rambouillet": "C00184",
         "E / Transdev Marne-et-Ourcq": "C02236",
         "E / Transdev Melun": "C00881",
         "E1 / Keolis Val d'Yerres Val de Seine": "C00600",
         "E2 / Keolis Val d'Yerres Val de Seine": "C00601",
         "EOLIEN / RATP": "C01338",
         "EX100 Chelles / Keolis Mobilit\u00e9 Roissy": "C02062",
         "EX100 Persan / Keolis Mobilit\u00e9 Roissy": "C01675",
+        "EX16 Ozoir / Keolis Portes et Val de Brie": "C00027",
+        "EX93 Bobigny / CIF": "C00223",
         "EXPRESS 91-01 / Keolis Val d'Yerres Val de Seine": "C01562",
         "EXPRESS 91-04 / Albatrans": "C01565",
         "EXPRESS 91-05 / RD Saclay": "C01566",
         "EXPRESS 91-06 / RD Saclay": "C01567",
         "EXPRESS 91-08 / RD Saclay": "C01569",
         "EXPRESS 91-09 / Keolis Val d'Yerres Val de Seine": "C01570",
         "EXPRESS 91-10 / Albatrans": "C01571",
@@ -1500,15 +1511,14 @@
         "Emplet / INTERVAL": "C01443",
         "Es / Transdev Marne-et-Ourcq": "C02237",
         "Express 01 / Transdev Brie et 2 Morin": "C01062",
         "Express 07 / ProCars": "C01505",
         "Express 1 / Transdev Boucle des Lys": "C00143",
         "Express 100 / Transdev Ile-de-France Lys": "C00263",
         "Express 100 Les Mureaux St Quentin / Stile": "C00655",
-        "Express 16 / N4 Mobilit\u00e9s": "C00027",
         "Express 16 / Transdev Ile-de-France Conflans": "C00151",
         "Express 17 / Transdev Brie et 2 Morin": "C01063",
         "Express 18 / Transdev Marne-et-Ourcq": "C00637",
         "Express 19 / AMV": "C00639",
         "Express 191-100 / Keolis Val d'Yerres Val de Seine": "C00379",
         "Express 20 / Transdev Marne-et-Ourcq": "C00661",
         "Express 27 / Transdev Ile-de-France Conflans": "C02204",
@@ -1519,75 +1529,70 @@
         "Express 50 / ProCars": "C01500",
         "Express 60 / Transdev Ile-de-France Houdan": "C00062",
         "Express 62 / Transdev Brie et 2 Morin": "C00947",
         "Express 67 / Transdev Brie et 2 Morin": "C00960",
         "Express 67 / Transdev Ile-de-France Houdan": "C00064",
         "Express 69 / Transdev Marne-et-Ourcq": "C00961",
         "Express 78 / Cars Hourtoule": "C00426",
-        "Express 93 / CIF": "C00223",
         "Express 95-18 / Transdev Ile-de-France Conflans": "C01472",
         "Express A14 Bonni\u00e8res / RD Mantois": "C02248",
-        "Express A14 Chambourcy / Transdev Boucle des Lys": "C02269",
         "Express A14 Les Mureaux / Stile": "C00753",
         "Express A14 Mantes / RD Mantois": "C02249",
         "Express A14 Verneuil / Stile": "C00754",
         "Extr\u00eame Soir\u00e9e / RD Mantois": "C02479",
         "F / Autocars Dominique": "C01902",
         "F / INTERVAL": "C01442",
         "F / Keolis Argenteuil Boucles de Seine": "C02150",
         "F / Keolis Val d'Oise": "C01662",
-        "F / Keolis Val d'Yerres Val de Seine": "C00577",
+        "F / Keolis Val d'Yerres Val de Seine": "C00360",
         "F / RD Mantois": "C01613",
         "F / Transdev Marne-et-Ourcq": "C00900",
         "F / Transdev Melun": "C00882",
         "F4 / Keolis Val d'Yerres Val de Seine": "C00586",
         "FA / STAVO": "C01874",
         "Fd / Transdev Melun": "C00883",
         "Fileo Saint-Pathus (sur r\u00e9servation) / Keolis Mobilit\u00e9 Roissy": "C01823",
         "Fil\u00e9o Goussainville (sur r\u00e9servation) / Keolis Mobilit\u00e9 Roissy": "C01432",
         "Fil\u00e9o Othis (sur r\u00e9servation) / Keolis Mobilit\u00e9 Roissy": "C01429",
         "Fil\u00e9o Roissy Sud - Sevran et Aulnay / Keolis Mobilit\u00e9 Roissy": "C01670",
         "Fil\u00e9o Roissy Sud - Tremblay (sur r\u00e9servation) / Keolis Mobilit\u00e9 Roissy": "C01434",
-        "Fil\u00e9o Roissy Sud - Villeparisis Mitry-Mory(sur r\u00e9servation) / Keolis Mobilit\u00e9 Roissy": "C01430",
         "Fil\u00e9o Roissy Sud - Villeparisis et Mitry (sur r\u00e9servation) / Keolis Mobilit\u00e9 Roissy": "C02060",
         "Fil\u00e9o Roissy Sud - Villepinte (sur r\u00e9servation) / Keolis Mobilit\u00e9 Roissy": "C01671",
         "Fil\u00e9o Sarcelles (sur r\u00e9servation) / Keolis Mobilit\u00e9 Roissy": "C01431",
         "Fil\u00e9o Survilliers (sur r\u00e9servation) / Keolis Mobilit\u00e9 Roissy": "C01712",
         "Fil\u00e9o Villiers-le-Bel (sur r\u00e9servation) / Keolis Mobilit\u00e9 Roissy": "C01433",
         "Fs / Transdev Marne-et-Ourcq": "C02230",
         "G / Autocars Dominique": "C01836",
         "G / INTERVAL": "C01439",
         "G / Keolis Argenteuil Boucles de Seine": "C00337",
         "G / Keolis Val d'Oise": "C00605",
         "G / RD Mantois": "C01614",
         "G / Transdev Marne-et-Ourcq": "C00957",
         "G / Transdev Melun": "C00891",
-        "G1-G2 / Keolis Val d'Yerres Val de Seine": "C00587",
-        "G2 / Keolis Val d'Yerres Val de Seine": "C00588",
+        "GPSO Bus / SAVAC": "C02301",
         "Gbus / CIF": "C00224",
         "H / Autocars Dominique": "C01903",
         "H / Keolis Argenteuil Boucles de Seine": "C00317",
         "H / Keolis Val d'Yerres Val de Seine": "C00576",
         "H / SNCF": "C01842",
         "H / Transdev Marne-et-Ourcq": "C00955",
         "I / INTERVAL": "C01441",
         "I / Keolis Val d'Yerres Val de Seine": "C00592",
         "I / RD Mantois": "C01603",
         "I / Transdev Marne-et-Ourcq": "C00959",
         "I / Transdev Melun": "C00801",
-        "I / Ulysse": "C01905",
         "Inter-Vals / Keolis Val d'Yerres Val de Seine": "C00351",
         "J / Autocars Dominique": "C01837",
         "J / Keolis Argenteuil Boucles de Seine": "C00316",
         "J / SNCF": "C01846",
         "J / Transdev Marne-et-Ourcq": "C00898",
         "J / Transdev Melun": "C00895",
         "J1 / STRAV": "C00574",
         "J2 / STRAV": "C00575",
-        "JV / Cars Hourtoule": "C02174",
+        "JV / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C02174",
         "Js / Transdev Marne-et-Ourcq": "C00899",
         "K / Autocars Dominique": "C02439",
         "K / Keolis Argenteuil Boucles de Seine": "C00334",
         "K / RD Mantois": "C01605",
         "K / SNCF": "C01844",
         "K / STRAV": "C00573",
         "K / Transdev Marne-et-Ourcq": "C00949",
@@ -1604,15 +1609,14 @@
         "L'Hirondelle / Transdev Vall\u00e9e Sud": "C01370",
         "LA NAVETTE / RATP": "C01335",
         "LM1 / Keolis Val d'Yerres Val de Seine": "C00365",
         "LM2 / Keolis Val d'Yerres Val de Seine": "C00366",
         "LM3 / Keolis Val d'Yerres Val de Seine": "C00367",
         "LP1 / Keolis Val d'Yerres Val de Seine": "C00363",
         "LP2 / Keolis Val d'Yerres Val de Seine": "C00374",
-        "La Navette de Garches": "C01928",
         "La Navette de Thiais / RATP": "C01780",
         "La Traverse Batignolles-Bichat / RATP": "C01332",
         "La Traverse Bi\u00e8vre Montsouris / RATP": "C01330",
         "La Traverse Brancion-Commerce / Autocars Dominique": "C01757",
         "La Traverse Ney - Flandre / RATP": "C01333",
         "La Traverse de Charonne / RATP": "C01329",
         "Le Bus du port / RATP": "C01839",
@@ -1625,52 +1629,51 @@
         "M / Autocars Dominique": "C02423",
         "M / Cars Hourtoule": "C00424",
         "M / Keolis Argenteuil Boucles de Seine": "C00336",
         "M / Keolis Val d'Yerres Val de Seine": "C00591",
         "M / RD Mantois": "C01606",
         "M / Transdev Marne-et-Ourcq": "C00915",
         "M / Transdev Melun": "C00885",
+        "MONTBUS / Transdev Vall\u00e9e Sud": "C01336",
         "Magical Shuttle CDG / Magical Shuttle": "C01545",
         "Magical Shuttle Orly / Magical Shuttle": "C01546",
         "Magical Shuttle Selected / Magical Shuttle": "C01544",
         "Ms / Transdev Marne-et-Ourcq": "C02232",
         "N / Autocars Dominique": "C02424",
-        "N / Keolis Val d'Yerres Val de Seine": "C00584",
         "N / RD Mantois": "C01607",
         "N / SNCF": "C01845",
         "N / Transdev Marne-et-Ourcq": "C02234",
         "N / Transdev Melun": "C00884",
         "N01 / RATP": "C01413",
         "N02 / RATP": "C01414",
         "N1 / ADP": "C00562",
-        "N1 / Keolis Seine et Oise Est": "C01784",
         "N11 / RATP": "C01415",
         "N12 / RATP": "C01420",
         "N122 / RATP": "C01421",
         "N13 / RATP": "C01419",
-        "N130 / SNCF": "C01634",
+        "N130 / Transdev Brie et 2 Morin": "C01634",
         "N131 / SNCF": "C01636",
         "N132 / SNCF": "C01633",
-        "N133 / SNCF": "C01648",
-        "N134 / SNCF": "C01642",
-        "N135 / SNCF": "C01643",
+        "N133 / Keolis Val d'Yerres Val de Seine": "C01648",
+        "N134 / Keolis Val d'Yerres Val de Seine": "C01642",
+        "N135 / Keolis Val d'Yerres Val de Seine": "C01643",
         "N138 / Transdev Brie et 2 Morin": "C02487",
         "N14 / RATP": "C01418",
         "N140 / SNCF": "C01638",
-        "N141 / SNCF": "C01639",
-        "N142 / SNCF": "C01640",
+        "N141 / Transdev Marne-et-Ourcq": "C01639",
+        "N142 / Keolis Portes et Val de Brie": "C01640",
         "N143 / SNCF": "C01644",
         "N144 / SNCF": "C01645",
         "N145 / SNCF": "C01646",
         "N15 / RATP": "C01417",
-        "N150 / SNCF": "C01637",
+        "N150 / Transdev Vexin": "C01637",
         "N151 / RD Mantois": "C01635",
-        "N152 / SNCF": "C01641",
+        "N152 / Transdev Vexin": "C01641",
         "N153 / RATP": "C01422",
-        "N154 / SNCF": "C01647",
+        "N154 / Transdev Vexin": "C01647",
         "N155 / Keolis Seine et Oise Est": "C02526",
         "N16 / RATP": "C01416",
         "N2 / ADP": "C01792",
         "N21 / RATP": "C01401",
         "N22 / RATP": "C01407",
         "N23 / RATP": "C01397",
         "N24 / RATP": "C01392",
@@ -1690,17 +1693,15 @@
         "N61 / RATP": "C01402",
         "N62 / RATP": "C01403",
         "N63 / RATP": "C01408",
         "N66 / RATP": "C01807",
         "N71 / RATP": "C01410",
         "NANGIBUS / ProCars": "C02294",
         "Navette Bel Air - La For\u00eat / SAVAC": "C02394",
-        "Navette Paris-Beauvais / A\u00e9roport Paris Beauvais": "C02179",
-        "Navette autonome Vincennes / RATP": "C02488",
-        "Navette de Bouffemont / Cars Rose": "C00479",
+        "Navette de Bouffemont / Cars Lacroix": "C00479",
         "Ns / Transdev Marne-et-Ourcq": "C02235",
         "O / Autocars Dominique": "C02425",
         "O / Transdev Melun": "C00897",
         "O1 / STRAV": "C00594",
         "O2 / STRAV": "C01751",
         "ORLYBUS / RATP": "C01261",
         "Os / Transdev Marne-et-Ourcq": "C02233",
@@ -1734,34 +1735,29 @@
         "R109 / CIF": "C00244",
         "R110 / CIF": "C00235",
         "R111 / CIF": "C00236",
         "R112 / CIF": "C00237",
         "R113 / CIF": "C00238",
         "R114 / CIF": "C01816",
         "R117 / CIF": "C00226",
-        "R1A / Keolis Val d'Yerres Val de Seine": "C02101",
-        "R1B / Keolis Val d'Yerres Val de Seine": "C02102",
         "R2 / CIF": "C00229",
-        "R2 / Keolis Val d'Yerres Val de Seine": "C02103",
         "R2 Nord / Transdev Boucle des Lys": "C00158",
         "R2 Sud / Transdev Boucle des Lys": "C00159",
         "R3 / CIF": "C00230",
-        "R3 / Keolis Val d'Yerres Val de Seine": "C02104",
         "R3 Nord / Transdev Boucle des Lys": "C00161",
         "R3 Sud / Transdev Boucle des Lys": "C00162",
         "R4 / CIF": "C00231",
         "R4 / Transdev Boucle des Lys": "C00156",
         "R48 / CIF": "C00219",
         "R5 / CIF": "C00232",
         "R5 / Transdev Boucle des Lys": "C00157",
         "R6 / CIF": "C00233",
         "R7 / CIF": "C00234",
         "R8 / CIF": "C00207",
         "RD / Keolis Val d'Yerres Val de Seine": "C00377",
-        "RD14 / Keolis Val d'Yerres Val de Seine": "C02484",
         "RIVER PLAZA / RATP": "C01356",
         "ROISSYBUS / RATP": "C01300",
         "S / Keolis Val d'Yerres Val de Seine": "C00590",
         "S1 / Keolis Argenteuil Boucles de Seine": "C02148",
         "S1 / RD Saclay": "C01651",
         "S1 / Transdev CEAT": "C01703",
         "S1 / Transdev Melun": "C00892",
@@ -1793,92 +1789,80 @@
         "S6 / Transdev Melun": "C00886",
         "S7 / Keolis Argenteuil Boucles de Seine": "C02147",
         "S7 / Transdev Melun": "C02283",
         "S8 / Transdev Melun": "C02284",
         "S9 / RD Saclay": "C02224",
         "S9 / Transdev Melun": "C02209",
         "SAMOIS / Cars Losay": "C01494",
-        "SRL Houilles / Keolis Argenteuil Boucles de Seine": "C02515",
-        "SRL Le V\u00e9sinet / Keolis Argenteuil Boucles de Seine": "C02516",
         "SUBB / RATP": "C01353",
         "Soir Saint-Germain-en-Laye / Transdev Boucle des Lys": "C02491",
         "Soir Versailles-Chantiers / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C02513",
         "Soir\u00e9e Bouray / Keolis Val d'Essonne Deux Vall\u00e9es": "C02486",
         "Soir\u00e9e Boussy Saint Antoine / Keolis Val d'Yerres Val de Seine": "C02508",
         "Soir\u00e9e Brunoy Sud / Keolis Val d'Yerres Val de Seine": "C02507",
         "Soir\u00e9e Crosne / Keolis Val d'Yerres Val de Seine": "C02504",
         "Soir\u00e9e Domont / Transdev Valmy": "C02464",
         "Soir\u00e9e Draveil / Keolis Val d'Yerres Val de Seine": "C02260",
         "Soir\u00e9e Etampes / Francilit\u00e9 Ouest Essonne": "C02474",
         "Soir\u00e9e Louvres / CIF": "C02030",
-        "Soir\u00e9e Meaux Nord / Transdev Marne-et-Ourcq": "C02489",
-        "Soir\u00e9e Meaux Sud / Transdev Marne-et-Ourcq": "C02490",
         "Soir\u00e9e Mennecy / Keolis Val d'Essonne Deux Vall\u00e9es": "C02220",
         "Soir\u00e9e Montgeron / Keolis Val d'Yerres Val de Seine": "C02262",
         "Soir\u00e9e Ozoir-la-Ferri\u00e8re / Keolis Portes et Val de Brie": "C02523",
+        "Soir\u00e9e Poissy - Carri\u00e8res-sous-Poissy - Verneuil-sur-Seine - Les Mureaux / Keolis Seine et Oise Est": "C02589",
         "Soir\u00e9e Quincy sous S\u00e9nart / Keolis Val d'Yerres Val de Seine": "C02509",
         "Soir\u00e9e Survilliers - Fosses / CIF": "C02255",
         "Soir\u00e9e Tournan-Gretz / Keolis Portes et Val de Brie": "C02522",
         "Soir\u00e9e Vigneux / Keolis Val d'Yerres Val de Seine": "C02261",
         "Soir\u00e9e Yerres Nord / Keolis Val d'Yerres Val de Seine": "C02505",
         "Soir\u00e9e Yerres Sud / Keolis Val d'Yerres Val de Seine": "C02506",
         "Soir\u00e9e \u00c9couen \u00c9zanville / Transdev Valmy": "C02465",
         "T / Autocars Dominique": "C02500",
         "T / Keolis Argenteuil Boucles de Seine": "C02144",
         "T / Transdev Melun": "C02282",
-        "T'bus 1 / CIF": "C02265",
-        "T'bus 2 / CIF": "C02266",
-        "T'bus 3 / CIF": "C02267",
-        "T11 / SNCF": "C02019",
+        "T'bus 1 / Transdev Nord Seine-Saint-Denis": "C02265",
+        "T'bus 2 / Transdev Nord Seine-Saint-Denis": "C02266",
+        "T'bus 3 / Transdev Nord Seine-Saint-Denis": "C02267",
         "T13 / SNCF": "C02469",
         "T4 / SNCF": "C01683",
-        "TAD divergent - CC Brie Nangissienne": "C02476",
-        "TER Bourgogne - Franche-Comt\u00e9 Bus / SNCF": "C01855",
-        "TER Centre - Val de Loire Bus / SNCF": "C02369",
-        "TER Centre - Val-de-Loire Bus / SNCF": "C01858",
-        "TER Grand-Est Bus / SNCF": "C01854",
-        "TER Hauts-de-France Bus / SNCF": "C01862",
-        "TER Normandie Bus / SNCF": "C02371",
-        "TG / Cars Hourtoule": "C02175",
+        "TG / Francilit\u00e9 Saint-Quentin-en-Yvelines": "C02175",
         "TILLBUS / RATP": "C01331",
         "TIM / RATP": "C01352",
         "TRANSPORT URBAIN BONDYNOIS / RATP": "C01342",
         "TUC / RATP": "C01354",
         "TUVIM / RATP": "C01365",
         "TVM / RATP": "C01071",
         "Tzen1 / Transdev Senart": "C00859",
         "T\u00e0D 201/202 / Keolis Val d'Essonne Deux Vall\u00e9es": "C02496",
         "T\u00e0D 205 / Keolis Val d'Essonne Deux Vall\u00e9es": "C02495",
         "T\u00e0D 31 / Keolis V\u00e9lizy Vall\u00e9e de la Bi\u00e8vre": "C02485",
-        "T\u00e0D 43 / Transdev Brie et 2 Morin": "C02291",
         "T\u00e0D 52 / ProCars": "C02295",
         "T\u00e0D 6 / Transdev CEAT": "C02383",
         "T\u00e0D 78 / Transdev Boucle des Lys": "C02503",
         "T\u00e0D Coeur Essonne 1 / Keolis Meyer": "C02466",
         "T\u00e0D Coeur Essonne 2 / Keolis Meyer": "C02467",
         "T\u00e0D Coeur Essonne 5 / Keolis Meyer": "C02468",
         "T\u00e0D Courtaboeuf / RD Saclay": "C02493",
         "T\u00e0D Eaubonne Domont / Transdev Valmy": "C02422",
-        "T\u00e0D Saint-Fargeau / Transdev Melun": "C01895",
         "U / Autocars Dominique": "C02501",
         "U / SNCF": "C01840",
         "U / STRAV": "C00597",
         "V / Autocars Dominique": "C02502",
         "V / Cars Hourtoule": "C00422",
-        "V / Keolis Val d'Yerres Val de Seine": "C02386",
         "V / Transdev Melun": "C02276",
         "V2 / RATP": "C01361",
         "V3 / RATP": "C01359",
         "V4 / RATP": "C01347",
         "V5 / RATP": "C01362",
         "V6 / RATP": "C01367",
         "V7 / RATP": "C01363",
         "Vitavil / CIF": "C00261",
         "X / Keolis Val d'Yerres Val de Seine": "C00602",
         "X / RD Mantois": "C01612",
+        "X409 / Keolis Seine et Oise Est": "C00273",
+        "X419 / Keolis Seine et Oise Est": "C00114",
         "Y / Autocars Dominique": "C02498",
         "Z / Autocars Dominique": "C02499",
         "Z / RD Mantois": "C01604"
     },
     "funicular": {
         "FUNICULAIRE": "C01385"
     },
@@ -1911,25 +1895,20 @@
         "J": "C01739",
         "K": "C01738",
         "L": "C01740",
         "N": "C01736",
         "ORLYVAL": "C01388",
         "P": "C01730",
         "R": "C01731",
-        "TER Bourgogne - Franche-Comt\u00e9": "C01745",
-        "TER Centre - Val de Loire": "C01744",
-        "TER Centre - Val-de-Loire": "C01857",
-        "TER Grand-Est": "C01747",
-        "TER Hauts-de-France": "C01863",
-        "TER Normandie": "C02370",
         "U": "C01741"
     },
     "tram": {
         "T1": "C01389",
-        "T11 Express": "C01999",
+        "T10": "C02528",
+        "T11": "C01999",
         "T13": "C02344",
         "T2": "C01390",
         "T3a": "C01391",
         "T3b": "C01679",
         "T4": "C01843",
         "T5": "C01684",
         "T6": "C01794",
```

### Comparing `idfm_api-1.1.1/idfm_api/models.py` & `idfm_api-1.2.0/idfm_api/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,88 @@
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from functools import total_ordering
 from enum import Enum, unique
 
+
 @unique
 class TransportType(str, Enum):
     """
     Represents the type of transport
     """
+
     METRO = "metro"
     TRAM = "tram"
     TRAIN = "rail"
     BUS = "bus"
 
+
 @unique
 class TransportStatus(str, Enum):
     """
     Represents the status of a transport
     """
+
     ON_TIME = "onTime"
     MISSED = "missed"
     ARRIVED = "arrived"
     NOT_EXPECTED = "notExpected"
     DELAYED = "delayed"
     EARLY = "early"
     CANCELLED = "cancelled"
     NO_REPORT = "noReport"
     UNKNOWN = "unknown"
 
+
 @dataclass(frozen=True)
 class LineData:
     """
     Represents a line of a transport
     """
+
     name: str
     id: str
     type: TransportType
 
+
 @dataclass(frozen=True)
 class StopData:
     """
     Represents a stop area of a line
     """
+
     name: str
-    id: str
+    stop_id: str
     x: float
     y: float
     zip_code: str
     city: str
+    exchange_area_id: str
+    exchange_area_name: str
 
     @staticmethod
     def from_json(data: dict):
-        return StopData(name=data.get("name"), id=data.get("stop_id"), x=data.get("x"), y=data.get("y"), zip_code=data.get("zipCode"), city=data.get("city"))
+        return StopData(
+            name=data.get("name"),
+            stop_id=data.get("stop_id"),
+            x=data.get("x"),
+            y=data.get("y"),
+            zip_code=data.get("zipCode"),
+            city=data.get("city"),
+            exchange_area_id=data.get("exchange_area_id"),
+            exchange_area_name=data.get("exchange_area_name"),
+        )
+
 
 @dataclass(frozen=True)
 class InfoData:
     """
     Represents a traffic information fragment
     """
+
     id: str
     name: str
     message: str
     start_time: datetime
     end_time: datetime
     severity: int
     type: str
@@ -78,26 +99,32 @@
                     if i["MessageType"] == "SHORT_MESSAGE":
                         name = i["MessageText"]["value"]
 
         return InfoData(
             name=name,
             id=data.get("id"),
             message=message,
-            start_time=datetime.strptime(data.get("RecordedAtTime"), '%Y-%m-%dT%H:%M:%S.%fZ').replace(tzinfo=timezone.utc),
-            end_time=datetime.strptime(data.get("ValidUntilTime"), '%Y-%m-%dT%H:%M:%S.%fZ').replace(tzinfo=timezone.utc),
+            start_time=datetime.strptime(
+                data.get("RecordedAtTime"), "%Y-%m-%dT%H:%M:%S.%fZ"
+            ).replace(tzinfo=timezone.utc),
+            end_time=datetime.strptime(
+                data.get("ValidUntilTime"), "%Y-%m-%dT%H:%M:%S.%fZ"
+            ).replace(tzinfo=timezone.utc),
             type=data["InfoChannelRef"]["value"],
-            severity=data.get("InfoMessageVersion")
+            severity=data.get("InfoMessageVersion"),
         )
 
+
 @dataclass(frozen=True)
 @total_ordering
 class TrafficData:
     """
     Represents a schedule for a specific path
     """
+
     line_id: str
     note: str
     destination_name: str
     destination_id: str
     direction: str
     schedule: datetime
     retarted: bool
@@ -115,57 +142,96 @@
         try:
             note = data["MonitoredVehicleJourney"]["JourneyNote"][0]["value"]
         except (KeyError, IndexError):
             note = ""
 
         sch = None
         if "ExpectedArrivalTime" in data["MonitoredVehicleJourney"]["MonitoredCall"]:
-            sch = datetime.strptime(data["MonitoredVehicleJourney"]["MonitoredCall"]["ExpectedArrivalTime"], '%Y-%m-%dT%H:%M:%S.%fZ').replace(tzinfo=timezone.utc)
-        elif "ExpectedDepartureTime" in data["MonitoredVehicleJourney"]["MonitoredCall"]:
-            sch = datetime.strptime(data["MonitoredVehicleJourney"]["MonitoredCall"]["ExpectedDepartureTime"], '%Y-%m-%dT%H:%M:%S.%fZ').replace(tzinfo=timezone.utc)
+            sch = datetime.strptime(
+                data["MonitoredVehicleJourney"]["MonitoredCall"]["ExpectedArrivalTime"],
+                "%Y-%m-%dT%H:%M:%S.%fZ",
+            ).replace(tzinfo=timezone.utc)
+        elif (
+            "ExpectedDepartureTime" in data["MonitoredVehicleJourney"]["MonitoredCall"]
+        ):
+            sch = datetime.strptime(
+                data["MonitoredVehicleJourney"]["MonitoredCall"][
+                    "ExpectedDepartureTime"
+                ],
+                "%Y-%m-%dT%H:%M:%S.%fZ",
+            ).replace(tzinfo=timezone.utc)
         else:
             return None
 
         try:
             atstop = data["MonitoredVehicleJourney"]["MonitoredCall"]["VehicleAtStop"]
         except KeyError:
             atstop = None
 
         try:
-            plat = data["MonitoredVehicleJourney"]["MonitoredCall"]["ArrivalPlatformName"]["value"]
+            plat = data["MonitoredVehicleJourney"]["MonitoredCall"][
+                "ArrivalPlatformName"
+            ]["value"]
         except KeyError:
             plat = ""
 
-        if "ArrivalStatus" in data["MonitoredVehicleJourney"]["MonitoredCall"] and data["MonitoredVehicleJourney"]["MonitoredCall"]["ArrivalStatus"] != "":
-            status = TransportStatus(data["MonitoredVehicleJourney"]["MonitoredCall"]["ArrivalStatus"])
-        elif "DepartureStatus" in data["MonitoredVehicleJourney"]["MonitoredCall"] and data["MonitoredVehicleJourney"]["MonitoredCall"]["DepartureStatus"] != "":
-            status = TransportStatus(data["MonitoredVehicleJourney"]["MonitoredCall"]["DepartureStatus"])
+        if (
+            "ArrivalStatus" in data["MonitoredVehicleJourney"]["MonitoredCall"]
+            and data["MonitoredVehicleJourney"]["MonitoredCall"]["ArrivalStatus"] != ""
+        ):
+            status = TransportStatus(
+                data["MonitoredVehicleJourney"]["MonitoredCall"]["ArrivalStatus"]
+            )
+        elif (
+            "DepartureStatus" in data["MonitoredVehicleJourney"]["MonitoredCall"]
+            and data["MonitoredVehicleJourney"]["MonitoredCall"]["DepartureStatus"]
+            != ""
+        ):
+            status = TransportStatus(
+                data["MonitoredVehicleJourney"]["MonitoredCall"]["DepartureStatus"]
+            )
         else:
             status = TransportStatus.UNKNOWN
 
         return TrafficData(
             line_id=data["MonitoredVehicleJourney"]["LineRef"]["value"],
             note=note,
-            destination_name=data["MonitoredVehicleJourney"]["DestinationName"][0]["value"],
+            destination_name=data["MonitoredVehicleJourney"]["DestinationName"][0][
+                "value"
+            ],
             destination_id=data["MonitoredVehicleJourney"]["DestinationRef"]["value"],
             direction=dir,
             schedule=sch,
-            retarted=status not in [TransportStatus.ON_TIME, TransportStatus.ARRIVED, TransportStatus.UNKNOWN],
+            retarted=status
+            not in [
+                TransportStatus.ON_TIME,
+                TransportStatus.ARRIVED,
+                TransportStatus.UNKNOWN,
+            ],
             at_stop=atstop,
             platform=plat,
-            status=status
+            status=status,
         )
 
     def __eq__(self, other):
         if type(other) is TrafficData:
-            return self.schedule == other.schedule and self.line_id == other.line_id and self.destination_id == other.destination_id
+            return (
+                self.schedule == other.schedule
+                and self.line_id == other.line_id
+                and self.destination_id == other.destination_id
+            )
         else:
             return False
 
     def __lt__(self, other):
         if type(other) is datetime:
             return self.schedule < other
         elif type(other) is TrafficData:
-            return ((self.schedule is None or other.schedule is None) or self.schedule < other.schedule) or ((self.destination_name is None or other.destination_name is None) or self.destination_name < other.destination_name)
+            return (
+                (self.schedule is None or other.schedule is None)
+                or self.schedule < other.schedule
+            ) or (
+                (self.destination_name is None or other.destination_name is None)
+                or self.destination_name < other.destination_name
+            )
         else:
             return NotImplemented
-
```

### Comparing `idfm_api-1.1.1/idfm_api.egg-info/PKG-INFO` & `idfm_api-1.2.0/idfm_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idfm-api
-Version: 1.1.1
+Version: 1.2.0
 Summary: API for Ile de france mobilite
 Home-page: https://github.com/droso-hass/idfm-api
 Author: drosocode
 License: MIT
 Project-URL: Documentation, https://idfm-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/droso-hass/idfm-api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `idfm_api-1.1.1/setup.py` & `idfm_api-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 setup(
     name='idfm_api',
     packages=find_packages(include=['idfm_api']),
     package_data={
         'idfm_api': ['lines.json', 'stops.json'],
     },
-    version='1.1.1',
+    version='1.2.0',
     author='drosocode',
     license='MIT',
     description='API for Ile de france mobilite',
     url="https://github.com/droso-hass/idfm-api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

