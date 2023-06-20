# Comparing `tmp/nonebot_plugin_smart_reply-0.0.9.tar.gz` & `tmp/nonebot_plugin_smart_reply-0.1.114514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_smart_reply-0.0.9.tar", last modified: Mon Nov 21 14:06:32 2022, max compression
+gzip compressed data, was "nonebot_plugin_smart_reply-0.1.114514.tar", last modified: Tue Jun 20 13:24:56 2023, max compression
```

## Comparing `nonebot_plugin_smart_reply-0.0.9.tar` & `nonebot_plugin_smart_reply-0.1.114514.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxrwxrwx   0        0        0        0 2022-11-21 14:06:32.872003 nonebot_plugin_smart_reply-0.0.9/
--rw-rw-rw-   0        0        0      269 2022-11-21 14:06:32.871003 nonebot_plugin_smart_reply-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      366 2022-06-18 06:47:22.000000 nonebot_plugin_smart_reply-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2022-11-21 14:06:32.814003 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/
--rw-rw-rw-   0        0        0     3561 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-21 14:06:32.811004 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/
-drwxrwxrwx   0        0        0        0 2022-11-21 14:06:32.869003 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/
--rw-rw-rw-   0        0        0    32921 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac
--rw-rw-rw-   0        0        0   122981 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac
--rw-rw-rw-   0        0        0    67013 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac
--rw-rw-rw-   0        0        0    42760 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac
--rw-rw-rw-   0        0        0    36232 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac
--rw-rw-rw-   0        0        0    11615 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/傻逼.aac
--rw-rw-rw-   0        0        0    68879 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/南通啊.aac
--rw-rw-rw-   0        0        0    15206 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/去死吧.aac
--rw-rw-rw-   0        0        0   101527 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/变态啊.aac
--rw-rw-rw-   0        0        0   105258 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac
--rw-rw-rw-   0        0        0     6491 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac
--rw-rw-rw-   0        0        0    15706 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/操你妈.aac
--rw-rw-rw-   0        0        0    96863 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/救命啊.aac
--rw-rw-rw-   0        0        0    14470 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac
--rw-rw-rw-   0        0        0    74476 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac
-drwxrwxrwx   0        0        0        0 2022-11-21 14:06:32.870003 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/json/
--rw-rw-rw-   0        0        0    81633 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/json/data.json
--rw-rw-rw-   0        0        0     3594 2022-11-21 14:05:38.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-21 14:06:32.842004 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/
--rw-rw-rw-   0        0        0      269 2022-11-21 14:06:32.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1298 2022-11-21 14:06:32.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-21 14:06:32.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2022-11-21 14:06:32.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2022-11-21 14:06:32.000000 nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-21 14:06:32.872003 nonebot_plugin_smart_reply-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      585 2022-11-21 14:06:07.000000 nonebot_plugin_smart_reply-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:24:56.249155 nonebot_plugin_smart_reply-0.1.114514/
+-rw-rw-rw-   0        0        0      274 2023-06-20 13:24:56.249155 nonebot_plugin_smart_reply-0.1.114514/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 13:24:56.132040 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/
+-rw-rw-rw-   0        0        0     4030 2023-06-20 13:24:19.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/__init__.py
+-rw-rw-rw-   0        0        0     1362 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/config.py
+-rw-rw-rw-   0        0        0     6708 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/getnewbing.py
+-rw-rw-rw-   0        0        0     7021 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/getopenai.py
+-rw-rw-rw-   0        0        0     5938 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/keywordhandle.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:24:56.120033 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/
+drwxrwxrwx   0        0        0        0 2023-06-20 13:24:56.213969 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/
+-rw-rw-rw-   0        0        0    32921 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac
+-rw-rw-rw-   0        0        0   122981 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac
+-rw-rw-rw-   0        0        0    67013 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac
+-rw-rw-rw-   0        0        0    42760 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac
+-rw-rw-rw-   0        0        0    36232 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac
+-rw-rw-rw-   0        0        0    11615 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/傻逼.aac
+-rw-rw-rw-   0        0        0    68879 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/南通啊.aac
+-rw-rw-rw-   0        0        0    15206 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/去死吧.aac
+-rw-rw-rw-   0        0        0   101527 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/变态啊.aac
+-rw-rw-rw-   0        0        0   105258 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac
+-rw-rw-rw-   0        0        0     6491 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac
+-rw-rw-rw-   0        0        0    15706 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/操你妈.aac
+-rw-rw-rw-   0        0        0    96863 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/救命啊.aac
+-rw-rw-rw-   0        0        0    14470 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac
+-rw-rw-rw-   0        0        0    74476 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac
+drwxrwxrwx   0        0        0        0 2023-06-20 13:24:56.247156 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/json/
+-rw-rw-rw-   0        0        0    81951 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/json/data.json
+-rw-rw-rw-   0        0        0     2031 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/txtToImg.py
+-rw-rw-rw-   0        0        0    10994 2023-06-20 13:22:22.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:24:56.158102 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply.egg-info/
+-rw-rw-rw-   0        0        0      274 2023-06-20 13:24:55.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1489 2023-06-20 13:24:56.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:24:55.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-06-20 13:24:55.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-20 13:24:55.000000 nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 13:24:56.250158 nonebot_plugin_smart_reply-0.1.114514/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-06-20 13:24:38.000000 nonebot_plugin_smart_reply-0.1.114514/setup.py
```

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/傻逼.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/傻逼.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/南通啊.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/南通啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/去死吧.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/去死吧.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/变态啊.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/变态啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/操你妈.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/操你妈.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/救命啊.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/救命啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply/resource/json/data.json` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply/resource/json/data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992937853107344%*

 * *Differences: {"'123'": "{insert: [(3, '456')]}"}*

