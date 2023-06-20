# Comparing `tmp/locatieserver-0.5.0.tar.gz` & `tmp/locatieserver-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locatieserver-0.5.0.tar", max compression
+gzip compressed data, was "locatieserver-0.5.2.tar", max compression
```

## Comparing `locatieserver-0.5.0.tar` & `locatieserver-0.5.2.tar`

### file list

```diff
@@ -1,34 +1,30 @@
--rw-r--r--   0        0        0     1073 2022-11-08 10:13:30.060681 locatieserver-0.5.0/LICENSE
--rw-r--r--   0        0        0     2545 2022-11-08 10:13:30.060681 locatieserver-0.5.0/README.rst
--rw-r--r--   0        0        0      127 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/__init__.py
--rw-r--r--   0        0        0      203 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/__init__.py
--rw-r--r--   0        0        0       71 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/config.py
--rw-r--r--   0        0        0     4100 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/free.py
--rw-r--r--   0        0        0     3200 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/lookup.py
--rw-r--r--   0        0        0     4809 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/suggest.py
--rw-r--r--   0        0        0       16 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/tests/__init__.py
--rw-r--r--   0        0        0    12471 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/tests/test_free.json
--rw-r--r--   0        0        0      244 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/tests/test_free.py
--rw-r--r--   0        0        0     1386 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/tests/test_lookup.json
--rw-r--r--   0        0        0      248 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/tests/test_lookup.py
--rw-r--r--   0        0        0     3550 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/tests/test_suggest.json
--rw-r--r--   0        0        0      260 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/tests/test_suggest.py
--rw-r--r--   0        0        0     1935 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/client/utils.py
--rw-r--r--   0        0        0        0 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/py.typed
--rw-r--r--   0        0        0        0 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/__init__.py
--rw-r--r--   0        0        0      166 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/base.py
--rw-r--r--   0        0        0      328 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/error.json
--rw-r--r--   0        0        0      378 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/error.py
--rw-r--r--   0        0        0     1369 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/free.json
--rw-r--r--   0        0        0     1151 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/free.py
--rw-r--r--   0        0        0     1292 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/lookup.json
--rw-r--r--   0        0        0     1426 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/lookup.py
--rw-r--r--   0        0        0      693 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/openapi.py
--rw-r--r--   0        0        0     4684 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/suggest.json
--rw-r--r--   0        0        0     1383 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/suggest.py
--rw-r--r--   0        0        0        0 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/tests/__init__.py
--rw-r--r--   0        0        0      861 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/tests/test_utils.py
--rw-r--r--   0        0        0      613 2022-11-08 10:13:30.060681 locatieserver-0.5.0/locatieserver/schema/utils.py
--rw-r--r--   0        0        0     2213 2022-11-08 10:13:30.064681 locatieserver-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3536 1970-01-01 00:00:00.000000 locatieserver-0.5.0/setup.py
--rw-r--r--   0        0        0     3597 1970-01-01 00:00:00.000000 locatieserver-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-20 09:51:09.809853 locatieserver-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2545 2023-06-20 09:51:09.809853 locatieserver-0.5.2/README.rst
+-rw-r--r--   0        0        0      127 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/__init__.py
+-rw-r--r--   0        0        0      203 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/client/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/client/config.py
+-rw-r--r--   0        0        0     4100 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/client/free.py
+-rw-r--r--   0        0        0     3200 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/client/lookup.py
+-rw-r--r--   0        0        0     4809 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/client/suggest.py
+-rw-r--r--   0        0        0       16 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/client/tests/__init__.py
+-rw-r--r--   0        0        0      179 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/client/tests/test_free.py
+-rw-r--r--   0        0        0      173 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/client/tests/test_lookup.py
+-rw-r--r--   0        0        0      185 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/client/tests/test_suggest.py
+-rw-r--r--   0        0        0     1498 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/client/utils.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/py.typed
+-rw-r--r--   0        0        0        0 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/__init__.py
+-rw-r--r--   0        0        0      166 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/base.py
+-rw-r--r--   0        0        0      328 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/error.json
+-rw-r--r--   0        0        0      378 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/error.py
+-rw-r--r--   0        0        0     1369 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/free.json
+-rw-r--r--   0        0        0     1151 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/free.py
+-rw-r--r--   0        0        0     1292 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/lookup.json
+-rw-r--r--   0        0        0     1426 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/lookup.py
+-rw-r--r--   0        0        0      693 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/openapi.py
+-rw-r--r--   0        0        0     4684 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/suggest.json
+-rw-r--r--   0        0        0     1383 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/suggest.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/tests/__init__.py
+-rw-r--r--   0        0        0      861 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/tests/test_utils.py
+-rw-r--r--   0        0        0      613 2023-06-20 09:51:09.809853 locatieserver-0.5.2/locatieserver/schema/utils.py
+-rw-r--r--   0        0        0     2125 2023-06-20 09:51:09.813853 locatieserver-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 locatieserver-0.5.2/PKG-INFO
```

### Comparing `locatieserver-0.5.0/LICENSE` & `locatieserver-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/README.rst` & `locatieserver-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/locatieserver/client/free.py` & `locatieserver-0.5.2/locatieserver/client/free.py`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/locatieserver/client/lookup.py` & `locatieserver-0.5.2/locatieserver/client/lookup.py`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/locatieserver/client/suggest.py` & `locatieserver-0.5.2/locatieserver/client/suggest.py`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/locatieserver/client/tests/test_lookup.json` & `locatieserver-0.5.2/locatieserver/schema/lookup.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7433894230769231%*

 * *Differences: {"'response'": "{'docs': {0: {'centroide_ll': 'POINT(5.10696041 52.06415055)', "*

 * *               "'gekoppeld_perceel': {delete: [1]}, delete: ['huisnummertoevoeging', "*

 * *               "'huisletter']}}, 'numFound': 1, delete: ['num_found']}"}*

```diff
@@ -1,25 +1,22 @@
 {
     "response": {
         "docs": [
             {
                 "adresseerbaarobject_id": "0344010000006589",
                 "bron": "BAG",
-                "centroide_ll": "POINT(5.10696048 52.06415055)",
+                "centroide_ll": "POINT(5.10696041 52.06415055)",
                 "centroide_rd": "POINT(135782.745 452910.011)",
                 "gekoppeld_perceel": [
-                    "UTT00-R-364",
-                    "UTT00-R-365"
+                    "UTT00-R-364"
                 ],
                 "gemeentecode": "0344",
                 "gemeentenaam": "Utrecht",
                 "huis_nlt": "93",
-                "huisletter": "",
                 "huisnummer": 93,
-                "huisnummertoevoeging": "",
                 "id": "adr-bf54db721969487ed33ba84d9973c702",
                 "identificatie": "0344010000006589-0344200000128086",
                 "nummeraanduiding_id": "0344200000128086",
                 "openbareruimte_id": "0344300000000177",
                 "openbareruimtetype": "Weg",
                 "postcode": "3526KP",
                 "provincieafkorting": "UT",
@@ -29,11 +26,11 @@
                 "straatnaam_verkort": "Europaln",
                 "type": "adres",
                 "weergavenaam": "Europalaan 93, 3526KP Utrecht",
                 "woonplaatscode": "3295",
                 "woonplaatsnaam": "Utrecht"
             }
         ],
-        "num_found": 1,
+        "numFound": 1,
         "start": 0
     }
 }
