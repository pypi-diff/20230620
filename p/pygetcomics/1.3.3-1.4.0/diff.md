# Comparing `tmp/pygetcomics-1.3.3.tar.gz` & `tmp/pygetcomics-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygetcomics-1.3.3.tar", max compression
+gzip compressed data, was "pygetcomics-1.4.0.tar", max compression
```

## Comparing `pygetcomics-1.3.3.tar` & `pygetcomics-1.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1323 2017-01-14 11:37:10.942799 pygetcomics-1.3.3/LICENSE
--rw-r--r--   0        0        0       73 2018-09-02 10:16:15.940076 pygetcomics-1.3.3/README.rst
--rw-r--r--   0        0        0      638 2023-06-10 19:44:37.513034 pygetcomics-1.3.3/berhoel/__init__.py
--rw-r--r--   0        0        0     1362 2023-03-18 17:04:23.687285 pygetcomics-1.3.3/berhoel/get_comics/__init__.py
--rw-r--r--   0        0        0     1732 2023-03-19 18:35:26.907425 pygetcomics-1.3.3/berhoel/get_comics/garfield/__init__.py
--rw-r--r--   0        0        0     2430 2023-03-19 18:37:25.695432 pygetcomics-1.3.3/berhoel/get_comics/gen_pdf/__init__.py
--rw-r--r--   0        0        0     1363 2017-01-22 21:50:10.690581 pygetcomics-1.3.3/berhoel/get_comics/gen_pdf/template/book.tex
--rw-r--r--   0        0        0     9164 2023-06-13 18:34:28.970218 pygetcomics-1.3.3/berhoel/get_comics/gocomics/__init__.py
--rw-r--r--   0        0        0     3591 2022-08-09 15:38:07.250228 pygetcomics-1.3.3/berhoel/get_comics/peanuts/__init__.py
--rw-r--r--   0        0        0     1186 2022-08-09 15:01:30.240906 pygetcomics-1.3.3/berhoel/get_comics/peanuts/clean_up.py
--rw-r--r--   0        0        0     5507 2023-03-19 18:38:06.927435 pygetcomics-1.3.3/berhoel/get_comics/peanuts/gen_book.py
--rw-r--r--   0        0        0     1160 2022-08-09 15:51:27.853290 pygetcomics-1.3.3/berhoel/get_comics/tests/test_get_comics.py
--rw-r--r--   0        0        0     2491 2023-06-13 18:34:58.946213 pygetcomics-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 pygetcomics-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1323 2017-01-14 11:37:10.942799 pygetcomics-1.4.0/LICENSE
+-rw-r--r--   0        0        0       73 2018-09-02 10:16:15.940076 pygetcomics-1.4.0/README.rst
+-rw-r--r--   0        0        0      638 2023-06-10 19:44:37.513034 pygetcomics-1.4.0/berhoel/__init__.py
+-rw-r--r--   0        0        0     1362 2023-03-18 17:04:23.687285 pygetcomics-1.4.0/berhoel/get_comics/__init__.py
+-rw-r--r--   0        0        0     1732 2023-03-19 18:35:26.907425 pygetcomics-1.4.0/berhoel/get_comics/garfield/__init__.py
+-rw-r--r--   0        0        0     2430 2023-03-19 18:37:25.695432 pygetcomics-1.4.0/berhoel/get_comics/gen_pdf/__init__.py
+-rw-r--r--   0        0        0     1363 2017-01-22 21:50:10.690581 pygetcomics-1.4.0/berhoel/get_comics/gen_pdf/template/book.tex
+-rw-r--r--   0        0        0     8543 2023-06-20 19:57:11.318498 pygetcomics-1.4.0/berhoel/get_comics/gocomics/__init__.py
+-rw-r--r--   0        0        0     3591 2022-08-09 15:38:07.250228 pygetcomics-1.4.0/berhoel/get_comics/peanuts/__init__.py
+-rw-r--r--   0        0        0     1186 2022-08-09 15:01:30.240906 pygetcomics-1.4.0/berhoel/get_comics/peanuts/clean_up.py
+-rw-r--r--   0        0        0     5507 2023-03-19 18:38:06.927435 pygetcomics-1.4.0/berhoel/get_comics/peanuts/gen_book.py
+-rw-r--r--   0        0        0     1160 2022-08-09 15:51:27.853290 pygetcomics-1.4.0/berhoel/get_comics/tests/test_get_comics.py
+-rw-r--r--   0        0        0     2491 2023-06-20 19:58:58.538570 pygetcomics-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 pygetcomics-1.4.0/PKG-INFO
```

### Comparing `pygetcomics-1.3.3/LICENSE` & `pygetcomics-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.3/berhoel/__init__.py` & `pygetcomics-1.4.0/berhoel/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.3/berhoel/get_comics/__init__.py` & `pygetcomics-1.4.0/berhoel/get_comics/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.3/berhoel/get_comics/garfield/__init__.py` & `pygetcomics-1.4.0/berhoel/get_comics/garfield/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.3/berhoel/get_comics/gen_pdf/__init__.py` & `pygetcomics-1.4.0/berhoel/get_comics/gen_pdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.3/berhoel/get_comics/gen_pdf/template/book.tex` & `pygetcomics-1.4.0/berhoel/get_comics/gen_pdf/template/book.tex`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.3/berhoel/get_comics/gocomics/__init__.py` & `pygetcomics-1.4.0/berhoel/get_comics/gocomics/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,54 +23,41 @@
 # Third party library imports.
 from selenium import webdriver
 from lxml.html import fromstring
 from selenium.webdriver.common import action_chains
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.chrome.options import Options
 
-__date__ = "2023/06/13 20:34:28 hoel"
+__date__ = "2023/06/20 21:57:10 hoel"
 __author__ = "Berthold Höllmann"
 __copyright__ = "Copyright © 2011-2017 by Berthold Höllmann"
 __credits__ = ["Berthold Höllmann"]
 __maintainer__ = "Berthold Höllmann"
 __email__ = "berhoel@gmail.com"
 
 FILE_MODE = stat.S_IRUSR | stat.S_IWUSR | stat.S_IRGRP | stat.S_IROTH
 TOUCH_FMT = "%Y%m%d0300"
 
 
-class SeleniumSingleton(object):
+class SeleniumSingleton:
     __instance = None
 
     def __init__(self):
         """Virtually private constructor."""
+        self.driver = None
         if SeleniumSingleton.__instance is None:
-            driverpath = None
-            for path in [
-                Path(i)
-                for i in (
-                    "/usr/bin/",
-                    "/usr/lib64/chromium/",
-                    "/usr/lib/chromium-browser",
-                )
-            ]:
-                if (driverpath := path / "chromedriver").is_file():
-                    break
-
             # https://stackoverflow.com/questions/46920243/how-to-configure-chromedriver-to-initiate-chrome-browser-in-headless-mode-throug
             options = Options()
             options.add_argument("--headless")
             options.binary_location = "/usr/bin/google-chrome-stable"
             if os.name == "nt":
                 options.add_argument(
                     "--disable-gpu"
                 )  # Last I checked this was necessary.
-            self.driver = webdriver.Chrome(
-                executable_path=driverpath, chrome_options=options
-            )
+            self.driver = webdriver.Chrome(options)
             self.driver.get("http://www.gocomics.com/")
             if self.driver.current_url.startswith("https://login.microsoftonline.com/"):
                 self.ms_login()
             SeleniumSingleton.__instance = self
         else:
             raise Exception("This class is a singleton!")
 
@@ -96,24 +83,16 @@
     @staticmethod
     def get_instance():
         """Static access method."""
         if SeleniumSingleton.__instance is None:
             SeleniumSingleton()
         return SeleniumSingleton.__instance
 
-    def close(self):
-        self.driver.close()
-        SeleniumSingleton.__instance = None
-
-    def __del__(self):
-        self.driver.close()
-        SeleniumSingleton.__instance = None
-
 
-class SaveState(object):
+class SaveState:
     "Save state information on already downloaded files and dates tried"
 
     def __init__(self):
         self.loaded = {}
         self.tried = {}
         self.downloaded = [0, 0, 0, 0]
 
@@ -135,15 +114,15 @@
             | stat.S_IROTH
             | stat.S_IXOTH
         )
         path.mkdir(mode=mode, parents=True)
         path.chmod(mode)
 
 
-class GoComics(object):
+class GoComics:
     """Download comics from GoComics."""
 
     start_year = -1
     start_month = -1
     start_day = -1
 
     skip = {}
```

