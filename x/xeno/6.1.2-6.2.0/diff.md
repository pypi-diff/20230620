# Comparing `tmp/xeno-6.1.2.tar.gz` & `tmp/xeno-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeno-6.1.2.tar", last modified: Wed May 24 16:28:40 2023, max compression
+gzip compressed data, was "xeno-6.2.0.tar", last modified: Tue Jun 20 01:23:36 2023, max compression
```

## Comparing `xeno-6.1.2.tar` & `xeno-6.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-24 16:28:40.918533 xeno-6.1.2/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-02-22 19:19:33.000000 xeno-6.1.2/LICENSE
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-02-22 19:19:33.000000 xeno-6.1.2/MANIFEST.in
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-05-24 16:28:40.918533 xeno-6.1.2/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-02-22 19:19:33.000000 xeno-6.1.2/README.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-24 16:28:40.918533 xeno-6.1.2/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1160 2023-05-24 16:28:25.000000 xeno-6.1.2/setup.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-24 16:28:40.918533 xeno-6.1.2/xeno/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-05-24 16:26:11.000000 xeno-6.1.2/xeno/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/abstract.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/async_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/attributes.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19488 2023-05-24 16:26:03.000000 xeno-6.1.2/xeno/build.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5004 2023-05-01 08:08:44.000000 xeno-6.1.2/xeno/color.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10217 2023-05-24 16:25:54.000000 xeno-6.1.2/xeno/cookbook.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/decorators.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-02-22 19:19:33.000000 xeno-6.1.2/xeno/errors.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7250 2023-05-01 07:35:53.000000 xeno-6.1.2/xeno/events.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-02-22 19:19:33.000000 xeno-6.1.2/xeno/namespaces.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-03-04 18:15:00.000000 xeno-6.1.2/xeno/pkg_config.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    25812 2023-05-24 16:14:14.000000 xeno-6.1.2/xeno/recipe.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7140 2023-05-01 08:08:44.000000 xeno-6.1.2/xeno/shell.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2056 2023-05-01 08:08:44.000000 xeno-6.1.2/xeno/spinner.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/sync_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/testing.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3258 2023-04-25 17:49:02.000000 xeno-6.1.2/xeno/utils.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-24 16:28:40.918533 xeno-6.1.2/xeno.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-05-24 16:28:40.000000 xeno-6.1.2/xeno.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-05-24 16:28:40.000000 xeno-6.1.2/xeno.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-24 16:28:40.000000 xeno-6.1.2/xeno.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-05-24 16:28:40.000000 xeno-6.1.2/xeno.egg-info/top_level.txt
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-06-20 01:23:36.169479 xeno-6.2.0/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-02-22 19:19:33.000000 xeno-6.2.0/LICENSE
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-02-22 19:19:33.000000 xeno-6.2.0/MANIFEST.in
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-06-20 01:23:36.169479 xeno-6.2.0/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-02-22 19:19:33.000000 xeno-6.2.0/README.md
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-06-20 01:23:36.169479 xeno-6.2.0/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1160 2023-05-31 16:32:48.000000 xeno-6.2.0/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-06-20 01:23:36.169479 xeno-6.2.0/xeno/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-05-24 16:26:11.000000 xeno-6.2.0/xeno/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-25 17:49:02.000000 xeno-6.2.0/xeno/abstract.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-25 17:49:02.000000 xeno-6.2.0/xeno/async_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-25 17:49:02.000000 xeno-6.2.0/xeno/attributes.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    20234 2023-05-31 16:48:30.000000 xeno-6.2.0/xeno/build.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5004 2023-05-01 08:08:44.000000 xeno-6.2.0/xeno/color.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10217 2023-05-24 16:25:54.000000 xeno-6.2.0/xeno/cookbook.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-25 17:49:02.000000 xeno-6.2.0/xeno/decorators.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-02-22 19:19:33.000000 xeno-6.2.0/xeno/errors.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7250 2023-05-01 07:35:53.000000 xeno-6.2.0/xeno/events.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-02-22 19:19:33.000000 xeno-6.2.0/xeno/namespaces.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-03-04 18:15:00.000000 xeno-6.2.0/xeno/pkg_config.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    25909 2023-05-31 16:50:00.000000 xeno-6.2.0/xeno/recipe.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7140 2023-05-01 08:08:44.000000 xeno-6.2.0/xeno/shell.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2056 2023-05-01 08:08:44.000000 xeno-6.2.0/xeno/spinner.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-25 17:49:02.000000 xeno-6.2.0/xeno/sync_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-25 17:49:02.000000 xeno-6.2.0/xeno/testing.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3258 2023-04-25 17:49:02.000000 xeno-6.2.0/xeno/utils.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-06-20 01:23:36.169479 xeno-6.2.0/xeno.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-06-20 01:23:36.000000 xeno-6.2.0/xeno.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-06-20 01:23:36.000000 xeno-6.2.0/xeno.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-06-20 01:23:36.000000 xeno-6.2.0/xeno.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-06-20 01:23:36.000000 xeno-6.2.0/xeno.egg-info/top_level.txt
```

### Comparing `xeno-6.1.2/LICENSE` & `xeno-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/PKG-INFO` & `xeno-6.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 6.1.2
+Version: 6.2.0
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: IOC dependency injector
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xeno-6.1.2/README.md` & `xeno-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/setup.py` & `xeno-6.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="xeno",
-    version="6.1.2",
+    version="6.2.0",
     description="The Python dependency injector from outer space.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/xeno",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
