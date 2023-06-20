# Comparing `tmp/boxtec-2.8.tar.gz` & `tmp/boxtec-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxtec-2.8.tar", last modified: Fri Oct 21 15:20:25 2022, max compression
+gzip compressed data, was "boxtec-2.9.tar", last modified: Wed Oct 26 21:25:48 2022, max compression
```

## Comparing `boxtec-2.8.tar` & `boxtec-2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2022-10-21 15:20:25.060478 boxtec-2.8/
--rw-r--r--   0 max        (501) staff       (20)      110 2022-10-21 15:20:25.060360 boxtec-2.8/PKG-INFO
-drwxr-xr-x   0 max        (501) staff       (20)        0 2022-10-21 15:20:25.059640 boxtec-2.8/boxtec/
--rw-r--r--   0 max        (501) staff       (20)       29 2022-10-21 15:12:01.000000 boxtec-2.8/boxtec/__init__.py
--rw-r--r--   0 max        (501) staff       (20)      316 2022-10-19 12:22:38.000000 boxtec-2.8/boxtec/db.py
--rw-r--r--   0 max        (501) staff       (20)     1262 2022-10-19 17:17:19.000000 boxtec-2.8/boxtec/dt.py
--rw-r--r--   0 max        (501) staff       (20)      600 2022-10-21 15:20:17.000000 boxtec-2.8/boxtec/scraper.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2022-10-21 15:20:25.060200 boxtec-2.8/boxtec.egg-info/
--rw-r--r--   0 max        (501) staff       (20)      110 2022-10-21 15:20:24.000000 boxtec-2.8/boxtec.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      228 2022-10-21 15:20:25.000000 boxtec-2.8/boxtec.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2022-10-21 15:20:24.000000 boxtec-2.8/boxtec.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       21 2022-10-21 15:20:24.000000 boxtec-2.8/boxtec.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)        7 2022-10-21 15:20:25.000000 boxtec-2.8/boxtec.egg-info/top_level.txt
--rw-r--r--   0 max        (501) staff       (20)       38 2022-10-21 15:20:25.060521 boxtec-2.8/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)      292 2022-10-19 12:08:39.000000 boxtec-2.8/setup.py
--rw-r--r--   0 max        (501) staff       (20)        3 2022-10-21 15:20:24.000000 boxtec-2.8/version
+drwxr-xr-x   0 max        (501) staff       (20)        0 2022-10-26 21:25:48.989085 boxtec-2.9/
+-rw-r--r--   0 max        (501) staff       (20)      110 2022-10-26 21:25:48.988971 boxtec-2.9/PKG-INFO
+drwxr-xr-x   0 max        (501) staff       (20)        0 2022-10-26 21:25:48.988183 boxtec-2.9/boxtec/
+-rw-r--r--   0 max        (501) staff       (20)       29 2022-10-21 15:12:01.000000 boxtec-2.9/boxtec/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)      574 2022-10-26 21:25:08.000000 boxtec-2.9/boxtec/db.py
+-rw-r--r--   0 max        (501) staff       (20)     1262 2022-10-19 17:17:19.000000 boxtec-2.9/boxtec/dt.py
+-rw-r--r--   0 max        (501) staff       (20)      577 2022-10-21 15:24:49.000000 boxtec-2.9/boxtec/scraper.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2022-10-26 21:25:48.988820 boxtec-2.9/boxtec.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)      110 2022-10-26 21:25:48.000000 boxtec-2.9/boxtec.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      228 2022-10-26 21:25:48.000000 boxtec-2.9/boxtec.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2022-10-26 21:25:48.000000 boxtec-2.9/boxtec.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       21 2022-10-26 21:25:48.000000 boxtec-2.9/boxtec.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)        7 2022-10-26 21:25:48.000000 boxtec-2.9/boxtec.egg-info/top_level.txt
+-rw-r--r--   0 max        (501) staff       (20)       38 2022-10-26 21:25:48.989125 boxtec-2.9/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)      292 2022-10-19 12:08:39.000000 boxtec-2.9/setup.py
+-rw-r--r--   0 max        (501) staff       (20)        3 2022-10-26 21:25:48.000000 boxtec-2.9/version
```

### Comparing `boxtec-2.8/boxtec/dt.py` & `boxtec-2.9/boxtec/dt.py`

 * *Files identical despite different names*

