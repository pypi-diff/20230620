# Comparing `tmp/nonebot-plugin-bwiki-navigator-0.1.0.tar.gz` & `tmp/nonebot_plugin_bwiki_navigator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-bwiki-navigator-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_bwiki_navigator-0.2.0.tar", max compression
```

## Comparing `nonebot-plugin-bwiki-navigator-0.1.0.tar` & `nonebot_plugin_bwiki_navigator-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    35184 2022-09-17 11:44:36.472824 nonebot-plugin-bwiki-navigator-0.1.0/LICENSE
--rw-r--r--   0        0        0      839 2022-09-17 15:35:56.587513 nonebot-plugin-bwiki-navigator-0.1.0/nonebot_plugin_bwiki_navigator/__init__.py
--rw-r--r--   0        0        0      310 2022-09-17 15:35:41.823392 nonebot-plugin-bwiki-navigator-0.1.0/nonebot_plugin_bwiki_navigator/config.py
--rw-r--r--   0        0        0     5360 2022-09-17 15:35:36.857185 nonebot-plugin-bwiki-navigator-0.1.0/nonebot_plugin_bwiki_navigator/handler.py
--rw-r--r--   0        0        0     1937 2022-09-17 15:17:55.038355 nonebot-plugin-bwiki-navigator-0.1.0/nonebot_plugin_bwiki_navigator/parser.py
--rw-r--r--   0        0        0      701 2022-09-17 12:44:01.449967 nonebot-plugin-bwiki-navigator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2433 2022-09-17 15:49:40.883632 nonebot-plugin-bwiki-navigator-0.1.0/README.md
--rw-r--r--   0        0        0     3253 1970-01-01 00:00:00.000000 nonebot-plugin-bwiki-navigator-0.1.0/setup.py
--rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 nonebot-plugin-bwiki-navigator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-09-17 11:44:36.472824 nonebot_plugin_bwiki_navigator-0.2.0/LICENSE
+-rw-r--r--   0        0        0      939 2023-06-19 16:39:40.770995 nonebot_plugin_bwiki_navigator-0.2.0/nonebot_plugin_bwiki_navigator/__init__.py
+-rw-r--r--   0        0        0      310 2022-09-17 15:35:41.823392 nonebot_plugin_bwiki_navigator-0.2.0/nonebot_plugin_bwiki_navigator/config.py
+-rw-r--r--   0        0        0     5360 2022-09-17 15:35:36.857185 nonebot_plugin_bwiki_navigator-0.2.0/nonebot_plugin_bwiki_navigator/handler.py
+-rw-r--r--   0        0        0     1937 2022-09-17 15:17:55.038355 nonebot_plugin_bwiki_navigator-0.2.0/nonebot_plugin_bwiki_navigator/parser.py
+-rw-r--r--   0        0        0      702 2023-06-19 16:47:48.675866 nonebot_plugin_bwiki_navigator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2420 2023-06-19 16:41:05.619764 nonebot_plugin_bwiki_navigator-0.2.0/README.md
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 nonebot_plugin_bwiki_navigator-0.2.0/PKG-INFO
```

### Comparing `nonebot-plugin-bwiki-navigator-0.1.0/LICENSE` & `nonebot_plugin_bwiki_navigator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-bwiki-navigator-0.1.0/nonebot_plugin_bwiki_navigator/__init__.py` & `nonebot_plugin_bwiki_navigator-0.2.0/nonebot_plugin_bwiki_navigator/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,11 +13,13 @@
 __plugin_meta__ = PluginMetadata(
     name='Bwiki Navigator',
     description='Bwiki助手（官方移植版）',
     usage=f'''欢迎使用Bwiki助手移植版，召唤方法如下：
 {default_start}{cmd_str} bwiki子站域名 页面名(可选)
 例如：{default_start}{cmd_str} clover 凯瑟琳
 {default_start}{cmd_str} clover''',
-    extra={'version': '0.1.0'}
+    type='application',
+    homepage='https://github.com/xzhouqd/nonebot-plugin-bwiki-navigator',
+    extra={'version': '0.2.0'}
 )
 
 from .handler import bwiki
