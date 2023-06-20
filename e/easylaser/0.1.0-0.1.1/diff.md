# Comparing `tmp/easylaser-0.1.0.tar.gz` & `tmp/easylaser-0.1.1.tar.gz`

## Comparing `easylaser-0.1.0.tar` & `easylaser-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 easylaser-0.1.0/Distribution.md
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 easylaser-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 easylaser-0.1.0/easylaser/__init__.py
--rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 easylaser-0.1.0/easylaser/align.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 easylaser-0.1.0/easylaser/get_model.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 easylaser-0.1.0/easylaser/laser.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 easylaser-0.1.0/easylaser/embed/embed.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 easylaser-0.1.0/easylaser/embed/encoder.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 easylaser-0.1.0/easylaser/embed/laserLstmEncoder.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 easylaser-0.1.0/easylaser/embed/laserTransformerEncoder.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 easylaser-0.1.0/easylaser/embed/multiGpuEncoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easylaser-0.1.0/easylaser/lib/__init__.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 easylaser-0.1.0/easylaser/lib/constants.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 easylaser-0.1.0/easylaser/lib/text_processing.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 easylaser-0.1.0/test/fake_data.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 easylaser-0.1.0/test/test_laser.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 easylaser-0.1.0/.gitignore
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 easylaser-0.1.0/LICENSE
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 easylaser-0.1.0/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 easylaser-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6568 2020-02-02 00:00:00.000000 easylaser-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 easylaser-0.1.1/Distribution.md
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 easylaser-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/__init__.py
+-rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/align.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/get_model.py
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/laser.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/embed/embed.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/embed/encoder.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/embed/laserLstmEncoder.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/embed/laserTransformerEncoder.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/embed/multiGpuEncoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/lib/__init__.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/lib/constants.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 easylaser-0.1.1/easylaser/lib/text_processing.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 easylaser-0.1.1/test/fake_data.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 easylaser-0.1.1/test/test_laser.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 easylaser-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 easylaser-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 easylaser-0.1.1/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 easylaser-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 easylaser-0.1.1/PKG-INFO
```

### Comparing `easylaser-0.1.0/easylaser/align.py` & `easylaser-0.1.1/easylaser/align.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.0/easylaser/get_model.py` & `easylaser-0.1.1/easylaser/get_model.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.0/easylaser/laser.py` & `easylaser-0.1.1/easylaser/laser.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,18 @@
     def stop_encoder(self):
         """
         Stop the encoder, free the GPU/CPU memory
         """
         del self.encoder
 
     def is_encoder_active(self):
-        return hasattr(self, "encoder")
+        try:
+            return not self.encoder is None
+        except AttributeError:
+            return False
 
     def start_encoder(self, device: list[str] | str = None):
         """
         Start the encoder, you can overwrite the target_device and cpu parameters, else it will use the one specified at init
         :param target_device: ids of a GPU to use for embedding, if None, will use the first GPU available. If you want to use multiple GPUs, use launchMultiGpuEncoder
         :param cpu: if True, will use CPU for embedding and ignore target_devices
         """
```

### Comparing `easylaser-0.1.0/easylaser/embed/embed.py` & `easylaser-0.1.1/easylaser/embed/embed.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.0/easylaser/embed/encoder.py` & `easylaser-0.1.1/easylaser/embed/encoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.0/easylaser/embed/laserLstmEncoder.py` & `easylaser-0.1.1/easylaser/embed/laserLstmEncoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.0/easylaser/embed/laserTransformerEncoder.py` & `easylaser-0.1.1/easylaser/embed/laserTransformerEncoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.0/easylaser/embed/multiGpuEncoder.py` & `easylaser-0.1.1/easylaser/embed/multiGpuEncoder.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.0/easylaser/lib/constants.py` & `easylaser-0.1.1/easylaser/lib/constants.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.0/easylaser/lib/text_processing.py` & `easylaser-0.1.1/easylaser/lib/text_processing.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.0/test/fake_data.py` & `easylaser-0.1.1/test/fake_data.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.0/test/test_laser.py` & `easylaser-0.1.1/test/test_laser.py`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.0/LICENSE` & `easylaser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easylaser-0.1.0/README.md` & `easylaser-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 
 So as we have seen you can use it with a context manager or without
 
 ```python
 from easylaser import Laser
 sentences = ["This is a sentence", "this is another sentences."]
 
-#with context manager
+# with context manager
 with Laser() as laser:
     embeddings = laser.embed_sentences(sentences=sentences)
 
-#without
+# without
 laser = Laser()
-laser.is_encoder_active() #return False
+laser.is_encoder_active() # return False
 laser.start_encoder()
 embeddings = laser.embed_sentences(sentences=sentences)
-laser.is_encoder_active() #return True
+laser.is_encoder_active() # return True
 laser.stop_encoder()
 ```
 
 ## Multi GPU
 
 You can specify the hardware you want to run on :
```

### Comparing `easylaser-0.1.0/pyproject.toml` & `easylaser-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "easylaser"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Lingua Custodia", email="it@linguacustodia.com" },
 ]
 description = "An easy to use interface to LASER"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `easylaser-0.1.0/PKG-INFO` & `easylaser-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easylaser
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy to use interface to LASER
 Author-email: Lingua Custodia <it@linguacustodia.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
@@ -52,24 +52,24 @@
 
 So as we have seen you can use it with a context manager or without
 
 ```python
 from easylaser import Laser
 sentences = ["This is a sentence", "this is another sentences."]
 
-#with context manager
+# with context manager
 with Laser() as laser:
     embeddings = laser.embed_sentences(sentences=sentences)
 
-#without
+# without
 laser = Laser()
-laser.is_encoder_active() #return False
+laser.is_encoder_active() # return False
 laser.start_encoder()
 embeddings = laser.embed_sentences(sentences=sentences)
-laser.is_encoder_active() #return True
+laser.is_encoder_active() # return True
 laser.stop_encoder()
 ```
 
 ## Multi GPU
 
 You can specify the hardware you want to run on :
```

