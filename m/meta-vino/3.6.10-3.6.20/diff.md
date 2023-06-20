# Comparing `tmp/meta-vino-3.6.10.tar.gz` & `tmp/meta-vino-3.6.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-vino-3.6.10.tar", last modified: Fri Jun  9 13:27:17 2023, max compression
+gzip compressed data, was "dist/meta-vino-3.6.20.tar", last modified: Tue Jun 20 10:31:06 2023, max compression
```

## Comparing `meta-vino-3.6.10.tar` & `meta-vino-3.6.20.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-09 13:27:17.000000 meta-vino-3.6.10/
--rw-rw-r--   0 cash      (1000) cash      (1000)      285 2023-06-09 13:27:17.000000 meta-vino-3.6.10/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)       40 2022-11-09 06:00:33.000000 meta-vino-3.6.10/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-09 13:27:17.000000 meta-vino-3.6.10/meta_vino.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      285 2023-06-09 13:27:17.000000 meta-vino-3.6.10/meta_vino.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)      560 2023-06-09 13:27:17.000000 meta-vino-3.6.10/meta_vino.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-06-09 13:27:17.000000 meta-vino-3.6.10/meta_vino.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       47 2023-06-09 13:27:17.000000 meta-vino-3.6.10/meta_vino.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-06-09 13:27:17.000000 meta-vino-3.6.10/meta_vino.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-06-09 13:17:04.000000 meta-vino-3.6.10/meta_vino.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-09 13:27:17.000000 meta-vino-3.6.10/metavino/
--rw-rw-r--   0 cash      (1000) cash      (1000)      139 2023-06-09 09:59:52.000000 meta-vino-3.6.10/metavino/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-09 13:27:17.000000 meta-vino-3.6.10/metavino/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)      313 2023-06-09 09:59:37.000000 meta-vino-3.6.10/metavino/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2549 2022-11-10 09:22:51.000000 meta-vino-3.6.10/metavino/app/instance_segment_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1679 2022-11-09 08:30:52.000000 meta-vino-3.6.10/metavino/app/object_classification_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      275 2022-11-08 11:30:35.000000 meta-vino-3.6.10/metavino/app/object_detection_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      990 2022-11-08 12:47:07.000000 meta-vino-3.6.10/metavino/app/onnx_to_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1889 2022-11-10 08:16:13.000000 meta-vino-3.6.10/metavino/app/saliency_segment_vino.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4507 2023-06-09 11:23:11.000000 meta-vino-3.6.10/metavino/app/yolo_segment_vino.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-09 13:27:17.000000 meta-vino-3.6.10/metavino/model_zoo/
--rw-rw-r--   0 cash      (1000) cash      (1000)        0 2022-11-08 11:30:50.000000 meta-vino-3.6.10/metavino/model_zoo/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-09 13:27:17.000000 meta-vino-3.6.10/metavino/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)       23 2022-11-08 12:00:00.000000 meta-vino-3.6.10/metavino/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     8033 2023-06-09 10:18:29.000000 meta-vino-3.6.10/metavino/utils/general.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-06-09 13:27:17.000000 meta-vino-3.6.10/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      674 2023-06-09 11:22:59.000000 meta-vino-3.6.10/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 10:31:06.000000 meta-vino-3.6.20/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      285 2023-06-20 10:31:06.000000 meta-vino-3.6.20/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)       40 2022-11-09 06:00:33.000000 meta-vino-3.6.20/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      285 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)      560 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       47 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-06-20 10:31:06.000000 meta-vino-3.6.20/meta_vino.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 10:31:06.000000 meta-vino-3.6.20/metavino/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      139 2023-06-09 09:59:52.000000 meta-vino-3.6.20/metavino/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 10:31:06.000000 meta-vino-3.6.20/metavino/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      313 2023-06-09 09:59:37.000000 meta-vino-3.6.20/metavino/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2549 2022-11-10 09:22:51.000000 meta-vino-3.6.20/metavino/app/instance_segment_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1679 2022-11-09 08:30:52.000000 meta-vino-3.6.20/metavino/app/object_classification_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      275 2022-11-08 11:30:35.000000 meta-vino-3.6.20/metavino/app/object_detection_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      990 2022-11-08 12:47:07.000000 meta-vino-3.6.20/metavino/app/onnx_to_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1889 2022-11-10 08:16:13.000000 meta-vino-3.6.20/metavino/app/saliency_segment_vino.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4340 2023-06-20 10:24:32.000000 meta-vino-3.6.20/metavino/app/yolo_segment_vino.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 10:31:06.000000 meta-vino-3.6.20/metavino/model_zoo/
+-rw-rw-r--   0 cash      (1000) cash      (1000)        0 2022-11-08 11:30:50.000000 meta-vino-3.6.20/metavino/model_zoo/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-06-20 10:31:06.000000 meta-vino-3.6.20/metavino/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       23 2022-11-08 12:00:00.000000 meta-vino-3.6.20/metavino/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7238 2023-06-20 10:28:43.000000 meta-vino-3.6.20/metavino/utils/general.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-06-20 10:31:06.000000 meta-vino-3.6.20/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      674 2023-06-20 10:29:54.000000 meta-vino-3.6.20/setup.py
```

### Comparing `meta-vino-3.6.10/meta_vino.egg-info/SOURCES.txt` & `meta-vino-3.6.20/meta_vino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meta-vino-3.6.10/metavino/app/instance_segment_vino.py` & `meta-vino-3.6.20/metavino/app/instance_segment_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-3.6.10/metavino/app/object_classification_vino.py` & `meta-vino-3.6.20/metavino/app/object_classification_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-3.6.10/metavino/app/onnx_to_vino.py` & `meta-vino-3.6.20/metavino/app/onnx_to_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-3.6.10/metavino/app/saliency_segment_vino.py` & `meta-vino-3.6.20/metavino/app/saliency_segment_vino.py`

 * *Files identical despite different names*

### Comparing `meta-vino-3.6.10/metavino/app/yolo_segment_vino.py` & `meta-vino-3.6.20/metavino/app/yolo_segment_vino.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import cv2
 import numpy as np
 from openvino.runtime import Core
 from ..utils import preproc, postprocess, sigmoid, fast_dot
 
 
 class YoloSegmentVino:
