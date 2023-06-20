# Comparing `tmp/animeworld-1.5.1.tar.gz` & `tmp/animeworld-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animeworld-1.5.1.tar", last modified: Tue Apr  4 19:31:32 2023, max compression
+gzip compressed data, was "animeworld-1.6.0.tar", last modified: Tue Jun 20 16:44:47 2023, max compression
```

## Comparing `animeworld-1.5.1.tar` & `animeworld-1.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:31:32.786422 animeworld-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-04 19:31:21.000000 animeworld-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-04 19:31:32.786422 animeworld-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-04 19:31:21.000000 animeworld-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:31:32.786422 animeworld-1.5.1/animeworld/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-04 19:31:21.000000 animeworld-1.5.1/animeworld/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-04 19:31:21.000000 animeworld-1.5.1/animeworld/anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-04 19:31:21.000000 animeworld-1.5.1/animeworld/episodio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-04 19:31:21.000000 animeworld-1.5.1/animeworld/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:31:32.786422 animeworld-1.5.1/animeworld/servers/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-04 19:31:21.000000 animeworld-1.5.1/animeworld/servers/AnimeWorld_Server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-04-04 19:31:21.000000 animeworld-1.5.1/animeworld/servers/Server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-04 19:31:21.000000 animeworld-1.5.1/animeworld/servers/Streamtape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-04 19:31:21.000000 animeworld-1.5.1/animeworld/servers/YouTube.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-04 19:31:21.000000 animeworld-1.5.1/animeworld/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-04 19:31:21.000000 animeworld-1.5.1/animeworld/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:31:32.786422 animeworld-1.5.1/animeworld.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-04 19:31:32.000000 animeworld-1.5.1/animeworld.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-04 19:31:32.000000 animeworld-1.5.1/animeworld.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:31:32.000000 animeworld-1.5.1/animeworld.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-04 19:31:32.000000 animeworld-1.5.1/animeworld.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 19:31:32.000000 animeworld-1.5.1/animeworld.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 19:31:32.786422 animeworld-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-04 19:31:21.000000 animeworld-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:44:47.884548 animeworld-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-20 16:44:39.000000 animeworld-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-20 16:44:47.884548 animeworld-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-20 16:44:39.000000 animeworld-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:44:47.884548 animeworld-1.6.0/animeworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/episodio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:44:47.884548 animeworld-1.6.0/animeworld/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/servers/AnimeWorld_Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/servers/Server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/servers/Streamtape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/servers/YouTube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-20 16:44:39.000000 animeworld-1.6.0/animeworld/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:44:47.884548 animeworld-1.6.0/animeworld.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-20 16:44:47.000000 animeworld-1.6.0/animeworld.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-20 16:44:47.000000 animeworld-1.6.0/animeworld.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:44:47.000000 animeworld-1.6.0/animeworld.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 16:44:47.000000 animeworld-1.6.0/animeworld.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 16:44:47.000000 animeworld-1.6.0/animeworld.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:44:47.884548 animeworld-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-20 16:44:39.000000 animeworld-1.6.0/setup.py
```

### Comparing `animeworld-1.5.1/LICENSE` & `animeworld-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `animeworld-1.5.1/PKG-INFO` & `animeworld-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animeworld
-Version: 1.5.1
+Version: 1.6.0
 Summary: AnimeWorld UNOFFICIAL API
 Home-page: https://github.com/MainKronos/AnimeWorld-API
 Author: MainKronos
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 ![Activity](https://img.shields.io/github/commit-activity/w/MainKronos/AnimeWorld-API) 
 ![Publish to PyPI](https://github.com/MainKronos/AnimeWorld-API/workflows/Publish%20to%20PyPI/badge.svg)
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/animeworld)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/animeworld)
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/animeworld)
 
-AnimeWorld-API is an unofficial library for [AnimeWorld](https://www.animeworld.tv/) (Italian anime site).
+AnimeWorld-API is an unofficial library for [AnimeWorld](https://www.animeworld.so/) (Italian anime site).
 
 ## Installazione
 Questa libreria richiede [Python 3.6](https://www.python.org/) o superiore.
 
 È Possibile installarare la libreria tramite pip:
 ```shell script
 pip install animeworld
