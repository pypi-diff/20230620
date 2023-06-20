# Comparing `tmp/playwrightcapture-1.20.6.tar.gz` & `tmp/playwrightcapture-1.20.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.20.6.tar", max compression
+gzip compressed data, was "playwrightcapture-1.20.7.tar", max compression
```

## Comparing `playwrightcapture-1.20.6.tar` & `playwrightcapture-1.20.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.6/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.6/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.6/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    36868 2023-06-19 09:52:41.331440 playwrightcapture-1.20.6/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.6/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.6/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.6/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1828 2023-06-19 14:49:16.933781 playwrightcapture-1.20.6/pyproject.toml
--rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.20.6/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.7/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.7/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.7/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    36999 2023-06-20 10:33:48.545728 playwrightcapture-1.20.7/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.7/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.7/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.7/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1828 2023-06-20 10:37:46.358743 playwrightcapture-1.20.7/pyproject.toml
+-rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.20.7/PKG-INFO
```

### Comparing `playwrightcapture-1.20.6/LICENSE` & `playwrightcapture-1.20.7/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.6/README.md` & `playwrightcapture-1.20.7/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.6/playwrightcapture/capture.py` & `playwrightcapture-1.20.7/playwrightcapture/capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,17 +421,16 @@
             parsed_url = urlparse(url, allow_fragments=True)
 
             try:
                 # NOTE 2022-12-02: allow 15s less than the general timeout to get a DOM
                 await page.goto(url, wait_until='domcontentloaded', timeout=self.general_timeout - 15000, referer=referer if referer else '')
             except Error as initial_error:
                 self._update_exceptions(initial_error)
-                if self._exception_is_network_error(initial_error):
-                    raise initial_error
-                elif initial_error.name == 'Download is starting':
+                # So this one is really annoying: chromium raises a net::ERR_ABORTED when it hits a download
+                if initial_error.name in ['Download is starting', 'net::ERR_ABORTED']:
                     # page.goto failed, but it triggered a download event.
                     # Let's re-trigger it.
                     try:
                         async with page.expect_download(timeout=self.general_timeout - 15000) as download_info:
                             try:
                                 await page.goto(url, timeout=self.general_timeout - 15000, referer=referer if referer else '')
                             except Exception:
@@ -452,14 +451,16 @@
                             if not error_msg:
                                 raise e
                             to_return['error'] = f"Error while downloading: {error_msg}"
                             self.logger.info(to_return['error'])
                             self.should_retry = True
                         except Exception:
                             raise e
+                elif self._exception_is_network_error(initial_error):
+                    raise initial_error
             else:
                 await page.bring_to_front()
 
                 # page instrumentation
                 await page.wait_for_timeout(5000)  # Wait 5 sec after document loaded
 
                 # ==== recaptcha
```

### Comparing `playwrightcapture-1.20.6/playwrightcapture/helpers.py` & `playwrightcapture-1.20.7/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.6/pyproject.toml` & `playwrightcapture-1.20.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.20.6"
+version = "1.20.7"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
```

### Comparing `playwrightcapture-1.20.6/PKG-INFO` & `playwrightcapture-1.20.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.20.6
+Version: 1.20.7
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