```

### Comparing `nonebot-plugin-bwiki-navigator-0.1.0/nonebot_plugin_bwiki_navigator/handler.py` & `nonebot_plugin_bwiki_navigator-0.2.0/nonebot_plugin_bwiki_navigator/handler.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-bwiki-navigator-0.1.0/nonebot_plugin_bwiki_navigator/parser.py` & `nonebot_plugin_bwiki_navigator-0.2.0/nonebot_plugin_bwiki_navigator/parser.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-bwiki-navigator-0.1.0/pyproject.toml` & `nonebot_plugin_bwiki_navigator-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "nonebot-plugin-bwiki-navigator"
-version = "0.1.0"
+version = "0.2.0"
 description = "A nonebot2 plugin version of bwiki official bot"
 authors = ["XZhouQD <X.Zhou.QD@hotmail.com>"]
 license = "AGPL v3"
 readme = "README.md"
 include = [
     "LICENSE",
 ]
 homepage = "https://github.com/XZhouQD/nonebot-plugin-bwiki-navigator"
 repository = "https://github.com/XZhouQD/nonebot-plugin-bwiki-navigator"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-nonebot2 = "^2.0.0-beta.4"
+nonebot2 = "^2.0.0"
 nonebot-adapter-onebot = "^2.0.0-beta.1"
-httpx = { version = "^0.20.0", extras = ["http2"] }
+httpx = { version = ">=0.20.0,<1.0.0", extras = ["http2"] }
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot-plugin-bwiki-navigator-0.1.0/README.md` & `nonebot_plugin_bwiki_navigator-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-bwiki-navigator">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-bwiki-navigator?color=green&style=for-the-badge" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-^3.8-blue?style=for-the-badge" alt="python">
 <br />
 <img src="https://img.shields.io/badge/tested_python-3.10.4-blue?style=for-the-badge" alt="python">
-<img src="https://img.shields.io/static/v1?label=tested+env&message=go-cqhttp+1.0.0-rc3&color=blue&style=for-the-badge" alt="python">
+<img src="https://img.shields.io/static/v1?label=tested+env&message=go-cqhttp+1.0.0&color=blue&style=for-the-badge" alt="python">
 <br />
 <a href="https://github.com/botuniverse/onebot/blob/master/README.md">
     <img src="https://img.shields.io/badge/Onebot-v11-brightgreen?style=for-the-badge" alt="onebot">
 </a>
 <a href="https://github.com/nonebot/nonebot2">
-    <img src="https://img.shields.io/static/v1?label=Nonebot&message=^2.0.0%2Dbeta.4&color=red&style=for-the-badge" alt="nonebot">
+    <img src="https://img.shields.io/static/v1?label=Nonebot&message=^2.0.0&color=red&style=for-the-badge" alt="nonebot">
 </a>
 <a href="https://pypi.org/project/nonebot-adapter-cqhttp/">
     <img src="https://img.shields.io/static/v1?label=Nonebot-adapters-onebot&message=^2.0.0%2Dbeta.1&color=red&style=for-the-badge" alt="nonebot-adapters-cqhttp">
 </a>
 </div>
 
 ## 简介
