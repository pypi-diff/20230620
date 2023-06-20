# Comparing `tmp/bev-0.8.0.tar.gz` & `tmp/bev-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bev-0.8.0.tar", last modified: Wed May 17 14:15:25 2023, max compression
+gzip compressed data, was "bev-0.8.1.tar", last modified: Tue Jun 20 16:08:58 2023, max compression
```

## Comparing `bev-0.8.0.tar` & `bev-0.8.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:25.972943 bev-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-05-17 14:15:21.000000 bev-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-17 14:15:21.000000 bev-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-17 14:15:25.972943 bev-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-17 14:15:21.000000 bev-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:25.968943 bev-0.8.0/bev/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-17 14:15:21.000000 bev-0.8.0/bev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-17 14:15:21.000000 bev-0.8.0/bev/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:25.972943 bev-0.8.0/bev/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/blame.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-17 14:15:21.000000 bev-0.8.0/bev/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:25.972943 bev-0.8.0/bev/config/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-17 14:15:21.000000 bev-0.8.0/bev/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-17 14:15:21.000000 bev-0.8.0/bev/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-17 14:15:21.000000 bev-0.8.0/bev/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-17 14:15:21.000000 bev-0.8.0/bev/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-17 14:15:21.000000 bev-0.8.0/bev/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-17 14:15:21.000000 bev-0.8.0/bev/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-17 14:15:21.000000 bev-0.8.0/bev/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-17 14:15:21.000000 bev-0.8.0/bev/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:21.000000 bev-0.8.0/bev/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-17 14:15:21.000000 bev-0.8.0/bev/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-17 14:15:21.000000 bev-0.8.0/bev/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-17 14:15:21.000000 bev-0.8.0/bev/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-17 14:15:21.000000 bev-0.8.0/bev/vc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-17 14:15:21.000000 bev-0.8.0/bev/wc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 14:15:25.968943 bev-0.8.0/bev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-17 14:15:25.000000 bev-0.8.0/bev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-17 14:15:25.000000 bev-0.8.0/bev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 14:15:25.000000 bev-0.8.0/bev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 14:15:25.000000 bev-0.8.0/bev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 14:15:25.000000 bev-0.8.0/bev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 14:15:25.000000 bev-0.8.0/bev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-17 14:15:21.000000 bev-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 14:15:21.000000 bev-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 14:15:25.972943 bev-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-17 14:15:21.000000 bev-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:58.763427 bev-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-20 16:08:52.000000 bev-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 16:08:52.000000 bev-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-20 16:08:58.763427 bev-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-20 16:08:52.000000 bev-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:58.763427 bev-0.8.1/bev/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 16:08:52.000000 bev-0.8.1/bev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 16:08:52.000000 bev-0.8.1/bev/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:58.763427 bev-0.8.1/bev/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/blame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:58.763427 bev-0.8.1/bev/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-20 16:08:52.000000 bev-0.8.1/bev/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-20 16:08:52.000000 bev-0.8.1/bev/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-20 16:08:52.000000 bev-0.8.1/bev/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-20 16:08:52.000000 bev-0.8.1/bev/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-20 16:08:52.000000 bev-0.8.1/bev/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-20 16:08:52.000000 bev-0.8.1/bev/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-20 16:08:52.000000 bev-0.8.1/bev/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:52.000000 bev-0.8.1/bev/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-20 16:08:52.000000 bev-0.8.1/bev/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-20 16:08:52.000000 bev-0.8.1/bev/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-20 16:08:52.000000 bev-0.8.1/bev/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-20 16:08:52.000000 bev-0.8.1/bev/vc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-20 16:08:52.000000 bev-0.8.1/bev/wc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:58.763427 bev-0.8.1/bev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-20 16:08:58.000000 bev-0.8.1/bev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-20 16:08:58.000000 bev-0.8.1/bev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:08:58.000000 bev-0.8.1/bev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 16:08:58.000000 bev-0.8.1/bev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 16:08:58.000000 bev-0.8.1/bev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 16:08:58.000000 bev-0.8.1/bev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-20 16:08:52.000000 bev-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 16:08:52.000000 bev-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:08:58.763427 bev-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-20 16:08:52.000000 bev-0.8.1/setup.py
```

### Comparing `bev-0.8.0/LICENSE` & `bev-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/PKG-INFO` & `bev-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bev
-Version: 0.8.0
+Version: 0.8.1
 Summary: A small manager for versioned data
 Home-page: https://github.com/neuro-ml/bev
 License: MIT
