# Comparing `tmp/tflite_runtime_nightly-2.14.0.dev20230617-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tflite_runtime_nightly-2.14.0.dev20230618-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 2404843 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-Jun-18 05:00 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  6832424 b- defN 23-Jun-18 05:02 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-Jun-18 05:00 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-Jun-18 05:00 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-Jun-18 05:00 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1441 b- defN 23-Jun-18 05:02 tflite_runtime_nightly-2.14.0.dev20230617.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 23-Jun-18 05:02 tflite_runtime_nightly-2.14.0.dev20230617.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-18 05:02 tflite_runtime_nightly-2.14.0.dev20230617.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-Jun-18 05:02 tflite_runtime_nightly-2.14.0.dev20230617.dist-info/RECORD
+-rw-rw-r--  2.0 unx       80 b- defN 23-Jun-19 05:05 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  6832424 b- defN 23-Jun-19 05:07 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-Jun-19 05:05 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-Jun-19 05:05 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-Jun-19 05:05 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1441 b- defN 23-Jun-19 05:07 tflite_runtime_nightly-2.14.0.dev20230618.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 23-Jun-19 05:07 tflite_runtime_nightly-2.14.0.dev20230618.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-19 05:07 tflite_runtime_nightly-2.14.0.dev20230618.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Jun-19 05:07 tflite_runtime_nightly-2.14.0.dev20230618.dist-info/RECORD
 9 files, 6877314 bytes uncompressed, 2403297 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230617.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.14.0.dev20230618.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230617.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.14.0.dev20230618.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230617.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.14.0.dev20230618.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230617.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.14.0.dev20230618.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.14.0dev20230617'
-__git_version__ = '0.6.0-149398-g08bd7e1a8e5'
+__version__ = '2.14.0dev20230618'
+__git_version__ = '0.6.0-149402-gc70da227c52'
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230617.dist-info/METADATA` & `tflite_runtime_nightly-2.14.0.dev20230618.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.14.0.dev20230617
+Version: 2.14.0.dev20230618
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

