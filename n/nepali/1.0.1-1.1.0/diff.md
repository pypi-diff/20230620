# Comparing `tmp/nepali-1.0.1.tar.gz` & `tmp/nepali-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepali-1.0.1.tar", last modified: Tue May 16 15:34:07 2023, max compression
+gzip compressed data, was "nepali-1.1.0.tar", last modified: Tue Jun 20 14:53:07 2023, max compression
```

## Comparing `nepali-1.0.1.tar` & `nepali-1.1.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.179097 nepali-1.0.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-05-16 15:33:53.000000 nepali-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-05-16 15:34:07.179097 nepali-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-05-16 15:33:53.000000 nepali-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.171095 nepali-1.0.1/nepali/
--rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3437 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/char.py
--rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/date_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.175096 nepali-1.0.1/nepali/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/_humanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/_nepalimonth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/_nepaliweek.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.175096 nepali-1.0.1/nepali/datetime/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/parser/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/parser/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      329 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.175096 nepali-1.0.1/nepali/locations/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   216494 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/locations/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/locations/_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/locations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/locations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.175096 nepali-1.0.1/nepali/number/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/number/_nepalinumber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/number/_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/number/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.175096 nepali-1.0.1/nepali/templatetags/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/templatetags/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4754 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/templatetags/nepalidatetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/templatetags/nepalinumber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.179097 nepali-1.0.1/nepali/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_date_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_humanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_nepalimonth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_nepaliweek.py
--rw-r--r--   0 runner    (1001) docker     (123)   117623 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_timezone.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1962 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/timezone.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.175096 nepali-1.0.1/nepali.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-05-16 15:34:07.000000 nepali-1.0.1/nepali.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-16 15:34:07.000000 nepali-1.0.1/nepali.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:34:07.000000 nepali-1.0.1/nepali.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 15:34:07.000000 nepali-1.0.1/nepali.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 15:34:07.179097 nepali-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-05-16 15:33:53.000000 nepali-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:53:07.818009 nepali-1.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-06-20 14:52:54.000000 nepali-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-06-20 14:53:07.818009 nepali-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-06-20 14:52:54.000000 nepali-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:53:07.802009 nepali-1.1.0/nepali/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3437 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/char.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/date_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:53:07.806009 nepali-1.1.0/nepali/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/datetime/_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/datetime/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/datetime/_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/datetime/_nepalimonth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/datetime/_nepaliweek.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:53:07.806009 nepali-1.1.0/nepali/datetime/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/datetime/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/datetime/parser/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/datetime/parser/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/datetime/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      329 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:53:07.810009 nepali-1.1.0/nepali/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   216494 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/locations/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/locations/_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/locations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/locations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:53:07.810009 nepali-1.1.0/nepali/number/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19561 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/number/_nepalinumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/number/_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/number/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:53:07.814009 nepali-1.1.0/nepali/templatetags/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/templatetags/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5789 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/templatetags/nepalidatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/templatetags/nepalinumber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:53:07.818009 nepali-1.1.0/nepali/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/tests/test_date_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/tests/test_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/tests/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/tests/test_nepalimonth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/tests/test_nepaliweek.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117664 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/tests/test_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/tests/test_timezone.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1995 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/timezone.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-06-20 14:52:54.000000 nepali-1.1.0/nepali/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:53:07.802009 nepali-1.1.0/nepali.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-06-20 14:53:07.000000 nepali-1.1.0/nepali.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-20 14:53:07.000000 nepali-1.1.0/nepali.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:53:07.000000 nepali-1.1.0/nepali.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 14:53:07.000000 nepali-1.1.0/nepali.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:53:07.818009 nepali-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1867 2023-06-20 14:52:54.000000 nepali-1.1.0/setup.py
```

### Comparing `nepali-1.0.1/LICENSE` & `nepali-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nepali-1.0.1/PKG-INFO` & `nepali-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,13 @@
-Metadata-Version: 2.1
-Name: nepali
-Version: 1.0.1
-Summary: nepalidatetime compatible with python's datetime feature. Converting nepali date to english, parsing nepali datetime, nepali timezone, and timedelta support in nepali datetime
-Home-page: https://github.com/opensource-nepal/py-nepali
-Author: opensource-nepal
-Author-email: aj3sshh@gmail.com, sugatbajracharya49@gmail.com
-Keywords: nepali date conversion,convert date,nepali date time,python convert date,parse nepali date time
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nepali
 
 [![PyPI version](https://badge.fury.io/py/nepali.svg)](https://badge.fury.io/py/nepali)
-[![CI status](https://github.com/opensource-nepal/py-nepali/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/opensource-nepal/py-nepali/actions)
+[![CI status](https://github.com/opensource-nepal/py-nepali/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/opensource-nepal/py-nepali/actions)
 [![Downloads](https://img.shields.io/pypi/dm/nepali.svg?maxAge=180)](https://pypi.org/project/nepali/)
-[![codecov](https://codecov.io/gh/opensource-nepal/py-nepali/branch/master/graph/badge.svg?token=PTUHYWCJ4I)](https://codecov.io/gh/opensource-nepal/py-nepali)
+[![codecov](https://codecov.io/gh/opensource-nepal/py-nepali/branch/main/graph/badge.svg?token=PTUHYWCJ4I)](https://codecov.io/gh/opensource-nepal/py-nepali)
 
 `nepali` is a python package containing features that will be useful for Nepali projects.
 
 The major feature of this package is nepalidatetime, which is compatible with python's datetime feature. It helps nepali date to english, parsing nepali datetime, nepali timezone, and timedelta support in nepali datetime.
 
 ## Example
 
@@ -307,15 +293,15 @@
 
 | Directive | Meaning                                                   | Example                        |
 | --------- | --------------------------------------------------------- | ------------------------------ |
 | `%A`      | Weekday as locale’s abbreviated name.                     | Sun, Mon, …, Sat (आइत, सोम, …) |
 | `%A`      | Weekday as locale’s full name.                            | Sunday, Monday, …, Saturday    |
 | `%d`      | Day of the month as a zero-padded decimal number.         | 01, 02, …, 31                  |
 | `%-d`     | Day of the month as a decimal number.                     | 1, 2, …, 31                    |
-| `%B`      | Month as locale’s full name.                              | Baishak, Jestha, …, Chaitra    |
+| `%B`      | Month as locale’s full name.                              | Baishakh, Jestha, …, Chaitra   |
 | `%m`      | Month as a zero-padded decimal number.                    | 01, 02, …, 12                  |
 | `%-m`     | Month as a decimal number.                                | 1, 2, …, 12                    |
 | `%y`      | Year without century as a zero-padded decimal number.     | 00, 01, …, 99                  |
 | `%Y`      | Year with century as a decimal number.                    | 2001, 2078, 2079, …, 2099      |
 | `%H`      | Hour (24-hour clock) as a zero-padded decimal number.     | 00, 01, …, 23                  |
 | `%-H`     | Hour (24-hour clock) as a decimal number.                 | 0, 1, 2, …, 23                 |
 | `%I`      | Hour (12-hour clock) as a zero-padded decimal number.     | 01, 02, …, 12                  |
@@ -443,91 +429,14 @@
 # Municipality
 get_municipality(name_nepali="विराटनगर")
 # Biratnagar Metropolitan City
 ```
 
 ---
 
-## For Django Template
-
-Add `'nepali'` to your `INSTALLED_APPS` setting.
-
-```python
-INSTALLED_APPS = [
-    ...
-    'nepali',
-    ...
-]
-```
-
-### nepalidatetime
-
-In your Template
-
-```python
-{% load nepalidatetime %}
-```
-
-#### nepalinow
-
-`nepalinow` renders the current Nepali date and time in 'en-US' locale (English).
-
-```python
-{% nepalinow %}
-```
-
-```python
-{% nepalinow '%Y-%m-%d' %}
-```
-
-#### nepalinow_ne
-
-`nepalinow_ne` renders the current Nepali date and time in 'ne' locale (Nepali).
-
-```python
-{% nepalinow_ne %}
-```
-
-#### nepalidate
-
-`nepalidate` renders the datetime object into nepali datetime format in 'en-US' locale (English).
-
-```python
-{{ datetime_obj|nepalidate:"%Y-%m-%d" }}
-```
-
-#### nepalidate_ne
-
-`nepalidate_ne` renders the datetime object into nepali datetime format in 'ne' locale (Nepali).
-
-```python
-{{ datetime_obj|nepalidate_ne:"%Y-%m-%d" }}
-```
-
-#### nepalihumanize
-
-`nepalihumanize` renders the datetime object to a human readable form for 'ne' locale (Nepali)
-
-```python
-{{ datetime_obj|nepalihumanize }}
-```
-
-### nepalinumber
-
-In your Template
-
-```python
-{% load nepalinumber %}
-```
-
-`nepalinumber` renders the english number into nepali format (devanagari)
-
-```python
-{{ forloop.counter|nepalinumber }}
-
-{{ 150|nepalinumber }}
-```
+## For Django
 
+We have created a new Django package called [django-nepali](https://github.com/opensource-nepal/django-nepali) to support `nepali` package. For more information, please visit [django-nepali](https://github.com/opensource-nepal/django-nepali).
 
 ## Contribution
 
 We appreciate feedback and contribution to this package. To get started please see our [contribution guide](CONTRIBUTION.md)
```

### Comparing `nepali-1.0.1/README.md` & `nepali-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,30 @@
+Metadata-Version: 2.1
+Name: nepali
+Version: 1.1.0
+Summary: nepalidatetime compatible with python's datetime feature. Converting nepali date to english, parsing nepali datetime, nepali timezone, and timedelta support in nepali datetime
+Home-page: https://github.com/opensource-nepal/py-nepali
+Author: opensource-nepal
+Author-email: aj3sshh@gmail.com, sugatbajracharya49@gmail.com
+License: MIT
+Project-URL: Source, https://github.com/opensource-nepal/py-nepali
+Project-URL: Changelog, https://github.com/opensource-nepal/py-nepali/blob/main/CHANGELOG.md
+Keywords: nepali date conversion,convert date,nepali date time,python convert date,parse nepali date time
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nepali
 
 [![PyPI version](https://badge.fury.io/py/nepali.svg)](https://badge.fury.io/py/nepali)
-[![CI status](https://github.com/opensource-nepal/py-nepali/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/opensource-nepal/py-nepali/actions)
+[![CI status](https://github.com/opensource-nepal/py-nepali/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/opensource-nepal/py-nepali/actions)
 [![Downloads](https://img.shields.io/pypi/dm/nepali.svg?maxAge=180)](https://pypi.org/project/nepali/)
-[![codecov](https://codecov.io/gh/opensource-nepal/py-nepali/branch/master/graph/badge.svg?token=PTUHYWCJ4I)](https://codecov.io/gh/opensource-nepal/py-nepali)
+[![codecov](https://codecov.io/gh/opensource-nepal/py-nepali/branch/main/graph/badge.svg?token=PTUHYWCJ4I)](https://codecov.io/gh/opensource-nepal/py-nepali)
 
 `nepali` is a python package containing features that will be useful for Nepali projects.
 
 The major feature of this package is nepalidatetime, which is compatible with python's datetime feature. It helps nepali date to english, parsing nepali datetime, nepali timezone, and timedelta support in nepali datetime.
 
 ## Example
 
@@ -293,15 +310,15 @@
 
 | Directive | Meaning                                                   | Example                        |
 | --------- | --------------------------------------------------------- | ------------------------------ |
 | `%A`      | Weekday as locale’s abbreviated name.                     | Sun, Mon, …, Sat (आइत, सोम, …) |
 | `%A`      | Weekday as locale’s full name.                            | Sunday, Monday, …, Saturday    |
 | `%d`      | Day of the month as a zero-padded decimal number.         | 01, 02, …, 31                  |
 | `%-d`     | Day of the month as a decimal number.                     | 1, 2, …, 31                    |
-| `%B`      | Month as locale’s full name.                              | Baishak, Jestha, …, Chaitra    |
+| `%B`      | Month as locale’s full name.                              | Baishakh, Jestha, …, Chaitra   |
 | `%m`      | Month as a zero-padded decimal number.                    | 01, 02, …, 12                  |
 | `%-m`     | Month as a decimal number.                                | 1, 2, …, 12                    |
 | `%y`      | Year without century as a zero-padded decimal number.     | 00, 01, …, 99                  |
 | `%Y`      | Year with century as a decimal number.                    | 2001, 2078, 2079, …, 2099      |
 | `%H`      | Hour (24-hour clock) as a zero-padded decimal number.     | 00, 01, …, 23                  |
 | `%-H`     | Hour (24-hour clock) as a decimal number.                 | 0, 1, 2, …, 23                 |
 | `%I`      | Hour (12-hour clock) as a zero-padded decimal number.     | 01, 02, …, 12                  |
@@ -429,91 +446,14 @@
 # Municipality
 get_municipality(name_nepali="विराटनगर")
 # Biratnagar Metropolitan City
 ```
 
 ---
 
-## For Django Template
-
-Add `'nepali'` to your `INSTALLED_APPS` setting.
-
-```python
-INSTALLED_APPS = [
-    ...
-    'nepali',
-    ...
-]
-```
-
-### nepalidatetime
-
-In your Template
-
-```python
-{% load nepalidatetime %}
-```
-
-#### nepalinow
-
-`nepalinow` renders the current Nepali date and time in 'en-US' locale (English).
-
-```python
-{% nepalinow %}
-```
-
-```python
-{% nepalinow '%Y-%m-%d' %}
-```
-
-#### nepalinow_ne
-
-`nepalinow_ne` renders the current Nepali date and time in 'ne' locale (Nepali).
-
-```python
-{% nepalinow_ne %}
-```
-
-#### nepalidate
-
-`nepalidate` renders the datetime object into nepali datetime format in 'en-US' locale (English).
-
-```python
-{{ datetime_obj|nepalidate:"%Y-%m-%d" }}
-```
-
-#### nepalidate_ne
-
-`nepalidate_ne` renders the datetime object into nepali datetime format in 'ne' locale (Nepali).
-
-```python
-{{ datetime_obj|nepalidate_ne:"%Y-%m-%d" }}
-```
-
-#### nepalihumanize
-
-`nepalihumanize` renders the datetime object to a human readable form for 'ne' locale (Nepali)
-
-```python
-{{ datetime_obj|nepalihumanize }}
-```
-
-### nepalinumber
-
-In your Template
-
-```python
-{% load nepalinumber %}
-```
-
-`nepalinumber` renders the english number into nepali format (devanagari)
-
-```python
-{{ forloop.counter|nepalinumber }}
-
-{{ 150|nepalinumber }}
-```
+## For Django
 
+We have created a new Django package called [django-nepali](https://github.com/opensource-nepal/django-nepali) to support `nepali` package. For more information, please visit [django-nepali](https://github.com/opensource-nepal/django-nepali).
 
 ## Contribution
 
 We appreciate feedback and contribution to this package. To get started please see our [contribution guide](CONTRIBUTION.md)
```

### Comparing `nepali-1.0.1/nepali/char.py` & `nepali-1.1.0/nepali/char.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.1/nepali/date_converter.py` & `nepali-1.1.0/nepali/date_converter.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.1/nepali/datetime/_datetime.py` & `nepali-1.1.0/nepali/datetime/_datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime as pythonDateTime
 
 from nepali.date_converter import converter as nepali_date_converter
-from nepali.timezone import NepaliTimeZone, utc_now, to_nepali_timezone
+from nepali.timezone import NepaliTimeZone, to_nepali_timezone, utc_now
 
 from ._nepalimonth import nepalimonth
 
 
 class formatter_class_mixin:
     """
     mixin for date time formatter.
@@ -13,39 +13,39 @@
     """
 
     def get_formatter_class(self):
         return self.__class__.init_formatter_class()
 
     @classmethod
     def init_formatter_class(cls):
-        if not hasattr(cls, "__formatter_class__Cache"):
+        if not hasattr(cls, "_formatter_class_cache"):
             from ._formatter import NepaliDateTimeFormatter
 
-            cls.__formatter_class__Cache = NepaliDateTimeFormatter
-        return cls.__formatter_class__Cache
+            cls._formatter_class_cache = NepaliDateTimeFormatter
+        return cls._formatter_class_cache
 
     @classmethod
     def get_strptime_method(cls):
-        if not hasattr(cls, "_strptime_method_CACHE"):
+        if not hasattr(cls, "_strptime_method_cache"):
             from .parser import strptime
 
-            cls._strptime_method_CACHE = strptime
-        return cls._strptime_method_CACHE
+            cls._strptime_method_cache = strptime
+        return cls._strptime_method_cache
 
     def strftime(self, format: str) -> str:
         return self.strftime_en(format)
 
     def strftime_en(self, format: str) -> str:
-        NepaliDateTimeFormatter = self.get_formatter_class()
-        formatter = NepaliDateTimeFormatter(self, devanagari=False)
+        nepali_datetime_formatter = self.get_formatter_class()
+        formatter = nepali_datetime_formatter(self, devanagari=False)
         return formatter.get_str(format)
 
     def strftime_ne(self, format: str) -> str:
-        NepaliDateTimeFormatter = self.get_formatter_class()
-        formatter = NepaliDateTimeFormatter(self, devanagari=True)
+        nepali_datetime_formatter = self.get_formatter_class()
+        formatter = nepali_datetime_formatter(self, devanagari=True)
         return formatter.get_str(format)
 
 
 class nepalidate(formatter_class_mixin):
     def __init__(self, year, month, day) -> None:
         if isinstance(month, nepalimonth):
             month = month.value
@@ -190,20 +190,19 @@
 
     @staticmethod
     def from_datetime(datetime_object):
         return nepalidate.from_date(datetime_object.date())
 
     @staticmethod
     def from_date(date_object):
-        npDate = nepalidate(
+        return nepalidate(
             *nepali_date_converter.english_to_nepali(
                 date_object.year, date_object.month, date_object.day
             )
         )
-        return npDate
 
     @staticmethod
     def from_nepalidatetime(datetime_object):
         return datetime_object.date()
 
     # property
```

### Comparing `nepali-1.0.1/nepali/datetime/_formatter.py` & `nepali-1.1.0/nepali/datetime/_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime as pythonDateTime
+
 from nepali import number
 from nepali.exceptions import (
     InvalidDateFormatException,
     InvalidNepaliDateTimeObjectException,
 )
 
 from ._datetime import nepalidate, nepalidatetime
@@ -36,15 +37,15 @@
         "M": "minute",
         "-M": "minute_nonzero",
         "S": "second",
         "-S": "second_nonzero",
     }
 
     def __init__(self, datetime_object, devanagari=False):
-        # TODO: Change variable npDateTime into snakecase: `np_date_time`
+        # TODO: Change variable npDateTime into snake case: `np_date_time`
         if type(datetime_object) == nepalidatetime:
             self.npDateTime = datetime_object
         elif type(datetime_object) == nepalidate:
             self.npDateTime = datetime_object.to_nepalidatetime()
         elif type(datetime_object) == pythonDateTime.date:
             self.npDateTime = nepalidatetime.from_date(datetime_object)
         elif type(datetime_object) == pythonDateTime.datetime:
@@ -96,15 +97,15 @@
             raise Exception("Unable to convert NepaliDateTime to str")
         time_str = "".join(time_str)
 
         return time_str
 
     def get_format_map(self, ch: str) -> str:
         if ch not in self.format_map:
-            raise InvalidDateFormatException("Invalid Date format %{}".format(ch))
+            raise InvalidDateFormatException(f"Invalid Date format %{ch}")
         return self.format_map[ch]
 
     @property
     def weekdayHalf(self):
         """
         %a
         """
```

### Comparing `nepali-1.0.1/nepali/datetime/_humanize.py` & `nepali-1.1.0/nepali/datetime/_humanize.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import datetime as pythonDateTime
-
 from nepali import number
-from nepali.timezone import now, to_nepali_timezone
-from nepali.exceptions import InvalidNepaliDateTimeObjectException
+from nepali.timezone import now
 
-from ._datetime import nepalidate, nepalidatetime
+from .utils import to_nepalidatetime
 
 
 class HumanizeDateTime:
     """
     HumanizeDate converts NepaliDateTime to nepali human readable form
     """
 
@@ -25,59 +22,48 @@
     def __init__(self, datetime_obj, **kwargs):
         """
         initializes humanize class
         datetime_obj: python datetime object to be humanized
         threshold (kwargs): threshold to be humanize
         format (kwargs): format to display behind threshold
         """
-        if type(datetime_obj) == nepalidatetime:
-            self.datetime_obj = datetime_obj.to_datetime()
-        elif type(datetime_obj) == nepalidate:
-            self.datetime_obj = nepalidatetime.from_nepali_date(
-                datetime_obj
-            ).to_datetime()
-        elif type(datetime_obj) == pythonDateTime.date:
-            self.datetime_obj = nepalidatetime.from_date(datetime_obj).to_datetime()
-        elif type(datetime_obj) == pythonDateTime.datetime:
-            self.datetime_obj = to_nepali_timezone(datetime_obj)
-        else:
-            raise InvalidNepaliDateTimeObjectException(
-                "Argument must be instance of NepaliDate or NepaliDateTime or datetime.datetime or datetime.date"
-            )
+        self.datetime_obj = to_nepalidatetime(datetime_obj)
 
         self.threshold = kwargs.get("threshold")
         self.format = kwargs.get("format")
 
         # seconds after from now to datetime_obj
         self.seconds = 0
 
     def __calc_seconds(self):
         """calculates total seconds from now"""
         current_date_time = now()
-        date = self.datetime_obj
-        self.seconds = int((current_date_time - date).total_seconds())
+
+        # TODO (@aj3sh): support datetime - nepalidatetime
+        self.seconds = int(
+            (current_date_time - self.datetime_obj.to_datetime()).total_seconds()
+        )
 
         self.interval_tense = self.__past_text
         if self.seconds < 0:
             self.seconds *= -1
             self.interval_tense = self.__future_text
 
         return self.seconds
 
     def to_str(self):
         """returns humanize string"""
         seconds = self.__calc_seconds()  # calculating seconds
 
-        if self.threshold is not None:
-            if seconds >= self.threshold:
-                return self.get_datetime().strip()
+        if self.threshold is not None and seconds >= self.threshold:
+            return self._get_datetime_str().strip()
 
-        return self.get_humanize().strip()
+        return self._get_humanize_str().strip()
 
-    def get_humanize(self):
+    def _get_humanize_str(self):
         """
         returns humanize datetime
         """
         interval_value = 0
         interval_text = ""
         if self.seconds == 0:
             # now
@@ -114,22 +100,21 @@
             interval_text = self.__year_text
 
         interval_value = number.english_to_nepali(interval_value)
         return (
             str(interval_value) + " " + str(interval_text) + " " + self.interval_tense
         )
 
-    def get_datetime(self):
+    def _get_datetime_str(self):
         """
         returns date in nepali characters
         """
         if not self.format:
             self.format = "%B %d, %Y"
-        ndt = nepalidatetime.from_datetime(self.datetime_obj)
-        return ndt.strftime_ne(self.format)
+        return self.datetime_obj.strftime_ne(self.format)
 
     def __str__(self):
         return self.to_str()
 
     def __repr__(self):
         return str(self)
```

### Comparing `nepali-1.0.1/nepali/datetime/_nepalimonth.py` & `nepali-1.1.0/nepali/datetime/_nepalimonth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from functools import cached_property
 from typing import Any, Dict, Optional, Union
 
-from .constants import MONTHS_EN, MONTHS_NE
+from nepali.constants import NEPALI_MONTHS_EN, NEPALI_MONTHS_NE
 
 
 class NepaliMonthMeta(type):
     _cache: Dict[int, "nepalimonth"] = {}
 
     def __call__(cls, month: Union[int, str], *args, **kwargs) -> "nepalimonth":
         """
@@ -36,41 +36,42 @@
         if value not in cls._cache:
             cls._cache[value] = super(NepaliMonthMeta, cls).__call__(
                 value, *args, **kwargs
             )
 
         return cls._cache[value]
 
-    def _parse_str(cls, month: str) -> int:
+    @staticmethod
+    def _parse_str(month: str) -> int:
         """
         Parses str value of the month and returns int.
 
         :param month: A string representing the month.
         :type month: str
         :return: An integer representing the month.
         :rtype: int
         :raises ValueError: If the given string does not represent a valid month.
         """
         if month.isdigit():
             return int(month)
 
         month = month.capitalize()
-        month_names = MONTHS_EN + MONTHS_NE
+        month_names = NEPALI_MONTHS_EN + NEPALI_MONTHS_NE
         try:
             index = month_names.index(month)
         except ValueError:
             raise ValueError(f"Invalid month name: {month}")
 
         return (index % 12) + 1
 
 
 class nepalimonth(metaclass=NepaliMonthMeta):
     """
     Represents Nepali month: Baishakh, Jestha, ..., Chaitra.
-    Baishak: 1,
+    Baishakh: 1,
     Jestha: 2,
     ...
     Chaitra: 12
 
     >>> nepalimonth(1)
     >>> nepalimonth("Baishakh")
     >>> nepalimonth("बैशाख")
@@ -103,13 +104,13 @@
     @cached_property
     def value(self) -> int:
         return self.__value
 
     @cached_property
     def name(self) -> str:
         """Month's english name"""
-        return MONTHS_EN[self.__value - 1]
+        return NEPALI_MONTHS_EN[self.__value - 1]
 
     @cached_property
     def name_ne(self) -> str:
         """Month's nepali name"""
-        return MONTHS_NE[self.__value - 1]
+        return NEPALI_MONTHS_NE[self.__value - 1]
```

### Comparing `nepali-1.0.1/nepali/datetime/_nepaliweek.py` & `nepali-1.1.0/nepali/datetime/_nepaliweek.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from functools import cached_property
 from typing import Any, Dict, Optional, Union
 
-from .constants import WEEKS_EN, WEEKS_NE, WEEKS_ABBR_EN, WEEKS_ABBR_NE
+from nepali.constants import WEEKS_ABBR_EN, WEEKS_ABBR_NE, WEEKS_EN, WEEKS_NE
 
 
 class NepaliWeekMeta(type):
     _cache: Dict[int, "nepaliweek"] = {}
 
     def __call__(cls, week: Union[int, str], *args, **kwargs) -> "nepaliweek":
         """
@@ -24,24 +24,25 @@
         elif isinstance(week, str):
             try:
                 value = cls._parse_str(week)
             except ValueError:
                 pass
 
         # checking if week is valid
-        if value is None or not (0 <= value <= 6):
+        if value is None or not 0 <= value <= 6:
             raise ValueError(f"Invalid week: {week}")
 
         # checking cache
         if value not in cls._cache:
             cls._cache[value] = super().__call__(value, *args, **kwargs)
 
         return cls._cache[value]
 
-    def _parse_str(cls, week: str) -> int:
+    @staticmethod
+    def _parse_str(week: str) -> int:
         """
         Parses str value of the week and returns int.
 
         :param week: A string representing the week.
         :type week: str
         :return: An integer representing the week.
         :rtype: int
```

### Comparing `nepali-1.0.1/nepali/datetime/parser/_parser.py` & `nepali-1.1.0/nepali/datetime/parser/_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nepali.exceptions import InvalidDateTimeFormatException, FormatNotMatchException
+from nepali.exceptions import FormatNotMatchException, InvalidDateTimeFormatException
 
 from .validators import validate
 
 __all__ = [
     "strptime",
     "parse",
 ]
@@ -49,28 +49,26 @@
         "%H:%M:%S:%f",
     ]
 
     _standard_datetime_format_CACHE = STANDARD_DATE_FORMAT.copy()
     for time_format in STANDARD_TIME_FORMAT:
         for date_format in STANDARD_DATE_FORMAT:
             _standard_datetime_format_CACHE += [
-                "{} {}".format(date_format, time_format)
-            ]
-            _standard_datetime_format_CACHE += [
-                "{}, {}".format(date_format, time_format)
+                f"{date_format} {time_format}",
+                f"{date_format}, {time_format}",
             ]
     return _standard_datetime_format_CACHE
 
 
 def parse(datetime_str):
     """
     parses nepali datetime
     eg. parse('2078-10-12') => <NepaliDateTime: 2078-10-12>
     """
     standard_formats = _get_standard_formats()
-    nepalidatetime_object = None
     for format in standard_formats:
-        nepalidatetime_object = validate(datetime_str, format=format)
-        if nepalidatetime_object is not None:
-            return nepalidatetime_object
+        try:
+            return strptime(datetime_str, format=format)
+        except FormatNotMatchException:
+            pass
 
     raise InvalidDateTimeFormatException("Invalid format to parse nepali datetime.")
```

### Comparing `nepali-1.0.1/nepali/datetime/parser/validators.py` & `nepali-1.1.0/nepali/datetime/parser/validators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 validates parsing
 """
 import re
+from typing import Optional, Tuple
 
 from nepali.char import nepali_to_english_text
+from nepali.constants import NEPALI_MONTHS_EN, WEEKS_ABBR_EN, WEEKS_EN
 from nepali.datetime import nepalidatetime, nepalimonth, nepaliweek
-from nepali.datetime.constants import MONTHS_EN, WEEKS_EN, WEEKS_ABBR_EN
-
 
 __nepali_time_re__CACHE = None
 
 
 class NepaliTimeRE(dict):
     def __init__(self):
         """Create keys/values.
@@ -37,16 +37,16 @@
                 "-S": r"(?P<S>6[0-1]|[0-5]\d|\d)",  # same as "S"
                 "w": r"(?P<w>[0-6])",
                 "y": r"(?P<y>\d\d)",
                 "Y": r"(?P<Y>\d\d\d\d)",
                 "z": r"(?P<z>[+-]\d\d:?[0-5]\d(:?[0-5]\d(\.\d{1,6})?)?|(?-i:Z))",
                 "A": self.__seqToRE(WEEKS_EN, "A"),
                 "a": self.__seqToRE(WEEKS_ABBR_EN, "a"),
-                "B": self.__seqToRE(MONTHS_EN, "B"),
-                "b": self.__seqToRE(MONTHS_EN, "b"),
+                "B": self.__seqToRE(NEPALI_MONTHS_EN, "B"),
+                "b": self.__seqToRE(NEPALI_MONTHS_EN, "b"),
                 "p": self.__seqToRE(
                     (
                         "AM",
                         "PM",
                     ),
                     "p",
                 ),
@@ -64,47 +64,50 @@
         to_convert = sorted(to_convert, key=len, reverse=True)
         for value in to_convert:
             if value != "":
                 break
         else:
             return ""
         regex = "|".join(re.escape(stuff) for stuff in to_convert)
-        regex = "(?P<%s>%s" % (directive, regex)
-        return "%s)" % regex
+        regex = f"(?P<{directive}>{regex}"
+        return f"{regex})"
 
-    def pattern(self, format):
+    def pattern(self, date_format):
         """
-        Handle conversion from format directives to regexes.
+        Handle conversion from format directives to regex.
         """
         processed_format = ""
         regex_chars = re.compile(r"([\\.^$*+?\(\){}\[\]|])")
-        format = regex_chars.sub(r"\\\1", format)
+        date_format = regex_chars.sub(r"\\\1", date_format)
         whitespace_replacement = re.compile(r"\s+")
-        format = whitespace_replacement.sub(r"\\s+", format)
-        while "%" in format:
-            directive_index = format.index("%") + 1
+        date_format = whitespace_replacement.sub(r"\\s+", date_format)
+        while "%" in date_format:
+            directive_index = date_format.index("%") + 1
             index_increment = 1
 
-            if format[directive_index] == "-":
+            if date_format[directive_index] == "-":
                 index_increment = 2
 
-            if format[directive_index : directive_index + index_increment] not in self:
+            if (
+                date_format[directive_index : directive_index + index_increment]
+                not in self
+            ):
                 return None
 
             processed_format = "%s%s%s" % (
                 processed_format,
-                format[: directive_index - 1],
-                self[format[directive_index : directive_index + index_increment]],
+                date_format[: directive_index - 1],
+                self[date_format[directive_index : directive_index + index_increment]],
             )
-            format = format[directive_index + index_increment :]
-        return "^%s%s$" % (processed_format, format)
+            date_format = date_format[directive_index + index_increment :]
+        return f"^{processed_format}{date_format}$"
 
-    def compile(self, format):
+    def compile(self, date_format):
         """Return a compiled re object for the format string."""
-        return re.compile(self.pattern(format), re.IGNORECASE)
+        return re.compile(self.pattern(date_format), re.IGNORECASE)
 
 
 def get_nepali_time_re_object():
     global __nepali_time_re__CACHE
     if __nepali_time_re__CACHE is None:
         __nepali_time_re__CACHE = NepaliTimeRE()
     return __nepali_time_re__CACHE
@@ -127,21 +130,152 @@
         "d": 12,
     }
     """
 
     # converting datetime_str to english if any exists
     datetime_str = nepali_to_english_text(datetime_str)
 
-    re_compiled_format = get_nepali_time_re_object().compile(format=format)
+    re_compiled_format = get_nepali_time_re_object().compile(format)
     match = re_compiled_format.match(datetime_str)
     if match is None:
         return {}
     return match.groupdict()
 
 
+def __convert_12_hour_to_24_hour(hour: int, am_pm: str) -> int:
+    """Converts hours from 12-hour format to 24-hour format.
+
+    :param hour: The hour value to convert.
+    :param am_pm: Either "am" or "pm"; signifies whether the hour is in am or pm.
+
+    :returns: The value of `hour` converted to 24-hour format.
+    """
+    am_pm = am_pm.lower()
+    if am_pm == "am" and hour == 12:
+        return 0
+    elif am_pm == "pm" and hour != 12:
+        return hour + 12
+    return hour
+
+
+def __calculate_year(data: dict) -> Optional[int]:
+    """Calculates the year value from given data.
+
+    :param data: The dictionary of the format:
+                    {
+                        "Y": 2078,
+                        "b": "Mangsir",
+                        "d": 12,
+                        ...
+                    }
+
+    :returns: The year value of given date data.
+    """
+    if "y" in data:
+        return int(data["y"]) + 2000
+    elif "Y" in data:
+        return int(data["Y"])
+    return None
+
+
+def __calculate_month(data: dict) -> nepalimonth:
+    """Calculates the month value from given data.
+
+    :param data: The dictionary of the format:
+                    {
+                        "Y": 2078,
+                        "b": "Mangsir",
+                        "d": 12,
+                        ...
+                    }
+
+    :returns: The month value of given date data.
+    """
+    if "m" in data:
+        return nepalimonth(int(data["m"]))
+    elif "b" in data:
+        return nepalimonth(data["b"])
+    elif "B" in data:
+        return nepalimonth(data["B"])
+    return nepalimonth(1)
+
+
+def __calculate_day(data: dict) -> int:
+    """Calculates the day value from given data.
+
+    :param data: The dictionary of the format:
+                    {
+                        "Y": 2078,
+                        "b": "Mangsir",
+                        "d": 12,
+                        ...
+                    }
+
+    :returns: The day value of given date data.
+    """
+    if "d" in data:
+        return int(data["d"])
+    return 1
+
+
+def __calculate_hour_minute_seconds(data: dict) -> Tuple[int, int, int, int]:
+    """Calculates hour, minutes, seconds and microseconds from given data.
+
+    :param data: The dictionary of the format:
+                    {
+                        "Y": 2078,
+                        "b": "Mangsir",
+                        "d": 12,
+                        "H": 12,
+                        "M": 12,
+                        "S": 12,
+                        "f": 12,
+                        ...
+                    }
+
+    :returns: A tuple of hour, minute, seconds and microseconds.
+    """
+    hour = minute = second = fraction = 0
+    if "H" in data:
+        hour = int(data["H"])
+    elif "I" in data:
+        am_pm = data.get("p", "").lower() or "am"
+        hour = __convert_12_hour_to_24_hour(hour=int(data["I"]), am_pm=am_pm)
+
+    if "M" in data:
+        minute = int(data["M"])
+
+    if "S" in data:
+        second = int(data["S"])
+
+    if "f" in data:
+        s = data["f"]
+        # Pad to always return microseconds.
+        s += "0" * (6 - len(s))
+        fraction = int(s)
+
+    return hour, minute, second, fraction
+
+
+def __calculate_weekday(data: dict) -> Optional[nepaliweek]:
+    """Calculates the weekday of the date given in data.
+
+    :param data: The data that describes the date.
+
+    :returns: The weekday value; 0 for Sunday, 1 for Monday, etc.
+    """
+    if "a" in data:
+        return nepaliweek(data["a"])
+    elif "A" in data:
+        return nepaliweek(data["A"])
+    elif "w" in data:
+        return nepaliweek((int(data["w"]) - 1) % 7)
+    return None
+
+
 def transform(data: dict):
     """
     transforms different format data to uniform data
 
     eg.
     INPUT:
     data = {
@@ -156,70 +290,20 @@
         "year": 2078,
         "month": 8,
         "day": 12,
         ...
     }
     """
 
-    year = None
-    month = day = 1
-    hour = minute = second = fraction = 0
-    weekday = None
+    year = __calculate_year(data)
+    month = __calculate_month(data)
+    day = __calculate_day(data)
+    hour, minute, second, fraction = __calculate_hour_minute_seconds(data)
+    weekday = __calculate_weekday(data)
 
-    for date_key in data.keys():
-        if date_key == "y":
-            year = int(data["y"])
-            year += 2000
-        elif date_key == "Y":
-            year = int(data["Y"])
-        elif date_key == "m":
-            month = int(data["m"])
-        elif date_key == "B":
-            month = nepalimonth(data["B"])
-        elif date_key == "b":
-            month = nepalimonth(data["b"])
-        elif date_key == "d":
-            day = int(data["d"])
-        elif date_key == "H":
-            hour = int(data["H"])
-        elif date_key == "I":
-            hour = int(data["I"])
-            ampm = data.get("p", "").lower()
-            # If there was no AM/PM indicator, we'll treat this like AM
-            if ampm in ("", "am"):
-                # We're in AM so the hour is correct unless we're
-                # looking at 12 midnight.
-                # 12 midnight == 12 AM == hour 0
-                if hour == 12:
-                    hour = 0
-            elif ampm == "pm":
-                # We're in PM so we need to add 12 to the hour unless
-                # we're looking at 12 noon.
-                # 12 noon == 12 PM == hour 12
-                if hour != 12:
-                    hour += 12
-        elif date_key == "M":
-            minute = int(data["M"])
-        elif date_key == "S":
-            second = int(data["S"])
-        elif date_key == "f":
-            s = data["f"]
-            # Pad to always return microseconds.
-            s += "0" * (6 - len(s))
-            fraction = int(s)
-        elif date_key == "A":
-            weekday = nepaliweek(data["A"])
-        elif date_key == "a":
-            weekday = nepaliweek(data["a"])
-        elif date_key == "w":
-            weekday = int(data["w"])
-            if weekday == 0:
-                weekday = 6
-            else:
-                weekday -= 1
     return {
         "year": year,
         "month": month,
         "day": day,
         "hour": hour,
         "minute": minute,
         "second": second,
@@ -235,15 +319,15 @@
     -
     -
     returns False if validation failed
     returns nepalidatetime object if validation success.
     """
 
     # 1. validate if format is correct.
-    if get_nepali_time_re_object().pattern(format=format) is None:
+    if get_nepali_time_re_object().pattern(format) is None:
         # regex pattern generation failed
         return None
 
     # 2. validate if parse result if not empty
     parsed_result = extract(datetime_str, format)
     if parsed_result.get("Y") is None and parsed_result.get("y") is None:
         # compilation failed or year included
```

### Comparing `nepali-1.0.1/nepali/datetime/utils.py` & `nepali-1.1.0/nepali/datetime/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 from typing import Any
+
 from nepali.exceptions import InvalidNepaliDateTimeObjectException
 
 from ._datetime import nepalidate, nepalidatetime
 
 
 def to_nepalidatetime(datetime_object: Any) -> nepalidatetime:
     """
```

### Comparing `nepali-1.0.1/nepali/locations/_data.py` & `nepali-1.1.0/nepali/locations/_data.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.1/nepali/locations/_locations.py` & `nepali-1.1.0/nepali/locations/_locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Tuple
 
-from .models import Province, District, Municipality, MunicipalityType
+from .models import District, Municipality, MunicipalityType, Province
 
 
 def _loadData() -> Tuple[List[Province], List[District], List[Municipality]]:
     from ._data import _location_data
 
     provinces = []
     districts = []
```

### Comparing `nepali-1.0.1/nepali/locations/models.py` & `nepali-1.1.0/nepali/locations/models.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.1/nepali/locations/utils.py` & `nepali-1.1.0/nepali/locations/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 from functools import partial
 
-from ._locations import provinces, districts, municipalities
-
+from ._locations import districts, municipalities, provinces
 
 __all__ = [
     "get_province",
     "get_district",
     "get_municipality",
 ]
```

### Comparing `nepali-1.0.1/nepali/number/_nepalinumber.py` & `nepali-1.1.0/nepali/number/_nepalinumber.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Contains the class for the nepalinumber feature
 """
 
 from typing import Any, Tuple, Type, Union
+
 from .utils import NP_NUMBERS, NP_NUMBERS_SET, english_to_nepali
 
 
 class nepalinumber:
     """
     Represents the nepali(devanagari) numbers and
     the features related to arithmetic operations
@@ -15,18 +16,31 @@
 
     def __init__(self, value: Any) -> None:
         """
         Constructor/Initializer
         """
         self.__value = self.__parse(value)
 
-    def _raise_parse_exception(self, obj, ex_class: Type[Exception] = ValueError):
-        raise ex_class(
+    def get_parse_exception(
+        self, obj: object, ex_class: Type[Exception] = ValueError
+    ) -> Exception:
+        """
+        Returns the exception object to be raised when the parse is failed.
+        The methods also sets a proper message to the exception class.
+
+        :param obj: Object that is failed during the parse
+        :type obj: object
+        :param ex_class: Exception class type to be returned, defaults to ValueError
+        :type ex_class: Type[Exception], optional
+        :return: Exception object to be raised
+        :rtype: Exception
+        """
+        return ex_class(
             f"could not convert {obj.__class__.__name__} to {self.__class__.__name__}: '{obj}'"
-        ) from None
+        )
 
     def __parse(self, value: Any) -> Union[int, float]:
         """
         Parses nepali number input into a valid value.
 
         Eg:
         >>> self.__parse("१२")
@@ -57,40 +71,40 @@
     def __parse_str(self, value: str) -> Union[int, float]:
         """
         Parses str object into int and float.
         This is a low level implementation.
 
         :raises ValueError: If the value is invalid
         """
-        result = 0
+        result: float = 0
         sign = 1
         decimal_found = False
-        decimal_place = 1
+        decimal_place: float = 1
         i = 0
 
         # for negative sign
         if value[0] == "-":
             sign = -1
             i = 1
 
         while i < len(value):
             # decimal number found
             if value[i] == ".":
                 if decimal_found:
                     # decimal was already found
-                    self._raise_parse_exception(value)
+                    raise self.get_parse_exception(value) from None
                 decimal_found = True
                 i += 1
                 continue
 
             digit = ord(value[i]) - ord("0")
             if digit < 0 or digit > 9:
                 # checking nepali character
                 if value[i] not in NP_NUMBERS_SET:
-                    self._raise_parse_exception(value)
+                    raise self.get_parse_exception(value) from None
                 digit = NP_NUMBERS.index(value[i])
 
             if decimal_found:
                 decimal_place /= 10
                 result += digit * decimal_place
             else:
                 result = result * 10 + digit
@@ -109,15 +123,15 @@
                 return float(obj)
             elif hasattr(obj, "__int__"):
                 return int(obj)
 
             return self.__parse_str(str(obj))
         except (ValueError, TypeError):
             # object conversion must raise TypeError if fails
-            self._raise_parse_exception(obj, ex_class=TypeError)
+            raise self.get_parse_exception(obj, ex_class=TypeError) from None
 
     def __convert_or_return(self, obj) -> Union["nepalinumber", object]:
         """
         Will try to parse the given object and convert to nepalinumber
         else will return the same object
 
         :param obj: The object to convert
@@ -180,28 +194,28 @@
         return self.__value * other
 
     def __eq__(self, other) -> bool:
         """
         Checks if nepalinumber is equal to another object
 
         :param other: The other number/object which is to be checked for
-            equality againt nepalinumber
+            equality against nepalinumber
         :return: True if equal else False
         """
         if isinstance(other, nepalinumber):
             return self.__value == other.value
 
         return self.__value == other
 
     def __ne__(self, other) -> bool:
         """
         Checks if nepalinumber is not equal to another object
 
         :param other: The other number/object which is to be checked for
-            equality againt nepalinumber
+            equality against nepalinumber
         :return: True if not equal else False
         """
         if isinstance(other, nepalinumber):
             return self.__value != other.value
 
         return self.__value != other
 
@@ -345,15 +359,15 @@
 
     def __rtruediv__(self, other) -> Union["nepalinumber", object]:
         """
         Called when the division operator / is used before
         the nepalinumber object
 
         :param other: The other number/object that is to get
-            dividied by the value in the nepalinumber object
+            divided by the value in the nepalinumber object
         :raises TypeError: Raised when nepalinumber object is
             used to divide unsupported data types
         :return: Returns the quotient number as a nepalinumber
              object
         """
         try:
             if isinstance(other, nepalinumber):
@@ -384,15 +398,15 @@
 
     def __rfloordiv__(self, other) -> Union["nepalinumber", object]:
         """
         Called when the floor/integer division operator // is used
         before the nepalinumber object
 
         :param other: The other number/object that is to get
-            dividied by the value in the nepalinumber object
+            divided by the value in the nepalinumber object
         :raises TypeError: Raised when nepalinumber object is
             used to divide unsupported data types
         :return: Returns the quotient number as a nepalinumber
              object
         """
         try:
             if isinstance(other, nepalinumber):
```

### Comparing `nepali-1.0.1/nepali/number/_number.py` & `nepali-1.1.0/nepali/number/_number.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 import warnings
 
-from .utils import (
-    add_comma,
-    add_comma_english,
-    english_to_nepali,
-    nepali_to_english,
-)
+from .utils import add_comma, add_comma_english, english_to_nepali, nepali_to_english
 
 
 # Backward compatibility support for legacy NepaliNumber
 class NepaliNumber:
     @classmethod
     def convert_and_add_comma(cls, number):
         warnings.warn(
```

### Comparing `nepali-1.0.1/nepali/number/utils.py` & `nepali-1.1.0/nepali/number/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Any
 
-
 NP_NUMBERS = ["०", "१", "२", "३", "४", "५", "६", "७", "८", "९"]
 NP_NUMBERS_SET = set(NP_NUMBERS)
 
 
 def english_to_nepali(number: Any) -> str:
     """
     Converts english number to nepali.
@@ -35,15 +34,15 @@
 
 
 def add_comma_english(number: Any) -> str:
     """
     Adds comma in english style
     Eg. 123456789 => 123,456,789
     """
-    return "{:,}".format(int(number))
+    return f"{int(number):,}"
 
 
 def add_comma(number: Any, convert=False) -> str:
     """
     Adds comma in nepali style
     Eg. 123456789 => 12,34,56,789
```

### Comparing `nepali-1.0.1/nepali/phone_number.py` & `nepali-1.1.0/nepali/phone_number.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 from enum import Enum
 from typing import Union
 
-
-_mobile_number_re = re.compile(r"^(?:\+977|977)?(?:-)?(?:98|97|96)[0-9]{8}$")
+_mobile_number_re = re.compile(r"^(?:\+977|977)?(?:-)?(?:98|97|96)\d{8}$")
 _landline_number_re = re.compile(
-    r"^(?:\+977|977)?(?:-)?(?:0)?(?:[01][1-9]|2[13-9]|[3-9][0-9])[0-9]{6,7}$"
+    r"^(?:\+977|977)?(?:-)?(?:0)?(?:[01][1-9]|2[13-9]|[3-9]\d)\d{6,7}$"
 )
 
 
 class Operator(Enum):
     NEPAL_TELECOM = "Nepal Telecom"
     NCELL = "Ncell"
     SMART_CELL = "Smart Cell"
```

### Comparing `nepali-1.0.1/nepali/tests/test_date_converter.py` & `nepali-1.1.0/nepali/tests/test_date_converter.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.1/nepali/tests/test_datetime.py` & `nepali-1.1.0/nepali/tests/test_datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import unittest
 
-from nepali.datetime import nepalidate, nepalitime, nepalidatetime
-from nepali.datetime.utils import to_nepalidatetime, to_nepalidate
+from nepali.datetime import nepalidate, nepalidatetime, nepalitime
+from nepali.datetime.utils import to_nepalidate, to_nepalidatetime
 from nepali.exceptions import InvalidNepaliDateTimeObjectException
 from nepali.timezone import NepaliTimeZone
 
 
 class TestNepaliDateTime(unittest.TestCase):
     #
     # nepalidate
@@ -246,17 +246,15 @@
         nepalidatetime_obj2 = nepalidatetime(
             year=2051, month=4, day=29, hour=5, minute=28, second=23
         )
         nepalidatetime_obj1 = nepalidatetime_obj1 + datetime.timedelta(days=1)
         self.assertEqual(
             nepalidatetime_obj1,
             nepalidatetime_obj2,
-            msg="{} and {} are not equal".format(
-                nepalidatetime_obj1, nepalidatetime_obj2
-            ),
+            msg=f"{nepalidatetime_obj1} and {nepalidatetime_obj2} are not equal",
         )
 
 
 class TestDatetimeUtils(unittest.TestCase):
     # to_nepalidate
     def test_to_nepalidate_raises_exception_on_invalid_input(self):
         with self.assertRaises(InvalidNepaliDateTimeObjectException):
```

### Comparing `nepali-1.0.1/nepali/tests/test_humanize.py` & `nepali-1.1.0/nepali/tests/test_humanize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import datetime
 import unittest
 from unittest.mock import patch
 
-from nepali.datetime import nepalihumanize, HumanizeDateTime, nepalidate, nepalidatetime
+from nepali.datetime import HumanizeDateTime, nepalidate, nepalidatetime, nepalihumanize
 from nepali.exceptions import InvalidNepaliDateTimeObjectException
 from nepali.timezone import NepaliTimeZone
 
-
 REF_TIME = datetime.datetime(2015, 1, 1, 10, 15, tzinfo=NepaliTimeZone())
 
 
 @patch("nepali.datetime._humanize.now", return_value=REF_TIME)
 class TestNepaliHumanizeFunction(unittest.TestCase):
     def test_nepalihumanize_for_just_now(self, *_):
         humanize_str = nepalihumanize(REF_TIME)
```

### Comparing `nepali-1.0.1/nepali/tests/test_locations.py` & `nepali-1.1.0/nepali/tests/test_locations.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import unittest
 
 from nepali import locations
 from nepali.locations.models import (
+    District,
     Location,
+    Municipality,
     MunicipalityType,
     Province,
-    District,
-    Municipality,
 )
 from nepali.locations.utils import (
     _filter_location,
-    get_province,
     get_district,
     get_municipality,
+    get_province,
 )
 
 
 class TestLocations(unittest.TestCase):
     def test_locations_count(self):
         self.assertEqual(len(locations.provinces), 7)
         self.assertEqual(len(locations.districts), 77)
```

### Comparing `nepali-1.0.1/nepali/tests/test_nepalimonth.py` & `nepali-1.1.0/nepali/tests/test_nepalimonth.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.1/nepali/tests/test_nepaliweek.py` & `nepali-1.1.0/nepali/tests/test_nepaliweek.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.1/nepali/tests/test_number.py` & `nepali-1.1.0/nepali/tests/test_number.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
     python -m unittest nepali/tests/test_number.py -v
 """
 import sys
 import unittest
 
 from nepali import number
-from nepali.number import nepalinumber, NepaliNumber
+from nepali.number import NepaliNumber, nepalinumber
 
 
 class TestNumber(unittest.TestCase):
     def test_number_english_to_nepali(self):
         self.assertEqual(
             number.english_to_nepali("0123456789०१२३४५६७८९hello"),
             "०१२३४५६७८९०१२३४५६७८९hello",
@@ -166,15 +166,15 @@
     def test_nepalinumber_integer_is_addable_to_negative_float_to_give_negative_nepali_float(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_integer_10 + (-15.5), self.nepalinumber_negative_float_5_5
         )
 
-    def test_nepalinumber_integer_is_addable_to_postive_nepali_number_integer(self):
+    def test_nepalinumber_integer_is_addable_to_positive_nepali_number_integer(self):
         self.assertEqual(
             self.nepalinumber_integer_10 + self.nepalinumber_integer_10,
             self.nepalinumber_integer_20,
         )
 
     def test_nepalinumber_integer_is_addable_to_positive_nepali_number_float(self):
         self.assertEqual(
@@ -276,15 +276,15 @@
     def test_negative_nepalinumber_integer_is_addable_to_positive_float_to_give_positive_nepali_float(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_integer_10 + 15.5, self.nepalinumber_float_5_5
         )
 
-    def test_negative_nepalinumber_integer_is_addable_to_postive_nepali_number_integer(
+    def test_negative_nepalinumber_integer_is_addable_to_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_integer_10 + self.nepalinumber_integer_10,
             self.nepalinumber_zero,
         )
 
@@ -361,15 +361,15 @@
     def test_nepalinumber_float_is_addable_to_negative_float_to_give_negative_nepali_float(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_float_10_1 + (-15.6), self.nepalinumber_negative_float_5_5
         )
 
-    def test_nepalinumber_float_is_addable_to_postive_nepali_number_integer(self):
+    def test_nepalinumber_float_is_addable_to_positive_nepali_number_integer(self):
         self.assertEqual(
             self.nepalinumber_float_10_1 + self.nepalinumber_integer_10,
             self.nepalinumber_float_20_1,
         )
 
     def test_nepalinumber_float_is_addable_to_positive_nepali_number_float(self):
         self.assertEqual(
@@ -439,15 +439,15 @@
     def test_negative_nepalinumber_float_is_addable_to_positive_float_to_give_positive_nepali_float(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_10_1 + 15.6, self.nepalinumber_float_5_5
         )
 
-    def test_negative_nepalinumber_float_is_addable_to_postive_nepali_number_integer(
+    def test_negative_nepalinumber_float_is_addable_to_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_10_1 + self.nepalinumber_integer_10,
             self.nepalinumber_negative_float_0_0_9,
         )
 
@@ -538,15 +538,15 @@
         )
 
     def test_nepalinumber_integer_is_subtractable_by_negative_float(self):
         self.assertEqual(
             self.nepalinumber_integer_10 - (-5.5), self.nepalinumber_float_15_5
         )
 
-    def test_nepalinumber_integer_is_subtractable_by_postive_nepali_number_integer(
+    def test_nepalinumber_integer_is_subtractable_by_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_integer_10 - self.nepalinumber_integer_10,
             self.nepalinumber_zero,
         )
 
@@ -625,15 +625,15 @@
     def test_negative_nepalinumber_integer_is_subtractable_by_negative_float_to_give_positive_nepali_float(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_integer_10 - (-15.5), self.nepalinumber_float_5_5
         )
 
-    def test_negative_nepalinumber_integer_is_subtractable_by_postive_nepali_number_integer(
+    def test_negative_nepalinumber_integer_is_subtractable_by_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_integer_10 - self.nepalinumber_integer_10,
             self.nepalinumber_negative_float_20_0,
         )
 
@@ -696,15 +696,15 @@
         )
 
     def test_nepalinumber_float_is_subtractable_by_negative_float(self):
         self.assertEqual(
             self.nepalinumber_float_10_1 - (-5.4), self.nepalinumber_float_15_5
         )
 
-    def test_nepalinumber_float_is_subtractable_by_postive_nepali_number_integer(self):
+    def test_nepalinumber_float_is_subtractable_by_positive_nepali_number_integer(self):
         self.assertEqual(
             self.nepalinumber_float_10_1 - self.nepalinumber_integer_10,
             self.nepalinumber_float_0_0_9,
         )
 
     def test_nepalinumber_float_is_subtractable_by_positive_nepali_number_float(self):
         self.assertEqual(
@@ -767,15 +767,15 @@
     def test_negative_nepalinumber_float_is_subtractable_by_negative_float_to_give_positive_nepali_float(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_10_1 - (-15.6), self.nepalinumber_float_5_5
         )
 
-    def test_negative_nepalinumber_float_is_subtractable_by_postive_nepali_number_integer(
+    def test_negative_nepalinumber_float_is_subtractable_by_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_10_1 - self.nepalinumber_integer_10,
             self.nepalinumber_negative_float_20_1,
         )
 
@@ -868,15 +868,15 @@
         )
 
     def test_nepalinumber_integer_is_multiplicable_to_negative_float(self):
         self.assertEqual(
             self.nepalinumber_integer_10 * (-1.5), self.nepalinumber_negative_integer_15
         )
 
-    def test_nepalinumber_integer_is_multiplicable_to_postive_nepali_number_integer(
+    def test_nepalinumber_integer_is_multiplicable_to_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_integer_10 * self.nepalinumber_integer_2,
             self.nepalinumber_integer_20,
         )
 
@@ -951,15 +951,15 @@
 
     def test_negative_nepalinumber_integer_is_multiplicable_to_negative_float(self):
         self.assertEqual(
             self.nepalinumber_negative_integer_10 * (-1.5),
             self.nepalinumber_integer_15,
         )
 
-    def test_negative_nepalinumber_integer_is_multiplicable_to_postive_nepali_number_integer(
+    def test_negative_nepalinumber_integer_is_multiplicable_to_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_integer_10 * self.nepalinumber_integer_2,
             self.nepalinumber_negative_integer_20,
         )
 
@@ -1004,15 +1004,17 @@
         )
 
     def test_nepalinumber_float_is_multiplicable_to_negative_float(self):
         self.assertEqual(
             self.nepalinumber_float_4_5 * (-2.2), self.nepalinumber_negative_float_9_9
         )
 
-    def test_nepalinumber_float_is_multiplicable_to_postive_nepali_number_integer(self):
+    def test_nepalinumber_float_is_multiplicable_to_positive_nepali_number_integer(
+        self,
+    ):
         self.assertEqual(
             self.nepalinumber_float_10_1 * self.nepalinumber_integer_2,
             self.nepalinumber_float_20_2,
         )
 
     def test_nepalinumber_float_is_multiplicable_to_positive_nepali_number_float(self):
         self.assertEqual(
@@ -1055,15 +1057,15 @@
 
     def test_negative_nepalinumber_float_is_multiplicable_to_negative_float(self):
         self.assertEqual(
             self.nepalinumber_negative_float_1_5 * (-3.5),
             self.nepalinumber_float_5_25,
         )
 
-    def test_negative_nepalinumber_float_is_multiplicable_to_postive_nepali_number_integer(
+    def test_negative_nepalinumber_float_is_multiplicable_to_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_10_1 * self.nepalinumber_integer_2,
             self.nepalinumber_negative_float_20_2,
         )
 
@@ -1071,15 +1073,15 @@
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_1_5 * self.nepalinumber_float_1_5,
             self.nepalinumber_negative_float_2_25,
         )
 
-    def test_negative_nepalinumber_float_is_mutliplicable_to_negative_nepali_number_integer(
+    def test_negative_nepalinumber_float_is_multiplicable_to_negative_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_10_1
             * self.nepalinumber_negative_integer_2,
             self.nepalinumber_float_20_2,
         )
@@ -1176,15 +1178,15 @@
         )
 
     def test_nepalinumber_integer_is_divisible_by_negative_float(self):
         self.assertEqual(
             self.nepalinumber_integer_10 / (-2.5), self.nepalinumber_negative_integer_4
         )
 
-    def test_nepalinumber_integer_is_divisible_by_postive_nepali_number_integer(self):
+    def test_nepalinumber_integer_is_divisible_by_positive_nepali_number_integer(self):
         self.assertEqual(
             self.nepalinumber_integer_20 / self.nepalinumber_integer_10,
             self.nepalinumber_integer_2,
         )
 
     def test_nepalinumber_integer_is_divisible_by_positive_nepali_number_float(self):
         self.assertEqual(
@@ -1272,15 +1274,15 @@
     def test_negative_nepalinumber_integer_is_divisible_by_negative_float_to_give_positive_nepali_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_integer_10 / -2.5, self.nepalinumber_integer_4
         )
 
-    def test_negative_nepalinumber_integer_is_divisible_by_postive_nepali_number_integer(
+    def test_negative_nepalinumber_integer_is_divisible_by_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_integer_20 / self.nepalinumber_integer_10,
             self.nepalinumber_negative_integer_2,
         )
 
@@ -1334,15 +1336,15 @@
         )
 
     def test_nepalinumber_float_is_divisible_by_negative_float(self):
         self.assertEqual(
             self.nepalinumber_float_20_2 / (-10.1), self.nepalinumber_negative_integer_2
         )
 
-    def test_nepalinumber_float_is_divisible_by_postive_nepali_number_integer(self):
+    def test_nepalinumber_float_is_divisible_by_positive_nepali_number_integer(self):
         self.assertEqual(
             self.nepalinumber_float_20_2 / self.nepalinumber_integer_2,
             self.nepalinumber_float_10_1,
         )
 
     def test_nepalinumber_float_is_divisible_by_positive_nepali_number_float(self):
         self.assertEqual(
@@ -1383,15 +1385,15 @@
 
     def test_negative_nepalinumber_float_is_divisible_by_negative_float(self):
         self.assertEqual(
             self.nepalinumber_negative_float_20_2 / (-10.1),
             self.nepalinumber_integer_2,
         )
 
-    def test_negative_nepalinumber_float_is_divisible_by_postive_nepali_number_integer(
+    def test_negative_nepalinumber_float_is_divisible_by_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_20_2 / self.nepalinumber_integer_2,
             self.nepalinumber_negative_float_10_1,
         )
 
@@ -1466,15 +1468,15 @@
 
     def test_nepalinumber_throws_error_when_divided_by_zero_nepalinumber(self):
         with self.assertRaises(ZeroDivisionError) as ze:
             _ = self.nepalinumber_integer_2 / self.nepalinumber_zero
 
         self.assertEqual(str(ze.exception), "division by zero")
 
-    # floor divison
+    # floor division
     # nepalinumber positive integer division tests
     def test_nepalinumber_integer_is_floor_divisible_by_positive_integer(self):
         self.assertEqual(
             self.nepalinumber_integer_20 // 2, self.nepalinumber_integer_10
         )
 
     def test_nepalinumber_integer_is_floor_divisible_by_positive_float(self):
@@ -1488,15 +1490,15 @@
         )
 
     def test_nepalinumber_integer_is_floor_divisible_by_negative_float(self):
         self.assertEqual(
             self.nepalinumber_integer_10 // (-2.5), self.nepalinumber_negative_integer_4
         )
 
-    def test_nepalinumber_integer_is_floor_divisible_by_postive_nepali_number_integer(
+    def test_nepalinumber_integer_is_floor_divisible_by_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_integer_20 // self.nepalinumber_integer_10,
             self.nepalinumber_integer_2,
         )
 
@@ -1596,15 +1598,15 @@
     def test_negative_nepalinumber_integer_is_floor_divisible_by_negative_float_to_give_positive_nepali_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_integer_10 // -2.5, self.nepalinumber_integer_4
         )
 
-    def test_negative_nepalinumber_integer_is_floor_divisible_by_postive_nepali_number_integer(
+    def test_negative_nepalinumber_integer_is_floor_divisible_by_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_integer_20 // self.nepalinumber_integer_10,
             self.nepalinumber_negative_integer_2,
         )
 
@@ -1661,15 +1663,15 @@
 
     def test_nepalinumber_float_is_floor_divisible_by_negative_float(self):
         self.assertEqual(
             self.nepalinumber_float_20_2 // (-10.1),
             self.nepalinumber_negative_integer_2,
         )
 
-    def test_nepalinumber_float_is_floor_divisible_by_postive_nepali_number_integer(
+    def test_nepalinumber_float_is_floor_divisible_by_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_float_20_2 // self.nepalinumber_integer_2,
             self.nepalinumber_integer_10,
         )
 
@@ -1718,15 +1720,15 @@
 
     def test_negative_nepalinumber_float_is_floor_divisible_by_negative_float(self):
         self.assertEqual(
             self.nepalinumber_negative_float_20_2 // (-10.1),
             self.nepalinumber_integer_2,
         )
 
-    def test_negative_nepalinumber_float_is_floor_divisible_by_postive_nepali_number_integer(
+    def test_negative_nepalinumber_float_is_floor_divisible_by_positive_nepali_number_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_20_2 // self.nepalinumber_integer_2,
             self.nepalinumber_negative_integer_11,
         )
 
@@ -1892,15 +1894,15 @@
         self,
     ):
         self.assertEqual(
             self.nepalinumber_integer_10 % self.nepalinumber_negative_integer_20,
             self.nepalinumber_negative_integer_10,
         )
 
-    def test_nepalinumber_integer_can_be_modulo_divided_by_negative_nepainumber_float(
+    def test_nepalinumber_integer_can_be_modulo_divided_by_negative_nepalinumber_float(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_integer_10 % self.nepalinumber_negative_float_15_5,
             self.nepalinumber_negative_float_5_5,
         )
 
@@ -1941,15 +1943,15 @@
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_integer_10 % self.nepalinumber_integer_20,
             self.nepalinumber_integer_10,
         )
 
-    def test_negative_nepalinumber_float_can_be_modulo_divided_by_positive_nepainumber_float(
+    def test_negative_nepalinumber_float_can_be_modulo_divided_by_positive_nepalinumber_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_15_5 % self.nepalinumber_integer_10,
             self.nepalinumber_float_4_5,
         )
 
@@ -1996,15 +1998,15 @@
     ):
         self.assertEqual(
             self.nepalinumber_negative_integer_10
             % self.nepalinumber_negative_integer_20,
             self.nepalinumber_negative_integer_10,
         )
 
-    def test_negative_nepalinumber_integer_can_be_modulo_divided_by_negative_nepainumber_float(
+    def test_negative_nepalinumber_integer_can_be_modulo_divided_by_negative_nepalinumber_float(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_integer_10
             % self.nepalinumber_negative_float_15_5,
             self.nepalinumber_negative_integer_10,
         )
@@ -2044,15 +2046,15 @@
         self,
     ):
         self.assertEqual(
             self.nepalinumber_float_4_5 % self.nepalinumber_negative_integer_10,
             self.nepalinumber_negative_float_5_5,
         )
 
-    def test_negative_nepalinumber_float_can_be_modulo_divided_by_negative_nepainumber_integer(
+    def test_negative_nepalinumber_float_can_be_modulo_divided_by_negative_nepalinumber_integer(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_15_5
             % self.nepalinumber_negative_integer_10,
             self.nepalinumber_negative_float_5_5,
         )
@@ -2092,15 +2094,15 @@
         self,
     ):
         self.assertEqual(
             self.nepalinumber_float_4_5 % self.nepalinumber_negative_integer_20,
             self.nepalinumber_negative_float_15_5,
         )
 
-    def test_nepalinumber_float_can_be_modulo_divided_by_negative_nepainumber_float(
+    def test_nepalinumber_float_can_be_modulo_divided_by_negative_nepalinumber_float(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_float_4_5 % self.nepalinumber_negative_float_15_5,
             self.nepalinumber_negative_integer_11,
         )
 
@@ -2144,15 +2146,15 @@
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_15_5 % self.nepalinumber_float_2_5,
             self.nepalinumber_integer_2,
         )
 
-    def test_negative_nepalinumber_float_can_be_modulo_divided_by_negative_nepalinumber_integer(
+    def test_negative_nepalinumber_float_can_be_modulo_divided_by_negative_nepalinumber_integer_2(
         self,
     ):
         self.assertEqual(
             self.nepalinumber_negative_float_4_5
             % self.nepalinumber_negative_integer_20,
             self.nepalinumber_negative_float_4_5,
         )
@@ -2286,15 +2288,15 @@
             divmod(self.nepalinumber_integer_10, self.nepalinumber_negative_float_5_5),
             (
                 self.nepalinumber_negative_integer_2,
                 self.nepalinumber_negative_integer_1,
             ),
         )
 
-    # divmod positive nepalinumber integer as divisior tests
+    # divmod positive nepalinumber integer as divisor tests
     def test_positive_integer_can_be_divmod_with_positive_nepalinumber_integer(self):
         self.assertEqual(
             divmod(10, self.nepalinumber_integer_2),
             (self.nepalinumber_integer_5, self.nepalinumber_zero),
         )
 
     def test_positive_float_can_be_divmod_with_positive_nepalinumber_integer(self):
@@ -2393,15 +2395,15 @@
             divmod(self.nepalinumber_float_4_5, -2.5),
             (
                 self.nepalinumber_negative_integer_2,
                 self.nepalinumber_negative_float_0_5,
             ),
         )
 
-    # divmod positive nepalinumber float as divisior tests
+    # divmod positive nepalinumber float as divisor tests
     def test_positive_integer_can_be_divmod_with_positive_nepalinumber_float(self):
         self.assertEqual(
             divmod(10, self.nepalinumber_float_2_5),
             (self.nepalinumber_integer_4, self.nepalinumber_zero),
         )
 
     def test_positive_float_can_be_divmod_with_positive_nepalinumber_float(self):
@@ -2481,15 +2483,15 @@
             divmod(
                 self.nepalinumber_negative_integer_10,
                 self.nepalinumber_negative_float_5_5,
             ),
             (self.nepalinumber_integer_1, self.nepalinumber_negative_float_4_5),
         )
 
-    # divmod negative nepalinumber integer as divisior tests
+    # divmod negative nepalinumber integer as divisor tests
     def test_positive_integer_can_be_divmod_with_negative_nepalinumber_integer(self):
         self.assertEqual(
             divmod(10, self.nepalinumber_negative_integer_2),
             (self.nepalinumber_negative_integer_5, self.nepalinumber_zero),
         )
 
     def test_positive_float_can_be_divmod_with_negative_nepalinumber_integer(self):
@@ -2553,15 +2555,15 @@
         self,
     ):
         self.assertEqual(
             divmod(self.nepalinumber_negative_float_4_5, -2.5),
             (self.nepalinumber_integer_1, self.nepalinumber_negative_integer_2),
         )
 
-    # divmod negative nepalinumber float as divisior tests
+    # divmod negative nepalinumber float as divisor tests
     def test_positive_integer_can_be_divmod_with_negative_nepalinumber_float(self):
         self.assertEqual(
             divmod(10, self.nepalinumber_negative_float_2_5),
             (self.nepalinumber_negative_integer_4, self.nepalinumber_zero),
         )
 
     def test_positive_float_can_be_divmod_with_negative_nepalinumber_float(self):
```

### Comparing `nepali-1.0.1/nepali/tests/test_parser.py` & `nepali-1.1.0/nepali/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.1/nepali/tests/test_phone_number.py` & `nepali-1.1.0/nepali/tests/test_phone_number.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import unittest
 from unittest import mock
 
 from nepali.phone_number import (
+    Operator,
     _get_area_code,
     _get_operator,
     _parse_landline_number,
     _parse_mobile_number,
-    is_mobile_number,
+    get_exact_number,
     is_landline_number,
+    is_mobile_number,
     is_valid,
-    get_exact_number,
     parse,
-    Operator,
 )
 
 
 class TestOperator(unittest.TestCase):
     def test_operator_with_invalid_data(self):
         with self.assertRaises(ValueError):
             Operator("Hello")
```

### Comparing `nepali-1.0.1/nepali/tests/test_timezone.py` & `nepali-1.1.0/nepali/tests/test_timezone.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 
     python -m unittest nepali/tests/test_timezone.py -v
 """
 import datetime
 import unittest
 from unittest.mock import patch
 
+from nepali.constants import NEPAL_TIMEZONE
 from nepali.timezone import (
     NepaliTimeZone,
+    get_timezone,
+    now,
     to_nepali_timezone,
     to_utc_timezone,
     utc_now,
-    now,
-    get_timezone,
 )
 
 
 class TestNepaliTimeZone(unittest.TestCase):
     def setUp(self):
         self.nepali_timezone = NepaliTimeZone()
         return super().setUp()
@@ -28,21 +29,21 @@
     def test_nepali_timezone_utcoffset(self):
         self.assertEqual(
             self.nepali_timezone.utcoffset(None),
             datetime.timedelta(hours=5, minutes=45),
         )
 
     def test_nepali_timezone_tzname(self):
-        self.assertEqual(self.nepali_timezone.tzname(None), "Asia/Kathmandu")
+        self.assertEqual(self.nepali_timezone.tzname(None), NEPAL_TIMEZONE)
 
     def test_nepali_timezone_str(self):
-        self.assertEqual(str(self.nepali_timezone), "Asia/Kathmandu")
+        self.assertEqual(str(self.nepali_timezone), NEPAL_TIMEZONE)
 
     def test_nepali_timezone_repr(self):
-        self.assertEqual(repr(self.nepali_timezone), "Asia/Kathmandu")
+        self.assertEqual(repr(self.nepali_timezone), NEPAL_TIMEZONE)
 
     def test_datetime_with_nepali_timezone(self):
         dt = datetime.datetime(2015, 10, 14, tzinfo=self.nepali_timezone)
         self.assertEqual(dt.tzinfo, self.nepali_timezone)
         self.assertEqual(dt.tzname(), self.nepali_timezone.tzname(dt))
         self.assertEqual(dt.utcoffset(), self.nepali_timezone.utcoffset(dt))
```

### Comparing `nepali-1.0.1/nepali/timezone.py` & `nepali-1.1.0/nepali/timezone.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import datetime
 from typing import Union
 
+from .constants import NEPAL_TIMEZONE
+
 
 class NepaliTimeZone(datetime.tzinfo):
     """
     NepaliTimeZone: "Asia/Kathmandu", +05:45
     """
 
     def utcoffset(self, dt):
         return self.dst(dt) + datetime.timedelta(hours=5, minutes=45)
 
     def dst(self, dt):
         return datetime.timedelta(0)
 
     def tzname(self, dt):
-        return "Asia/Kathmandu"
+        return NEPAL_TIMEZONE
 
     def __str__(self):
-        return "Asia/Kathmandu"
+        return NEPAL_TIMEZONE
 
     def __repr__(self):
-        return "Asia/Kathmandu"
+        return NEPAL_TIMEZONE
 
     def __eq__(self, o: object) -> bool:
         return isinstance(o, self.__class__)
 
 
 def get_timezone() -> Union[datetime.tzinfo, None]:
     """
```

### Comparing `nepali-1.0.1/nepali.egg-info/PKG-INFO` & `nepali-1.1.0/nepali.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: nepali
-Version: 1.0.1
+Version: 1.1.0
 Summary: nepalidatetime compatible with python's datetime feature. Converting nepali date to english, parsing nepali datetime, nepali timezone, and timedelta support in nepali datetime
 Home-page: https://github.com/opensource-nepal/py-nepali
 Author: opensource-nepal
 Author-email: aj3sshh@gmail.com, sugatbajracharya49@gmail.com
+License: MIT
+Project-URL: Source, https://github.com/opensource-nepal/py-nepali
+Project-URL: Changelog, https://github.com/opensource-nepal/py-nepali/blob/main/CHANGELOG.md
 Keywords: nepali date conversion,convert date,nepali date time,python convert date,parse nepali date time
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nepali
 
 [![PyPI version](https://badge.fury.io/py/nepali.svg)](https://badge.fury.io/py/nepali)
-[![CI status](https://github.com/opensource-nepal/py-nepali/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/opensource-nepal/py-nepali/actions)
+[![CI status](https://github.com/opensource-nepal/py-nepali/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/opensource-nepal/py-nepali/actions)
 [![Downloads](https://img.shields.io/pypi/dm/nepali.svg?maxAge=180)](https://pypi.org/project/nepali/)
-[![codecov](https://codecov.io/gh/opensource-nepal/py-nepali/branch/master/graph/badge.svg?token=PTUHYWCJ4I)](https://codecov.io/gh/opensource-nepal/py-nepali)
+[![codecov](https://codecov.io/gh/opensource-nepal/py-nepali/branch/main/graph/badge.svg?token=PTUHYWCJ4I)](https://codecov.io/gh/opensource-nepal/py-nepali)
 
 `nepali` is a python package containing features that will be useful for Nepali projects.
 
 The major feature of this package is nepalidatetime, which is compatible with python's datetime feature. It helps nepali date to english, parsing nepali datetime, nepali timezone, and timedelta support in nepali datetime.
 
 ## Example
 
@@ -307,15 +310,15 @@
 
 | Directive | Meaning                                                   | Example                        |
 | --------- | --------------------------------------------------------- | ------------------------------ |
 | `%A`      | Weekday as locale’s abbreviated name.                     | Sun, Mon, …, Sat (आइत, सोम, …) |
 | `%A`      | Weekday as locale’s full name.                            | Sunday, Monday, …, Saturday    |
 | `%d`      | Day of the month as a zero-padded decimal number.         | 01, 02, …, 31                  |
 | `%-d`     | Day of the month as a decimal number.                     | 1, 2, …, 31                    |
-| `%B`      | Month as locale’s full name.                              | Baishak, Jestha, …, Chaitra    |
+| `%B`      | Month as locale’s full name.                              | Baishakh, Jestha, …, Chaitra   |
 | `%m`      | Month as a zero-padded decimal number.                    | 01, 02, …, 12                  |
 | `%-m`     | Month as a decimal number.                                | 1, 2, …, 12                    |
 | `%y`      | Year without century as a zero-padded decimal number.     | 00, 01, …, 99                  |
 | `%Y`      | Year with century as a decimal number.                    | 2001, 2078, 2079, …, 2099      |
 | `%H`      | Hour (24-hour clock) as a zero-padded decimal number.     | 00, 01, …, 23                  |
 | `%-H`     | Hour (24-hour clock) as a decimal number.                 | 0, 1, 2, …, 23                 |
 | `%I`      | Hour (12-hour clock) as a zero-padded decimal number.     | 01, 02, …, 12                  |
@@ -443,91 +446,14 @@
 # Municipality
 get_municipality(name_nepali="विराटनगर")
 # Biratnagar Metropolitan City
 ```
 
 ---
 
-## For Django Template
-
-Add `'nepali'` to your `INSTALLED_APPS` setting.
-
-```python
-INSTALLED_APPS = [
-    ...
-    'nepali',
-    ...
-]
-```
-
-### nepalidatetime
-
-In your Template
-
-```python
-{% load nepalidatetime %}
-```
-
-#### nepalinow
-
-`nepalinow` renders the current Nepali date and time in 'en-US' locale (English).
-
-```python
-{% nepalinow %}
-```
-
-```python
-{% nepalinow '%Y-%m-%d' %}
-```
-
-#### nepalinow_ne
-
-`nepalinow_ne` renders the current Nepali date and time in 'ne' locale (Nepali).
-
-```python
-{% nepalinow_ne %}
-```
-
-#### nepalidate
-
-`nepalidate` renders the datetime object into nepali datetime format in 'en-US' locale (English).
-
-```python
-{{ datetime_obj|nepalidate:"%Y-%m-%d" }}
-```
-
-#### nepalidate_ne
-
-`nepalidate_ne` renders the datetime object into nepali datetime format in 'ne' locale (Nepali).
-
-```python
-{{ datetime_obj|nepalidate_ne:"%Y-%m-%d" }}
-```
-
-#### nepalihumanize
-
-`nepalihumanize` renders the datetime object to a human readable form for 'ne' locale (Nepali)
-
-```python
-{{ datetime_obj|nepalihumanize }}
-```
-
-### nepalinumber
-
-In your Template
-
-```python
-{% load nepalinumber %}
-```
-
-`nepalinumber` renders the english number into nepali format (devanagari)
-
-```python
-{{ forloop.counter|nepalinumber }}
-
-{{ 150|nepalinumber }}
-```
+## For Django
 
+We have created a new Django package called [django-nepali](https://github.com/opensource-nepal/django-nepali) to support `nepali` package. For more information, please visit [django-nepali](https://github.com/opensource-nepal/django-nepali).
 
 ## Contribution
 
 We appreciate feedback and contribution to this package. To get started please see our [contribution guide](CONTRIBUTION.md)
```

### Comparing `nepali-1.0.1/nepali.egg-info/SOURCES.txt` & `nepali-1.1.0/nepali.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 nepali/__init__.py
 nepali/char.py
+nepali/constants.py
 nepali/date_converter.py
 nepali/exceptions.py
 nepali/phone_number.py
 nepali/timezone.py
 nepali/utils.py
 nepali.egg-info/PKG-INFO
 nepali.egg-info/SOURCES.txt
@@ -14,15 +15,14 @@
 nepali.egg-info/top_level.txt
 nepali/datetime/__init__.py
 nepali/datetime/_datetime.py
 nepali/datetime/_formatter.py
 nepali/datetime/_humanize.py
 nepali/datetime/_nepalimonth.py
 nepali/datetime/_nepaliweek.py
-nepali/datetime/constants.py
 nepali/datetime/utils.py
 nepali/datetime/parser/__init__.py
 nepali/datetime/parser/_parser.py
 nepali/datetime/parser/validators.py
 nepali/locations/__init__.py
 nepali/locations/_data.py
 nepali/locations/_locations.py
```

### Comparing `nepali-1.0.1/setup.py` & `nepali-1.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,16 +12,20 @@
 
     python setup.py sdist bdist_wheel
     twine upload dist/*
 
 """
 import os
 import sys
+
 import setuptools
 
+GITHUB_URL = "https://github.com/opensource-nepal/py-nepali"
+CHANGELOG_URL = "https://github.com/opensource-nepal/py-nepali/blob/main/CHANGELOG.md"
+
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 if sys.argv[-1] == "publish":
     if os.system("pip3 freeze | grep twine"):
         print("twine not installed.\nUse `pip install twine`.\nExiting.")
@@ -30,32 +34,37 @@
     os.system("python3 setup.py sdist bdist_wheel")
     os.system("twine upload dist/*")
     sys.exit()
 
 
 setuptools.setup(
     name="nepali",
-    version="1.0.1",
+    version="1.1.0",
+    license="MIT",
     author="opensource-nepal",
     author_email="aj3sshh@gmail.com, sugatbajracharya49@gmail.com",
     description="nepalidatetime compatible with python's datetime feature. "
     "Converting nepali date to english, parsing nepali datetime, "
     "nepali timezone, and timedelta support in nepali datetime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
         "nepali date conversion",
         "convert date",
         "nepali date time",
         "python convert date",
         "parse nepali date time",
     ],
-    url="https://github.com/opensource-nepal/py-nepali",
-    packages=setuptools.find_packages(),
+    url=GITHUB_URL,
+    packages=setuptools.find_packages(exclude=["tests*"]),
     test_suite="nepali.tests",
     install_requires=[],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    project_urls={
+        "Source": GITHUB_URL,
+        "Changelog": CHANGELOG_URL,
+    },
 )
```

