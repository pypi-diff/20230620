# Comparing `tmp/vstools-2.2.1.tar.gz` & `tmp/vstools-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstools-2.2.1.tar", last modified: Mon Jun  5 20:27:15 2023, max compression
+gzip compressed data, was "vstools-2.3.0.tar", last modified: Tue Jun 20 15:14:24 2023, max compression
```

## Comparing `vstools-2.2.1.tar` & `vstools-2.3.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.397402 vstools-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-05 20:26:47.000000 vstools-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-05 20:27:15.397402 vstools-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 20:26:47.000000 vstools-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 20:27:15.397402 vstools-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-05 20:26:47.000000 vstools-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.377401 vstools-2.2.1/vstools/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.381401 vstools-2.2.1/vstools/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34595 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/enums/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.385401 vstools-2.2.1/vstools/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/exceptions/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.389402 vstools-2.2.1/vstools/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/heuristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/timecodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.389402 vstools-2.2.1/vstools/types/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/types/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/types/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/types/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/types/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18463 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/types/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.397402 vstools-2.2.1/vstools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/__file_headers.json
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/clips.py
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/ffprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/mime_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/props.py
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)    27233 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/vs_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-06-05 20:26:47.000000 vstools-2.2.1/vstools/utils/vs_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:27:15.381401 vstools-2.2.1/vstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-05 20:27:15.000000 vstools-2.2.1/vstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-05 20:27:15.000000 vstools-2.2.1/vstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:27:15.000000 vstools-2.2.1/vstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 20:27:15.000000 vstools-2.2.1/vstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 20:27:15.000000 vstools-2.2.1/vstools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:14:24.189320 vstools-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 15:13:59.000000 vstools-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-20 15:14:24.189320 vstools-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-20 15:13:59.000000 vstools-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-20 15:14:24.189320 vstools-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-20 15:13:59.000000 vstools-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:14:24.173320 vstools-2.3.0/vstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:14:24.177320 vstools-2.3.0/vstools/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/enums/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34595 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/enums/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/enums/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/enums/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/enums/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/enums/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:14:24.181320 vstools-2.3.0/vstools/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/exceptions/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/exceptions/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/exceptions/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/exceptions/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/exceptions/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:14:24.181320 vstools-2.3.0/vstools/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/functions/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/functions/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/functions/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/functions/heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/functions/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/functions/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/functions/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/functions/timecodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20770 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:14:24.185320 vstools-2.3.0/vstools/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/types/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/types/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/types/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18450 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/types/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:14:24.189320 vstools-2.3.0/vstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/__file_headers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/clips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/ffprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10350 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/mime_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27233 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/vs_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28734 2023-06-20 15:13:59.000000 vstools-2.3.0/vstools/utils/vs_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:14:24.177320 vstools-2.3.0/vstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-20 15:14:24.000000 vstools-2.3.0/vstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-20 15:14:24.000000 vstools-2.3.0/vstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:14:24.000000 vstools-2.3.0/vstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 15:14:24.000000 vstools-2.3.0/vstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 15:14:24.000000 vstools-2.3.0/vstools.egg-info/top_level.txt
```

### Comparing `vstools-2.2.1/LICENSE` & `vstools-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/PKG-INFO` & `vstools-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstools
-Version: 2.2.1
+Version: 2.3.0
 Summary: Functions and utils related to VapourSynth
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-tools
 Project-URL: Documentation, https://vstools.encoding.moe/en/latest/
```

### Comparing `vstools-2.2.1/README.md` & `vstools-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/setup.cfg` & `vstools-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/setup.py` & `vstools-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/enums/base.py` & `vstools-2.3.0/vstools/enums/base.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/enums/color.py` & `vstools-2.3.0/vstools/enums/color.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/enums/generic.py` & `vstools-2.3.0/vstools/enums/generic.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/enums/other.py` & `vstools-2.3.0/vstools/enums/other.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/enums/stubs.py` & `vstools-2.3.0/vstools/enums/stubs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/exceptions/base.py` & `vstools-2.3.0/vstools/exceptions/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -151,35 +151,33 @@
             if sys.stdout and sys.stdout.isatty():
                 func_header = f'\033[0;36m{func_header}\033[0m'
 
             func_header = f'({func_header}) '
         else:
             func_header = ''
 
