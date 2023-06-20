# Comparing `tmp/meta-trt-3.3.29.tar.gz` & `tmp/meta-trt-3.6.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-trt-3.3.29.tar", last modified: Wed Mar 29 08:09:25 2023, max compression
+gzip compressed data, was "dist/meta-trt-3.6.20.tar", last modified: Tue Jun 20 09:33:38 2023, max compression
```

## Comparing `meta-trt-3.3.29.tar` & `meta-trt-3.6.20.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-03-29 08:09:25.000000 meta-trt-3.3.29/
--rw-rw-r--   0 cash      (1000) cash      (1000)      273 2023-03-29 08:09:25.000000 meta-trt-3.3.29/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)       35 2022-11-09 06:02:25.000000 meta-trt-3.3.29/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-03-29 08:09:25.000000 meta-trt-3.3.29/meta_trt.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      273 2023-03-29 08:09:24.000000 meta-trt-3.3.29/meta_trt.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)      771 2023-03-29 08:09:24.000000 meta-trt-3.3.29/meta_trt.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-03-29 08:09:24.000000 meta-trt-3.3.29/meta_trt.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       54 2023-03-29 08:09:24.000000 meta-trt-3.3.29/meta_trt.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        8 2023-03-29 08:09:24.000000 meta-trt-3.3.29/meta_trt.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-03-29 08:09:24.000000 meta-trt-3.3.29/meta_trt.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-03-29 08:09:25.000000 meta-trt-3.3.29/metatrt/
--rw-rw-r--   0 cash      (1000) cash      (1000)      111 2022-11-28 13:09:57.000000 meta-trt-3.3.29/metatrt/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-03-29 08:09:25.000000 meta-trt-3.3.29/metatrt/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)      256 2022-11-28 13:09:41.000000 meta-trt-3.3.29/metatrt/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2688 2023-03-29 07:42:45.000000 meta-trt-3.3.29/metatrt/app/instance_segment_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      849 2022-11-25 02:30:17.000000 meta-trt-3.3.29/metatrt/app/object_classification_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2243 2022-11-25 02:30:49.000000 meta-trt-3.3.29/metatrt/app/object_detection_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1232 2023-02-13 03:43:09.000000 meta-trt-3.3.29/metatrt/app/onnx_to_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      694 2022-10-30 08:26:29.000000 meta-trt-3.3.29/metatrt/app/saliency_segment_trt.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-03-29 08:09:25.000000 meta-trt-3.3.29/metatrt/model_zoo/
--rw-rw-r--   0 cash      (1000) cash      (1000)      266 2022-11-28 13:09:21.000000 meta-trt-3.3.29/metatrt/model_zoo/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2557 2023-03-02 07:35:49.000000 meta-trt-3.3.29/metatrt/model_zoo/classification_trt_predictor.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1782 2022-11-30 10:22:20.000000 meta-trt-3.3.29/metatrt/model_zoo/detection_trt_predictor.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4685 2023-03-29 07:42:45.000000 meta-trt-3.3.29/metatrt/model_zoo/instance_trt_predictor.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1415 2022-11-03 15:52:40.000000 meta-trt-3.3.29/metatrt/model_zoo/segment_trt_predictor.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    15434 2023-02-13 03:41:43.000000 meta-trt-3.3.29/metatrt/model_zoo/trt_export.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-03-29 08:09:25.000000 meta-trt-3.3.29/metatrt/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)       71 2022-10-30 06:23:59.000000 meta-trt-3.3.29/metatrt/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    10181 2023-03-29 08:02:51.000000 meta-trt-3.3.29/metatrt/utils/general.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7059 2023-02-13 03:41:21.000000 meta-trt-3.3.29/metatrt/utils/image_batch.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7013 2023-03-20 07:40:18.000000 meta-trt-3.3.29/metatrt/utils/utils.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-03-29 08:09:25.000000 meta-trt-3.3.29/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      680 2023-03-29 08:05:45.000000 meta-trt-3.3.29/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 09:33:38.000000 meta-trt-3.6.20/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      273 2023-06-20 09:33:38.000000 meta-trt-3.6.20/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)       35 2022-11-09 06:02:25.000000 meta-trt-3.6.20/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 09:33:38.000000 meta-trt-3.6.20/meta_trt.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      273 2023-06-20 09:33:38.000000 meta-trt-3.6.20/meta_trt.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)      771 2023-06-20 09:33:38.000000 meta-trt-3.6.20/meta_trt.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-06-20 09:33:38.000000 meta-trt-3.6.20/meta_trt.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       54 2023-06-20 09:33:38.000000 meta-trt-3.6.20/meta_trt.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        8 2023-06-20 09:33:38.000000 meta-trt-3.6.20/meta_trt.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-06-20 09:33:38.000000 meta-trt-3.6.20/meta_trt.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 09:33:38.000000 meta-trt-3.6.20/metatrt/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      111 2022-11-28 13:09:57.000000 meta-trt-3.6.20/metatrt/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 09:33:38.000000 meta-trt-3.6.20/metatrt/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      256 2022-11-28 13:09:41.000000 meta-trt-3.6.20/metatrt/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2641 2023-06-20 09:05:59.000000 meta-trt-3.6.20/metatrt/app/instance_segment_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      849 2022-11-25 02:30:17.000000 meta-trt-3.6.20/metatrt/app/object_classification_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2243 2022-11-25 02:30:49.000000 meta-trt-3.6.20/metatrt/app/object_detection_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1232 2023-02-13 03:43:09.000000 meta-trt-3.6.20/metatrt/app/onnx_to_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      694 2022-10-30 08:26:29.000000 meta-trt-3.6.20/metatrt/app/saliency_segment_trt.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 09:33:38.000000 meta-trt-3.6.20/metatrt/model_zoo/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      266 2022-11-28 13:09:21.000000 meta-trt-3.6.20/metatrt/model_zoo/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2557 2023-03-02 07:35:49.000000 meta-trt-3.6.20/metatrt/model_zoo/classification_trt_predictor.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1782 2022-11-30 10:22:20.000000 meta-trt-3.6.20/metatrt/model_zoo/detection_trt_predictor.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4885 2023-06-20 09:29:38.000000 meta-trt-3.6.20/metatrt/model_zoo/instance_trt_predictor.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1415 2022-11-03 15:52:40.000000 meta-trt-3.6.20/metatrt/model_zoo/segment_trt_predictor.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    15434 2023-06-09 09:55:29.000000 meta-trt-3.6.20/metatrt/model_zoo/trt_export.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 09:33:38.000000 meta-trt-3.6.20/metatrt/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       71 2022-10-30 06:23:59.000000 meta-trt-3.6.20/metatrt/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    10217 2023-06-20 06:16:26.000000 meta-trt-3.6.20/metatrt/utils/general.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7059 2023-02-13 03:41:21.000000 meta-trt-3.6.20/metatrt/utils/image_batch.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     6963 2023-06-20 09:30:03.000000 meta-trt-3.6.20/metatrt/utils/utils.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-06-20 09:33:38.000000 meta-trt-3.6.20/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      680 2023-06-20 07:37:41.000000 meta-trt-3.6.20/setup.py
```

### Comparing `meta-trt-3.3.29/meta_trt.egg-info/SOURCES.txt` & `meta-trt-3.6.20/meta_trt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meta-trt-3.3.29/metatrt/app/instance_segment_trt.py` & `meta-trt-3.6.20/metatrt/app/instance_segment_trt.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     def __init__(self,
                  trt_file="models/yolov7-seg.trt",
                  input_shape=(640, 640),
                  conf=0.01,
                  iou=0.45,
                  use_mask=False,
                  use_cupy=False,
-                 multi_label=False):
+                 v8=False):
         self.conf = conf
         self.iou = iou
         self.use_mask = use_mask
         self.use_cupy = use_cupy