-Download-URL: https://github.com/neuro-ml/bev/archive/v0.8.0.tar.gz
+Download-URL: https://github.com/neuro-ml/bev/archive/v0.8.1.tar.gz
 Keywords: data,version control
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `bev-0.8.0/README.md` & `bev-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/cli/add.py` & `bev-0.8.1/bev/cli/add.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/cli/app.py` & `bev-0.8.1/bev/cli/app.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/cli/blame.py` & `bev-0.8.1/bev/cli/blame.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/cli/fetch.py` & `bev-0.8.1/bev/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/cli/init.py` & `bev-0.8.1/bev/cli/init.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/cli/pull.py` & `bev-0.8.1/bev/cli/pull.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/cli/storage.py` & `bev-0.8.1/bev/cli/storage.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/cli/update.py` & `bev-0.8.1/bev/cli/update.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/cli/utils.py` & `bev-0.8.1/bev/cli/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/config/base.py` & `bev-0.8.1/bev/config/base.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/config/hostname.py` & `bev-0.8.1/bev/config/hostname.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/config/include.py` & `bev-0.8.1/bev/config/include.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/config/parse.py` & `bev-0.8.1/bev/config/parse.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/config/registry.py` & `bev-0.8.1/bev/config/registry.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/config/remote.py` & `bev-0.8.1/bev/config/remote.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/config/utils.py` & `bev-0.8.1/bev/config/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/hash.py` & `bev-0.8.1/bev/hash.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/interface.py` & `bev-0.8.1/bev/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from .hash import Key, is_hash, is_tree, load_key, load_tree, strip_tree, to_hash
 from .local import Local
 from .utils import PathOrStr
 from .vc import VC, CommittedVersion, SubprocessGit, Version
 from .wc import BevLocalGlob, BevVCGlob
 
 
+_NoArg = object()
+
+
 class Repository:
     """
     Interface that represents a `bev` repository.
 
     Parameters
     ----------
     root:
@@ -40,14 +43,24 @@
         self.root = Path(*root)
         self.prefix = Path()
         self.storage, self.cache = build_storage(self.root)
         self.vc: VC = SubprocessGit(self.root)
         self.fetch, self.version, self.check = fetch, version, check
         self._cache = {}
 
+    def copy(self, fetch: bool = _NoArg, version: Optional[Version] = _NoArg, check: bool = _NoArg,
+             prefix: PathOrStr = _NoArg, cache: dict = _NoArg):
+        result = type(self)(
+            self.root, fetch=_resolve_arg(self.fetch, fetch), version=_resolve_arg(self.version, version),
+            check=_resolve_arg(self.check, check),
+        )
+        result.prefix = Path(_resolve_arg(self.prefix, prefix))
+        result._cache = _resolve_arg(self._cache, cache)
+        return result
+
     @classmethod
     def from_here(cls, *relative: PathOrStr, fetch: bool = True, version: Optional[Version] = None,
                   check: Optional[bool] = None) -> 'Repository':
         """
         Creates a repository with a path `relative` to the file in which this method is called.
 
         Examples
@@ -201,19 +214,16 @@
     # navigation
 
     def __truediv__(self, other: PathOrStr):
         other = Path(other)
         if other.is_absolute():
             raise ValueError('Only relative paths are supported')
 
-        child = Repository(self.root, fetch=self.fetch, version=self.version, check=self.check)
-        # FIXME
-        child.prefix = self.prefix / other
-        child._cache = self._cache
-        return child
+        prefix = self.prefix / other
+        return self.copy(prefix=prefix)
 
     @property
     def path(self):
         return self.root / self.prefix
 
     # internal logic
 
@@ -285,7 +295,11 @@
 
     @staticmethod
     def _expand_folders(tree) -> set:
         result = set(tree)
         for file in tree:
             result.update(map(str, list(Path(file).parents)[:-1]))
         return result
+
+
+def _resolve_arg(x, y):
+    return x if y is _NoArg else y
```

### Comparing `bev-0.8.0/bev/ops.py` & `bev-0.8.1/bev/ops.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/shortcuts.py` & `bev-0.8.1/bev/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/testing.py` & `bev-0.8.1/bev/testing.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/utils.py` & `bev-0.8.1/bev/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/vc.py` & `bev-0.8.1/bev/vc.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev/wc.py` & `bev-0.8.1/bev/wc.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/bev.egg-info/PKG-INFO` & `bev-0.8.1/bev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bev
-Version: 0.8.0
+Version: 0.8.1
 Summary: A small manager for versioned data
 Home-page: https://github.com/neuro-ml/bev
 License: MIT
-Download-URL: https://github.com/neuro-ml/bev/archive/v0.8.0.tar.gz
+Download-URL: https://github.com/neuro-ml/bev/archive/v0.8.1.tar.gz
 Keywords: data,version control
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `bev-0.8.0/bev.egg-info/SOURCES.txt` & `bev-0.8.1/bev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/pyproject.toml` & `bev-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bev-0.8.0/setup.py` & `bev-0.8.1/setup.py`

 * *Files identical despite different names*