-        kwargs = self.kwargs.copy()
-
-        if kwargs:
-            kwargs = {
-                key: norm_display_name(value) for key, value in kwargs.items()
+        if self.kwargs:
+            self.kwargs = {
+                key: norm_display_name(value) for key, value in self.kwargs.items()
             }
 
         if self.reason:
-            reason = norm_display_name(self.reason)
+            reason = self.reason = norm_display_name(self.reason)
 
             if reason:
                 if not isinstance(self.reason, dict):
                     reason = f'({reason})'
 
                 if sys.stdout and sys.stdout.isatty():
                     reason = f'\033[0;33m{reason}\033[0m'
                 reason = f' {reason}'
         else:
             reason = ''
 
-        return f'{func_header}{self.message!s}{reason}'.format(**kwargs).strip()
+        return f'{func_header}{self.message!s}{reason}'.format(**self.kwargs).strip()
 
 
 SelfError = TypeVar('SelfError', bound=CustomError)
 
 
 class CustomValueError(CustomError, ValueError):
     """Thrown when a specified value is invalid."""
```

### Comparing `vstools-2.2.1/vstools/exceptions/color.py` & `vstools-2.3.0/vstools/exceptions/color.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/exceptions/enum.py` & `vstools-2.3.0/vstools/exceptions/enum.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/exceptions/file.py` & `vstools-2.3.0/vstools/exceptions/file.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/exceptions/generic.py` & `vstools-2.3.0/vstools/exceptions/generic.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/exceptions/module.py` & `vstools-2.3.0/vstools/exceptions/module.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/functions/check.py` & `vstools-2.3.0/vstools/functions/check.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/functions/clip.py` & `vstools-2.3.0/vstools/functions/clip.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/functions/funcs.py` & `vstools-2.3.0/vstools/functions/funcs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/functions/heuristics.py` & `vstools-2.3.0/vstools/functions/heuristics.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/functions/normalize.py` & `vstools-2.3.0/vstools/functions/normalize.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/functions/progress.py` & `vstools-2.3.0/vstools/functions/progress.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/functions/render.py` & `vstools-2.3.0/vstools/functions/render.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/functions/timecodes.py` & `vstools-2.3.0/vstools/functions/timecodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,34 +331,43 @@
 
             prop_clip, callback = mode.prepare_clip(clip, height), mode.check_cb()
 
             return replace_ranges(clip, propset_clip, callback, prop_src=prop_clip)
 
         return replace_ranges(clip, propset_clip, self)
 
-    def to_file(self, out: FilePathType, format: int = V1, func: FuncExceptT | None = None) -> None:
+    def to_file(
+        self, out: FilePathType, format: int = V1, func: FuncExceptT | None = None,
+        header: bool = True, force: bool = False
+    ) -> None:
         from ..utils import check_perms
 
         func = func or self.to_file
 
         out_path = Path(str(out)).resolve()
 
+        if out_path.exists():
+            if not force:
+                return
+
+            out_path.unlink()
+
         out_path.parent.mkdir(parents=True, exist_ok=True)
 
         check_perms(out_path, 'w+', func=func)
 
         if format == Keyframes.V1:
             out_text = [
-                '# keyframe format v1', 'fps 0', '',
+                *(['# keyframe format v1', 'fps 0', ''] if header else []),
                 *(f'{n} I -1' for n in self), ''
             ]
         elif format == Keyframes.XVID:
             lut_self = set(self)
             out_text = [
-                '# XviD 2pass stat file', '',
+                *(['# XviD 2pass stat file', '',] if header else []),
                 *(
                     (lut_self.remove(i) or 'i') if i in lut_self else 'b'  # type: ignore
                     for i in range(max(self))
                 )
             ]
 
         out_path.unlink(True)
```

### Comparing `vstools-2.2.1/vstools/functions/utils.py` & `vstools-2.3.0/vstools/functions/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import string
-from typing import Any, Iterable, Literal, Mapping, cast, overload
+from typing import Any, Iterable, Literal, Mapping, Sequence, cast, overload
 from weakref import WeakValueDictionary
 
 import vapoursynth as vs
 
 from ..enums import ColorRange, ColorRangeT, CustomStrEnum, Matrix
 from ..exceptions import ClipLengthError, CustomIndexError, CustomValueError, InvalidColorFamilyError
 from ..types import HoldsVideoFormatT, PlanesT, VideoFormatT
@@ -23,14 +23,16 @@
     'get_y', 'get_u', 'get_v',
     'get_r', 'get_g', 'get_b',
 
     'insert_clip',
 
     'plane',
     'join', 'split',
+
+    'stack_clips'
 ]
 
 
 EXPR_VARS = (alph := list(string.ascii_lowercase))[(idx := alph.index('x')):] + alph[:idx]
 """Variables to access clips in core.std.Expr."""
 
 
@@ -606,7 +608,30 @@
 
     assert check_variable_format(clip, split)
 
     return [clip] if clip.format.num_planes == 1 else cast(list[vs.VideoNode], clip.std.SplitPlanes())
 
 
 depth_func = depth
