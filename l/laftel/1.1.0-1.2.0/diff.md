# Comparing `tmp/laftel-1.1.0-py3-none-any.whl.zip` & `tmp/laftel-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 17222 bytes, number of entries: 9
--rw-r--r--  2.0 unx      125 b- defN 21-Jul-29 06:35 laftel/__init__.py
--rw-r--r--  2.0 unx     1244 b- defN 21-Jul-29 07:10 laftel/laftel.py
--rw-r--r--  2.0 unx     3387 b- defN 21-Jul-29 07:09 laftel/models.py
--rw-r--r--  2.0 unx      256 b- defN 21-May-27 04:15 laftel/utils.py
--rw-r--r--  2.0 unx    35149 b- defN 21-Jul-29 07:12 laftel-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3716 b- defN 21-Jul-29 07:12 laftel-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jul-29 07:12 laftel-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 21-Jul-29 07:12 laftel-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      672 b- defN 21-Jul-29 07:12 laftel-1.1.0.dist-info/RECORD
-9 files, 44648 bytes uncompressed, 16078 bytes compressed:  64.0%
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-19 23:35 laftel/__init__.py
+-rw-r--r--  2.0 unx     1244 b- defN 23-Jun-19 23:34 laftel/laftel.py
+-rw-r--r--  2.0 unx     3387 b- defN 21-Aug-11 17:16 laftel/models.py
+-rw-r--r--  2.0 unx      256 b- defN 23-Jun-19 23:35 laftel/utils.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-19 23:35 laftel-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3718 b- defN 23-Jun-19 23:35 laftel-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 23:35 laftel-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-19 23:35 laftel-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      672 b- defN 23-Jun-19 23:35 laftel-1.2.0.dist-info/RECORD
+9 files, 44650 bytes uncompressed, 16078 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: laftel/models.py
 Comment: 
 
 Filename: laftel/utils.py
 Comment: 
 
-Filename: laftel-1.1.0.dist-info/LICENSE
+Filename: laftel-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: laftel-1.1.0.dist-info/METADATA
+Filename: laftel-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: laftel-1.1.0.dist-info/WHEEL
+Filename: laftel-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: laftel-1.1.0.dist-info/top_level.txt
+Filename: laftel-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: laftel-1.1.0.dist-info/RECORD
+Filename: laftel-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## laftel/__init__.py

```diff
@@ -1,4 +1,4 @@
 from .laftel import getAnimeInfo, searchAnime, sync
 
 __all__ = ["sync", "searchAnime", "getAnimeInfo"]
-__version__ = "1.1.0"
+__version__ = "1.2.0"
```

## laftel/laftel.py

```diff
@@ -1,16 +1,16 @@
 from .models import AnimeInfo, SearchResult
 from .utils import api_request
 from typing import List
 import asyncio
 
 
 class ApiUrl:
-    AnimeItem = "https://laftel.net/api/items/v1/{id}/"
-    SearchAnime = "https://laftel.net/api/search/v1/keyword/?keyword={query}"
+    AnimeItem = "https://laftel.net/api/items/v2/{id}/"
+    SearchAnime = "https://laftel.net/api/search/v3/keyword/?keyword={query}"
 
 
 async def getAnimeInfo(id: int) -> AnimeInfo:
     return AnimeInfo(await api_request(ApiUrl.AnimeItem.format(id=id)))
 
 
 async def searchAnime(query: str, issync: bool = False) -> List[SearchResult]:
```

## Comparing `laftel-1.1.0.dist-info/LICENSE` & `laftel-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `laftel-1.1.0.dist-info/METADATA` & `laftel-1.2.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: laftel
-Version: 1.1.0
+Version: 1.2.0
 Summary: 파이썬 라프텔 라이브러리, Unofficial Python Laftel API Wrapper(Laftel)
 Home-page: https://github.com/331leo/laftel
+Download-URL: https://github.com/331leo/laftel
 Author: LeoK
 Author-email: support@leok.kr
 License: GPL-V3
-Download-URL: https://github.com/331leo/laftel
 Keywords: anime,laftel,info,API,wrapper
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: aiohttp
 
 <h3 align="center"> <img src="https://asset.laftel.net/static/media/purple.e17b0b50.svg" alt="img" width="30" height=""> Laftel <img src="https://asset.laftel.net/static/media/purple.e17b0b50.svg" alt="img" width="30" height=""> </h3>
 
 <h6 align="center">Unofficial Python Laftel.net API Wrapper</h6>
 
 <div align="center" id="badges"> <img src="https://img.shields.io/pypi/pyversions/laftel?color=816BFF&style=flat-square"> <img src="https://img.shields.io/pypi/v/laftel?color=816BFF&label=laftel&logo=python&logoColor=816BFF&style=flat-square"> <img src="https://img.shields.io/pypi/l/laftel?color=816BFF&logo=gnu&logoColor=816BFF&style=flat-square"> <img src="https://img.shields.io/pypi/dm/laftel?color=816BFF&style=flat-square"> <img src="https://img.shields.io/pypi/status/laftel?color=816BFF&style=flat-square">  </div>
@@ -91,9 +91,7 @@
     view_male: int  # Percentage of male in total watched user (남성 시청자 비율)
     view_female: int  # Percentage of woman in total watched user (여성 시청자 비율)
 ```
 
 ## Example
 
 [View example.py](example.py)
-
-
```

## Comparing `laftel-1.1.0.dist-info/RECORD` & `laftel-1.2.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-laftel/__init__.py,sha256=YUDxOXZm1ds_6tYFkefS2aAjMPgZ1A7_UcfHf6uWkOk,125
-laftel/laftel.py,sha256=BeCVHckVv1E5f6wXIdMRRTaLFzkH_37yC_l1Xa97lk0,1244
+laftel/__init__.py,sha256=teom9GtPUC8_ya5zGVSYb4Hb9c7Zey1wdDndmcCNNQs,125
+laftel/laftel.py,sha256=2ZKamKaPhM2wyp0QwlSebGqP2521D4TrsXHSuJFgZkw,1244
 laftel/models.py,sha256=3Jmrt9McJ8GvPrs1KX0VlzH01nqJm-_WDOdE_fJNy54,3387
 laftel/utils.py,sha256=8zILW3kNwx5OHyn8o3SCUX7zrhVgY0CuJp2YY0vRZ0c,256
-laftel-1.1.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-laftel-1.1.0.dist-info/METADATA,sha256=xiSf2HLvS9GCwJmN_-xpyKZ9SCRYLJg2swZu1_FvJ10,3716
-laftel-1.1.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-laftel-1.1.0.dist-info/top_level.txt,sha256=IUcersvf4Rhh-A_UDhhUoRJpPOraZNfYssiQtH3Yv7Q,7
-laftel-1.1.0.dist-info/RECORD,,
+laftel-1.2.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+laftel-1.2.0.dist-info/METADATA,sha256=E72MnQqzI5BVevaE8O1hwBSJesvYtn-0HAvzo9jq4aw,3718
+laftel-1.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+laftel-1.2.0.dist-info/top_level.txt,sha256=IUcersvf4Rhh-A_UDhhUoRJpPOraZNfYssiQtH3Yv7Q,7
+laftel-1.2.0.dist-info/RECORD,,
```

