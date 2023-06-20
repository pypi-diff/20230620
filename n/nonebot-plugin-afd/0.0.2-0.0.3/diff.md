# Comparing `tmp/nonebot-plugin-afd-0.0.2.tar.gz` & `tmp/nonebot-plugin-afd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-afd-0.0.2.tar", last modified: Sun Jun 18 17:05:08 2023, max compression
+gzip compressed data, was "nonebot-plugin-afd-0.0.3.tar", last modified: Tue Jun 20 15:41:08 2023, max compression
```

## Comparing `nonebot-plugin-afd-0.0.2.tar` & `nonebot-plugin-afd-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:05:08.098715 nonebot-plugin-afd-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-18 17:04:58.000000 nonebot-plugin-afd-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-18 17:05:08.098715 nonebot-plugin-afd-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-18 17:04:58.000000 nonebot-plugin-afd-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:05:08.098715 nonebot-plugin-afd-0.0.2/nonebot_plugin_afd/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-18 17:04:58.000000 nonebot-plugin-afd-0.0.2/nonebot_plugin_afd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-18 17:04:58.000000 nonebot-plugin-afd-0.0.2/nonebot_plugin_afd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-18 17:04:58.000000 nonebot-plugin-afd-0.0.2/nonebot_plugin_afd/group_new_member.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:05:08.098715 nonebot-plugin-afd-0.0.2/nonebot_plugin_afd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-18 17:05:08.000000 nonebot-plugin-afd-0.0.2/nonebot_plugin_afd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-18 17:05:08.000000 nonebot-plugin-afd-0.0.2/nonebot_plugin_afd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:05:08.000000 nonebot-plugin-afd-0.0.2/nonebot_plugin_afd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-18 17:05:08.000000 nonebot-plugin-afd-0.0.2/nonebot_plugin_afd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 17:05:08.000000 nonebot-plugin-afd-0.0.2/nonebot_plugin_afd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 17:05:08.098715 nonebot-plugin-afd-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-18 17:04:58.000000 nonebot-plugin-afd-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:41:08.597215 nonebot-plugin-afd-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 15:40:56.000000 nonebot-plugin-afd-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-20 15:41:08.597215 nonebot-plugin-afd-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-20 15:40:56.000000 nonebot-plugin-afd-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:41:08.593215 nonebot-plugin-afd-0.0.3/nonebot_plugin_afd/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 15:40:56.000000 nonebot-plugin-afd-0.0.3/nonebot_plugin_afd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-20 15:40:56.000000 nonebot-plugin-afd-0.0.3/nonebot_plugin_afd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-20 15:40:56.000000 nonebot-plugin-afd-0.0.3/nonebot_plugin_afd/group_new_member.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:41:08.593215 nonebot-plugin-afd-0.0.3/nonebot_plugin_afd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-20 15:41:08.000000 nonebot-plugin-afd-0.0.3/nonebot_plugin_afd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-20 15:41:08.000000 nonebot-plugin-afd-0.0.3/nonebot_plugin_afd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:41:08.000000 nonebot-plugin-afd-0.0.3/nonebot_plugin_afd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 15:41:08.000000 nonebot-plugin-afd-0.0.3/nonebot_plugin_afd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 15:41:08.000000 nonebot-plugin-afd-0.0.3/nonebot_plugin_afd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:41:08.597215 nonebot-plugin-afd-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-20 15:40:56.000000 nonebot-plugin-afd-0.0.3/setup.py
```

### Comparing `nonebot-plugin-afd-0.0.2/LICENSE` & `nonebot-plugin-afd-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-afd-0.0.2/PKG-INFO` & `nonebot-plugin-afd-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-afd
-Version: 0.0.2
+Version: 0.0.3
 Summary: 基于NoneBot的自动审核爱发电订单号进群的插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-afd
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nonebot-plugin-afd-0.0.2/README.md` & `nonebot-plugin-afd-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-afd-0.0.2/nonebot_plugin_afd/group_new_member.py` & `nonebot-plugin-afd-0.0.3/nonebot_plugin_afd/group_new_member.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-afd-0.0.2/nonebot_plugin_afd.egg-info/PKG-INFO` & `nonebot-plugin-afd-0.0.3/nonebot_plugin_afd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-afd
-Version: 0.0.2
+Version: 0.0.3
 Summary: 基于NoneBot的自动审核爱发电订单号进群的插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-afd
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nonebot-plugin-afd-0.0.2/setup.py` & `nonebot-plugin-afd-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-afd",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.2",  # 程序版本
+    version="0.0.3",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="基于NoneBot的自动审核爱发电订单号进群的插件",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/nonebot-plugin-afd",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     classifiers=[
         "Programming Language :: Python :: 3.9",  # 使用Python3.9
         "License :: OSI Approved :: GNU Affero General Public License v3",  # 开源协议
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'nonebot2>=2.0.0rc3',
+        'nonebot2>=2.0.0',
         'nonebot-adapter-onebot>=2.2.1',
         'pydantic>=1.10.4',
         'httpx>=0.23.3'
     ]
 )
```