+
+
+def stack_clips(
+    clips: Sequence[vs.VideoNode | Sequence[vs.VideoNode | Sequence[
+        vs.VideoNode | Sequence[vs.VideoNode | Sequence[vs.VideoNode | Sequence[vs.VideoNode]]]
+    ]]]
+) -> vs.VideoNode:
+    """
+    Stack clips in the following repeating order: hor->ver->hor->ver->...
+
+    :param clips:   Sequence of clips to stack recursively.
+
+    :return:        Stacked clips.
+    """
+
+    return vs.core.std.StackHorizontal([
+        inner_clips if isinstance(inner_clips, vs.VideoNode) else (
+            vs.core.std.StackVertical([
+                clipa if isinstance(clipa, vs.VideoNode) else stack_clips(clipa) for clipa in inner_clips
+            ])
+        )
+        for inner_clips in clips
+    ])
```

### Comparing `vstools-2.2.1/vstools/types/builtins.py` & `vstools-2.3.0/vstools/types/builtins.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/types/file.py` & `vstools-2.3.0/vstools/types/file.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/types/funcs.py` & `vstools-2.3.0/vstools/types/funcs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/types/generic.py` & `vstools-2.3.0/vstools/types/generic.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/types/utils.py` & `vstools-2.3.0/vstools/types/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -436,48 +436,39 @@
     This is especially useful if you have to hold a reference to a VideoNode or Plugin/Function object
     in this object as you need to remove it for the VapourSynth core to be freed correctly.
     """
 
     __vsdel_register: Callable[[int], None] | None = None
 
     def __new__(cls: type[VSObjSelf], *args: Any, **kwargs: Any) -> VSObjSelf:
-        from ..utils.vs_proxy import register_on_creation, register_on_destroy
+        from ..utils.vs_proxy import core, register_on_creation
 
         try:
             self = super().__new__(cls, *args, **kwargs)
         except TypeError:
             self = super().__new__(cls)
 
         if hasattr(self, '__vs_del__'):
             def _register(core_id: int) -> None:
-                register_on_destroy(partial(self.__vs_del__, core_id))
+                self.__vsdel_partial_register = partial(self.__vs_del__, core_id)
+                core.register_on_destroy(self.__vsdel_partial_register)
 
             # [un]register_on_creation/destroy will only hold a weakref to the object
             self.__vsdel_register = _register
             register_on_creation(self.__vsdel_register)
 
         return self
 
     def __post_init__(self) -> None:
         ...
 
     if TYPE_CHECKING:
         def __vs_del__(self, core_id: int) -> None:
             """Special dunder that will be called when a core is getting freed."""
 
-    @staticmethod
-    def core_unbound(deleter: F) -> F:
-        """
-        Decorate a __vs_del__ with this to indicate that it should
-        be called when the environment is getting freed instead of the core.
-        """
-
-        deleter._is_core_unbound = True  # type: ignore
-        return deleter
-
 
 VSObjSelf = TypeVar('VSObjSelf', bound=vs_object)
 
 SingleMeta = TypeVar('SingleMeta', bound=type)
 
 
 class SingletonMeta(type):
@@ -504,45 +495,53 @@
 class Singleton(metaclass=SingletonMeta):
     """Handy class to inherit to have the SingletonMeta metaclass."""
 
 
 class VSDebug(Singleton, init=True):
     """Special class that follows the VapourSynth lifecycle for debug purposes."""
 
-    def __init__(self, *, env_life: bool = True, core_fetch: bool = False) -> None:
+    _print_func = print
+
+    def __init__(self, *, env_life: bool = True, core_fetch: bool = False, use_logging: bool = False) -> None:
         """
         Print useful debug information.
 
         :param env_life:    Print creation/destroy of VapourSynth environment.
         :param core_fetch:  Print traceback of the code that led to the first concrete core fetch.
                             Especially useful when trying to find the code path that is
                             locking you into a EnvironmentPolicy.
         """
 
         from ..utils.vs_proxy import register_on_creation
 
+        if use_logging:
+            import logging
+            VSDebug._print_func = logging.debug
+        else:
+            VSDebug._print_func = print
+
         if env_life:
-            register_on_creation(VSDebug._print_env_live)
+            register_on_creation(VSDebug._print_env_live, True)
 
         if core_fetch:
-            register_on_creation(VSDebug._print_stack)
+            register_on_creation(VSDebug._print_stack, True)
 
     @staticmethod
     def _print_stack(core_id: int) -> None:
         raise Exception
 
     @staticmethod
     def _print_env_live(core_id: int) -> None:
-        from ..utils.vs_proxy import core, get_current_environment, register_on_destroy
+        from ..utils.vs_proxy import core, register_on_destroy
 
-        print(f'New core created with id: {core_id}')
+        VSDebug._print_func(f'New core created with id: {core_id}')
 
-        core.register_on_destroy(VSDebug._print_core_destroy)
-        register_on_destroy(partial(VSDebug._print_destroy, get_current_environment().env_id, core_id))
+        core.register_on_destroy(VSDebug._print_core_destroy, False)
+        register_on_destroy(partial(VSDebug._print_destroy, core.env.env_id, core_id))
 
     @staticmethod
     def _print_destroy(env_id: int, core_id: int) -> None:
-        print(f'Environment destroyed with id: {env_id}, current core id: {core_id}')
+        VSDebug._print_func(f'Environment destroyed with id: {env_id}, current core id: {core_id}')
 
     @staticmethod
     def _print_core_destroy(_: int, core_id: int) -> None:
-        print(f'Core destroyed with id: {core_id}')
+        VSDebug._print_func(f'Core destroyed with id: {core_id}')
```

### Comparing `vstools-2.2.1/vstools/utils/__file_headers.json` & `vstools-2.3.0/vstools/utils/__file_headers.json`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/__init__.py` & `vstools-2.3.0/vstools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/cache.py` & `vstools-2.3.0/vstools/utils/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         if __key not in self:
             self.add_frame(__key, self.clip.get_frame(__key))  # type: ignore
 
         return super().__getitem__(__key)
 
     def __vs_del__(self, core_id: int) -> None:
         self.clear()
-        del self.clip
+        self.clip = None  # type: ignore
 
 
 class ClipFramesCache(vs_object, dict[vs.VideoNode, FramesCache[vs.VideoFrame]]):
     def _ensure_key(self, key: vs.VideoNode) -> None:
         if key not in self:
             super().__setitem__(key, FramesCache[vs.VideoFrame](key))
```

### Comparing `vstools-2.2.1/vstools/utils/clips.py` & `vstools-2.3.0/vstools/utils/clips.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/colors.py` & `vstools-2.3.0/vstools/utils/colors.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/ffprobe.py` & `vstools-2.3.0/vstools/utils/ffprobe.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/file.py` & `vstools-2.3.0/vstools/utils/file.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/funcs.py` & `vstools-2.3.0/vstools/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/info.py` & `vstools-2.3.0/vstools/utils/info.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/math.py` & `vstools-2.3.0/vstools/utils/math.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/mime.py` & `vstools-2.3.0/vstools/utils/mime.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,21 +202,25 @@
     """File type for generic files, like applications."""
 
     @classmethod
     def _missing_(cls, value: Any) -> FileType:
         if value is None:
             return FileType.AUTO
 
-        if isinstance(value, str) and '/' in value:
-            fbase, ftype, *_ = value.split('/')
+        if isinstance(value, str):
+            if '/' in value:
+                fbase, ftype, *_ = value.split('/')
 
-            if fbase == 'index':
-                return FileType.INDEX(ftype)
+                if fbase == 'index':
+                    return FileType.INDEX(ftype)
 
-            return FileType(ftype)
+                if value.endswith('-image'):
+                    return FileType.IMAGE
+
+                return FileType(ftype)
 
         return FileType.OTHER
 
     @inject_self.with_args(AUTO)
     def parse(
         self, path: FilePathType, *, func: FuncExceptT | None = None, force_ffprobe: bool | None = None
     ) -> ParsedFile:
```

### Comparing `vstools-2.2.1/vstools/utils/mime_base.py` & `vstools-2.3.0/vstools/utils/mime_base.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/misc.py` & `vstools-2.3.0/vstools/utils/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,26 +62,25 @@
     assert check_variable(ref, match_clip)
 
     clip = clip * ref.num_frames if length else clip
     clip = clip.resize.Bicubic(ref.width, ref.height) if dimensions else clip
 
     if vformat:
         assert ref.format
-        clip = clip.resize.Bicubic(format=ref.format, matrix=Matrix.from_video(ref))
+        clip = clip.resize.Bicubic(format=ref.format.id, matrix=Matrix.from_video(ref))
 
     if matrices:
         ref_frame = ref.get_frame(0)
         clip = clip.std.SetFrameProps(
             _Matrix=Matrix(ref_frame), _Transfer=Transfer(ref_frame), _Primaries=Primaries(ref_frame)
         )
 
     return clip.std.AssumeFPS(fpsnum=ref.fps.numerator, fpsden=ref.fps.denominator)
 
 
-
 def padder(
     clip: vs.VideoNode, left: int = 0, right: int = 0, top: int = 0, bottom: int = 0, reflect: bool = True
 ) -> vs.VideoNode:
     """
     Pad out the pixels on the side by the given amount of pixels.
 
     There are two padding modes:
@@ -151,35 +150,27 @@
     assert clip.format
 
     return func_float if clip.format.sample_type == vs.FLOAT else func_int
 
 
 def set_output(
     node: vs.RawNode | Iterable[vs.RawNode | Iterable[vs.RawNode | Iterable[vs.RawNode]]],
-    name: str | bool = True, cache: bool | None = None, **kwargs: Any
+    name: str | bool = True, **kwargs: Any
 ) -> None:
     """Set output node with optional name, and if available, use vspreview set_output."""
-    from ..functions import flatten
-    from ..utils import cache_clip
-
-    if cache is None:
-        try:
-            from vspreview import is_preview
-            cache = is_preview()
-        except Exception:
-            ...
+    from ..functions import flatten_vnodes
 
     last_index = len(vs.get_outputs())
 
     ref_id = str(id(node))
 
     title = 'Node'
 
     if isinstance(node, Iterable):
-        node = list[vs.RawNode](flatten(node))  # type: ignore
+        node = list[vs.RawNode](flatten_vnodes(node))  # type: ignore
         index = ''
     else:
         index = ' ' + str(last_index)
 
     checktype = node[0] if isinstance(node, list) else node
 
     if isinstance(checktype, vs.VideoNode):
@@ -200,24 +191,13 @@
                 name = vname
                 break
 
     try:
         from vspreview import set_output as vsp_set_output
         if isinstance(node, list):
             for idx, n in enumerate(node, 0 if index else last_index):
