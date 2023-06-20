# Comparing `tmp/playlisterUtil-2.0.2.tar.gz` & `tmp/playlisterutil-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playlisterUtil-2.0.2.tar", last modified: Tue Jun 20 00:09:27 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `playlisterUtil-2.0.2.tar` & `playlisterutil-2.0.3.tar`

### file list

```diff
@@ -1,16 +1,8 @@
-drwxrwxr-x   0 faded     (1000) faded     (1000)        0 2023-06-20 00:09:27.338441 playlisterUtil-2.0.2/
--rw-rw-r--   0 faded     (1000) faded     (1000)     1074 2023-06-20 00:02:30.000000 playlisterUtil-2.0.2/LICENSE
--rw-rw-r--   0 faded     (1000) faded     (1000)      229 2023-06-20 00:09:27.338441 playlisterUtil-2.0.2/PKG-INFO
--rw-rw-r--   0 faded     (1000) faded     (1000)       10 2023-06-20 00:02:23.000000 playlisterUtil-2.0.2/README.md
-drwxrwxr-x   0 faded     (1000) faded     (1000)        0 2023-06-20 00:09:27.338441 playlisterUtil-2.0.2/playlisterUtil.egg-info/
--rw-rw-r--   0 faded     (1000) faded     (1000)      229 2023-06-20 00:09:27.000000 playlisterUtil-2.0.2/playlisterUtil.egg-info/PKG-INFO
--rw-rw-r--   0 faded     (1000) faded     (1000)      272 2023-06-20 00:09:27.000000 playlisterUtil-2.0.2/playlisterUtil.egg-info/SOURCES.txt
--rw-rw-r--   0 faded     (1000) faded     (1000)        1 2023-06-20 00:09:27.000000 playlisterUtil-2.0.2/playlisterUtil.egg-info/dependency_links.txt
--rw-rw-r--   0 faded     (1000) faded     (1000)       15 2023-06-20 00:09:27.000000 playlisterUtil-2.0.2/playlisterUtil.egg-info/requires.txt
--rw-rw-r--   0 faded     (1000) faded     (1000)        4 2023-06-20 00:09:27.000000 playlisterUtil-2.0.2/playlisterUtil.egg-info/top_level.txt
--rw-rw-r--   0 faded     (1000) faded     (1000)      127 2023-06-20 00:02:04.000000 playlisterUtil-2.0.2/pyproject.toml
--rw-rw-r--   0 faded     (1000) faded     (1000)       38 2023-06-20 00:09:27.338441 playlisterUtil-2.0.2/setup.cfg
-drwxrwxr-x   0 faded     (1000) faded     (1000)        0 2023-06-20 00:09:27.338441 playlisterUtil-2.0.2/src/
--rw-rw-r--   0 faded     (1000) faded     (1000)        0 2023-06-18 02:01:05.000000 playlisterUtil-2.0.2/src/__init__.py
--rw-rw-r--   0 faded     (1000) faded     (1000)     4745 2023-06-19 22:40:22.000000 playlisterUtil-2.0.2/src/playlisterUtil.py
--rw-rw-r--   0 faded     (1000) faded     (1000)      293 2023-06-19 23:56:25.000000 playlisterUtil-2.0.2/src/setup.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-2.0.3/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-2.0.3/src/__init__.py
+-rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 playlisterutil-2.0.3/src/playlisterUtil.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-2.0.3/src/setup.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-2.0.3/LICENSE
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-2.0.3/PKG-INFO
```

### Comparing `playlisterUtil-2.0.2/LICENSE` & `playlisterutil-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `playlisterUtil-2.0.2/src/playlisterUtil.py` & `playlisterutil-2.0.3/src/playlisterUtil.py`

 * *Files identical despite different names*

