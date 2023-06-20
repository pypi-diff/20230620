# Comparing `tmp/kaya_module_sdk-1.3.tar.gz` & `tmp/kaya_module_sdk-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaya_module_sdk-1.3.tar", last modified: Sat Jun 17 03:45:04 2023, max compression
+gzip compressed data, was "kaya_module_sdk-1.4.tar", last modified: Tue Jun 20 19:37:50 2023, max compression
```

## Comparing `kaya_module_sdk-1.3.tar` & `kaya_module_sdk-1.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.466796 kaya_module_sdk-1.3/
--rw-r--r--   0 root         (0) root         (0)    11356 2023-06-12 21:13:44.000000 kaya_module_sdk-1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3401 2023-06-17 03:45:04.462796 kaya_module_sdk-1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2419 2023-06-16 23:11:50.000000 kaya_module_sdk-1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.442796 kaya_module_sdk-1.3/kaya_module_sdk/
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      705 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/sdk.py
--rwxr-xr-x   0 root         (0) root         (0)     4209 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.446796 kaya_module_sdk-1.3/kaya_module_sdk/src/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)      541 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.450796 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5148 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/_k_number.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_float.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_int.py
--rw-r--r--   0 root         (0) root         (0)     3590 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_list.py
--rw-r--r--   0 root         (0) root         (0)      491 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_string.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_time_series.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.450796 kaya_module_sdk-1.3/kaya_module_sdk/src/module/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1005 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/module/run.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/module/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.450796 kaya_module_sdk-1.3/kaya_module_sdk/src/testing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3847 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/testing/kit.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/testing/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.450796 kaya_module_sdk-1.3/kaya_module_sdk/tst/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.454796 kaya_module_sdk-1.3/kaya_module_sdk/tst/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1022 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/integration/test_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.454796 kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/test_module.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/test_sdk.py
--rw-r--r--   0 root         (0) root         (0)    10946 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/test_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.446796 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3401 2023-06-17 03:45:04.000000 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1700 2023-06-17 03:45:04.000000 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 03:45:04.000000 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-17 03:45:04.000000 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-17 03:45:04.000000 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 23:14:30.000000 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 03:45:04.466796 kaya_module_sdk-1.3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     4209 2023-06-16 22:37:50.000000 kaya_module_sdk-1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.454796 kaya_module_sdk-1.3/src/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 16:03:20.000000 kaya_module_sdk-1.3/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)      541 2023-06-05 05:47:56.000000 kaya_module_sdk-1.3/src/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.458796 kaya_module_sdk-1.3/src/data_types/
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 23:34:41.000000 kaya_module_sdk-1.3/src/data_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5148 2023-04-06 00:33:46.000000 kaya_module_sdk-1.3/src/data_types/_k_number.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-04-03 20:31:53.000000 kaya_module_sdk-1.3/src/data_types/k_float.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-04-03 20:31:45.000000 kaya_module_sdk-1.3/src/data_types/k_int.py
--rw-r--r--   0 root         (0) root         (0)     3590 2023-04-03 20:31:37.000000 kaya_module_sdk-1.3/src/data_types/k_list.py
--rw-r--r--   0 root         (0) root         (0)      491 2023-03-18 03:32:53.000000 kaya_module_sdk-1.3/src/data_types/k_string.py
--rw-r--r--   0 root         (0) root         (0)     1548 2023-03-18 03:13:25.000000 kaya_module_sdk-1.3/src/data_types/k_time_series.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.458796 kaya_module_sdk-1.3/src/module/
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 23:34:52.000000 kaya_module_sdk-1.3/src/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1005 2023-06-02 00:44:27.000000 kaya_module_sdk-1.3/src/module/run.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-09 16:25:01.000000 kaya_module_sdk-1.3/src/module/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.462796 kaya_module_sdk-1.3/src/testing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 16:58:36.000000 kaya_module_sdk-1.3/src/testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3847 2023-06-17 03:30:24.000000 kaya_module_sdk-1.3/src/testing/kit.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-06-17 03:30:31.000000 kaya_module_sdk-1.3/src/testing/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.462796 kaya_module_sdk-1.3/tst/
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 23:33:13.000000 kaya_module_sdk-1.3/tst/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.462796 kaya_module_sdk-1.3/tst/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 23:31:50.000000 kaya_module_sdk-1.3/tst/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1022 2023-06-16 23:12:35.000000 kaya_module_sdk-1.3/tst/integration/test_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.462796 kaya_module_sdk-1.3/tst/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 23:31:54.000000 kaya_module_sdk-1.3/tst/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-06-16 23:12:41.000000 kaya_module_sdk-1.3/tst/unit/test_module.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-06-16 23:12:55.000000 kaya_module_sdk-1.3/tst/unit/test_sdk.py
--rw-r--r--   0 root         (0) root         (0)    10946 2023-06-16 23:13:07.000000 kaya_module_sdk-1.3/tst/unit/test_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.703495 kaya_module_sdk-1.4/
+-rw-r--r--   0 root         (0) root         (0)    11356 2023-06-12 21:13:44.000000 kaya_module_sdk-1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-06-20 19:37:50.699495 kaya_module_sdk-1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-06-16 23:11:50.000000 kaya_module_sdk-1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.679495 kaya_module_sdk-1.4/kaya_module_sdk/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      705 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/sdk.py
+-rwxr-xr-x   0 root         (0) root         (0)     4209 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.683495 kaya_module_sdk-1.4/kaya_module_sdk/src/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      541 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.687495 kaya_module_sdk-1.4/kaya_module_sdk/src/data_types/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/data_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5148 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/data_types/_k_number.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/data_types/k_float.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/data_types/k_int.py
+-rw-r--r--   0 root         (0) root         (0)     3590 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/data_types/k_list.py
+-rw-r--r--   0 root         (0) root         (0)      491 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/data_types/k_string.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/data_types/k_time_series.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.687495 kaya_module_sdk-1.4/kaya_module_sdk/src/module/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/module/run.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/module/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.687495 kaya_module_sdk-1.4/kaya_module_sdk/src/testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/testing/kit.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/src/testing/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.687495 kaya_module_sdk-1.4/kaya_module_sdk/tst/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/tst/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.691495 kaya_module_sdk-1.4/kaya_module_sdk/tst/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/tst/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/tst/integration/test_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.691495 kaya_module_sdk-1.4/kaya_module_sdk/tst/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/tst/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/tst/unit/test_module.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/tst/unit/test_sdk.py
+-rw-r--r--   0 root         (0) root         (0)    10946 2023-06-20 19:37:48.000000 kaya_module_sdk-1.4/kaya_module_sdk/tst/unit/test_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.683495 kaya_module_sdk-1.4/kaya_module_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-06-20 19:37:50.000000 kaya_module_sdk-1.4/kaya_module_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-06-20 19:37:50.000000 kaya_module_sdk-1.4/kaya_module_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 19:37:50.000000 kaya_module_sdk-1.4/kaya_module_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-20 19:37:50.000000 kaya_module_sdk-1.4/kaya_module_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-20 19:37:50.000000 kaya_module_sdk-1.4/kaya_module_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 19:36:14.000000 kaya_module_sdk-1.4/kaya_module_sdk.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 19:37:50.703495 kaya_module_sdk-1.4/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     4209 2023-06-20 19:34:09.000000 kaya_module_sdk-1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.691495 kaya_module_sdk-1.4/src/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 16:03:20.000000 kaya_module_sdk-1.4/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      541 2023-06-05 05:47:56.000000 kaya_module_sdk-1.4/src/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.695495 kaya_module_sdk-1.4/src/data_types/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 23:34:41.000000 kaya_module_sdk-1.4/src/data_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5148 2023-04-06 00:33:46.000000 kaya_module_sdk-1.4/src/data_types/_k_number.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-03 20:31:53.000000 kaya_module_sdk-1.4/src/data_types/k_float.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-04-03 20:31:45.000000 kaya_module_sdk-1.4/src/data_types/k_int.py
+-rw-r--r--   0 root         (0) root         (0)     3590 2023-04-03 20:31:37.000000 kaya_module_sdk-1.4/src/data_types/k_list.py
+-rw-r--r--   0 root         (0) root         (0)      491 2023-03-18 03:32:53.000000 kaya_module_sdk-1.4/src/data_types/k_string.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-03-18 03:13:25.000000 kaya_module_sdk-1.4/src/data_types/k_time_series.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.695495 kaya_module_sdk-1.4/src/module/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 23:34:52.000000 kaya_module_sdk-1.4/src/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-06-02 00:44:27.000000 kaya_module_sdk-1.4/src/module/run.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-06-20 19:15:06.000000 kaya_module_sdk-1.4/src/module/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.695495 kaya_module_sdk-1.4/src/testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 16:58:36.000000 kaya_module_sdk-1.4/src/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-06-20 19:33:46.000000 kaya_module_sdk-1.4/src/testing/kit.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-06-17 03:30:31.000000 kaya_module_sdk-1.4/src/testing/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.699495 kaya_module_sdk-1.4/tst/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 23:33:13.000000 kaya_module_sdk-1.4/tst/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.699495 kaya_module_sdk-1.4/tst/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 23:31:50.000000 kaya_module_sdk-1.4/tst/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-06-16 23:12:35.000000 kaya_module_sdk-1.4/tst/integration/test_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 19:37:50.699495 kaya_module_sdk-1.4/tst/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 23:31:54.000000 kaya_module_sdk-1.4/tst/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-06-16 23:12:41.000000 kaya_module_sdk-1.4/tst/unit/test_module.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-06-16 23:12:55.000000 kaya_module_sdk-1.4/tst/unit/test_sdk.py
+-rw-r--r--   0 root         (0) root         (0)    10946 2023-06-16 23:13:07.000000 kaya_module_sdk-1.4/tst/unit/test_types.py
```

### Comparing `kaya_module_sdk-1.3/LICENSE` & `kaya_module_sdk-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/PKG-INFO` & `kaya_module_sdk-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaya_module_sdk
-Version: 1.3
+Version: 1.4
 Summary: Provides the user a way to create custom strategy modules.
 Home-page: https://kaya.wanolabs.com
 Download-URL: http://pypi.python.org/pypi/kaya-module-sdk
 Author: Del:Tango
 Author-email: alvearesolutions@gmail.com
 License: BSD
 Project-URL: Documentation, https://kaya.wanolabs.com.readthedocs.io/en/latest
