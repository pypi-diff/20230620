# Comparing `tmp/baekjoonapi-0.2.2.tar.gz` & `tmp/baekjoonapi-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baekjoonapi-0.2.2.tar", max compression
+gzip compressed data, was "baekjoonapi-0.2.4.tar", max compression
```

## Comparing `baekjoonapi-0.2.2.tar` & `baekjoonapi-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      456 2023-04-30 07:05:06.371000 baekjoonapi-0.2.2/LICENSE.md
--rw-r--r--   0        0        0       99 2023-04-30 07:05:06.371000 baekjoonapi-0.2.2/README.md
--rw-r--r--   0        0        0     5587 2023-04-30 07:11:24.351000 baekjoonapi-0.2.2/bojapi/__init__.py
--rw-r--r--   0        0        0      477 2023-04-30 07:13:12.259000 baekjoonapi-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 baekjoonapi-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      456 2023-04-30 07:05:06.371000 baekjoonapi-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0       99 2023-04-30 07:05:06.371000 baekjoonapi-0.2.4/README.md
+-rw-r--r--   0        0        0     6091 2023-06-20 06:59:33.139000 baekjoonapi-0.2.4/bojapi/__init__.py
+-rw-r--r--   0        0        0      477 2023-06-20 06:59:58.610000 baekjoonapi-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 baekjoonapi-0.2.4/PKG-INFO
```

### Comparing `baekjoonapi-0.2.2/bojapi/__init__.py` & `baekjoonapi-0.2.4/bojapi/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,33 +61,44 @@
         self.username = _cache.find("a").text
         self.start = min(map(int, self.__timestamp__(_cache.find("blockquote").find_all("span", {"class": "update-local-time"}))))
         self.stop = max(map(int, self.__timestamp__(_cache.find("blockquote").find_all("span", {"class": "update-local-time"}))))
 
     def __timestamp__(self, a: list[Tag]):
         return [i["data-timestamp"] for i in a]
 
+class SolvedACClassDecoration:
+    none = "none",
+    silver = "silver",
+    gold = "gold"
+
 class SolvedACUser:
     """Solved.ac 유저의 정보 클래스 (Solved.ac User Information Class)"""
     def __init__(self, name):
         """유저의 정보를 가져옵니다 (Get user information)"""
         tiers = ["Unranked", "Bronze V", "Bronze IV", "Bronze III", "Bronze II", "Bronze I", "Silver V", "Silver IV", "Silver III", "Silver II", "Silver I", "Gold V", "Gold IV", "Gold III", "Gold II", "Gold I", "Platinum V", "Platinum I",
                  "Diamond IV", "Diamond III", "Diamond II", "Diamond I", "Ruby V", "Ruby IV", "Ruby III", "Ruby II", "Ruby I", "Master"]
         self.name = name
         apire = get("https://solved.ac/api/v3/user/show", params={"handle": name}, headers={"Content-Type": "application/json"}).json()
         self.bio = apire["bio"]
-        self.badge = apire["badgeId"]
+        self.badge = apire.get("badgeId")
         self.background = apire["backgroundId"]
         self.profileimage = apire["profileImageUrl"]
-        self.solved = apire["solvedCount"]
-        self.cla = apire["class"]
+        self.solved = int(apire["solvedCount"])
+        self.vote = int(apire["voteCount"])
+        self.solvedacclass = int(apire["class"])
         self.classDecoration = apire["classDecoration"]
         self.tier = tiers[apire["tier"]]
-        self.rating = apire["rating"]
-        self.ratingByProblemsSum = apire["ratingByProblemsSum"]
-        self.ratingByClass = apire["ratingByClass"]
-        self.ratingByVoteCount = apire["ratingByVoteCount"]
-        self.exp = apire["exp"]
-        self.rivalCount = apire["rivalCount"]
-        self.reverseRivalCount = apire["reverseRivalCount"]
-        self.maxStreak = apire["maxStreak"]
-        self.rank = apire["rank"]
-
+        self.rating = int(apire["rating"])
+        self.ratingByProblemsSum = int(apire["ratingByProblemsSum"])
+        self.ratingByClass = int(apire["ratingByClass"])
+        self.ratingByVoteCount = int(apire["ratingByVoteCount"])
+        self.rivalCount = int(apire["rivalCount"])
+        self.reverseRivalCount = int(apire["reverseRivalCount"])
+        self.maxStreak = int(apire["maxStreak"])
+        self.coins = int(apire["coins"])
+        self.stardusts = int(apire["stardusts"])
+        self.joinedAt = apire["joinedAt"]
+        self.bannedUntil = apire["bannedUntil"]
+        self.proUntil = apire["proUntil"]
+        self.rank = int(apire["rank"])
+        self.isRival = apire["isRival"] == 'true'
+        self.isReverseRival = apire["isReversedRival"] == 'true'
```

### Comparing `baekjoonapi-0.2.2/PKG-INFO` & `baekjoonapi-0.2.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baekjoonapi
-Version: 0.2.2
+Version: 0.2.4
 Summary: BaekjoonAPI for Python
 Home-page: https://github.com/misilelab/baekjoonapi
 License: MisileLab License
 Author: MisileLaboratory
 Requires-Python: >=3.7,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (==0.0.1)
 Requires-Dist: lxml (==4.9.2)
 Requires-Dist: random-user-agent (==1.0.1)
-Requires-Dist: requests (==2.29.0)
+Requires-Dist: requests (==2.31.0)
 Project-URL: Repository, https://github.com/misilelab/baekjoonapi
 Description-Content-Type: text/markdown
 
 # BaekjoonAPI
 
 BaekjoonAPI for python
```

