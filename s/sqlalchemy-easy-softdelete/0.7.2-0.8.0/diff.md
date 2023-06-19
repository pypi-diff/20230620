# Comparing `tmp/sqlalchemy_easy_softdelete-0.7.2.tar.gz` & `tmp/sqlalchemy_easy_softdelete-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_easy_softdelete-0.7.2.tar", max compression
+gzip compressed data, was "sqlalchemy_easy_softdelete-0.8.0.tar", max compression
```

## Comparing `sqlalchemy_easy_softdelete-0.7.2.tar` & `sqlalchemy_easy_softdelete-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1497 2023-04-20 16:00:56.614862 sqlalchemy_easy_softdelete-0.7.2/LICENSE
--rw-r--r--   0        0        0     2875 2023-04-20 16:00:56.614862 sqlalchemy_easy_softdelete-0.7.2/README.md
--rw-r--r--   0        0        0     2264 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      140 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/__init__.py
--rw-r--r--   0        0        0       65 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/handler/__init__.py
--rw-r--r--   0        0        0     6089 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py
--rw-r--r--   0        0        0      850 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py
--rw-r--r--   0        0        0     1623 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/mixin.py
--rw-r--r--   0        0        0       56 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/__init__.py
--rw-r--r--   0        0        0     1971 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/conftest.py
--rw-r--r--   0        0        0     2580 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/model.py
--rw-r--r--   0        0        0      360 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/seed_data/__init__.py
--rw-r--r--   0        0        0     2025 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/seed_data/parent_child_childchild.py
--rw-r--r--   0        0        0        0 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/snapshots/__init__.py
--rw-r--r--   0        0        0     6518 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/snapshots/snap_test_queries.py
--rw-r--r--   0        0        0     9931 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/snapshots/snap_test_seed_data.py
--rw-r--r--   0        0        0     6340 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/test_queries.py
--rw-r--r--   0        0        0      595 2023-04-20 16:00:56.618862 sqlalchemy_easy_softdelete-0.7.2/tests/test_seed_data.py
--rw-r--r--   0        0        0     4478 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2977 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/README.md
+-rw-r--r--   0        0        0     1620 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/sqlalchemy_easy_softdelete/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/sqlalchemy_easy_softdelete/handler/__init__.py
+-rw-r--r--   0        0        0     6089 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py
+-rw-r--r--   0        0        0      850 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py
+-rw-r--r--   0        0        0     1623 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/sqlalchemy_easy_softdelete/mixin.py
+-rw-r--r--   0        0        0       56 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1971 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     2580 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/tests/model.py
+-rw-r--r--   0        0        0      360 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/tests/seed_data/__init__.py
+-rw-r--r--   0        0        0     2025 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/tests/seed_data/parent_child_childchild.py
+-rw-r--r--   0        0        0        0 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0     4006 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/tests/snapshots/snap_test_queries.py
+-rw-r--r--   0        0        0     9931 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/tests/snapshots/snap_test_seed_data.py
+-rw-r--r--   0        0        0     7591 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/tests/test_queries.py
+-rw-r--r--   0        0        0      595 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/tests/test_seed_data.py
+-rw-r--r--   0        0        0     1992 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-19 23:09:12.081643 sqlalchemy_easy_softdelete-0.8.0/tests/utils/simple_select_extractor.py
+-rw-r--r--   0        0        0     3746 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.8.0/PKG-INFO
```

### Comparing `sqlalchemy_easy_softdelete-0.7.2/LICENSE` & `sqlalchemy_easy_softdelete-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.2/README.md` & `sqlalchemy_easy_softdelete-0.8.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SQLAlchemy Easy Soft-Delete
 
 [![pypi](https://img.shields.io/pypi/v/sqlalchemy-easy-softdelete.svg)](https://pypi.org/project/sqlalchemy-easy-softdelete/)
 [![python](https://img.shields.io/pypi/pyversions/sqlalchemy-easy-softdelete.svg)](https://pypi.org/project/sqlalchemy-easy-softdelete/)
 [![Build Status](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml/badge.svg)](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml)
+![Supported SQLAlchemy Versions](https://img.shields.io/badge/SQLAlchemy-1.4%20%2F%202.0-brightgreen)
 
 [//]: # ([![codecov]&#40;https://codecov.io/gh/flipbit03/sqlalchemy-easy-softdelete/branch/main/graphs/badge.svg&#41;]&#40;https://codecov.io/github/flipbit03/sqlalchemy-easy-softdelete&#41;)
 
 Easily add soft-deletion to your SQLAlchemy Models and automatically filter out soft-deleted objects from your queries and relationships.
 
 This package can generate a tailor-made SQLAlchemy Mixin that can be added to your SQLAlchemy Models, making them contain a field that, when set, will mark the entity as being soft-deleted.
```

### Comparing `sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py` & `sqlalchemy_easy_softdelete-0.8.0/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py` & `sqlalchemy_easy_softdelete-0.8.0/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.2/sqlalchemy_easy_softdelete/mixin.py` & `sqlalchemy_easy_softdelete-0.8.0/sqlalchemy_easy_softdelete/mixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.2/tests/conftest.py` & `sqlalchemy_easy_softdelete-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.2/tests/model.py` & `sqlalchemy_easy_softdelete-0.8.0/tests/model.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.2/tests/seed_data/parent_child_childchild.py` & `sqlalchemy_easy_softdelete-0.8.0/tests/seed_data/parent_child_childchild.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.2/tests/snapshots/snap_test_seed_data.py` & `sqlalchemy_easy_softdelete-0.8.0/tests/snapshots/snap_test_seed_data.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.2/tests/test_queries.py` & `sqlalchemy_easy_softdelete-0.8.0/tests/test_queries.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,86 +3,113 @@
 
 import pytest
 from sqlalchemy import func, insert, select, table, text
 from sqlalchemy.orm import Query
 from sqlalchemy.sql import Select
 
 from tests.model import SDBaseRequest, SDChild, SDChildChild, SDDerivedRequest, SDParent, SDSimpleTable
+from tests.utils import is_filtering_for_softdeleted
 
 
 def test_query_single_table(snapshot, seeded_session, rewriter):
     """Query with one table"""
     test_query: Query = seeded_session.query(SDChild)
 
-    snapshot.assert_match(str(rewriter.rewrite_statement(test_query.statement)))
+    soft_deleted_rewritten_statement = rewriter.rewrite_statement(test_query.statement)
+
+    assert (
+        is_filtering_for_softdeleted(
+            soft_deleted_rewritten_statement,
+            {
+                SDChild.__table__,
+            },
+        )
+        is True
+    )
+
     snapshot.assert_match(sorted(test_query.all(), key=lambda i: i.id))
 
 
 def test_query_with_join(snapshot, seeded_session, rewriter):
     """Query with a simple join"""
     test_query: Query = seeded_session.query(SDChild).join(SDParent)  # noqa -- wrong typing stub in SA
 
-    snapshot.assert_match(str(rewriter.rewrite_statement(test_query.statement)))
+    soft_deleted_rewritten_statement = rewriter.rewrite_statement(test_query.statement)
+
+    assert (
+        is_filtering_for_softdeleted(soft_deleted_rewritten_statement, {SDChild.__table__, SDParent.__table__}) is True
+    )
 
     snapshot.assert_match(sorted(test_query.all(), key=lambda i: i.id))
 
 
 def test_query_union_sdchild(snapshot, seeded_session, rewriter):
     """Two queries joined via UNION"""
     test_query: Query = seeded_session.query(SDChild).union(seeded_session.query(SDChild))
 
-    snapshot.assert_match(str(rewriter.rewrite_statement(test_query.statement)))
+    soft_deleted_rewritten_statement = rewriter.rewrite_statement(test_query.statement)
+
+    assert is_filtering_for_softdeleted(soft_deleted_rewritten_statement, {SDChild.__table__}) is True
 
     snapshot.assert_match(sorted(test_query.all(), key=lambda i: i.id))
 
 
 def test_query_union_sdchild_core(snapshot, seeded_session, rewriter):
     """Two queries joined via UNION, using SQLAlchemy Core"""
     sdchild = SDChild.__table__
 
     select_as_core = (select(sdchild.c.id, sdchild.c.parent_id).select_from(sdchild)).union(
         select(sdchild.c.id, sdchild.c.parent_id).select_from(sdchild)
     )
 
-    snapshot.assert_match(str(rewriter.rewrite_statement(select_as_core)))
+    soft_deleted_rewritten_statement = rewriter.rewrite_statement(select_as_core)
+
+    assert is_filtering_for_softdeleted(soft_deleted_rewritten_statement, {SDChild.__table__}) is True
 
 
 def test_query_with_union_but_union_softdelete_disabled(snapshot, seeded_session, rewriter):
     """Two queries joined via UNION but the second one has soft-delete disabled"""
 
     # Two SDChild .all() queries with results joined via UNION
     # the first one has soft delete applied
     # the second one has soft delete DISABLED
     # the second query is a superset of the first one, and results in
     # all objects in the DB being returned
     test_query: Query = seeded_session.query(SDChild).union(
         seeded_session.query(SDChild).execution_options(include_deleted=True)
     )
 
-    snapshot.assert_match(str(rewriter.rewrite_statement(test_query.statement)))
+    soft_deleted_rewritten_statement = rewriter.rewrite_statement(test_query.statement)
+
+    assert is_filtering_for_softdeleted(soft_deleted_rewritten_statement, {SDChild.__table__}) is True
 
     all_children: List[SDChild] = seeded_session.query(SDChild).execution_options(include_deleted=True).all()
 
     assert sorted(test_query.all(), key=lambda x: x.id) == sorted(all_children, key=lambda x: x.id)
 
     snapshot.assert_match(sorted(test_query.all(), key=lambda i: i.id))
 
 
 def test_ensure_aggregate_from_multiple_table_deletion_works_active_object_count(snapshot, seeded_session, rewriter):
     """Aggregate function from a query that contains a join"""
     test_query: Query = seeded_session.query(SDChild).join(SDParent).with_entities(func.count())  # noqa
 
-    snapshot.assert_match(str(rewriter.rewrite_statement(test_query.statement)))
+    soft_deleted_rewritten_statement = rewriter.rewrite_statement(test_query.statement)
+
+    assert is_filtering_for_softdeleted(soft_deleted_rewritten_statement, {SDChild.__table__}) is True
+
     snapshot.assert_match(test_query.count())
 
 
 def test_ensure_table_with_inheritance_works(snapshot, seeded_session, rewriter):
     test_query: Query = seeded_session.query(SDDerivedRequest)
 
-    snapshot.assert_match(str(rewriter.rewrite_statement(test_query.statement)))
+    soft_deleted_rewritten_statement = rewriter.rewrite_statement(test_query.statement)
+
+    assert is_filtering_for_softdeleted(soft_deleted_rewritten_statement, {SDBaseRequest.__table__}) is True
 
     test_query_results = test_query.all()
     assert len(test_query_results) == 2
     snapshot.assert_match(sorted(test_query_results, key=lambda i: i.id))
 
     all_active_and_deleted_derived_requests = (
         seeded_session.query(SDDerivedRequest).execution_options(include_deleted=True).all()
@@ -142,17 +169,29 @@
 
     result = seeded_session.execute(insert_returning)
 
     assert list(result)[0][0].int_field == 10
 
 
 def test_query_with_more_than_one_join(snapshot, seeded_session, rewriter):
-    query = (
+    test_query = (
         seeded_session.query(SDParent)
         .join(SDChild)
         .join(SDChildChild)
         .filter(
             SDParent.id > 0,
         )
     )
 
-    snapshot.assert_match(str(rewriter.rewrite_statement(query.statement)))
+    soft_deleted_rewritten_statement = rewriter.rewrite_statement(test_query.statement)
+
+    assert (
+        is_filtering_for_softdeleted(
+            soft_deleted_rewritten_statement,
+            {
+                SDParent.__table__,
+                SDChild.__table__,
+                SDChildChild.__table__,
+            },
+        )
+        is True
+    )
```

### Comparing `sqlalchemy_easy_softdelete-0.7.2/tests/test_seed_data.py` & `sqlalchemy_easy_softdelete-0.8.0/tests/test_seed_data.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.7.2/PKG-INFO` & `sqlalchemy_easy_softdelete-0.8.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,33 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-easy-softdelete
-Version: 0.7.2
+Version: 0.8.0
 Summary: Easily add soft-deletion to your SQLAlchemy Models.
 Home-page: https://github.com/flipbit03/sqlalchemy-easy-softdelete
 License: BSD-3-Clause
 Author: Cadu
 Author-email: cadu.coelho@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Provides-Extra: dev
-Provides-Extra: test
 Requires-Dist: SQLAlchemy (>=1.4,<2.1)
-Requires-Dist: black (>=21.5b2,<22.0) ; extra == "test"
-Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
-Requires-Dist: flake8 (>=3.9.2,<4.0.0) ; extra == "test"
-Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
-Requires-Dist: isort (>=5.8.0,<6.0.0) ; extra == "test"
-Requires-Dist: pip ; extra == "dev"
-Requires-Dist: pre-commit (>=2.12.0,<3.0.0) ; extra == "dev"
-Requires-Dist: pytest (>=6.2.4,<7.0.0) ; extra == "test"
-Requires-Dist: pytest-cov (>=2.12.0,<3.0.0) ; extra == "test"
-Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
-Requires-Dist: tox (>=3.20.1,<4.0.0) ; extra == "dev"
-Requires-Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev"
-Requires-Dist: virtualenv (>=20.2.2,<21.0.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 # SQLAlchemy Easy Soft-Delete
 
 [![pypi](https://img.shields.io/pypi/v/sqlalchemy-easy-softdelete.svg)](https://pypi.org/project/sqlalchemy-easy-softdelete/)
 [![python](https://img.shields.io/pypi/pyversions/sqlalchemy-easy-softdelete.svg)](https://pypi.org/project/sqlalchemy-easy-softdelete/)
 [![Build Status](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml/badge.svg)](https://github.com/flipbit03/sqlalchemy-easy-softdelete/actions/workflows/test.yml)
+![Supported SQLAlchemy Versions](https://img.shields.io/badge/SQLAlchemy-1.4%20%2F%202.0-brightgreen)
 
 [//]: # ([![codecov]&#40;https://codecov.io/gh/flipbit03/sqlalchemy-easy-softdelete/branch/main/graphs/badge.svg&#41;]&#40;https://codecov.io/github/flipbit03/sqlalchemy-easy-softdelete&#41;)
 
 Easily add soft-deletion to your SQLAlchemy Models and automatically filter out soft-deleted objects from your queries and relationships.
 
 This package can generate a tailor-made SQLAlchemy Mixin that can be added to your SQLAlchemy Models, making them contain a field that, when set, will mark the entity as being soft-deleted.
```