-                if cache:
-                    n = cache_clip(n)
                 vsp_set_output(n, name and f'{name} {idx}', **kwargs)
         else:
-            vsp_set_output(cache_clip(node) if cache else node, name, **kwargs)
+            vsp_set_output(node, name, **kwargs)
     except ModuleNotFoundError:
-        if isinstance(name, str) and isinstance(node, vs.VideoNode):
-            if isinstance(node, list):
-                for idx, n in enumerate(node, 0 if index else last_index):
-                    if cache:
-                        n = cache_clip(n)
-                    n.std.SetFrameProp('Name', data=f'{name.title()} {idx}').set_output(last_index)
-                    last_index += 1
-            else:
-                if cache:
-                    n = cache_clip(n)
-                n.std.SetFrameProp('Name', data=name.title()).set_output(last_index)
+        for idx, n in enumerate(node if isinstance(node, list) else [node], last_index):
+            n.set_output(idx)
```

### Comparing `vstools-2.2.1/vstools/utils/other.py` & `vstools-2.3.0/vstools/utils/other.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/props.py` & `vstools-2.3.0/vstools/utils/props.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/ranges.py` & `vstools-2.3.0/vstools/utils/ranges.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/scale.py` & `vstools-2.3.0/vstools/utils/scale.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/vs_enums.py` & `vstools-2.3.0/vstools/utils/vs_enums.py`

 * *Files identical despite different names*

### Comparing `vstools-2.2.1/vstools/utils/vs_proxy.py` & `vstools-2.3.0/vstools/utils/vs_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,18 @@
     TRANSFER_UNSPECIFIED, UNDEFINED, VIDEO, WIDE_LEFT, WIDE_RIGHT, YUV, AudioChannels, AudioFrame, AudioNode,
     ChromaLocation, ColorFamily, ColorPrimaries, ColorRange, Core, CoreCreationFlags, Environment, EnvironmentData,
     EnvironmentPolicy, EnvironmentPolicyAPI, Error, FieldBased, FilterMode, FrameProps, FramePtr, Func, FuncData,
     Function, LogHandle, MatrixCoefficients, MediaType, MessageType, Plugin, RawFrame, RawNode, SampleType,
     TransferCharacteristics, VideoFormat, VideoFrame, VideoNode, VideoOutputTuple, __api_version__, __version__,
     _CoreProxy, ccfDisableAutoLoading, ccfDisableLibraryUnloading, ccfEnableGraphInspection, clear_output,
     clear_outputs, fmFrameState, fmParallel, fmParallelRequests, fmUnordered, get_current_environment, get_output,
-    get_outputs, has_policy, register_policy
+    get_outputs, has_policy, register_on_destroy, register_policy, unregister_on_destroy
 )
 
 from ..exceptions import CustomRuntimeError
-from .other import IS_DOCS
 from .vs_enums import (
     GRAY8, GRAY9, GRAY10, GRAY11, GRAY12, GRAY13, GRAY14, GRAY15, GRAY16, GRAY17, GRAY18, GRAY19, GRAY20, GRAY21,
     GRAY22, GRAY23, GRAY24, GRAY25, GRAY26, GRAY27, GRAY28, GRAY29, GRAY30, GRAY31, GRAY32, GRAYH, GRAYS, RGB24, RGB27,
     RGB30, RGB33, RGB36, RGB39, RGB42, RGB45, RGB48, RGB51, RGB54, RGB57, RGB60, RGB63, RGB66, RGB69, RGB72, RGB75,
     RGB78, RGB81, RGB84, RGB87, RGB90, RGB93, RGB96, RGBH, RGBS, YUV410P8, YUV410P9, YUV410P10, YUV410P11, YUV410P12,
     YUV410P13, YUV410P14, YUV410P15, YUV410P16, YUV410P17, YUV410P18, YUV410P19, YUV410P20, YUV410P21, YUV410P22,
     YUV410P23, YUV410P24, YUV410P25, YUV410P26, YUV410P27, YUV410P28, YUV410P29, YUV410P30, YUV410P31, YUV410P32,
@@ -113,22 +112,20 @@
     'ccfEnableGraphInspection', 'clear_output', 'clear_outputs', 'construct_parameter', 'construct_signature',
     'construct_type', 'core', 'fmFrameState', 'fmParallel', 'fmParallelRequests', 'fmUnordered',
     'get_current_environment', 'get_output', 'get_outputs', 'has_policy', 'pyx_capi', 'register_on_creation',
     'register_on_destroy', 'register_policy', 'try_enable_introspection', 'unregister_on_creation',
     'unregister_on_destroy', 'vs_file', 'clear_cache'
 ]
 
