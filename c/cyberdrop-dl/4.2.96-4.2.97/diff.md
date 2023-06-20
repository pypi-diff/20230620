# Comparing `tmp/cyberdrop-dl-4.2.96.tar.gz` & `tmp/cyberdrop-dl-4.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.96.tar", last modified: Sat Jun 17 17:10:41 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.97.tar", last modified: Tue Jun 20 01:13:31 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.96.tar` & `cyberdrop-dl-4.2.97.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:41.759051 cyberdrop-dl-4.2.96/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18943 2023-06-17 17:10:41.759051 cyberdrop-dl-4.2.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18508 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:41.751051 cyberdrop-dl-4.2.96/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:41.751051 cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:41.755051 cyberdrop-dl-4.2.96/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:41.755051 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:41.755051 cyberdrop-dl-4.2.96/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22462 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23724 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:41.755051 cyberdrop-dl-4.2.96/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20933 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:10:41.751051 cyberdrop-dl-4.2.96/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18943 2023-06-17 17:10:41.000000 cyberdrop-dl-4.2.96/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-17 17:10:41.000000 cyberdrop-dl-4.2.96/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:10:41.000000 cyberdrop-dl-4.2.96/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-17 17:10:41.000000 cyberdrop-dl-4.2.96/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-17 17:10:41.000000 cyberdrop-dl-4.2.96/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 17:10:41.000000 cyberdrop-dl-4.2.96/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-17 17:10:41.759051 cyberdrop-dl-4.2.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 17:10:30.000000 cyberdrop-dl-4.2.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:31.708335 cyberdrop-dl-4.2.97/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-06-20 01:13:31.708335 cyberdrop-dl-4.2.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18678 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:31.696334 cyberdrop-dl-4.2.97/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:31.700335 cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:31.700335 cyberdrop-dl-4.2.97/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:31.704335 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7910 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:31.708335 cyberdrop-dl-4.2.97/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22462 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:31.708335 cyberdrop-dl-4.2.97/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:13:31.700335 cyberdrop-dl-4.2.97/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-06-20 01:13:31.000000 cyberdrop-dl-4.2.97/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-20 01:13:31.000000 cyberdrop-dl-4.2.97/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:13:31.000000 cyberdrop-dl-4.2.97/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 01:13:31.000000 cyberdrop-dl-4.2.97/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-20 01:13:31.000000 cyberdrop-dl-4.2.97/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 01:13:31.000000 cyberdrop-dl-4.2.97/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-20 01:13:31.708335 cyberdrop-dl-4.2.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 01:13:18.000000 cyberdrop-dl-4.2.97/setup.py
```

### Comparing `cyberdrop-dl-4.2.96/LICENSE` & `cyberdrop-dl-4.2.97/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/PKG-INFO` & `cyberdrop-dl-4.2.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.96
+Version: 4.2.97
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -159,14 +159,16 @@
 --filesize-minimum-videos               minimum filesize for videos (in bytes)
 --filesize-minimum-other                minimum filesize for other files (in bytes)
 --include-id                            include the ID in the download folder name
 --max-concurrent-threads                number of threads to download simultaneously
 --max-concurrent-domains                number of domains to download simultaneously
 --max-concurrent-albums                 number of albums to download simultaneously
 --max-concurrent-downloads-per-domain   number of simultaneous downloads per domain
+--max-filename-length                   maximum filename length
+--max-folder-name-length                maximum folder name length
 --skip-download-mark-completed          sets the scraped files as downloaded without downloading
 --output-errored-urls                   sets the failed urls to be output to the errored urls file
 --output-unsupported-urls               sets the unsupported urls to be output to the unsupported urls file
 --proxy                                 HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:[port]
 --remove-bunkr-identifier               removes the bunkr added identifier from output filenames
 --required-free-space                   required free space (in gigabytes) for the program to run
 
