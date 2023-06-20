# Comparing `tmp/lesiwka-2.1.20230616.0.tar.gz` & `tmp/lesiwka-2.1.20230620.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesiwka-2.1.20230616.0.tar", last modified: Fri Jun 16 23:07:51 2023, max compression
+gzip compressed data, was "lesiwka-2.1.20230620.0.tar", last modified: Tue Jun 20 19:16:18 2023, max compression
```

## Comparing `lesiwka-2.1.20230616.0.tar` & `lesiwka-2.1.20230620.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:07:51.143426 lesiwka-2.1.20230616.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 23:07:51.143426 lesiwka-2.1.20230616.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:07:51.139426 lesiwka-2.1.20230616.0/lesiwka/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:07:51.143426 lesiwka-2.1.20230616.0/lesiwka/_decode/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_3.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_4.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_5.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_6.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_7.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_2_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_3_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_3_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_3_4.py
--rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/diacritics.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/punctuation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:07:51.139426 lesiwka-2.1.20230616.0/lesiwka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 23:07:51.000000 lesiwka-2.1.20230616.0/lesiwka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-16 23:07:51.000000 lesiwka-2.1.20230616.0/lesiwka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 23:07:51.000000 lesiwka-2.1.20230616.0/lesiwka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 23:07:51.000000 lesiwka-2.1.20230616.0/lesiwka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 23:07:51.000000 lesiwka-2.1.20230616.0/lesiwka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 23:07:51.143426 lesiwka-2.1.20230616.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:16:18.362577 lesiwka-2.1.20230620.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-20 19:16:18.362577 lesiwka-2.1.20230620.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:16:18.362577 lesiwka-2.1.20230620.0/lesiwka/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:16:18.362577 lesiwka-2.1.20230620.0/lesiwka/_decode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/rule_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/rule_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/rule_1_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/rule_1_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/rule_1_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/rule_1_6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/rule_1_7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/rule_2_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/rule_3_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/rule_3_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_decode/rule_3_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/diacritics.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/punctuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/lesiwka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:16:18.362577 lesiwka-2.1.20230620.0/lesiwka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-20 19:16:18.000000 lesiwka-2.1.20230620.0/lesiwka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-20 19:16:18.000000 lesiwka-2.1.20230620.0/lesiwka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:16:18.000000 lesiwka-2.1.20230620.0/lesiwka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 19:16:18.000000 lesiwka-2.1.20230620.0/lesiwka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 19:16:18.000000 lesiwka-2.1.20230620.0/lesiwka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-20 19:16:18.366577 lesiwka-2.1.20230620.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 19:16:10.000000 lesiwka-2.1.20230620.0/setup.py
```

### Comparing `lesiwka-2.1.20230616.0/LICENSE` & `lesiwka-2.1.20230620.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230616.0/PKG-INFO` & `lesiwka-2.1.20230620.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesiwka
-Version: 2.1.20230616.0
+Version: 2.1.20230620.0
 Summary: Python library to convert to/from Lesivka
 Author: Oleksandr Tishyn
 Author-email: 1079805+Mystic-Mirage@users.noreply.github.com
 License: CC0 1.0 Universal
 Project-URL: Source Code, https://github.com/lesiwka/python-lesiwka
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `lesiwka-2.1.20230616.0/lesiwka/__main__.py` & `lesiwka-2.1.20230620.0/lesiwka/__main__.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230616.0/lesiwka/_decode/__init__.py` & `lesiwka-2.1.20230620.0/lesiwka/_decode/__init__.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230616.0/lesiwka/_decode/postprocess.py` & `lesiwka-2.1.20230620.0/lesiwka/_decode/postprocess.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230616.0/lesiwka/_decode/preprocess.py` & `lesiwka-2.1.20230620.0/lesiwka/_decode/preprocess.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230616.0/lesiwka/_decode/rule_2_2.py` & `lesiwka-2.1.20230620.0/lesiwka/_decode/rule_2_2.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230616.0/lesiwka/_encode.py` & `lesiwka-2.1.20230620.0/lesiwka/_encode.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 iotted_upper_out = iotted_lower_out.upper()
 
 iotted_lower_lat = "eiua"
 iotted_upper_lat = iotted_lower_lat.upper()
 
 iot_lower_cyr = "й"
 iot_upper_cyr = iot_lower_cyr.upper()
+iot_cyr = iot_lower_cyr + iot_upper_cyr
 
 iot_lower_lat = "j"
 iot_upper_lat = iot_lower_lat.upper()
+iot_lat = iot_lower_lat + iot_upper_lat
 
-consonants_lower_cyr = "бвдгґжзйклмнпрстфхцчш"
+consonants_lower_cyr = "бвдгґжзклмнпрстфхцчш"
 consonants_upper_cyr = consonants_lower_cyr.upper()
 consonants_cyr = consonants_lower_cyr + consonants_upper_cyr
 
-consonants_lower_lat = "bvdhgžzjklmnprstfxcčš"
+consonants_lower_lat = "bvdhgžzklmnprstfxcčš"
 consonants_upper_lat = consonants_lower_lat.upper()
 consonants_lat = consonants_lower_lat + consonants_upper_lat
 
 soft_sign_lower_cyr = "ь"
 soft_sign_upper_cyr = soft_sign_lower_cyr.upper()
 soft_sign_cyr = soft_sign_lower_cyr + soft_sign_upper_cyr
 
@@ -52,25 +54,27 @@
 w_cyr = "вВ"
 w_lat = "wW"
 
 lower_cyr = (
     vowels_lower_cyr
     + iotted_lower_cyr
     + consonants_lower_cyr
+    + iot_lower_cyr
     + soft_sign_lower_cyr
     + sqcq_lower_cyr
 )
 upper_cyr = (
     vowels_upper_cyr
     + iotted_upper_cyr
     + consonants_upper_cyr
+    + iot_upper_cyr
     + soft_sign_upper_cyr
     + sqcq_upper_cyr
 )
-all_cyr = vowels_cyr + iotted_cyr + consonants_cyr + soft_sign_cyr + sqcq_cyr
+all_cyr = lower_cyr + upper_cyr
 
 abbr = (
     ("ЄІБ", "JeIB"),
     ("ЄАВТ", "JeAVT"),
     ("ЄАЕС", "JeAES"),
     ("ЄАНТК", "JeANTK"),
     ("ЄАР", "JeAR"),
@@ -310,32 +314,37 @@
 )
 
 w_pattern = (
     r"((?<=\b)|(?<=[_%s])){0}((?=[%s])|(?=[%s])|(?=\W*$)|"
     r"(?=\W*[%s](?:\W|$))|(?=\W+[%s]))"
     % (
         vowels_cyr + iotted_cyr + w_cyr,
-        consonants_cyr + sqcq_cyr,
+        consonants_cyr + iot_cyr + sqcq_cyr,
         APOSTROPHES,
         DELIMITERS,
-        consonants_cyr + sqcq_cyr + iotted_cyr + consonants_lat,
+        consonants_cyr
+        + iot_cyr
+        + sqcq_cyr
+        + iotted_cyr
+        + consonants_lat
+        + iot_lat,
     )
 )
 
 capital_pattern = r"(?<=[%s]){0}(?=\W*$)"
 sqcq_capital_pattern = capital_pattern % upper_cyr
 iotted_capital_pattern = capital_pattern % (
     vowels_upper_cyr + iotted_upper_cyr
 )
 
 apostrophe_pattern = r"(?<=[%s])[%s]{0}" % (all_cyr + w_lat, APOSTROPHES)
 iotted_pattern = r"((?<=\b)|(?<=[%s])){0}" % (vowels_cyr + iotted_cyr)
 ending_pattern = r"(?=[%s]|\W+[%s]|\W*$)" % (
     lower_cyr + "w",
-    lower_cyr + vowels_lat + consonants_lat + w_lat
+    lower_cyr + vowels_lat + consonants_lat + iot_lat + w_lat,
 )
 acuted_pattern = r"(?<=[%s]){0}" % (consonants_cyr + sqcq_cyr)
 
 affricate_exclude_patterns = (
     r"(?i:(?<=ме)){0}(?i:((?=заклад)|(?=захис)))",
     r"(?i:(?<=\bро)){0}(?i:(?=зал))",
     (
@@ -416,16 +425,16 @@
     (affricate_pattern_2.format("Дж"), "Đ"),
     (affricate_pattern_2.format("дз"), "ƶ"),
     (affricate_pattern_2.format("Дз"), "Ƶ"),
 )
 
 table = dict(
     zip(
-        vowels_cyr + consonants_cyr + soft_sign_cyr,
-        vowels_lat + consonants_lat + soft_sign_lat,
+        vowels_cyr + consonants_cyr + iot_cyr + soft_sign_cyr,
+        vowels_lat + consonants_lat + iot_lat + soft_sign_lat,
     )
 )
 table.update(
     {
         cyr: iot_lower_lat + lat
         for cyr, lat in zip(iotted_lower_cyr, iotted_lower_lat)
     }
```

### Comparing `lesiwka-2.1.20230616.0/lesiwka/ascii.py` & `lesiwka-2.1.20230620.0/lesiwka/ascii.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230616.0/lesiwka/utils.py` & `lesiwka-2.1.20230620.0/lesiwka/utils.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230616.0/lesiwka.egg-info/PKG-INFO` & `lesiwka-2.1.20230620.0/lesiwka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesiwka
-Version: 2.1.20230616.0
+Version: 2.1.20230620.0
 Summary: Python library to convert to/from Lesivka
 Author: Oleksandr Tishyn
 Author-email: 1079805+Mystic-Mirage@users.noreply.github.com
 License: CC0 1.0 Universal
 Project-URL: Source Code, https://github.com/lesiwka/python-lesiwka
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `lesiwka-2.1.20230616.0/lesiwka.egg-info/SOURCES.txt` & `lesiwka-2.1.20230620.0/lesiwka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230616.0/setup.cfg` & `lesiwka-2.1.20230620.0/setup.cfg`

 * *Files identical despite different names*

