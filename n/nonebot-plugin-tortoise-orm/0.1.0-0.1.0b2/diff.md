# Comparing `tmp/nonebot_plugin_tortoise_orm-0.1.0.tar.gz` & `tmp/nonebot_plugin_tortoise_orm-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tortoise_orm-0.1.0.tar", last modified: Tue Jun 20 08:34:21 2023, max compression
+gzip compressed data, was "nonebot_plugin_tortoise_orm-0.1.0b2.tar", last modified: Tue Jun 20 08:00:23 2023, max compression
```

## Comparing `nonebot_plugin_tortoise_orm-0.1.0.tar` & `nonebot_plugin_tortoise_orm-0.1.0b2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1062 2023-06-20 08:34:12.659043 nonebot_plugin_tortoise_orm-0.1.0/LICENSE
--rw-r--r--   0        0        0     2371 2023-06-20 08:34:12.659043 nonebot_plugin_tortoise_orm-0.1.0/README.md
--rw-r--r--   0        0        0     1113 2023-06-20 08:34:12.659043 nonebot_plugin_tortoise_orm-0.1.0/nonebot_plugin_tortoise_orm/__init__.py
--rw-r--r--   0        0        0     1008 2023-06-20 08:34:12.659043 nonebot_plugin_tortoise_orm-0.1.0/nonebot_plugin_tortoise_orm/config.py
--rw-r--r--   0        0        0      761 2023-06-20 08:34:21.123135 nonebot_plugin_tortoise_orm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 nonebot_plugin_tortoise_orm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-20 07:59:59.096009 nonebot_plugin_tortoise_orm-0.1.0b2/LICENSE
+-rw-r--r--   0        0        0     2371 2023-06-20 07:59:59.096009 nonebot_plugin_tortoise_orm-0.1.0b2/README.md
+-rw-r--r--   0        0        0     1113 2023-06-20 07:59:59.096009 nonebot_plugin_tortoise_orm-0.1.0b2/nonebot_plugin_tortoise_orm/__init__.py
+-rw-r--r--   0        0        0      649 2023-06-20 07:59:59.100009 nonebot_plugin_tortoise_orm-0.1.0b2/nonebot_plugin_tortoise_orm/config.py
+-rw-r--r--   0        0        0      768 2023-06-20 08:00:23.568399 nonebot_plugin_tortoise_orm-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 nonebot_plugin_tortoise_orm-0.1.0b2/PKG-INFO
```

### Comparing `nonebot_plugin_tortoise_orm-0.1.0/LICENSE` & `nonebot_plugin_tortoise_orm-0.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tortoise_orm-0.1.0/README.md` & `nonebot_plugin_tortoise_orm-0.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tortoise_orm-0.1.0/nonebot_plugin_tortoise_orm/__init__.py` & `nonebot_plugin_tortoise_orm-0.1.0b2/nonebot_plugin_tortoise_orm/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tortoise_orm-0.1.0/nonebot_plugin_tortoise_orm/config.py` & `nonebot_plugin_tortoise_orm-0.1.0b2/nonebot_plugin_tortoise_orm/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Dict
-from pathlib import Path
 
 from nonebot import get_driver
 from pydantic import Extra, BaseModel, root_validator
 from nonebot.log import logger
 from nonebot_plugin_localstore import get_data_dir
 
 
@@ -12,18 +11,12 @@
 
     @root_validator(pre=True, allow_reuse=True)
     def set_default(cls, value: Dict):
         if not value.get("db_url"):
             value["db_url"] = f'sqlite:///{get_data_dir("") / "db.sqlite3"}'
             logger.warning(f"没有设置数据库地址, 使用 {value['db_url']}")
 
-            if Path("db.sqlite3").exists():
-                logger.warning("使用了旧版 db.sqlite3")
-                logger.warning("为了防止数据丢失, 保留使用 db.sqlite3")
-                logger.warning(f'请将sqlite移到 {get_data_dir("") / "db.sqlite3"}')
-                value["db_url"] = "sqlite://db.sqlite3"
-
         return value
 
 
 plugin_config = Config.parse_obj(get_driver().config)
 DB_URL = plugin_config.db_url
```

### Comparing `nonebot_plugin_tortoise_orm-0.1.0/pyproject.toml` & `nonebot_plugin_tortoise_orm-0.1.0b2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-tortoise-orm"
-version = "0.1.0"
+version = "0.1.0.beta.2"
 description = "一个通用数据库连接插件"
 authors = [
     { name = "kexue", email = "xana278@foxmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-plugin-localstore>=0.5.0",
```

### Comparing `nonebot_plugin_tortoise_orm-0.1.0/PKG-INFO` & `nonebot_plugin_tortoise_orm-0.1.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tortoise-orm
-Version: 0.1.0
+Version: 0.1.0b2
 Summary: 一个通用数据库连接插件
 Home-page: https://github.com/kexue-z/nonebot-plugin-tortoise-orm
 Author-Email: kexue <xana278@foxmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/kexue-z/nonebot-plugin-tortoise-orm
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0
```