@@ -42,22 +42,22 @@
 res = aw.find("No game no life")
 print(res)
 ```
 La funzione estituirà un dizionario contentente per chiave il nome dell'anime e per valore il link della pagina di animeworld.
 ```python
 {
 	'name': 'No Game no Life',
-	'link': 'https://www.animeworld.tv/play/no-game-no-life.IJUH1'
+	'link': 'https://www.animeworld.so/play/no-game-no-life.IJUH1'
 }
 ```
 È Possibile anche scaricare gli episodi di un anime.
 ```python
 import animeworld as aw
 
-anime = aw.Anime(link="https://www.animeworld.tv/play/danmachi-3.Ydt8-")
+anime = aw.Anime(link="https://www.animeworld.so/play/danmachi-3.Ydt8-")
 for episodio in anime.getEpisodes():
     print("Episodio Numero: ", episodio.number)
         
     if(episodio.download()):
         print("scaricato")
     else:
         print("errore")
```

### Comparing `animeworld-1.5.1/README.md` & `animeworld-1.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ![Activity](https://img.shields.io/github/commit-activity/w/MainKronos/AnimeWorld-API) 
 ![Publish to PyPI](https://github.com/MainKronos/AnimeWorld-API/workflows/Publish%20to%20PyPI/badge.svg)
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/animeworld)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/animeworld)
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/animeworld)
 
