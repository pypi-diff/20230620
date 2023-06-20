# Comparing `tmp/datamazing-0.0.2.tar.gz` & `tmp/datamazing-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-0.0.2.tar", max compression
+gzip compressed data, was "datamazing-0.0.3.tar", max compression
```

## Comparing `datamazing-0.0.2.tar` & `datamazing-0.0.3.tar`

### file list

```diff
@@ -1,3 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-19 13:06:07.174808 datamazing-0.0.2/datamazing/__init__.py
--rw-r--r--   0        0        0      690 2023-06-19 13:06:07.174808 datamazing-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      225 2023-06-20 08:36:26.019143 datamazing-0.0.3/datamazing/__init__.py
+-rw-r--r--   0        0        0      185 2023-06-20 08:36:26.019143 datamazing-0.0.3/datamazing/datacollection/__init__.py
+-rw-r--r--   0        0        0       21 2023-06-20 08:36:26.019143 datamazing-0.0.3/datamazing/transformations/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:36:26.019143 datamazing-0.0.3/datamazing/transformations/pandas/__init__.py
+-rw-r--r--   0        0        0      649 2023-06-20 08:36:26.019143 datamazing-0.0.3/datamazing/transformations/pandas/basic.py
+-rw-r--r--   0        0        0     1998 2023-06-20 08:36:26.019143 datamazing-0.0.3/datamazing/transformations/pandas/grouping.py
+-rw-r--r--   0        0        0      868 2023-06-20 08:36:26.019143 datamazing-0.0.3/datamazing/transformations/pandas/resampling.py
+-rw-r--r--   0        0        0      690 2023-06-20 08:36:26.019143 datamazing-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-0.0.3/PKG-INFO
```

### Comparing `datamazing-0.0.2/pyproject.toml` & `datamazing-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "0.0.2"
+version = "0.0.3"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `datamazing-0.0.2/PKG-INFO` & `datamazing-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamazing
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for working with pandas Dataset, but wit specialized functions used for Energinet
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

