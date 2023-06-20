# Comparing `tmp/gameyamlspiderandgenerator-1.6.5.tar.gz` & `tmp/gameyamlspiderandgenerator-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.6.5.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.6.6.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.6.5.tar` & `gameyamlspiderandgenerator-1.6.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1069 2023-06-17 07:02:01.936469 gameyamlspiderandgenerator-1.6.5/LICENSE
--rwxr-xr-x   0        0        0     1446 2023-06-20 08:26:16.341618 gameyamlspiderandgenerator-1.6.5/README.md
--rwxr-xr-x   0        0        0      568 2023-06-17 07:02:01.937320 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1871 2023-06-20 09:25:47.496894 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      675 2023-06-17 07:02:01.937746 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-06-17 07:02:01.938073 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      235 2023-06-17 07:02:01.938303 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0       56 2023-06-17 07:02:01.939367 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     3177 2023-06-20 08:55:31.013097 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7088 2023-06-17 07:02:01.939929 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7919 2023-06-17 07:02:01.940217 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-06-17 07:02:01.940509 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-06-17 07:02:01.940795 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1848 2023-06-17 07:02:01.941019 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-06-17 07:02:01.941257 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     2855 2023-06-20 09:27:12.882725 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2550 2023-06-20 07:58:45.635538 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      265 2023-06-17 07:02:01.942014 gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/util/thread.py
--rwxr-xr-x   0        0        0      766 2023-06-20 09:28:58.110713 gameyamlspiderandgenerator-1.6.5/pyproject.toml
--rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.6.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-06-17 07:02:01.936469 gameyamlspiderandgenerator-1.6.6/LICENSE
+-rwxr-xr-x   0        0        0     1446 2023-06-20 08:26:16.341618 gameyamlspiderandgenerator-1.6.6/README.md
+-rwxr-xr-x   0        0        0      568 2023-06-17 07:02:01.937320 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1888 2023-06-20 09:36:24.142803 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      675 2023-06-17 07:02:01.937746 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-06-17 07:02:01.938073 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      235 2023-06-17 07:02:01.938303 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0       56 2023-06-17 07:02:01.939367 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     3177 2023-06-20 08:55:31.013097 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7088 2023-06-17 07:02:01.939929 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7919 2023-06-17 07:02:01.940217 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-06-17 07:02:01.940509 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-06-17 07:02:01.940795 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1816 2023-06-20 09:35:26.330476 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-06-17 07:02:01.941257 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     2846 2023-06-20 09:36:24.047081 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2550 2023-06-20 07:58:45.635538 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      265 2023-06-17 07:02:01.942014 gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/thread.py
+-rwxr-xr-x   0        0        0      766 2023-06-20 09:36:44.110154 gameyamlspiderandgenerator-1.6.6/pyproject.toml
+-rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.6.6/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.6.5/LICENSE` & `gameyamlspiderandgenerator-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.5/README.md` & `gameyamlspiderandgenerator-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from yaml import safe_load
 
 from .util.config import config
 from .util.fgi import default_config
 from .util.fgi_yaml import get_valid_filename
 from .util.plugin_manager import pkg
-import sys
 from loguru import logger
 from gameyamlspiderandgenerator import produce_yaml
 
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "-f",
     "--config",
@@ -40,15 +39,16 @@
     setting = args.config
 if args.fast:
     setting['hook'] = None
 config.update(setting)
 pkg.__init__()
 yml = produce_yaml(args.url)
 if args.output is None:
-    print(yml)
+    if yml is not None:
+        print(yml)
 elif "." not in args.output:
     if args.output == "zip":
         with open(get_valid_filename(yml.raw_dict['name']) + ".zip", 'wb') as f:
             f.write(bytes(yml))
     elif args.output == "yaml":
         with open(get_valid_filename(yml.raw_dict['name']) + ".yaml", 'w') as f:
             f.write(str(yml))
```

### Comparing `gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/fgi.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,16 +38,15 @@
         "match": "(https://weibo.com/u/.+)",
         "prefix": ".weibo",
         "replace": "\\g<1>",
     },
 ]
 default_config = {'api': {'apple': 'a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90',
                           'google-play': 'a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90'},
-                  'gitToken': 'your token',
-                  'hook': ['search'],
+                  'hook': ['search', 'validate'],
                   'plugin': ['steam', 'itchio'],
                   'proxy': {}}
 template_dict = {
     "name": 'NAME',
     "brief-description": 'BRIEF-DESC',
     "description": 'DESC',
     "description-format": "markdown",
```

### Comparing `gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,21 +54,21 @@
                 logger.error(f"Imported {_dir} but no {_type.__name__} found: {plugin}")
 
     def load_plugins(self):
         self._load("plugin", BasePlugin)
 
     def load_hooks(self):
         if config["hook"] is None:
-            if None not in self["log"]:
+            if None not in self.log:
                 logger.warning(f"All hooks are disabled")
-                self["log"].append(None)
+                self.log.append(None)
             return
         for plugin in getattr(config, "hook", []):
             try:
-                if plugin in self["log"]:
+                if plugin in self.log:
                     continue
                 logger.info(f"Loading hook: {plugin}")
                 self["log"].append(plugin)
                 temp = importlib.import_module(f"yamlgenerator_hook_{plugin}")
                 self["hook"][plugin] = [
                     o
                     for o in temp.__dict__.values()
```

### Comparing `gameyamlspiderandgenerator-1.6.5/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.6.6/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.5/pyproject.toml` & `gameyamlspiderandgenerator-1.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.6.5"
+version = "1.6.6"
 description = "A useful tool for generating Furrygameindex yaml files"
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gameyamlspiderandgenerator-1.6.5/PKG-INFO` & `gameyamlspiderandgenerator-1.6.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.6.5
+Version: 1.6.6
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

