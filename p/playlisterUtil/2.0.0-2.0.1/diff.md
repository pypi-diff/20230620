# Comparing `tmp/playlisterUtil-2.0.0.tar.gz` & `tmp/playlisterUtil-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playlisterUtil-2.0.0.tar", last modified: Mon Jun 19 23:14:54 2023, max compression
+gzip compressed data, was "playlisterUtil-2.0.1.tar", last modified: Mon Jun 19 23:42:53 2023, max compression
```

## Comparing `playlisterUtil-2.0.0.tar` & `playlisterUtil-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 faded     (1000) faded     (1000)        0 2023-06-19 23:14:54.308367 playlisterUtil-2.0.0/
--rw-rw-r--   0 faded     (1000) faded     (1000)      139 2023-06-19 23:14:54.308367 playlisterUtil-2.0.0/PKG-INFO
-drwxrwxr-x   0 faded     (1000) faded     (1000)        0 2023-06-19 23:14:54.308367 playlisterUtil-2.0.0/playlisterUtil.egg-info/
--rw-rw-r--   0 faded     (1000) faded     (1000)      139 2023-06-19 23:14:54.000000 playlisterUtil-2.0.0/playlisterUtil.egg-info/PKG-INFO
--rw-rw-r--   0 faded     (1000) faded     (1000)      197 2023-06-19 23:14:54.000000 playlisterUtil-2.0.0/playlisterUtil.egg-info/SOURCES.txt
--rw-rw-r--   0 faded     (1000) faded     (1000)        1 2023-06-19 23:14:54.000000 playlisterUtil-2.0.0/playlisterUtil.egg-info/dependency_links.txt
--rw-rw-r--   0 faded     (1000) faded     (1000)       15 2023-06-19 23:14:54.000000 playlisterUtil-2.0.0/playlisterUtil.egg-info/requires.txt
--rw-rw-r--   0 faded     (1000) faded     (1000)        1 2023-06-19 23:14:54.000000 playlisterUtil-2.0.0/playlisterUtil.egg-info/top_level.txt
--rw-rw-r--   0 faded     (1000) faded     (1000)       38 2023-06-19 23:14:54.308367 playlisterUtil-2.0.0/setup.cfg
--rw-rw-r--   0 faded     (1000) faded     (1000)      186 2023-06-19 23:14:35.000000 playlisterUtil-2.0.0/setup.py
+drwxrwxr-x   0 faded     (1000) faded     (1000)        0 2023-06-19 23:42:53.827274 playlisterUtil-2.0.1/
+-rw-rw-r--   0 faded     (1000) faded     (1000)      139 2023-06-19 23:42:53.827274 playlisterUtil-2.0.1/PKG-INFO
+drwxrwxr-x   0 faded     (1000) faded     (1000)        0 2023-06-19 23:42:53.827274 playlisterUtil-2.0.1/playlisterUtil.egg-info/
+-rw-rw-r--   0 faded     (1000) faded     (1000)      139 2023-06-19 23:42:53.000000 playlisterUtil-2.0.1/playlisterUtil.egg-info/PKG-INFO
+-rw-rw-r--   0 faded     (1000) faded     (1000)      197 2023-06-19 23:42:53.000000 playlisterUtil-2.0.1/playlisterUtil.egg-info/SOURCES.txt
+-rw-rw-r--   0 faded     (1000) faded     (1000)        1 2023-06-19 23:42:53.000000 playlisterUtil-2.0.1/playlisterUtil.egg-info/dependency_links.txt
+-rw-rw-r--   0 faded     (1000) faded     (1000)       15 2023-06-19 23:42:53.000000 playlisterUtil-2.0.1/playlisterUtil.egg-info/requires.txt
+-rw-rw-r--   0 faded     (1000) faded     (1000)        1 2023-06-19 23:42:53.000000 playlisterUtil-2.0.1/playlisterUtil.egg-info/top_level.txt
+-rw-rw-r--   0 faded     (1000) faded     (1000)       38 2023-06-19 23:42:53.827274 playlisterUtil-2.0.1/setup.cfg
+-rw-rw-r--   0 faded     (1000) faded     (1000)      186 2023-06-19 23:42:49.000000 playlisterUtil-2.0.1/setup.py
```