### Comparing `pygetcomics-1.3.3/berhoel/get_comics/peanuts/__init__.py` & `pygetcomics-1.4.0/berhoel/get_comics/peanuts/__init__.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.3/berhoel/get_comics/peanuts/clean_up.py` & `pygetcomics-1.4.0/berhoel/get_comics/peanuts/clean_up.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.3/berhoel/get_comics/peanuts/gen_book.py` & `pygetcomics-1.4.0/berhoel/get_comics/peanuts/gen_book.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.3/berhoel/get_comics/tests/test_get_comics.py` & `pygetcomics-1.4.0/berhoel/get_comics/tests/test_get_comics.py`

 * *Files identical despite different names*

### Comparing `pygetcomics-1.3.3/pyproject.toml` & `pygetcomics-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyGetComics"
-version = "1.3.3"
+version = "1.4.0"
 
 description = "Download various daily comics."
 
 packages = [
     { include = "berhoel" },
 ]
```

### Comparing `pygetcomics-1.3.3/PKG-INFO` & `pygetcomics-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygetcomics
-Version: 1.3.3
+Version: 1.4.0
 Summary: Download various daily comics.
 Home-page: https://gitlab.com/berhoel/python/pyGetComics.git
 License: BSD-2-Clause
 Author: Berthold Höllmann
 Author-email: berhoel@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

