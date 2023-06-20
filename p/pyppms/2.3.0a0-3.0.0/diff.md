# Comparing `tmp/pyppms-2.3.0a0.tar.gz` & `tmp/pyppms-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppms-2.3.0a0.tar", max compression
+gzip compressed data, was "pyppms-3.0.0.tar", max compression
```

## Comparing `pyppms-2.3.0a0.tar` & `pyppms-3.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-2.3.0a0/README.md
--rw-r--r--   0        0        0     1115 2023-06-19 20:15:36.108800 pyppms-2.3.0a0/pyproject.toml
--rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-2.3.0a0/src/pyppms/__init__.py
--rw-r--r--   0        0        0     5609 2023-04-26 16:03:26.526029 pyppms-2.3.0a0/src/pyppms/booking.py
--rw-r--r--   0        0        0     7051 2022-04-19 16:41:02.244253 pyppms-2.3.0a0/src/pyppms/common.py
--rw-r--r--   0        0        0    46371 2023-06-19 20:08:14.598898 pyppms-2.3.0a0/src/pyppms/ppms.py
--rw-r--r--   0        0        0     3961 2023-04-26 16:03:26.526029 pyppms-2.3.0a0/src/pyppms/system.py
--rw-r--r--   0        0        0     2287 2022-04-20 14:50:49.117838 pyppms-2.3.0a0/src/pyppms/user.py
--rw-r--r--   0        0        0     3789 1970-01-01 00:00:00.000000 pyppms-2.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0     2942 2022-04-20 07:35:38.348949 pyppms-3.0.0/README.md
+-rw-r--r--   0        0        0     1146 2023-06-20 11:18:22.862069 pyppms-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      231 2023-04-26 16:03:26.526029 pyppms-3.0.0/src/pyppms/__init__.py
+-rw-r--r--   0        0        0     5593 2023-06-20 11:17:40.005575 pyppms-3.0.0/src/pyppms/booking.py
+-rw-r--r--   0        0        0     7035 2023-06-20 11:17:40.005575 pyppms-3.0.0/src/pyppms/common.py
+-rw-r--r--   0        0        0    46975 2023-06-20 11:17:40.009575 pyppms-3.0.0/src/pyppms/ppms.py
+-rw-r--r--   0        0        0     3944 2023-06-20 11:17:40.009575 pyppms-3.0.0/src/pyppms/system.py
+-rw-r--r--   0        0        0     2270 2023-06-20 11:17:40.009575 pyppms-3.0.0/src/pyppms/user.py
+-rw-r--r--   0        0        0     3776 1970-01-01 00:00:00.000000 pyppms-3.0.0/PKG-INFO
```

### Comparing `pyppms-2.3.0a0/README.md` & `pyppms-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyppms-2.3.0a0/pyproject.toml` & `pyppms-3.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 description = "A Python package to communicate with Stratocore's PUMAPI."
 name = "pyppms"
-version = "2.3.0a0"
+version = "3.0.0"
 
 license = "GPLv3"
 
 authors = [
   "Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>",
   "Laurent Guerard <laurent.guerard@unibas.ch>",
 ]
@@ -14,25 +14,26 @@
 
 documentation = "https://imcf.one/apidocs/pyppms/pyppms.html"
 homepage = "https://pypi.org/project/pyppms/"
 keywords = ["ppms", "pumapi", "booking-system", "reservation-system"]
 repository = "https://github.com/imcf/pyppms"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-requests = "^2.25.1"
-
-[tool.poetry.dev-dependencies]
-PyYAML = "^6.0"
-black = "^22.0"
-pdoc = "^10.0"
-pylint = "^2.9.3"
+python = "^3.9"
+requests = "^2.31.0"
+loguru = "^0.7.0"
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+pdoc = "^14.0.0"
+pylint = "^2.17.4"
 pylint-pytest = "^1.1.2"
-pytest = "^7.0"
-pytest-cov = "^3.0"
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
+pyyaml = "^6.0"
 
 [build-system]
 build-backend = "poetry_dynamic_versioning.backend"
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `pyppms-2.3.0a0/src/pyppms/booking.py` & `pyppms-3.0.0/src/pyppms/booking.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Module representing bookings / reservations in PPMS."""
 
-import logging
 from datetime import datetime
 
-from .common import time_rel_to_abs
+from loguru import logger as log
 
-LOG = logging.getLogger(__name__)
+from .common import time_rel_to_abs
 
 
 class PpmsBooking:
 
     """Object representing a booking (reservation) in PPMS.
 
     Attributes
@@ -58,18 +57,18 @@
 
             self.username = lines[0]
             self.system_id = int(system_id)
             self.starttime = starttime
             self.endtime = endtime
             self.session = lines[2]
         except Exception as err:
-            LOG.error("Parsing booking response failed (%s), text was:\n%s", err, text)
+            log.error("Parsing booking response failed ({}), text was:\n{}", err, text)
             raise
 
-        LOG.debug(str(self))
+        log.trace(str(self))
 
     @classmethod
     def from_runningsheet(cls, entry, system_id, username, date):
         """Alternative constructor using a (parsed) getrunningsheet response.
 
         Parameters
         ----------
@@ -92,16 +91,16 @@
         """
         try:
             response = f"{username}\n0\n\n"
             booking = cls(response, "get", system_id)
             booking.starttime_fromstr(entry["Start time"], date)
             booking.endtime_fromstr(entry["End time"], date)
         except Exception as err:
-            LOG.error(
-                "Parsing runningsheet entry failed (%s), text was:\n%s", err, entry
+            log.error(
+                "Parsing runningsheet entry failed ({}), text was:\n{}", err, entry
             )
             raise
 
         return booking
 
     def starttime_fromstr(self, time_str, date=None):
         """Change the starting time and / or day of a booking.
@@ -119,15 +118,15 @@
         start = date.replace(
             hour=int(time_str.split(":")[0]),
             minute=int(time_str.split(":")[1]),
             second=0,
             microsecond=0,
         )
         self.starttime = start
-        LOG.debug("New starttime: %s", self)
+        log.debug("New starttime: {}", self)
 
     def endtime_fromstr(self, time_str, date=None):
         """Change the ending time and / or day of a booking.
 
         Parameters
         ----------
         time_str : str
@@ -141,15 +140,15 @@
         end = date.replace(
             hour=int(time_str.split(":")[0]),
             minute=int(time_str.split(":")[1]),
             second=0,
             microsecond=0,
         )
         self.endtime = end
-        LOG.debug("New endtime: %s", self)
+        log.debug("New endtime: {}", self)
 
     def __str__(self):
         def fmt_time(time):
             # in case a booking was created from a "nextbooking" response it will not
             # have the `endtime` attribute set, so treat this separately:
             if time is None:
                 return "===UNDEFINED==="
```