```

### Comparing `nonebot-plugin-bwiki-navigator-0.1.0/setup.py` & `nonebot_plugin_bwiki_navigator-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,83 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-bwiki-navigator
+Version: 0.2.0
+Summary: A nonebot2 plugin version of bwiki official bot
+Home-page: https://github.com/XZhouQD/nonebot-plugin-bwiki-navigator
+License: AGPL v3
+Author: XZhouQD
+Author-email: X.Zhou.QD@hotmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx[http2] (>=0.20.0,<1.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Project-URL: Repository, https://github.com/XZhouQD/nonebot-plugin-bwiki-navigator
+Description-Content-Type: text/markdown
+
+<div align="center">
+
+# nonebot-plugin-bwiki-navigator
+### BWiki助手Nonebot2插件移植版
+
+<a href="https://raw.githubusercontent.com/xzhouqd/nonebot-plugin-bwiki-navigator/main/LICENSE">
+    <img src="https://img.shields.io/github/license/xzhouqd/nonebot-plugin-help?style=for-the-badge" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-bwiki-navigator">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-bwiki-navigator?color=green&style=for-the-badge" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-^3.8-blue?style=for-the-badge" alt="python">
+<br />
+<img src="https://img.shields.io/badge/tested_python-3.10.4-blue?style=for-the-badge" alt="python">
+<img src="https://img.shields.io/static/v1?label=tested+env&message=go-cqhttp+1.0.0&color=blue&style=for-the-badge" alt="python">
+<br />
+<a href="https://github.com/botuniverse/onebot/blob/master/README.md">
+    <img src="https://img.shields.io/badge/Onebot-v11-brightgreen?style=for-the-badge" alt="onebot">
+</a>
+<a href="https://github.com/nonebot/nonebot2">
+    <img src="https://img.shields.io/static/v1?label=Nonebot&message=^2.0.0&color=red&style=for-the-badge" alt="nonebot">
+</a>
+<a href="https://pypi.org/project/nonebot-adapter-cqhttp/">
+    <img src="https://img.shields.io/static/v1?label=Nonebot-adapters-onebot&message=^2.0.0%2Dbeta.1&color=red&style=for-the-badge" alt="nonebot-adapters-cqhttp">
+</a>
+</div>
+
+## 简介
+本插件是针对BWIKI助手解析的非官方Nonebot2插件移植版
+
+关于BWiki助手解析接入方式，请参阅 [BWIKI - WIKI助手文档](https://wiki.biligame.com/wiki/WIKI%E5%8A%A9%E6%89%8B%E6%96%87%E6%A1%A3)
+
+### 可配置项（可选）
+```
+BWIKI_NAVIGATOR_COMMAND="bwiki"                 // 本插件的主查询命令名
+BWIKI_NAVIGATOR_COMMAND_ALIAS=["wiki"]         // 本插件的查询命令别名列表
+```
+
+### 使用方法
+```
+/bwiki bwiki子站域名 页面名(可选)
+```
+
+### 示例
+```
+/bwiki clover
+
+四叶草剧场WIKI https://wiki.biligame.com/clover
+
+
+/bwiki clover 沙盒
+
+四叶草剧场WIKI 沙盒
+https://wiki.biligame.com/clover/?curid=19
+在这里测试你的代码！
+隐藏的wiki bot转换语句
+[图片]
+[图片]
+```
 
-packages = \
-['nonebot_plugin_bwiki_navigator']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['httpx[http2]>=0.20.0,<0.21.0',
- 'nonebot-adapter-onebot>=2.0.0-beta.1,<3.0.0',
- 'nonebot2>=2.0.0-beta.4,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-bwiki-navigator',
-    'version': '0.1.0',
-    'description': 'A nonebot2 plugin version of bwiki official bot',
-    'long_description': '<div align="center">\n\n# nonebot-plugin-bwiki-navigator\n### BWiki助手Nonebot2插件移植版\n\n<a href="https://raw.githubusercontent.com/xzhouqd/nonebot-plugin-bwiki-navigator/main/LICENSE">\n    <img src="https://img.shields.io/github/license/xzhouqd/nonebot-plugin-help?style=for-the-badge" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot-plugin-bwiki-navigator">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-bwiki-navigator?color=green&style=for-the-badge" alt="pypi">\n</a>\n<img src="https://img.shields.io/badge/python-^3.8-blue?style=for-the-badge" alt="python">\n<br />\n<img src="https://img.shields.io/badge/tested_python-3.10.4-blue?style=for-the-badge" alt="python">\n<img src="https://img.shields.io/static/v1?label=tested+env&message=go-cqhttp+1.0.0-rc3&color=blue&style=for-the-badge" alt="python">\n<br />\n<a href="https://github.com/botuniverse/onebot/blob/master/README.md">\n    <img src="https://img.shields.io/badge/Onebot-v11-brightgreen?style=for-the-badge" alt="onebot">\n</a>\n<a href="https://github.com/nonebot/nonebot2">\n    <img src="https://img.shields.io/static/v1?label=Nonebot&message=^2.0.0%2Dbeta.4&color=red&style=for-the-badge" alt="nonebot">\n</a>\n<a href="https://pypi.org/project/nonebot-adapter-cqhttp/">\n    <img src="https://img.shields.io/static/v1?label=Nonebot-adapters-onebot&message=^2.0.0%2Dbeta.1&color=red&style=for-the-badge" alt="nonebot-adapters-cqhttp">\n</a>\n</div>\n\n## 简介\n本插件是针对BWIKI助手解析的非官方Nonebot2插件移植版\n\n关于BWiki助手解析接入方式，请参阅 [BWIKI - WIKI助手文档](https://wiki.biligame.com/wiki/WIKI%E5%8A%A9%E6%89%8B%E6%96%87%E6%A1%A3)\n\n### 可配置项（可选）\n```\nBWIKI_NAVIGATOR_COMMAND="bwiki"                 // 本插件的主查询命令名\nBWIKI_NAVIGATOR_COMMAND_ALIAS=["wiki"]         // 本插件的查询命令别名列表\n```\n\n### 使用方法\n```\n/bwiki bwiki子站域名 页面名(可选)\n```\n\n### 示例\n```\n/bwiki clover\n\n四叶草剧场WIKI https://wiki.biligame.com/clover\n\n\n/bwiki clover 沙盒\n\n四叶草剧场WIKI 沙盒\nhttps://wiki.biligame.com/clover/?curid=19\n在这里测试你的代码！\n隐藏的wiki bot转换语句\n[图片]\n[图片]\n```\n\n### 已完整接入帮助菜单\n[nonebot-plugin-help](https://github.com/xzhouqd/nonebot-plugin-help) ([PyPI](https://pypi.python.org/pypi/nonebot-plugin-help))',
-    'author': 'XZhouQD',
-    'author_email': 'X.Zhou.QD@hotmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/XZhouQD/nonebot-plugin-bwiki-navigator',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
+### 已完整接入帮助菜单
+[nonebot-plugin-help](https://github.com/xzhouqd/nonebot-plugin-help) ([PyPI](https://pypi.python.org/pypi/nonebot-plugin-help))
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_bwiki_navigator'] package_data = \ {'': ['*']}
-install_requires = \ ['httpx[http2]>=0.20.0,<0.21.0', 'nonebot-adapter-
-onebot>=2.0.0-beta.1,<3.0.0', 'nonebot2>=2.0.0-beta.4,<3.0.0'] setup_kwargs =
-{ 'name': 'nonebot-plugin-bwiki-navigator', 'version': '0.1.0', 'description':
-'A nonebot2 plugin version of bwiki official bot', 'long_description': '
-                   \n\n# nonebot-plugin-bwiki-navigator\n###
- BWikiå©æNonebot2æä»¶ç§»æ¤ç\n\n\n_[license]\n\n\n_[pypi]\n\n[python]\n
-                            \n[python]\n[python]\n
-       \n\n_[onebot]\n\n\n_[nonebot]\n\n\n_[nonebot-adapters-cqhttp]\n\n
-\n\n##
-ç®ä»\næ¬æä»¶æ¯éå¯¹BWIKIå©æè§£æçéå®æ¹Nonebot2æä»¶ç§»æ¤ç\n\nå³äºBWikiå©æè§£ææ¥å¥æ¹å¼ï¼è¯·åé
-[BWIKI - WIKIå©æææ¡£](https://wiki.biligame.com/wiki/
-WIKI%E5%8A%A9%E6%89%8B%E6%96%87%E6%A1%A3)\n\n###
-å¯éç½®é¡¹ï¼å¯éï¼\n```\nBWIKI_NAVIGATOR_COMMAND="bwiki" /
-/ æ¬æä»¶çä¸»æ¥è¯¢å½ä»¤å\nBWIKI_NAVIGATOR_COMMAND_ALIAS=["wiki"] /
-/ æ¬æä»¶çæ¥è¯¢å½ä»¤å«ååè¡¨\n```\n\n### ä½¿ç¨æ¹æ³\n```\n/bwiki
-bwikiå­ç«åå é¡µé¢å(å¯é)\n```\n\n### ç¤ºä¾\n```\n/bwiki
-clover\n\nåå¶èå§åºWIKI https://wiki.biligame.com/clover\n\n\n/bwiki
-clover æ²ç\n\nåå¶èå§åºWIKI æ²ç\nhttps://wiki.biligame.com/clover/
-?curid=19\nå¨è¿éæµè¯ä½ çä»£ç ï¼\néèçwiki botè½¬æ¢è¯­å¥\n
-[å¾ç]\n[å¾ç]\n```\n\n### å·²å®æ´æ¥å¥å¸®å©èå\n[nonebot-plugin-
-help](https://github.com/xzhouqd/nonebot-plugin-help) ([PyPI](https://
-pypi.python.org/pypi/nonebot-plugin-help))', 'author': 'XZhouQD',
-'author_email': 'X.Zhou.QD@hotmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/XZhouQD/nonebot-plugin-
-bwiki-navigator', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.8,<4.0', } setup
-(**setup_kwargs)
+Metadata-Version: 2.1 Name: nonebot-plugin-bwiki-navigator Version: 0.2.0
+Summary: A nonebot2 plugin version of bwiki official bot Home-page: https://
+github.com/XZhouQD/nonebot-plugin-bwiki-navigator License: AGPL v3 Author:
+XZhouQD Author-email: X.Zhou.QD@hotmail.com Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx[http2] (>=0.20.0,<1.0.0) Requires-Dist: nonebot-adapter-
+onebot (>=2.0.0-beta.1,<3.0.0) Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Project-URL: Repository, https://github.com/XZhouQD/nonebot-plugin-bwiki-
+navigator Description-Content-Type: text/markdown
+   # nonebot-plugin-bwiki-navigator ### BWikiå©æNonebot2æä»¶ç§»æ¤ç
+                          [license] [pypi] [python]
+                              [python] [python]
+                 [onebot] [nonebot] [nonebot-adapters-cqhttp]
+## ç®ä»
+æ¬æä»¶æ¯éå¯¹BWIKIå©æè§£æçéå®æ¹Nonebot2æä»¶ç§»æ¤ç
+å³äºBWikiå©æè§£ææ¥å¥æ¹å¼ï¼è¯·åé [BWIKI - WIKIå©æææ¡£]
+(https://wiki.biligame.com/wiki/WIKI%E5%8A%A9%E6%89%8B%E6%96%87%E6%A1%A3) ###
+å¯éç½®é¡¹ï¼å¯éï¼ ``` BWIKI_NAVIGATOR_COMMAND="bwiki" /
+/ æ¬æä»¶çä¸»æ¥è¯¢å½ä»¤å BWIKI_NAVIGATOR_COMMAND_ALIAS=["wiki"] /
+/ æ¬æä»¶çæ¥è¯¢å½ä»¤å«ååè¡¨ ``` ### ä½¿ç¨æ¹æ³ ``` /bwiki
+bwikiå­ç«åå é¡µé¢å(å¯é) ``` ### ç¤ºä¾ ``` /bwiki clover
+åå¶èå§åºWIKI https://wiki.biligame.com/clover /bwiki clover æ²ç
+åå¶èå§åºWIKI æ²ç https://wiki.biligame.com/clover/?curid=19
+å¨è¿éæµè¯ä½ çä»£ç ï¼ éèçwiki botè½¬æ¢è¯­å¥ [å¾ç] [å¾ç]
+``` ### å·²å®æ´æ¥å¥å¸®å©èå [nonebot-plugin-help](https://github.com/
+xzhouqd/nonebot-plugin-help) ([PyPI](https://pypi.python.org/pypi/nonebot-
+plugin-help))
```

