# Comparing `tmp/d-popcorn-1.1.0.tar.gz` & `tmp/d-popcorn-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d-popcorn-1.1.0.tar", last modified: Fri Jun  2 08:35:40 2023, max compression
+gzip compressed data, was "d-popcorn-1.1.2.tar", last modified: Tue Jun 20 12:46:25 2023, max compression
```

## Comparing `d-popcorn-1.1.0.tar` & `d-popcorn-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-06-02 08:35:40.897526 d-popcorn-1.1.0/
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     1069 2023-04-12 09:35:52.000000 d-popcorn-1.1.0/LICENSE
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      492 2023-06-02 08:35:40.897526 d-popcorn-1.1.0/PKG-INFO
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     3060 2023-06-02 08:27:50.000000 d-popcorn-1.1.0/README.md
-drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-06-02 08:35:40.897526 d-popcorn-1.1.0/d_popcorn.egg-info/
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      492 2023-06-02 08:35:40.000000 d-popcorn-1.1.0/d_popcorn.egg-info/PKG-INFO
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      306 2023-06-02 08:35:40.000000 d-popcorn-1.1.0/d_popcorn.egg-info/SOURCES.txt
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        1 2023-06-02 08:35:40.000000 d-popcorn-1.1.0/d_popcorn.egg-info/dependency_links.txt
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       53 2023-06-02 08:35:40.000000 d-popcorn-1.1.0/d_popcorn.egg-info/entry_points.txt
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        6 2023-06-02 08:35:40.000000 d-popcorn-1.1.0/d_popcorn.egg-info/requires.txt
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        8 2023-06-02 08:35:40.000000 d-popcorn-1.1.0/d_popcorn.egg-info/top_level.txt
-drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-06-02 08:35:40.897526 d-popcorn-1.1.0/popcorn/
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       22 2023-06-02 08:34:11.000000 d-popcorn-1.1.0/popcorn/__init__.py
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     6627 2023-06-02 08:29:15.000000 d-popcorn-1.1.0/popcorn/dump.py
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)    15287 2023-06-02 08:29:16.000000 d-popcorn-1.1.0/popcorn/popcornS3.py
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     4595 2023-06-02 08:29:16.000000 d-popcorn-1.1.0/popcorn/popcorn_cli.py
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       38 2023-06-02 08:35:40.897526 d-popcorn-1.1.0/setup.cfg
--rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     1060 2023-06-02 08:29:16.000000 d-popcorn-1.1.0/setup.py
+drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-06-20 12:46:25.542868 d-popcorn-1.1.2/
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     1069 2023-04-12 09:35:52.000000 d-popcorn-1.1.2/LICENSE
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      492 2023-06-20 12:46:25.542868 d-popcorn-1.1.2/PKG-INFO
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     3060 2023-06-02 08:27:50.000000 d-popcorn-1.1.2/README.md
+drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-06-20 12:46:25.542868 d-popcorn-1.1.2/d_popcorn.egg-info/
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      492 2023-06-20 12:46:25.000000 d-popcorn-1.1.2/d_popcorn.egg-info/PKG-INFO
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)      306 2023-06-20 12:46:25.000000 d-popcorn-1.1.2/d_popcorn.egg-info/SOURCES.txt
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        1 2023-06-20 12:46:25.000000 d-popcorn-1.1.2/d_popcorn.egg-info/dependency_links.txt
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       53 2023-06-20 12:46:25.000000 d-popcorn-1.1.2/d_popcorn.egg-info/entry_points.txt
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        6 2023-06-20 12:46:25.000000 d-popcorn-1.1.2/d_popcorn.egg-info/requires.txt
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)        8 2023-06-20 12:46:25.000000 d-popcorn-1.1.2/d_popcorn.egg-info/top_level.txt
+drwxrwxr-x   0 oelbakouchi  (1001) oelbakouchi  (1001)        0 2023-06-20 12:46:25.542868 d-popcorn-1.1.2/popcorn/
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       22 2023-06-20 12:24:36.000000 d-popcorn-1.1.2/popcorn/__init__.py
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     6627 2023-06-02 08:29:15.000000 d-popcorn-1.1.2/popcorn/dump.py
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)    15299 2023-06-20 12:23:53.000000 d-popcorn-1.1.2/popcorn/popcornS3.py
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     4595 2023-06-02 08:29:16.000000 d-popcorn-1.1.2/popcorn/popcorn_cli.py
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)       38 2023-06-20 12:46:25.542868 d-popcorn-1.1.2/setup.cfg
+-rw-rw-r--   0 oelbakouchi  (1001) oelbakouchi  (1001)     1060 2023-06-02 08:29:16.000000 d-popcorn-1.1.2/setup.py
```

### Comparing `d-popcorn-1.1.0/LICENSE` & `d-popcorn-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `d-popcorn-1.1.0/README.md` & `d-popcorn-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `d-popcorn-1.1.0/popcorn/dump.py` & `d-popcorn-1.1.2/popcorn/dump.py`

 * *Files identical despite different names*

### Comparing `d-popcorn-1.1.0/popcorn/popcornS3.py` & `d-popcorn-1.1.2/popcorn/popcornS3.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         try:
             # with self._bucket.Object(self.meta_file).get() as f:
             #     metadata = json.loads(f.read().decode('utf-8'))
             #     print(metadata)
             #     return metadata
             response = self._bucket.Object(self.meta_file).get()
             existing_metadata = json.loads(response["Body"].read().decode("utf-8"))
-            print(existing_metadata)
+            # print(existing_metadata)
             return existing_metadata
         except Exception as e:
             print("here", e)
             return {"files": {}, "projects": {}}
 
     def _generate_hash(self, file):
         hasher = hashlib.sha256()
@@ -295,15 +295,15 @@
             }
             metadata["projects"][args.project] = project_metadata_tags
 
         if file_hash not in metadata["files"]:
             print("Adding file metadata to json")
             metadata["files"][file_hash] = file_metadata_tags
 
-        self._bucket.put_object(Body=json.dumps(metadata), Key=self.meta_file)
+        self._bucket.put_object(Body=json.dumps(metadata, indent=4), Key=self.meta_file)
         print(f"Metadata for {file_name} added successfully.")
         #####################
         #    HANDLE FILE    #
         #####################
         # check if file with same hash already exists
         for f in self.get_file_hashes():
             if f == file_hash:
```

### Comparing `d-popcorn-1.1.0/popcorn/popcorn_cli.py` & `d-popcorn-1.1.2/popcorn/popcorn_cli.py`

 * *Files identical despite different names*

### Comparing `d-popcorn-1.1.0/setup.py` & `d-popcorn-1.1.2/setup.py`

 * *Files identical despite different names*