-if IS_DOCS:
-    register_on_destroy_poly = True
-else:
-    register_on_destroy_poly = __version__.release_major < 61
 
 if not TYPE_CHECKING:
     import inspect
+    import re
     import sys
+    import warnings
     from pathlib import Path
     from types import ModuleType
 
     import __main__
 
     if not hasattr(__main__, '__file__') and '__vapoursynth__' not in sys.modules:
         first_stack = inspect.stack()[-1]
@@ -137,41 +134,40 @@
 
         cope = (Path.cwd() / first_stack.filename).resolve()
 
         sys.modules['__vapoursynth__'].__file__ = str(cope)
 
         sys.path.append(str(cope.parent))
 
-
-if not register_on_destroy_poly:
-    from vapoursynth import register_on_destroy, unregister_on_destroy
-else:
-    def register_on_destroy(callback: Callable[..., None]) -> None:
-        core.register_on_destroy(callback)
-
-    def unregister_on_destroy(callback: Callable[..., None]) -> None:
-        core.unregister_on_destroy(callback)
+    warnings._add_filter('ignore', re.compile('.*smallest subnormal.*numpy.*'), Warning, None, 0, append=False)
+    warnings._add_filter('ignore', re.compile('.*divide by zero.*'), Warning, None, 0, append=False)
 
 
-def register_on_creation(callback: Callable[..., None]) -> None:
+def register_on_creation(callback: Callable[..., None], strict: bool = False) -> None:
     """Register a callback on every core creation."""
     core_on_creation_callbacks.update({id(callback): weakref.ref(callback)})
 
+    if not strict and core.active:
+        try:
+            callback(core.core_id)
+        except TypeError:
+            callback()
+
 
 def unregister_on_creation(callback: Callable[..., None]) -> None:
     """Unregister this callback from every core creation."""
     core_on_creation_callbacks.pop(id(callback), None)
 
 
 def clear_cache() -> None:
     try:
-        cache_size = core.max_cache_size
+        cache_size = int(core.max_cache_size)
         core.max_cache_size = 1
         try:
-            for output in list(get_outputs().values()):
+            for output in get_outputs().values():
                 if isinstance(output, VideoOutputTuple):
                     output.clip.get_frame(0)
                     break
         except Exception:
             core.std.BlankClip().get_frame(0)
         core.max_cache_size = cache_size
     except Exception:
@@ -184,23 +180,30 @@
 
     class PluginProxyBase(Plugin):
         ...
 
     class CoreProxyBase(Core):
         def __init__(self) -> None:
             ...
+
+    class EnvironmentProxyBase(Environment):
+        def __init__(self) -> None:
+            ...
 else:
-    FunctionProxyBase = PluginProxyBase = CoreProxyBase = object
+    FunctionProxyBase = PluginProxyBase = CoreProxyBase = EnvironmentProxyBase = object
 
 
 class FunctionProxy(FunctionProxyBase):
     def __init__(self, plugin: PluginProxy, func_name: str) -> None:
         self.__dict__['func_ref'] = (plugin, func_name)
 
     def __getattr__(self, name: str) -> Function:
+        if name == '__isabstractmethod__':
+            return False  # type: ignore
+
         function = proxy_utils.get_vs_function(self)
 
         return getattr(function, name)  # type: ignore
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return proxy_utils.get_vs_function(self)(*args, **kwargs)
 
@@ -248,17 +251,17 @@
         vs_core_ref, vs_proxy = core.__dict__['vs_core_ref']
 
         vs_core = (vs_core_ref and vs_core_ref())
 
         if vs_core_ref and vs_core is None:
             if object.__getattribute__(vs_proxy, '_own_core'):
                 raise CustomRuntimeError('The VapourSynth core has been freed!', CoreProxy)
-            else:
-                vs_core = _get_core(vs_proxy)
-                core.__dict__['vs_core_ref'] = (vs_core and weakref.ref(vs_core), vs_proxy)
+
+            vs_core = _get_core(vs_proxy)
+            core.__dict__['vs_core_ref'] = (vs_core and weakref.ref(vs_core), vs_proxy)
 
         return vs_core or _get_core_with_cb()
 
     @staticmethod
     def get_vs_function(func: FunctionProxy) -> Function:
         plugin, func_name = proxy_utils.get_plugin(func)
         core, namespace = proxy_utils.get_core(plugin)
@@ -308,78 +311,151 @@
             'The core the proxy made reference to was freed!', 'VSCoreProxy'
         )
 
     return None
 
 
 if TYPE_CHECKING:
-    core_on_destroy_callbacks = dict[int, dict[int, weakref.ReferenceType[Callable[..., None]]]]()
+    core_on_destroy_callbacks = dict[int, dict[int, tuple[weakref.ReferenceType[Callable[..., None]], bool]]]()
 else:
     core_on_destroy_callbacks = {}
 
 if TYPE_CHECKING:
     core_on_creation_callbacks = dict[int, weakref.ReferenceType[Callable[..., None]]]()
 else:
     core_on_creation_callbacks = {}
 
 core_on_creation_callbacks_cores = set[int]()
 
 added_callback_cores = set[int]()
 
 
-def _finalize_core(env_id: int, core_id: int) -> None:
+def _finalize_core(env_id: int, core_id: int, _forced: bool = True) -> None:
     if env_id not in core_on_destroy_callbacks:
         return
 
-    destroy_env = env_id in core_on_destroy_callbacks
-
     for cb_id in list(core_on_destroy_callbacks[env_id].keys()):
-        callback_ref = core_on_destroy_callbacks[env_id].get(cb_id)
+        if _forced:
+            callback_ref = core_on_destroy_callbacks[env_id].get(cb_id)
+        else:
+            callback_ref = core_on_destroy_callbacks[env_id].pop(cb_id)
 
-        pop_cb = True
+        if callback_ref and (callback_ref[1] if _forced else True):
+            callback = callback_ref[0]()
 
-        if callback_ref and (callback := callback_ref()):
-            if hasattr(callback, '_is_core_unbound') and callback._is_core_unbound:
-                pop_cb = destroy_env = False
+            if not callback:
+                core_on_destroy_callbacks[env_id].pop(cb_id, None)
+                continue
 
             try:
                 callback(env_id, core_id)
             except TypeError:
                 callback()
 
-        if pop_cb:
-            core_on_destroy_callbacks[env_id].pop(cb_id, None)
-
-    if destroy_env:
+    if not _forced:
         core_on_destroy_callbacks.pop(env_id)
 
     gc.collect()
 
 
 def _get_core_with_cb(self: VSCoreProxy | None = None) -> Core:
-    core = _get_core(self) if self else None
+    _vs_core = _get_core(self) if self else None
 
-    if not core:
-        core = vs.core.core
+    if not _vs_core:
+        _vs_core = vs.core.core
 
-    if (core_id := id(core)) not in core_on_creation_callbacks_cores:
+    if (core_id := id(_vs_core)) not in core_on_creation_callbacks_cores:
         for cb_id in list(core_on_creation_callbacks.keys()):
-            if (callback_ref := core_on_creation_callbacks.pop(cb_id, None)) and (callback := callback_ref()):
+            callback_ref = core_on_creation_callbacks.get(cb_id, None)
+
+            if callback_ref and (callback := callback_ref()):
                 try:
                     callback(core_id)
                 except TypeError:
                     callback()
+            else:
+                # remove dead references
+                core_on_creation_callbacks.pop(cb_id, None)
 
-        core_on_creation_callbacks_cores.add(id(core))
+        core_on_creation_callbacks_cores.add(id(_vs_core))
 
     if core_id not in added_callback_cores:
         env_id = get_current_environment().env_id
-        weakref.finalize(core, lambda: _finalize_core(env_id, core_id))
+        weakref.finalize(_vs_core, lambda: _finalize_core(env_id, core_id, False))
+
+    return _vs_core
+
+
+def _find_ref(start_data: Any, to_return: type | tuple[type, ...], it: int = 3) -> Any:
+    if not it:
+        return None
+
+    for objects in [gc.get_referents(start_data), gc.get_referrers(start_data)]:
+        for obj in objects:
+            if isinstance(obj, to_return):
+                return obj
+
+            if (isinstance(obj, dict) and '__name__' in obj):
+                continue
 
-    return core
+            if isinstance(obj, (Core, _CoreProxy, _FastManager)):
+                continue
+
+            for obj_obj in gc.get_referents(obj):
+                if isinstance(obj_obj, to_return):
+                    return obj_obj
+
+                value = _find_ref(obj, to_return, it - 1)
+
+                if value:
+                    return value
+
+    return None
+
+
+class EnvironmentProxy(EnvironmentProxyBase):
+    def __getattr__(self, name: str) -> Plugin:
+        return getattr(get_current_environment(), name)  # type: ignore
+
+    def __setattr__(self, name: str, value: Any) -> None:
+        return setattr(get_current_environment(), name, value)
+
+    @property
+    def data(self) -> None:
+        data = self.env()  # type: ignore
+        assert data
+        return data  # type: ignore
+
+    @property
+    def policy(self) -> EnvironmentPolicy:
+        policy = _find_ref(self.data, (EnvironmentPolicy, VSScriptEnvironmentPolicy, StandaloneEnvironmentPolicy))
+        assert policy is not None
+        return policy  # type: ignore
+
+    @property
+    def api(self) -> EnvironmentPolicyAPI:
+        api = _find_ref(self.policy, EnvironmentPolicyAPI)
+        assert api is not None
+        return api  # type: ignore
+
+    @property
+    def has_core(self) -> bool:
+        import gc
+
+        found_core = _find_ref(self.data, Core)
+
+        if not found_core:
+            return False
+
+        core_refs = gc.get_referrers(found_core)
+
+        return len(core_refs) > 1
+
+
+_curr_env_proxy = EnvironmentProxy()
 
 
 class VSCoreProxy(CoreProxyBase):
     """Class for wrapping a VapourSynth core."""
 
     def __init__(self, core: Core | None = None) -> None:
         object.__setattr__(self, '_own_core', core is not None)