### Comparing `pyppms-2.3.0a0/src/pyppms/common.py` & `pyppms-3.0.0/src/pyppms/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Common functions related to Stratocore's PPMS Utility Management API."""
 
 # pylint: disable-msg=fixme
 
 from datetime import datetime, timedelta
-import logging
 import csv
 from io import StringIO
 
-LOG = logging.getLogger(__name__)
+from loguru import logger as log
 
 
 def process_response_values(values):
     """Process (in-place) a list of strings, remove quotes, detect boolean etc.
 
     Check all (str) elements of the given list, remove surrounding double-quotes
     and convert 'true' / 'false' strings into Python booleans.
@@ -70,36 +69,36 @@
     # TODO: this should probably rather raise a ValueError but we need to test
     # all effects on existing code first!
     if text == "\n\n":
         return {"": ""}
     try:
         lines = list(csv.reader(StringIO(text), delimiter=","))
         if len(lines) != 2:
-            LOG.warning("Response expected to have exactly two lines: %s", text)
+            log.warning("Response expected to have exactly two lines: {}", text)
             if not graceful:
                 raise ValueError("Invalid response format!")
         header = lines[0]
         data = lines[1]
         process_response_values(data)
         if len(header) != len(data):
             msg = "Parsing CSV failed, mismatch of header vs. data fields count"
-            LOG.warning("%s (%s vs. %s)", msg, len(header), len(data))
+            log.warning("{} ({} vs. {})", msg, len(header), len(data))
             if not graceful:
                 raise ValueError(msg)
             minimum = min(len(header), len(data))
             if minimum < len(header):
-                LOG.warning("Discarding header-fields: %s", header[minimum:])
+                log.warning("Discarding header-fields: {}", header[minimum:])
                 header = header[:minimum]
             else:
-                LOG.warning("Discarding data-fields: %s", data[minimum:])
+                log.warning("Discarding data-fields: {}", data[minimum:])
                 data = data[:minimum]
 
     except Exception as err:
         msg = f"Unable to parse data returned by PUMAPI: {text} - ERROR: {err}"
-        LOG.error(msg)
+        log.error(msg)
         raise ValueError(msg) from err
 
     parsed = dict(zip(header, data))
     return parsed
 
 
 def parse_multiline_response(text, graceful=True):
@@ -131,15 +130,15 @@
         parameter has been set to false, or if parsing fails for any other
         unforeseen reason.
     """
     parsed = []
     try:
         lines = text.splitlines()
         if len(lines) < 2:
-            LOG.warning("Response expected to have two or more lines: %s", text)
+            log.warning("Response expected to have two or more lines: {}", text)
             if not graceful:
                 raise ValueError("Invalid response format!")
             return parsed
 
         header = lines[0].split(",")
         for i, entry in enumerate(header):
             header[i] = entry.strip()
@@ -148,40 +147,40 @@
         for line in lines[1:]:
             data = line.split(",")
             process_response_values(data)
             lines_max = max(lines_max, len(data))
             lines_min = min(lines_min, len(data))
             if len(header) != len(data):
                 msg = "Parsing CSV failed, mismatch of header vs. data fields count"
-                LOG.warning("%s (%s vs. %s)", msg, len(header), len(data))
+                log.warning("{} ({} vs. {})", msg, len(header), len(data))
                 if not graceful:
                     raise ValueError(msg)
 
                 minimum = min(len(header), len(data))
                 if minimum < len(header):
-                    LOG.warning("Discarding header-fields: %s", header[minimum:])
+                    log.warning("Discarding header-fields: {}", header[minimum:])
                     header = header[:minimum]
                 else:
-                    LOG.warning("Discarding data-fields: %s", data[minimum:])
+                    log.warning("Discarding data-fields: {}", data[minimum:])
                     data = data[:minimum]
 
             details = dict(zip(header, data))
-            # LOG.debug(details)
+            # log.debug(details)
             parsed.append(details)
 
         if lines_min != lines_max:
             msg = (
                 "Inconsistent data detected, not all dicts will have the "
                 "same number of elements!"
             )
-            LOG.warning(msg)
+            log.warning(msg)
 
     except Exception as err:
         msg = f"Unable to parse data returned by PUMAPI: {text} - ERROR: {err}"
-        LOG.error(msg)
+        log.error(msg)
         raise ValueError(msg) from err
 
     return parsed
 
 
 def time_rel_to_abs(minutes_from_now):
     """Convert a relative time given in minutes from now to a datetime object.
```

### Comparing `pyppms-2.3.0a0/src/pyppms/ppms.py` & `pyppms-3.0.0/src/pyppms/ppms.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,45 +4,45 @@
 
 # NOTE: the "pyppms" package is simply a wrapper for the existing API, so we can't make
 #       any design decisions here - hence it is pointless to complain about the number
 #       of instance attributes, public methods or other stuff:
 # pylint: disable-msg=too-many-instance-attributes
 # pylint: disable-msg=too-many-public-methods
 
-import logging
 import os
 import os.path
 import shutil
 from io import open
 
 import requests
+from loguru import logger as log
 
 from .common import dict_from_single_response, parse_multiline_response
 from .user import PpmsUser
 from .system import PpmsSystem
 from .booking import PpmsBooking
 
 
-LOG = logging.getLogger(__name__)
-
-
 class PpmsConnection:
 
     """Connection object to communicate with a PPMS instance.
 
     Attributes
     ----------
     url : str
         The URL of the PUMAPI instance.
     api_key : str
         The API key used for authenticating against the PUMAPI.
     timeout : float
         The timeout value used in the ``requests.post`` calls.
     cache_path : str
         A path to a local directory used for caching responses.
