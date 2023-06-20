# Comparing `tmp/clown_sort-1.8.0.tar.gz` & `tmp/clown_sort-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.8.0.tar", max compression
+gzip compressed data, was "clown_sort-1.8.1.tar", max compression
```

## Comparing `clown_sort-1.8.0.tar` & `clown_sort-1.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3302 2023-06-20 03:21:16.499883 clown_sort-1.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.8.0/LICENSE
--rw-r--r--   0        0        0     9088 2023-06-20 03:19:34.505801 clown_sort-1.8.0/README.md
--rw-r--r--   0        0        0     3347 2023-06-20 03:19:34.506319 clown_sort-1.8.0/clown_sort/__init__.py
--rw-r--r--   0        0        0     7987 2023-06-03 00:19:42.985646 clown_sort-1.8.0/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.8.0/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.8.0/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     3069 2023-06-15 23:22:00.182053 clown_sort-1.8.0/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    12052 2023-06-20 03:19:34.507174 clown_sort-1.8.0/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3456 2023-06-15 23:17:52.887054 clown_sort-1.8.0/clown_sort/sort_selector.py
--rw-r--r--   0        0        0    11758 2023-06-20 03:19:34.507783 clown_sort-1.8.0/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.8.0/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.8.0/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.8.0/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3705 2023-06-20 03:19:34.508422 clown_sort-1.8.0/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.8.0/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.8.0/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.8.0/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1619 2023-06-20 03:21:16.505459 clown_sort-1.8.0/pyproject.toml
--rw-r--r--   0        0        0    10510 1970-01-01 00:00:00.000000 clown_sort-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     3405 2023-06-20 05:50:48.559552 clown_sort-1.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.8.1/LICENSE
+-rw-r--r--   0        0        0     9322 2023-06-20 05:48:55.384657 clown_sort-1.8.1/README.md
+-rw-r--r--   0        0        0     4215 2023-06-20 05:47:05.935055 clown_sort-1.8.1/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7987 2023-06-03 00:19:42.985646 clown_sort-1.8.1/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.8.1/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.8.1/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     3069 2023-06-15 23:22:00.182053 clown_sort-1.8.1/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    12052 2023-06-20 03:19:34.507174 clown_sort-1.8.1/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3456 2023-06-15 23:17:52.887054 clown_sort-1.8.1/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0    11758 2023-06-20 03:19:34.507783 clown_sort-1.8.1/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.8.1/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.8.1/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.8.1/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3705 2023-06-20 03:19:34.508422 clown_sort-1.8.1/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.8.1/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.8.1/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.8.1/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1712 2023-06-20 05:50:48.565217 clown_sort-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0    10744 1970-01-01 00:00:00.000000 clown_sort-1.8.1/PKG-INFO
```

### Comparing `clown_sort-1.8.0/CHANGELOG.md` & `clown_sort-1.8.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # NEXT RELEASE
 
+### 1.8.1
+* Actually make `extract_text_from_files` executable
+
 # 1.8.0
-* Add a script to 
+* Add a script to extract files
+* More default sort rules
 
 ### 1.7.1
 * Handle 0 byte PDF error
 * More default rules
 
 # 1.7.0
 * Skip comment rows starting with `#` in rules CSVs.
```

### Comparing `clown_sort-1.8.0/LICENSE` & `clown_sort-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/README.md` & `clown_sort-1.8.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -131,19 +131,19 @@
 ```sh
 pipx install clown_sort[gui]
 ```
 
 ![](doc/manual_select_box.png)
 
 
-## One Offs
-There is a script you can use to extract text from a single file (or a bunch of files, or all the files in a given directory). Just run:
+## One Off Extractions
+Sometimes you just want to see the extracted text from a PDF or image and aren't trying to sort anything. There is a convenience script ou can use to extract text from a single file, multiple files, or all the files in a given directory. Just run `extract_text_from_files MY_FILE` to extract a single file. As an example for extracting multiple files and/or directories:
 
 ```
-scripts/extract_text_from_files.py MY_FILE1 MY_FILE2 SOME_DIR3
+extract_text_from_files MY_FILE1 MY_FILE2 SOME_DIR3
 ```
 
 This will parse and display the text in `MY_FILE1`, `MY_FILE2`, and all the files in `SOME_DIR3`.
 
 
 # Contributing
 Feel free to file issues or open pull requests.
```

### Comparing `clown_sort-1.8.0/clown_sort/config.py` & `clown_sort-1.8.1/clown_sort/config.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/clown_sort/filename_extractor.py` & `clown_sort-1.8.1/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/clown_sort/files/image_file.py` & `clown_sort-1.8.1/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/clown_sort/files/pdf_file.py` & `clown_sort-1.8.1/clown_sort/files/pdf_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/clown_sort/files/sortable_file.py` & `clown_sort-1.8.1/clown_sort/files/sortable_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/clown_sort/sort_selector.py` & `clown_sort-1.8.1/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.8.1/clown_sort/sorting_rules/crypto.csv`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/clown_sort/util/argument_parser.py` & `clown_sort-1.8.1/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/clown_sort/util/constants.py` & `clown_sort-1.8.1/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/clown_sort/util/filesystem_helper.py` & `clown_sort-1.8.1/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/clown_sort/util/rich_helper.py` & `clown_sort-1.8.1/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/clown_sort/util/string_helper.py` & `clown_sort-1.8.1/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.0/pyproject.toml` & `clown_sort-1.8.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.8.0"
+version = "1.8.1"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
@@ -64,8 +64,9 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.scripts]
 sort_screenshots = 'clown_sort:sort_screenshots'
-set_screenshot_timestamps = 'clown_sort:set_screenshot_timestamps'
+set_screenshot_timestamps_from_filenames = 'clown_sort:set_screenshot_timestamps_from_filenames'
+extract_text_from_files = 'clown_sort:extract_text_from_files'
```

### Comparing `clown_sort-1.8.0/PKG-INFO` & `clown_sort-1.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.8.0
+Version: 1.8.1
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -164,19 +164,19 @@
 ```sh
 pipx install clown_sort[gui]
 ```
 
 ![](doc/manual_select_box.png)
 
 
-## One Offs
-There is a script you can use to extract text from a single file (or a bunch of files, or all the files in a given directory). Just run:
+## One Off Extractions
+Sometimes you just want to see the extracted text from a PDF or image and aren't trying to sort anything. There is a convenience script ou can use to extract text from a single file, multiple files, or all the files in a given directory. Just run `extract_text_from_files MY_FILE` to extract a single file. As an example for extracting multiple files and/or directories:
 
 ```
-scripts/extract_text_from_files.py MY_FILE1 MY_FILE2 SOME_DIR3
+extract_text_from_files MY_FILE1 MY_FILE2 SOME_DIR3
 ```
 
 This will parse and display the text in `MY_FILE1`, `MY_FILE2`, and all the files in `SOME_DIR3`.
 
 
 # Contributing
 Feel free to file issues or open pull requests.
```