@@ -213,8 +215,8 @@
 --refresh-rate                  changes the refresh rate of the progress table
 --visible-rows-threads          number of visible rows to use for the threads table
 --visible-rows-domains          number of visible rows to use for the domains table
 --visible-rows-albums           number of visible rows to use for the albums table
 --visible-rows-files            number of visible rows to use for the files table
 ```
 
-`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
+`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "coomer.su", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "jpg.fishing", "jpg.pet", "kemono.party", "lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.96 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.97 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -139,55 +139,56 @@
 other files (in bytes) --filesize-minimum-images minimum filesize for images
 (in bytes) --filesize-minimum-videos minimum filesize for videos (in bytes) --
 filesize-minimum-other minimum filesize for other files (in bytes) --include-id
 include the ID in the download folder name --max-concurrent-threads number of
 threads to download simultaneously --max-concurrent-domains number of domains
 to download simultaneously --max-concurrent-albums number of albums to download
 simultaneously --max-concurrent-downloads-per-domain number of simultaneous
-downloads per domain --skip-download-mark-completed sets the scraped files as
-downloaded without downloading --output-errored-urls sets the failed urls to be
-output to the errored urls file --output-unsupported-urls sets the unsupported
-urls to be output to the unsupported urls file --proxy HTTP/HTTPS proxy used
-for downloading, format [protocol]://[ip]:[port] --remove-bunkr-identifier
-removes the bunkr added identifier from output filenames --required-free-space
-required free space (in gigabytes) for the program to run --sort-downloads
-sorts downloaded files after downloads have finished --sort-directory folder to
-download files to --sorted-audio schema to sort audio --sorted-images schema to
-sort images --sorted-others schema to sort other --sorted-videos schema to sort
-videos --connection-timeout number of seconds to wait attempting to connect to
-a URL during the downloading phase --ratelimit this applies to requests made in
-the program during scraping, the number you provide is in requests/seconds --
-read-timeout number of seconds to wait for data to be read from a URL during
-the downloading phase --throttle this is a throttle between requests during the
-downloading phase, the number is in seconds --output-last-forum-post outputs
-the last post of a forum scrape to use as a starting point for future runs --
-scrape-single-post scrapes a single post from a forum thread --separate-posts
-separates forum scraping into folders by post number --gofile-api-key api key
-for premium gofile --gofile-website-token website token for gofile --
-pixeldrain-api-key api key for premium pixeldrain --nudostar-username username
-to login to nudostar --nudostar-password password to login to nudostar --
-simpcity-username username to login to simpcity --simpcity-password password to
-login to simpcity --socialmediagirls-username username to login to
-socialmediagirls --socialmediagirls-password password to login to
-socialmediagirls --xbunker-username username to login to xbunker --xbunker-
-password password to login to xbunker --apply-jdownloader enables sending
-unsupported URLs to a running jdownloader2 instance to download --jdownloader-
-username username to login to jdownloader --jdownloader-password password to
-login to jdownloader --jdownloader-device device name to login to for
-jdownloader --hide-new-progress disables the new rich progress entirely and
+downloads per domain --max-filename-length maximum filename length --max-
+folder-name-length maximum folder name length --skip-download-mark-completed
+sets the scraped files as downloaded without downloading --output-errored-urls
+sets the failed urls to be output to the errored urls file --output-
+unsupported-urls sets the unsupported urls to be output to the unsupported urls
+file --proxy HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:
+[port] --remove-bunkr-identifier removes the bunkr added identifier from output
+filenames --required-free-space required free space (in gigabytes) for the
+program to run --sort-downloads sorts downloaded files after downloads have
+finished --sort-directory folder to download files to --sorted-audio schema to
+sort audio --sorted-images schema to sort images --sorted-others schema to sort
+other --sorted-videos schema to sort videos --connection-timeout number of
+seconds to wait attempting to connect to a URL during the downloading phase --
+ratelimit this applies to requests made in the program during scraping, the
+number you provide is in requests/seconds --read-timeout number of seconds to
+wait for data to be read from a URL during the downloading phase --throttle
+this is a throttle between requests during the downloading phase, the number is
+in seconds --output-last-forum-post outputs the last post of a forum scrape to
+use as a starting point for future runs --scrape-single-post scrapes a single
+post from a forum thread --separate-posts separates forum scraping into folders
+by post number --gofile-api-key api key for premium gofile --gofile-website-
+token website token for gofile --pixeldrain-api-key api key for premium
+pixeldrain --nudostar-username username to login to nudostar --nudostar-
+password password to login to nudostar --simpcity-username username to login to
+simpcity --simpcity-password password to login to simpcity --socialmediagirls-
+username username to login to socialmediagirls --socialmediagirls-password
+password to login to socialmediagirls --xbunker-username username to login to
+xbunker --xbunker-password password to login to xbunker --apply-jdownloader
+enables sending unsupported URLs to a running jdownloader2 instance to download
+--jdownloader-username username to login to jdownloader --jdownloader-password
+password to login to jdownloader --jdownloader-device device name to login to
+for jdownloader --hide-new-progress disables the new rich progress entirely and
 uses older methods --hide-overall-progress removes overall progress section
 while downloading --hide-forum-progress removes forum progress section while
 downloading --hide-thread-progress removes thread progress section while
 downloading --hide-domain-progress removes domain progress section while
 downloading --hide-album-progress removes album progress section while
 downloading --hide-file-progress removes file progress section while
 downloading --refresh-rate changes the refresh rate of the progress table --
 visible-rows-threads number of visible rows to use for the threads table --
 visible-rows-domains number of visible rows to use for the domains table --
 visible-rows-albums number of visible rows to use for the albums table --
 visible-rows-files number of visible rows to use for the files table ``` `--
 only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
-"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
-"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
-"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
-"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
-"socialmediagirls", "xbunker", "xbunkr"`
+"coomer.party", "coomer.su", "cyberdrop", "cyberfile", "e-hentai", "erome",
+"fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi",
+"imgbox", "jpg.church", "jpg.fish", "jpg.fishing", "jpg.pet", "kemono.party",
+"lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li",
+"postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.2.96/README.md` & `cyberdrop-dl-4.2.97/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,16 @@
 --filesize-minimum-videos               minimum filesize for videos (in bytes)
 --filesize-minimum-other                minimum filesize for other files (in bytes)
 --include-id                            include the ID in the download folder name
 --max-concurrent-threads                number of threads to download simultaneously
 --max-concurrent-domains                number of domains to download simultaneously
 --max-concurrent-albums                 number of albums to download simultaneously
 --max-concurrent-downloads-per-domain   number of simultaneous downloads per domain
