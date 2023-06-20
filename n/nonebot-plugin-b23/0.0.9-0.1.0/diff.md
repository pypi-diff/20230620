# Comparing `tmp/nonebot-plugin-b23-0.0.9.tar.gz` & `tmp/nonebot-plugin-b23-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-b23-0.0.9.tar", last modified: Tue Jun 20 04:50:37 2023, max compression
+gzip compressed data, was "nonebot-plugin-b23-0.1.0.tar", last modified: Tue Jun 20 05:07:08 2023, max compression
```

## Comparing `nonebot-plugin-b23-0.0.9.tar` & `nonebot-plugin-b23-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:50:37.479389 nonebot-plugin-b23-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-20 04:50:24.000000 nonebot-plugin-b23-0.0.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-20 04:50:37.479389 nonebot-plugin-b23-0.0.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:50:37.479389 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-20 04:50:24.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-20 04:50:24.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:50:37.479389 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-20 04:50:37.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 04:50:37.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:50:37.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 04:50:37.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 04:50:37.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 04:50:37.479389 nonebot-plugin-b23-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-20 04:50:24.000000 nonebot-plugin-b23-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:07:08.121469 nonebot-plugin-b23-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-20 05:06:52.000000 nonebot-plugin-b23-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-20 05:07:08.121469 nonebot-plugin-b23-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:07:08.121469 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-20 05:06:52.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-20 05:06:52.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:07:08.121469 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-20 05:07:08.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-20 05:07:08.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:07:08.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 05:07:08.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 05:07:08.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-20 05:06:52.000000 nonebot-plugin-b23-0.1.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-20 05:07:08.121469 nonebot-plugin-b23-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-20 05:06:52.000000 nonebot-plugin-b23-0.1.0/setup.py
```

### Comparing `nonebot-plugin-b23-0.0.9/LICENSE.txt` & `nonebot-plugin-b23-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-b23-0.0.9/nonebot_plugin_b23/__init__.py` & `nonebot-plugin-b23-0.1.0/nonebot_plugin_b23/__init__.py`

 * *Files identical despite different names*

