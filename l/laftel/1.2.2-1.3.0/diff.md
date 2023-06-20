# Comparing `tmp/laftel-1.2.2-py3-none-any.whl.zip` & `tmp/laftel-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17401 bytes, number of entries: 9
--rw-r--r--  2.0 unx      125 b- defN 23-Jun-20 00:36 laftel/__init__.py
--rw-r--r--  2.0 unx     1739 b- defN 23-Jun-20 00:33 laftel/laftel.py
--rw-r--r--  2.0 unx     3314 b- defN 23-Jun-20 00:36 laftel/models.py
--rw-r--r--  2.0 unx      256 b- defN 23-Jun-20 00:24 laftel/utils.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jun-20 00:36 laftel-1.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3965 b- defN 23-Jun-20 00:36 laftel-1.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 00:36 laftel-1.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-20 00:36 laftel-1.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      672 b- defN 23-Jun-20 00:36 laftel-1.2.2.dist-info/RECORD
-9 files, 45319 bytes uncompressed, 16257 bytes compressed:  64.1%
+Zip file size: 17949 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      189 b- defN 23-Jun-20 06:04 laftel/__init__.py
+-rw-r--r--  2.0 unx     2258 b- defN 23-Jun-20 00:55 laftel/laftel.py
+-rw-r--r--  2.0 unx     4486 b- defN 23-Jun-20 02:30 laftel/models.py
+-rw-r--r--  2.0 unx      460 b- defN 23-Jun-20 06:04 laftel/utils.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-20 06:04 laftel-1.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3965 b- defN 23-Jun-20 06:04 laftel-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 06:04 laftel-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-20 06:04 laftel-1.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      672 b- defN 23-Jun-20 06:04 laftel-1.3.0.dist-info/RECORD
+9 files, 47278 bytes uncompressed, 16805 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: laftel/models.py
 Comment: 
 
 Filename: laftel/utils.py
 Comment: 
 
-Filename: laftel-1.2.2.dist-info/LICENSE
+Filename: laftel-1.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: laftel-1.2.2.dist-info/METADATA
+Filename: laftel-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: laftel-1.2.2.dist-info/WHEEL
+Filename: laftel-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: laftel-1.2.2.dist-info/top_level.txt
+Filename: laftel-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: laftel-1.2.2.dist-info/RECORD
+Filename: laftel-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## laftel/__init__.py

```diff
@@ -1,4 +1,4 @@
-from .laftel import getAnimeInfo, searchAnime, sync
+from .laftel import getAnimeInfo, searchAnime, searchSeries, searchEpisodes, sync
 
-__all__ = ["sync", "searchAnime", "getAnimeInfo"]
-__version__ = "1.2.2"
+__all__ = ["sync", "searchAnime", "getAnimeInfo", "searchSeries", "searchEpisodes"]
+__version__ = "1.3.0"
```

## laftel/laftel.py

```diff
@@ -1,17 +1,18 @@
-from .models import AnimeInfo, SearchResult, SeriesSearchResult
+from .models import AnimeInfo, SearchEpisode, SearchResult, SeriesSearchResult
 from .utils import api_request
 from typing import List
 import asyncio
 
 
 class ApiUrl:
     AnimeItem = "https://laftel.net/api/items/v2/{id}/"
     SearchAnime = "https://laftel.net/api/search/v3/keyword/?keyword={query}"
     SearchSeries = "https://laftel.net/api/items/v2/series/{id}/?limit=50&offset=0"
+    SearchEpisodes = "https://laftel.net/api/episodes/v2/list/?item_id={id}&sort=oldest&limit=50&show_playback_offset=true&offset=0"
 
 
 async def getAnimeInfo(id: int) -> AnimeInfo:
     return AnimeInfo(await api_request(ApiUrl.AnimeItem.format(id=id)))
 
 
 async def searchSeries(id: int) -> List[SeriesSearchResult]:
@@ -39,18 +40,30 @@
 
         obj.get_data = get_data
 
         return_list.append(obj)
     return return_list
 
 
+async def searchEpisodes(id: int) -> List[SearchEpisode]:
+    return [
+        SearchEpisode(data)
+        for data in (await api_request(ApiUrl.SearchEpisodes.format(id=id))).get(
+            "results"
+        )
+    ]
+
+
 class sync:
     def getAnimeInfo(id: int, loop=asyncio.get_event_loop()) -> AnimeInfo:
         return loop.run_until_complete(getAnimeInfo(id))
 
     def searchAnime(query: str, loop=asyncio.get_event_loop()) -> List[SearchResult]:
         return loop.run_until_complete(searchAnime(query=query, issync=True))
 
     def searchSeries(
         id: int, loop=asyncio.get_event_loop()
     ) -> List[SeriesSearchResult]:
         return loop.run_until_complete(searchSeries(id=id))
+
+    def searchEpisodes(id: int, loop=asyncio.get_event_loop()) -> List[SearchEpisode]:
+        return loop.run_until_complete(searchEpisodes(id=id))
```

