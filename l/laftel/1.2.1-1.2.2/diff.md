# Comparing `tmp/laftel-1.2.1-py3-none-any.whl.zip` & `tmp/laftel-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17244 bytes, number of entries: 9
--rw-r--r--  2.0 unx      125 b- defN 23-Jun-20 00:22 laftel/__init__.py
+Zip file size: 17401 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      125 b- defN 23-Jun-20 00:36 laftel/__init__.py
 -rw-r--r--  2.0 unx     1739 b- defN 23-Jun-20 00:33 laftel/laftel.py
--rw-r--r--  2.0 unx     3312 b- defN 23-Jun-20 00:30 laftel/models.py
+-rw-r--r--  2.0 unx     3314 b- defN 23-Jun-20 00:36 laftel/models.py
 -rw-r--r--  2.0 unx      256 b- defN 23-Jun-20 00:24 laftel/utils.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jun-20 00:33 laftel-1.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3662 b- defN 23-Jun-20 00:33 laftel-1.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 00:33 laftel-1.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-20 00:33 laftel-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      672 b- defN 23-Jun-20 00:33 laftel-1.2.1.dist-info/RECORD
-9 files, 45014 bytes uncompressed, 16100 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jun-20 00:36 laftel-1.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3965 b- defN 23-Jun-20 00:36 laftel-1.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 00:36 laftel-1.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-20 00:36 laftel-1.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      672 b- defN 23-Jun-20 00:36 laftel-1.2.2.dist-info/RECORD
+9 files, 45319 bytes uncompressed, 16257 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: laftel/models.py
 Comment: 
 
 Filename: laftel/utils.py
 Comment: 
 
-Filename: laftel-1.2.1.dist-info/LICENSE
+Filename: laftel-1.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: laftel-1.2.1.dist-info/METADATA
+Filename: laftel-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: laftel-1.2.1.dist-info/WHEEL
+Filename: laftel-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: laftel-1.2.1.dist-info/top_level.txt
+Filename: laftel-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: laftel-1.2.1.dist-info/RECORD
+Filename: laftel-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## laftel/__init__.py

```diff
@@ -1,4 +1,4 @@
 from .laftel import getAnimeInfo, searchAnime, sync
 
 __all__ = ["sync", "searchAnime", "getAnimeInfo"]
-__version__ = "1.2.1"
+__version__ = "1.2.2"
```

## laftel/models.py

```diff
@@ -32,15 +32,15 @@
         self.image = data.get("img")
         self.content = data.get("content")
         self.ended = data.get("is_ending")
         self.awards = data.get("awards")
 
         self.content_rating = data.get("content_rating")
         self.adultonly = data.get("is_adult")
-        self.viewable = data.get("viewable")
+        self.viewable = data.get("is_viewing")
         self.genres = data.get("genres")
         self.tags = data.get("tags")
 
         self.air_year_quarter = data.get("air_year_quarter", "")
         self.air_day = data.get("distributed_air_time", "")
 
         self.avg_rating = data.get("avg_rating")
```

## Comparing `laftel-1.2.1.dist-info/LICENSE` & `laftel-1.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `laftel-1.2.1.dist-info/METADATA` & `laftel-1.2.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laftel
-Version: 1.2.1
+Version: 1.2.2
 Summary: 파이썬 라프텔 라이브러리, Unofficial Python Laftel API Wrapper(Laftel)
 Home-page: https://github.com/331leo/laftel
 Download-URL: https://github.com/331leo/laftel
 Author: LeoK
 Author-email: support@leok.kr
 License: GPL-V3
 Keywords: anime,laftel,info,API,wrapper
@@ -88,10 +88,17 @@
     air_day: str  # Airing day (방영 요일)
     avg_rating: float  # Average User Rating out of 5 (5점 만점 중 평균 별점)
 
     series_id: Optional[int]  # Series ID (시리즈 아이디)
     production: str  # Production company (제작사)
 ```
 
+## Discord Bot Example
+<img width="615" alt="image" src="https://user-images.githubusercontent.com/30466064/147765695-1b33c6cc-9954-4e5b-b1f5-53122aca7759.png">
+<img width="596" alt="image" src="https://user-images.githubusercontent.com/30466064/147765773-16b1d228-675f-4766-8e57-5baff42ffaf3.png">
+
 ## Example
 
 [View example.py](example.py)
+
+
+
```

## Comparing `laftel-1.2.1.dist-info/RECORD` & `laftel-1.2.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-laftel/__init__.py,sha256=VIAf3HFxdGvUkz185zhUHb2rO6vC-SMYlFTupQxqb-M,125
+laftel/__init__.py,sha256=6km18Umje_fV173PUvejsPvdCxdOOJliPA9sS9_TaI8,125
 laftel/laftel.py,sha256=auH0Bd1WzqcopoSmfGcMBcact7H8FeqKtfPq2EYitkw,1739
-laftel/models.py,sha256=9se5bABb1QsnVqX_W2bHy8h032lfyl83oWtWSpGmaeQ,3312
+laftel/models.py,sha256=S1StitTFG32cisOR_pSMAn8wR0_wyqT6dYcTknQAAps,3314
 laftel/utils.py,sha256=8zILW3kNwx5OHyn8o3SCUX7zrhVgY0CuJp2YY0vRZ0c,256
-laftel-1.2.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-laftel-1.2.1.dist-info/METADATA,sha256=ETmryMImgyeO97zh8Va-uFTA82K4_xBRGrWVQgdGptc,3662
-laftel-1.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-laftel-1.2.1.dist-info/top_level.txt,sha256=IUcersvf4Rhh-A_UDhhUoRJpPOraZNfYssiQtH3Yv7Q,7
-laftel-1.2.1.dist-info/RECORD,,
+laftel-1.2.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+laftel-1.2.2.dist-info/METADATA,sha256=R4_ZrW8W7J58geDizL7pqhv3AWAhwBW-ovWWzulHhIQ,3965
+laftel-1.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+laftel-1.2.2.dist-info/top_level.txt,sha256=IUcersvf4Rhh-A_UDhhUoRJpPOraZNfYssiQtH3Yv7Q,7
+laftel-1.2.2.dist-info/RECORD,,
```

