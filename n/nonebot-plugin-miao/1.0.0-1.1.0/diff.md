# Comparing `tmp/nonebot_plugin_miao-1.0.0.tar.gz` & `tmp/nonebot_plugin_miao-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_miao-1.0.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_miao-1.1.0.tar", max compression
```

## Comparing `nonebot_plugin_miao-1.0.0.tar` & `nonebot_plugin_miao-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34523 2023-03-26 14:03:49.636141 nonebot_plugin_miao-1.0.0/LICENSE
--rw-r--r--   0        0        0     2050 2023-03-26 14:03:49.636141 nonebot_plugin_miao-1.0.0/README.md
--rw-r--r--   0        0        0      995 2023-03-26 14:03:49.636141 nonebot_plugin_miao-1.0.0/nonebot_plugin_miao/__init__.py
--rw-r--r--   0        0        0      411 2023-03-26 14:03:49.636141 nonebot_plugin_miao-1.0.0/nonebot_plugin_miao/config.py
--rw-r--r--   0        0        0      493 2023-03-26 14:03:49.636141 nonebot_plugin_miao-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2734 1970-01-01 00:00:00.000000 nonebot_plugin_miao-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-20 14:21:15.863165 nonebot_plugin_miao-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2051 2023-06-20 14:21:15.863165 nonebot_plugin_miao-1.1.0/README.md
+-rw-r--r--   0        0        0     1315 2023-06-20 14:21:15.863165 nonebot_plugin_miao-1.1.0/nonebot_plugin_miao/__init__.py
+-rw-r--r--   0        0        0      411 2023-06-20 14:21:15.863165 nonebot_plugin_miao-1.1.0/nonebot_plugin_miao/config.py
+-rw-r--r--   0        0        0      492 2023-06-20 14:21:15.863165 nonebot_plugin_miao-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2735 1970-01-01 00:00:00.000000 nonebot_plugin_miao-1.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_miao-1.0.0/LICENSE` & `nonebot_plugin_miao-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_miao-1.0.0/README.md` & `nonebot_plugin_miao-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 ## 🔧 配置项
 
 在你的bot的配置文件(.env.*)中添加以下配置项(不区分大小写)
 
 |       配置项        |    默认值     |                     说明                      |
 |:----------------:|:----------:|:-------------------------------------------:|
-|    miao_texts    | ["喵", "旺"] |                    口癖词列表                    |
+|    miao_words    | ["喵", "旺"] |                    口癖词列表                    |
 | miao_probability |    0.5     |                   添加口癖的概率                   |
 |  miao_position   |    end     | 添加口癖的位置，可选start(开头)、end(结尾)、random(句子中随机位置) |
 |    miao_count    |     1      |                  最多添加的词数量                   |
 
 ## 💝 鸣谢
 
