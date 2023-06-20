# Comparing `tmp/nonebot-plugin-b23-0.0.8.tar.gz` & `tmp/nonebot-plugin-b23-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-b23-0.0.8.tar", last modified: Tue Jun 13 14:19:08 2023, max compression
+gzip compressed data, was "nonebot-plugin-b23-0.0.9.tar", last modified: Tue Jun 20 04:50:37 2023, max compression
```

## Comparing `nonebot-plugin-b23-0.0.8.tar` & `nonebot-plugin-b23-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:08.795253 nonebot-plugin-b23-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-13 14:18:52.000000 nonebot-plugin-b23-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 14:19:08.795253 nonebot-plugin-b23-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:08.795253 nonebot-plugin-b23-0.0.8/nonebot_plugin_b23/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-13 14:18:52.000000 nonebot-plugin-b23-0.0.8/nonebot_plugin_b23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-13 14:18:52.000000 nonebot-plugin-b23-0.0.8/nonebot_plugin_b23/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:08.795253 nonebot-plugin-b23-0.0.8/nonebot_plugin_b23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 14:19:08.000000 nonebot-plugin-b23-0.0.8/nonebot_plugin_b23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-13 14:19:08.000000 nonebot-plugin-b23-0.0.8/nonebot_plugin_b23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:19:08.000000 nonebot-plugin-b23-0.0.8/nonebot_plugin_b23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 14:19:08.000000 nonebot-plugin-b23-0.0.8/nonebot_plugin_b23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 14:19:08.000000 nonebot-plugin-b23-0.0.8/nonebot_plugin_b23.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 14:19:08.795253 nonebot-plugin-b23-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-13 14:18:52.000000 nonebot-plugin-b23-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:50:37.479389 nonebot-plugin-b23-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-20 04:50:24.000000 nonebot-plugin-b23-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-20 04:50:37.479389 nonebot-plugin-b23-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:50:37.479389 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-20 04:50:24.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-20 04:50:24.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:50:37.479389 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-20 04:50:37.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 04:50:37.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:50:37.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 04:50:37.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 04:50:37.000000 nonebot-plugin-b23-0.0.9/nonebot_plugin_b23.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 04:50:37.479389 nonebot-plugin-b23-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-20 04:50:24.000000 nonebot-plugin-b23-0.0.9/setup.py
```

### Comparing `nonebot-plugin-b23-0.0.8/LICENSE.txt` & `nonebot-plugin-b23-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-b23-0.0.8/nonebot_plugin_b23/__init__.py` & `nonebot-plugin-b23-0.0.9/nonebot_plugin_b23/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 __plugin_meta__ = PluginMetadata(
     name="B站热搜",
     description="获取B站热搜(移动端)",
     usage=(
         "发送指令获取B站热搜(移动端)\n"
         f"指令:{','.join(config.b23_commands)}"
     ),
+    type="application",
     homepage="https://github.com/eya46/nonebot_plugin_b23",
     config=Config,
     supported_adapters=None,
 )
 
 b23_command = on_command(
     "b站热搜",
```

### Comparing `nonebot-plugin-b23-0.0.8/setup.py` & `nonebot-plugin-b23-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="nonebot-plugin-b23",
-    version="0.0.8",
+    version="0.0.9",
     author="eya46",
     install_requires=[
         'httpx~=0.23.0',
         'nonebot2~=2.0.0',
         'pydantic~=1.10.4'
     ],
     author_email="eya46@qq.com",
```

