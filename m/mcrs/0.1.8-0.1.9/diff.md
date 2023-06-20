# Comparing `tmp/mcrs-0.1.8.tar.gz` & `tmp/mcrs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcrs-0.1.8.tar", last modified: Sun Mar 19 19:04:43 2023, max compression
+gzip compressed data, was "mcrs-0.1.9.tar", last modified: Tue Jun 20 08:41:26 2023, max compression
```

## Comparing `mcrs-0.1.8.tar` & `mcrs-0.1.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 19:04:43.579216 mcrs-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-19 19:04:43.579216 mcrs-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-19 19:04:01.000000 mcrs-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 19:04:43.571215 mcrs-0.1.8/mcrs/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 19:04:43.575215 mcrs-0.1.8/mcrs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 19:04:43.575215 mcrs-0.1.8/mcrs/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 19:04:43.579216 mcrs-0.1.8/mcrs/environment/config/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/environment/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/environment/config/env_conf_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/environment/config/environment_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/environment/config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/environment/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/environment/imanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/environment/immutable_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/environment/lazy_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/environment/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/environment/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/execution_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/imicroservice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 19:04:43.579216 mcrs-0.1.8/mcrs/lifespan/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/lifespan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/lifespan/delayed_interrupt.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/lifespan/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/lifespan/test_delayed_interrupt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/os_info.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/python_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/resource_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-19 19:04:01.000000 mcrs-0.1.8/mcrs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 19:04:43.575215 mcrs-0.1.8/mcrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-19 19:04:43.000000 mcrs-0.1.8/mcrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-19 19:04:43.000000 mcrs-0.1.8/mcrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 19:04:43.000000 mcrs-0.1.8/mcrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 19:04:43.000000 mcrs-0.1.8/mcrs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-19 19:04:43.000000 mcrs-0.1.8/mcrs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-19 19:04:01.000000 mcrs-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 19:04:43.579216 mcrs-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-19 19:04:01.000000 mcrs-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:26.180360 mcrs-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-20 08:41:26.180360 mcrs-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 08:40:47.000000 mcrs-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:26.172360 mcrs-0.1.9/mcrs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:26.176360 mcrs-0.1.9/mcrs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:26.180360 mcrs-0.1.9/mcrs/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:26.180360 mcrs-0.1.9/mcrs/environment/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/environment/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/environment/config/env_conf_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/environment/config/environment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/environment/config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/environment/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/environment/imanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/environment/immutable_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/environment/lazy_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/environment/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/environment/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/imicroservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:26.180360 mcrs-0.1.9/mcrs/lifespan/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/lifespan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/lifespan/delayed_interrupt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/lifespan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/lifespan/test_delayed_interrupt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/os_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/python_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/resource_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-20 08:40:47.000000 mcrs-0.1.9/mcrs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:26.176360 mcrs-0.1.9/mcrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-20 08:41:26.000000 mcrs-0.1.9/mcrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-20 08:41:26.000000 mcrs-0.1.9/mcrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:41:26.000000 mcrs-0.1.9/mcrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:41:26.000000 mcrs-0.1.9/mcrs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 08:41:26.000000 mcrs-0.1.9/mcrs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-20 08:40:47.000000 mcrs-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:41:26.180360 mcrs-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-20 08:40:47.000000 mcrs-0.1.9/setup.py
```

### Comparing `mcrs-0.1.8/mcrs/__init__.py` & `mcrs-0.1.9/mcrs/__init__.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs/cli/main.py` & `mcrs-0.1.9/mcrs/cli/main.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs/environment/__init__.py` & `mcrs-0.1.9/mcrs/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs/environment/config/env_conf_value.py` & `mcrs-0.1.9/mcrs/environment/config/env_conf_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         self.validator = validator
         self.converter = converter
         self._loaded = False
         self._value = None
 
     def load_value(self, environment: IEnvironmentManager) -> None:
         loader = environment.get(self.key)
-        if self.optional is not None:
+        if self.optional is True:
             loader.optional()
         if self.validator is not None:
             loader.validator(self.validator)
         if self.converter is not None:
             loader.converter(self.converter)
         if self.default is not None:
             loader.default(self.default)
```

### Comparing `mcrs-0.1.8/mcrs/environment/config/environment_config.py` & `mcrs-0.1.9/mcrs/environment/config/environment_config.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs/environment/lazy_value.py` & `mcrs-0.1.9/mcrs/environment/lazy_value.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs/environment/manager.py` & `mcrs-0.1.9/mcrs/environment/manager.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs/execution_context.py` & `mcrs-0.1.9/mcrs/execution_context.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs/launcher.py` & `mcrs-0.1.9/mcrs/launcher.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs/lifespan/delayed_interrupt.py` & `mcrs-0.1.9/mcrs/lifespan/delayed_interrupt.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs/lifespan/test_delayed_interrupt.py` & `mcrs-0.1.9/mcrs/lifespan/test_delayed_interrupt.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs/network.py` & `mcrs-0.1.9/mcrs/network.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs/resource_limits.py` & `mcrs-0.1.9/mcrs/resource_limits.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs/utils.py` & `mcrs-0.1.9/mcrs/utils.py`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/mcrs.egg-info/SOURCES.txt` & `mcrs-0.1.9/mcrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcrs-0.1.8/setup.py` & `mcrs-0.1.9/setup.py`

 * *Files identical despite different names*

