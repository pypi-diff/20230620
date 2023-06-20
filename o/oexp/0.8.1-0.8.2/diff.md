# Comparing `tmp/oexp-0.8.1.tar.gz` & `tmp/oexp-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.8.1.tar", last modified: Tue Jun 20 16:30:53 2023, max compression
+gzip compressed data, was "oexp-0.8.2.tar", last modified: Tue Jun 20 16:39:34 2023, max compression
```

## Comparing `oexp-0.8.1.tar` & `oexp-0.8.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:30:53.042634 oexp-0.8.1/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 16:30:53.042460 oexp-0.8.1/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.8.1/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:30:53.041218 oexp-0.8.1/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      189 2023-06-20 15:09:33.000000 oexp-0.8.1/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    81295 2023-06-20 16:24:01.000000 oexp-0.8.1/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-20 16:23:58.000000 oexp-0.8.1/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2011 2023-06-12 01:50:22.000000 oexp-0.8.1/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:30:53.042295 oexp-0.8.1/oexp/util/
--rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.8.1/oexp/util/__init__.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.8.1/oexp/util/ops.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.8.1/oexp/util/vals.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:30:53.041917 oexp-0.8.1/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 16:30:53.000000 oexp-0.8.1/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-20 16:30:53.000000 oexp-0.8.1/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-20 16:30:53.000000 oexp-0.8.1/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-20 16:30:53.000000 oexp-0.8.1/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-20 16:30:53.000000 oexp-0.8.1/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-20 16:30:48.000000 oexp-0.8.1/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-20 16:30:53.042685 oexp-0.8.1/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:39:34.741430 oexp-0.8.2/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 16:39:34.741265 oexp-0.8.2/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.8.2/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:39:34.740005 oexp-0.8.2/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      189 2023-06-20 15:09:33.000000 oexp-0.8.2/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    81355 2023-06-20 16:39:14.000000 oexp-0.8.2/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-20 16:39:07.000000 oexp-0.8.2/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2011 2023-06-12 01:50:22.000000 oexp-0.8.2/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:39:34.741096 oexp-0.8.2/oexp/util/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.8.2/oexp/util/__init__.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.8.2/oexp/util/ops.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.8.2/oexp/util/vals.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 16:39:34.740705 oexp-0.8.2/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 16:39:34.000000 oexp-0.8.2/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-20 16:39:34.000000 oexp-0.8.2/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-20 16:39:34.000000 oexp-0.8.2/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-20 16:39:34.000000 oexp-0.8.2/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-20 16:39:34.000000 oexp-0.8.2/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-20 16:39:30.000000 oexp-0.8.2/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-20 16:39:34.741474 oexp-0.8.2/setup.cfg
```

### Comparing `oexp-0.8.1/oexp/access.py` & `oexp-0.8.2/oexp/access.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     global _SAFE_PROCESS, _SAFE_THREAD
     if current_process().pid != _SAFE_PROCESS or current_thread().ident != _SAFE_THREAD:
         raise Exception(
             f"Python-Kotlin communication is currently not safe to use across multiple threads or processes. If you need this feature, please let me know."
         )
 
 
-JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/553/oexp-front-0-all.jar"
+JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/556/oexp-front-0-all.jar"
 
 
 class OexpExitSocketHeaders(Enum):
     EXIT = b"\x00"
 
 
 EXIT = b"\x00"
@@ -1219,28 +1219,14 @@
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
         else:
             return False
 
 
-# [[matt.oexp.olang.lab.model.Trial]]
-class Trial(KBClass, abc.ABC):
-    # [[matt.oexp.olang.lab.model.Trial]]
-    def to_json(self):
-        _ensure_synchronized()
-        _sendall(GET_JSON)
-        _send_long(self._id._id)
-        return _recv_string(nullable=False)
-
-    # [[matt.oexp.olang.lab.model.Trial]]
-    def to_dict(self):
-        return json.loads(self.to_json())
-
-
 def trial_manifest(trials=NO_DEFAULT, skip=DEFAULT_VALUE):
     _check_required_parameters(**dict(trials=trials))
     return TrialManifest(trials, skip)
 
 
 # [[matt.oexp.olang.lab.model.TrialManifest]]
 class TrialManifest(KBDClass):
@@ -1307,14 +1293,28 @@
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
         else:
             return False
 
 
+# [[matt.oexp.olang.lab.model.trial.Trial]]
+class Trial(KBClass, abc.ABC):
+    # [[matt.oexp.olang.lab.model.trial.Trial]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.lab.model.trial.Trial]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+
 def encrypted_stimulus_path(cipher_path=NO_DEFAULT):
     _check_required_parameters(**dict(cipher_path=cipher_path))
     return EncryptedStimulusPath(cipher_path)
 
 
 # [[matt.oexp.olang.model.EncryptedStimulusPath]]
 class EncryptedStimulusPath(KBVClass):
@@ -2193,64 +2193,64 @@
 
 
 def gallery_trial(query=NO_DEFAULT, distractors=NO_DEFAULT):
     _check_required_parameters(**dict(query=query, distractors=distractors))
     return GalleryTrial(query, distractors)
 
 
-# [[matt.oexp.olang.lab.model.GalleryTrial]]
+# [[matt.oexp.olang.lab.model.trial.GalleryTrial]]
 class GalleryTrial(Trial, KBDClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.lab.model.GalleryTrial")
+            _send_string("matt.oexp.olang.lab.model.trial.GalleryTrial")
             _send_string(args[0])
             _send_int(len(args[1]))
             for e in args[1]:
                 _send_string(e)
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.lab.model.GalleryTrial#distractors]]
+    # [[matt.oexp.olang.lab.model.trial.GalleryTrial#distractors]]
     @property
     def distractors(self) -> List[str]:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
         temp = _recv_list(
             elementReceiveFun=lambda: _recv_string(nullable=False), nullable=False
         )
         return temp
 
-    # [[matt.oexp.olang.lab.model.GalleryTrial#query]]
+    # [[matt.oexp.olang.lab.model.trial.GalleryTrial#query]]
     @property
     def query(self) -> str:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(1)
         temp = _recv_string(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.lab.model.GalleryTrial]]
+    # [[matt.oexp.olang.lab.model.trial.GalleryTrial]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.lab.model.GalleryTrial]]
+    # [[matt.oexp.olang.lab.model.trial.GalleryTrial]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.lab.model.GalleryTrial]]
+    # [[matt.oexp.olang.lab.model.trial.GalleryTrial]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
```

### Comparing `oexp-0.8.1/oexp/jbridge.py` & `oexp-0.8.2/oexp/jbridge.py`

 * *Files identical despite different names*

### Comparing `oexp-0.8.1/oexp/util/ops.py` & `oexp-0.8.2/oexp/util/ops.py`

 * *Files identical despite different names*

### Comparing `oexp-0.8.1/oexp/util/vals.py` & `oexp-0.8.2/oexp/util/vals.py`

 * *Files identical despite different names*