+--max-filename-length                   maximum filename length
+--max-folder-name-length                maximum folder name length
 --skip-download-mark-completed          sets the scraped files as downloaded without downloading
 --output-errored-urls                   sets the failed urls to be output to the errored urls file
 --output-unsupported-urls               sets the unsupported urls to be output to the unsupported urls file
 --proxy                                 HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:[port]
 --remove-bunkr-identifier               removes the bunkr added identifier from output filenames
 --required-free-space                   required free space (in gigabytes) for the program to run
 
@@ -201,8 +203,8 @@
 --refresh-rate                  changes the refresh rate of the progress table
 --visible-rows-threads          number of visible rows to use for the threads table
 --visible-rows-domains          number of visible rows to use for the domains table
 --visible-rows-albums           number of visible rows to use for the albums table
 --visible-rows-files            number of visible rows to use for the files table
 ```
 
-`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
+`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "coomer.su", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "jpg.fishing", "jpg.pet", "kemono.party", "lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

#### html2text {}

```diff
@@ -133,55 +133,56 @@
 other files (in bytes) --filesize-minimum-images minimum filesize for images
 (in bytes) --filesize-minimum-videos minimum filesize for videos (in bytes) --
 filesize-minimum-other minimum filesize for other files (in bytes) --include-id
 include the ID in the download folder name --max-concurrent-threads number of
 threads to download simultaneously --max-concurrent-domains number of domains
 to download simultaneously --max-concurrent-albums number of albums to download
 simultaneously --max-concurrent-downloads-per-domain number of simultaneous
