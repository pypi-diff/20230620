# Comparing `tmp/playlisterutil-2.0.4.tar.gz` & `tmp/playlisterutil-2.0.5.tar.gz`

## Comparing `playlisterutil-2.0.4.tar` & `playlisterutil-2.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-2.0.4/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-2.0.4/src/playlisterUtil/__init__.py
--rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 playlisterutil-2.0.4/src/playlisterUtil/playlisterUtil.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-2.0.4/src/playlisterUtil/setup.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-2.0.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-2.0.4/LICENSE
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-2.0.4/pyproject.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/src/playlisterUtil/__init__.py
+-rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/src/playlisterUtil/playlisterUtil.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/src/playlisterUtil/setup.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/LICENSE
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-2.0.5/PKG-INFO
```

### Comparing `playlisterutil-2.0.4/src/playlisterUtil/playlisterUtil.py` & `playlisterutil-2.0.5/src/playlisterUtil/playlisterUtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,17 @@
             # 0 not processed, 1 in process, 2 processed
             'processed': 0,
             # 0 didn't succeed, 1 succeed
             'success': 0,
             'retries': 0
         }
 
+    def __init__(self, dict):
+        self.data = dict
+
     def get_value(self, key, default=None):
         keys = key.split('.')
         value = self.data
         for k in keys:
             value = value.get(k)
             if value is None:
                 return default
```

### Comparing `playlisterutil-2.0.4/.gitignore` & `playlisterutil-2.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `playlisterutil-2.0.4/LICENSE` & `playlisterutil-2.0.5/LICENSE`

 * *Files identical despite different names*

