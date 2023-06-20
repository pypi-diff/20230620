# Comparing `tmp/naruno_api-0.58.0.tar.gz` & `tmp/naruno_api-0.58.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_api-0.58.0.tar", last modified: Mon May 22 16:18:01 2023, max compression
+gzip compressed data, was "naruno_api-0.58.1.tar", last modified: Tue Jun 20 12:51:06 2023, max compression
```

## Comparing `naruno_api-0.58.0.tar` & `naruno_api-0.58.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:18:01.286032 naruno_api-0.58.0/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 16:18:01.286032 naruno_api-0.58.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:18:01.286032 naruno_api-0.58.0/naruno_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 16:18:01.000000 naruno_api-0.58.0/naruno_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-22 16:18:01.000000 naruno_api-0.58.0/naruno_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:18:01.000000 naruno_api-0.58.0/naruno_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:18:01.000000 naruno_api-0.58.0/naruno_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 16:18:01.000000 naruno_api-0.58.0/naruno_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:18:01.000000 naruno_api-0.58.0/naruno_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:18:01.286032 naruno_api-0.58.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-22 16:17:45.000000 naruno_api-0.58.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:06.490291 naruno_api-0.58.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-20 12:51:06.490291 naruno_api-0.58.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:06.490291 naruno_api-0.58.1/naruno_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-20 12:51:06.000000 naruno_api-0.58.1/naruno_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-20 12:51:06.000000 naruno_api-0.58.1/naruno_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:51:06.000000 naruno_api-0.58.1/naruno_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:51:06.000000 naruno_api-0.58.1/naruno_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 12:51:06.000000 naruno_api-0.58.1/naruno_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:51:06.000000 naruno_api-0.58.1/naruno_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 12:51:06.490291 naruno_api-0.58.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 12:50:53.000000 naruno_api-0.58.1/setup.py
```

### Comparing `naruno_api-0.58.0/setup.py` & `naruno_api-0.58.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from setuptools import setup
 
 setup(
     name="naruno_api",
-    version="0.58.0",
+    version="0.58.1",
     description="""This is API mode installer for Naruno""",
     url="https://docs.naruno.org/",
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     license="MPL-2.0",
     install_requires="""
 flask==2.0.0
```