-downloads per domain --skip-download-mark-completed sets the scraped files as
-downloaded without downloading --output-errored-urls sets the failed urls to be
-output to the errored urls file --output-unsupported-urls sets the unsupported
-urls to be output to the unsupported urls file --proxy HTTP/HTTPS proxy used
-for downloading, format [protocol]://[ip]:[port] --remove-bunkr-identifier
-removes the bunkr added identifier from output filenames --required-free-space
-required free space (in gigabytes) for the program to run --sort-downloads
-sorts downloaded files after downloads have finished --sort-directory folder to
-download files to --sorted-audio schema to sort audio --sorted-images schema to
-sort images --sorted-others schema to sort other --sorted-videos schema to sort
-videos --connection-timeout number of seconds to wait attempting to connect to
-a URL during the downloading phase --ratelimit this applies to requests made in
-the program during scraping, the number you provide is in requests/seconds --
-read-timeout number of seconds to wait for data to be read from a URL during
-the downloading phase --throttle this is a throttle between requests during the
-downloading phase, the number is in seconds --output-last-forum-post outputs
-the last post of a forum scrape to use as a starting point for future runs --
-scrape-single-post scrapes a single post from a forum thread --separate-posts
-separates forum scraping into folders by post number --gofile-api-key api key
-for premium gofile --gofile-website-token website token for gofile --
-pixeldrain-api-key api key for premium pixeldrain --nudostar-username username
-to login to nudostar --nudostar-password password to login to nudostar --
-simpcity-username username to login to simpcity --simpcity-password password to
-login to simpcity --socialmediagirls-username username to login to
-socialmediagirls --socialmediagirls-password password to login to
-socialmediagirls --xbunker-username username to login to xbunker --xbunker-
-password password to login to xbunker --apply-jdownloader enables sending
-unsupported URLs to a running jdownloader2 instance to download --jdownloader-
-username username to login to jdownloader --jdownloader-password password to
-login to jdownloader --jdownloader-device device name to login to for
-jdownloader --hide-new-progress disables the new rich progress entirely and
+downloads per domain --max-filename-length maximum filename length --max-
+folder-name-length maximum folder name length --skip-download-mark-completed
+sets the scraped files as downloaded without downloading --output-errored-urls
+sets the failed urls to be output to the errored urls file --output-
+unsupported-urls sets the unsupported urls to be output to the unsupported urls
+file --proxy HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:
+[port] --remove-bunkr-identifier removes the bunkr added identifier from output
+filenames --required-free-space required free space (in gigabytes) for the
+program to run --sort-downloads sorts downloaded files after downloads have
+finished --sort-directory folder to download files to --sorted-audio schema to
+sort audio --sorted-images schema to sort images --sorted-others schema to sort
+other --sorted-videos schema to sort videos --connection-timeout number of
+seconds to wait attempting to connect to a URL during the downloading phase --
+ratelimit this applies to requests made in the program during scraping, the
+number you provide is in requests/seconds --read-timeout number of seconds to
+wait for data to be read from a URL during the downloading phase --throttle
+this is a throttle between requests during the downloading phase, the number is
+in seconds --output-last-forum-post outputs the last post of a forum scrape to
+use as a starting point for future runs --scrape-single-post scrapes a single
+post from a forum thread --separate-posts separates forum scraping into folders
+by post number --gofile-api-key api key for premium gofile --gofile-website-
+token website token for gofile --pixeldrain-api-key api key for premium
+pixeldrain --nudostar-username username to login to nudostar --nudostar-
+password password to login to nudostar --simpcity-username username to login to
+simpcity --simpcity-password password to login to simpcity --socialmediagirls-
+username username to login to socialmediagirls --socialmediagirls-password
+password to login to socialmediagirls --xbunker-username username to login to
+xbunker --xbunker-password password to login to xbunker --apply-jdownloader
+enables sending unsupported URLs to a running jdownloader2 instance to download
+--jdownloader-username username to login to jdownloader --jdownloader-password
+password to login to jdownloader --jdownloader-device device name to login to
+for jdownloader --hide-new-progress disables the new rich progress entirely and
 uses older methods --hide-overall-progress removes overall progress section
 while downloading --hide-forum-progress removes forum progress section while
 downloading --hide-thread-progress removes thread progress section while
 downloading --hide-domain-progress removes domain progress section while
 downloading --hide-album-progress removes album progress section while
 downloading --hide-file-progress removes file progress section while
 downloading --refresh-rate changes the refresh rate of the progress table --
 visible-rows-threads number of visible rows to use for the threads table --
 visible-rows-domains number of visible rows to use for the domains table --
 visible-rows-albums number of visible rows to use for the albums table --
 visible-rows-files number of visible rows to use for the files table ``` `--
 only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
