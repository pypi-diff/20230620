# Comparing `tmp/mask2bbox-0.0.7.tar.gz` & `tmp/mask2bbox-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask2bbox-0.0.7.tar", last modified: Wed May 10 08:36:28 2023, max compression
+gzip compressed data, was "mask2bbox-0.0.8.tar", last modified: Tue Jun 20 14:33:55 2023, max compression
```

## Comparing `mask2bbox-0.0.7.tar` & `mask2bbox-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:28.420374 mask2bbox-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-10 08:36:28.420374 mask2bbox-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:36:28.420374 mask2bbox-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:28.412374 mask2bbox-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:28.416374 mask2bbox-0.0.7/src/mask2bbox/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/src/mask2bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/src/mask2bbox/_bboxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/src/mask2bbox/mask2bbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:28.416374 mask2bbox-0.0.7/src/mask2bbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-10 08:36:28.000000 mask2bbox-0.0.7/src/mask2bbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-10 08:36:28.000000 mask2bbox-0.0.7/src/mask2bbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:36:28.000000 mask2bbox-0.0.7/src/mask2bbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 08:36:28.000000 mask2bbox-0.0.7/src/mask2bbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 08:36:28.000000 mask2bbox-0.0.7/src/mask2bbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:28.416374 mask2bbox-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:28.416374 mask2bbox-0.0.7/tests/test_mask2bbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/tests/test_mask2bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 08:36:17.000000 mask2bbox-0.0.7/tests/test_mask2bbox/test_mask2bbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:55.585099 mask2bbox-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-20 14:33:55.585099 mask2bbox-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:33:55.585099 mask2bbox-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:55.577099 mask2bbox-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:55.581099 mask2bbox-0.0.8/src/mask2bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/src/mask2bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17797 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/src/mask2bbox/_bboxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/src/mask2bbox/mask2bbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:55.581099 mask2bbox-0.0.8/src/mask2bbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-20 14:33:55.000000 mask2bbox-0.0.8/src/mask2bbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 14:33:55.000000 mask2bbox-0.0.8/src/mask2bbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:33:55.000000 mask2bbox-0.0.8/src/mask2bbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 14:33:55.000000 mask2bbox-0.0.8/src/mask2bbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 14:33:55.000000 mask2bbox-0.0.8/src/mask2bbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:55.581099 mask2bbox-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:55.585099 mask2bbox-0.0.8/tests/test_mask2bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/tests/test_mask2bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/tests/test_mask2bbox/test_mask2bbox.py
```

### Comparing `mask2bbox-0.0.7/LICENSE.txt` & `mask2bbox-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mask2bbox-0.0.7/PKG-INFO` & `mask2bbox-0.0.8/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,88 @@
-Metadata-Version: 2.1
-Name: mask2bbox
-Version: 0.0.7
-Summary: Gets the bounding boxes from a mask file.
-Home-page: https://github.com/SchapiroLabor/mask2bbox
-Author: Miguel Ibarra
-Author-email: c180l058j@mozmail.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 # mask2bbox
 [![PyPI](https://img.shields.io/pypi/v/mask2bbox?style=flat-square)](https://pypi.org/project/mask2bbox/)
 
 For a given mask, gets the coordinates of bounding box of each element of the mask. It will also allow for more operations in the future.
 
 ## Instalation
 
 `pip install mask2bbox`
 
 ## Usage
 
 ```python
+import numpy as np
 from mask2bbox import BBoxes
 
 # Create a BBoxes object
-all_boxes = BBoxes("path/to/mask.png")
+all_boxes = BBoxes.from_mask("path/to/mask.png")
 
 # Expand the bounding boxes
-all_boxes.expand(n=10)
+all_boxes = all_boxes.expand(n=10)
 
 # Remove the bounding boxes that are located on the edge of the image
-all_boxes.remove_edge_boxes()
-
-# Get the area of all the bounding boxes
-araa = all_boxes.get_bbox_areas()
+all_boxes = all_boxes.remove_from_edge()
 
-# Get the dimensions on x and y of all the bounding boxes
-dims = all_boxes.get_bbox_dims()
+# Get the sides of all the bounding boxes
+sides = all_boxes.get("sides")
 
-# Get the center of all the bounding boxes
-centers = all_boxes.get_bbox_centers()
-
-# Get the ratio x/y of all the bounding boxes
-ratios = all_boxes.get_bbox_ratios()
+# Filter the bounding boxes by the sides
+filtered_boxes = all_boxes.filter("sides", np.greater_equal, (35, 35))
 
 # Get the IoU matrix of all the bounding boxes
-iou = all_boxes.iou_matrix()
+iou = filtered_boxes.iou_matrix()
 
 # Save the IoU matrix to a csv file
-all_boxes.save_iou("path/to/save/iou.csv")
+filtered_boxes.save_iou("path/to/save/iou.csv")
 
 # Plot the bounding boxes on the mask image
-all_boxes.plot_to_mask("path/to/save/image.png")
+filtered_boxes.plot_to_mask("path/to/save/image.png")
 
 # Save your bounding boxes
-all_boxes.save_csv("path/to/bounding_boxes.csv")
+filtered_boxes.save_csv("path/to/bounding_boxes.csv")
+
+# Get resize factors to resize the bounding boxes to a given size
+resize_factors = filtered_boxes.de(desired_ratio=0.7, size=(256, 256))
+
+# Extract the bounding boxes as images
+filtered_boxes.extract(resize_factors, size=(256, 256), output="path/to/save/images")
 ```
 
 ## Version Notes
+
+### 0.0.8 - Change methods, change constructor, added functionality. 
+- **Constructor:** BBox object is now constructed with the syntax `BBoxes.from_mask(mask)` instead of `BBoxes(mask)`.
+- **Operations:** BBox object operations are no longer performed in place, the affected methods are:
+  - `BBoxes.remove_from_edge()`
+  - `BBoxes.expand()`
+  - `BBoxes.filter()`
+
+- **Removed methods:**
+  - `is_area_smaller_than()`
+  - `is_area_larger_than()`
+  - `are_dims_smaller_than()`
+  - `are_dims_larger_than()`
+  - `filter_identities()`  
+
+These methods used in-place operations and are no longer needed, they were substituted with.  
+- **Renamed:**
+  - `BBoxes.get_bbox_areas()` -> `BBoxes.get_areas()`
+  - `BBoxes.get_bbox_dims()` -> `BBoxes.get_sizes()`
+  - `BBoxes.get_bbox_centers()` -> `BBoxes.get_centers()`
+  - `BBoxes.get_bbox_ratios()` -> `BBoxes.get_ratios()`
+  
+- **New methods:**
+  - `BBoxes.filter():` This method allows to filter the bounding boxes by any of the attributes in the object specifying the comparison operator and threshold value. It returns a new BBoxes object with the filtered values.
+  - `BBoxes.get():` This method allows to get the values of the attributes in the object. It works as a simplification to `BBoxes.get_areas()`, `BBoxes.get_centers()`, `BBoxes.get_sizes()` and `BBoxes.get_ratios()`.
+  - `BBoxes.extract():` This new method isolates the bounding boxes as images and saves them to the desired location.
+  - `BBoxes.calculate_resizing_factor():` This method calculates the resizing factor needed to resize the bounding boxes to a given size.
+  - `BBoxes._pad_crop():` Helper method to pad or crop the bounding boxes to a desired output size.
+  - `BBoxes.plot_to_image():` This method plots the bounding boxes to the corresponding image and saves it to the desired location.
+
+
 ### 0.0.7 - Improved functionality
 Improvements in IoU calculation
 
 ### 0.0.6 - Added functionality
 
 ### 0.0.5 - Added functionality
```

### Comparing `mask2bbox-0.0.7/setup.py` & `mask2bbox-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mask2bbox",
-    version="0.0.7",
+    version="0.0.8",
     description="Gets the bounding boxes from a mask file.",
     url="https://github.com/SchapiroLabor/mask2bbox",
     author="Miguel Ibarra",
     author_email="c180l058j@mozmail.com",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

