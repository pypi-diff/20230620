# Comparing `tmp/playlisterUtil-2.0.1.tar.gz` & `tmp/playlisterUtil-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playlisterUtil-2.0.1.tar", last modified: Mon Jun 19 23:42:53 2023, max compression
+gzip compressed data, was "playlisterUtil-2.0.2.tar", last modified: Tue Jun 20 00:09:27 2023, max compression
```

## Comparing `playlisterUtil-2.0.1.tar` & `playlisterUtil-2.0.2.tar`

### file list

```diff
@@ -1,10 +1,16 @@
-drwxrwxr-x   0 faded     (1000) faded     (1000)        0 2023-06-19 23:42:53.827274 playlisterUtil-2.0.1/
--rw-rw-r--   0 faded     (1000) faded     (1000)      139 2023-06-19 23:42:53.827274 playlisterUtil-2.0.1/PKG-INFO
-drwxrwxr-x   0 faded     (1000) faded     (1000)        0 2023-06-19 23:42:53.827274 playlisterUtil-2.0.1/playlisterUtil.egg-info/
--rw-rw-r--   0 faded     (1000) faded     (1000)      139 2023-06-19 23:42:53.000000 playlisterUtil-2.0.1/playlisterUtil.egg-info/PKG-INFO
--rw-rw-r--   0 faded     (1000) faded     (1000)      197 2023-06-19 23:42:53.000000 playlisterUtil-2.0.1/playlisterUtil.egg-info/SOURCES.txt
--rw-rw-r--   0 faded     (1000) faded     (1000)        1 2023-06-19 23:42:53.000000 playlisterUtil-2.0.1/playlisterUtil.egg-info/dependency_links.txt
--rw-rw-r--   0 faded     (1000) faded     (1000)       15 2023-06-19 23:42:53.000000 playlisterUtil-2.0.1/playlisterUtil.egg-info/requires.txt
--rw-rw-r--   0 faded     (1000) faded     (1000)        1 2023-06-19 23:42:53.000000 playlisterUtil-2.0.1/playlisterUtil.egg-info/top_level.txt
--rw-rw-r--   0 faded     (1000) faded     (1000)       38 2023-06-19 23:42:53.827274 playlisterUtil-2.0.1/setup.cfg
--rw-rw-r--   0 faded     (1000) faded     (1000)      186 2023-06-19 23:42:49.000000 playlisterUtil-2.0.1/setup.py
+drwxrwxr-x   0 faded     (1000) faded     (1000)        0 2023-06-20 00:09:27.338441 playlisterUtil-2.0.2/
+-rw-rw-r--   0 faded     (1000) faded     (1000)     1074 2023-06-20 00:02:30.000000 playlisterUtil-2.0.2/LICENSE
+-rw-rw-r--   0 faded     (1000) faded     (1000)      229 2023-06-20 00:09:27.338441 playlisterUtil-2.0.2/PKG-INFO
+-rw-rw-r--   0 faded     (1000) faded     (1000)       10 2023-06-20 00:02:23.000000 playlisterUtil-2.0.2/README.md
+drwxrwxr-x   0 faded     (1000) faded     (1000)        0 2023-06-20 00:09:27.338441 playlisterUtil-2.0.2/playlisterUtil.egg-info/
+-rw-rw-r--   0 faded     (1000) faded     (1000)      229 2023-06-20 00:09:27.000000 playlisterUtil-2.0.2/playlisterUtil.egg-info/PKG-INFO
+-rw-rw-r--   0 faded     (1000) faded     (1000)      272 2023-06-20 00:09:27.000000 playlisterUtil-2.0.2/playlisterUtil.egg-info/SOURCES.txt
+-rw-rw-r--   0 faded     (1000) faded     (1000)        1 2023-06-20 00:09:27.000000 playlisterUtil-2.0.2/playlisterUtil.egg-info/dependency_links.txt
+-rw-rw-r--   0 faded     (1000) faded     (1000)       15 2023-06-20 00:09:27.000000 playlisterUtil-2.0.2/playlisterUtil.egg-info/requires.txt
+-rw-rw-r--   0 faded     (1000) faded     (1000)        4 2023-06-20 00:09:27.000000 playlisterUtil-2.0.2/playlisterUtil.egg-info/top_level.txt
+-rw-rw-r--   0 faded     (1000) faded     (1000)      127 2023-06-20 00:02:04.000000 playlisterUtil-2.0.2/pyproject.toml
+-rw-rw-r--   0 faded     (1000) faded     (1000)       38 2023-06-20 00:09:27.338441 playlisterUtil-2.0.2/setup.cfg
+drwxrwxr-x   0 faded     (1000) faded     (1000)        0 2023-06-20 00:09:27.338441 playlisterUtil-2.0.2/src/
+-rw-rw-r--   0 faded     (1000) faded     (1000)        0 2023-06-18 02:01:05.000000 playlisterUtil-2.0.2/src/__init__.py
+-rw-rw-r--   0 faded     (1000) faded     (1000)     4745 2023-06-19 22:40:22.000000 playlisterUtil-2.0.2/src/playlisterUtil.py
+-rw-rw-r--   0 faded     (1000) faded     (1000)      293 2023-06-19 23:56:25.000000 playlisterUtil-2.0.2/src/setup.py
```