```diff
@@ -1,12 +1,13 @@
 {
     "123": [
         "boom\uff01\u4f60\u6709\u6ca1\u6709\u88ab\u54b1\u5413\u5230\uff1f",
         "\u6728\u5934\u4eba~\u4f60\u4e0d\u8bb8\u52a8\uff1ew\uff1c",
-        "\u4e0a\u5c71\u6253\u8001\u864e\uff0c\u8001\u864e\u6ca1\u6253\u5230\n\u54b1\u6765\u51d1\u6570\u2014\u2014\u55f7\u545c\u55f7\u545c\u2517|\uff40O\u2032|\u251b\u55f7~~"
+        "\u4e0a\u5c71\u6253\u8001\u864e\uff0c\u8001\u864e\u6ca1\u6253\u5230\n\u54b1\u6765\u51d1\u6570\u2014\u2014\u55f7\u545c\u55f7\u545c\u2517|\uff40O\u2032|\u251b\u55f7~~",
+        "456"
     ],
     "awsl": [
         "\u4f60\u522b\u6b7b\u554a\uff01\uff08\u62b1\u4f4f\u4f7f\u52b2\u6643\uff09",
         "\u4f60\u522b\u6b7b\u554a\uff01\u54b1\u53c8\u8981\u5b64\u5355\u4e00\u4e2a\u4eba\u4e86QAQ",
         "\u554a\uff01\u600e\u4e48\u53c8\u6b7b\u4e86\u5440"
     ],
     "baka": [
```

### Comparing `nonebot_plugin_smart_reply-0.0.9/nonebot_plugin_smart_reply.egg-info/SOURCES.txt` & `nonebot_plugin_smart_reply-0.1.114514/nonebot_plugin_smart_reply.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-README.md
 setup.py
 nonebot_plugin_smart_reply/__init__.py
+nonebot_plugin_smart_reply/config.py
+nonebot_plugin_smart_reply/getnewbing.py
+nonebot_plugin_smart_reply/getopenai.py
+nonebot_plugin_smart_reply/keywordhandle.py
+nonebot_plugin_smart_reply/txtToImg.py
 nonebot_plugin_smart_reply/utils.py
 nonebot_plugin_smart_reply.egg-info/PKG-INFO
 nonebot_plugin_smart_reply.egg-info/SOURCES.txt
 nonebot_plugin_smart_reply.egg-info/dependency_links.txt
 nonebot_plugin_smart_reply.egg-info/requires.txt
 nonebot_plugin_smart_reply.egg-info/top_level.txt
 nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac
```

### Comparing `nonebot_plugin_smart_reply-0.0.9/setup.py` & `nonebot_plugin_smart_reply-0.1.114514/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 
 from setuptools import find_packages, setup
 name = 'nonebot_plugin_smart_reply'
 
 setup(
     name=name,  
-    version='0.0.9',
+    version='0.01.114514',
     author="Special-Week",
     author_email='2385612749@qq.com',
     description="encapsulate logger",
-    python_requires=">=3.8.*",
+    python_requires=">=3.8.1",
     packages=find_packages(),
     long_description="reply插件",
     url="https://github.com/Special-Week/nonebot_plugin_smart_reply",
 
     package_data={name: ['resource/json/*', 'resource/audio/*']},
 
     # 设置依赖包
-    install_requires=["ujson","httpx","nonebot2","nonebot-adapter-onebot"],
-)
+    install_requires=["EdgeGPT","revChatGPT","httpx","loguru","pillow","nonebot2","nonebot-adapter-onebot"],
+)
```