-"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
-"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
-"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
-"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
-"socialmediagirls", "xbunker", "xbunkr"`
+"coomer.party", "coomer.su", "cyberdrop", "cyberfile", "e-hentai", "erome",
+"fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi",
+"imgbox", "jpg.church", "jpg.fish", "jpg.fishing", "jpg.pet", "kemono.party",
+"lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li",
+"postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/base_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,15 @@
     },
     'Audio': {
         '.mp3', '.flac', '.wav', '.m4a',
     }
 }
 
 logger = logging.getLogger(__name__)
-MAX_FILENAME_LENGTH = 95
-
+MAX_NAME_LENGTHS = {"FILE": 95, "FOLDER": 60}
 
 async def clear() -> None:
     """Clears the terminal screen"""
     clear_screen_proc = await asyncio.create_subprocess_shell('cls' if os.name == 'nt' else 'clear')
     await clear_screen_proc.wait()
 
 
@@ -81,15 +80,15 @@
 
 async def make_title_safe(title: str) -> str:
     """Simple sanitization to remove illegal characters from titles and trim the length to be less than 60 chars"""
     title = title.replace("\n", "").strip()
     title = title.replace("\t", "").strip()
     title = re.sub(' +', ' ', title)
     title = re.sub(r'[\\*?:"<>|./]', "-", title)
-    title = title[:60].strip()
+    title = title[:MAX_NAME_LENGTHS['FOLDER']].strip()
     return title
 
 
 async def check_direct(url: URL) -> bool:
     """Checks whether the given url is a direct link to a content item"""
     mapping_direct = [r'i.pixl.li', r'i..pixl.li', r'img-...cyberdrop...', r'f.cyberdrop...',
                       r'fs-...cyberdrop...', r'jpg.church/images/...', r'simp..jpg.church', r'jpg.fish/images/...',
@@ -103,15 +102,15 @@
     """Returns the filename and extension of a given file, throws NoExtensionFailure if there is no extension"""
     filename_parts = filename.rsplit('.', 1)
     if len(filename_parts) == 1:
         raise NoExtensionFailure()
     if filename_parts[-1].isnumeric() and forum:
         filename_parts = filename_parts[0].rsplit('-', 1)
     ext = "." + filename_parts[-1].lower()
-    filename = filename_parts[0][:MAX_FILENAME_LENGTH] if len(filename_parts[0]) > MAX_FILENAME_LENGTH else filename_parts[0]
+    filename = filename_parts[0][:MAX_NAME_LENGTHS['FILE']] if len(filename_parts[0]) > MAX_NAME_LENGTHS['FILE'] else filename_parts[0]
     filename = filename.strip()
     filename = await sanitize(filename + ext)
     return filename, ext
 
 
 async def create_media_item(url: URL, referer: URL, sql_helper: SQLHelper, domain: str) -> MediaItem:
     """Returns the MediaItem of a given url, throws NoExtensionFailure if url.name doesn't have extension"""
```

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/config_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,16 @@
             "filesize_maximum_other": 0,
             "filesize_maximum_videos": 0,
             "include_id": False,
             "max_concurrent_threads": 0,
             "max_concurrent_domains": 0,
             "max_concurrent_albums": 0,
             "max_concurrent_downloads_per_domain": 4,
+            "max_filename_length": 95,
+            "max_folder_name_length": 60,
             "output_errored_urls": False,
             "output_unsupported_urls": False,
             "proxy": "",
             "remove_bunkr_identifier": False,
             "required_free_space": 5,
             "skip_download_mark_completed": False,
             "user_agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/112.0",
```

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/data_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     async def remove_lock(self, filename: str) -> None:
         self.locked_files.remove(filename.lower())
 
 
 @dataclass
 class SkipData:
     """The allows optoins for domains to skip when scraping"""
-    supported_hosts: ClassVar[Tuple[str, ...]] = ("anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
-                                                  "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gofile",
-                                                  "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish",
+    supported_hosts: ClassVar[Tuple[str, ...]] = ("anonfiles", "bayfiles", "bunkr", "coomer.party", "coomer.su",
+                                                  "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat",
+                                                  "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish",
                                                   "jpg.fishing", "jpg.pet", "gallery.deltaporno.com", "kemono.party",
                                                   "lovefap", "nsfw.xxx", "pimpandhost", "pixeldrain", "pixl.li",
                                                   "postimg", "saint", "nudostar", "simpcity", "socialmediagirls",
                                                   "xbunker", "xbunkr")
     sites: List[str]
```

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         return cascade, title
 
     async def handle_coomeno(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem) -> str:
         """Coomer/Kemono director function"""
         title = f"Loose {domain.capitalize()} Files"
         if "thumbnail" in url.parts:
             parts = [x for x in url.parts if x not in ("thumbnail", "/")]
-            link = URL(f"https://{domain}.party/{'/'.join(parts)}")
+            link = URL(f"https://{url.host}/{'/'.join(parts)}")
 
             media_item = await create_media_item(link, url, self.SQL_Helper, domain)
             await cascade.add_to_album(domain, title, media_item)
 
         elif "data" in url.parts:
             media_item = await create_media_item(url, url, self.SQL_Helper, domain)
             await cascade.add_to_album(domain, title, media_item)
