# Comparing `tmp/free-sample-api-0.1.0.tar.gz` & `tmp/free-sample-api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "free-sample-api-0.1.0.tar", last modified: Sun Jun 18 13:41:27 2023, max compression
+gzip compressed data, was "free-sample-api-0.1.1.tar", last modified: Tue Jun 20 09:31:23 2023, max compression
```

## Comparing `free-sample-api-0.1.0.tar` & `free-sample-api-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 mignot    (1000) mignot    (1000)        0 2023-06-18 13:41:27.745327 free-sample-api-0.1.0/
--rw-rw-r--   0 mignot    (1000) mignot    (1000)      225 2023-06-18 13:41:27.745327 free-sample-api-0.1.0/PKG-INFO
-drwxrwxr-x   0 mignot    (1000) mignot    (1000)        0 2023-06-18 13:41:27.745327 free-sample-api-0.1.0/free_sample_api/
--rw-rw-r--   0 mignot    (1000) mignot    (1000)       21 2023-06-18 10:35:31.000000 free-sample-api-0.1.0/free_sample_api/__init__.py
--rw-r--r--   0 mignot    (1000) mignot    (1000)     1571 2023-06-18 08:21:56.000000 free-sample-api-0.1.0/free_sample_api/search.py
-drwxrwxr-x   0 mignot    (1000) mignot    (1000)        0 2023-06-18 13:41:27.745327 free-sample-api-0.1.0/free_sample_api.egg-info/
--rw-rw-r--   0 mignot    (1000) mignot    (1000)      225 2023-06-18 13:41:27.000000 free-sample-api-0.1.0/free_sample_api.egg-info/PKG-INFO
--rw-rw-r--   0 mignot    (1000) mignot    (1000)      218 2023-06-18 13:41:27.000000 free-sample-api-0.1.0/free_sample_api.egg-info/SOURCES.txt
--rw-rw-r--   0 mignot    (1000) mignot    (1000)        1 2023-06-18 13:41:27.000000 free-sample-api-0.1.0/free_sample_api.egg-info/dependency_links.txt
--rw-rw-r--   0 mignot    (1000) mignot    (1000)       16 2023-06-18 13:41:27.000000 free-sample-api-0.1.0/free_sample_api.egg-info/top_level.txt
--rw-rw-r--   0 mignot    (1000) mignot    (1000)       38 2023-06-18 13:41:27.745327 free-sample-api-0.1.0/setup.cfg
--rw-rw-r--   0 mignot    (1000) mignot    (1000)      358 2023-06-18 13:21:00.000000 free-sample-api-0.1.0/setup.py
+drwxrwxr-x   0 mignot    (1000) mignot    (1000)        0 2023-06-20 09:31:23.029834 free-sample-api-0.1.1/
+-rw-rw-r--   0 mignot    (1000) mignot    (1000)      225 2023-06-20 09:31:23.029834 free-sample-api-0.1.1/PKG-INFO
+drwxrwxr-x   0 mignot    (1000) mignot    (1000)        0 2023-06-20 09:31:23.029834 free-sample-api-0.1.1/free_sample_api/
+-rw-rw-r--   0 mignot    (1000) mignot    (1000)       21 2023-06-18 10:35:31.000000 free-sample-api-0.1.1/free_sample_api/__init__.py
+-rw-r--r--   0 mignot    (1000) mignot    (1000)     1883 2023-06-20 09:29:03.000000 free-sample-api-0.1.1/free_sample_api/search.py
+drwxrwxr-x   0 mignot    (1000) mignot    (1000)        0 2023-06-20 09:31:23.029834 free-sample-api-0.1.1/free_sample_api.egg-info/
+-rw-rw-r--   0 mignot    (1000) mignot    (1000)      225 2023-06-20 09:31:22.000000 free-sample-api-0.1.1/free_sample_api.egg-info/PKG-INFO
+-rw-rw-r--   0 mignot    (1000) mignot    (1000)      218 2023-06-20 09:31:22.000000 free-sample-api-0.1.1/free_sample_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 mignot    (1000) mignot    (1000)        1 2023-06-20 09:31:22.000000 free-sample-api-0.1.1/free_sample_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 mignot    (1000) mignot    (1000)       16 2023-06-20 09:31:22.000000 free-sample-api-0.1.1/free_sample_api.egg-info/top_level.txt
+-rw-rw-r--   0 mignot    (1000) mignot    (1000)       38 2023-06-20 09:31:23.029834 free-sample-api-0.1.1/setup.cfg
+-rw-rw-r--   0 mignot    (1000) mignot    (1000)      358 2023-06-20 09:30:23.000000 free-sample-api-0.1.1/setup.py
```

