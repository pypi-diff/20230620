# Comparing `tmp/playlisterutil-2.0.7.tar.gz` & `tmp/playlisterutil-2.0.8.tar.gz`

## Comparing `playlisterutil-2.0.7.tar` & `playlisterutil-2.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/src/playlisterUtil/__init__.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/src/playlisterUtil/playlisterUtil.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/src/playlisterUtil/setup.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/LICENSE
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/pyproject.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/src/playlisterUtil/__init__.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/src/playlisterUtil/playlisterUtil.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/src/playlisterUtil/setup.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/LICENSE
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 playlisterutil-2.0.8/PKG-INFO
```

### Comparing `playlisterutil-2.0.7/src/playlisterUtil/playlisterUtil.py` & `playlisterutil-2.0.8/src/playlisterUtil/playlisterUtil.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,34 +86,36 @@
 
     def __delitem__(self, key):
         raise KeyError("Cannot delete key-value pairs")
     
     def insert_one_mongo(self, collection, collection_id):
         collection[collection_id].insert_one(self.data)
 
-    def update_value_mongo(self, collection, collection_id, id, key, value):
+    def update_value_mongo(self, collection, collection_id, key, value):
         try:
             self.set_value(key, value)
         except KeyError:
             return False
         
         # Updating the whole document cannot be efficient right?
         res = collection[collection_id].update_one(
-            {'id': id},
+            {'id': self.data['id']},
             {'$set': self.data}
         )
 
         return res
 
-    def update_values_mongo(self, collection, collection_id, id):
+    def update_values_mongo(self, collection, collection_id):
         res = collection[collection_id].update_one(
-            {'id': id},
+            {'id': self.data['id']},
             {'$set': self.data}
         )
 
+        return res
+
     def get_keys(self):
         def _recursive_keys(dictionary, parent_key=''):
             keys = []
             for key, value in dictionary.items():
                 current_key = f'{parent_key}.{key}' if parent_key else key
                 if isinstance(value, dict):
                     keys.extend(_recursive_keys(value, current_key))
```

### Comparing `playlisterutil-2.0.7/.gitignore` & `playlisterutil-2.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `playlisterutil-2.0.7/LICENSE` & `playlisterutil-2.0.8/LICENSE`

 * *Files identical despite different names*

