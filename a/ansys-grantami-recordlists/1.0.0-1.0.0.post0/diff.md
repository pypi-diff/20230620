# Comparing `tmp/ansys_grantami_recordlists-1.0.0.tar.gz` & `tmp/ansys_grantami_recordlists-1.0.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_grantami_recordlists-1.0.0.tar", max compression
+gzip compressed data, was "ansys_grantami_recordlists-1.0.0.post0.tar", max compression
```

## Comparing `ansys_grantami_recordlists-1.0.0.tar` & `ansys_grantami_recordlists-1.0.0.post0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1089 2023-06-19 09:12:29.436558 ansys_grantami_recordlists-1.0.0/LICENSE
--rw-r--r--   0        0        0     3400 2023-06-19 09:12:29.436558 ansys_grantami_recordlists-1.0.0/README.rst
--rw-r--r--   0        0        0     2313 2023-06-19 09:12:29.440559 ansys_grantami_recordlists-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      591 2023-06-19 09:12:29.440559 ansys_grantami_recordlists-1.0.0/src/ansys/grantami/recordlists/__init__.py
--rw-r--r--   0        0        0    25391 2023-06-19 09:12:29.440559 ansys_grantami_recordlists-1.0.0/src/ansys/grantami/recordlists/_connection.py
--rw-r--r--   0        0        0      114 2023-06-19 09:12:29.440559 ansys_grantami_recordlists-1.0.0/src/ansys/grantami/recordlists/_logger.py
--rw-r--r--   0        0        0    26419 2023-06-19 09:12:29.440559 ansys_grantami_recordlists-1.0.0/src/ansys/grantami/recordlists/_models.py
--rw-r--r--   0        0        0        0 2023-06-19 09:12:29.440559 ansys_grantami_recordlists-1.0.0/src/ansys/grantami/recordlists/py.typed
--rw-r--r--   0        0        0     4487 1970-01-01 00:00:00.000000 ansys_grantami_recordlists-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-19 15:03:55.496597 ansys_grantami_recordlists-1.0.0.post0/LICENSE
+-rw-r--r--   0        0        0     3424 2023-06-19 15:03:55.496597 ansys_grantami_recordlists-1.0.0.post0/README.rst
+-rw-r--r--   0        0        0     2319 2023-06-19 15:03:55.500598 ansys_grantami_recordlists-1.0.0.post0/pyproject.toml
+-rw-r--r--   0        0        0      591 2023-06-19 15:03:55.500598 ansys_grantami_recordlists-1.0.0.post0/src/ansys/grantami/recordlists/__init__.py
+-rw-r--r--   0        0        0    25391 2023-06-19 15:03:55.500598 ansys_grantami_recordlists-1.0.0.post0/src/ansys/grantami/recordlists/_connection.py
+-rw-r--r--   0        0        0      114 2023-06-19 15:03:55.500598 ansys_grantami_recordlists-1.0.0.post0/src/ansys/grantami/recordlists/_logger.py
+-rw-r--r--   0        0        0    26419 2023-06-19 15:03:55.500598 ansys_grantami_recordlists-1.0.0.post0/src/ansys/grantami/recordlists/_models.py
+-rw-r--r--   0        0        0        0 2023-06-19 15:03:55.500598 ansys_grantami_recordlists-1.0.0.post0/src/ansys/grantami/recordlists/py.typed
+-rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ansys_grantami_recordlists-1.0.0.post0/PKG-INFO
```

### Comparing `ansys_grantami_recordlists-1.0.0/LICENSE` & `ansys_grantami_recordlists-1.0.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.0.0/README.rst` & `ansys_grantami_recordlists-1.0.0.post0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?labelColor=black&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
-.. |python| image:: https://img.shields.io/pypi/pyversions/grantami-recordlists?logo=pypi
-   :target: https://pypi.org/project/grantami-recordlists/
+.. |python| image:: https://img.shields.io/pypi/pyversions/ansys-grantami-recordlists?logo=pypi
+   :target: https://pypi.org/project/ansys-grantami-recordlists/
    :alt: Python
 
-.. |pypi| image:: https://img.shields.io/pypi/v/grantami-recordlists.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/grantami-recordlists
+.. |pypi| image:: https://img.shields.io/pypi/v/ansys-grantami-recordlists.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/ansys-grantami-recordlists
    :alt: PyPI
 
 .. |codecov| image:: https://codecov.io/gh/pyansys/grantami-recordlists/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/pyansys/grantami-recordlists
    :alt: Codecov
 
 .. |GH-CI| image:: https://github.com/pyansys/grantami-recordlists/actions/workflows/ci_cd.yml/badge.svg
```

### Comparing `ansys_grantami_recordlists-1.0.0/pyproject.toml` & `ansys_grantami_recordlists-1.0.0.post0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-grantami-recordlists"
-version = "1.0.0"
+version = "1.0.0.post0"
 description = "A python wrapper for the Granta MI RecordLists API"
 license = "MIT"
 authors = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 maintainers = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/ansys/grantami-recordlists"
 documentation = "https://recordlists.grantami.docs.pyansys.com"
```

### Comparing `ansys_grantami_recordlists-1.0.0/src/ansys/grantami/recordlists/__init__.py` & `ansys_grantami_recordlists-1.0.0.post0/src/ansys/grantami/recordlists/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.0.0/src/ansys/grantami/recordlists/_connection.py` & `ansys_grantami_recordlists-1.0.0.post0/src/ansys/grantami/recordlists/_connection.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.0.0/src/ansys/grantami/recordlists/_models.py` & `ansys_grantami_recordlists-1.0.0.post0/src/ansys/grantami/recordlists/_models.py`

 * *Files identical despite different names*

### Comparing `ansys_grantami_recordlists-1.0.0/PKG-INFO` & `ansys_grantami_recordlists-1.0.0.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-grantami-recordlists
-Version: 1.0.0
+Version: 1.0.0.post0
 Summary: A python wrapper for the Granta MI RecordLists API
 Home-page: https://github.com/ansys/grantami-recordlists
 License: MIT
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
@@ -26,20 +26,20 @@
 
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
 .. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?labelColor=black&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
    :target: https://docs.pyansys.com/
    :alt: PyAnsys
 
-.. |python| image:: https://img.shields.io/pypi/pyversions/grantami-recordlists?logo=pypi
-   :target: https://pypi.org/project/grantami-recordlists/
+.. |python| image:: https://img.shields.io/pypi/pyversions/ansys-grantami-recordlists?logo=pypi
+   :target: https://pypi.org/project/ansys-grantami-recordlists/
    :alt: Python
 
-.. |pypi| image:: https://img.shields.io/pypi/v/grantami-recordlists.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/grantami-recordlists
+.. |pypi| image:: https://img.shields.io/pypi/v/ansys-grantami-recordlists.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/ansys-grantami-recordlists
    :alt: PyPI
 
 .. |codecov| image:: https://codecov.io/gh/pyansys/grantami-recordlists/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/pyansys/grantami-recordlists
    :alt: Codecov
 
 .. |GH-CI| image:: https://github.com/pyansys/grantami-recordlists/actions/workflows/ci_cd.yml/badge.svg
```

