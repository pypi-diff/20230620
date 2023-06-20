# Comparing `tmp/opensearch_orm-0.1.9.tar.gz` & `tmp/opensearch_orm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch_orm-0.1.9.tar", max compression
+gzip compressed data, was "opensearch_orm-0.2.0.tar", max compression
```

## Comparing `opensearch_orm-0.1.9.tar` & `opensearch_orm-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-04-16 08:43:48.684499 opensearch_orm-0.1.9/LICENSE
--rw-r--r--   0        0        0     3199 2023-06-17 07:12:43.411841 opensearch_orm-0.1.9/README.md
--rw-r--r--   0        0        0      120 2023-04-16 08:43:48.684682 opensearch_orm-0.1.9/opensearchorm/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-16 08:43:48.684860 opensearch_orm-0.1.9/opensearchorm/aggs.py
--rw-r--r--   0        0        0      254 2023-04-16 08:43:48.684942 opensearch_orm-0.1.9/opensearchorm/model.py
--rw-r--r--   0        0        0     5570 2023-06-17 04:45:40.491762 opensearch_orm-0.1.9/opensearchorm/query.py
--rw-r--r--   0        0        0     6598 2023-06-19 09:46:32.475159 opensearch_orm-0.1.9/opensearchorm/session.py
--rw-r--r--   0        0        0      497 2023-04-16 08:43:48.685191 opensearch_orm-0.1.9/opensearchorm/utils.py
--rw-r--r--   0        0        0      443 2023-06-19 14:51:43.058855 opensearch_orm-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3813 1970-01-01 00:00:00.000000 opensearch_orm-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-16 08:43:48.684499 opensearch_orm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3199 2023-06-17 07:12:43.411841 opensearch_orm-0.2.0/README.md
+-rw-r--r--   0        0        0      120 2023-04-16 08:43:48.684682 opensearch_orm-0.2.0/opensearchorm/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-16 08:43:48.684860 opensearch_orm-0.2.0/opensearchorm/aggs.py
+-rw-r--r--   0        0        0      254 2023-04-16 08:43:48.684942 opensearch_orm-0.2.0/opensearchorm/model.py
+-rw-r--r--   0        0        0     5570 2023-06-17 04:45:40.491762 opensearch_orm-0.2.0/opensearchorm/query.py
+-rw-r--r--   0        0        0     6619 2023-06-19 15:24:22.408152 opensearch_orm-0.2.0/opensearchorm/session.py
+-rw-r--r--   0        0        0      497 2023-04-16 08:43:48.685191 opensearch_orm-0.2.0/opensearchorm/utils.py
+-rw-r--r--   0        0        0      443 2023-06-19 15:24:57.639486 opensearch_orm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3813 1970-01-01 00:00:00.000000 opensearch_orm-0.2.0/PKG-INFO
```

### Comparing `opensearch_orm-0.1.9/LICENSE` & `opensearch_orm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.9/README.md` & `opensearch_orm-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.9/opensearchorm/aggs.py` & `opensearch_orm-0.2.0/opensearchorm/aggs.py`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.9/opensearchorm/query.py` & `opensearch_orm-0.2.0/opensearchorm/query.py`

 * *Files identical despite different names*

### Comparing `opensearch_orm-0.1.9/opensearchorm/session.py` & `opensearch_orm-0.2.0/opensearchorm/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,21 +83,22 @@
         self.__limit = limit
         return self
 
     def offset(self, offset: int):
         self.__offset = offset
         return self
 
-    def sort_by(self, *fields: str):
+    def order_by(self, *fields: str):
         sort = []
         for field in fields:
             order = 'desc' if field.startswith('-') else 'asc'
             field = field.strip('+-')
             sort.append({field: order})
         self.__sort = sort
+        return self
 
     def _search(self, fields: List[str], **kwargs):
         """
         :arg fields: include source fields
 
         :arg kwargs: any additional arguments will be passed on to the opensearch-py call
         """
```

### Comparing `opensearch_orm-0.1.9/PKG-INFO` & `opensearch_orm-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-orm
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 Author: yim7
 Author-email: yimchiu7@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