```

### Comparing `kaya_module_sdk-1.3/README.md` & `kaya_module_sdk-1.4/README.md`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/sdk.py` & `kaya_module_sdk-1.4/kaya_module_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/setup.py` & `kaya_module_sdk-1.4/kaya_module_sdk/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 # TODO - Check type hints used or break compilation
 #MyPyCommand().run()
 
 add_package_dir_to_path()
 setup_info = dict(
     name='kaya_module_sdk',
-    version='1.3',
+    version='1.4',
     author='Del:Tango',
     author_email='alvearesolutions@gmail.com',
     url='https://kaya.wanolabs.com',
     download_url='http://pypi.python.org/pypi/kaya-module-sdk',
     project_urls={
         'Documentation': 'https://kaya.wanolabs.com.readthedocs.io/en/latest',
         'Source': 'https://github.com/WanoLabs/KayaModuleSDK',
```

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/src/config.py` & `kaya_module_sdk-1.4/kaya_module_sdk/src/config.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/_k_number.py` & `kaya_module_sdk-1.4/kaya_module_sdk/src/data_types/_k_number.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_list.py` & `kaya_module_sdk-1.4/kaya_module_sdk/src/data_types/k_list.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_time_series.py` & `kaya_module_sdk-1.4/kaya_module_sdk/src/data_types/k_time_series.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/src/module/run.py` & `kaya_module_sdk-1.4/kaya_module_sdk/src/module/run.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/src/module/template.py` & `kaya_module_sdk-1.4/kaya_module_sdk/src/module/template.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,30 +26,33 @@
         for cls_name, obj in inspect.getmembers(module):
             if inspect.isclass(obj) and issubclass(obj, Module) \
                     and obj != Module and cls_name != 'KayaStrategyModule':
                 subclass_instance = obj()
                 self.subclasses.append(subclass_instance)
         return self.subclasses
 
