# Comparing `tmp/hyutils-hyutil-hoyun-lab-0.0.6.2.tar.gz` & `tmp/hyutils-hyutil-hoyun-lab-0.0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.2.tar", last modified: Mon Jun 19 04:39:45 2023, max compression
+gzip compressed data, was "hyutils-hyutil-hoyun-lab-0.0.6.3.tar", last modified: Tue Jun 20 05:34:53 2023, max compression
```

## Comparing `hyutils-hyutil-hoyun-lab-0.0.6.2.tar` & `hyutils-hyutil-hoyun-lab-0.0.6.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 04:39:45.134768 hyutils-hyutil-hoyun-lab-0.0.6.2/
--rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/LICENSE.txt
--rw-rw-rw-   0        0        0      600 2023-06-19 04:39:45.134296 hyutils-hyutil-hoyun-lab-0.0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/README.md
--rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 04:39:45.135100 hyutils-hyutil-hoyun-lab-0.0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-06-19 04:39:18.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 04:39:45.111597 hyutils-hyutil-hoyun-lab-0.0.6.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 04:39:45.127597 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/
--rw-rw-rw-   0        0        0      347 2023-06-19 04:39:23.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/__init__.py
--rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/appcontrol.py
--rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/date_time.py
--rw-rw-rw-   0        0        0     1144 2023-06-15 02:19:32.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/dirjob.py
--rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/filejob.py
--rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/hashing.py
--rw-rw-rw-   0        0        0    14695 2023-06-19 04:38:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/tfrecrod_utils.py
--rw-rw-rw-   0        0        0     4046 2023-06-16 04:49:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/xml_util.py
-drwxrwxrwx   0        0        0        0 2023-06-19 04:39:45.132598 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/
--rw-rw-rw-   0        0        0      600 2023-06-19 04:39:45.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2023-06-19 04:39:45.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 04:39:45.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-19 04:39:45.000000 hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 05:34:53.152474 hyutils-hyutil-hoyun-lab-0.0.6.3/
+-rw-rw-rw-   0        0        0       37 2023-06-08 03:25:08.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      600 2023-06-20 05:34:53.151973 hyutils-hyutil-hoyun-lab-0.0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-07 07:35:00.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 07:28:49.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 05:34:53.152649 hyutils-hyutil-hoyun-lab-0.0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-06-20 05:32:24.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:34:53.127974 hyutils-hyutil-hoyun-lab-0.0.6.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 05:34:53.144474 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/
+-rw-rw-rw-   0        0        0      347 2023-06-20 05:32:24.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-01-19 02:15:34.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/appcontrol.py
+-rw-rw-rw-   0        0        0      614 2023-05-30 04:04:27.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/date_time.py
+-rw-rw-rw-   0        0        0     1144 2023-06-15 02:19:32.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/dirjob.py
+-rw-rw-rw-   0        0        0      477 2023-06-16 04:42:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/filejob.py
+-rw-rw-rw-   0        0        0     1086 2023-02-02 02:25:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/hashing.py
+-rw-rw-rw-   0        0        0    15304 2023-06-20 04:05:24.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/tfrecrod_utils.py
+-rw-rw-rw-   0        0        0     4046 2023-06-16 04:49:56.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/xml_util.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:34:53.150474 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-06-20 05:34:53.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2023-06-20 05:34:53.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 05:34:53.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 05:34:53.000000 hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/top_level.txt
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.2/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6.2
+Version: 0.0.6.3
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.2/setup.py` & `hyutils-hyutil-hoyun-lab-0.0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 
 setuptools.setup(
     name="hyutils-hyutil-hoyun-lab",
-    version="0.0.6.2",
+    version="0.0.6.3",
     url="https://www.hoyun.co.kr",
     license="MIT",
     author="nohgan im",
     author_email="fory2k@hoyun.co.kr",
     description="Hoyun Lab Python Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/date_time.py` & `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/date_time.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/dirjob.py` & `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/dirjob.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/hashing.py` & `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/hashing.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/tfrecrod_utils.py` & `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/tfrecrod_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,15 +311,15 @@
     xmin = parsed_record['image/object/bbox/xmin']
     xmax = parsed_record['image/object/bbox/xmax']
     ymin = parsed_record['image/object/bbox/ymin']
     ymax = parsed_record['image/object/bbox/ymax']
     filename = parsed_record['image/filename']
     return image, label, filename, xmin, xmax, ymin, ymax
 
-def tfrecord_valid_check(tfrecord_path):
+def tfrecord_valid_check(tfrecord_path, mode):
     # for example in tf.io..tf_record_iterator(tfrecord_path):
     #     print(tf.train.Example.FromString(example))
 
     if os.path.exists(tfrecord_path):
         # 지정된 tfrecord 파일에 대한 데이터셋을 만듬.
         dataset = tf.data.TFRecordDataset(tfrecord_path)
 
@@ -335,20 +335,26 @@
             image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
             xmin = tf.sparse.to_dense(xmin, default_value=0.0).numpy()
             xmax = tf.sparse.to_dense(xmax, default_value=0.0).numpy()
             ymin = tf.sparse.to_dense(ymin, default_value=0.0).numpy()
             ymax = tf.sparse.to_dense(ymax, default_value=0.0).numpy()
             label = tf.sparse.to_dense(label, default_value='???').numpy()
 
-            # 레이블 출력
-            for idx in np.arange(0, len(label)):
-                print(f'filename:{filename}  label:{label[idx]} > xmin:{xmin[idx]} xmax:{xmax[idx]} ymin:{ymin[idx]} ymax:{ymax[idx]}')
-                cv2.rectangle(image, (int(xmin[idx] * w), int(ymin[idx] * h)), (int(xmax[idx] * w), int(ymax[idx] * h)), (255, 255, 0), 2)
+            if mode == 'print':
+                print(f'filename:{filename}  label:{label[idx]} > xmin:{xmin[idx]} xmax:{xmax[idx]} ymin:{ymin[idx]} ymax:{ymax[idx]}, h:{h} w:{w} c:{c}')
+                if c != 3:
+                    print('---------------------- invalid image\'s channel size ----------------------')
+                    cv2.waitKey(0)
+            else:
+                # 레이블 출력
+                for idx in np.arange(0, len(label)):
+                    print(f'filename:{filename}  label:{label[idx]} > xmin:{xmin[idx]} xmax:{xmax[idx]} ymin:{ymin[idx]} ymax:{ymax[idx]}')
+                    cv2.rectangle(image, (int(xmin[idx] * w), int(ymin[idx] * h)), (int(xmax[idx] * w), int(ymax[idx] * h)), (255, 255, 0), 2)
 
-            cv2.imshow('image', image)
+                cv2.imshow('image', image)
 
 
 
         # for d in raw_dataset:
         #     ex = tf.train.Example()
         #     ex.ParseFromString(d.numpy())
         #     m = json.loads(MessageToJson(ex))
@@ -357,8 +363,12 @@
         # for raw_record in dataset:
         #     example = tf.train.Example()
         #     example.ParseFromString(raw_record.numpy())
         #     print(example)
         #     print('-----------------------------------------------------------')
             key = cv2.waitKey(0)
             if key == 27:
-                break
+                break
+
+# def merge_multiple_tfrecords(record_list, output_path):
+#     raw_dataset = tf.data.TFRecordDataset(record_list)
+#     merged_dataset = raw_dataset.concatenate(tf.data.TFRecordDataset(output_path))
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutil_hoyun_lab/xml_util.py` & `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutil_hoyun_lab/xml_util.py`

 * *Files identical despite different names*

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO` & `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyutils-hyutil-hoyun-lab
-Version: 0.0.6.2
+Version: 0.0.6.3
 Summary: Hoyun Lab Python Utils
 Home-page: https://www.hoyun.co.kr
 Author: nohgan im
 Author-email: fory2k@hoyun.co.kr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/schooldevops/python-tutorials/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyutils-hyutil-hoyun-lab-0.0.6.2/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt` & `hyutils-hyutil-hoyun-lab-0.0.6.3/src/hyutils_hyutil_hoyun_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

