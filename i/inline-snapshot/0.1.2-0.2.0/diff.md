# Comparing `tmp/inline_snapshot-0.1.2.tar.gz` & `tmp/inline_snapshot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inline_snapshot-0.1.2.tar", max compression
+gzip compressed data, was "inline_snapshot-0.2.0.tar", max compression
```

## Comparing `inline_snapshot-0.1.2.tar` & `inline_snapshot-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2022-07-23 07:39:26.309198 inline_snapshot-0.1.2/LICENSE
--rw-r--r--   0        0        0     3804 2022-07-25 21:24:21.239347 inline_snapshot-0.1.2/README.md
--rw-r--r--   0        0        0       62 2022-07-25 19:49:01.300547 inline_snapshot-0.1.2/inline_snapshot/__init__.py
--rw-r--r--   0        0        0     3513 2022-12-11 06:30:51.707971 inline_snapshot-0.1.2/inline_snapshot/_inline_snapshot.py
--rw-r--r--   0        0        0     9101 2022-09-18 14:19:27.478278 inline_snapshot-0.1.2/inline_snapshot/_rewrite_code.py
--rw-r--r--   0        0        0     2468 2022-12-11 06:30:51.707971 inline_snapshot-0.1.2/inline_snapshot/pytest_plugin.py
--rw-r--r--   0        0        0     1019 2022-12-11 06:39:52.106406 inline_snapshot-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 inline_snapshot-0.1.2/setup.py
--rw-r--r--   0        0        0     5068 1970-01-01 00:00:00.000000 inline_snapshot-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-20 18:24:16.714717 inline_snapshot-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2053 2023-06-20 18:24:23.890787 inline_snapshot-0.2.0/README.md
+-rw-r--r--   0        0        0       62 2023-06-20 18:24:16.714717 inline_snapshot-0.2.0/inline_snapshot/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-20 18:24:23.890787 inline_snapshot-0.2.0/inline_snapshot/_format.py
+-rw-r--r--   0        0        0    14391 2023-06-20 18:24:23.890787 inline_snapshot-0.2.0/inline_snapshot/_inline_snapshot.py
+-rw-r--r--   0        0        0     5497 2023-06-20 18:24:23.890787 inline_snapshot-0.2.0/inline_snapshot/_rewrite_code.py
+-rw-r--r--   0        0        0     5445 2023-06-20 18:24:23.890787 inline_snapshot-0.2.0/inline_snapshot/pytest_plugin.py
+-rw-r--r--   0        0        0     1603 2023-06-20 18:24:32.250870 inline_snapshot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 inline_snapshot-0.2.0/PKG-INFO
```

### Comparing `inline_snapshot-0.1.2/LICENSE` & `inline_snapshot-0.2.0/LICENSE`

 * *Files identical despite different names*