```

### Comparing `xeno-6.1.2/xeno/__init__.py` & `xeno-6.2.0/xeno/__init__.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/abstract.py` & `xeno-6.2.0/xeno/abstract.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/async_injector.py` & `xeno-6.2.0/xeno/async_injector.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/attributes.py` & `xeno-6.2.0/xeno/attributes.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/build.py` & `xeno-6.2.0/xeno/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 #
 # Author: Lain Musgrove (lain.proliant@gmail.com)
 # Date: Friday March 17, 2023
 #
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 
-import fnmatch
 import asyncio
+import fnmatch
 import multiprocessing
 import sys
+import traceback
 from argparse import ArgumentParser, HelpFormatter
 from collections import defaultdict
 from typing import Any, Callable, Iterable, Optional, cast
 
 from xeno.async_injector import AsyncInjector
 from xeno.attributes import MethodAttributes
 from xeno.color import TextDecorator
@@ -43,14 +44,15 @@
         REBUILD = "rebuild"
         TREE = "tree"
 
     class CleanupMode:
         NONE = "none"
         SHALLOW = "shallow"
         RECURSIVE = "recursive"
+        RECURSIVE_WITH_DEPS = "recursive_with_deps"
 
     class ColorOptions:
         YES = "yes"
         NO = "no"
         AUTO = "auto"
 
     class SortingHelpFormatter(HelpFormatter):
