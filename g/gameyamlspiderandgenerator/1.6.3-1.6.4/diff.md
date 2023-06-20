# Comparing `tmp/gameyamlspiderandgenerator-1.6.3.tar.gz` & `tmp/gameyamlspiderandgenerator-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.6.3.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.6.4.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.6.3.tar` & `gameyamlspiderandgenerator-1.6.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1069 2023-06-17 07:02:01.936469 gameyamlspiderandgenerator-1.6.3/LICENSE
--rwxr-xr-x   0        0        0     1411 2023-06-20 08:04:11.255756 gameyamlspiderandgenerator-1.6.3/README.md
--rwxr-xr-x   0        0        0      568 2023-06-17 07:02:01.937320 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1908 2023-06-20 08:00:19.618735 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      675 2023-06-17 07:02:01.937746 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-06-17 07:02:01.938073 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      235 2023-06-17 07:02:01.938303 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0       56 2023-06-17 07:02:01.939367 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     3177 2023-06-17 07:02:01.939630 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7088 2023-06-17 07:02:01.939929 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7919 2023-06-17 07:02:01.940217 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-06-17 07:02:01.940509 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-06-17 07:02:01.940795 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1848 2023-06-17 07:02:01.941019 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-06-17 07:02:01.941257 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     2859 2023-06-18 00:42:23.550110 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2550 2023-06-20 07:58:45.635538 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      265 2023-06-17 07:02:01.942014 gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/util/thread.py
--rwxr-xr-x   0        0        0      765 2023-06-20 08:02:50.134003 gameyamlspiderandgenerator-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     2605 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.6.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-06-17 07:02:01.936469 gameyamlspiderandgenerator-1.6.4/LICENSE
+-rwxr-xr-x   0        0        0     1446 2023-06-20 08:26:16.341618 gameyamlspiderandgenerator-1.6.4/README.md
+-rwxr-xr-x   0        0        0      568 2023-06-17 07:02:01.937320 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1893 2023-06-20 08:31:40.549988 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      675 2023-06-17 07:02:01.937746 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-06-17 07:02:01.938073 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      235 2023-06-17 07:02:01.938303 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0       56 2023-06-17 07:02:01.939367 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     3177 2023-06-17 07:02:01.939630 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7088 2023-06-17 07:02:01.939929 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7919 2023-06-17 07:02:01.940217 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-06-17 07:02:01.940509 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-06-17 07:02:01.940795 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1848 2023-06-17 07:02:01.941019 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-06-17 07:02:01.941257 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     2609 2023-06-20 08:33:33.143165 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2550 2023-06-20 07:58:45.635538 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      265 2023-06-17 07:02:01.942014 gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/util/thread.py
+-rwxr-xr-x   0        0        0      766 2023-06-20 08:34:14.800637 gameyamlspiderandgenerator-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0     2640 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.6.4/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.6.3/LICENSE` & `gameyamlspiderandgenerator-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.3/README.md` & `gameyamlspiderandgenerator-1.6.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # - openai
 # if you don't want to set proxy, please fill in {}
 proxy: { }
 # http: socks5://127.0.0.1:7891
 # https: socks5://127.0.0.1:7891
 gitToken: 'your token'
 api:
-  google-play: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
+  google-play: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90 # Get your api key via serpapi.com
   apple: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
   openai: yourkey
 
 ```
 ## Try to make yaml data file
 ```bash
  python3.10 -m gameyamlspiderandgenerator -f /home/user/desktop/config.yaml  https://store.steampowered.com/app/290340/Armello/ -o 1.zip
```

### Comparing `gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     with open(args.config) as f:
         setting = safe_load(f)
 else:
     setting = args.config
 if args.fast:
     setting['hook'] = None
 config.update(setting)
-pkg.__init__()
 yml = produce_yaml(args.url)
 if args.output is None:
     print(yml)
 elif "." not in args.output:
     if args.output == "zip":
         with open(get_valid_filename(yml.raw_dict['name']) + ".zip", 'wb') as f:
             f.write(bytes(yml))
```

### Comparing `gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,24 +33,21 @@
         base = __package__.split(".")[0] + "." + _dir
         for plugin in getattr(config, _dir, []):
             if plugin.startswith("_"):
                 logger.warning(f"Skip loading protected {_dir} {plugin}")
                 continue
             try:
                 package = f"{base}.{plugin}"
-                if plugin in self["log"]:
-                    continue
                 logger.info(f"Loading {_dir}: {plugin}")
                 temp = importlib.import_module(package)
                 self[_dir][plugin] = [
                     o
                     for o in temp.__dict__.values()
                     if isinstance(o, type) and issubclass(o, _type) and o is not _type
                 ][-1]
-                self["log"].append(temp.__name__.split(".")[-1])
             except ImportError as e:
                 logger.trace(e)
                 logger.error(f"Failed to import {_dir}: {plugin}")
             except IndexError:
                 logger.error(f"Imported {_dir} but no {_type.__name__} found: {plugin}")
 
     def load_plugins(self):
@@ -60,18 +57,15 @@
         if config["hook"] is None:
             if None not in self["log"]:
                 logger.warning(f"All hooks are disabled")
                 self["log"].append(None)
             return
         for plugin in getattr(config, "hook", []):
             try:
-                if plugin in self["log"]:
-                    continue
                 logger.info(f"Loading hook: {plugin}")
-                self["log"].append(plugin)
                 temp = importlib.import_module(f"yamlgenerator_hook_{plugin}")
                 self["hook"][plugin] = [
                     o
                     for o in temp.__dict__.values()
                     if isinstance(o, type) and issubclass(o, BaseHook) and o is not BaseHook
                 ][-1]
             except ImportError as e:
```

### Comparing `gameyamlspiderandgenerator-1.6.3/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.6.4/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.3/pyproject.toml` & `gameyamlspiderandgenerator-1.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.6.3"
+version = "1.6.4"
 description = "A useful tool for generating Furrygameindex yaml files"
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -22,13 +22,14 @@
 pyyaml = "^6.0"
 pysocks = "^1.7.1"
 lxml = "^4.9.2"
 py3langid = "^0.2.2"
 yamlgenerator-hook-validate = "^0.1.0"
 yamlgenerator-hook-search = "^0.1.0"
 
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `gameyamlspiderandgenerator-1.6.3/PKG-INFO` & `gameyamlspiderandgenerator-1.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.6.3
+Version: 1.6.4
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -48,15 +48,15 @@
 # - openai
 # if you don't want to set proxy, please fill in {}
 proxy: { }
 # http: socks5://127.0.0.1:7891
 # https: socks5://127.0.0.1:7891
 gitToken: 'your token'
 api:
-  google-play: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
+  google-play: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90 # Get your api key via serpapi.com
   apple: a714b00383f0662a61b2e382d55c685f17015617aa7048972da58a756fb75e90
   openai: yourkey
 
 ```
 ## Try to make yaml data file
 ```bash
  python3.10 -m gameyamlspiderandgenerator -f /home/user/desktop/config.yaml  https://store.steampowered.com/app/290340/Armello/ -o 1.zip
```

