# Comparing `tmp/amazon-scraper-toolkit-1.0.0.tar.gz` & `tmp/amazon-scraper-toolkit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-scraper-toolkit-1.0.0.tar", last modified: Mon Jun 19 14:20:05 2023, max compression
+gzip compressed data, was "amazon-scraper-toolkit-1.0.1.tar", last modified: Tue Jun 20 10:13:34 2023, max compression
```

## Comparing `amazon-scraper-toolkit-1.0.0.tar` & `amazon-scraper-toolkit-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 14:20:05.446330 amazon-scraper-toolkit-1.0.0/
--rw-rw-rw-   0        0        0     1100 2023-06-05 04:51:21.000000 amazon-scraper-toolkit-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2026 2023-06-19 14:20:05.446330 amazon-scraper-toolkit-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-04 02:35:50.000000 amazon-scraper-toolkit-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 14:20:05.425937 amazon-scraper-toolkit-1.0.0/amazon_scrape_toolkit/
--rw-rw-rw-   0        0        0      138 2023-06-04 02:23:01.000000 amazon-scraper-toolkit-1.0.0/amazon_scrape_toolkit/__init__.py
--rw-rw-rw-   0        0        0    12265 2023-06-19 14:02:48.000000 amazon-scraper-toolkit-1.0.0/amazon_scrape_toolkit/main.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:20:05.446330 amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/
--rw-rw-rw-   0        0        0     2026 2023-06-19 14:20:05.000000 amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-06-19 14:20:05.000000 amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 14:20:05.000000 amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-19 14:20:05.000000 amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-19 14:20:05.000000 amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1353 2023-06-19 14:18:27.000000 amazon-scraper-toolkit-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 14:20:05.452042 amazon-scraper-toolkit-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 10:13:34.709078 amazon-scraper-toolkit-1.0.1/
+-rw-rw-rw-   0        0        0     1100 2023-06-05 04:51:21.000000 amazon-scraper-toolkit-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2026 2023-06-20 10:13:34.707077 amazon-scraper-toolkit-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-04 02:35:50.000000 amazon-scraper-toolkit-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 10:13:34.691089 amazon-scraper-toolkit-1.0.1/amazon_scrape_toolkit/
+-rw-rw-rw-   0        0        0      138 2023-06-04 02:23:01.000000 amazon-scraper-toolkit-1.0.1/amazon_scrape_toolkit/__init__.py
+-rw-rw-rw-   0        0        0    12362 2023-06-20 04:19:03.000000 amazon-scraper-toolkit-1.0.1/amazon_scrape_toolkit/main.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:13:34.705078 amazon-scraper-toolkit-1.0.1/amazon_scraper_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     2026 2023-06-20 10:13:34.000000 amazon-scraper-toolkit-1.0.1/amazon_scraper_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-06-20 10:13:34.000000 amazon-scraper-toolkit-1.0.1/amazon_scraper_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:13:34.000000 amazon-scraper-toolkit-1.0.1/amazon_scraper_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-20 10:13:34.000000 amazon-scraper-toolkit-1.0.1/amazon_scraper_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-20 10:13:34.000000 amazon-scraper-toolkit-1.0.1/amazon_scraper_toolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1076 2023-06-20 04:26:41.000000 amazon-scraper-toolkit-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 10:13:34.709516 amazon-scraper-toolkit-1.0.1/setup.cfg
```

### Comparing `amazon-scraper-toolkit-1.0.0/LICENSE` & `amazon-scraper-toolkit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-scraper-toolkit-1.0.0/PKG-INFO` & `amazon-scraper-toolkit-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-scraper-toolkit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Some Helpful Classes and Functions for Scraping Amazon Data
 Author: Tejas
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `amazon-scraper-toolkit-1.0.0/amazon_scrape_toolkit/main.py` & `amazon-scraper-toolkit-1.0.1/amazon_scrape_toolkit/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 @dataclass
 class ProductInfo:
     """Data class representing the information of a product"""
 
     other_products: list[str]
-    ratings: dict[str:int]
+    ratings: dict[str, int]
     data: dict
     custom_scraper_time_taken: float
     ratings_scraper_time_taken: float
     more_phones_scraper_time_taken: float
 
 
 def timer():
@@ -165,18 +165,22 @@
     """
 
     def inner_decorator(func):
         @wraps(func)
         def _wrapper(soup: bs4.BeautifulSoup, product_id: str, *args, **kwargs):
             data_func_timer = timer()
             next(data_func_timer)
-            data = func(soup, product_id, *args, **kwargs)
+            try:
+                data = func(soup, product_id, *args, **kwargs)
+            except Exception:
+                data = None
+
             assert data is None or isinstance(
-                data, dict
-            ), "Output should be Dict or None!"
+                    data, dict
+                    ), "Output should be Dict or None!"
 
             if data is None:
                 logger.info(f"page_failed [{product_id}]")
                 return None
 
             data_func_timer = next(data_func_timer)
             new_phones_to_add = [] if get_others else None
```

### Comparing `amazon-scraper-toolkit-1.0.0/amazon_scraper_toolkit.egg-info/PKG-INFO` & `amazon-scraper-toolkit-1.0.1/amazon_scraper_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-scraper-toolkit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Some Helpful Classes and Functions for Scraping Amazon Data
 Author: Tejas
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `amazon-scraper-toolkit-1.0.0/pyproject.toml` & `amazon-scraper-toolkit-1.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amazon-scraper-toolkit"
-version = "1.0.0"
+version = "1.0.1"
 description = "Some Helpful Classes and Functions for Scraping Amazon Data"
 readme = "README.md"
 authors = [{ name = "Tejas" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
@@ -30,19 +30,7 @@
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "pylint", "pep8"]
 
 [project.urls]
 Homepage = "https://github.com/KidCoderT/amazon-scraper"
-
-[tool.bumpver]
-current_version = "1.0.0"
-version_pattern = "MAJOR.MINOR.PATCH"
-commit_message = "bump version {old_version} -> {new_version}"
-commit = true
-tag = true
-push = false
-
-[tool.bumpver.file_patterns]
-"pyproject.toml" = ['current_version = "{version}"']
-
```

