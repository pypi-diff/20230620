# Comparing `tmp/cp-version-testing-1.0.4.tar.gz` & `tmp/cp-version-testing-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cp-version-testing-1.0.4.tar", last modified: Tue Jun 20 10:35:27 2023, max compression
+gzip compressed data, was "cp-version-testing-1.0.5.tar", last modified: Tue Jun 20 10:48:45 2023, max compression
```

## Comparing `cp-version-testing-1.0.4.tar` & `cp-version-testing-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:35:27.163313 cp-version-testing-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 10:35:27.163313 cp-version-testing-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 10:35:18.000000 cp-version-testing-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:35:27.163313 cp-version-testing-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-20 10:35:18.000000 cp-version-testing-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:35:27.159313 cp-version-testing-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:35:27.159313 cp-version-testing-1.0.4/src/cp-version-testing/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 10:35:18.000000 cp-version-testing-1.0.4/src/cp-version-testing/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:35:27.163313 cp-version-testing-1.0.4/src/cp_version_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 10:35:27.000000 cp-version-testing-1.0.4/src/cp_version_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-20 10:35:27.000000 cp-version-testing-1.0.4/src/cp_version_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:35:27.000000 cp-version-testing-1.0.4/src/cp_version_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 10:35:27.000000 cp-version-testing-1.0.4/src/cp_version_testing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:48:45.573970 cp-version-testing-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 10:48:45.573970 cp-version-testing-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 10:48:34.000000 cp-version-testing-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:48:45.569970 cp-version-testing-1.0.5/cp_version_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 10:48:45.000000 cp-version-testing-1.0.5/cp_version_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-20 10:48:45.000000 cp-version-testing-1.0.5/cp_version_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:48:45.000000 cp-version-testing-1.0.5/cp_version_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-20 10:48:45.000000 cp-version-testing-1.0.5/cp_version_testing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:48:45.000000 cp-version-testing-1.0.5/cp_version_testing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:48:45.573970 cp-version-testing-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-20 10:48:34.000000 cp-version-testing-1.0.5/setup.py
```

