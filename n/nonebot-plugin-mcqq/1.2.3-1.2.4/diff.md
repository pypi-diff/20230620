# Comparing `tmp/nonebot-plugin-mcqq-1.2.3.tar.gz` & `tmp/nonebot-plugin-mcqq-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcqq-1.2.3.tar", last modified: Sun Jun 18 16:42:22 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcqq-1.2.4.tar", last modified: Tue Jun 20 15:36:28 2023, max compression
```

## Comparing `nonebot-plugin-mcqq-1.2.3.tar` & `nonebot-plugin-mcqq-1.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:22.048681 nonebot-plugin-mcqq-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-18 16:42:14.000000 nonebot-plugin-mcqq-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-18 16:42:22.048681 nonebot-plugin-mcqq-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-18 16:42:14.000000 nonebot-plugin-mcqq-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:22.048681 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-18 16:42:14.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-18 16:42:14.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-18 16:42:14.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:42:22.048681 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-18 16:42:22.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-18 16:42:22.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:42:22.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-18 16:42:22.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 16:42:22.000000 nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 16:42:22.048681 nonebot-plugin-mcqq-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-18 16:42:14.000000 nonebot-plugin-mcqq-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:28.390237 nonebot-plugin-mcqq-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 15:36:22.000000 nonebot-plugin-mcqq-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-20 15:36:28.390237 nonebot-plugin-mcqq-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-20 15:36:22.000000 nonebot-plugin-mcqq-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:28.390237 nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-20 15:36:22.000000 nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-20 15:36:22.000000 nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-20 15:36:22.000000 nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:28.390237 nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-20 15:36:28.000000 nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 15:36:28.000000 nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:36:28.000000 nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 15:36:28.000000 nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 15:36:28.000000 nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:36:28.390237 nonebot-plugin-mcqq-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-20 15:36:22.000000 nonebot-plugin-mcqq-1.2.4/setup.py
```

### Comparing `nonebot-plugin-mcqq-1.2.3/LICENSE` & `nonebot-plugin-mcqq-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.3/PKG-INFO` & `nonebot-plugin-mcqq-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.2.3
+Version: 1.2.4
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.2.3/README.md` & `nonebot-plugin-mcqq-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/__init__.py` & `nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 __plugin_meta__ = PluginMetadata(
     name="MC_QQ",
     description="基于NoneBot的与Minecraft Server互通消息的插件",
     homepage="https://github.com/17TheWord/nonebot-plugin-mcqq",
     usage="在群聊发送消息即可同步至 Minecraft 服务器",
     config=Config,
     type="application",
-    supported_adapters=[
+    supported_adapters={
         "nonebot.adapters.onebot.v11"
-    ]
+    }
 )
 
 mc_qq = on_message(priority=2, rule=msg_rule)
 
 mc_qq_cmd = on_command("minecraft_command", aliases={"mcc"}, priority=1, rule=msg_rule, block=True)
 
 driver = get_driver()
```

### Comparing `nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/data_source.py` & `nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq/utils.py` & `nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.2.3/nonebot_plugin_mcqq.egg-info/PKG-INFO` & `nonebot-plugin-mcqq-1.2.4/nonebot_plugin_mcqq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.2.3
+Version: 1.2.4
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.2.3/setup.py` & `nonebot-plugin-mcqq-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcqq",
-    version="1.2.3",
+    version="1.2.4",
     author="17TheWord",
     author_email="17theword@gmail.com",
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通插件",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/17TheWord/nonebot-plugin-mcqq",
     packages=["nonebot_plugin_mcqq"],
```

