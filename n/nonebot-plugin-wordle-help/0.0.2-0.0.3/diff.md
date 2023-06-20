# Comparing `tmp/nonebot_plugin_wordle_help-0.0.2.tar.gz` & `tmp/nonebot_plugin_wordle_help-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_wordle_help-0.0.2.tar", last modified: Tue Jun  6 15:13:07 2023, max compression
+gzip compressed data, was "nonebot_plugin_wordle_help-0.0.3.tar", last modified: Tue Jun 20 13:30:57 2023, max compression
```

## Comparing `nonebot_plugin_wordle_help-0.0.2.tar` & `nonebot_plugin_wordle_help-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 15:13:07.661599 nonebot_plugin_wordle_help-0.0.2/
--rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_wordle_help-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      378 2023-06-06 15:13:07.659562 nonebot_plugin_wordle_help-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 15:13:07.650550 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help/
--rw-rw-rw-   0        0        0      804 2023-06-06 15:11:46.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help/__init__.py
--rw-rw-rw-   0        0        0   338729 2023-06-06 15:09:58.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help/data.json
--rw-rw-rw-   0        0        0     1980 2023-06-06 15:09:58.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help/handle.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:13:07.657559 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help.egg-info/
--rw-rw-rw-   0        0        0      378 2023-06-06 15:13:07.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-06-06 15:13:07.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 15:13:07.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-06 15:13:07.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-06 15:13:07.000000 nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 15:13:07.661599 nonebot_plugin_wordle_help-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      618 2023-06-06 15:13:00.000000 nonebot_plugin_wordle_help-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:30:57.283700 nonebot_plugin_wordle_help-0.0.3/
+-rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_wordle_help-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      378 2023-06-20 13:30:57.282699 nonebot_plugin_wordle_help-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 13:30:57.273700 nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help/
+-rw-rw-rw-   0        0        0      917 2023-06-20 13:28:36.000000 nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help/__init__.py
+-rw-rw-rw-   0        0        0   338729 2023-06-20 13:27:33.000000 nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help/data.json
+-rw-rw-rw-   0        0        0     1980 2023-06-20 13:27:33.000000 nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help/handle.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:30:57.280700 nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-06-20 13:30:57.000000 nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-20 13:30:57.000000 nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:30:57.000000 nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-20 13:30:57.000000 nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-20 13:30:57.000000 nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 13:30:57.283700 nonebot_plugin_wordle_help-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      618 2023-06-20 13:30:48.000000 nonebot_plugin_wordle_help-0.0.3/setup.py
```

### Comparing `nonebot_plugin_wordle_help-0.0.2/LICENSE` & `nonebot_plugin_wordle_help-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help/__init__.py` & `nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+import contextlib
+
 from nonebot import on_regex
-from nonebot.plugin import PluginMetadata
-from .handle import wordle_help
 
+from .handle import wordle_help
 
 # 注册正则表达式, 优先级为10, 阻断式, 处理函数为wordle_help.main
 on_regex(
     r'^(?=.*[a-zA-Z])(?=.*_)[a-zA-Z_]+(#(?=[a-zA-Z]+$)[a-zA-Z]*)?$',
     priority=10,
     block=True,
     handlers=[wordle_help.main]
 )
 
-
-__plugin_meta__ = PluginMetadata(
-    name="wordle_help",
-    description="wordle游戏小助手",
-    usage=r'^(?=.*[a-zA-Z])(?=.*_)[a-zA-Z_]+(#(?=[a-zA-Z]+$)[a-zA-Z]*)?$',
-    type="application",
-    homepage="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/wordle_help",
-    supported_adapters={"~onebot.v11"},
-    extra={
-        'author':   'Special-Week',
-        'version':  '0.0.1',
-        'priority': 10,
-    }
-)
+with contextlib.suppress(Exception):
+    from nonebot.plugin import PluginMetadata
+    __plugin_meta__ = PluginMetadata(
+        name="wordle_help",
+        description="wordle游戏小助手",
+        usage=r'^(?=.*[a-zA-Z])(?=.*_)[a-zA-Z_]+(#(?=[a-zA-Z]+$)[a-zA-Z]*)?$',
+        type="application",
+        homepage="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/wordle_help",
+        supported_adapters={"~onebot.v11"},
+        extra={
+            'author':   'Special-Week',
+            'version':  '0.0.1',
+            'priority': 10,
+        }
+    )
```

### Comparing `nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help/data.json` & `nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help/data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle_help-0.0.2/nonebot_plugin_wordle_help/handle.py` & `nonebot_plugin_wordle_help-0.0.3/nonebot_plugin_wordle_help/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_wordle_help-0.0.2/setup.py` & `nonebot_plugin_wordle_help-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 from setuptools import find_packages, setup
 name = 'nonebot_plugin_wordle_help'
 
 setup(
     name=name,
-    version='0.0.2',
+    version='0.0.3',
     author="Special-Week",
     author_email='2385612749@qq.com',
     description="wordle小游戏工具",
     python_requires=">=3.8.0",
     packages=find_packages(),
     long_description="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/wordle_help",
     url="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/wordle_help",
```

