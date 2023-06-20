# Comparing `tmp/bank_scrapers-1.0.3.tar.gz` & `tmp/bank_scrapers-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bank_scrapers-1.0.3.tar", last modified: Sun Jun 18 14:12:22 2023, max compression
+gzip compressed data, was "bank_scrapers-1.0.4.tar", last modified: Tue Jun 20 11:13:08 2023, max compression
```

## Comparing `bank_scrapers-1.0.3.tar` & `bank_scrapers-1.0.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/
--rw-rw-r--   0 eric      (1000) eric      (1000)     1066 2023-06-18 06:33:32.000000 bank_scrapers-1.0.3/LICENSE
--rw-rw-r--   0 eric      (1000) eric      (1000)    19810 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)    18278 2023-06-18 08:57:03.000000 bank_scrapers-1.0.3/README.md
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.631040 bank_scrapers-1.0.3/bank_scrapers/
--rw-rw-r--   0 eric      (1000) eric      (1000)      476 2023-06-18 14:11:13.000000 bank_scrapers-1.0.3/bank_scrapers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.631040 bank_scrapers-1.0.3/bank_scrapers/api_wrappers/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-12 11:03:00.000000 bank_scrapers-1.0.3/bank_scrapers/api_wrappers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.631040 bank_scrapers-1.0.3/bank_scrapers/api_wrappers/kraken/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-12 11:03:11.000000 bank_scrapers-1.0.3/bank_scrapers/api_wrappers/kraken/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     2863 2023-06-17 11:54:24.000000 bank_scrapers-1.0.3/bank_scrapers/api_wrappers/kraken/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/cli/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-18 04:02:26.000000 bank_scrapers-1.0.3/bank_scrapers/cli/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     9027 2023-06-18 08:52:15.000000 bank_scrapers-1.0.3/bank_scrapers/cli/cli.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/common/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-18 04:04:49.000000 bank_scrapers-1.0.3/bank_scrapers/common/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      272 2023-06-18 04:49:40.000000 bank_scrapers-1.0.3/bank_scrapers/common/log.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:17:21.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/becu/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/becu/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4284 2023-06-18 08:44:27.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/becu/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/chase/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/chase/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     9153 2023-06-18 14:10:29.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/chase/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/common/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:48:23.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/common/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4541 2023-06-18 14:09:43.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/common/functions.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/fidelity_netbenefits/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/fidelity_netbenefits/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8335 2023-06-18 14:10:29.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/fidelity_netbenefits/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/roundpoint/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/roundpoint/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8626 2023-06-18 14:10:29.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/roundpoint/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/smbc_prestia/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/smbc_prestia/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     4627 2023-06-18 08:44:27.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/smbc_prestia/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/uhfcu/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/uhfcu/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     8643 2023-06-18 14:10:29.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/uhfcu/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/vanguard/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/vanguard/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     7716 2023-06-18 14:10:29.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/vanguard/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/bank_scrapers/scrapers/zillow/
--rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/zillow/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     3457 2023-06-18 08:44:27.000000 bank_scrapers-1.0.3/bank_scrapers/scrapers/zillow/driver.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-18 14:12:22.631040 bank_scrapers-1.0.3/bank_scrapers.egg-info/
--rw-rw-r--   0 eric      (1000) eric      (1000)    19810 2023-06-18 14:12:22.000000 bank_scrapers-1.0.3/bank_scrapers.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     1347 2023-06-18 14:12:22.000000 bank_scrapers-1.0.3/bank_scrapers.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-06-18 14:12:22.000000 bank_scrapers-1.0.3/bank_scrapers.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       59 2023-06-18 14:12:22.000000 bank_scrapers-1.0.3/bank_scrapers.egg-info/entry_points.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      118 2023-06-18 14:12:22.000000 bank_scrapers-1.0.3/bank_scrapers.egg-info/requires.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       14 2023-06-18 14:12:22.000000 bank_scrapers-1.0.3/bank_scrapers.egg-info/top_level.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)      945 2023-06-18 14:11:13.000000 bank_scrapers-1.0.3/pyproject.toml
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-06-18 14:12:22.635040 bank_scrapers-1.0.3/setup.cfg
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1066 2023-06-18 06:33:32.000000 bank_scrapers-1.0.4/LICENSE
+-rw-rw-r--   0 eric      (1000) eric      (1000)    22197 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)    20665 2023-06-20 11:10:36.000000 bank_scrapers-1.0.4/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      476 2023-06-20 11:12:39.000000 bank_scrapers-1.0.4/bank_scrapers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/api_wrappers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-12 11:03:00.000000 bank_scrapers-1.0.4/bank_scrapers/api_wrappers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/api_wrappers/kraken/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-12 11:03:11.000000 bank_scrapers-1.0.4/bank_scrapers/api_wrappers/kraken/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2863 2023-06-17 11:54:24.000000 bank_scrapers-1.0.4/bank_scrapers/api_wrappers/kraken/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/cli/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-18 04:02:26.000000 bank_scrapers-1.0.4/bank_scrapers/cli/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     9027 2023-06-18 08:52:15.000000 bank_scrapers-1.0.4/bank_scrapers/cli/cli.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-18 04:04:49.000000 bank_scrapers-1.0.4/bank_scrapers/common/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      272 2023-06-18 04:49:40.000000 bank_scrapers-1.0.4/bank_scrapers/common/log.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:17:21.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/becu/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/becu/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4284 2023-06-18 08:44:27.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/becu/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/chase/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/chase/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     9191 2023-06-19 14:19:32.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/chase/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/common/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:48:23.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/common/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4712 2023-06-20 11:11:51.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/common/functions.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/fidelity_netbenefits/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/fidelity_netbenefits/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8335 2023-06-18 14:10:29.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/fidelity_netbenefits/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/roundpoint/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/roundpoint/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8626 2023-06-18 14:25:51.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/roundpoint/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/smbc_prestia/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/smbc_prestia/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     4632 2023-06-20 10:44:36.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/smbc_prestia/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/uhfcu/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/uhfcu/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     8655 2023-06-20 10:47:15.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/uhfcu/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/vanguard/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/vanguard/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     7740 2023-06-20 10:47:15.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/vanguard/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers/scrapers/zillow/
+-rw-rw-r--   0 eric      (1000) eric      (1000)        0 2023-06-11 08:18:17.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/zillow/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3457 2023-06-18 08:44:27.000000 bank_scrapers-1.0.4/bank_scrapers/scrapers/zillow/driver.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/bank_scrapers.egg-info/
+-rw-rw-r--   0 eric      (1000) eric      (1000)    22197 2023-06-20 11:13:08.000000 bank_scrapers-1.0.4/bank_scrapers.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1347 2023-06-20 11:13:08.000000 bank_scrapers-1.0.4/bank_scrapers.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-06-20 11:13:08.000000 bank_scrapers-1.0.4/bank_scrapers.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       59 2023-06-20 11:13:08.000000 bank_scrapers-1.0.4/bank_scrapers.egg-info/entry_points.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      118 2023-06-20 11:13:08.000000 bank_scrapers-1.0.4/bank_scrapers.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       14 2023-06-20 11:13:08.000000 bank_scrapers-1.0.4/bank_scrapers.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)      945 2023-06-20 11:12:39.000000 bank_scrapers-1.0.4/pyproject.toml
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-06-20 11:13:08.967790 bank_scrapers-1.0.4/setup.cfg
```

### Comparing `bank_scrapers-1.0.3/LICENSE` & `bank_scrapers-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.3/PKG-INFO` & `bank_scrapers-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bank_scrapers
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library for working with bank_scrapers drivers.
 Author: Eric Bette
 License: MIT License
         
         Copyright (c) 2023 Eric Bette
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,39 +25,116 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: homepage, https://github.com/eebette/bank_scrapers/tree/master
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Table of Contents
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [Introduction](#introduction)
+- [Getting Started](#getting-started)
+  - [Installation](#installation)
+  - [Usage](#usage)
 - [Drivers](#drivers)
   - [BECU](#becu)
   - [Chase](#chase)
   - [Fidelity NetBenefits](#fidelity-netbenefits)
   - [RoundPoint](#roundpoint)
   - [SMBC Prestia](#smbc-prestia)
   - [UHFCU](#uhfcu)
   - [Vanguard](#vanguard)
   - [Zillow](#zillow)
 - [API Wrappers](#api-wrappers)
   - [Kraken](#kraken)
+- [Disclaimer](#disclaimer)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
+# Quick Start 
+
+```shell
+pip install bank_scrapers
+```
+
+```shell
+bank-scrape {subcommand} $LOGIN_USER $LOGIN_PASS
+```
+
 # Introduction
 
 `bank_scrapers` is a library containing drivers for scraping account information from various financial websites. 
 
 Since most traditional financial institutions don't provide an API for accessing one's account data, most of these
 drivers utilize `Selenium` to impersonate the user using the provided credentials.
 
+# Getting Started
+
+## Installation
+
+### `stable`
+```shell
+pip install bank_scrapers
+```
+
+
+### `experimental`
+```shell
+pip install git+https://github.com/eebette/bank_scrapers.git
+```
+
+## Usage
+
+> 💡 Usage examples for each driver are listed in that driver's documentation
+
+### CLI
+
+#### For general info and complete usage documentation
+```shell
+bank-scrape -h
+```
+
+#### General usage pattern
+```shell
+bank-scrape {subcommand} $LOGIN_USER $LOGIN_PASS
+```
+
+### API
+
+API results are returned as a Python list of pandas dataframes, containing relevant data scraped from the site. See each
+ driver's section for info on what is in that driver's return tables. 
+
+```python
+from bank_scrapers.scrapers.becu.driver import get_accounts_info
+
+tables = get_accounts_info(username="{username}", password="{password}")
+for t in tables:
+  print(t.to_string())
+```
+
+#### Drivers that need a tmp directory
+
+Some drivers download the accounts data and process the downloaded file. This requires the use of a temp directory to
+ use as Chromium's downloads folder, and **the location of this folder must be specified in `get_accounts_info()`**.
+
+> ❗️Selenium often has issues writing to `/tmp/` in Linux distributions, hence this requirement in the code.
+
+> ❗️**NOTE** `tmp_dir` MUST be empty for this function to work
+
+```python
+from bank_scrapers.scrapers.fidelity_netbenefits.driver import get_accounts_info
+
+tables = get_accounts_info(username="{username}", password="{password}", tmp_dir="~/tmp")
+for t in tables:
+  print(t.to_string())
+```
+
+    
 # Drivers
 
 These are all written in Python using the Selenium driver and, for the most part, try to simulate the real user
 experience/workflow as seen in the eyes of the website provider. 
 
 ## BECU
 
@@ -81,20 +158,20 @@
 
 tables = get_accounts_info(username="{username}", password="{password}")
 for t in tables:
   print(t.to_string())
 ```
 #### Example Result
 ```
-      Account  YTD Interest  Current Balance  Available Balance
-0  ##########          #.##          ####.##            ####.##
-1  ##########         ##.##         #####.##           #####.##
-2  ##########        ###.##         #####.##           #####.##
-   Account  Current Balance  Available Credit
-0     ####           ###.##           #####.#
+   Account  YTD Interest  Current Balance  Available Balance
+##########          #.##          ####.##            ####.##
+##########         ##.##         #####.##           #####.##
+##########        ###.##         #####.##           #####.##
+ Account  Current Balance  Available Credit
+    ####           ###.##           #####.#
 ```
 
 ### Return Schema
 
 #### For non-loan Account
 | Column Name       |
 |-------------------|
@@ -626,7 +703,19 @@
 ### Return Schema
 
 #### Balance Info
 | Column Name |
 |-------------|
 | symbol      |
 | quantity    |
+
+# Disclaimer
+
+The intended purpose of this code is purely academic in nature, and it IS NOT intended to be used for any real life
+production use, nefarious or otherwise.
+
+Usage of this code is potentially against your bank's terms of service and could result in you or your IP getting
+flagged, listed, or blocked as bad actors. I don't take any responsibility for any effects this code may have on your
+bank accounts or your relationships with your banking institutions.
+
+Please don't try to learn anything about me or my life based on the banks that I've arbitrarily decided to write
+drivers for.
```

### Comparing `bank_scrapers-1.0.3/README.md` & `bank_scrapers-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,109 @@
+# Table of Contents
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [Introduction](#introduction)
+- [Getting Started](#getting-started)
+  - [Installation](#installation)
+  - [Usage](#usage)
 - [Drivers](#drivers)
   - [BECU](#becu)
   - [Chase](#chase)
   - [Fidelity NetBenefits](#fidelity-netbenefits)
   - [RoundPoint](#roundpoint)
   - [SMBC Prestia](#smbc-prestia)
   - [UHFCU](#uhfcu)
   - [Vanguard](#vanguard)
   - [Zillow](#zillow)
 - [API Wrappers](#api-wrappers)
   - [Kraken](#kraken)
+- [Disclaimer](#disclaimer)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
+# Quick Start 
+
+```shell
+pip install bank_scrapers
+```
+
+```shell
+bank-scrape {subcommand} $LOGIN_USER $LOGIN_PASS
+```
+
 # Introduction
 
 `bank_scrapers` is a library containing drivers for scraping account information from various financial websites. 
 
 Since most traditional financial institutions don't provide an API for accessing one's account data, most of these
 drivers utilize `Selenium` to impersonate the user using the provided credentials.
 
+# Getting Started
+
+## Installation
+
+### `stable`
+```shell
+pip install bank_scrapers
+```
+
+
+### `experimental`
+```shell
+pip install git+https://github.com/eebette/bank_scrapers.git
+```
+
+## Usage
+
+> 💡 Usage examples for each driver are listed in that driver's documentation
+
+### CLI
+
+#### For general info and complete usage documentation
+```shell
+bank-scrape -h
+```
+
+#### General usage pattern
+```shell
+bank-scrape {subcommand} $LOGIN_USER $LOGIN_PASS
+```
+
+### API
+
+API results are returned as a Python list of pandas dataframes, containing relevant data scraped from the site. See each
+ driver's section for info on what is in that driver's return tables. 
+
+```python
+from bank_scrapers.scrapers.becu.driver import get_accounts_info
+
+tables = get_accounts_info(username="{username}", password="{password}")
+for t in tables:
+  print(t.to_string())
+```
+
+#### Drivers that need a tmp directory
+
+Some drivers download the accounts data and process the downloaded file. This requires the use of a temp directory to
+ use as Chromium's downloads folder, and **the location of this folder must be specified in `get_accounts_info()`**.
+
+> ❗️Selenium often has issues writing to `/tmp/` in Linux distributions, hence this requirement in the code.
+
+> ❗️**NOTE** `tmp_dir` MUST be empty for this function to work
+
+```python
+from bank_scrapers.scrapers.fidelity_netbenefits.driver import get_accounts_info
+
+tables = get_accounts_info(username="{username}", password="{password}", tmp_dir="~/tmp")
+for t in tables:
+  print(t.to_string())
+```
+
+    
 # Drivers
 
 These are all written in Python using the Selenium driver and, for the most part, try to simulate the real user
 experience/workflow as seen in the eyes of the website provider. 
 
 ## BECU
 
@@ -50,20 +127,20 @@
 
 tables = get_accounts_info(username="{username}", password="{password}")
 for t in tables:
   print(t.to_string())
 ```
 #### Example Result
 ```
-      Account  YTD Interest  Current Balance  Available Balance
-0  ##########          #.##          ####.##            ####.##
-1  ##########         ##.##         #####.##           #####.##
-2  ##########        ###.##         #####.##           #####.##
-   Account  Current Balance  Available Credit
-0     ####           ###.##           #####.#
+   Account  YTD Interest  Current Balance  Available Balance
+##########          #.##          ####.##            ####.##
+##########         ##.##         #####.##           #####.##
+##########        ###.##         #####.##           #####.##
+ Account  Current Balance  Available Credit
+    ####           ###.##           #####.#
 ```
 
 ### Return Schema
 
 #### For non-loan Account
 | Column Name       |
 |-------------------|
@@ -594,8 +671,20 @@
 
 ### Return Schema
 
 #### Balance Info
 | Column Name |
 |-------------|
 | symbol      |
-| quantity    |
+| quantity    |
+
+# Disclaimer
+
+The intended purpose of this code is purely academic in nature, and it IS NOT intended to be used for any real life
+production use, nefarious or otherwise.
+
+Usage of this code is potentially against your bank's terms of service and could result in you or your IP getting
+flagged, listed, or blocked as bad actors. I don't take any responsibility for any effects this code may have on your
+bank accounts or your relationships with your banking institutions.
+
+Please don't try to learn anything about me or my life based on the banks that I've arbitrarily decided to write
+drivers for.
```

### Comparing `bank_scrapers-1.0.3/bank_scrapers/api_wrappers/kraken/driver.py` & `bank_scrapers-1.0.4/bank_scrapers/api_wrappers/kraken/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.3/bank_scrapers/cli/cli.py` & `bank_scrapers-1.0.4/bank_scrapers/cli/cli.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.3/bank_scrapers/scrapers/becu/driver.py` & `bank_scrapers-1.0.4/bank_scrapers/scrapers/becu/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.3/bank_scrapers/scrapers/chase/driver.py` & `bank_scrapers-1.0.4/bank_scrapers/scrapers/chase/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 for t in tables:
     print(t.to_string())
 ```
 """
 
 # Standard Library Imports
 from typing import Dict
+from time import sleep
 
 # Non-Standard Imports
 import pandas as pd
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.by import By
 
 # Local Imports
@@ -62,14 +63,15 @@
     # Wait for the expand option to become clickable or else can lead to bugs where the list doesn't expand correctly
     expand_button: WebElement = wait_and_find_click_element(
         driver, wait, (By.ID, "header-simplerAuth-dropdownoptions-styledselect")
     )
 
     # Then click it
     expand_button.click()
+    sleep(0.5)
 
     # Identify MFA options
     labels: List[WebElement] = wait_and_find_elements(
         driver, wait, (By.XPATH, "//a[@role='option']")
     )
 
     # Prompt user input for MFA option
```

### Comparing `bank_scrapers-1.0.3/bank_scrapers/scrapers/common/functions.py` & `bank_scrapers-1.0.4/bank_scrapers/scrapers/common/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,29 +29,25 @@
     A workaround for getting this to run on arm64. Use the locally installed chromedriver as a base if it's there
     :param options: An Options object to use for the driver
     :return: An undetectable chrome instance
     """
     # Check if there's an existing chromedriver
     if os.path.exists("/usr/bin/chromedriver"):
 
-        filepath = os.path.join(f"{Path.home()}/.local/share/undetected_chromedriver", "chromedriver_copy")
+        filepath = os.path.join(
+            f"{Path.home()}/.local/share/undetected_chromedriver", "chromedriver_copy"
+        )
         if not os.path.exists(f"{Path.home()}/.local/share/undetected_chromedriver"):
             os.makedirs(f"{Path.home()}/.local/share/undetected_chromedriver")
 
         # If there is, copy it to the undetected chrome installation path
-        shutil.copy(
-            "/usr/bin/chromedriver",
-            filepath,
-        )
+        shutil.copy("/usr/bin/chromedriver", filepath)
 
         # Instantiating the Driver with the chromedriver copy
-        driver: Chrome = Chrome(
-            options=options,
-            driver_executable_path=filepath,
-        )
+        driver: Chrome = Chrome(options=options, driver_executable_path=filepath)
     else:
         # Otherwise start as normal
         driver: Chrome = Chrome(options=options)
 
     return driver
 
 
@@ -115,16 +111,20 @@
     try:
         driver.find_element(*identifier)
     except NoSuchElementException:
         return False
     return True
 
 
-def leave_on_timeout(driver):
+def leave_on_timeout(driver: WebDriver | WebElement | Chrome | ShadowRoot) -> None:
+    """
+    Takes a screenshot of the current page in the user's some folder and exits with code 1
+    :param driver: The web driver object that is exiting
+    """
     print(driver.current_url)
     driver.save_screenshot(
         f"{Path.home()}/{datetime.today().strftime('%Y%M%d%H%m%s')}.png"
     )
     print(
         f"Screenshot saved to {Path.home()}/bank_scrapers_err_{datetime.today().strftime('%Y%M%d%H%m%s')}.png"
     )
-    sys.exit(1)
+    sys.exit(1)
```

### Comparing `bank_scrapers-1.0.3/bank_scrapers/scrapers/fidelity_netbenefits/driver.py` & `bank_scrapers-1.0.4/bank_scrapers/scrapers/fidelity_netbenefits/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.3/bank_scrapers/scrapers/roundpoint/driver.py` & `bank_scrapers-1.0.4/bank_scrapers/scrapers/roundpoint/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # Local Imports
 from bank_scrapers.scrapers.common.functions import *
 
 # Logon page
 HOMEPAGE: str = "https://loansphereservicingdigital.bkiconnect.com/servicinghome/#/login"
 
 # Timeout
-TIMEOUT: int = 15
+TIMEOUT: int = 30
 
 # Chrome config
 CHROME_OPTIONS: List[str] = [
     "--no-sandbox",
     "--window-size=1920,1080",
     "--headless",
     "--disable-gpu",
```

### Comparing `bank_scrapers-1.0.3/bank_scrapers/scrapers/smbc_prestia/driver.py` & `bank_scrapers-1.0.4/bank_scrapers/scrapers/smbc_prestia/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import pandas as pd
 from selenium.webdriver.common.by import By
 
 # Local Imports
 from bank_scrapers.scrapers.common.functions import *
 
 # Logon page
-HOMEPAGE = "https://login.smbctb.co.jp/ib/portal/POSNIN1prestiatop.prst?LOCALE=en_JP"
+HOMEPAGE: str = "https://login.smbctb.co.jp/ib/portal/POSNIN1prestiatop.prst?LOCALE=en_JP"
 
 # Timeout
 TIMEOUT: int = 15
 
 # Chrome config
 CHROME_OPTIONS: List[str] = [
     "--no-sandbox",
```

### Comparing `bank_scrapers-1.0.3/bank_scrapers/scrapers/uhfcu/driver.py` & `bank_scrapers-1.0.4/bank_scrapers/scrapers/uhfcu/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
     # Enter Password
     passwd: WebElement = wait_and_find_element(driver, wait, (By.ID, "password"))
     passwd.send_keys(password)
     sleep(2)
 
     # Submit will sometimes stay inactive unless interacted with
-    submit = wait_and_find_click_element(
+    submit: WebElement = wait_and_find_click_element(
         driver, wait, (By.XPATH, "//button[@type='submit']")
     )
     submit.click()
 
 
 def seek_credit_accounts_data(
     driver: Chrome, wait: WebDriverWait, t: WebElement
```

### Comparing `bank_scrapers-1.0.3/bank_scrapers/scrapers/vanguard/driver.py` & `bank_scrapers-1.0.4/bank_scrapers/scrapers/vanguard/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     # Enter Password
     passwd: WebElement = wait_and_find_element(
         driver, wait, (By.ID, "PASSWORD-blocked")
     )
     passwd.send_keys(password)
 
     # Submit credentials
-    submit = wait_and_find_click_element(
+    submit: WebElement = wait_and_find_click_element(
         driver, wait, (By.ID, "username-password-submit-btn")
     )
     submit.click()
 
 
 def seek_accounts_data(driver: Chrome, wait: WebDriverWait, tmp_dir: str) -> None:
     """
@@ -161,15 +161,15 @@
     wait.until(EC.presence_of_element_located((By.ID, "mat-checkbox-1-input")))
     mat_checkbox = wait_and_find_click_element(
         driver, wait, (By.ID, "mat-checkbox-1-input")
     )
     mat_checkbox.click()
 
     # Submit download request
-    submit = wait_and_find_click_element(driver, wait, (By.ID, "submitOFXDownload"))
+    submit: WebElement = wait_and_find_click_element(driver, wait, (By.ID, "submitOFXDownload"))
     submit.click()
 
     # Allow the download to process
     while not os.path.exists(f"{tmp_dir}/OfxDownload.csv"):
         sleep(1)
```

### Comparing `bank_scrapers-1.0.3/bank_scrapers/scrapers/zillow/driver.py` & `bank_scrapers-1.0.4/bank_scrapers/scrapers/zillow/driver.py`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.3/bank_scrapers.egg-info/PKG-INFO` & `bank_scrapers-1.0.4/bank_scrapers.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bank-scrapers
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library for working with bank_scrapers drivers.
 Author: Eric Bette
 License: MIT License
         
         Copyright (c) 2023 Eric Bette
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,39 +25,116 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: homepage, https://github.com/eebette/bank_scrapers/tree/master
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Table of Contents
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [Introduction](#introduction)
+- [Getting Started](#getting-started)
+  - [Installation](#installation)
+  - [Usage](#usage)
 - [Drivers](#drivers)
   - [BECU](#becu)
   - [Chase](#chase)
   - [Fidelity NetBenefits](#fidelity-netbenefits)
   - [RoundPoint](#roundpoint)
   - [SMBC Prestia](#smbc-prestia)
   - [UHFCU](#uhfcu)
   - [Vanguard](#vanguard)
   - [Zillow](#zillow)
 - [API Wrappers](#api-wrappers)
   - [Kraken](#kraken)
+- [Disclaimer](#disclaimer)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
+# Quick Start 
+
+```shell
+pip install bank_scrapers
+```
+
+```shell
+bank-scrape {subcommand} $LOGIN_USER $LOGIN_PASS
+```
+
 # Introduction
 
 `bank_scrapers` is a library containing drivers for scraping account information from various financial websites. 
 
 Since most traditional financial institutions don't provide an API for accessing one's account data, most of these
 drivers utilize `Selenium` to impersonate the user using the provided credentials.
 
+# Getting Started
+
+## Installation
+
+### `stable`
+```shell
+pip install bank_scrapers
+```
+
+
+### `experimental`
+```shell
+pip install git+https://github.com/eebette/bank_scrapers.git
+```
+
+## Usage
+
+> 💡 Usage examples for each driver are listed in that driver's documentation
+
+### CLI
+
+#### For general info and complete usage documentation
+```shell
+bank-scrape -h
+```
+
+#### General usage pattern
+```shell
+bank-scrape {subcommand} $LOGIN_USER $LOGIN_PASS
+```
+
+### API
+
+API results are returned as a Python list of pandas dataframes, containing relevant data scraped from the site. See each
+ driver's section for info on what is in that driver's return tables. 
+
+```python
+from bank_scrapers.scrapers.becu.driver import get_accounts_info
+
+tables = get_accounts_info(username="{username}", password="{password}")
+for t in tables:
+  print(t.to_string())
+```
+
+#### Drivers that need a tmp directory
+
+Some drivers download the accounts data and process the downloaded file. This requires the use of a temp directory to
+ use as Chromium's downloads folder, and **the location of this folder must be specified in `get_accounts_info()`**.
+
+> ❗️Selenium often has issues writing to `/tmp/` in Linux distributions, hence this requirement in the code.
+
+> ❗️**NOTE** `tmp_dir` MUST be empty for this function to work
+
+```python
+from bank_scrapers.scrapers.fidelity_netbenefits.driver import get_accounts_info
+
+tables = get_accounts_info(username="{username}", password="{password}", tmp_dir="~/tmp")
+for t in tables:
+  print(t.to_string())
+```
+
+    
 # Drivers
 
 These are all written in Python using the Selenium driver and, for the most part, try to simulate the real user
 experience/workflow as seen in the eyes of the website provider. 
 
 ## BECU
 
@@ -81,20 +158,20 @@
 
 tables = get_accounts_info(username="{username}", password="{password}")
 for t in tables:
   print(t.to_string())
 ```
 #### Example Result
 ```
-      Account  YTD Interest  Current Balance  Available Balance
-0  ##########          #.##          ####.##            ####.##
-1  ##########         ##.##         #####.##           #####.##
-2  ##########        ###.##         #####.##           #####.##
-   Account  Current Balance  Available Credit
-0     ####           ###.##           #####.#
+   Account  YTD Interest  Current Balance  Available Balance
+##########          #.##          ####.##            ####.##
+##########         ##.##         #####.##           #####.##
+##########        ###.##         #####.##           #####.##
+ Account  Current Balance  Available Credit
+    ####           ###.##           #####.#
 ```
 
 ### Return Schema
 
 #### For non-loan Account
 | Column Name       |
 |-------------------|
@@ -626,7 +703,19 @@
 ### Return Schema
 
 #### Balance Info
 | Column Name |
 |-------------|
 | symbol      |
 | quantity    |
+
+# Disclaimer
+
+The intended purpose of this code is purely academic in nature, and it IS NOT intended to be used for any real life
+production use, nefarious or otherwise.
+
+Usage of this code is potentially against your bank's terms of service and could result in you or your IP getting
+flagged, listed, or blocked as bad actors. I don't take any responsibility for any effects this code may have on your
+bank accounts or your relationships with your banking institutions.
+
+Please don't try to learn anything about me or my life based on the banks that I've arbitrarily decided to write
+drivers for.
```

### Comparing `bank_scrapers-1.0.3/bank_scrapers.egg-info/SOURCES.txt` & `bank_scrapers-1.0.4/bank_scrapers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bank_scrapers-1.0.3/pyproject.toml` & `bank_scrapers-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 dependencies = [
     "beautifulsoup4>=4.12.2",
     "pandas>=2.0.2",
     "requests>=2.31.0",
     "undetected-chromedriver>=3.5.0",
     "lxml>=4.9.2",
-    "bank_scrapers==1.0.3",
+    "bank_scrapers==1.0.4",
 ]
 
 [project.urls]
 homepage = "https://github.com/eebette/bank_scrapers/tree/master"
 
 [project.scripts]
 bank-scrape = "bank_scrapers.cli.cli:main"
```

