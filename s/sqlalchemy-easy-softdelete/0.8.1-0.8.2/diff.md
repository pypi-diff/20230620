# Comparing `tmp/sqlalchemy_easy_softdelete-0.8.1.tar.gz` & `tmp/sqlalchemy_easy_softdelete-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_easy_softdelete-0.8.1.tar", max compression
+gzip compressed data, was "sqlalchemy_easy_softdelete-0.8.2.tar", max compression
```

## Comparing `sqlalchemy_easy_softdelete-0.8.1.tar` & `sqlalchemy_easy_softdelete-0.8.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1497 2023-06-19 23:15:20.997063 sqlalchemy_easy_softdelete-0.8.1/LICENSE
--rw-r--r--   0        0        0     2977 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/README.md
--rw-r--r--   0        0        0     1620 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      140 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/sqlalchemy_easy_softdelete/__init__.py
--rw-r--r--   0        0        0       65 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/sqlalchemy_easy_softdelete/handler/__init__.py
--rw-r--r--   0        0        0     6089 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py
--rw-r--r--   0        0        0      850 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py
--rw-r--r--   0        0        0     1623 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/sqlalchemy_easy_softdelete/mixin.py
--rw-r--r--   0        0        0       56 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0     1971 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/tests/conftest.py
--rw-r--r--   0        0        0     2580 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/tests/model.py
--rw-r--r--   0        0        0      360 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/tests/seed_data/__init__.py
--rw-r--r--   0        0        0     2025 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/tests/seed_data/parent_child_childchild.py
--rw-r--r--   0        0        0        0 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/tests/snapshots/__init__.py
--rw-r--r--   0        0        0     4006 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/tests/snapshots/snap_test_queries.py
--rw-r--r--   0        0        0     9931 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/tests/snapshots/snap_test_seed_data.py
--rw-r--r--   0        0        0     7591 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/tests/test_queries.py
--rw-r--r--   0        0        0      595 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/tests/test_seed_data.py
--rw-r--r--   0        0        0     1992 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     2288 2023-06-19 23:15:21.001063 sqlalchemy_easy_softdelete-0.8.1/tests/utils/simple_select_extractor.py
--rw-r--r--   0        0        0     3746 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-06-19 23:27:22.062430 sqlalchemy_easy_softdelete-0.8.2/LICENSE
+-rw-r--r--   0        0        0     2984 2023-06-19 23:27:22.062430 sqlalchemy_easy_softdelete-0.8.2/README.md
+-rw-r--r--   0        0        0     1620 2023-06-19 23:27:22.062430 sqlalchemy_easy_softdelete-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-06-19 23:27:22.062430 sqlalchemy_easy_softdelete-0.8.2/sqlalchemy_easy_softdelete/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/sqlalchemy_easy_softdelete/handler/__init__.py
+-rw-r--r--   0        0        0     6089 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py
+-rw-r--r--   0        0        0      850 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py
+-rw-r--r--   0        0        0     1623 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/sqlalchemy_easy_softdelete/mixin.py
+-rw-r--r--   0        0        0       56 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/tests/__init__.py
+-rw-r--r--   0        0        0     1971 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/tests/conftest.py
+-rw-r--r--   0        0        0     2580 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/tests/model.py
+-rw-r--r--   0        0        0      360 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/tests/seed_data/__init__.py
+-rw-r--r--   0        0        0     2025 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/tests/seed_data/parent_child_childchild.py
+-rw-r--r--   0        0        0        0 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0     4006 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/tests/snapshots/snap_test_queries.py
+-rw-r--r--   0        0        0     9931 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/tests/snapshots/snap_test_seed_data.py
+-rw-r--r--   0        0        0     7591 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/tests/test_queries.py
+-rw-r--r--   0        0        0      595 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/tests/test_seed_data.py
+-rw-r--r--   0        0        0     1992 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2288 2023-06-19 23:27:22.066430 sqlalchemy_easy_softdelete-0.8.2/tests/utils/simple_select_extractor.py
+-rw-r--r--   0        0        0     3753 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.8.2/PKG-INFO
```

### Comparing `sqlalchemy_easy_softdelete-0.8.1/LICENSE` & `sqlalchemy_easy_softdelete-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/README.md` & `sqlalchemy_easy_softdelete-0.8.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SQLAlchemy Easy Soft-Delete
 
 [![pypi](https://img.shields.io/pypi/v/sqlalchemy-easy-softdelete.svg)](https://pypi.org/project/sqlalchemy-easy-softdelete/)
 [![python](https://img.shields.io/pypi/pyversions/sqlalchemy-easy-softdelete.svg)](https://pypi.org/project/sqlalchemy-easy-softdelete/)
-[![Build Status](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml/badge.svg)](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml)
+[![Build Status](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test_matrix.yml/badge.svg)](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml)
 ![Supported SQLAlchemy Versions](https://img.shields.io/badge/SQLAlchemy-1.4%20%2F%202.0-brightgreen)
 
 [//]: # ([![codecov]&#40;https://codecov.io/gh/flipbit03/sqlalchemy-easy-softdelete/branch/main/graphs/badge.svg&#41;]&#40;https://codecov.io/github/flipbit03/sqlalchemy-easy-softdelete&#41;)
 
 Easily add soft-deletion to your SQLAlchemy Models and automatically filter out soft-deleted objects from your queries and relationships.
 
 This package can generate a tailor-made SQLAlchemy Mixin that can be added to your SQLAlchemy Models, making them contain a field that, when set, will mark the entity as being soft-deleted.
```

### Comparing `sqlalchemy_easy_softdelete-0.8.1/pyproject.toml` & `sqlalchemy_easy_softdelete-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "sqlalchemy-easy-softdelete"
-version = "0.8.1"
+version = "0.8.2"
 homepage = "https://github.com/flipbit03/sqlalchemy-easy-softdelete"
 description = "Easily add soft-deletion to your SQLAlchemy Models."
 authors = ["Cadu <cadu.coelho@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
```

### Comparing `sqlalchemy_easy_softdelete-0.8.1/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py` & `sqlalchemy_easy_softdelete-0.8.2/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py` & `sqlalchemy_easy_softdelete-0.8.2/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/sqlalchemy_easy_softdelete/mixin.py` & `sqlalchemy_easy_softdelete-0.8.2/sqlalchemy_easy_softdelete/mixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/tests/conftest.py` & `sqlalchemy_easy_softdelete-0.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/tests/model.py` & `sqlalchemy_easy_softdelete-0.8.2/tests/model.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/tests/seed_data/parent_child_childchild.py` & `sqlalchemy_easy_softdelete-0.8.2/tests/seed_data/parent_child_childchild.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/tests/snapshots/snap_test_queries.py` & `sqlalchemy_easy_softdelete-0.8.2/tests/snapshots/snap_test_queries.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/tests/snapshots/snap_test_seed_data.py` & `sqlalchemy_easy_softdelete-0.8.2/tests/snapshots/snap_test_seed_data.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/tests/test_queries.py` & `sqlalchemy_easy_softdelete-0.8.2/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/tests/test_seed_data.py` & `sqlalchemy_easy_softdelete-0.8.2/tests/test_seed_data.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/tests/utils/__init__.py` & `sqlalchemy_easy_softdelete-0.8.2/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/tests/utils/simple_select_extractor.py` & `sqlalchemy_easy_softdelete-0.8.2/tests/utils/simple_select_extractor.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.8.1/PKG-INFO` & `sqlalchemy_easy_softdelete-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-easy-softdelete
-Version: 0.8.1
+Version: 0.8.2
 Summary: Easily add soft-deletion to your SQLAlchemy Models.
 Home-page: https://github.com/flipbit03/sqlalchemy-easy-softdelete
 License: BSD-3-Clause
 Author: Cadu
 Author-email: cadu.coelho@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,15 @@
 Requires-Dist: SQLAlchemy (>=1.4,<2.1)
 Description-Content-Type: text/markdown
 
 # SQLAlchemy Easy Soft-Delete
 
 [![pypi](https://img.shields.io/pypi/v/sqlalchemy-easy-softdelete.svg)](https://pypi.org/project/sqlalchemy-easy-softdelete/)
 [![python](https://img.shields.io/pypi/pyversions/sqlalchemy-easy-softdelete.svg)](https://pypi.org/project/sqlalchemy-easy-softdelete/)
-[![Build Status](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml/badge.svg)](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml)
+[![Build Status](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test_matrix.yml/badge.svg)](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml)
 ![Supported SQLAlchemy Versions](https://img.shields.io/badge/SQLAlchemy-1.4%20%2F%202.0-brightgreen)
 
 [//]: # ([![codecov]&#40;https://codecov.io/gh/flipbit03/sqlalchemy-easy-softdelete/branch/main/graphs/badge.svg&#41;]&#40;https://codecov.io/github/flipbit03/sqlalchemy-easy-softdelete&#41;)
 
 Easily add soft-deletion to your SQLAlchemy Models and automatically filter out soft-deleted objects from your queries and relationships.
 
 This package can generate a tailor-made SQLAlchemy Mixin that can be added to your SQLAlchemy Models, making them contain a field that, when set, will mark the entity as being soft-deleted.
```

