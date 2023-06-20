# Comparing `tmp/playlisterutil-2.0.6.tar.gz` & `tmp/playlisterutil-2.0.7.tar.gz`

## Comparing `playlisterutil-2.0.6.tar` & `playlisterutil-2.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/src/playlisterUtil/__init__.py
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/src/playlisterUtil/playlisterUtil.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/src/playlisterUtil/setup.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/LICENSE
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/pyproject.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/src/playlisterUtil/__init__.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/src/playlisterUtil/playlisterUtil.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/src/playlisterUtil/setup.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/LICENSE
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/PKG-INFO
```

### Comparing `playlisterutil-2.0.6/src/playlisterUtil/playlisterUtil.py` & `playlisterutil-2.0.7/src/playlisterUtil/playlisterUtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,7 +139,11 @@
                         filtered_dict[key] = filtered_value
                 elif nested_key not in keys_to_filter:
                     filtered_dict[key] = value
             return filtered_dict
 
         stripped = _recursive_filter(self.data.copy())
         return stripped
+    
+    def filter_mongo_doc(dict):
+        dict.pop('_id')
+        return MongoDoc(dict)
```

### Comparing `playlisterutil-2.0.6/.gitignore` & `playlisterutil-2.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `playlisterutil-2.0.6/LICENSE` & `playlisterutil-2.0.7/LICENSE`

 * *Files identical despite different names*

