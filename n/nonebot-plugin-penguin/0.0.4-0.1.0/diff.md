# Comparing `tmp/nonebot_plugin_penguin-0.0.4.tar.gz` & `tmp/nonebot_plugin_penguin-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_penguin-0.0.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_penguin-0.1.0.tar", max compression
```

## Comparing `nonebot_plugin_penguin-0.0.4.tar` & `nonebot_plugin_penguin-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1068 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/LICENSE
--rw-r--r--   0        0        0     5314 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/README.md
--rw-r--r--   0        0        0      894 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/__init__.py
--rw-r--r--   0        0        0     1570 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/config.py
--rw-r--r--   0        0        0     2507 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/db.py
--rw-r--r--   0        0        0       48 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/__init__.py
--rw-r--r--   0        0        0      870 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/item_sprite.py
--rw-r--r--   0        0        0     2793 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/table.py
--rw-r--r--   0        0        0      970 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/templates/app.css
--rw-r--r--   0        0        0     3309 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/templates/card.css
--rw-r--r--   0        0        0     2731 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/templates/item_card.html
--rw-r--r--   0        0        0  1171678 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/templates/sprite.202210111514.png
--rw-r--r--   0        0        0     2774 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/templates/stage_card.html
--rw-r--r--   0        0        0      197 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/utils.py
--rw-r--r--   0        0        0     5457 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/request.py
--rw-r--r--   0        0        0      318 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/schedule.py
--rw-r--r--   0        0        0      353 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/startup.py
--rw-r--r--   0        0        0     1291 2023-06-02 09:05:49.921450 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/trim.py
--rw-r--r--   0        0        0     2628 2023-06-02 09:05:49.925449 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/types.py
--rw-r--r--   0        0        0    10980 2023-06-02 09:05:49.925449 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/user.py
--rw-r--r--   0        0        0     2071 2023-06-02 09:05:49.925449 nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/utils.py
--rw-r--r--   0        0        0     1875 2023-06-02 09:05:49.925449 nonebot_plugin_penguin-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6435 1970-01-01 00:00:00.000000 nonebot_plugin_penguin-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5314 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/README.md
+-rw-r--r--   0        0        0      890 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/__init__.py
+-rw-r--r--   0        0        0     1570 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/config.py
+-rw-r--r--   0        0        0     2507 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/db.py
+-rw-r--r--   0        0        0       48 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/__init__.py
+-rw-r--r--   0        0        0      870 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/item_sprite.py
+-rw-r--r--   0        0        0     2793 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/table.py
+-rw-r--r--   0        0        0      970 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/templates/app.css
+-rw-r--r--   0        0        0     3309 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/templates/card.css
+-rw-r--r--   0        0        0     2731 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/templates/item_card.html
+-rw-r--r--   0        0        0  1171678 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/templates/sprite.202210111514.png
+-rw-r--r--   0        0        0     2774 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/templates/stage_card.html
+-rw-r--r--   0        0        0      197 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/utils.py
+-rw-r--r--   0        0        0     5457 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/request.py
+-rw-r--r--   0        0        0      318 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/schedule.py
+-rw-r--r--   0        0        0      353 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/startup.py
+-rw-r--r--   0        0        0     1291 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/trim.py
+-rw-r--r--   0        0        0     2628 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/types.py
+-rw-r--r--   0        0        0    10980 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/user.py
+-rw-r--r--   0        0        0     2071 2023-06-20 15:21:40.073996 nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/utils.py
+-rw-r--r--   0        0        0     1875 2023-06-20 15:21:40.077997 nonebot_plugin_penguin-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6435 1970-01-01 00:00:00.000000 nonebot_plugin_penguin-0.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_penguin-0.0.4/LICENSE` & `nonebot_plugin_penguin-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/README.md` & `nonebot_plugin_penguin-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/__init__.py` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "startup",
     "trim",
     "user",
     "types",
     "utils",
 ]
 
-__plugin_metadata__ = PluginMetadata(
+__plugin_meta__ = PluginMetadata(
     name="nonebot_plugin_penguin",
     description="使用nonebot2查询企鹅物流掉落物数据",
     usage="发送命令 `penguin -h` 查看帮助",
     type="application",
     homepage="https://github.com/AzideCupric/nonebot-plugin-penguin",
     config=PlugConfig,
     supported_adapters=None,
```

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/config.py` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/db.py` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/item_sprite.py` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/item_sprite.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/table.py` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/table.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/templates/app.css` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/templates/app.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/templates/card.css` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/templates/card.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/templates/item_card.html` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/templates/item_card.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/templates/sprite.202210111514.png` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/templates/sprite.202210111514.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/render/templates/stage_card.html` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/render/templates/stage_card.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/request.py` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/trim.py` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/trim.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/types.py` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/user.py` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/nonebot_plugin_penguin/utils.py` & `nonebot_plugin_penguin-0.1.0/nonebot_plugin_penguin/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.4/pyproject.toml` & `nonebot_plugin_penguin-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-penguin"
-version = "0.0.4"
+version = "0.1.0"
 description = "get penguin data and send from https://penguin-stats.io/"
 authors = ["Azide <rukuy@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_penguin" }]
 homepage = "https://github.com/AzideCupric/nonebot-plugin-penguin"
 repository = "https://github.com/AzideCupric/nonebot-plugin-penguin"
```

### Comparing `nonebot_plugin_penguin-0.0.4/PKG-INFO` & `nonebot_plugin_penguin-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-penguin
-Version: 0.0.4
+Version: 0.1.0
 Summary: get penguin data and send from https://penguin-stats.io/
 Home-page: https://github.com/AzideCupric/nonebot-plugin-penguin
 License: MIT
 Author: Azide
 Author-email: rukuy@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-penguin Version: 0.0.4 Summary: get
+Metadata-Version: 2.1 Name: nonebot-plugin-penguin Version: 0.1.0 Summary: get
 penguin data and send from https://penguin-stats.io/ Home-page: https://
 github.com/AzideCupric/nonebot-plugin-penguin License: MIT Author: Azide
 Author-email: rukuy@qq.com Requires-Python: >=3.10,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

