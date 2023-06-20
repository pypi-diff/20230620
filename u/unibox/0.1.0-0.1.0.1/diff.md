# Comparing `tmp/unibox-0.1.0.tar.gz` & `tmp/unibox-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibox-0.1.0.tar", max compression
+gzip compressed data, was "unibox-0.1.0.1.tar", max compression
```

## Comparing `unibox-0.1.0.tar` & `unibox-0.1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35823 2023-06-18 08:36:51.420874 unibox-0.1.0/LICENSE
--rw-r--r--   0        0        0      386 2023-06-18 08:44:50.049574 unibox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       20 2023-06-18 08:36:51.420874 unibox-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-18 08:37:40.664482 unibox-0.1.0/unibox/__init__.py
--rw-r--r--   0        0        0      279 2023-06-18 08:43:55.025999 unibox-0.1.0/unibox/cli.py
--rw-r--r--   0        0        0       21 2023-06-18 08:43:55.014999 unibox-0.1.0/unibox/setup/__init__.py
--rw-r--r--   0        0        0      118 2023-06-18 08:43:55.005596 unibox-0.1.0/unibox/setup/setups.py
--rw-r--r--   0        0        0      503 1970-01-01 00:00:00.000000 unibox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-06-18 08:36:51.420874 unibox-0.1.0.1/LICENSE
+-rw-r--r--   0        0        0      388 2023-06-20 06:39:29.456309 unibox-0.1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-06-20 05:35:32.564227 unibox-0.1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 08:37:40.664482 unibox-0.1.0.1/unibox/__init__.py
+-rw-r--r--   0        0        0      744 2023-06-20 06:37:27.318871 unibox-0.1.0.1/unibox/cli.py
+-rw-r--r--   0        0        0       21 2023-06-18 08:43:55.014999 unibox-0.1.0.1/unibox/setup/__init__.py
+-rw-r--r--   0        0        0     1213 2023-06-20 06:37:45.192416 unibox-0.1.0.1/unibox/setup/setups.py
+-rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 unibox-0.1.0.1/PKG-INFO
```

### Comparing `unibox-0.1.0/LICENSE` & `unibox-0.1.0.1/LICENSE`

 * *Files identical despite different names*