-    # TODO - Refactor - run unit and sanity tests
-    @pysnooper.snoop
-    def run_tests(self, *args: str):
-        results = {}
-        test_dir = os.path.dirname(
-            os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-        )
-
-        # TODO - Remove
-        print(f'[ DEBUG ]: Test dir - {test_dir }')
-
-        if 'unit' in args:
-            unit_tests = pytest.main(['-s', '-v', test_dir])
-            results.update({'unit-tests': unit_tests})
+    @abstractmethod
+    def main(self,) -> None:
+        pass
+
+# CODE DUMP
+
+    # TODO - DEPRECATED
+#   @pysnooper.snoop
+#   def run_tests(self, *args: str):
+#       results = {}
+#       test_dir = os.path.dirname(
+#           os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+#       )
+
+#       # TODO - Remove
+#       print(f'[ DEBUG ]: Test dir - {test_dir }')
+
+#       if 'unit' in args:
+#           unit_tests = pytest.main(['-s', '-v', test_dir])
+#           results.update({'unit-tests': unit_tests})
 #       if 'integration' in args:
 #           # TODO
 #           integration_tests =
 #           results.update({'integration-tests': integration_tests})
-        return result
+#       return result
 
-    @abstractmethod
-    def main(self,) -> None:
-        pass
```

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/src/testing/kit.py` & `kaya_module_sdk-1.4/kaya_module_sdk/src/testing/kit.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,21 +14,21 @@
     '''
     [ KayaIntegrationTests ]: Morty puts his custom strategy module integration
         tests into subclasses of KIT.
     '''
     integration_tests = []
     docker_container_id = str()
     docker_container = None
-    runner_host = 'http://127.0.0.1:80'
+    runner_host = 'http://127.0.0.1:8080'
 
 #   @pysnooper.snoop()
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.docker_container_id = kwargs.get('docker_container_id', str())
-        self.runer_host = kwargs.get('runner_host', 'http://127.0.0.1:80')
+        self.runer_host = kwargs.get('runner_host', 'http://127.0.0.1:8080')
         self.docker_client = docker.from_env()
         self.integration_tests = [
             method for method in dir(self) if callable(getattr(self, method))
             and not method.startswith('__') and method.startswith('test_')
         ]
 
     @classmethod
```

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/src/testing/run.py` & `kaya_module_sdk-1.4/kaya_module_sdk/src/testing/run.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/tst/integration/test_module.py` & `kaya_module_sdk-1.4/kaya_module_sdk/tst/integration/test_module.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/test_module.py` & `kaya_module_sdk-1.4/kaya_module_sdk/tst/unit/test_module.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/test_sdk.py` & `kaya_module_sdk-1.4/kaya_module_sdk/tst/unit/test_sdk.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/test_types.py` & `kaya_module_sdk-1.4/kaya_module_sdk/tst/unit/test_types.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk.egg-info/PKG-INFO` & `kaya_module_sdk-1.4/kaya_module_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaya-module-sdk
-Version: 1.3
+Version: 1.4
 Summary: Provides the user a way to create custom strategy modules.
 Home-page: https://kaya.wanolabs.com
 Download-URL: http://pypi.python.org/pypi/kaya-module-sdk
 Author: Del:Tango
 Author-email: alvearesolutions@gmail.com
 License: BSD
 Project-URL: Documentation, https://kaya.wanolabs.com.readthedocs.io/en/latest
