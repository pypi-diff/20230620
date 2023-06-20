# Comparing `tmp/suanpan-sprt-0.5.8.tar.gz` & `tmp/suanpan-sprt-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/suanpan-sprt-0.5.8.tar", last modified: Tue Jun 20 09:53:52 2023, max compression
+gzip compressed data, was "dist/suanpan-sprt-0.5.9.tar", last modified: Tue Jun 20 09:56:04 2023, max compression
```

## Comparing `suanpan-sprt-0.5.8.tar` & `suanpan-sprt-0.5.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-20 09:53:52.000000 suanpan-sprt-0.5.8/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-20 09:53:52.000000 suanpan-sprt-0.5.8/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.8/README.md
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-06-20 09:53:52.000000 suanpan-sprt-0.5.8/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.8/setup.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-20 09:53:52.000000 suanpan-sprt-0.5.8/sprt/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.5.8/sprt/__init__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5251 2023-06-20 09:26:42.000000 suanpan-sprt-0.5.8/sprt/__main__.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.8/sprt/arguments.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1280 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.8/sprt/envs.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.8/sprt/exceptions.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4321 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.8/sprt/loader.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2069 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.8/sprt/log.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.8/sprt/master.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5353 2023-06-20 09:26:42.000000 suanpan-sprt-0.5.8/sprt/server.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6456 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.8/sprt/storage.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3448 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.8/sprt/testing.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.8/sprt/utils.py
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-06-20 09:53:51.000000 suanpan-sprt-0.5.8/sprt/version.py
-drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-20 09:53:52.000000 suanpan-sprt-0.5.8/suanpan_sprt.egg-info/
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-20 09:53:52.000000 suanpan-sprt-0.5.8/suanpan_sprt.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-06-20 09:53:52.000000 suanpan-sprt-0.5.8/suanpan_sprt.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-06-20 09:53:52.000000 suanpan-sprt-0.5.8/suanpan_sprt.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-06-20 09:53:52.000000 suanpan-sprt-0.5.8/suanpan_sprt.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-06-20 09:53:52.000000 suanpan-sprt-0.5.8/suanpan_sprt.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-06-20 09:53:52.000000 suanpan-sprt-0.5.8/suanpan_sprt.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      129 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.9/README.md
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       38 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1073 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.9/setup.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/sprt/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      100 2023-03-13 09:36:01.000000 suanpan-sprt-0.5.9/sprt/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5251 2023-06-20 09:26:42.000000 suanpan-sprt-0.5.9/sprt/__main__.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     8168 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.9/sprt/arguments.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1280 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.9/sprt/envs.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      242 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.9/sprt/exceptions.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     4321 2023-05-23 01:43:36.000000 suanpan-sprt-0.5.9/sprt/loader.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     2069 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.9/sprt/log.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      880 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.9/sprt/master.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     5353 2023-06-20 09:26:42.000000 suanpan-sprt-0.5.9/sprt/server.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     6456 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.9/sprt/storage.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     3448 2023-04-04 09:18:04.000000 suanpan-sprt-0.5.9/sprt/testing.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)     1290 2023-06-02 08:38:14.000000 suanpan-sprt-0.5.9/sprt/utils.py
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       22 2023-06-20 09:56:03.000000 suanpan-sprt-0.5.9/sprt/version.py
+drwxrwxr-x   0 gitlab-runner  (1003) gitlab-runner  (1003)        0 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      482 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      439 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        1 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)       70 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)      158 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1003) gitlab-runner  (1003)        5 2023-06-20 09:56:04.000000 suanpan-sprt-0.5.9/suanpan_sprt.egg-info/top_level.txt
```

### Comparing `suanpan-sprt-0.5.8/setup.py` & `suanpan-sprt-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.8/sprt/__main__.py` & `suanpan-sprt-0.5.9/sprt/__main__.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.8/sprt/arguments.py` & `suanpan-sprt-0.5.9/sprt/arguments.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.8/sprt/envs.py` & `suanpan-sprt-0.5.9/sprt/envs.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.8/sprt/loader.py` & `suanpan-sprt-0.5.9/sprt/loader.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.8/sprt/log.py` & `suanpan-sprt-0.5.9/sprt/log.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.8/sprt/master.py` & `suanpan-sprt-0.5.9/sprt/master.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.8/sprt/server.py` & `suanpan-sprt-0.5.9/sprt/server.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.8/sprt/storage.py` & `suanpan-sprt-0.5.9/sprt/storage.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.8/sprt/testing.py` & `suanpan-sprt-0.5.9/sprt/testing.py`

 * *Files identical despite different names*

### Comparing `suanpan-sprt-0.5.8/sprt/utils.py` & `suanpan-sprt-0.5.9/sprt/utils.py`

 * *Files identical despite different names*