@@ -388,14 +464,32 @@
     def __getattr__(self, name: str) -> Plugin:
         return getattr(_get_core_with_cb(self), name)  # type: ignore
 
     def __setattr__(self, name: str, value: Any) -> None:
         return setattr(_get_core_with_cb(self), name, value)
 
     @property
+    def env(self) -> EnvironmentProxy:
+        if not has_policy():
+            raise CustomRuntimeError('No policy has been registered!')
+
+        return _curr_env_proxy
+
+    @property
+    def core_id(self) -> int:
+        if not self.active:
+            raise CustomRuntimeError("Core hasn't been fetched yet!")
+
+        return id(self.core)
+
+    @property
+    def active(self) -> bool:
+        return (has_policy() and self.env.has_core) or (_get_core(self) is not None)
+
+    @property
     def core(self) -> Core:
         """The underlying VapourSynth Core instance."""
         return _get_core_with_cb(self)
 
     @property
     def proxied(self) -> CoreProxy:
         """
@@ -423,25 +517,25 @@
             _objproxies[self] = {}
 
         if 'lazy' not in _objproxies[self]:
             _objproxies[self]['lazy'] = CoreProxy(None, self, True)
 
         return _objproxies[self]['lazy']  # type: ignore
 
-    def register_on_destroy(self, callback: Callable[..., None]) -> None:
+    def register_on_destroy(self, callback: Callable[..., None], on_forced: bool = True) -> None:
         """Register a callback on this core destroy."""
 
         _check_environment()
 
         env_id = get_current_environment().env_id
 
         if env_id not in core_on_destroy_callbacks:
-            core_on_destroy_callbacks[env_id] = {id(callback): weakref.ref(callback)}
+            core_on_destroy_callbacks[env_id] = {id(callback): (weakref.ref(callback), on_forced)}
         else:
-            core_on_destroy_callbacks[env_id] |= {id(callback): weakref.ref(callback)}
+            core_on_destroy_callbacks[env_id] |= {id(callback): (weakref.ref(callback), on_forced)}
 
     def unregister_on_destroy(self, callback: Callable[..., None]) -> None:
         """Unregister a callback from this core destroy."""
 
         _check_environment()
 
         env_id = get_current_environment().env_id
@@ -504,17 +598,14 @@
 
 def _core_on_destroy_try() -> None:
     ...
 
 
 def _check_environment() -> None:
     try:
-        if register_on_destroy_poly:
-            raise RuntimeError
-
         register_on_destroy(_core_on_destroy_try)
         unregister_on_destroy(_core_on_destroy_try)
     except Exception as e:
         if isinstance(e, ValueError) or not get_current_environment().active:
             raise ValueError("The environment has already been destroyed.")
 
 
@@ -594,17 +685,21 @@
 
     class PythonVSScriptLoggingBridge(Handler):
         def __init__(self, parent: Handler, level: int = LogLevelUnset) -> None:
             ...
 
         def emit(self, record: LogRecord) -> None:
             ...
+
+    class _FastManager:
+        ...
 else:
     from vapoursynth import (
         CallbackData, PythonVSScriptLoggingBridge, StandaloneEnvironmentPolicy, VSScriptEnvironmentPolicy
     )
     from vapoursynth import __file__ as vs_file
     from vapoursynth import __pyx_capi__ as pyx_capi
     from vapoursynth import _construct_parameter as construct_parameter
     from vapoursynth import _construct_type as construct_type
+    from vapoursynth import _FastManager
     from vapoursynth import _try_enable_introspection as try_enable_introspection
     from vapoursynth import construct_signature
```

### Comparing `vstools-2.2.1/vstools.egg-info/PKG-INFO` & `vstools-2.3.0/vstools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstools
-Version: 2.2.1
+Version: 2.3.0
 Summary: Functions and utils related to VapourSynth
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-tools
 Project-URL: Documentation, https://vstools.encoding.moe/en/latest/
```

### Comparing `vstools-2.2.1/vstools.egg-info/SOURCES.txt` & `vstools-2.3.0/vstools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