```

### Comparing `kaya_module_sdk-1.3/kaya_module_sdk.egg-info/SOURCES.txt` & `kaya_module_sdk-1.4/kaya_module_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/setup.py` & `kaya_module_sdk-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 # TODO - Check type hints used or break compilation
 #MyPyCommand().run()
 
 add_package_dir_to_path()
 setup_info = dict(
     name='kaya_module_sdk',
-    version='1.3',
+    version='1.4',
     author='Del:Tango',
     author_email='alvearesolutions@gmail.com',
     url='https://kaya.wanolabs.com',
     download_url='http://pypi.python.org/pypi/kaya-module-sdk',
     project_urls={
         'Documentation': 'https://kaya.wanolabs.com.readthedocs.io/en/latest',
         'Source': 'https://github.com/WanoLabs/KayaModuleSDK',
```

### Comparing `kaya_module_sdk-1.3/src/config.py` & `kaya_module_sdk-1.4/src/config.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/src/data_types/_k_number.py` & `kaya_module_sdk-1.4/src/data_types/_k_number.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/src/data_types/k_list.py` & `kaya_module_sdk-1.4/src/data_types/k_list.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/src/data_types/k_time_series.py` & `kaya_module_sdk-1.4/src/data_types/k_time_series.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/src/module/run.py` & `kaya_module_sdk-1.4/src/module/run.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/src/module/template.py` & `kaya_module_sdk-1.4/src/module/template.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,30 +26,33 @@
         for cls_name, obj in inspect.getmembers(module):
             if inspect.isclass(obj) and issubclass(obj, Module) \
                     and obj != Module and cls_name != 'KayaStrategyModule':
                 subclass_instance = obj()
                 self.subclasses.append(subclass_instance)
         return self.subclasses
 
-    # TODO - Refactor - run unit and sanity tests
-    @pysnooper.snoop
-    def run_tests(self, *args: str):
-        results = {}
-        test_dir = os.path.dirname(
-            os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-        )
-
-        # TODO - Remove
-        print(f'[ DEBUG ]: Test dir - {test_dir }')
-
-        if 'unit' in args:
-            unit_tests = pytest.main(['-s', '-v', test_dir])
-            results.update({'unit-tests': unit_tests})
+    @abstractmethod
+    def main(self,) -> None:
+        pass
+
+# CODE DUMP
+
+    # TODO - DEPRECATED
+#   @pysnooper.snoop
+#   def run_tests(self, *args: str):
+#       results = {}
+#       test_dir = os.path.dirname(
+#           os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+#       )
+
+#       # TODO - Remove
+#       print(f'[ DEBUG ]: Test dir - {test_dir }')
+
+#       if 'unit' in args:
+#           unit_tests = pytest.main(['-s', '-v', test_dir])
+#           results.update({'unit-tests': unit_tests})
 #       if 'integration' in args:
 #           # TODO
 #           integration_tests =
 #           results.update({'integration-tests': integration_tests})
-        return result
+#       return result
 
-    @abstractmethod
-    def main(self,) -> None:
-        pass
```

### Comparing `kaya_module_sdk-1.3/src/testing/kit.py` & `kaya_module_sdk-1.4/src/testing/kit.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,21 +14,21 @@
     '''
     [ KayaIntegrationTests ]: Morty puts his custom strategy module integration
         tests into subclasses of KIT.
     '''
     integration_tests = []
     docker_container_id = str()
     docker_container = None
-    runner_host = 'http://127.0.0.1:80'
+    runner_host = 'http://127.0.0.1:8080'
 
 #   @pysnooper.snoop()
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.docker_container_id = kwargs.get('docker_container_id', str())
-        self.runer_host = kwargs.get('runner_host', 'http://127.0.0.1:80')
+        self.runer_host = kwargs.get('runner_host', 'http://127.0.0.1:8080')
         self.docker_client = docker.from_env()
         self.integration_tests = [
             method for method in dir(self) if callable(getattr(self, method))
             and not method.startswith('__') and method.startswith('test_')
         ]
 
     @classmethod
```

### Comparing `kaya_module_sdk-1.3/src/testing/run.py` & `kaya_module_sdk-1.4/src/testing/run.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/tst/integration/test_module.py` & `kaya_module_sdk-1.4/tst/integration/test_module.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/tst/unit/test_module.py` & `kaya_module_sdk-1.4/tst/unit/test_module.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/tst/unit/test_sdk.py` & `kaya_module_sdk-1.4/tst/unit/test_sdk.py`

 * *Files identical despite different names*

### Comparing `kaya_module_sdk-1.3/tst/unit/test_types.py` & `kaya_module_sdk-1.4/tst/unit/test_types.py`

 * *Files identical despite different names*

