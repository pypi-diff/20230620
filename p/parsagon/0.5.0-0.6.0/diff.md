# Comparing `tmp/parsagon-0.5.0.tar.gz` & `tmp/parsagon-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.5.0.tar", last modified: Wed Mar 29 04:41:57 2023, max compression
+gzip compressed data, was "parsagon-0.6.0.tar", last modified: Tue Jun 20 07:17:13 2023, max compression
```

## Comparing `parsagon-0.5.0.tar` & `parsagon-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-03-29 04:41:57.139177 parsagon-0.5.0/
--rw-r--r--   0 amsuh    (10002)    18010     1095 2023-03-29 04:40:13.000000 parsagon-0.5.0/LICENSE
--rw-r--r--   0 amsuh    (10002)    18010      420 2023-03-29 04:41:57.139315 parsagon-0.5.0/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010       26 2023-03-29 04:40:13.000000 parsagon-0.5.0/README.md
--rw-r--r--   0 amsuh    (10002)    18010      104 2023-03-29 04:40:13.000000 parsagon-0.5.0/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010      541 2023-03-29 04:41:57.140116 parsagon-0.5.0/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-03-29 04:41:57.134182 parsagon-0.5.0/src/
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-03-29 04:41:57.136674 parsagon-0.5.0/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010     2207 2023-03-29 04:40:13.000000 parsagon-0.5.0/src/parsagon/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-03-29 04:41:57.138876 parsagon-0.5.0/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010      420 2023-03-29 04:41:57.000000 parsagon-0.5.0/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      246 2023-03-29 04:41:57.000000 parsagon-0.5.0/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-03-29 04:41:57.000000 parsagon-0.5.0/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010        6 2023-03-29 04:41:57.000000 parsagon-0.5.0/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010        9 2023-03-29 04:41:57.000000 parsagon-0.5.0/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-20 07:17:13.475489 parsagon-0.6.0/
+-rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-20 07:17:13.475125 parsagon-0.6.0/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1054 2023-06-20 07:00:10.000000 parsagon-0.6.0/README.md
+-rw-r--r--   0 amsuh    (10002)    18010     1220 2023-06-20 07:14:01.000000 parsagon-0.6.0/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-06-20 07:17:13.475588 parsagon-0.6.0/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-20 07:17:13.463320 parsagon-0.6.0/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.6.0/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-20 07:17:13.469691 parsagon-0.6.0/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       46 2023-06-19 21:24:16.000000 parsagon-0.6.0/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3634 2023-06-20 03:09:34.000000 parsagon-0.6.0/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.6.0/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010    10607 2023-06-19 04:36:28.000000 parsagon-0.6.0/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010     5625 2023-06-20 03:50:17.000000 parsagon-0.6.0/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     1085 2023-06-18 04:18:36.000000 parsagon-0.6.0/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-20 07:17:13.474752 parsagon-0.6.0/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.6.0/src/parsagon/tests/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-20 07:17:13.474360 parsagon-0.6.0/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-20 07:17:13.000000 parsagon-0.6.0/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      437 2023-06-20 07:17:13.000000 parsagon-0.6.0/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-06-20 07:17:13.000000 parsagon-0.6.0/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010      141 2023-06-20 07:17:13.000000 parsagon-0.6.0/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      319 2023-06-20 07:17:13.000000 parsagon-0.6.0/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010       18 2023-06-20 07:17:13.000000 parsagon-0.6.0/src/parsagon.egg-info/top_level.txt
```

