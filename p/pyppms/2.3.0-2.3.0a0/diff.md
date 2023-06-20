# Comparing `tmp/pyppms-2.3.0.tar.gz` & `tmp/pyppms-2.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppms-2.3.0.tar", max compression
+gzip compressed data, was "pyppms-2.3.0a0.tar", max compression
```

## Comparing `pyppms-2.3.0.tar` & `pyppms-2.3.0a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-2.3.0/README.md
--rw-r--r--   0        0        0     1113 2023-06-20 08:30:15.274443 pyppms-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-2.3.0/src/pyppms/__init__.py
--rw-r--r--   0        0        0     5609 2023-04-26 16:03:26.526029 pyppms-2.3.0/src/pyppms/booking.py
--rw-r--r--   0        0        0     7051 2022-04-19 16:41:02.244253 pyppms-2.3.0/src/pyppms/common.py
--rw-r--r--   0        0        0    46935 2023-06-20 08:29:51.536287 pyppms-2.3.0/src/pyppms/ppms.py
--rw-r--r--   0        0        0     3961 2023-04-26 16:03:26.526029 pyppms-2.3.0/src/pyppms/system.py
--rw-r--r--   0        0        0     2287 2022-04-20 14:50:49.117838 pyppms-2.3.0/src/pyppms/user.py
--rw-r--r--   0        0        0     3787 1970-01-01 00:00:00.000000 pyppms-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-2.3.0a0/README.md
+-rw-r--r--   0        0        0     1115 2023-06-19 20:15:36.108800 pyppms-2.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-2.3.0a0/src/pyppms/__init__.py
+-rw-r--r--   0        0        0     5609 2023-04-26 16:03:26.526029 pyppms-2.3.0a0/src/pyppms/booking.py
+-rw-r--r--   0        0        0     7051 2022-04-19 16:41:02.244253 pyppms-2.3.0a0/src/pyppms/common.py
+-rw-r--r--   0        0        0    46371 2023-06-19 20:08:14.598898 pyppms-2.3.0a0/src/pyppms/ppms.py
+-rw-r--r--   0        0        0     3961 2023-04-26 16:03:26.526029 pyppms-2.3.0a0/src/pyppms/system.py
+-rw-r--r--   0        0        0     2287 2022-04-20 14:50:49.117838 pyppms-2.3.0a0/src/pyppms/user.py
+-rw-r--r--   0        0        0     3789 1970-01-01 00:00:00.000000 pyppms-2.3.0a0/PKG-INFO
```

### Comparing `pyppms-2.3.0/README.md` & `pyppms-2.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `pyppms-2.3.0/pyproject.toml` & `pyppms-2.3.0a0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 description = "A Python package to communicate with Stratocore's PUMAPI."
 name = "pyppms"
-version = "2.3.0"
+version = "2.3.0a0"
 
 license = "GPLv3"
 
 authors = [
   "Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>",
   "Laurent Guerard <laurent.guerard@unibas.ch>",
 ]
```

### Comparing `pyppms-2.3.0/src/pyppms/booking.py` & `pyppms-2.3.0a0/src/pyppms/booking.py`

 * *Files identical despite different names*

### Comparing `pyppms-2.3.0/src/pyppms/common.py` & `pyppms-2.3.0a0/src/pyppms/common.py`

 * *Files identical despite different names*

### Comparing `pyppms-2.3.0/src/pyppms/ppms.py` & `pyppms-2.3.0a0/src/pyppms/ppms.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         object's lifetime (can be empty if no calls to the :py:meth:`get_systems()` have
         been done yet).
     status : dict
         A dict with keys ``auth_state``, ``auth_response`` and
         ``auth_httpstatus``
     """
 
-    def __init__(self, url, api_key, timeout=10, cache="", cache_users_only=False):
+    def __init__(self, url, api_key, timeout=10, cache=""):
         """Constructor for the PPMS connection object.
 
         Open a connection to the PUMAPI defined in `url` and try to authenticate
         against it using the given API key (or use cache-only mode if key is an
         empty string). If an optional path to a caching location is specified,
         responses will be read from that location unless no matching file can be
         found there, in which case an on-line request will be done (with the
@@ -79,19 +79,14 @@
             How many seconds to wait for the PUMAPI server to send a response
             before giving up, by default 10.
         cache : str, optional
             A path to a local directory for caching responses from PUMAPI in
             individual text files. Useful for testing and for speeding up
             slow requests like 'getusers'. By default empty, which will result
             in no caching being done.
-        cache_users_only : bool, optional
-            If set to `True`, only `getuser` requests will be cached on disk.
-            This can be used in to speed up the slow requests (through the
-            cache), while everything else will be handled through online
-            requests. By default `False`.
 
         Raises
         ------
         requests.exceptions.ConnectionError
             Raised in case authentication fails.
         """
         self.url = url
@@ -102,15 +97,14 @@
         self.systems = {}
         self.status = {
             "auth_state": "NOT_TRIED",
             "auth_response": None,
             "auth_httpstatus": -1,
         }
         self.cache_path = cache
-        self.cache_users_only = cache_users_only
 
         # run in cache-only mode (e.g. for testing or off-line usage) if no API
         # key has been specified, skip authentication then:
         if api_key != "":
             self.__authenticate()
         elif cache == "":
             raise RuntimeError(
@@ -243,19 +237,14 @@
         Returns
         -------
         str
             The full path to a file name identified by all parameters of the
             request (except credentials like 'apikey').
         """
         action = req_data["action"]
-
-        if self.cache_users_only and action != "getuser":
-            LOG.debug(f"NOT caching '{action}' (cache_users_only is set)")
-            return None
-
         intercept_dir = os.path.join(self.cache_path, action)
         if create_dir and not os.path.exists(intercept_dir):  # pragma: no cover
             try:
                 os.makedirs(intercept_dir)
                 LOG.debug("Created dir to store response: %s", intercept_dir)
             except Exception as err:  # pylint: disable-msg=broad-except
                 LOG.warning("Failed creating [%s]: %s", intercept_dir, err)
@@ -307,15 +296,15 @@
                 self.text = text
                 self.status_code = int(status_code)
 
         if self.cache_path == "":
             raise LookupError("No cache path configured")
 
         intercept_file = self.__interception_path(req_data, create_dir=False)
-        if not intercept_file or not os.path.exists(intercept_file):  # pragma: no cover
+        if not os.path.exists(intercept_file):  # pragma: no cover
             raise LookupError(f"No cache hit for [{intercept_file}]")
 
         with open(intercept_file, "r", encoding="utf-8") as infile:
             text = infile.read()
         LOG.debug("Read intercepted response text from [%s]", intercept_file)
 
         status_code = 200
```

### Comparing `pyppms-2.3.0/src/pyppms/system.py` & `pyppms-2.3.0a0/src/pyppms/system.py`

 * *Files identical despite different names*

### Comparing `pyppms-2.3.0/src/pyppms/user.py` & `pyppms-2.3.0a0/src/pyppms/user.py`

 * *Files identical despite different names*

### Comparing `pyppms-2.3.0/PKG-INFO` & `pyppms-2.3.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppms
-Version: 2.3.0
+Version: 2.3.0a0
 Summary: A Python package to communicate with Stratocore's PUMAPI.
 Home-page: https://pypi.org/project/pyppms/
 License: GPLv3
 Keywords: ppms,pumapi,booking-system,reservation-system
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.8,<4.0
```