@@ -90,15 +92,23 @@
         )
         parser.add_argument(
             "--clean",
             "-c",
             dest="cleanup_mode",
             action="store_const",
             const=self.CleanupMode.RECURSIVE,
-            help="Clean the specified or default targets and their components.",
+            help="Clean the specified or default targets and all their components.",
+        )
+        parser.add_argument(
+            "--full-clean",
+            "-C",
+            dest="cleanup_mode",
+            action="store_const",
+            const=self.CleanupMode.RECURSIVE_WITH_DEPS,
+            help="Clean the specified or default targets and all their components and dependencies.",
         )
         parser.add_argument(
             "--cut",
             "-x",
             dest="cleanup_mode",
             action="store_const",
             const=self.CleanupMode.SHALLOW,
@@ -363,14 +373,20 @@
             case Config.CleanupMode.SHALLOW:
                 return await asyncio.gather(*[task.clean() for task in tasks])
             case Config.CleanupMode.RECURSIVE:
                 return await asyncio.gather(
                     *[task.clean() for task in tasks],
                     *[task.clean_components(recursive=True) for task in tasks],
                 )
+            case Config.CleanupMode.RECURSIVE_WITH_DEPS:
+                return await asyncio.gather(
+                    *[task.clean() for task in tasks],
+                    *[task.clean_components(recursive=True) for task in tasks],
+                    *[task.clean_deps() for task in tasks],
+                )
             case _:
                 raise ValueError("Config.cleanup_mode not specified.")
 
     async def _print_help(self, config: Config, tasks: Iterable[Recipe]):
         parser = config._argparser()
 
         self.txt(f"# {self.name}")
@@ -454,15 +470,15 @@
             Shell.set_max_jobs(max_jobs)
             bus.shutdown()
 
     async def _build_loop(self, bus, config: Config):
         result, _ = await asyncio.gather(self.build_async(config), bus.run())
         return result
 
-    def build(self, *argv, raise_errors=True):
+    def build(self, *argv, raise_errors=False):
         config = Config().parse_args(*argv)
 
         match config.color:
             case Config.ColorOptions.YES:
                 enable_color()
             case Config.ColorOptions.NO:
                 disable_color()
@@ -473,14 +489,16 @@
             with EventBus.session():
                 bus = EventBus.get()
                 for hook in self.bus_hooks:
                     hook(config, self, bus)
                 return asyncio.run(self._build_loop(bus, config))
 
         except BuildError as e:
+            if config.debug:
+                traceback.print_exc()
             if raise_errors:
                 raise e
 
 
 # --------------------------------------------------------------------
 class DefaultEngineHook:
     def __init__(self):
@@ -578,8 +596,8 @@
 recipe = engine.recipe
 factory = engine.factory
 task = engine.task
 
 
 # --------------------------------------------------------------------
 def build():
-    return engine.build(*sys.argv[1:], raise_errors=False)
+    return engine.build(*sys.argv[1:])
```

### Comparing `xeno-6.1.2/xeno/color.py` & `xeno-6.2.0/xeno/color.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/cookbook.py` & `xeno-6.2.0/xeno/cookbook.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/decorators.py` & `xeno-6.2.0/xeno/decorators.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/errors.py` & `xeno-6.2.0/xeno/errors.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/events.py` & `xeno-6.2.0/xeno/events.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/namespaces.py` & `xeno-6.2.0/xeno/namespaces.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/pkg_config.py` & `xeno-6.2.0/xeno/pkg_config.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/recipe.py` & `xeno-6.2.0/xeno/recipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -525,14 +525,16 @@
             return timedelta.max
         else:
             return min(max(c.age(ref), c.inputs_age(ref)) for c in self.components())
 
     def add_dependency(self, dep: "Recipe"):
         assert isinstance(dep, Recipe), f"Value `{dep}` is not a recipe."
         self._deps.append(dep)
+        for component in self.components():
+            component.add_dependency(dep)
 
     def dependencies(self) -> Generator["Recipe", None, None]:
         yield from self._deps
         if self.has_parent():
             yield from self.parent.dependencies()
 
     def dependencies_age(self, ref: datetime) -> timedelta:
@@ -613,25 +615,31 @@
             )
         exceptions = [e for e in results if isinstance(e, Exception)]
         if exceptions:
             raise self.composite_error(
                 exceptions, "Failed to clean one or more components."
             )
 
+    async def clean_deps(self):
+        deps = [*self.dependencies()]
+        results = await asyncio.gather(
+
+        )
+
     async def make_dependencies(self):
         recipes = [*self.dependencies()]
         if self.sync:
             for c in recipes:
                 try:
-                    await c(skiplock=True)
+                    await c()
                 except Exception as e:
                     raise self.error("Failed to make a dependency.") from e
         else:
             results = await asyncio.gather(
-                *(c(skiplock=True) for c in recipes), return_exceptions=True
+                *(c() for c in recipes), return_exceptions=True
             )
             exceptions = [e for e in results if isinstance(e, Exception)]
             if exceptions:
                 raise self.composite_error(
                     exceptions, "Failed to make one or more dependencies."
                 )
 
@@ -722,18 +730,15 @@
 
         if not self.done():
             self.saved_result = None
             raise self.error("Recipe make() didn't complete successfully.")
 
         return result
 
-    async def __call__(self, skiplock=False):
-        if self.lock.locked() and skiplock:
-            return None
-
+    async def __call__(self):
         async with self.lock:
             if self.done():
                 if self.has_target():
                     return self.target
                 elif self.memoize:
                     return self.saved_result
```

### Comparing `xeno-6.1.2/xeno/shell.py` & `xeno-6.2.0/xeno/shell.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/spinner.py` & `xeno-6.2.0/xeno/spinner.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/sync_injector.py` & `xeno-6.2.0/xeno/sync_injector.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/testing.py` & `xeno-6.2.0/xeno/testing.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno/utils.py` & `xeno-6.2.0/xeno/utils.py`

 * *Files identical despite different names*

### Comparing `xeno-6.1.2/xeno.egg-info/PKG-INFO` & `xeno-6.2.0/xeno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 6.1.2
+Version: 6.2.0
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: IOC dependency injector
 Classifier: Development Status :: 5 - Production/Stable
```