-        self.multi_label = multi_label
+        self.v8 = v8
         self.model = InstanceTrtPredictor(trt_file=trt_file, image_size=input_shape)
 
     def predict(self, image, class_names, use_preprocess=False):
         return self.model.predict(image, class_names, use_preprocess, self.conf, self.iou, self.use_mask,
-                                  self.use_cupy, self.multi_label)
+                                  self.use_cupy, self.v8)
 
     @staticmethod
     def show(image, results):
         if results is None or len(results) == 0:
             return image
 
         for i, result in enumerate(results):
             x1, y1, x2, y2, x3, y3, x4, y4, score, label = result
             cv2.line(image, pt1=(x1, y1), pt2=(x2, y2), color=(255, 255, 0), thickness=10)
             cv2.line(image, pt1=(x2, y2), pt2=(x3, y3), color=(255, 255, 0), thickness=10)
             cv2.line(image, pt1=(x3, y3), pt2=(x4, y4), color=(255, 255, 0), thickness=10)
             cv2.line(image, pt1=(x4, y4), pt2=(x1, y1), color=(255, 255, 0), thickness=10)
-            cv2.putText(image, 'id: %d, score: %.2f' % (label, score),
+            cv2.putText(image, '%d(%.2f)' % (label, score),
                         (x1, y1 - 4), cv2.FONT_HERSHEY_PLAIN, 2, (0, 0, 255), thickness=2)
         return image
 
     def predict_video(self, file_path=0, class_names=['person'], show=False):
         capture = cv2.VideoCapture(file_path)
         if capture.isOpened():
             if show:
```

### Comparing `meta-trt-3.3.29/metatrt/app/object_classification_trt.py` & `meta-trt-3.6.20/metatrt/app/object_classification_trt.py`

 * *Files identical despite different names*

### Comparing `meta-trt-3.3.29/metatrt/app/object_detection_trt.py` & `meta-trt-3.6.20/metatrt/app/object_detection_trt.py`

 * *Files identical despite different names*

### Comparing `meta-trt-3.3.29/metatrt/app/onnx_to_trt.py` & `meta-trt-3.6.20/metatrt/app/onnx_to_trt.py`

 * *Files identical despite different names*

### Comparing `meta-trt-3.3.29/metatrt/app/saliency_segment_trt.py` & `meta-trt-3.6.20/metatrt/app/saliency_segment_trt.py`

 * *Files identical despite different names*

### Comparing `meta-trt-3.3.29/metatrt/model_zoo/classification_trt_predictor.py` & `meta-trt-3.6.20/metatrt/model_zoo/classification_trt_predictor.py`

 * *Files identical despite different names*

### Comparing `meta-trt-3.3.29/metatrt/model_zoo/detection_trt_predictor.py` & `meta-trt-3.6.20/metatrt/model_zoo/detection_trt_predictor.py`

 * *Files identical despite different names*

### Comparing `meta-trt-3.3.29/metatrt/model_zoo/instance_trt_predictor.py` & `meta-trt-3.6.20/metatrt/model_zoo/instance_trt_predictor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import cv2
 import numpy as np
-from ..utils import preproc, multiclass_nms, singleclass_nms, sigmoid, fast_dot
+from ..utils import preproc, singleclass_nms, sigmoid, fast_dot
 from ..utils import BaseEngine
 import pycuda.driver as cuda
 
 
 class InstanceTrtPredictor(BaseEngine):
     def __init__(self, trt_file, image_size=(640, 640)):
         super(InstanceTrtPredictor, self).__init__(trt_file)
-        self.image_size = image_size  # (h, w)
+        self.image_size = image_size
+        self.feature_size = (image_size[0] // 4, image_size[1] // 4)  # (h, w)
+
+        self.ctx = cuda.Device(0).retain_primary_context()
         self.mean = None
         self.std = None
 
     @staticmethod
     def get_rect(mask):
         h, w = mask.shape[:2]
         _, pred = cv2.threshold(mask, 128, 255, cv2.THRESH_BINARY)
@@ -23,46 +26,47 @@
         area = [cv2.contourArea(c) for c in contours]
         max_idx = np.argmax(area)
         min_rect = cv2.minAreaRect(contours[max_idx])
         min_rect = cv2.boxPoints(min_rect)
 
         return min_rect
 
-    def predict(self, origin_img, class_names, use_preprocess, conf, iou, use_mask=False, use_cupy=False,
-                multi_label=False):
+    def predict(self, origin_img, class_names, use_preprocess, conf, iou, use_mask=False, use_cupy=False, v8=False):
         dets = []
         img, ratio = preproc(origin_img, self.image_size, self.mean, self.std) if use_preprocess else (origin_img, 1.0)
         data = self.infer(img)
         data = [np.ascontiguousarray(x, dtype=np.float64) for x in data]
         # 处理box
-        mi = 5 + len(class_names)
-        pred = np.reshape(data[-1], (1, -1, mi + 32))[0]
-        boxes = self.postprocess(pred, ratio=1., score_thr=conf, nms_thr=iou, multi_label=multi_label)
+        if v8:
+            mi = 4 + len(class_names)
+            pred = np.reshape(data[-1], (1, mi + 32, -1))[0].T
+        else:
+            mi = 5 + len(class_names)
+            pred = np.reshape(data[-1], (1, mi + 32, -1))[0]
+        boxes = self.postprocess(pred, ratio=1., score_thr=conf, nms_thr=iou, v8=v8)
         if boxes is None: return dets
         # 处理mask
         if use_mask:
             if use_cupy:
                 import cupy as cp
-
-                ctx = cuda.Device(0).retain_primary_context()
-                ctx.push()
+                self.ctx.push()
                 gpu_data0 = cp.asarray(data[0])
                 gpu_proto = cp.reshape(gpu_data0, (1, 32, -1))[0]
                 gpu_boxes = cp.asarray(boxes[:, 6:])
                 gpu_dot = cp.dot(gpu_boxes, gpu_proto)
                 gpu_sigmoid_dot = 1 / (1 + cp.exp(-gpu_dot))
-                gpu_masks = cp.reshape(gpu_sigmoid_dot, (-1, 160, 160))
+                gpu_masks = cp.reshape(gpu_sigmoid_dot, (-1, self.feature_size[0], self.feature_size[1]))
                 masks = cp.asnumpy(gpu_masks)
-                ih, iw = 160 / self.image_size[0], 160 / self.image_size[1]
-                ctx.pop()
+                ih, iw = self.feature_size[0] / self.image_size[0], self.feature_size[1] / self.image_size[1]
+                self.ctx.pop()
             else:
-                # csl: about 11ms on i7-8700
                 proto = np.reshape(data[0], (1, 32, -1))[0]
-                masks = np.reshape(sigmoid(fast_dot(boxes[:, 6:], proto)), (-1, 160, 160))
-                ih, iw = 160 / self.image_size[0], 160 / self.image_size[1]
+                masks = np.reshape(sigmoid(fast_dot(boxes[:, 6:], proto)),
+                                   (-1, self.feature_size[0], self.feature_size[1]))
+                ih, iw = self.feature_size[0] / self.image_size[0], self.feature_size[1] / self.image_size[1]
 
             for mask, box, score, label in zip(masks, boxes[:, :4], boxes[:, 4], boxes[:, 5]):
                 x1, y1, x2, y2 = box[0] * iw, box[1] * ih, box[2] * iw, box[3] * ih
                 crop = mask[int(y1):int(y2) + 1, int(x1):int(x2) + 1] * 255
                 min_rect = self.get_rect(crop.astype(np.uint8))
                 rect = [[(r[0] + x1) / ih / ratio, (r[1] + y1) / iw / ratio] for r in min_rect]
                 dets.append([max(int(rect[0][0]), 0), max(int(rect[0][1]), 0),
@@ -78,23 +82,23 @@
                              max(int(x2), 0), max(int(y2), 0),
                              max(int(x1), 0), max(int(y2), 0),
                              float(score), int(label)])
 
         return dets
 
     @staticmethod
-    def postprocess(predictions, ratio, score_thr, nms_thr, multi_label=False):
+    def postprocess(predictions, ratio, score_thr, nms_thr, v8=False):
         boxes = predictions[:, :4]
-        scores = predictions[:, 4:5] * predictions[:, 5:-32]
+        scores = predictions[:, 4:-32] if v8 else predictions[:, 4:5] * predictions[:, 5:-32]
         boxes_xyxy = np.ones_like(boxes)
         boxes_xyxy[:, 0] = boxes[:, 0] - boxes[:, 2] / 2.
         boxes_xyxy[:, 1] = boxes[:, 1] - boxes[:, 3] / 2.
         boxes_xyxy[:, 2] = boxes[:, 0] + boxes[:, 2] / 2.
         boxes_xyxy[:, 3] = boxes[:, 1] + boxes[:, 3] / 2.
         boxes_xyxy /= ratio
 
-        if multi_label:
-            dets = multiclass_nms(boxes_xyxy, scores, nms_thr=nms_thr, score_thr=score_thr, predictions=predictions)
-        else:
-            dets = singleclass_nms(boxes_xyxy, scores, nms_thr=nms_thr, score_thr=score_thr, predictions=predictions)
+        dets = singleclass_nms(boxes_xyxy, scores, nms_thr=nms_thr, score_thr=score_thr, predictions=predictions, v8=v8)
 
         return dets
+
+    def __del__(self):
+        self.cfx.pop()
```

### Comparing `meta-trt-3.3.29/metatrt/model_zoo/segment_trt_predictor.py` & `meta-trt-3.6.20/metatrt/model_zoo/segment_trt_predictor.py`

 * *Files identical despite different names*

### Comparing `meta-trt-3.3.29/metatrt/model_zoo/trt_export.py` & `meta-trt-3.6.20/metatrt/model_zoo/trt_export.py`

 * *Files identical despite different names*

### Comparing `meta-trt-3.3.29/metatrt/utils/general.py` & `meta-trt-3.6.20/metatrt/utils/general.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,18 +146,18 @@
 
         inds = np.where(ovr <= nms_thr)[0]
         order = order[inds + 1]
 
     return keep
 
 
-def singleclass_nms(boxes, scores, nms_thr, score_thr, predictions=None):
+def singleclass_nms(boxes, scores, nms_thr, score_thr, predictions=None, v8=False):
     """Multiclass NMS implemented in Numpy"""
     num_classes = scores.shape[1]
-    mi = 5 + num_classes  # mask start index
+    mi = (4 if v8 else 5) + num_classes  # mask start index
 
     cls_scores = np.max(scores, axis=1)
     cls_indexes = np.argmax(scores, axis=1)
     valid_score_mask = cls_scores > score_thr
     if valid_score_mask.sum() == 0:
         return None
     else:
@@ -166,15 +166,15 @@
         valid_boxes = boxes[valid_score_mask]
         valid_predictions = predictions[valid_score_mask]
         keep = nms(valid_boxes, valid_scores, nms_thr)
         if len(keep) > 0:
             if predictions is None:
                 dets = np.concatenate([valid_boxes[keep], valid_scores[keep, None], valid_indexes[keep]], 1)
             else:
-                valid_predictions[:, mi:] *= valid_predictions[:, 4:5]
+                if not v8: valid_predictions[:, mi:] *= valid_predictions[:, 4:5]
                 dets = np.concatenate(
                     [valid_boxes[keep], valid_scores[keep, None], valid_indexes[keep, None],
                      valid_predictions[keep, mi:]], 1)
 
     if len(dets) == 0:
         return None
     return dets
```

### Comparing `meta-trt-3.3.29/metatrt/utils/image_batch.py` & `meta-trt-3.6.20/metatrt/utils/image_batch.py`

 * *Files identical despite different names*

### Comparing `meta-trt-3.3.29/metatrt/utils/utils.py` & `meta-trt-3.6.20/metatrt/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import cv2
 import numpy as np
 import tensorrt as trt
-# import pycuda.autoinit
 import pycuda.driver as cuda
 from .general import *
 
 
 class BaseEngine(object):
     def __init__(self, trt_file, image_size=(640, 640)):
         self.image_size = image_size
@@ -25,18 +24,15 @@
                             'sandwich', 'orange', 'broccoli', 'carrot', 'hot dog', 'pizza', 'donut', 'cake', 'chair',
                             'couch',
                             'potted plant', 'bed', 'dining table', 'toilet', 'tv', 'laptop', 'mouse', 'remote',
                             'keyboard', 'cell phone',
                             'microwave', 'oven', 'toaster', 'sink', 'refrigerator', 'book', 'clock', 'vase', 'scissors',
                             'teddy bear',
                             'hair drier', 'toothbrush']
-
-        cuda.init()
         self.cfx = cuda.Device(0).make_context()
-
         logger = trt.Logger(trt.Logger.WARNING)
         runtime = trt.Runtime(logger)
         trt.init_libnvinfer_plugins(logger, '')
         with open(trt_file, "rb") as f:
             serialized_engine = f.read()
         engine = runtime.deserialize_cuda_engine(serialized_engine)
         self.context = engine.create_execution_context()
@@ -50,15 +46,15 @@
             self.bindings.append(int(device_mem))
             if engine.binding_is_input(binding):
                 self.inputs.append({'host': host_mem, 'device': device_mem})
             else:
                 self.outputs.append({'host': host_mem, 'device': device_mem})
 
     def __del__(self):
-        self.cfx.detach()
+        self.cfx.pop()
 
     def infer(self, img):
         self.cfx.push()
 
         self.inputs[0]['host'] = np.ravel(img)
         # transfer data to the gpu
         for inp in self.inputs:
```

### Comparing `meta-trt-3.3.29/setup.py` & `meta-trt-3.6.20/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     'setuptools',
     'tensorrt',
     'pycuda',
     'numpy',
     'pillow',
 ]
 
-__version__ = 'V3.3.29'
+__version__ = 'V3.6.20'
 
 setup(
     name='meta-trt',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
     url='https://github.com/CachCheng/cvtrt',
```