```

### Comparing `locatieserver-0.5.0/locatieserver/client/utils.py` & `locatieserver-0.5.2/locatieserver/client/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import inspect
-from functools import wraps
-from pathlib import Path
 from typing import Any, Callable, Dict
 
 import httpx
-from pydantic import BaseModel
 
 from locatieserver.client.config import BASE_URL
 from locatieserver.schema.error import ErrorResponse
 
 DEFAULT_CACHE = {}
 
 
@@ -55,23 +52,7 @@
         return response
     elif response.status_code == 400:
         error_response = ErrorResponse.parse_raw(response.content)
 
         raise LocatieserverResponseError(error_response.error.msg)
 
     return response
-
-
-def write_response(name: str, result: BaseModel):
-
-    output = Path(__file__).parent / "tests" / f"{name}.json"
-    output.write_text(result.json(indent=2))
-
-
-def safe_result(f):
-    @wraps(f)
-    def wrapper(*args, **kwds):
-        response = f(*args, **kwds)
-        write_response(f.__name__, response)
-        return response
-
-    return wrapper
```

### Comparing `locatieserver-0.5.0/locatieserver/schema/free.json` & `locatieserver-0.5.2/locatieserver/schema/free.json`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/locatieserver/schema/free.py` & `locatieserver-0.5.2/locatieserver/schema/free.py`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/locatieserver/schema/lookup.py` & `locatieserver-0.5.2/locatieserver/schema/lookup.py`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/locatieserver/schema/openapi.py` & `locatieserver-0.5.2/locatieserver/schema/openapi.py`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/locatieserver/schema/suggest.json` & `locatieserver-0.5.2/locatieserver/schema/suggest.json`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/locatieserver/schema/suggest.py` & `locatieserver-0.5.2/locatieserver/schema/suggest.py`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/locatieserver/schema/tests/test_utils.py` & `locatieserver-0.5.2/locatieserver/schema/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/locatieserver/schema/utils.py` & `locatieserver-0.5.2/locatieserver/schema/utils.py`

 * *Files identical despite different names*

### Comparing `locatieserver-0.5.0/pyproject.toml` & `locatieserver-0.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "locatieserver"
-version = "0.5.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.5.2"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Locatieserver api client"
 authors = ["Jelmer Draaijer <info@jelmert.nl>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/foarsitter/locatieserver"
 repository = "https://github.com/foarsitter/locatieserver"
 documentation = "https://locatieserver.readthedocs.io"
@@ -23,43 +23,41 @@
 [tool.poetry.dependencies]
 python = "^3.7.1"
 pydantic = "^1.8.2"
 httpx = "^0.23.0"
 
 
 [tool.poetry.dev-dependencies]
-respx = "^0.20.0"
-pytest = "^7.0.1"
-coverage = {extras = ["toml"], version = "^6.2"}
-safety = "^2.2.0"
-mypy = "^0.982"
+respx = "^0.20.1"
+pytest = "^7.2.1"
+coverage = {extras = ["toml"], version = "^7.1"}
+safety = "^2.3.3"
+mypy = "^0.991"
 typeguard = "^2.13.3"
-xdoctest = {extras = ["colors"], version = "^1.0.0"}
+xdoctest = {extras = ["colors"], version = "^1.1.1"}
 sphinx = "^5.1.1"
 sphinx-autobuild = "^2021.3.14"
 pre-commit = "^2.11.1"
 flake8 = "^3.8.4"
 black = "^22.3.0"
 flake8-bandit = "^3.0.0"
-flake8-bugbear = "^22.4.25"
+flake8-bugbear = "^23.1.20"
 flake8-docstrings = "^1.5.0"
-flake8-rst-docstrings = "^0.2.5"
+flake8-rst-docstrings = "^0.3.0"
 pep8-naming = "^0.13.2"
-darglint = "^1.8.1"
 reorder-python-imports = "^3.9.0"
-pre-commit-hooks = "^4.0.1"
+pre-commit-hooks = "^4.4.0"
 sphinx-rtd-theme = "^0.5.0"
 sphinx-click = "^3.1.0"
 Pygments = "^2.12.0"
 types-pkg-resources = "^0.1.2"
-types-requests = "^2.27.25"
+types-requests = "^2.28.11"
 types-attrs = "^19.1.0"
 sphinx-rtd-dark-mode = "^1.2.4"
 Jinja2 = "^3.0.0"
-datamodel-code-generator = {extras = ["http"], version = "^0.13.5"}
 
 [tool.poetry.scripts]
 locatieserver = "locatieserver.__main__:main"
 
 [tool.black]
 line-length = 120
```

### Comparing `locatieserver-0.5.0/PKG-INFO` & `locatieserver-0.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: locatieserver
-Version: 0.5.0
+Version: 0.5.2
 Summary: Locatieserver api client
 Home-page: https://github.com/foarsitter/locatieserver
 License: MIT
 Author: Jelmer Draaijer
 Author-email: info@jelmert.nl
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Project-URL: Documentation, https://locatieserver.readthedocs.io
 Project-URL: Repository, https://github.com/foarsitter/locatieserver
 Description-Content-Type: text/x-rst
 
 locatieserver
```