-- [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
+- [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
```

#### html2text {}

```diff
@@ -6,13 +6,13 @@
 éè¿on_calling_apié©å­ï¼ç»ä½ çBotççº¯ææ¬åè¨æ·»å ä¸äºå¥æªçå£ç
 (ã ## ð¿ å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```shell nb plugin install nonebot-plugin-miao
 ``` ## â¨ ä¾å­ ä»¥åç½®çechoæä»¶(ä½ç¨æ¯å¤è¯»ä½ çè¯)ä¸ºä¾ ``` -
 /echo è¯¶å¿ - è¯¶å¿åµ - /echo è¯¶å¦ä½ å¹²å - è¯¶å¦ä½ å¹²åæº ``` ##
 ð§ éç½®é¡¹ å¨ä½ çbotçéç½®æä»¶(.env.*)ä¸­æ·»å ä»¥ä¸éç½®é¡¹
 (ä¸åºåå¤§å°å) | éç½®é¡¹ | é»è®¤å¼ | è¯´æ | |:----------------:|:--
---------:|:-------------------------------------------:| | miao_texts | ["åµ",
+--------:|:-------------------------------------------:| | miao_words | ["åµ",
 "æº"] | å£çè¯åè¡¨ | | miao_probability | 0.5 | æ·»å å£ççæ¦ç | |
 miao_position | end | æ·»å å£ççä½ç½®ï¼å¯éstart(å¼å¤´)ãend
 (ç»å°¾)ãrandom(å¥å­ä¸­éæºä½ç½®) | | miao_count | 1 |
 æå¤æ·»å çè¯æ°é | ## ð é¸£è°¢ - [Nonebot](https://github.com/
 nonebot/nonebot2): æ¬é¡¹ç®çåºç¡ï¼éå¸¸å¥½ç¨çèå¤©æºå¨äººæ¡æ¶ã
```

### Comparing `nonebot_plugin_miao-1.0.0/nonebot_plugin_miao/__init__.py` & `nonebot_plugin_miao-1.1.0/nonebot_plugin_miao/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 import contextlib
 import random
 from typing import Dict, Any
 
 from nonebot.adapters import Bot
+from nonebot.plugin import PluginMetadata
 
-from .config import config
+from .config import config, Config
+
+__plugin_meta__ = PluginMetadata(
+    name="口癖",
+    description="让Bot的发言添加口癖",
+    usage="被动技能",
+    type="application",
+    homepage="https://github.com/CMHopeSunshine/nonebot-plugin-miao",
+    config=Config,
+    supported_adapters=None
+)
 
 
 @Bot.on_calling_api
 async def handle_miao(bot: Bot, api: str, data: Dict[str, Any]):
     with contextlib.suppress(Exception):
         if api not in ['send_msg', 'send_message']:
             return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_miao-1.0.0/PKG-INFO` & `nonebot_plugin_miao-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-miao
-Version: 1.0.0
+Version: 1.1.0
 Summary: Nonebot2 plugin to make your bot talk weird.
 Home-page: https://github.com/CMHopeSunshine/nonebot-plugin-miao
 License: AGPL
 Keywords: nonebot2
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
@@ -63,15 +63,16 @@
 
 ## 🔧 配置项
 
 在你的bot的配置文件(.env.*)中添加以下配置项(不区分大小写)
 
 |       配置项        |    默认值     |                     说明                      |
 |:----------------:|:----------:|:-------------------------------------------:|
-|    miao_texts    | ["喵", "旺"] |                    口癖词列表                    |
+|    miao_words    | ["喵", "旺"] |                    口癖词列表                    |
 | miao_probability |    0.5     |                   添加口癖的概率                   |
 |  miao_position   |    end     | 添加口癖的位置，可选start(开头)、end(结尾)、random(句子中随机位置) |
 |    miao_count    |     1      |                  最多添加的词数量                   |
 
 ## 💝 鸣谢
 
 - [Nonebot](https://github.com/nonebot/nonebot2): 本项目的基础，非常好用的聊天机器人框架。
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-miao Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-miao Version: 1.1.0 Summary:
 Nonebot2 plugin to make your bot talk weird. Home-page: https://github.com/
 CMHopeSunshine/nonebot-plugin-miao License: AGPL Keywords: nonebot2 Author:
 CMHopeSunshine Author-email: 277073121@qq.com Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -16,13 +16,13 @@
 éè¿on_calling_apié©å­ï¼ç»ä½ çBotççº¯ææ¬åè¨æ·»å ä¸äºå¥æªçå£ç
 (ã ## ð¿ å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```shell nb plugin install nonebot-plugin-miao
 ``` ## â¨ ä¾å­ ä»¥åç½®çechoæä»¶(ä½ç¨æ¯å¤è¯»ä½ çè¯)ä¸ºä¾ ``` -
 /echo è¯¶å¿ - è¯¶å¿åµ - /echo è¯¶å¦ä½ å¹²å - è¯¶å¦ä½ å¹²åæº ``` ##
 ð§ éç½®é¡¹ å¨ä½ çbotçéç½®æä»¶(.env.*)ä¸­æ·»å ä»¥ä¸éç½®é¡¹
 (ä¸åºåå¤§å°å) | éç½®é¡¹ | é»è®¤å¼ | è¯´æ | |:----------------:|:--
---------:|:-------------------------------------------:| | miao_texts | ["åµ",
+--------:|:-------------------------------------------:| | miao_words | ["åµ",
 "æº"] | å£çè¯åè¡¨ | | miao_probability | 0.5 | æ·»å å£ççæ¦ç | |
 miao_position | end | æ·»å å£ççä½ç½®ï¼å¯éstart(å¼å¤´)ãend
 (ç»å°¾)ãrandom(å¥å­ä¸­éæºä½ç½®) | | miao_count | 1 |
 æå¤æ·»å çè¯æ°é | ## ð é¸£è°¢ - [Nonebot](https://github.com/
 nonebot/nonebot2): æ¬é¡¹ç®çåºç¡ï¼éå¸¸å¥½ç¨çèå¤©æºå¨äººæ¡æ¶ã
```