-AnimeWorld-API is an unofficial library for [AnimeWorld](https://www.animeworld.tv/) (Italian anime site).
+AnimeWorld-API is an unofficial library for [AnimeWorld](https://www.animeworld.so/) (Italian anime site).
 
 ## Installazione
 Questa libreria richiede [Python 3.6](https://www.python.org/) o superiore.
 
 È Possibile installarare la libreria tramite pip:
 ```shell script
 pip install animeworld
@@ -27,22 +27,22 @@
 res = aw.find("No game no life")
 print(res)
 ```
 La funzione estituirà un dizionario contentente per chiave il nome dell'anime e per valore il link della pagina di animeworld.
 ```python
 {
 	'name': 'No Game no Life',
-	'link': 'https://www.animeworld.tv/play/no-game-no-life.IJUH1'
+	'link': 'https://www.animeworld.so/play/no-game-no-life.IJUH1'
 }
 ```
 È Possibile anche scaricare gli episodi di un anime.
 ```python
 import animeworld as aw
 
-anime = aw.Anime(link="https://www.animeworld.tv/play/danmachi-3.Ydt8-")
+anime = aw.Anime(link="https://www.animeworld.so/play/danmachi-3.Ydt8-")
 for episodio in anime.getEpisodes():
     print("Episodio Numero: ", episodio.number)
         
     if(episodio.download()):
         print("scaricato")
     else:
         print("errore")
```

### Comparing `animeworld-1.5.1/animeworld/anime.py` & `animeworld-1.6.0/animeworld/anime.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Modulo contenente la struttura a classe dell'anime.
 """
-import requests
+import httpx
 from bs4 import BeautifulSoup
 import re
 import time
 from typing import *
 
 from .utility import HealthCheck, SES
 from .exceptions import Error404, AnimeNotAvailable
@@ -33,32 +33,34 @@
 		- `link`: Link dell'anime.
 		"""
 		self.link = link
 		self.html = self.__getHTML().content
 		self.__check404()
 
 	# Private
-	def __getHTML(self) -> requests.Response:
+	def __getHTML(self) -> httpx.Response:
 		"""
 		Ottiene la pagina web di Animeworld dell'anime e aggiorna i cookies.
 		
 		```
 		return Response # Risposta GET
 		```
 		"""
 		r = None
+		retry = 0
 		while True:
 			try:
-				r = SES.get(self.link, timeout=(3, 27), allow_redirects=True)
+				r = SES.get(self.link, timeout=(3, 27), follow_redirects=True)
 
-				if len(list(filter(re.compile(r'30[^2]').search, [str(x.status_code) for x in r.history]))): # se c'è un redirect strano
-					continue
-
-			except requests.exceptions.ReadTimeout:
-				time.sleep(1) # errore
+			except httpx.ReadTimeout as e:
+				if retry <= 2:
+					retry +=1
+					time.sleep(1) # errore
+				else:
+					raise e
 				
 			else:
 				break
 		r.raise_for_status()
 		return r
 	
 	# Private
@@ -73,15 +75,15 @@
 	def __getServer(self) -> Dict[int, Dict[str, str]]:
 		"""
 		Ottiene tutti i server in cui sono hostati gli episodi.
 
 		```
 		return {
 		  int: { # ID del server
-		    name: str # Nome del server
+			name: str # Nome del server
 		  },
 		  ...
 		}
 		```
 		"""
 		soupeddata = BeautifulSoup(self.html, "html.parser")
 		block = soupeddata.find("span", { "class" : "servers-tabs" })
@@ -170,38 +172,37 @@
 		```
 		"""
 		soupeddata = BeautifulSoup(self.html.decode('utf-8', 'ignore'), "html.parser")
 
 		a_link = soupeddata.select_one('li.episode > a')
 		if a_link is None: raise AnimeNotAvailable(self.getName())
 
-		self.link = "https://www.animeworld.tv" + a_link.get('href')
+		self.link = "https://www.animeworld.so" + a_link.get('href')
 
 		provLegacy = self.__getServer() # vecchio sistema di cattura server
 
-
 		raw_eps = {}
 		for provID in provLegacy:
 			prov_soup = soupeddata.select_one(f"div[class*='server'][data-name='{provID}']")
 
 			for data in prov_soup.select('li.episode > a'):
 				epNum = data.get('data-episode-num')
 				epID = data.get('data-episode-id')
 
 				if epID not in raw_eps:
 					raw_eps[epID] = {
 						'number': epNum,
-						'link': f"https://www.animeworld.tv/api/download/{epID}",
+						'link': f"https://www.animeworld.so/api/download/{epID}",
 						'legacy': [{
 							"id": int(provID),
 							"name": provLegacy[provID]["name"],
-							"link": "https://www.animeworld.tv" + data.get("href")
+							"link": "https://www.animeworld.so" + data.get("href")
 						}]
 					}
 				else:
 					raw_eps[epID]['legacy'].append({
 					"id": int(provID),
 					"name": provLegacy[provID]["name"],
-					"link": "https://www.animeworld.tv" + data.get("href")
+					"link": "https://www.animeworld.so" + data.get("href")
 				})
 
 		return [Episodio(x['number'], x['link'], x['legacy']) for x in list(raw_eps.values())]
```

### Comparing `animeworld-1.5.1/animeworld/episodio.py` & `animeworld-1.6.0/animeworld/episodio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Modulo contenente la struttura a classe degli episodi.
 """
-import requests
+import httpx
 from bs4 import BeautifulSoup
 from typing import *
 import time
 
 from .utility import SES
 from .exceptions import ServerNotSupported
 from .servers import Server, AnimeWorld_Server, YouTube, Streamtape
@@ -23,14 +23,15 @@
 	"""
 
 	def __init__(self, number: str, link: str, legacy: List[Dict] = []):
 		"""
 		- `number`: Numero dell'episodio.
 		- `link`: Link dell'endpoint dell'episodio.
 		- `legacy`: Lista di tutti i link dei server in cui sono hostati gli episodi.
+		- `csrf_token`: Token per le chiamate api.
 		"""
 		self.number = number 
 		"""Numero dell'episodio."""
 		self.__link = link
 		"""Link dell'endpoint dell'episodio."""
 		self.__legacy = legacy
 		"""Lista di tutti i link dei server in cui sono hostati gli episodi."""
@@ -44,16 +45,15 @@
 		return [
 		  Server, # Classe Server
 		  ...
 		]
 		```
 		"""
 		tmp = [] # tutti i links
-
-		res = SES.post(self.__link, timeout=(3, 27))
+		res = SES.post(self.__link, timeout=(3, 27), follow_redirects=True)
 		data = res.json()
 
 		for provID in data["links"]:
 			key = [x for x in data["links"][provID].keys() if x != 'server'][0]
 			tmp.append({
 				"id": int(provID),
 				"name": data["links"][provID]["server"]["name"],
@@ -86,15 +86,15 @@
 		info = ""
 		err = None
 		for server in self.links:
 			try:
 				info = server.fileInfo()
 			except ServerNotSupported:
 				pass
-			except requests.exceptions.RequestException as exc:
+			except httpx.HTTPError as exc:
 				err = exc
 			else:
 				return info
 
 		raise err
 
 	def download(self, title: Optional[str]=None, folder: str='', *, hook: Callable[[Dict], None]=lambda *args:None, opt: List[str]=[]) -> Optional[str]: # Scarica l'episodio con il primo link nella lista
@@ -172,18 +172,18 @@
 		} for x in servers]
 
 		max_time = 0.5 # numero di secondi massimo
 
 		for test in speed_test:
 			try:
 				start = time.perf_counter()
-				with SES.get(test["server"].fileLink(), stream = True, timeout=0.9) as r:
-					for chunk in r.iter_content(chunk_size = 2048):
+				with SES.stream("GET", test["server"].fileLink(), timeout=0.9, follow_redirects=True) as r:
+					for chunk in r.iter_bytes(chunk_size = 2048):
 						if time.perf_counter() - start > max_time: break
 						test["bytes"] += len(chunk)
-			except (ServerNotSupported, requests.exceptions.RequestException):
+			except (ServerNotSupported, httpx.HTTPError):
 				continue
 		
 		speed_test = [x for x in speed_test if x["bytes"] != -1] # tolgo tutti i server che hanno generato un eccezione
 		if len(speed_test) == 0: return servers[0] # ritorno al caso standard
 
 		return max(speed_test, key=lambda x: x["bytes"])["server"] # restituisco il server che ha scaricato più byte in `max_time` secondi
```

### Comparing `animeworld-1.5.1/animeworld/exceptions.py` & `animeworld-1.6.0/animeworld/exceptions.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.5.1/animeworld/servers/AnimeWorld_Server.py` & `animeworld-1.6.0/animeworld/servers/AnimeWorld_Server.py`

 * *Files identical despite different names*

### Comparing `animeworld-1.5.1/animeworld/servers/Server.py` & `animeworld-1.6.0/animeworld/servers/Server.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,29 +84,29 @@
 		```
 		"""
 
 		raise ServerNotSupported(self.name)
 	
 	def _fileInfoIn(self) -> Dict[str,str]:
 		"""
-		Recupera le informazioni del file dell'episodio usando requests.
+		Recupera le informazioni del file dell'episodio usando httpx.
 		"""
 		url = self.fileLink()
 
-		with SES.head(url) as r:
-			r.raise_for_status()
+		r = SES.head(url)
+		r.raise_for_status()
 
-			return {
-				"content_type": r.headers['content-type'],
-				"total_bytes": int(r.headers['Content-Length']),
-				"last_modified": datetime.strptime(r.headers['Last-Modified'], "%a, %d %b %Y %H:%M:%S %Z"),
-				"server_name": self.name,
-				"server_id": self.Nid,
-				"url": url
-			}
+		return {
+			"content_type": r.headers['content-type'],
+			"total_bytes": int(r.headers['Content-Length']),
+			"last_modified": datetime.strptime(r.headers['Last-Modified'], "%a, %d %b %Y %H:%M:%S %Z"),
+			"server_name": self.name,
+			"server_id": self.Nid,
+			"url": url
+		}
 	
 	def _fileInfoEx(self) -> Dict[str,str]:
 		"""
 		Recupera le informazioni del file dell'episodio usando yutube_dl.
 		"""
 
 		class MyLogger(object):
@@ -158,15 +158,15 @@
 		"""
 		raise ServerNotSupported(self.name)
 
 	# Protected
 	def _downloadIn(self, title: str, folder: str, *, hook: Callable[[Dict], None], opt: List[str]) -> Optional[str]: # Scarica l'episodio
 
 		"""
-		Scarica il file utilizzando requests.
+		Scarica il file utilizzando httpx.
 
 		- `title`: Nome con cui verrà nominato il file scaricato.
 		- `folder`: Posizione in cui verrà spostato il file scaricato.
 		- `hook`: Funzione che viene richiamata varie volte durante il download; la funzione riceve come argomento un dizionario con le seguenti chiavi: 
 		  - `total_bytes`: Byte totali da scaricare.
 		  - `downloaded_bytes`: Byte attualmente scaricati.
 		  - `percentage`: Percentuale del progresso di download.
@@ -178,28 +178,28 @@
 		- `opt`: Lista per delle opzioni aggiuntive.
 		  - `'abort'`: Ferma forzatamente il download.
 
 		```
 		return str # File scaricato
 		```
 		"""
-		with SES.get(self.fileLink(), stream = True) as r:
+		with SES.stream("GET", self.fileLink(), follow_redirects=True) as r:
 			r.raise_for_status()
 			ext = r.headers['content-type'].split('/')[-1]
 			if ext == 'octet-stream': ext = 'mp4'
 			file = f"{title}.{ext}"
 
 			total_length = int(r.headers.get('content-length'))
 			current_lenght = 0
 			start = time.time()
 			step = time.time()
 
 			try:
 				with open(f"{os.path.join(folder,file)}", 'wb') as f:
-					for chunk in r.iter_content(chunk_size = 524288):
+					for chunk in r.iter_bytes(chunk_size = 524288):
 						if chunk: 
 							f.write(chunk)
 							f.flush()
 							
 							current_lenght += len(chunk)
 
 							hook({
```

### Comparing `animeworld-1.5.1/animeworld/servers/Streamtape.py` & `animeworld-1.6.0/animeworld/servers/Streamtape.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 		Recupera il link diretto per il download del file dell'episodio.
 
 		```
 		return str # Link del file
 		```
 		"""
 		
-		sb_get = SES.get(self.link, allow_redirects=False)
+		sb_get = SES.get(self.link)
 
 		if sb_get.status_code == 200:
 			soupeddata = BeautifulSoup(sb_get.content, "html.parser")
 
 			raw_link = re.search(r"document\.getElementById\('ideoooolink'\)\.innerHTML = (\".*'\))", soupeddata.prettify()).group(1)
 
 			raw_link = raw_link.replace('"', '').replace("'", "").replace('+', '')
```

### Comparing `animeworld-1.5.1/animeworld/servers/YouTube.py` & `animeworld-1.6.0/animeworld/servers/YouTube.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 		```
 		return str # Link del file
 		```
 		"""
 		
 		anime_id = self.link.split("/")[-1]
-		external_link = "https://www.animeworld.tv/api/episode/serverPlayerAnimeWorld?id={}".format(anime_id)
+		external_link = "https://www.animeworld.so/api/episode/serverPlayerAnimeWorld?id={}".format(anime_id)
 
 		sb_get = SES.get(self.link)
 		sb_get.raise_for_status()
 
 		sb_get = SES.get(external_link)
 		soupeddata = BeautifulSoup(sb_get.content, "html.parser")
 		sb_get.raise_for_status()
```

### Comparing `animeworld-1.5.1/animeworld/utility.py` & `animeworld-1.6.0/animeworld/utility.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,38 @@
 """
 Modulo per delle funzioni di utilità.
 """
-import requests
+import httpx
 from bs4 import BeautifulSoup
 import inspect
 from typing import *
 import re
 
 from datetime import datetime
 import time
 import locale
 
 from .exceptions import DeprecatedLibrary
 
-class MySession(requests.Session):
+class MySession(httpx.Client):
 	"""
-	Sessione requests.
+	Sessione httpx.
 	"""
 	def __init__(self) -> None:
-		super().__init__()
+		super().__init__(http2=True)
 		self.headers.update({'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.88 Safari/537.36'})
 		self.fixCookie()
 	
 	def fixCookie(self):
-		SecurityAW = re.compile(br'document\.cookie="SecurityAW=(.+) ;')
-		csrf_token = re.compile(br'<meta.*?id="csrf-token"\s*?content="(.*?)">')
-
-		for _ in range(2): # numero di tentativi
-			res = self.get("https://www.animeworld.tv")
+		"""Aggiunge il csrf_token all'headers."""
 
-			m = SecurityAW.search(res.content)
-			if m:
-				self.cookies.update({'SecurityAW': m.group(1).decode('utf-8')})
-				continue
-			
-			m = csrf_token.search(res.content)
-			if m:
-				self.headers.update({'csrf-token': m.group(1).decode('utf-8')})
-				break
-		else:
-			frame = inspect.getframeinfo(inspect.currentframe())
-			raise DeprecatedLibrary(frame.filename, frame.function, frame.lineno)
+		res = self.get("https://www.animeworld.so", follow_redirects=True)
+		csrf_token = re.compile(br'<meta.*?id="csrf-token"\s*?content="(.*?)">')
+		m = csrf_token.search(res.content)
+		self.headers.update({'csrf-token': m.group(1).decode('utf-8')})
 
 
 def HealthCheck(fun):
 	"""
 	Controlla se la libreria è deprecata
 	"""
 	def wrapper(*args, **kwargs):
@@ -74,74 +62,73 @@
 	Ricerca un anime tramite le API interne di Animeworld.
 
 	- `keyword`: Il nome dell'anime o una porzione di esso.
 
 	```
 	return [
 	  {
-	    "id": int, # ID interno di AnimeWorld
-	    "name": str, # Nome dell'anime
-	    "jtitle": str, # Nome giapponese (con caratteri latini)
-	    "studio": str, # Studio dell'anime
-	    "release": datetime, # Giorno, Mese e Anno della release dell'anime
-	    "episodes": int, # Numero di episodi
-	    "state": str, # Es. "0", "1", ...
-	    "story": str, # Trama dell'anime
-	    "categories": List[dict], # Es. [{"id": int, "name": str, "slug": str, "description": str}]
-	    "image": str, # Link dell'immagine di copertina
-	    "durationEpisodes": str, # Durata episodio
-	    "link": str, # Link dell'anime
-	    "createdAt": str, # Es. "2021-10-24T18:29:34.000Z"
-	    "language": str, # Es. "jp
-	    "year": str, # Anno di rilascio dell'anime
-	    "dub": bool, # Se è doppiato o meno
-	    "season": str, # Es. "winter"
-	    "totViews": int, # Numero totale di visite alla pagina AnimeWolrd
-	    "dayViews": int, # Numero giornaliero di visite alla pagina AnimeWolrd
-	    "weekViews": int, # Numero settimanale di visite alla pagina AnimeWolrd
-	    "monthViews": int, # Numero mensile di visite alla pagina AnimeWolrd
-	    "malId": int, # ID di MyAnimeList dell'anime
-	    "anilistId": int, # ID di AniList dell'anime
-	    "mangaworldId": int, # ID di MangaWorld dell'anime
-	    "malVote": float, # Valutazione di MyanimeList
-	    "trailer": str # Link del trailer dell'anime
+		"id": int, # ID interno di AnimeWorld
+		"name": str, # Nome dell'anime
+		"jtitle": str, # Nome giapponese (con caratteri latini)
+		"studio": str, # Studio dell'anime
+		"release": datetime, # Giorno, Mese e Anno della release dell'anime
+		"episodes": int, # Numero di episodi
+		"state": str, # Es. "0", "1", ...
+		"story": str, # Trama dell'anime
+		"categories": List[dict], # Es. [{"id": int, "name": str, "slug": str, "description": str}]
+		"image": str, # Link dell'immagine di copertina
+		"durationEpisodes": str, # Durata episodio
+		"link": str, # Link dell'anime
+		"createdAt": str, # Es. "2021-10-24T18:29:34.000Z"
+		"language": str, # Es. "jp
+		"year": str, # Anno di rilascio dell'anime
+		"dub": bool, # Se è doppiato o meno
+		"season": str, # Es. "winter"
+		"totViews": int, # Numero totale di visite alla pagina AnimeWolrd
+		"dayViews": int, # Numero giornaliero di visite alla pagina AnimeWolrd
+		"weekViews": int, # Numero settimanale di visite alla pagina AnimeWolrd
+		"monthViews": int, # Numero mensile di visite alla pagina AnimeWolrd
+		"malId": int, # ID di MyAnimeList dell'anime
+		"anilistId": int, # ID di AniList dell'anime
+		"mangaworldId": int, # ID di MangaWorld dell'anime
+		"malVote": float, # Valutazione di MyanimeList
+		"trailer": str # Link del trailer dell'anime
 	  }
 	]
 	```
 	"""
 
 	locale.setlocale(locale.LC_TIME, "it_IT.UTF-8")
-	res = SES.post("https://www.animeworld.tv/api/search/v2?", params = {"keyword": keyword})
+	res = SES.post("https://www.animeworld.so/api/search/v2?", params = {"keyword": keyword}, follow_redirects=True)
 
 	data = res.json()
 	if "error" in data: return []
 	data = data["animes"]
 
 	for elem in data:
 		for k in elem:
 			if elem[k] == "??":
 				elem[k] = None
 
 	data.sort(key=lambda a: a["dub"])
 
-
 	return [
 		{
 		"id": elem["id"],
 		"name": elem["name"],
 		"jtitle": elem["jtitle"],
 		"studio": elem["studio"],
 		"release": datetime.strptime(elem["release"], "%d %B %Y") if elem["release"] is not None else None,
 		"episodes": int(elem["episodes"]) if elem["episodes"] is not None else None,
 		"state": elem["state"],
 		"story": elem["story"],
 		"categories": elem["categories"],
 		"image": elem["image"],
 		"durationEpisodes": elem["durationEpisodes"],
-		"link": f"https://www.animeworld.tv/play/{elem['link']}.{elem['identifier']}" if elem['link'] is not None or elem['identifier'] is not None else None,
+		"link": f"https://www.animeworld.so/play/{elem['link']}.{elem['identifier']}" if elem['link'] is not None or elem['identifier'] is not None else None,
 		"createdAt": elem["createdAt"],
 		"language": elem["language"],
 		"year": elem["year"],
 		"dub": elem["dub"] != "0" if elem["dub"] is not None else None,
 		"season": elem["season"],
 		"totViews": elem["totViews"],
 		"dayViews": elem["dayViews"],
@@ -152,8 +139,8 @@
 		"mangaworldId": elem["mangaworldId"],
 		"malVote": elem["malVote"],
 		"trailer": elem["trailer"]
 		}for elem in data
 	]
 
 SES = MySession() # sessione contenente Cookie e headers
-"Sessione requests."
+"Sessione httpx."
```

### Comparing `animeworld-1.5.1/animeworld.egg-info/PKG-INFO` & `animeworld-1.6.0/animeworld.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animeworld
-Version: 1.5.1
+Version: 1.6.0
 Summary: AnimeWorld UNOFFICIAL API
 Home-page: https://github.com/MainKronos/AnimeWorld-API
 Author: MainKronos
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 ![Activity](https://img.shields.io/github/commit-activity/w/MainKronos/AnimeWorld-API) 
 ![Publish to PyPI](https://github.com/MainKronos/AnimeWorld-API/workflows/Publish%20to%20PyPI/badge.svg)
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/animeworld)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/animeworld)
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/animeworld)
 
-AnimeWorld-API is an unofficial library for [AnimeWorld](https://www.animeworld.tv/) (Italian anime site).
+AnimeWorld-API is an unofficial library for [AnimeWorld](https://www.animeworld.so/) (Italian anime site).
 
 ## Installazione
 Questa libreria richiede [Python 3.6](https://www.python.org/) o superiore.
 
 È Possibile installarare la libreria tramite pip:
 ```shell script
 pip install animeworld
@@ -42,22 +42,22 @@
 res = aw.find("No game no life")
 print(res)
 ```
 La funzione estituirà un dizionario contentente per chiave il nome dell'anime e per valore il link della pagina di animeworld.
 ```python
 {
 	'name': 'No Game no Life',
-	'link': 'https://www.animeworld.tv/play/no-game-no-life.IJUH1'
+	'link': 'https://www.animeworld.so/play/no-game-no-life.IJUH1'
 }
 ```
 È Possibile anche scaricare gli episodi di un anime.
 ```python
 import animeworld as aw
 
-anime = aw.Anime(link="https://www.animeworld.tv/play/danmachi-3.Ydt8-")
+anime = aw.Anime(link="https://www.animeworld.so/play/danmachi-3.Ydt8-")
 for episodio in anime.getEpisodes():
     print("Episodio Numero: ", episodio.number)
         
     if(episodio.download()):
         print("scaricato")
     else:
         print("errore")
```

### Comparing `animeworld-1.5.1/setup.py` & `animeworld-1.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="animeworld",
-    version="1.5.1",
+    version="1.6.0",
     author="MainKronos",
     description="AnimeWorld UNOFFICIAL API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MainKronos/AnimeWorld-API",
     packages=setuptools.find_packages(),
-    install_requires=['requests', 'youtube_dl', 'beautifulsoup4'],
+    install_requires=['httpx', 'youtube_dl', 'beautifulsoup4'],
 	license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
 		"Topic :: Utilities",
     ],
```

