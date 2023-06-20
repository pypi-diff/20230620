# Comparing `tmp/nonebot_plugin_homo_mathematician-0.0.3.tar.gz` & `tmp/nonebot_plugin_homo_mathematician-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_homo_mathematician-0.0.3.tar", last modified: Tue Jun  6 15:13:58 2023, max compression
+gzip compressed data, was "nonebot_plugin_homo_mathematician-0.0.4.tar", last modified: Tue Jun 20 13:32:08 2023, max compression
```

## Comparing `nonebot_plugin_homo_mathematician-0.0.3.tar` & `nonebot_plugin_homo_mathematician-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 15:13:58.168439 nonebot_plugin_homo_mathematician-0.0.3/
--rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_homo_mathematician-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      434 2023-06-06 15:13:58.167438 nonebot_plugin_homo_mathematician-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 15:13:58.159432 nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician/
--rw-rw-rw-   0        0        0     1057 2023-06-06 15:11:06.000000 nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician/__init__.py
--rw-rw-rw-   0        0        0     3228 2023-06-06 15:09:57.000000 nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician/handle.py
--rw-rw-rw-   0        0        0    12647 2023-06-06 15:09:57.000000 nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:13:58.166437 nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician.egg-info/
--rw-rw-rw-   0        0        0      434 2023-06-06 15:13:57.000000 nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-06-06 15:13:58.000000 nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 15:13:57.000000 nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-06 15:13:57.000000 nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-06-06 15:13:57.000000 nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 15:13:58.168439 nonebot_plugin_homo_mathematician-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-06-06 15:13:48.000000 nonebot_plugin_homo_mathematician-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:32:08.647036 nonebot_plugin_homo_mathematician-0.0.4/
+-rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_homo_mathematician-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      434 2023-06-20 13:32:08.646037 nonebot_plugin_homo_mathematician-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 13:32:08.638035 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician/
+-rw-rw-rw-   0        0        0     1172 2023-06-20 13:29:27.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician/__init__.py
+-rw-rw-rw-   0        0        0     3228 2023-06-20 13:27:33.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician/handle.py
+-rw-rw-rw-   0        0        0    12647 2023-06-20 13:27:33.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:32:08.645036 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-06-20 13:32:08.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-06-20 13:32:08.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:32:08.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-20 13:32:08.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-06-20 13:32:08.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 13:32:08.647036 nonebot_plugin_homo_mathematician-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-06-20 13:31:57.000000 nonebot_plugin_homo_mathematician-0.0.4/setup.py
```

### Comparing `nonebot_plugin_homo_mathematician-0.0.3/LICENSE` & `nonebot_plugin_homo_mathematician-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician/__init__.py` & `nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+import contextlib
+
 from nonebot import on_command
-from nonebot.plugin import PluginMetadata
 
 from .handle import homo_number, lagrange_interpolation
 
-__plugin_meta__ = PluginMetadata(
-    name="homo_mathematician",
-    description="任何实数都用连续的114514通过加减乘除达成, 任给一组数据都能找出其内在规律(函数表达式)",
-    usage=r'命令头: {lag, 找规律}  / {homonumber, 臭数字}  eg: 找规律 1 2 3 4 5 6 7 114514 1919810  / homonumber 2749903559',
-    type="application",
-    homepage="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/homo_mathematician",
-    supported_adapters={"~onebot.v11"},
-    extra={
-        'author':   'Special-Week',
-        'version':  '0.0.2',
-        'priority': 10,
-    }
-)
+with contextlib.suppress(Exception):
+    from nonebot.plugin import PluginMetadata
+    __plugin_meta__ = PluginMetadata(
+        name="homo_mathematician",
+        description="任何实数都用连续的114514通过加减乘除达成, 任给一组数据都能找出其内在规律(函数表达式)",
+        usage=r'命令头: {lag, 找规律}  / {homonumber, 臭数字}  eg: 找规律 1 2 3 4 5 6 7 114514 1919810  / homonumber 2749903559',
+        type="application",
+        homepage="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/homo_mathematician",
+        supported_adapters={"~onebot.v11"},
+        extra={
+            'author':   'Special-Week',
+            'version':  '0.0.2',
+            'priority': 10,
+        }
+    )
 
 
 
 on_command(
     cmd = "homonumber", 
     block=True, 
     priority=10,
```

### Comparing `nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician/handle.py` & `nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_homo_mathematician-0.0.3/nonebot_plugin_homo_mathematician/utils.py` & `nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_homo_mathematician-0.0.3/setup.py` & `nonebot_plugin_homo_mathematician-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 from setuptools import find_packages, setup
 name = 'nonebot_plugin_homo_mathematician'
 
 setup(
     name=name,  
-    version='0.0.3',
+    version='0.0.4',
     author="Special-Week",
     author_email='2749903559@qq.com',
     description="encapsulate logger",
     python_requires=">=3.8.0",
     packages=find_packages(),
     long_description="任何实数都用连续的114514通过加减乘除达成, 任给一组数据都能找出其内在规律(函数表达式)",
     url="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/homo_mathematician",
```