```

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from cyberdrop_dl.client.client import Client, ScrapeSession
 from cyberdrop_dl.downloader.downloader_utils import check_free_space
 from cyberdrop_dl.downloader.downloaders import DownloadDirector
 from cyberdrop_dl.downloader.old_downloaders import old_download_forums
 from cyberdrop_dl.scraper.Scraper import ScrapeMapper
 
 from . import __version__ as VERSION
+from .base_functions.base_functions import MAX_NAME_LENGTHS
 from .base_functions.data_classes import ForumItem, SkipData
 
 
 def parse_args() -> argparse.Namespace:
     """Parses the command line arguments passed into the program"""
     parser = argparse.ArgumentParser(description="Bulk downloader for multiple file hosts")
     parser.add_argument("-V", "--version", action="version", version=f"%(prog)s {VERSION}")
@@ -81,14 +82,16 @@
     runtime_opts.add_argument("--filesize-minimum-videos", type=int, default=config_group["filesize_minimum_videos"], help="minimum filesize for videos (in bytes) (default: %(default)s)")
     runtime_opts.add_argument("--filesize-minimum-other", type=int, default=config_group["filesize_minimum_other"], help="minimum filesize for other files (in bytes) (default: %(default)s)")
     runtime_opts.add_argument("--include-id", help="include the ID in the download folder name", action="store_true")
     runtime_opts.add_argument("--max-concurrent-threads", type=int, default=config_group["max_concurrent_threads"], help="Number of threads to download simultaneously (default: %(default)s)")
     runtime_opts.add_argument("--max-concurrent-domains", type=int, default=config_group["max_concurrent_domains"], help="Number of domains to download simultaneously (default: %(default)s)")
     runtime_opts.add_argument("--max-concurrent-albums", type=int, default=config_group["max_concurrent_albums"], help="Number of albums to download simultaneously (default: %(default)s)")
     runtime_opts.add_argument("--max-concurrent-downloads-per-domain", type=int, default=config_group["max_concurrent_downloads_per_domain"], help="Number of simultaneous downloads per domain (default: %(default)s)")
+    runtime_opts.add_argument("--max-filename-length", type=int, default=config_group["max_filename_length"], help="maximum filename length (default: %(default)s)")
+    runtime_opts.add_argument("--max-folder-name-length", type=int, default=config_group["max_folder_name_length"], help="maximum folder name length (default: %(default)s)")
     runtime_opts.add_argument("--skip-download-mark-completed", help="sets the scraped files as downloaded without downloading", action="store_true")
     runtime_opts.add_argument("--output-errored-urls", help="sets the failed urls to be output to the errored urls file", action="store_true")
     runtime_opts.add_argument("--output-unsupported-urls", help="sets the unsupported urls to be output to the unsupported urls file", action="store_true")
     runtime_opts.add_argument("--proxy", help="HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:[port]", default=config_group["proxy"])
     runtime_opts.add_argument("--remove-bunkr-identifier", help="removes the bunkr added identifier from output filenames", action="store_true")
     runtime_opts.add_argument("--required-free-space", type=int, default=config_group["required_free_space"], help="required free space (in gigabytes) for the program to run (default: %(default)s)")
 
@@ -271,14 +274,17 @@
 async def director(args: Dict, links: List) -> None:
     """This is the overarching director coordinator for CDL."""
     await clear()
     await document_args(args)
     log(f"We are running version {VERSION} of Cyberdrop Downloader")
     error_writer, cache_manager = await file_management(args, links)
 
+    MAX_NAME_LENGTHS["FILE"] = args["Runtime"]["max_filename_length"]
+    MAX_NAME_LENGTHS["FOLDER"] = args["Runtime"]["max_folder_name_length"]
+
     if not await check_free_space(args['Runtime']['required_free_space'], args['Files']['output_folder']):
         log("Not enough free space to continue. You can change the required space required using --required-free-space.", style="red")
         exit(1)
 
     links = await consolidate_links(args, links)
     client = Client(args['Ratelimiting']['ratelimit'], args['Ratelimiting']['throttle'],
                     args['Runtime']['allow_insecure_connections'], args["Ratelimiting"]["connection_timeout"],
```

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.97/cyberdrop_dl/scraper/Scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,17 +90,17 @@
                         "bunkr": self.Bunkr, "cyberdrop": self.Cyberdrop, "cyberfile": self.CyberFile,
                         "erome": self.Erome, "fapello": self.Fapello, "gfycat": self.Gfycat, "gofile": self.GoFile,
                         "hgamecg": self.HGameCG, "imgbox": self.ImgBox, "pixeldrain": self.PixelDrain,
                         "postimg": self.PostImg, "saint": self.Saint, "img.kiwi": self.ShareX,
                         "jpg.church": self.ShareX, "jpg.fish": self.ShareX, "jpg.pet": self.ShareX,
                         "pixl.li": self.ShareX, "nsfw.xxx": self.NSFW_XXX, "pimpandhost": self.PimpAndHost,
                         "lovefap": self.LoveFap, "e-hentai": self.EHentai, "gallery.deltaporno": self.ShareX,