+    cache_users_only : bool
+        Flag indicating that only PPMS user details will be stored in the
+        on-disk cache, nothing else.
     users : dict
         A dict with usernames as keys, mapping to the related
         :py:class:`pyppms.user.PpmsUser` object, serves as a cache during the object's
         lifetime (can be empty if no calls to :py:meth:`get_user()` have been done yet).
     fullname_mapping : dict
         A dict mapping a user's *fullname* ("``<LASTNAME> <FIRSTNAME>``") to the
         corresponding username. Entries are filled in dynamically by the
@@ -53,15 +53,15 @@
         object's lifetime (can be empty if no calls to the :py:meth:`get_systems()` have
         been done yet).
     status : dict
         A dict with keys ``auth_state``, ``auth_response`` and
         ``auth_httpstatus``
     """
 
-    def __init__(self, url, api_key, timeout=10, cache=""):
+    def __init__(self, url, api_key, timeout=10, cache="", cache_users_only=False):
         """Constructor for the PPMS connection object.
 
         Open a connection to the PUMAPI defined in `url` and try to authenticate
         against it using the given API key (or use cache-only mode if key is an
         empty string). If an optional path to a caching location is specified,
         responses will be read from that location unless no matching file can be
         found there, in which case an on-line request will be done (with the
@@ -79,14 +79,19 @@
             How many seconds to wait for the PUMAPI server to send a response
             before giving up, by default 10.
         cache : str, optional
             A path to a local directory for caching responses from PUMAPI in
             individual text files. Useful for testing and for speeding up
             slow requests like 'getusers'. By default empty, which will result
             in no caching being done.
+        cache_users_only : bool, optional
+            If set to `True`, only `getuser` requests will be cached on disk.
+            This can be used in to speed up the slow requests (through the
+            cache), while everything else will be handled through online
+            requests. By default `False`.
 
         Raises
         ------
         requests.exceptions.ConnectionError
             Raised in case authentication fails.
         """
         self.url = url
@@ -97,14 +102,15 @@
         self.systems = {}
         self.status = {
             "auth_state": "NOT_TRIED",
             "auth_response": None,
             "auth_httpstatus": -1,
         }
         self.cache_path = cache
+        self.cache_users_only = cache_users_only
 
         # run in cache-only mode (e.g. for testing or off-line usage) if no API
         # key has been specified, skip authentication then:
         if api_key != "":
             self.__authenticate()
         elif cache == "":
             raise RuntimeError(
@@ -115,57 +121,57 @@
         """Try to authenticate to PPMS using the `auth` request.
 
         Raises
         ------
         requests.exceptions.ConnectionError
             Raised in case authentication failed for any reason.
         """
-        LOG.debug(
-            "Attempting authentication against %s with key [%s...%s]",
+        log.debug(
+            "Attempting authentication against {} with key [{}...{}]",
             self.url,
             self.api_key[:2],
             self.api_key[-2:],
         )
         self.status["auth_state"] = "attempting"
         response = self.request("auth")
-        LOG.debug("Authenticate response: %s", response.text)
+        log.debug(f"Authenticate response: {response.text}")
         self.status["auth_response"] = response.text
         self.status["auth_httpstatus"] = response.status_code
 
         # NOTE: an unauthorized request has already been caught be the request() method
         # above. Our legacy code was additionally testing for 'error' in the response
         # text - however, it is unclear if PUMAPI ever returns this:
         if "error" in response.text.lower():
             self.status["auth_state"] = "FAILED-ERROR"
             msg = f"Authentication failed with an error: {response.text}"
-            LOG.error(msg)
+            log.error(msg)
             raise requests.exceptions.ConnectionError(msg)
 
         status_ok = requests.codes.ok  # pylint: disable-msg=no-member
 
         if response.status_code != status_ok:
             # NOTE: branch excluded from coverage as we don't have a known way
             # to produce such a response from the API
-            LOG.warning(
-                "Unexpected combination of response [%s] and status code [%s], it's "
+            log.warning(
+                "Unexpected combination of response [{}] and status code [{}], it's "
                 "unclear if authentication succeeded (assuming it didn't)",
                 response.status_code,
                 response.text,
             )
             self.status["auth_state"] = "FAILED-UNKNOWN"
 
             msg = (
                 f"Authenticating against {self.url} with key "
                 f"[{self.api_key[:2]}...{self.api_key[-2:]}] FAILED!"
             )
-            LOG.error(msg)
+            log.error(msg)
             raise requests.exceptions.ConnectionError(msg)
 
-        LOG.info("Authentication succeeded, response=[%s]", response.text)
-        LOG.debug("HTTP Status: %s", response.status_code)
+        log.info(f"Authentication succeeded, response=[{response.text}]")
+        log.debug(f"HTTP Status: {response.status_code}")
         self.status["auth_state"] = "good"
 
     def request(self, action, parameters={}, skip_cache=False):
         """Generic method to submit a request to PPMS and return the result.
 
         This convenience method deals with adding the API key to a given
         request, submitting it to the PUMAPI and checking the response for some
@@ -191,38 +197,38 @@
         Raises
         ------
         requests.exceptions.ConnectionError
             Raised in case the request is not authorized.
         """
         req_data = {"action": action, "apikey": self.api_key}
         req_data.update(parameters)
-        # LOG.debug("Request parameters: %s", parameters)
+        # log.debug("Request parameters: {}", parameters)
 
         response = None
         read_from_cache = False
         try:
             if skip_cache:  # pragma: no cover
                 raise LookupError("Skipping the cache has been requested")
             response = self.__intercept_read(req_data)
             read_from_cache = True
         except LookupError as err:
-            LOG.debug("Doing an on-line request: %s", err)
+            log.debug(f"Doing an on-line request: {err}")
             response = requests.post(self.url, data=req_data, timeout=self.timeout)
 
         # store the response if it hasn't been read from the cache before:
         if not read_from_cache:  # pragma: no cover
             self.__intercept_store(req_data, response)
 
         # NOTE: the HTTP status code returned is always `200` even if
         # authentication failed, so we need to check the actual response *TEXT*
         # to figure out if we have succeeded:
         if "request not authorized" in response.text.lower():
             self.status["auth_state"] = "FAILED"
             msg = f"Not authorized to run action `{req_data['action']}`"
-            LOG.error(msg)
+            log.error(msg)
             raise requests.exceptions.ConnectionError(msg)
 
         return response
 
     def __interception_path(self, req_data, create_dir=False):
         """Derive the path for a local cache file from a request's parameters.
 
@@ -237,21 +243,26 @@
         Returns
         -------
         str
             The full path to a file name identified by all parameters of the
             request (except credentials like 'apikey').
         """
         action = req_data["action"]
+
+        if self.cache_users_only and action != "getuser":
+            log.debug(f"NOT caching '{action}' (cache_users_only is set)")
+            return None
+
         intercept_dir = os.path.join(self.cache_path, action)
         if create_dir and not os.path.exists(intercept_dir):  # pragma: no cover
             try:
                 os.makedirs(intercept_dir)
-                LOG.debug("Created dir to store response: %s", intercept_dir)
+                log.debug(f"Created dir to store response: {intercept_dir}")
             except Exception as err:  # pylint: disable-msg=broad-except
-                LOG.warning("Failed creating [%s]: %s", intercept_dir, err)
+                log.warning(f"Failed creating [{intercept_dir}]: {err}")
                 return None
 
         signature = ""
         # different python versions are returning dict items in different order, so
         # simply iterating over them will not always produce the same result - hence we
         # build up a sorted list of keys first and use that one then:
         keylist = list(req_data.keys())
@@ -296,27 +307,27 @@
                 self.text = text
                 self.status_code = int(status_code)
 
         if self.cache_path == "":
             raise LookupError("No cache path configured")
 
         intercept_file = self.__interception_path(req_data, create_dir=False)
-        if not os.path.exists(intercept_file):  # pragma: no cover
+        if not intercept_file or not os.path.exists(intercept_file):  # pragma: no cover
             raise LookupError(f"No cache hit for [{intercept_file}]")
 
         with open(intercept_file, "r", encoding="utf-8") as infile:
             text = infile.read()
-        LOG.debug("Read intercepted response text from [%s]", intercept_file)
+        log.debug(f"Read intercepted response text from [{intercept_file}]")
 
         status_code = 200
         status_file = os.path.splitext(intercept_file)[0] + "_status-code.txt"
         if os.path.exists(status_file):
             with open(status_file, "r", encoding="utf-8") as infile:
                 status_code = infile.read()
-            LOG.debug("Read intercepted response status code from [%s]", status_file)
+            log.debug(f"Read intercepted response status code from [{status_file}]")
         return PseudoResponse(text, status_code)
 
     def __intercept_store(self, req_data, response):  # pragma: no cover
         """Store the response in a local cache file named after the request.
 
         Parameters
         ----------
@@ -330,29 +341,28 @@
         # triggered when testing in online mode with at least one request not being
         # served from the cache (which is orthogonal to off-line testing)
         if self.cache_path == "":
             return
 
         intercept_file = self.__interception_path(req_data, create_dir=True)
         if not intercept_file:
-            # FIXME: switch to loguru, turn into a trace-level message:
-            LOG.debug("Not storing intercepted results in cache.")
+            log.trace("Not storing intercepted results in cache.")
             return
 
         try:
             with open(intercept_file, "w", encoding="utf-8") as outfile:
                 outfile.write(response.text)
-            LOG.debug(
-                "Wrote response text to [%s] (%s lines)",
+            log.debug(
+                "Wrote response text to [{}] ({} lines)",
                 intercept_file,
                 len(response.text.splitlines()),
             )
         except Exception as err:  # pylint: disable-msg=broad-except
-            LOG.error("Storing response text in [%s] failed: %s", intercept_file, err)
-            LOG.error("Response text was:\n--------\n%s\n--------", response.text)
+            log.error("Storing response text in [{}] failed: {}", intercept_file, err)
+            log.error("Response text was:\n--------\n{}\n--------", response.text)
 
     def flush_cache(self, keep_users=False):
         """Flush the PyPPMS on-disk cache.
 
         Optionally flushes everything *except* the `getuser` cache if the
         `keep_users` flag is set to `True`, as this is clearly the most
         time-consuming operation when fetching data from PUMAPI and therefore
@@ -369,35 +379,35 @@
         Parameters
         ----------
         keep_users : bool, optional
             If set to `True` the `getuser` sub-directory in the cache location
             will be kept, by default `False`.
         """
         if self.cache_path == "":
-            LOG.info("No cache path configured, not flushing!")
+            log.info("No cache path configured, not flushing!")
             return
 
         dirs_to_remove = [self.cache_path]  # by default remove the entire cache dir
         keep_msg = ""
         if keep_users:
             keep_msg = " (keeping user details dirs)"
             dirs_to_remove = []
             cache_dirs = os.listdir(self.cache_path)
             for subdir in cache_dirs:
                 if subdir == "getuser":
                     continue
                 dirs_to_remove.append(os.path.join(self.cache_path, subdir))
 
-        LOG.info("Flushing the on-disk cache at [%s]%s...", self.cache_path, keep_msg)
+        log.info("Flushing the on-disk cache at [{}] {}...", self.cache_path, keep_msg)
         for directory in dirs_to_remove:
             try:
                 shutil.rmtree(directory)
-                LOG.debug("Removed directory [%s].", directory)
+                log.debug("Removed directory [{}].", directory)
             except Exception as ex:  # pylint: disable-msg=broad-except
-                LOG.warning("Removing the cache at [%s] failed: %s", directory, ex)
+                log.warning("Removing the cache at [{}] failed: {}", directory, ex)
 
     def get_admins(self):
         """Get all PPMS administrator users.
 
         Returns
         -------
         list(pyppms.user.PpmsUser)
@@ -406,15 +416,15 @@
         response = self.request("getadmins")
 
         admins = response.text.splitlines()
         users = []
         for username in admins:
             user = self.get_user(username)
             users.append(user)
-        LOG.debug("%s admins in the PPMS database: %s", len(admins), ", ".join(admins))
+        log.debug("{} admins in the PPMS database: {}", len(admins), ", ".join(admins))
         return users
 
     def get_booking(self, system_id, booking_type="get"):
         """Get the current or next booking of a system.
 
         WARNING: if the next booking is requested but it is too far in the future,
         PUMAPI silently ignores it - the response is identical to a system that has no
@@ -450,22 +460,22 @@
             raise ValueError(
                 f"Value for 'booking_type' ({booking_type}) not in {valid}!"
             )
 
         try:
             response = self.request(booking_type + "booking", {"id": system_id})
         except requests.exceptions.ConnectionError:
-            LOG.error("Requesting booking status for system %s failed!", system_id)
+            log.error("Requesting booking status for system {} failed!", system_id)
             return None
 
         desc = "any future bookings"
         if booking_type == "get":
             desc = "a currently active booking"
         if not response.text.strip():
-            LOG.debug("System [%s] doesn't have %s", system_id, desc)
+            log.debug("System [{}] doesn't have {}", system_id, desc)
             return None
 
         return PpmsBooking(response.text, booking_type, system_id)
 
     def get_current_booking(self, system_id):
         """Wrapper for `get_booking()` with 'booking_type' set to 'get'."""
         return self.get_booking(system_id, "get")
@@ -481,24 +491,24 @@
         Returns
         -------
         dict
             A dict with the group details, keys being derived from the header
             line of the PUMAPI response, values from the data line.
         """
         response = self.request("getgroup", {"unitlogin": group_id})
-        LOG.debug("Group details returned by PPMS (raw): %s", response.text)
+        log.debug("Group details returned by PPMS (raw): {}", response.text)
 
         if not response.text:
             msg = f"Group [{group_id}] is unknown to PPMS"
-            LOG.error(msg)
+            log.error(msg)
             raise KeyError(msg)
 
         details = dict_from_single_response(response.text)
 
-        LOG.debug("Details of group %s: %s", group_id, details)
+        log.debug("Details of group {}: {}", group_id, details)
         return details
 
     def get_group_users(self, unitlogin):
         """Get all members of a group in PPMS.
 
         Parameters
         ----------
@@ -513,16 +523,16 @@
         response = self.request("getgroupusers", {"unitlogin": unitlogin})
 
         members = response.text.splitlines()
         users = []
         for username in members:
             user = self.get_user(username)
             users.append(user)
-        LOG.debug(
-            "%s members in PPMS group [%s]: %s",
+        log.debug(
+            "{} members in PPMS group [{}]: {}",
             len(members),
             unitlogin,
             ", ".join(members),
         )
         return users
 
     def get_groups(self):
@@ -532,15 +542,15 @@
         -------
         list(str)
             A list with the group identifiers in PPMS.
         """
         response = self.request("getgroups")
 
         groups = response.text.splitlines()
-        LOG.debug("%s groups in the PPMS database: %s", len(groups), ", ".join(groups))
+        log.debug("{} groups in the PPMS database: {}", len(groups), ", ".join(groups))
         return groups
 
     def get_next_booking(self, system_id):
         """Wrapper for `get_booking()` with 'booking_type' set to 'next'."""
         return self.get_booking(system_id, "next")
 
     def get_running_sheet(self, core_facility_ref, date, ignore_uncached_users=False):
@@ -572,48 +582,48 @@
             there are no bookings or parsing the response failed.
         """
         bookings = []
         parameters = {
             "plateformid": f"{core_facility_ref}",
             "day": date.strftime("%Y-%m-%d"),
         }
-        LOG.debug("Requesting runningsheet for %s", parameters["day"])
+        log.debug("Requesting runningsheet for {}", parameters["day"])
         response = self.request("getrunningsheet", parameters)
         try:
             entries = parse_multiline_response(response.text, graceful=False)
         except Exception as err:  # pylint: disable-msg=broad-except
-            LOG.error("Parsing runningsheet details failed: %s", err)
+            log.error("Parsing runningsheet details failed: {}", err)
             # NOTE: in case no future bookings exist the response will be empty!
-            LOG.error("Possibly the runningsheet is empty as no bookings exist?")
-            LOG.debug("Runningsheet PUMPAI response was: %s", response.text)
+            log.error("Possibly the runningsheet is empty as no bookings exist?")
+            log.debug("Runningsheet PUMPAI response was: {}", response.text)
             return bookings
 
         for entry in entries:
             full = entry["User"]
             if full not in self.fullname_mapping:
                 if ignore_uncached_users:
-                    LOG.debug("Ignoring booking for uncached user [%s]", full)
+                    log.debug("Ignoring booking for uncached user [{}]", full)
                     continue
 
-                LOG.info("Booking for an uncached user (%s) found!", full)
+                log.info("Booking for an uncached user ({}) found!", full)
                 self.update_users()
 
             if full not in self.fullname_mapping:
-                LOG.error("PPMS doesn't seem to know user [%s], skipping", full)
+                log.error("PPMS doesn't seem to know user [{}], skipping", full)
                 continue
 
-            LOG.info(
-                "Booking for user '%s' (%s) found", self.fullname_mapping[full], full
+            log.info(
+                "Booking for user '{}' ({}) found", self.fullname_mapping[full], full
             )
             system_name = entry["Object"]
             system_ids = self.get_systems_matching("", [system_name])
             if len(system_ids) != 1:
                 # NOTE: more than one result should not happen as PPMS doesn't allow for
                 # multiple systems having the same name - no result might happen though!
-                LOG.error("Ignoring booking for unknown system [%s]", system_name)
+                log.error("Ignoring booking for unknown system [{}]", system_name)
                 continue
 
             booking = PpmsBooking.from_runningsheet(
                 entry,
                 system_ids[0],
                 self.fullname_mapping[full],
                 date,
@@ -636,15 +646,15 @@
         -------
         dict(pyppms.system.PpmsSystem)
             A dict with `PpmsSystem` objects parsed from the PUMAPI response where
             the system ID (int) is used as the dict's key. If parsing a system
             fails for any reason, the system is skipped entirely.
         """
         if self.systems and not force_refresh:
-            LOG.debug("Using cached details for %s systems", len(self.systems))
+            log.debug("Using cached details for {} systems", len(self.systems))
         else:
             self.update_systems()
 
         return self.systems
 
     def get_systems_matching(self, localisation, name_contains):
         """Query PPMS for systems with a specific location and name.
@@ -679,46 +689,46 @@
             raise TypeError("`name_contains` must be a list of str, not str!")
 
         loc = localisation
         loc_desc = f"with location matching [{localisation}]"
         if localisation == "":
             loc_desc = "(no location filter given)"
 
-        LOG.info(
-            "Querying PPMS for systems %s, name matching any of %s",
+        log.info(
+            "Querying PPMS for systems {}, name matching any of {}",
             loc_desc,
             name_contains,
         )
         system_ids = []
         systems = self.get_systems()
         for sys_id, system in systems.items():
             if loc.lower() not in str(system.localisation).lower():
-                LOG.debug(
-                    "System [%s] location (%s) is NOT matching (%s), ignoring",
+                log.debug(
+                    "System [{}] location ({}) is NOT matching ({}), ignoring",
                     system.name,
                     system.localisation,
                     loc,
                 )
                 continue
 
-            # LOG.debug('System [%s] is matching location [%s], checking if '
-            #           'the name is matching any of the valid pattern %s',
+            # log.debug('System [{}] is matching location [{}], checking if '
+            #           'the name is matching any of the valid pattern {}',
             #           system.name, loc, name_contains)
             for valid_name in name_contains:
                 if valid_name in system.name:
-                    LOG.debug("System [%s] matches all criteria", system.name)
+                    log.debug("System [{}] matches all criteria", system.name)
                     system_ids.append(sys_id)
                     break
 
             # if sys_id not in system_ids:
-            #     LOG.debug('System [%s] does NOT match a valid name: %s',
+            #     log.debug('System [{}] does NOT match a valid name: {}',
             #               system.name, name_contains)
 
-        LOG.info("Found %s bookable systems %s", len(system_ids), loc_desc)
-        LOG.debug("IDs of matching bookable systems %s: %s", loc_desc, system_ids)
+        log.info("Found {} bookable systems {}", len(system_ids), loc_desc)
+        log.debug("IDs of matching bookable systems {}: {}", loc_desc, system_ids)
         return system_ids
 
     def get_user(self, login_name, skip_cache=False):
         """Fetch user details from PPMS and create a PpmsUser object from it.
 
         Parameters
         ----------
@@ -739,15 +749,15 @@
         KeyError
             Raised if the user doesn't exist in PPMS.
         """
         response = self.request("getuser", {"login": login_name}, skip_cache=skip_cache)
 
         if not response.text:
             msg = f"User [{login_name}] is unknown to PPMS"
-            LOG.debug(msg)
+            log.debug(msg)
             raise KeyError(msg)
 
         user = PpmsUser(response.text)
         self.users[user.username] = user  # update / add to the cached user objs
         self.fullname_mapping[user.fullname] = user.username
         return user
 
@@ -790,28 +800,28 @@
         ValueError
             Raised if the user details can't be parsed from the PUMAPI response.
         """
         response = self.request("getuser", {"login": login_name}, skip_cache=skip_cache)
 
         if not response.text:
             msg = f"User [{login_name}] is unknown to PPMS"
-            LOG.error(msg)
+            log.error(msg)
             raise KeyError(msg)
 
         # EXAMPLE:
         # response.text = (
         #     u'login,lname,fname,email,'
         #     u'phone,bcode,affiliation,unitlogin,mustchpwd,mustchbcode,'
         #     u'active\r\n'
         #     u'"pyppms","Python","PumAPI","pyppms@python-facility.example",'
         #     u'"+98 (76) 54 3210","","","pyppms",false,false,'
         #     u'true\r\n'
         # )
         details = dict_from_single_response(response.text)
-        LOG.debug("Details for user [%s]: %s", login_name, details)
+        log.debug("Details for user [{}]: {}", login_name, details)
         return details
 
     def get_user_experience(self, login=None, system_id=None):
         """Get user experience ("User rights") from PPMS.
 
         Parameters
         ----------
@@ -831,16 +841,16 @@
         if login is not None:
             data["login"] = login
         if system_id is not None:
             data["id"] = system_id
         response = self.request("getuserexp", parameters=data)
 
         parsed = parse_multiline_response(response.text)
-        LOG.debug(
-            "Received %s experience entries for filters [user:%s] and [id:%s]",
+        log.debug(
+            "Received {} experience entries for filters [user:{}] and [id:{}]",
             len(parsed),
             login,
             system_id,
         )
         return parsed
 
     def get_user_ids(self, active=False):
@@ -863,16 +873,16 @@
         if active:
             parameters["active"] = "true"
 
         response = self.request("getusers", parameters)
 
         users = response.text.splitlines()
         active_desc = "active " if active else ""
-        LOG.info("%s %susers in the PPMS database", len(users), active_desc)
-        LOG.debug(", ".join(users))
+        log.info("{} {}users in the PPMS database", len(users), active_desc)
+        log.debug(", ".join(users))
         return users
 
     def get_users(self, force_refresh=False, active_only=True):
         """Get user objects for all (or cached) PPMS users.
 
         Parameters
         ----------
@@ -885,15 +895,15 @@
 
         Returns
         -------
         dict(pyppms.user.PpmsUser)
             A dict of PpmsUser objects with the username (login) as key.
         """
         if self.users and not force_refresh:
-            LOG.debug("Using cached details for %s users", len(self.users))
+            log.debug("Using cached details for {} users", len(self.users))
         else:
             self.update_users(active_only=active_only)
 
         return self.users
 
     def get_users_emails(self, users=None, active=False):
         """Get a list of user email addresses. WARNING - very slow!
@@ -914,17 +924,17 @@
         """
         emails = []
         if users is None:
             users = self.get_user_ids(active=active)
         for user in users:
             email = self.get_user_dict(user)["email"]
             if not email:
-                LOG.warning("--- WARNING: no email for user [%s]! ---", user)
+                log.warning("--- WARNING: no email for user [{}]! ---", user)
                 continue
-            # LOG.debug("%s: %s", user, email)
+            # log.debug("{}: {}", user, email)
             emails.append(email)
 
         return emails
 
     def get_users_with_access_to_system(self, system_id):
         """Get a list of usernames allowed to book the system with the given ID.
 
@@ -949,32 +959,32 @@
         response = self.request("getsysrights", {"id": system_id})
         # this response has a unique format, so parse it directly here:
         try:
             lines = response.text.splitlines()
             for line in lines:
                 permission, username = line.split(":")
                 if permission.upper() == "D":
-                    LOG.debug(
-                        "User [%s] is deactivated for booking system [%s], skipping",
+                    log.debug(
+                        "User [{}] is deactivated for booking system [{}], skipping",
                         username,
                         system_id,
                     )
                     continue
 
-                LOG.debug(
-                    "User [%s] has permission to book system [%s]", username, system_id
+                log.debug(
+                    "User [{}] has permission to book system [{}]", username, system_id
                 )
                 users.append(username)
 
         except Exception as err:
             msg = (
                 f"Unable to parse data returned by PUMAPI: {response.text} - "
                 f"ERROR: {err}"
             )
-            LOG.error(msg)
+            log.error(msg)
             raise ValueError(msg) from err
 
         return users
 
     def give_user_access_to_system(self, username, system_id):
         """Add permissions for a user to book a given system in PPMS.
 
@@ -1024,15 +1034,15 @@
 
         Raises
         ------
         RuntimeError
             Will be raised in case creating the user fails.
         """
         if self.user_exists(login):
-            LOG.warning("NOT creating user [%s] as it already exists!", login)
+            log.warning("NOT creating user [{}] as it already exists!", login)
             return
 
         req_data = {
             "login": login,
             "lname": lname,
             "fname": fname,
             "email": email,
@@ -1042,19 +1052,19 @@
             req_data["phone"] = phone
         if password:
             req_data["pwd"] = password
 
         response = self.request("newuser", req_data)
         if not "OK newuser" in response.text:
             msg = f"Creating new user failed: {response.text}"
-            LOG.error(msg)
+            log.error(msg)
             raise RuntimeError(msg)
 
-        LOG.info("Created user [%s] in PPMS.", login)
-        LOG.debug("Response was: %s", response.text)
+        log.info("Created user [{}] in PPMS.", login)
+        log.debug("Response was: {}", response.text)
 
     def remove_user_access_from_system(self, username, system_id):
         """Remove permissions for a user to book a given system in PPMS.
 
         Parameters
         ----------
         username : str
@@ -1120,72 +1130,72 @@
                 "S": "superuser",
             }
             try:
                 return mapping[shortname]
             except KeyError as err:
                 raise KeyError(f"Invalid permission [{shortname}] given") from err
 
-        LOG.debug(
-            "Setting permission level [%s] for user [%s] on system [%s]",
+        log.debug(
+            "Setting permission level [{}] for user [{}] on system [{}]",
             permission_name(permission),
             login,
             system_id,
         )
 
         parameters = {"id": system_id, "login": login, "type": permission}
         response = self.request("setright", parameters)
 
         # NOTE: the 'setright' action will accept ANY permission type and return 'done'
         # on the request, so there is no way to check from the response if setting the
         # permission really worked!!
-        # LOG.debug('Request returned text: %s', response.text)
+        # log.debug('Request returned text: {}', response.text)
         if response.text.lower().strip() == "done":
-            LOG.debug(
-                "User [%s] now has permission level [%s] on system [%s]",
+            log.debug(
+                "User [{}] now has permission level [{}] on system [{}]",
                 login,
                 permission_name(permission),
                 system_id,
             )
             return True
 
         if "invalid user" in response.text.lower():
-            LOG.warning("User [%s] doesn't seem to exist in PPMS", login)
+            log.warning("User [{}] doesn't seem to exist in PPMS", login)
         elif "system right not authorized" in response.text.lower():
-            LOG.error(
-                "Unable to set permissions for system %s: %s", system_id, response.text
+            log.error(
+                "Unable to set permissions for system {}: {}", system_id, response.text
             )
         else:
-            LOG.error("Unexpected response, assuming request failed: %s", response.text)
+            log.error("Unexpected response, assuming request failed: {}", response.text)
 
         return False
 
     def update_systems(self):
         """Update cached details for all bookable systems from PPMS.
 
         Get the details on all bookable systems from PPMS and store them in the local
         cache. If parsing the PUMAPI response for a system fails for any reason, the
         system is skipped entirely.
         """
-        LOG.debug("Updating list of bookable systems...")
+        log.debug("Updating list of bookable systems...")
         systems = {}
         parse_fails = 0
         response = self.request("getsystems")
         details = parse_multiline_response(response.text, graceful=False)
         for detail in details:
             try:
                 system = PpmsSystem(detail)
             except ValueError as err:
-                LOG.error("Error processing `getsystems` response: %s", err)
+                log.error("Error processing `getsystems` response: {}", err)
                 parse_fails += 1
                 continue
 
             systems[system.system_id] = system
 
-        LOG.debug(
-            "Updated %s bookable systems from PPMS (%s systems failed parsing)",
+        log.debug(
+            "Updated {} bookable systems from PPMS ({} systems failed parsing)",
             len(systems),
             parse_fails,
         )
 
         self.systems = systems
 
     def update_users(self, user_ids=[], active_only=True):
@@ -1205,19 +1215,19 @@
         active_only : bool, optional
             If set to `False` also "inactive" users will be fetched from PPMS,
             by default `True`.
         """
         if not user_ids:
             user_ids = self.get_user_ids(active=active_only)
 
-        LOG.debug("Updating details on %s users", len(user_ids))
+        log.debug("Updating details on {} users", len(user_ids))
         for user_id in user_ids:
             self.get_user(user_id, skip_cache=True)
 
-        LOG.debug("Collected details on %s users", len(self.users))
+        log.debug("Collected details on {} users", len(self.users))
 
     def user_exists(self, login):
         """Check if an account with the given login name already exists in PPMS.
 
         Parameters
         ----------
         login : str
```

### Comparing `pyppms-2.3.0a0/src/pyppms/system.py` & `pyppms-3.0.0/src/pyppms/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Module representing bookable systems in PPMS."""
 
 # pylint: disable-msg=too-many-instance-attributes
 # pylint: disable-msg=too-many-arguments
 
-import logging
-
-LOG = logging.getLogger(__name__)
+from loguru import logger as log
 
 
 class PpmsSystem:
 
     """Object representing a bookable system in PPMS.
 
     Attributes
@@ -52,37 +50,37 @@
         ----------
         details : dict
             A dict with the parsed response from a `getsystems` request.
         """
         try:
             self.system_id = int(details["System id"])
         except ValueError as err:
-            LOG.error("Unable to parse system ID: %s - %s", details["System id"], err)
+            log.error("Unable to parse system ID: {} - {}", details["System id"], err)
             raise
 
         self.name = details["Name"]
         self.localisation = details["Localisation"]
         self.system_type = details["Type"]
         self.core_facility_ref = details["Core facility ref"]
         self.schedules = details["Schedules"]
         self.active = details["Active"]
         self.stats = details["Stats"]
         self.bookable = details["Bookable"]
         self.autonomy_required = details["Autonomy Required"]
         self.autonomy_required_after_hours = details["Autonomy Required After Hours"]
-        LOG.debug(
-            "PpmsSystem(system_id=%s, name=[%s], localisation=[%s], system_type=[%s])",
+        log.trace(
+            "PpmsSystem(system_id={}, name=[{}], localisation=[{}], system_type=[{}])",
             self.system_id,
             self.name,
             self.localisation,
             self.system_type,
         )
-        # LOG.debug('PpmsSystem details: core_facility_ref=%s, schedules=%s, '
-        #           'active=%s, stats=%s, bookable=%s, autonomy_required=%s, '
-        #           'autonomy_required_after_hours=%s', core_facility_ref,
+        # log.debug('PpmsSystem details: core_facility_ref={}, schedules={}, '
+        #           'active={}, stats={}, bookable={}, autonomy_required={}, '
+        #           'autonomy_required_after_hours={}', core_facility_ref,
         #           schedules, active, stats, bookable, autonomy_required,
         #           autonomy_required_after_hours)
 
     def __str__(self):
         return (
             f"system_id: {self.system_id}, "
             f"name: {self.name}, "
```

### Comparing `pyppms-2.3.0a0/src/pyppms/user.py` & `pyppms-3.0.0/src/pyppms/user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Module representing user objects in PPMS."""
 
-import logging
+from loguru import logger as log
 
 from .common import dict_from_single_response
 
-LOG = logging.getLogger(__name__)
-
 
 class PpmsUser:
 
     """Object representing a user in PPMS.
 
     Attributes
     ----------
@@ -38,17 +36,17 @@
 
         self.username = str(details["login"])
         self.email = str(details["email"])
         self.active = details["active"]
         self.ppms_group = details["unitlogin"]
         self._fullname = f'{details["lname"]} {details["fname"]}'
 
-        LOG.debug(
-            "PpmsUser initialized: username=[%s], email=[%s], ppms_group=[%s], "
-            "fullname=[%s], active=[%s]",
+        log.trace(
+            "PpmsUser initialized: username=[{}], email=[{}], ppms_group=[{}], "
+            "fullname=[{}], active=[{}]",
             self.username,
             self.email,
             self.ppms_group,
             self._fullname,
             self.active,
         )
```

### Comparing `pyppms-2.3.0a0/PKG-INFO` & `pyppms-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyppms
-Version: 2.3.0a0
+Version: 3.0.0
 Summary: A Python package to communicate with Stratocore's PUMAPI.
 Home-page: https://pypi.org/project/pyppms/
 License: GPLv3
 Keywords: ppms,pumapi,booking-system,reservation-system
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (>=2.25.1,<3.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://imcf.one/apidocs/pyppms/pyppms.html
 Project-URL: Repository, https://github.com/imcf/pyppms
 Description-Content-Type: text/markdown
 
 # PyPPMS
 
 ## PUMAPI - Python Interface
```

