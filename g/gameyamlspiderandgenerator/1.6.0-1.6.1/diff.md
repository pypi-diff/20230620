# Comparing `tmp/gameyamlspiderandgenerator-1.6.0.tar.gz` & `tmp/gameyamlspiderandgenerator-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.6.0.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.6.1.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.6.0.tar` & `gameyamlspiderandgenerator-1.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.6.0/LICENSE
--rwxr-xr-x   0        0        0     1350 2023-06-11 10:23:19.902922 gameyamlspiderandgenerator-1.6.0/README.md
--rwxr-xr-x   0        0        0      568 2023-06-07 14:28:47.706873 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1924 2023-06-11 10:27:03.919708 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      675 2023-06-11 14:22:24.297547 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      235 2023-05-22 00:40:10.045341 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     1476 2023-06-11 10:23:19.905735 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/openai.py
--rwxr-xr-x   0        0        0     3890 2023-05-22 00:40:10.056295 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0      559 2023-05-22 00:40:10.056896 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/validate.py
--rwxr-xr-x   0        0        0       56 2023-06-07 14:15:34.823402 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     3177 2023-06-11 10:23:19.906828 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7001 2023-06-11 14:16:35.827355 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7919 2023-06-11 14:16:45.563698 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1838 2023-05-22 00:40:10.090828 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     2138 2023-06-11 10:23:19.909201 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2550 2023-06-11 10:23:19.910070 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      265 2023-05-22 00:40:10.091597 gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/thread.py
--rwxr-xr-x   0        0        0      735 2023-06-11 14:23:22.938339 gameyamlspiderandgenerator-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.6.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.6.1/LICENSE
+-rwxr-xr-x   0        0        0     1350 2023-06-11 10:23:19.902922 gameyamlspiderandgenerator-1.6.1/README.md
+-rwxr-xr-x   0        0        0      568 2023-06-07 14:28:47.706873 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1924 2023-06-11 10:27:03.919708 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      675 2023-06-11 14:22:24.297547 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      235 2023-05-22 00:40:10.045341 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     1476 2023-06-11 10:23:19.905735 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/hook/openai.py
+-rwxr-xr-x   0        0        0     3890 2023-05-22 00:40:10.056295 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0      592 2023-06-13 13:44:51.378803 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/hook/validate.py
+-rwxr-xr-x   0        0        0       56 2023-06-07 14:15:34.823402 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     3177 2023-06-11 10:23:19.906828 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7088 2023-06-13 14:02:11.945879 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7919 2023-06-11 14:16:45.563698 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1848 2023-06-13 13:39:03.156896 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     2138 2023-06-11 10:23:19.909201 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2550 2023-06-11 10:23:19.910070 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      265 2023-05-22 00:40:10.091597 gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/util/thread.py
+-rwxr-xr-x   0        0        0      756 2023-06-13 14:03:34.515334 gameyamlspiderandgenerator-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.6.1/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.6.0/LICENSE` & `gameyamlspiderandgenerator-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/README.md` & `gameyamlspiderandgenerator-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/openai.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/hook/openai.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/hook/search.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/hook/validate.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/hook/validate.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 
 
 class Verify(BaseHook):
     CHANGED = None
 
     def setup(self, data: dict):
         try:
-            validate(data, safe_load(get_text('https://raw.githubusercontent.com/FurryGamesIndex/games/master/schemas'
+            validate({**data,'thumbnail': 'thumbnail.png'}, safe_load(get_text('https://raw.githubusercontent.com/FurryGamesIndex/games/master/schemas'
                                               '/game.schema.yaml')))
             logger.success("verification complete")
         except Exception as e:
             logger.error(e)
         return data
```

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from contextlib import suppress
 from json import loads
 from bs4 import BeautifulSoup
 from html2text import html2text
 from langcodes import find
+from py3langid import langid, classify
 
 from ._base import BasePlugin
 from ..util.fgi import fgi_dict
 from ..util.fgi_yaml import YamlData, pss_dedent
 from ..util.spider import get_text
 
 
@@ -63,15 +64,15 @@
             "Windows": "windows",
             "macOS": "macos",
             "Linux": "linux",
             "Android": "android",
             "HTML5": "web",
             "iOS": "ios",
         }
-        platforms = self.more_info["Platforms"][0].split(",") if "Platforms" in self.more_info else ["Windows"]
+        platforms = self.more_info["Platforms"] if "Platforms" in self.more_info else ["Windows"]
         return [repl[i.strip()] for i in platforms]
 
     def get_authors(self) -> list[dict]:
         temp = []
         if "Authors" in self.more_info:
             temp = self.more_info["Authors"]
         elif "Author" in self.more_info:
@@ -106,15 +107,19 @@
 
         ret = []
         for i, value in repl.items():
             ret.extend(value for ii in self.tag if i in ii)
         return list(set(ret))
 
     def get_langs(self) -> list[str]:
-        temp = self.more_info["Languages"] if "Languages" in self.more_info else ["English"]
+        if "Languages" in self.more_info:
+            temp = self.more_info["Languages"]
+        else:
+            return [classify(self.get_desc())[0]]
+
         return list(set(find(i).language for i in temp))
 
     def get_links(self) -> list[dict]:
         link = [i.attrs["href"] for i in self.soup.select_one("div.left_col.column > "
                                                               "div.formatted_description.user_formatted")
         .select("a[href]")]
         data = [{"url": i, "processed": False} for i in list(set(link))]
@@ -164,15 +169,15 @@
             "thumbnail": self.get_thumbnail(),
             "screenshots": self.get_screenshots()  # + self.get_video(),
         }
         return YamlData(self.__load_hook__(ret))
 
     def get_type_tag(self):
         repl = {
-            "Visual Novel": "visual-nove",
+            "Visual Novel": "visual-novel",
             "Real time strategy": "real-time-strategy",
             "Strategy": "strategy",
             "Casual": "casual",
             "Adventure": "adventure",
             "Board Game": "board",
             "Action": "action",
             "Fantasy": "fantasy",
```

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/util/fgi.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     },
     {
         "match": "^https://www.youtube.com/channel/(.+[^/])/",
         "prefix": ".youtube",
         "replace": "youtube:\\g<1>",
     },
     {
-        "match": "^https://twitter.com/(.{1,})",
+        "match": "^https://twitter.com/([A-Za-z0-9_]+).*",
         "prefix": ".twitter",
         "replace": "twitter:\\g<1>",
     },
     {
         "match": "^https://www.patreon.com/(.+)",
         "prefix": ".patreon",
         "replace": "patreon:\\g<1>",
```

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.6.1/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.0/pyproject.toml` & `gameyamlspiderandgenerator-1.6.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.6.0"
+version = "1.6.1"
 description = "A useful tool for generating Furrygameindex yaml files"
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -21,14 +21,15 @@
 loguru = "^0.6.0"
 pyyaml = "^6.0"
 pysocks = "^1.7.1"
 epicstore-api = "^0.1.6"
 jsonschema = "^4.17.3"
 openai = "^0.27.6"
 lxml = "^4.9.2"
+py3langid = "^0.2.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `gameyamlspiderandgenerator-1.6.0/PKG-INFO` & `gameyamlspiderandgenerator-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.6.0
+Version: 1.6.1
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -15,14 +15,15 @@
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
+Requires-Dist: py3langid (>=0.2.2,<0.3.0)
 Requires-Dist: pysocks (>=1.7.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: ruamel-base (>=1.0.0,<2.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: ruamel.yaml.string (>=0.1.0,<0.2.0)
 Requires-Dist: urllib3 (>=1.26.14,<2.0.0)
```