-                        "vk.com": self.vk_redirect, "coomer.party": self.Coomeno, "kemono.party": self.Coomeno,
-                        "nudostar": self.Xenforo, "simpcity": self.Xenforo, "socialmediagirls": self.Xenforo,
-                        "xbunker": self.Xenforo}
+                        "vk.com": self.vk_redirect, "coomer.party": self.Coomeno, "coomer.su": self.Coomeno,
+                        "kemono.party": self.Coomeno, "nudostar": self.Xenforo, "simpcity": self.Xenforo,
+                        "socialmediagirls": self.Xenforo, "xbunker": self.Xenforo}
 
     async def _handle_album_additions(self, domain: str, album_obj: AlbumItem, title=None) -> None:
         if title:
             await album_obj.append_title(title)
             await self.Forums.add_album_to_thread(title, domain, album_obj)
         else:
             await self.Cascade.add_album(domain, album_obj.title, album_obj)
```

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.97/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.96
+Version: 4.2.97
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -159,14 +159,16 @@
 --filesize-minimum-videos               minimum filesize for videos (in bytes)
 --filesize-minimum-other                minimum filesize for other files (in bytes)
 --include-id                            include the ID in the download folder name
 --max-concurrent-threads                number of threads to download simultaneously
 --max-concurrent-domains                number of domains to download simultaneously
 --max-concurrent-albums                 number of albums to download simultaneously
 --max-concurrent-downloads-per-domain   number of simultaneous downloads per domain
+--max-filename-length                   maximum filename length
+--max-folder-name-length                maximum folder name length
 --skip-download-mark-completed          sets the scraped files as downloaded without downloading
 --output-errored-urls                   sets the failed urls to be output to the errored urls file
 --output-unsupported-urls               sets the unsupported urls to be output to the unsupported urls file
 --proxy                                 HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:[port]
 --remove-bunkr-identifier               removes the bunkr added identifier from output filenames
 --required-free-space                   required free space (in gigabytes) for the program to run
 
@@ -213,8 +215,8 @@
 --refresh-rate                  changes the refresh rate of the progress table
 --visible-rows-threads          number of visible rows to use for the threads table
 --visible-rows-domains          number of visible rows to use for the domains table
 --visible-rows-albums           number of visible rows to use for the albums table
 --visible-rows-files            number of visible rows to use for the files table
 ```
 
-`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
+`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "coomer.su", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "jpg.fishing", "jpg.pet", "kemono.party", "lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.96 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.97 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -139,55 +139,56 @@
 other files (in bytes) --filesize-minimum-images minimum filesize for images
 (in bytes) --filesize-minimum-videos minimum filesize for videos (in bytes) --
 filesize-minimum-other minimum filesize for other files (in bytes) --include-id
 include the ID in the download folder name --max-concurrent-threads number of
 threads to download simultaneously --max-concurrent-domains number of domains
 to download simultaneously --max-concurrent-albums number of albums to download
 simultaneously --max-concurrent-downloads-per-domain number of simultaneous