-    def __init__(self, xml_file="models/model.xml"):
+    def __init__(self, xml_file="models/model.xml", v8=False):
         self.xml_file = xml_file
         ie = Core()
         self.model = ie.read_model(model=self.xml_file)
         self.compiled_model = ie.compile_model(model=self.model, device_name="CPU")
         self.input_layer = self.compiled_model.input(0)
-        self.mask_layer = self.compiled_model.output(4)
+        self.feature_size = (self.input_layer.shape[2] // 4, self.input_layer.shape[3] // 4)  # (h, w)
+        self.mask_layer = self.compiled_model.output(1) if v8 else self.compiled_model.output(4)
         self.output_layer = self.compiled_model.output(0)
         self.mean = None
         self.std = None
+        self.v8 = v8
 
     @staticmethod
     def get_rect(mask):
         h, w = mask.shape[:2]
         _, pred = cv2.threshold(mask, 128, 255, cv2.THRESH_BINARY)
         contours, _ = cv2.findContours(pred, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
         if len(contours) < 1:
@@ -27,42 +29,30 @@
         area = [cv2.contourArea(c) for c in contours]
         max_idx = np.argmax(area)
         min_rect = cv2.minAreaRect(contours[max_idx])
         min_rect = cv2.boxPoints(min_rect)
 
         return min_rect
 
-    def predict(self, image, conf=0.25, iou=0.6, use_mask=False, use_cupy=False):
+    def predict(self, image, use_preprocess=True, conf=0.25, iou=0.6, use_mask=False):
         dets = []
         size_h, size_w = self.input_layer.shape[2], self.input_layer.shape[3]
-        img, ratio = preproc(image, (size_h, size_w), self.mean, self.std)
+        img, ratio = preproc(image, (size_h, size_w), self.mean, self.std) if use_preprocess else (image, 1.0)
         outputs = self.compiled_model([img[np.newaxis, :]])
 
-        pred = outputs[self.output_layer][0]
-        boxes = postprocess(pred, ratio=1., score_thr=conf, nms_thr=iou)
+        pred = outputs[self.output_layer][0].T if self.v8 else outputs[self.output_layer][0]
+        boxes = postprocess(pred, ratio=1., score_thr=conf, nms_thr=iou, v8=self.v8)
         if boxes is None: return dets
 
         if use_mask:
             proto = outputs[self.mask_layer]
-
-            if use_cupy:
-                import cupy as cp
-
-                gpu_data0 = cp.asarray(proto)
-                gpu_proto = cp.reshape(gpu_data0, (1, 32, -1))[0]
-                gpu_boxes = cp.asarray(boxes[:, 6:])
-                gpu_dot = cp.dot(gpu_boxes, gpu_proto)
-                gpu_sigmoid_dot = 1 / (1 + cp.exp(-gpu_dot))
-                gpu_masks = cp.reshape(gpu_sigmoid_dot, (-1, 160, 160))
-                masks = cp.asnumpy(gpu_masks)
-                ih, iw = 160 / size_h, 160 / size_w
-            else:
-                proto = np.reshape(proto, (1, 32, -1))[0]
-                masks = np.reshape(sigmoid(fast_dot(boxes[:, 6:], proto)), (-1, 160, 160))
-                ih, iw = 160 / size_h, 160 / size_w
+            proto = np.reshape(proto, (1, 32, -1))[0]
+            masks = np.reshape(sigmoid(fast_dot(boxes[:, 6:], proto)),
+                               (-1, self.feature_size[0], self.feature_size[1]))
+            ih, iw = self.feature_size[0] / size_h, self.feature_size[1] / size_w
 
             for mask, box, score, label in zip(masks, boxes[:, :4], boxes[:, 4], boxes[:, 5]):
                 x1, y1, x2, y2 = box[0] * iw, box[1] * ih, box[2] * iw, box[3] * ih
                 crop = mask[int(y1):int(y2) + 1, int(x1):int(x2) + 1] * 255
                 min_rect = self.get_rect(crop.astype(np.uint8))
                 rect = [[(r[0] + x1) / ih / ratio, (r[1] + y1) / iw / ratio] for r in min_rect]
                 dets.append([max(int(rect[0][0]), 0), max(int(rect[0][1]), 0),
```

### Comparing `meta-vino-3.6.10/metavino/utils/general.py` & `meta-vino-3.6.20/metavino/utils/general.py`

 * *Files 8% similar despite different names*

```diff
@@ -146,38 +146,14 @@
 
         inds = np.where(ovr <= nms_thr)[0]
         order = order[inds + 1]
 
     return keep
 
 
-def multiclass_nms(boxes, scores, nms_thr, score_thr):
-    """Multiclass NMS implemented in Numpy"""
-    final_dets = []
-    num_classes = scores.shape[1]
-    for cls_ind in range(num_classes):
-        cls_scores = scores[:, cls_ind]
-        valid_score_mask = cls_scores > score_thr
-        if valid_score_mask.sum() == 0:
-            continue
-        else:
-            valid_scores = cls_scores[valid_score_mask]
-            valid_boxes = boxes[valid_score_mask]
-            keep = nms(valid_boxes, valid_scores, nms_thr)
-            if len(keep) > 0:
-                cls_inds = np.ones((len(keep), 1)) * cls_ind
-                dets = np.concatenate(
-                    [valid_boxes[keep], valid_scores[keep, None], cls_inds], 1
-                )
-                final_dets.append(dets)
-    if len(final_dets) == 0:
-        return None
-    return np.concatenate(final_dets, 0)
-
-
 def preproc(image, input_size, mean, std, swap=(2, 0, 1)):
     if len(image.shape) == 3:
         padded_img = np.ones((input_size[0], input_size[1], 3)) * 114.0
     else:
         padded_img = np.ones(input_size) * 114.0
     img = np.array(image)
     r = min(input_size[0] / img.shape[0], input_size[1] / img.shape[1])
@@ -211,18 +187,18 @@
     if std is not None:
         padded_img /= np.array(std)
     padded_img = padded_img.transpose(swap)
     padded_img = np.ascontiguousarray(padded_img, dtype=np.float32)
     return padded_img
 
 
-def multiclass_nms(boxes, scores, nms_thr, score_thr, predictions=None):
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
@@ -231,30 +207,30 @@
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
 
 
-def postprocess(predictions, ratio, score_thr, nms_thr):
+def postprocess(predictions, ratio, score_thr, nms_thr, v8=False):
     boxes = predictions[:, :4]
-    scores = predictions[:, 4:5] * predictions[:, 5:-32]
+    scores = predictions[:, 4:-32] if v8 else predictions[:, 4:5] * predictions[:, 5:-32]
     boxes_xyxy = np.ones_like(boxes)
     boxes_xyxy[:, 0] = boxes[:, 0] - boxes[:, 2] / 2.
     boxes_xyxy[:, 1] = boxes[:, 1] - boxes[:, 3] / 2.
     boxes_xyxy[:, 2] = boxes[:, 0] + boxes[:, 2] / 2.
     boxes_xyxy[:, 3] = boxes[:, 1] + boxes[:, 3] / 2.
     boxes_xyxy /= ratio
 
-    dets = multiclass_nms(boxes_xyxy, scores, nms_thr=nms_thr, score_thr=score_thr, predictions=predictions)
+    dets = singleclass_nms(boxes_xyxy, scores, nms_thr=nms_thr, score_thr=score_thr, predictions=predictions, v8=v8)
 
     return dets
```

### Comparing `meta-vino-3.6.10/setup.py` & `meta-vino-3.6.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     'opencv-python',
     'setuptools',
     'openvino',
     'numpy',
     'pillow',
 ]
 
-__version__ = 'V3.06.10'
+__version__ = 'V3.06.20'
 
 setup(
     name='meta-vino',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
     url='https://github.com/CachCheng/cvopenvino',
```