## laftel/models.py

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
 from typing import Callable, List, Optional
 
 
-@dataclass(repr=True)
 class AnimeInfo:
     id: int  # Anime ID (애니 아이디)
     name: str  # Anime Title (애니 제목)
     url: str  # Anime Link (애니 링크)
     image: str  # Cover image URL (커버 사진 URL)
     content: str  # Summary of anime (애니 줄거리)
     ended: bool  # Anime complete or not (애니 완결 여부)
@@ -14,20 +13,20 @@
 
     content_rating: str  # Content Rating in korean (콘텐츠 등급 - 00세 이용가)
     adultonly: bool  # Adult Content (성인인증 필요 여부)
     viewable: bool  # Available in Laftel (라프텔 시청 가능 여부)
     genres: List[str]  # Genres in korean string (장르 태그 목록)
     tags: List[str]  # Anime tags from Laftel (라프텔이 붙인 태그)
 
-    air_year_quarter: str  # Airing quarter (방영분기 - 2020년 1분기)
-    air_day: str  # Airing day (방영 요일)
+    air_year_quarter: Optional[str]  # Airing quarter (방영분기 - 2020년 1분기)
+    air_day: Optional[str]  # Airing day (방영 요일)
     avg_rating: float  # Average User Rating out of 5 (5점 만점 중 평균 별점)
 
     series_id: Optional[int]  # Series ID (시리즈 아이디)
-    production: str  # Production company (제작사)
+    production: Optional[str]  # Production company (제작사)
 
     def __init__(self, data):
         self.id = data.get("id")
         self.name = data.get("name")
         self.url = f"https://laftel.net/item/{self.id}"
         self.image = data.get("img")
         self.content = data.get("content")
@@ -41,15 +40,15 @@
         self.tags = data.get("tags")
 
         self.air_year_quarter = data.get("air_year_quarter", "")
         self.air_day = data.get("distributed_air_time", "")
 
         self.avg_rating = data.get("avg_rating")
 
-        self.series_id = data.get("series_id")
+        self.series_id = data.get("series_id", None)
         self.production = data.get("production", "")
 
 
 @dataclass(repr=True)
 class SearchResult:
     id: int  # Anime ID (애니 아이디)
     name: str  # Anime Title (애니 제목)
@@ -81,7 +80,33 @@
 class SeriesSearchResult:
     id: int  # Anime ID (애니 아이디)
     name: str  # Anime Title (애니 제목)
 
     def __init__(self, data):
         self.id = data.get("id")
         self.name = data.get("name")
+
+
+@dataclass(repr=True)
+class SearchEpisode:
+    id: str  # Episode ID (에피소드 아이디)
+    title: str  # Anime Title (애니 제목)
+    subject: str  # Episode Title (에피소드 제목)
+    description: str  # Episode Description (에피소드 설명)
+    episode_num: str  # Episode Number (에피소드 번호)
+    episode_order: int  # Episode Order (에피소드 순서)
+    thumbnail_path: str  # Thumbnail URL (썸네일 URL)
+    running_time: str  # Running Time (재생 시간)
+    is_available: bool  # Available in Laftel (라프텔 시청 가능 여부)
+    assetid: str  # Asset ID (에셋 아이디)
+
+    def __init__(self, data):
+        self.id = data.get("id")
+        self.title = data.get("title")
+        self.subject = data.get("subject")
+        self.description = data.get("description")
+        self.episode_num = data.get("episode_num")
+        self.episode_order = data.get("episode_order")
+        self.thumbnail_path = data.get("thumbnail_path")
+        self.running_time = data.get("running_time")
+        self.is_available = data.get("is_viewing")
+        self.assetid = "/".join(self.thumbnail_path.split("/")[4:7])
```

## laftel/utils.py

```diff
@@ -1,9 +1,14 @@
 import aiohttp
 
 
 async def api_request(RequestUrl: str):
-    async with aiohttp.ClientSession(headers={"laftel": "TeJava"}) as session:
+    async with aiohttp.ClientSession(
+        headers={
+            "laftel": "TeJava",
+            "User-Agent": "Mozilla/5.0 (iPhone; CPU iPhone OS 9_1_4; like Mac OS X) AppleWebKit/600.11 (KHTML, like Gecko)  Chrome/54.0.1486.383 Mobile Safari/600.8",
+        }
+    ) as session:
         async with session.get(
             RequestUrl,
         ) as response:
             return await response.json()
```

## Comparing `laftel-1.2.2.dist-info/LICENSE` & `laftel-1.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `laftel-1.2.2.dist-info/METADATA` & `laftel-1.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laftel
-Version: 1.2.2
+Version: 1.3.0
 Summary: 파이썬 라프텔 라이브러리, Unofficial Python Laftel API Wrapper(Laftel)
 Home-page: https://github.com/331leo/laftel
 Download-URL: https://github.com/331leo/laftel
 Author: LeoK
 Author-email: support@leok.kr
 License: GPL-V3
 Keywords: anime,laftel,info,API,wrapper
```