-downloads per domain --skip-download-mark-completed sets the scraped files as
-downloaded without downloading --output-errored-urls sets the failed urls to be
-output to the errored urls file --output-unsupported-urls sets the unsupported
-urls to be output to the unsupported urls file --proxy HTTP/HTTPS proxy used
-for downloading, format [protocol]://[ip]:[port] --remove-bunkr-identifier
-removes the bunkr added identifier from output filenames --required-free-space
-required free space (in gigabytes) for the program to run --sort-downloads
-sorts downloaded files after downloads have finished --sort-directory folder to
-download files to --sorted-audio schema to sort audio --sorted-images schema to
-sort images --sorted-others schema to sort other --sorted-videos schema to sort
-videos --connection-timeout number of seconds to wait attempting to connect to
-a URL during the downloading phase --ratelimit this applies to requests made in
-the program during scraping, the number you provide is in requests/seconds --
-read-timeout number of seconds to wait for data to be read from a URL during
-the downloading phase --throttle this is a throttle between requests during the
-downloading phase, the number is in seconds --output-last-forum-post outputs
-the last post of a forum scrape to use as a starting point for future runs --
-scrape-single-post scrapes a single post from a forum thread --separate-posts
-separates forum scraping into folders by post number --gofile-api-key api key
-for premium gofile --gofile-website-token website token for gofile --
-pixeldrain-api-key api key for premium pixeldrain --nudostar-username username
-to login to nudostar --nudostar-password password to login to nudostar --
-simpcity-username username to login to simpcity --simpcity-password password to
-login to simpcity --socialmediagirls-username username to login to
-socialmediagirls --socialmediagirls-password password to login to
-socialmediagirls --xbunker-username username to login to xbunker --xbunker-
-password password to login to xbunker --apply-jdownloader enables sending
-unsupported URLs to a running jdownloader2 instance to download --jdownloader-
-username username to login to jdownloader --jdownloader-password password to
-login to jdownloader --jdownloader-device device name to login to for
-jdownloader --hide-new-progress disables the new rich progress entirely and
+downloads per domain --max-filename-length maximum filename length --max-
+folder-name-length maximum folder name length --skip-download-mark-completed
+sets the scraped files as downloaded without downloading --output-errored-urls
+sets the failed urls to be output to the errored urls file --output-
+unsupported-urls sets the unsupported urls to be output to the unsupported urls
+file --proxy HTTP/HTTPS proxy used for downloading, format [protocol]://[ip]:
+[port] --remove-bunkr-identifier removes the bunkr added identifier from output
+filenames --required-free-space required free space (in gigabytes) for the
+program to run --sort-downloads sorts downloaded files after downloads have
+finished --sort-directory folder to download files to --sorted-audio schema to
+sort audio --sorted-images schema to sort images --sorted-others schema to sort
+other --sorted-videos schema to sort videos --connection-timeout number of
+seconds to wait attempting to connect to a URL during the downloading phase --
+ratelimit this applies to requests made in the program during scraping, the
+number you provide is in requests/seconds --read-timeout number of seconds to
+wait for data to be read from a URL during the downloading phase --throttle
+this is a throttle between requests during the downloading phase, the number is
+in seconds --output-last-forum-post outputs the last post of a forum scrape to
+use as a starting point for future runs --scrape-single-post scrapes a single
+post from a forum thread --separate-posts separates forum scraping into folders
+by post number --gofile-api-key api key for premium gofile --gofile-website-
+token website token for gofile --pixeldrain-api-key api key for premium
+pixeldrain --nudostar-username username to login to nudostar --nudostar-
+password password to login to nudostar --simpcity-username username to login to
+simpcity --simpcity-password password to login to simpcity --socialmediagirls-
+username username to login to socialmediagirls --socialmediagirls-password
+password to login to socialmediagirls --xbunker-username username to login to
+xbunker --xbunker-password password to login to xbunker --apply-jdownloader
+enables sending unsupported URLs to a running jdownloader2 instance to download
+--jdownloader-username username to login to jdownloader --jdownloader-password
+password to login to jdownloader --jdownloader-device device name to login to
+for jdownloader --hide-new-progress disables the new rich progress entirely and
 uses older methods --hide-overall-progress removes overall progress section
 while downloading --hide-forum-progress removes forum progress section while
 downloading --hide-thread-progress removes thread progress section while
 downloading --hide-domain-progress removes domain progress section while
 downloading --hide-album-progress removes album progress section while
 downloading --hide-file-progress removes file progress section while
 downloading --refresh-rate changes the refresh rate of the progress table --
 visible-rows-threads number of visible rows to use for the threads table --
 visible-rows-domains number of visible rows to use for the domains table --
 visible-rows-albums number of visible rows to use for the albums table --
 visible-rows-files number of visible rows to use for the files table ``` `--
 only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
-"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
-"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
-"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
-"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
-"socialmediagirls", "xbunker", "xbunkr"`
+"coomer.party", "coomer.su", "cyberdrop", "cyberfile", "e-hentai", "erome",
+"fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi",
+"imgbox", "jpg.church", "jpg.fish", "jpg.fishing", "jpg.pet", "kemono.party",
+"lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li",
+"postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.2.96/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.97/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.96/setup.cfg` & `cyberdrop-dl-4.2.97/setup.cfg`

 * *Files identical despite different names*

