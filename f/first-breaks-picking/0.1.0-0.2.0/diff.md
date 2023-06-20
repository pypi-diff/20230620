# Comparing `tmp/first-breaks-picking-0.1.0.tar.gz` & `tmp/first-breaks-picking-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "first-breaks-picking-0.1.0.tar", last modified: Sun Jun  4 19:06:09 2023, max compression
+gzip compressed data, was "first-breaks-picking-0.2.0.tar", last modified: Tue Jun 20 18:34:08 2023, max compression
```

## Comparing `first-breaks-picking-0.1.0.tar` & `first-breaks-picking-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,56 @@
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-04 19:06:09.156089 first-breaks-picking-0.1.0/
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    11357 2023-06-04 18:14:03.000000 first-breaks-picking-0.1.0/LICENSE
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    19116 2023-06-04 19:06:09.156089 first-breaks-picking-0.1.0/PKG-INFO
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    17922 2023-06-04 18:58:50.000000 first-breaks-picking-0.1.0/README.md
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-04 19:06:09.156089 first-breaks-picking-0.1.0/first_breaks/
--rw-rw-r--   0 daloro    (1000) daloro    (1000)        0 2023-06-04 18:14:03.000000 first-breaks-picking-0.1.0/first_breaks/__init__.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)      352 2023-06-04 18:55:43.000000 first-breaks-picking-0.1.0/first_breaks/cli.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     1069 2023-06-04 18:33:16.000000 first-breaks-picking-0.1.0/first_breaks/const.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-04 19:06:09.156089 first-breaks-picking-0.1.0/first_breaks/desktop/
--rw-rw-r--   0 daloro    (1000) daloro    (1000)        0 2023-06-04 18:14:03.000000 first-breaks-picking-0.1.0/first_breaks/desktop/__init__.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    15314 2023-06-04 18:46:15.000000 first-breaks-picking-0.1.0/first_breaks/desktop/graph.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    14877 2023-06-04 18:42:03.000000 first-breaks-picking-0.1.0/first_breaks/desktop/main_gui.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     4781 2023-06-04 18:46:41.000000 first-breaks-picking-0.1.0/first_breaks/desktop/picking_widget.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     2146 2023-06-04 18:40:15.000000 first-breaks-picking-0.1.0/first_breaks/desktop/threads.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     1008 2023-06-04 18:55:33.000000 first-breaks-picking-0.1.0/first_breaks/desktop/warn_widget.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-04 19:06:09.156089 first-breaks-picking-0.1.0/first_breaks/picking/
--rw-rw-r--   0 daloro    (1000) daloro    (1000)        0 2023-06-04 18:14:03.000000 first-breaks-picking-0.1.0/first_breaks/picking/__init__.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     2662 2023-06-04 18:33:16.000000 first-breaks-picking-0.1.0/first_breaks/picking/picker.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     7682 2023-06-04 18:49:17.000000 first-breaks-picking-0.1.0/first_breaks/picking/task.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)      437 2023-06-04 18:33:16.000000 first-breaks-picking-0.1.0/first_breaks/picking/utils.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-04 19:06:09.156089 first-breaks-picking-0.1.0/first_breaks/sgy/
--rw-rw-r--   0 daloro    (1000) daloro    (1000)        0 2023-06-04 18:14:03.000000 first-breaks-picking-0.1.0/first_breaks/sgy/__init__.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     7799 2023-06-04 18:33:16.000000 first-breaks-picking-0.1.0/first_breaks/sgy/headers.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    13219 2023-06-04 18:55:47.000000 first-breaks-picking-0.1.0/first_breaks/sgy/reader.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-04 19:06:09.156089 first-breaks-picking-0.1.0/first_breaks/utils/
--rw-rw-r--   0 daloro    (1000) daloro    (1000)        0 2023-06-04 18:14:03.000000 first-breaks-picking-0.1.0/first_breaks/utils/__init__.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)      635 2023-06-04 18:14:03.000000 first-breaks-picking-0.1.0/first_breaks/utils/debug.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     3286 2023-06-04 18:55:30.000000 first-breaks-picking-0.1.0/first_breaks/utils/utils.py
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     3815 2023-06-04 18:14:03.000000 first-breaks-picking-0.1.0/first_breaks/utils/visualizations.py
-drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-04 19:06:09.156089 first-breaks-picking-0.1.0/first_breaks_picking.egg-info/
--rw-rw-r--   0 daloro    (1000) daloro    (1000)    19116 2023-06-04 19:06:09.000000 first-breaks-picking-0.1.0/first_breaks_picking.egg-info/PKG-INFO
--rw-rw-r--   0 daloro    (1000) daloro    (1000)      903 2023-06-04 19:06:09.000000 first-breaks-picking-0.1.0/first_breaks_picking.egg-info/SOURCES.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)        1 2023-06-04 19:06:09.000000 first-breaks-picking-0.1.0/first_breaks_picking.egg-info/dependency_links.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)       71 2023-06-04 19:06:09.000000 first-breaks-picking-0.1.0/first_breaks_picking.egg-info/entry_points.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)      123 2023-06-04 19:06:09.000000 first-breaks-picking-0.1.0/first_breaks_picking.egg-info/requires.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)       13 2023-06-04 19:06:09.000000 first-breaks-picking-0.1.0/first_breaks_picking.egg-info/top_level.txt
--rw-rw-r--   0 daloro    (1000) daloro    (1000)      337 2023-06-04 19:06:09.156089 first-breaks-picking-0.1.0/setup.cfg
--rw-rw-r--   0 daloro    (1000) daloro    (1000)     1980 2023-06-04 19:04:08.000000 first-breaks-picking-0.1.0/setup.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    11357 2023-05-10 12:43:20.000000 first-breaks-picking-0.2.0/LICENSE
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)    23658 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/PKG-INFO
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    22444 2023-06-20 18:03:09.000000 first-breaks-picking-0.2.0/README.md
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.2.0/first_breaks/__init__.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/_pytorch/
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/_pytorch/models/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-06-14 14:08:31.000000 first-breaks-picking-0.2.0/first_breaks/_pytorch/models/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     5730 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/_pytorch/models/unet3plus.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      352 2023-06-12 06:38:44.000000 first-breaks-picking-0.2.0/first_breaks/cli.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1171 2023-06-14 14:08:31.000000 first-breaks-picking-0.2.0/first_breaks/const.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/desktop/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.2.0/first_breaks/desktop/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    17108 2023-06-20 18:20:30.000000 first-breaks-picking-0.2.0/first_breaks/desktop/graph.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    17672 2023-06-20 18:24:58.000000 first-breaks-picking-0.2.0/first_breaks/desktop/main_gui.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     6739 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/desktop/picking_widget.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     2700 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/desktop/threads.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     2394 2023-06-20 18:22:43.000000 first-breaks-picking-0.2.0/first_breaks/desktop/utils.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/picking/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-30 07:39:18.000000 first-breaks-picking-0.2.0/first_breaks/picking/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      955 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/picking/ipicker.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     4952 2023-06-20 13:01:25.000000 first-breaks-picking-0.2.0/first_breaks/picking/picker_onnx.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     8990 2023-06-20 18:09:50.000000 first-breaks-picking-0.2.0/first_breaks/picking/task.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      437 2023-06-12 06:38:44.000000 first-breaks-picking-0.2.0/first_breaks/picking/utils.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/sgy/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.2.0/first_breaks/sgy/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     7843 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/sgy/headers.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)    14416 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/sgy/reader.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks/utils/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-05-10 12:43:20.000000 first-breaks-picking-0.2.0/first_breaks/utils/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      635 2023-05-10 12:43:20.000000 first-breaks-picking-0.2.0/first_breaks/utils/debug.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     4191 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/first_breaks/utils/utils.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     3815 2023-05-26 13:27:32.000000 first-breaks-picking-0.2.0/first_breaks/utils/visualizations.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)    23658 2023-06-20 18:34:08.000000 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/PKG-INFO
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)     1290 2023-06-20 18:34:08.000000 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/SOURCES.txt
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)        1 2023-06-20 18:34:08.000000 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/dependency_links.txt
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)       71 2023-06-20 18:34:08.000000 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/entry_points.txt
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)      168 2023-06-20 18:34:08.000000 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/requires.txt
+-rw-rw-r--   0 daloro    (1000) daloro    (1000)       19 2023-06-20 18:34:08.000000 first-breaks-picking-0.2.0/first_breaks_picking.egg-info/top_level.txt
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      337 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/setup.cfg
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     2229 2023-06-20 18:30:32.000000 first-breaks-picking-0.2.0/setup.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/tests/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)      330 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_demo_sgy.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/tests/test_desktop/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_desktop/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_desktop/test_graph.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1559 2023-06-20 14:17:10.000000 first-breaks-picking-0.2.0/tests/test_markdown_examples.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/tests/test_picking/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_picking/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1288 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_picking/test_picker.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     3329 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_picking/test_task.py
+drwxrwxr-x   0 daloro    (1000) daloro    (1000)        0 2023-06-20 18:34:08.753592 first-breaks-picking-0.2.0/tests/test_sgy/
+-rw-r--r--   0 daloro    (1000) daloro    (1000)        0 2023-06-19 06:24:05.000000 first-breaks-picking-0.2.0/tests/test_sgy/__init__.py
+-rw-r--r--   0 daloro    (1000) daloro    (1000)     1867 2023-06-20 14:27:17.000000 first-breaks-picking-0.2.0/tests/test_sgy/test_reader.py
```

### Comparing `first-breaks-picking-0.1.0/LICENSE` & `first-breaks-picking-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.1.0/PKG-INFO` & `first-breaks-picking-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: first-breaks-picking
-Version: 0.1.0
-Summary: Tool for picking first breaks in seismic gather
-Home-page: https://github.com/DaloroAT/first_breaks_picking
-Author: Aleksei Tarasov
-Author-email: aleksei.v.tarasov@gmail.com
-License: Apache License 2.0
-Project-URL: Homepage, https://github.com/DaloroAT/first_breaks_picking
-Keywords: seismic,first-breaks,computer-vision,deep-learning,segmentation,data-science
-Classifier: Environment :: Console
-Classifier: Environment :: X11 Applications :: Qt
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7,<4.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # First breaks picking
 This project is devoted to pick waves that are the first to be detected on a seismogram (first breaks, first arrivals).
 Traditionally, this procedure is performed manually. When processing field data, the number of picks reaches hundreds of
 thousands. Existing analytical methods allow you to automate picking only on high-quality data with a high
 signal / noise ratio.
 
 As a more robust algorithm, it is proposed to use a neural network to pick the first breaks. Since the data on adjacent
@@ -98,58 +71,80 @@
 
 ![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_6.png)
 
 </details>
 
 # Installation
 
-Library is available in PyPI:
+Library is available in [PyPI](https://pypi.org/project/first-breaks-picking/):
 ```shell
 pip install -U first-breaks-picking
 ```
 
+### GPU support
+
+You can use the capabilities of GPU to significantly reduce picking time. Before started, check
+[here](https://developer.nvidia.com/cuda-gpus) that your GPU is CUDA compatible.
+
+Install GPU supported version of library:
+```shell
+pip install -U first-breaks-picking[gpu]
+```
+
+The following steps are operating system dependent and must be performed manually:
+
+- Install [latest NVIDIA drivers](https://www.nvidia.com/Download/index.aspx).
+- Install [CUDA toolkit](https://developer.nvidia.com/cuda-downloads).
+**The version must be between 11.x, starting with 11.6. Version 12 is not supported**.
+- Install ZLib and CuDNN:
+[Windows](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html#install-windows) and
+[Linux](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html#install-linux).
+
 ### Extra data
 
 - To pick first breaks you need
 to [download model](https://oml.daloroserver.com/download/seis/fb.onnx).
 
 - If you have no seismic data, you can also
 [download small SGY file](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/data/real_gather.sgy).
 
 It's also possible to download them with Python using the following snippet:
 
+[code-block-start]:downloading-extra
 ```python
 from first_breaks.utils.utils import (download_demo_sgy,
                                       download_model_onnx)
 
 sgy_filename = 'data.sgy'
 model_filename = 'model.onnx'
 
 download_demo_sgy(sgy_filename)
 download_model_onnx(model_filename)
 ```
+[code-block-end]:downloading-extra
 
 # How to use it
 
 The library can be used in Python, or you can use the desktop application.
 
 ## Python
 
 Programmatic way has more flexibility for building your own picking scenario and processing multiple files.
 
 ### Minimal example
 
 The following snippet implements the picking process of the demo file. As a result, you can get an image from
 the project preview.
 
+[code-block-start]:e2e-example
 ```python
 from first_breaks.utils.utils import download_demo_sgy
 from first_breaks.sgy.reader import SGY
 from first_breaks.picking.task import Task
-from first_breaks.picking.picker import PickerONNX
+from first_breaks.picking.picker_onnx import PickerONNX
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 download_demo_sgy(fname=sgy_filename)
 sgy = SGY(sgy_filename)
 
 task = Task(sgy_filename,
@@ -170,67 +165,91 @@
              traces_window=(79.5, 90.5),
              show_processing_region=False,
              headers_total_pixels=80,
              height=500,
              width=700,
              hide_traces_axis=True)
 ```
+[code-block-end]:e2e-example
 
 For a better understanding of the steps taken, expand and read the next section.
 
 ### Detailed examples
 
 <details>
 
 <summary>Show examples</summary>
 
+### Download demo SGY
+
+Let's download the demo file. All the following examples assume that the file is downloaded and saved as `data.sgy`.
+You can also put your own SGY file.
+
+```python
+from first_breaks.utils.utils import download_demo_sgy
+
+sgy_filename = 'data.sgy'
+download_demo_sgy(fname=sgy_filename)
+```
+
 ### Create SGY
 We provide several ways to create `SGY` object: from file, `bytes` or `numpy` array.
 
 From file:
+
+[code-block-start]:init-from-path
 ```python
 from first_breaks.sgy.reader import SGY
 
-sgy_filename = ...  # put path to your file.
+sgy_filename = 'data.sgy'
 sgy = SGY(sgy_filename)
 ```
+[code-block-end]:init-from-path
 
 From `bytes`:
+
+[code-block-start]:init-from-bytes
 ```python
 from first_breaks.sgy.reader import SGY
 
-sgy_filename = ...  # put path to your file.
+sgy_filename = 'data.sgy'
 
 with open(sgy_filename, 'rb') as fin:
     sgy_bytes = fin.read()
 
 sgy = SGY(sgy_bytes)
 ```
+[code-block-end]:init-from-bytes
 
 If you want to create from `numpy` array, extra argument `dt_mcs` is required:
+
+[code-block-start]:init-from-np
 ```python
 import numpy as np
 from first_breaks.sgy.reader import SGY
 
 num_samples = 1000
 num_traces = 48
 dt_mcs = 1e3
 
 traces = np.random.random((num_samples, num_traces))
 sgy = SGY(traces, dt_mcs=dt_mcs)
 ```
+[code-block-end]:init-from-np
 
 ### Content of SGY
 
 Created `SGY` allows you to read traces, get observation parameters and view headers (empty if created from `numpy`)
 
+[code-block-start]:sgy-content
 ```python
 from first_breaks.sgy.reader import SGY
 
-sgy: SGY = ...  # put here previously created SGY
+sgy_filename = 'data.sgy'
+sgy = SGY(sgy_filename)
 
 # get all traces or specific traces limited by time
 all_traces = sgy.read()
 block_of_data = sgy.read_traces_by_ids(ids=[1, 2, 3, 10],
                                        min_sample=100,
                                        max_sample=500)
 
@@ -244,64 +263,114 @@
 print(sgy.dt, sgy.dt_mcs, sgy.dt_ms)
 
 # dict with headers in the first 3600 bytes of the file
 print(sgy.general_headers)
 # pandas DataFrame with headers for each trace
 print(sgy.traces_headers.head())
 ```
+[code-block-end]:sgy-content
 
 ### Create task for picking
 
 Next, we create a task for picking and pass the picking parameters to it. They have default values, but for the
 best quality, they must be matched to specific data. You can use the desktop application to evaluate the parameters.
 A detailed description of the parameters can be found  in the `Picking process` chapter.
 
+[code-block-start]:create-task
 ```python
 from first_breaks.sgy.reader import SGY
 from first_breaks.picking.task import Task
 
-sgy: SGY = ...  # put here previously created SGY
+sgy_filename = 'data.sgy'
+sgy = SGY(sgy_filename)
+
 task = Task(sgy,
             traces_per_gather=24,
             maximum_time=200)
 ```
+[code-block-end]:create-task
+
+
+### Create Picker
+In this step, we instantiate the neural network for picking. If you downloaded the model according to the
+installation section, then pass the path to it. Or leave the path to the model empty so that we can download it
+automatically.
+
+It's also possible to use GPU/CUDA to accelerate computation. By default `cuda` is selected if you have finished
+all steps regarding GPU in `Installation` section. Otherwise, it's `cpu`.
+
+You can also set the value of parameter `batch_size`, which can further speed up the calculations on the GPU.
+However, this will require additional video memory (VRAM).
+
+NOTE: When using the CPU, increasing `batch_size` does not speed up the calculation at all, but it may
+require additional memory costs (RAM). So don't increase this parameter when using CPU.
+
+[code-block-start]:create-picker
+```python
+from first_breaks.picking.picker_onnx import PickerONNX
+
+# the library will determine the best available device
+picker_default = PickerONNX()
+
+# create picker explicitly on CPU
+picker_cpu = PickerONNX(device='cpu')
+
+# create picker explicitly on GPU
+picker_gpu = PickerONNX(device='cuda', batch_size=2)
+
+# transfer model to another device
+picker_cpu.change_settings(device='cuda', batch_size=3)
+picker_gpu.change_settings(device='cpu', batch_size=1)
+```
+[code-block-end]:create-picker
 
 ### Pick first breaks
 
-In this step, we use the neural network for picking. If you downloaded the model according to the installation section,
-then pass the path to it. Or leave the path to the model empty so that we can download it automatically.
+Now, using all the created components, we can pick the first breaks and export the results.
 
+[code-block-start]:pick-fb
 ```python
 from first_breaks.picking.task import Task
-from first_breaks.picking.picker import PickerONNX
+from first_breaks.picking.picker_onnx import PickerONNX
+from first_breaks.sgy.reader import SGY
+
+sgy_filename = 'data.sgy'
+sgy = SGY(sgy_filename)
 
-task: Task = ...  # put here previously created task
+task = Task(sgy,
+            traces_per_gather=24,
+            maximum_time=200)
 picker = PickerONNX()
 task = picker.process_task(task)
 
 # you can see results of picking
 print(task.picks_in_samples)
 print(task.picks_in_ms)
 print(task.confidence)
 
 # you can export picks to file as plain text
 task.export_result('result.txt', as_plain=True)
 # or save as json file
-task.export_result('result.json', as_plain=False)
+task.export_result('result.json', as_json=True)
+# or make a copy of source SGY and put picks to 236 byte
+task.export_result('result.segy', as_sgy=True)
 ```
+[code-block-end]:pick-fb
 
 ### Visualizations
 
 You can save the seismogram and picks as an image. We use Qt backend for visualizations. Here we describe some usage
 scenarios.
 
 We've added named arguments to various scenarios for demonstration purposes, but in practice you can
 use them all. See the function arguments for more visualization options.
 
 Plot `SGY` only:
+
+[code-block-start]:plot-sgy
 ```python
 from first_breaks.sgy.reader import SGY
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 image_filename = 'image.png'
 
@@ -309,16 +378,19 @@
 export_image(sgy, image_filename,
              normalize=False,
              traces_window=(5, 10),
              time_window=(0, 200),
              height=300,
              width_per_trace=30)
 ```
+[code-block-end]:plot-sgy
 
 Plot `numpy` traces:
+
+[code-block-start]:plot-np
 ```python
 import numpy as np
 from first_breaks.sgy.reader import SGY
 from first_breaks.desktop.graph import export_image
 
 image_filename = 'image.png'
 num_traces = 48
@@ -331,16 +403,19 @@
              clip=0.5)
 
 # or create SGY as discussed before
 sgy = SGY(traces, dt_mcs=dt_mcs)
 export_image(sgy, image_filename,
              gain=2)
 ```
+[code-block-end]:plot-np
 
 Plot `SGY` with custom picks:
+
+[code-block-start]:plot-sgy-custom-picks
 ```python
 import numpy as np
 from first_breaks.sgy.reader import SGY
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 image_filename = 'image.png'
@@ -349,51 +424,63 @@
 picks_ms = np.random.uniform(low=0,
                              high=sgy.ns * sgy.dt_ms,
                              size=sgy.ntr)
 export_image(sgy, image_filename,
              picks_ms=picks_ms,
              picks_color=(0, 100, 100))
 ```
+[code-block-end]:plot-sgy-custom-picks
 
 Plot result of picking:
+
+[code-block-start]:plot-sgy-real-picks
 ```python
 from first_breaks.picking.task import Task
+from first_breaks.picking.picker_onnx import PickerONNX
 from first_breaks.desktop.graph import export_image
+from first_breaks.sgy.reader import SGY
 
+sgy_filename = 'data.sgy'
 image_filename = 'image.png'
 
-task: Task = ...  # put here previously created task
-# if the task was not finished, then picks will not be drawn
+sgy = SGY(sgy_filename)
+task = Task(sgy,
+            traces_per_gather=24,
+            maximum_time=200)
+picker = PickerONNX()
+task = picker.process_task(task)
 
 export_image(task, image_filename,
              show_processing_region=False,
              fill_black_left=False,
              width=1000)
 ```
+[code-block-end]:plot-sgy-real-picks
 
 ### *Limit processing region
 
 Unfortunately, processing of a part of a file is not currently supported natively. We will add this functionality soon!
 
 However, you can use the following workaround to do this:
 
+[code-block-start]:pick-limited
 ```python
 from first_breaks.sgy.reader import SGY
 
 sgy_filename = 'data.sgy'
-
 sgy = SGY(sgy_filename)
 
 interesting_traces = sgy.read_traces_by_ids(ids=list(range(20, 40)),
                                             min_sample=100,
                                             max_sample=200)
 
 # we create new SGY based on region of interests
 sgy = SGY(interesting_traces, dt_mcs=sgy.dt_mcs)
 ```
+[code-block-end]:pick-limited
 
 </details>
 
 ## Desktop application
 
 ***Application under development***
 
@@ -417,14 +504,15 @@
 Click on 2 button to select SGY. After successful reading you can analyze SGY file.
 
 The following mouse interactions are available:
 - Left button drag / Middle button drag: Pan the scene.
 - Right button drag: Scales the scene. Dragging left/right scales horizontally; dragging up/down scales vertically.
 - Right button click: Open dialog with extra options, such as limit by X/Y axes and export.
 - Wheel spin: Zooms the scene in and out.
+- Left click: *After picking with model*, you can manually change picks.
 
 You can also use slider in toolbar to change gain of traces. **The gain value for the slider is only used for
 visualization, it is not used in picking process**.
 
 ### Load model
 
 To use picker in desktop app you have to download model. See the `Installation` section for instructions
@@ -437,24 +525,36 @@
 
 Click on 3 button to open window with picking parameters. A detailed description of the parameters can be found
 in the `Picking process` chapter. Then run picking process. After some time, a line will appear connecting the first
 arrivals.
 
 Run again with different parameters to achieve optimal values of the picking parameters for your data.
 
+If you have CUDA compatible GPU and installed GPU supported version of library (see `Installation` section), you can
+select `CUDA/GPU` device  to use GPU acceleration. It can drastically decrease computation time.
+
+Parameter `Batch size` determine how many gathers will be processed simultaneously on GPU. It also can decrease
+computation time, but make sure that you have enough free GPU memory (`Batch size=10` requires > 10 Gb VRAM on Windows).
+
 ### Processing grid
 
 Click on 4 button to toggle the display of the processing grid on or off. Horizontal line
 shows `Maximum time` and vertical lines are drawn at intervals equal to `Traces per gather`. The neural network
 processes blocks independently, as separate images.
 
 ### Save results
 
-Click on 5 button to save picks, picking parameters and info about SGY file into plain `.txt` file.
+Click on 5 button to save picks into file. Depending on file extension, results will be saved as `json`,
+as plain `txt`, or as `segy` file.
+
+For extensions `txt` and `json`, picking parameters and model confidence for each peak are additionally saved.
 
+When choosing an extension `segy`, the copy of original SGY file is saved with the values of the first breaks in the
+trace headers. They are stored in the last 4 bytes (236 byte if counting from 0) to be decoded as an unsigned integer.
+Values are in microseconds.
 # Picking process
 
 Neural network process file as series of **images**. There is why **the traces should not be random**,
 since we are using information about adjacent traces.
 
 To obtain the first breaks we do the following steps:
 1) Read all traces in the file.
```

### Comparing `first-breaks-picking-0.1.0/first_breaks/const.py` & `first-breaks-picking-0.2.0/first_breaks/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import os
 from os import environ
 from pathlib import Path
 from sys import platform
 
 
+def is_windows() -> bool:
+    return "win" in platform
+
+
+def is_linux() -> bool:
+    return "linux" in platform
+
+
+def is_macos() -> bool:
+    return "darwin" in platform
+
+
 def get_cache_folder() -> Path:
-    if platform == "linux" or platform == "linux2":
+    if is_linux():
         return Path(environ.get("XDG_CACHE_HOME", Path.home() / ".cache")) / "first_breaks_picking"
-
-    elif platform == "darwin":  # mac os
+    elif is_macos():
         return Path.home() / "Library" / "Caches" / "first_breaks_picking"
-
-    elif platform.startswith("win"):
+    elif is_windows():
         return Path.home() / ".cache" / "first_breaks_picking"
-
     else:
         raise ValueError(f"Unexpected platform {platform}.")
 
 
 PROJECT_ROOT = Path(__file__).parent.parent
 CACHE_FOLDER = get_cache_folder()
```

### Comparing `first-breaks-picking-0.1.0/first_breaks/desktop/graph.py` & `first-breaks-picking-0.2.0/first_breaks/desktop/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import os
 import warnings
 from pathlib import Path
 from typing import Any, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pyqtgraph as pg
 from PyQt5.QtCore import Qt, QTimer, pyqtSlot
 from PyQt5.QtGui import QColor, QFont, QPainterPath, QPen
 from PyQt5.QtWidgets import QApplication
 from pyqtgraph.exporters import ImageExporter
+from pyqtgraph.GraphicsScene.mouseEvents import MouseClickEvent
 
 from first_breaks.const import HIGH_DPI
 from first_breaks.picking.task import Task
 from first_breaks.picking.utils import preprocess_gather
 from first_breaks.sgy.reader import SGY
 
 if HIGH_DPI:
@@ -29,16 +31,16 @@
     picks_color: TColor = (255, 0, 0)
     region_contour_color: TColor = (100, 100, 100)
     region_contour_width: float = 0.2
     region_poly_color: TColor = (100, 100, 100, 50)
 
 
 class GraphWidget(pg.PlotWidget):
-    def __init__(self, *args: Any, **kwargs: Any):
-        super().__init__(*args, **kwargs)
+    def __init__(self, use_open_gl: bool = True, *args: Any, **kwargs: Any):
+        super().__init__(useOpenGL=use_open_gl, *args, **kwargs)
         self.getPlotItem().disableAutoRange()
         self.setAntialiasing(False)
         self.getPlotItem().setClipToView(True)
         self.getPlotItem().setDownsampling(mode="peak")
 
         self.getPlotItem().invertY(True)
         self.getPlotItem().showAxis("top", True)
@@ -52,34 +54,60 @@
         self.x_ax.setLabel("trace", **labelstyle)
         self.y_ax.setLabel("t, ms", **labelstyle)
         self.x_ax.setTickFont(font)
         self.y_ax.setTickFont(font)
         self.plotItem.ctrlMenu = None
 
         self.sgy: Optional[SGY] = None
-        self.picks_as_item: Optional[pg.QtWidgets.QGraphicsPathItem] = None
+        self.picks_in_ms: Optional[np.ndarray] = None
+        self.picks_as_item: Optional[pg.PlotCurveItem] = None
         self.processing_region_as_items: List[pg.QtWidgets.QGraphicsPathItem] = []
         self.traces_as_items: List[pg.QtWidgets.QGraphicsPathItem] = []
+        self.is_picks_modified_manually = False
+
+        self.mouse_click_signal = pg.SignalProxy(self.sceneObj.sigMouseClicked, rateLimit=60, slot=self.mouse_clicked)
+
+    def mouse_clicked(self, ev: Tuple[MouseClickEvent]) -> None:
+        ev = ev[0]
+        if self.picks_as_item is not None and ev.button() == 1:
+            mouse_point = self.getPlotItem().vb.mapSceneToView(ev.scenePos())
+            x, y = mouse_point.x(), mouse_point.y()
+            ids, picks = self.picks_as_item.getData()
+            closest = np.argmin(np.abs(ids - x))
+            y = np.clip(y, 0, self.sgy.max_time_ms)
+            picks[closest] = y
+            self.picks_as_item.setData(ids, picks)
+            self.picks_in_ms = picks
+            self.is_picks_modified_manually = True
+
+    def full_clean(self) -> None:
+        self.remove_picks()
+        self.remove_traces()
+        self.remove_processing_region()
+        self.picks_as_item = None
+        self.picks_in_ms = None
+        self.is_picks_modified_manually = False
+        self.clear()
 
     def plotseis(
         self,
         sgy: SGY,
         clip: float = GraphDefaults.clip,
         gain: float = GraphDefaults.gain,
         normalize: bool = GraphDefaults.normalize,
         fill_black_left: bool = GraphDefaults.fill_black_left,
         refresh_view: bool = True,
     ) -> None:
-
         self.sgy = sgy
-        traces = self.sgy.read()
 
+        traces = self.sgy.read()
         traces = preprocess_gather(traces, gain=gain, clip=clip, normalize=normalize, copy=True)
 
         self.clear()
+
         num_sample, num_traces = self.sgy.shape
         t = np.arange(num_sample) * self.sgy.dt_ms
 
         self.getViewBox().setLimits(xMin=0, xMax=num_traces + 1, yMin=0, yMax=t[-1])
 
         if refresh_view:
             self.getPlotItem().setYRange(0, t[-1])
@@ -119,16 +147,19 @@
         pen.setWidth(0.1)
         item.setPen(pen)
         item.setBrush(Qt.black)
         self.addItem(item)
         self.traces_as_items.append(item)
 
     def remove_picks(self) -> None:
+        self.is_picks_modified_manually = False
         if self.picks_as_item:
             self.removeItem(self.picks_as_item)
+            self.picks_as_item = None
+            self.picks_in_ms = None
 
     def remove_processing_region(self) -> None:
         if self.processing_region_as_items:
             for item in self.processing_region_as_items:
                 self.removeItem(item)
 
     def remove_traces(self) -> None:
@@ -171,21 +202,22 @@
         poly_item.setPen(contour_pen)
         poly_item.setBrush(poly_brush)
         self.processing_region_as_items.append(poly_item)
         self.addItem(poly_item)
 
     def plot_picks(self, picks_ms: Sequence[float], color: TColor = GraphDefaults.picks_color) -> None:
         self.remove_picks()
+        self.is_picks_modified_manually = False
 
-        num_traces = self.sgy.shape[1]
         picks_ms = np.array(picks_ms)
-        ids = np.arange(num_traces) + 1
+        ids = np.arange(self.sgy.num_traces) + 1
 
-        path = pg.arrayToQPath(ids, picks_ms, np.ones(num_traces, dtype=np.int32))
-        self.picks_as_item = pg.QtWidgets.QGraphicsPathItem(path)
+        self.picks_in_ms = picks_ms
+        self.picks_as_item = pg.PlotCurveItem()
+        self.picks_as_item.setData(ids, picks_ms)
 
         pen = pg.mkPen(color=color, width=3)
         self.picks_as_item.setPen(pen)
         self.addItem(self.picks_as_item)
 
 
 class HighMemoryConsumption(Exception):
@@ -203,14 +235,21 @@
 )
 
 
 class GraphExporter(GraphWidget):
     MAX_SIDE_SIZE = 65000
     MAX_NUM_PIXELS = MAX_SIDE_SIZE * 2000
 
+    def __init__(self, *args: Any, **kwargs: Any):
+        os.environ["DEBIAN_FRONTEND"] = "noninteractive"
+        os.environ["LIBGL_ALWAYS_INDIRECT"] = "1"
+        os.environ["QT_QPA_PLATFORM"] = "offscreen"
+        super().__init__(*args, **kwargs)
+        self.setAntialiasing(True)
+
     @classmethod
     def avoid_memory_bomb(
         cls,
         height_image: int,
         width_image: int,
     ) -> None:
 
@@ -284,15 +323,15 @@
         self.clear()
         self.plotseis(
             sgy, normalize=normalize, clip=clip, gain=gain, fill_black_left=fill_black_left, refresh_view=True
         )
 
         if task:
             picks_to_plot = task.picks_in_ms  # type: ignore
-        elif picks_ms:
+        elif picks_ms is not None:
             picks_to_plot = picks_ms  # type: ignore
         else:
             picks_to_plot = None  # type: ignore
 
         if picks_to_plot is not None:
             self.plot_picks(picks_to_plot, color=picks_color)
 
@@ -424,7 +463,14 @@
         headers_font_pixels=headers_font_pixels,
         time_spacing=time_spacing,
         traces_spacing=traces_spacing,
         hide_traces_axis=hide_traces_axis,
     )
     app.exec()
     warnings.resetwarnings()
+
+
+if __name__ == "__main__":
+    from first_breaks.utils.utils import download_demo_sgy
+
+    demo_sgy = download_demo_sgy()
+    export_image(demo_sgy, "demo_sgy.png")
```

### Comparing `first-breaks-picking-0.1.0/first_breaks/desktop/main_gui.py` & `first-breaks-picking-0.2.0/first_breaks/desktop/main_gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import sys
 import warnings
 from pathlib import Path
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional, Type, Union
 
 from PyQt5.QtCore import QSize, Qt, QThreadPool
 from PyQt5.QtWidgets import (
     QAction,
     QApplication,
-    QDesktopWidget,
+    QDialog,
     QFileDialog,
     QHBoxLayout,
     QLabel,
     QMainWindow,
     QProgressBar,
     QSizePolicy,
     QSlider,
     QStyle,
     QToolBar,
     QWidget,
 )
 
-from first_breaks.const import HIGH_DPI, MODEL_ONNX_HASH
+from first_breaks.const import DEMO_SGY_PATH, HIGH_DPI, MODEL_ONNX_HASH, MODEL_ONNX_PATH
 from first_breaks.desktop.graph import GraphWidget
 from first_breaks.desktop.picking_widget import PickingWindow
-from first_breaks.desktop.threads import InitNet, PickerQRunnable
-from first_breaks.desktop.warn_widget import WarnBox
-from first_breaks.picking.picker import PickerONNX
+from first_breaks.desktop.threads import CallInThread, PickerQRunnable
+from first_breaks.desktop.utils import MessageBox, set_geometry
+from first_breaks.picking.ipicker import IPicker
+from first_breaks.picking.picker_onnx import PickerONNX
 from first_breaks.picking.task import Task
 from first_breaks.sgy.reader import SGY
-from first_breaks.utils.utils import calc_hash
+from first_breaks.utils.utils import (
+    calc_hash,
+    download_demo_sgy,
+    download_model_onnx,
+    multiply_iterable_by,
+    remove_unused_kwargs,
+)
 
 warnings.filterwarnings("ignore")
 
 if HIGH_DPI:
     QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
     QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
 
@@ -69,104 +76,92 @@
     @classmethod
     def value2slider(cls, value: float) -> int:
         a = int(cls.multiplier * value)
         return a
 
 
 class MainWindow(QMainWindow):
-    def __init__(self):  # type: ignore
+    def __init__(self, use_open_gl: bool = True):  # type: ignore
         super(MainWindow, self).__init__()
 
         if getattr(sys, "frozen", False):
             self.main_folder = Path(sys._MEIPASS)  # type: ignore
         else:
             self.main_folder = Path(__file__).parent
 
-        # main window settings
-        h, w = self.screen().size().height(), self.screen().size().width()
-        left = int(0.2 * w)
-        top = int(0.2 * h)
-        width = int(0.6 * w)
-        height = int(0.6 * h)
-        self.setGeometry(left, top, width, height)
-
-        qt_rectangle = self.frameGeometry()
-        center_point = QDesktopWidget().availableGeometry().center()
-        qt_rectangle.moveCenter(center_point)
-        self.move(qt_rectangle.topLeft())
-
+        set_geometry(self, width_rel=0.6, height_rel=0.6, fix_size=False, centralize=True)
         self.setWindowTitle("First breaks picking")
 
         # toolbar
-        toolbar = QToolBar()
-        toolbar.setIconSize(QSize(30, 30))
-        self.addToolBar(toolbar)
+        self.toolbar = QToolBar()
+        self.toolbar.setIconSize(QSize(30, 30))
+        self.addToolBar(self.toolbar)
 
         # buttons on toolbar
         icon_load_nn = self.style().standardIcon(QStyle.SP_ComputerIcon)
         # icon_load_nn = QIcon(str(self.main_folder / "icons" / "nn.png"))
         self.button_load_nn = QAction(icon_load_nn, "Load model", self)
         self.button_load_nn.triggered.connect(self.load_nn)
         self.button_load_nn.setEnabled(True)
-        toolbar.addAction(self.button_load_nn)
+        self.toolbar.addAction(self.button_load_nn)
 
         icon_get_filename = self.style().standardIcon(QStyle.SP_DirIcon)
         # icon_get_filename = QIcon(str(self.main_folder / "icons" / "sgy.png"))
         self.button_get_filename = QAction(icon_get_filename, "Open SGY-file", self)
         self.button_get_filename.triggered.connect(self.get_filename)
         self.button_get_filename.setEnabled(True)
-        toolbar.addAction(self.button_get_filename)
+        self.toolbar.addAction(self.button_get_filename)
 
-        toolbar.addSeparator()
+        self.toolbar.addSeparator()
 
         icon_fb = self.style().standardIcon(QStyle.SP_FileDialogContentsView)
         # icon_fb = QIcon(str(self.main_folder / "icons" / "picking.png"))
         self.button_fb = QAction(icon_fb, "Neural network FB picking", self)
         self.button_fb.triggered.connect(self.pick_fb)
         self.button_fb.setEnabled(False)
-        toolbar.addAction(self.button_fb)
+        self.toolbar.addAction(self.button_fb)
 
         self.need_processing_region = True
         icon_processing_show = self.style().standardIcon(QStyle.SP_FileDialogListView)
         # icon_export = QIcon(str(self.main_folder / "icons" / "export.png"))
         self.button_processing_show = QAction(icon_processing_show, "Show processing grid", self)
         self.button_processing_show.triggered.connect(self.processing_region_changed)
         self.button_processing_show.setChecked(self.need_processing_region)
         self.button_processing_show.setEnabled(True)
         self.button_processing_show.setCheckable(True)
         if self.need_processing_region:
             self.button_processing_show.toggle()
-        toolbar.addAction(self.button_processing_show)
+        self.toolbar.addAction(self.button_processing_show)
 
-        toolbar.addSeparator()
+        self.toolbar.addSeparator()
 
         default_gain_value = 1.0
         self.gain_value = default_gain_value
         self.gain_label = QLabel(str(default_gain_value))
         self.slider_gain = QSlider(Qt.Horizontal)
         self.slider_gain.setRange(SliderConverter.value2slider(-5), SliderConverter.value2slider(5))
         self.slider_gain.setValue(SliderConverter.value2slider(1))
         self.slider_gain.setSingleStep(SliderConverter.value2slider(0.1))
         self.slider_gain.wheelEvent = lambda *args: args[-1].ignore()  # block scrolling with wheel
         self.slider_gain.setMaximumWidth(150)
         self.slider_gain.valueChanged.connect(self.gain_changed)
         self.slider_gain.sliderReleased.connect(self.update_plot)
-        toolbar.addWidget(self.slider_gain)
-        toolbar.addWidget(self.gain_label)
+        self.toolbar.addWidget(self.slider_gain)
+        self.toolbar.addWidget(self.gain_label)
 
         icon_export = self.style().standardIcon(QStyle.SP_DialogSaveButton)
         # icon_export = QIcon(str(self.main_folder / "icons" / "export.png"))
         self.button_export = QAction(icon_export, "Export picks to file", self)
         self.button_export.triggered.connect(self.export)
         self.button_export.setEnabled(False)
-        toolbar.addAction(self.button_export)
+        self.toolbar.addAction(self.button_export)
 
         spacer = QWidget(self)
         spacer.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
-        toolbar.addWidget(spacer)
+        self.toolbar.addWidget(spacer)
 
         self.status = self.statusBar()
         self.status_progress = QProgressBar()
         self.status_progress.hide()
 
         self.status_message = QLabel()
         self.status_message.setText("Open SGY file or load model")
@@ -176,31 +171,34 @@
         status_widget.setLayout(status_layout)
         status_layout.addWidget(self.status_progress)
         status_layout.addWidget(self.status_message)
 
         self.status.addPermanentWidget(status_widget)
 
         # graph widget
-        self.graph = GraphWidget(background="w")
+        self.graph = GraphWidget(use_open_gl=use_open_gl, background="w")
         self.graph.hide()
         self.setCentralWidget(self.graph)
 
-        # picking widget
-        self.picking = PickingWindow()
-        self.picking.hide()
-
         # placeholders
         self.sgy: Optional[SGY] = None
         self.fn_sgy: Optional[Union[str, Path]] = None
         self.ready_to_process = ReadyToProcess()
-        self.picker: Optional[PickerONNX] = None
         self.last_task: Optional[Task] = None
         self.settings: Optional[Dict[str, Any]] = None
         self.last_folder: Optional[Union[str, Path]] = None
 
+        self.picker_class: Type[IPicker] = PickerONNX
+        self.picker: Optional[IPicker] = None
+        self.picker_hash = MODEL_ONNX_HASH
+        self.picker_extra_kwargs_init = {"show_progressbar": False, "device": "cpu"}
+
+        self.picking_window_class = PickingWindow
+        self.picking_window_extra_kwargs: Dict[str, Any] = {}
+
         self.threadpool = QThreadPool()
 
         self.show()
 
     def get_last_folder(self) -> str:
         if self.last_folder is None:
             return str(Path.home())
@@ -218,48 +216,72 @@
             self.last_folder = None
 
     def gain_changed(self, gain_from_slider: int) -> None:
         self.gain_value = SliderConverter.slider2value(gain_from_slider)
         self.gain_label.setText(str(self.gain_value))
 
     def _thread_init_net(self, weights: Union[str, Path]) -> None:
-        worker = InitNet(weights)
-        worker.signals.finished.connect(self.init_net)
-        self.threadpool.start(worker)
+        task = CallInThread(self.picker_class, model_path=weights, **self.picker_extra_kwargs_init)
+        task.signals.result.connect(self.init_net)
+        self.threadpool.start(task)
 
     def init_net(self, picker: PickerONNX) -> None:
         self.picker = picker
 
     def receive_settings(self, settings: Dict[str, Any]) -> None:
+        self.picking_window_extra_kwargs = remove_unused_kwargs(settings, self.picker.change_settings)
         self.settings = settings
 
     def pick_fb(self) -> None:
-        settings = PickingWindow(self.last_task)
-        settings.export_settings_signal.connect(self.receive_settings)
-        settings.exec_()
+        if self.graph.is_picks_modified_manually:
+            overwrite_manual_changes_dialog = MessageBox(
+                self,
+                title="Overwrite manual picking",
+                message="There are manual modifications in the current picks. "
+                "They will be lost when the new picking starts. "
+                "Do you agree?",
+                add_cancel_option=True,
+            )
+            reply = overwrite_manual_changes_dialog.exec_()
+            if reply == QDialog.Accepted:
+                is_accepted_open_picking_settings = True
+            else:
+                is_accepted_open_picking_settings = False
+        else:
+            is_accepted_open_picking_settings = True
+
+        if is_accepted_open_picking_settings:
+            picking_settings = self.picking_window_class(task=self.last_task, **self.picking_window_extra_kwargs)
+            picking_settings.export_settings_signal.connect(self.receive_settings)
+            picking_settings.exec_()
+        else:
+            return
 
         if not self.settings:
             return
 
         try:
-            task = Task(self.sgy, **self.settings)
+            task_kwargs = remove_unused_kwargs(self.settings, Task)
+            task = Task(self.sgy, **task_kwargs)
+            change_settings_kwargs = remove_unused_kwargs(self.settings, self.picker_class.change_settings)
+            self.picker.change_settings(**change_settings_kwargs)
             self.process_task(task)
         except Exception as e:
-            window_err = WarnBox(self, title=e.__class__.__name__, message=str(e))
+            window_err = MessageBox(self, title=e.__class__.__name__, message=str(e))
             window_err.exec_()
 
     def process_task(self, task: Task) -> None:
         self.button_fb.setEnabled(False)
         self.button_get_filename.setEnabled(False)
         worker = PickerQRunnable(self.picker, task)
         worker.signals.started.connect(self.on_start_task)
         worker.signals.result.connect(self.on_result_task)
         worker.signals.progress.connect(self.on_progressbar_task)
         worker.signals.message.connect(self.on_message_task)
-        worker.signals.finished.connect(self.on_finish_task)
+        worker.signals.result.connect(self.on_finish_task)
         self.threadpool.start(worker)
 
     def store_task(self, task: Task) -> None:
         self.last_task = task
 
     def on_start_task(self) -> None:
         self.status_progress.show()
@@ -277,15 +299,15 @@
     def on_result_task(self, result: Task) -> None:
         self.store_task(result)
         if result.success:
             self.graph.plot_picks(self.last_task.picks_in_ms)
             self.run_processing_region()
             self.button_export.setEnabled(True)
         else:
-            window_error = WarnBox(self, title="InternalError", message=result.error_message)
+            window_error = MessageBox(self, title="InternalError", message=result.error_message)
             window_error.exec_()
 
         self.button_get_filename.setEnabled(True)
         self.button_fb.setEnabled(True)
 
     def processing_region_changed(self, toggle: bool) -> None:
         self.need_processing_region = toggle
@@ -317,56 +339,58 @@
         self.show_picks()
 
     def unlock_pickng_if_ready(self) -> None:
         if self.ready_to_process.is_ready():
             self.button_fb.setEnabled(True)
             self.status_message.setText("Click on picking to start processing")
 
-    def load_nn(self, filename: Optional[str] = None) -> None:
+    def load_nn(self, filename: Optional[Union[str, Path]] = None) -> None:
         if not filename:
             options = QFileDialog.Options()
             filename, _ = QFileDialog.getOpenFileName(
                 self, "Select file with NN weights", directory=self.get_last_folder(), options=options
             )
 
         if filename:
-            if FileState.get_file_state(filename, MODEL_ONNX_HASH) == FileState.valid_file:
+            if FileState.get_file_state(filename, self.picker_hash) == FileState.valid_file:
                 self._thread_init_net(weights=filename)
                 self.button_load_nn.setEnabled(False)
                 self.ready_to_process.model_loaded = True
 
                 status_message = "Model loaded successfully"
                 if not self.ready_to_process.sgy_selected:
                     status_message += ". Open SGY file to start picking"
                 self.status_message.setText(status_message)
 
                 self.unlock_pickng_if_ready()
                 self.set_last_folder_based_on_file(filename)
             else:
-                window_err = WarnBox(
+                window_err = MessageBox(
                     self,
                     title="Model loading error",
                     message="The file cannot be used as model weights. "
                     "Download the file according to the manual and select it.",
                 )
                 window_err.exec_()
 
-    def get_filename(self, filename: Optional[str] = None) -> None:
+    def get_filename(self, filename: Optional[Union[str, Path]] = None) -> None:
         if not filename:
-            options = QFileDialog.Options()
             filename, _ = QFileDialog.getOpenFileName(
-                self, "Open SGY-file", directory=self.get_last_folder(), filter="SGY-file (*.sgy)", options=options
+                self,
+                "Open SEGY-file",
+                directory=self.get_last_folder(),
+                filter="SEGY-file (*.segy *.sgy);; Any file (*)",
             )
         if filename:
             try:
                 self.fn_sgy = Path(filename)
                 self.last_task = None
-                self.sgy = SGY(self.fn_sgy, use_delayed_init=False)
+                self.sgy = SGY(self.fn_sgy)
 
-                self.graph.clear()
+                self.graph.full_clean()
                 self.update_plot(refresh_view=True)
                 self.graph.show()
                 self.button_export.setEnabled(False)
 
                 self.button_get_filename.setEnabled(True)
                 self.ready_to_process.sgy_selected = True
 
@@ -374,31 +398,57 @@
                     status_message = "Load model to start picking"
                     self.status_message.setText(status_message)
 
                 self.unlock_pickng_if_ready()
                 self.set_last_folder_based_on_file(filename)
 
             except Exception as e:
-                window_err = WarnBox(self, title=e.__class__.__name__, message=str(e))
+                window_err = MessageBox(self, title=e.__class__.__name__, message=str(e))
                 window_err.exec_()
 
     def export(self) -> None:
-        options = QFileDialog.Options()
-        filename, _ = QFileDialog.getSaveFileName(
-            self, "Save result", directory=self.get_last_folder(), filter="TXT (*.txt)", options=options
-        )
+        formats = ["SEGY-file (*.segy *.sgy)", "JSON-file (*.json)", "TXT-file (*.txt)"]
+        formats = ";; ".join(formats)
+        filename, _ = QFileDialog.getSaveFileName(self, "Save result", directory=self.get_last_folder(), filter=formats)
 
         if filename:
+            filename = Path(filename).resolve()
             if self.last_task is not None and self.last_task.success:
-                Path(filename).parent.mkdir(parents=True, exist_ok=True)
-                self.last_task.export_result(str(Path(filename).resolve()), as_plain=True)
-                self.set_last_folder_based_on_file(filename)
+                filename.parent.mkdir(parents=True, exist_ok=True)
+
+                picks_in_samples_prev = self.last_task.picks_in_samples
+                if self.graph.is_picks_modified_manually:
+                    self.last_task.picks_in_samples = multiply_iterable_by(
+                        self.graph.picks_in_ms, 1 / self.sgy.dt_ms, int
+                    )
+                if filename.suffix.lower() in (".sgy", ".segy"):
+                    self.last_task.export_result(str(filename), as_sgy=True)  # type: ignore
+                elif filename.suffix.lower() == ".txt":
+                    self.last_task.export_result(str(filename), as_plain=True)
+                elif filename.suffix.lower() == ".json":
+                    self.last_task.export_result(str(filename), as_json=True)
+                else:
+                    message_er = "The file can only be saved in '.sgy', '.segy', '.txt, or '.json' formats"
+                    window_err = MessageBox(self, title="Wrong filename", message=message_er)
+                    window_err.exec_()
+                if self.graph.is_picks_modified_manually:
+                    self.last_task.picks_in_samples = picks_in_samples_prev
 
 
 def run_app() -> None:
     app = QApplication([])
     _ = MainWindow()
     app.exec_()
 
 
+def fetch_data_and_run_app() -> None:
+    download_model_onnx(MODEL_ONNX_PATH)
+    download_demo_sgy(DEMO_SGY_PATH)
+    app = QApplication([])
+    window = MainWindow()
+    window.load_nn(MODEL_ONNX_PATH)
+    window.get_filename(DEMO_SGY_PATH)
+    app.exec_()
+
+
 if __name__ == "__main__":
-    run_app()
+    fetch_data_and_run_app()
```

### Comparing `first-breaks-picking-0.1.0/first_breaks/desktop/threads.py` & `first-breaks-picking-0.2.0/first_breaks/desktop/threads.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,47 @@
-from pathlib import Path
-from typing import Union
+from typing import Any
 
 from PyQt5.QtCore import QObject, QRunnable, pyqtSignal, pyqtSlot
 
-from first_breaks.picking.picker import PickerONNX
+from first_breaks.picking.ipicker import IPicker
 from first_breaks.picking.task import Task
 
 
 class PickerSignals(QObject):
     started = pyqtSignal()
     progress = pyqtSignal(int)
     finished = pyqtSignal()
     result = pyqtSignal(Task)
     message = pyqtSignal(str)
 
 
 class PickerQRunnable(QRunnable):
-    def __init__(self, picker: PickerONNX, task: Task):
+    def __init__(self, picker: IPicker, task: Task):
         super().__init__()
 
         self.signals = PickerSignals()
 
         self.picker = picker
         self.task = task
 
         self.picker.callback_step_finished = self.callback_step_finished  # type: ignore
         self.picker.callback_processing_started = self.callback_processing_started  # type: ignore
+        self.picker.callback_processing_finished = self._do_nothing  # type: ignore
 
-        self.len = task.num_gathers
+        self.len = 0
+
+    def _do_nothing(self, *args: Any, **kwargs: Any) -> None:
+        pass
 
     def callback_step_finished(self, idx_batch: int) -> None:
         progress = int(100 * (idx_batch + 1) / self.len)
         self.signals.progress.emit(progress)
 
     def callback_processing_started(self, length: int) -> None:  # type: ignore
+        self.len = length
         self.signals.progress.emit(0)
         self.signals.message.emit("Picking")
 
     @pyqtSlot()
     def run(self) -> None:
         self.signals.started.emit()
         self.signals.message.emit("Started")
@@ -51,21 +55,35 @@
             message = "Completed" if self.task.success else "Picking Error"
             self.signals.progress.emit(100)
             self.signals.finished.emit()
             self.signals.message.emit(message)
             self.signals.result.emit(self.task)
 
 
-class InitNetSignals(QObject):
-    finished = pyqtSignal(PickerONNX)
+class CallInThreadSignals(QObject):
+    started = pyqtSignal()
+    finished = pyqtSignal()
+    success = pyqtSignal(bool)
+    result = pyqtSignal(object)
 
 
-class InitNet(QRunnable):
-    def __init__(self, weights: Union[str, Path]):
+class CallInThread(QRunnable):
+    def __init__(self, callable_obj: Any, *args: Any, **kwargs: Any):
         super().__init__()
-        self.weights = weights
-        self.signals = InitNetSignals()
+        self.callable_obj = callable_obj
+        self.args = args
+        self.kwargs = kwargs
+        self.signals = CallInThreadSignals()
 
     @pyqtSlot()
     def run(self) -> None:
-        picker = PickerONNX(self.weights, show_progressbar=False)
-        self.signals.finished.emit(picker)
+        self.signals.started.emit()
+        try:
+            result = self.callable_obj(*self.args, **self.kwargs)
+            success = True
+        except Exception as e:
+            result = e
+            success = False
+
+        self.signals.finished.emit()
+        self.signals.success.emit(success)
+        self.signals.result.emit(result)
```

### Comparing `first-breaks-picking-0.1.0/first_breaks/picking/task.py` & `first-breaks-picking-0.2.0/first_breaks/picking/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
+import warnings
 from pathlib import Path
 from typing import List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from first_breaks.sgy.reader import SGY
-from first_breaks.utils.utils import chunk_iterable, sample2ms
+from first_breaks.utils.utils import chunk_iterable, multiply_iterable_by
 
 MINIMUM_TRACES_PER_GATHER = 2
 
 
 class ProcessingParametersException(Exception):
     pass
 
@@ -31,15 +32,15 @@
         self.maximum_time = maximum_time
         self.traces_to_inverse = traces_to_inverse
         self.gain = gain
         self.clip = clip
 
         self.traces_per_gather_parsed = self.validate_and_parse_traces_per_gather(traces_per_gather)
         self.maximum_time_parsed = self.validate_and_parse_maximum_time(maximum_time)
-        self.maximum_time_sample = self._convert_maximum_time_to_index()
+        self.maximum_time_sample = self.sgy.ms2index(self.maximum_time_parsed)
         self.traces_to_inverse_parsed = self.validate_and_parse_traces_to_inverse(traces_to_inverse)
         self.gain_parsed = self.validate_and_parse_gain(gain)
         self.clip_parsed = self.validate_and_parse_clip(clip)
 
         self.picks_in_samples: Optional[Union[Sequence[float], np.ndarray]] = None
         self.confidence: Optional[Union[Sequence[float], np.ndarray]] = None
         self.success: Optional[bool] = None
@@ -91,16 +92,26 @@
     def validate_and_parse_traces_per_gather(self, traces_per_gather: int) -> int:
         self.validate_traces_per_gather(traces_per_gather)
         ntr = self.sgy.shape[1]
         return min(ntr, traces_per_gather)
 
     def validate_and_parse_maximum_time(self, maximum_time: float) -> float:
         self.validate_maximum_time(maximum_time)
-        if maximum_time > 0.0:
-            maximum_time = min(maximum_time, self.sgy.shape[0] * self.sgy.dt_ms)
+        if maximum_time == 0.0:
+            maximum_time = self.sgy.max_time_ms
+        else:
+            index = self.sgy.ms2index(maximum_time)
+            if index == 0:
+                warnings.warn(
+                    "The maximum time is not zero and is less than the duration of one sample, "
+                    "so the maximum time will be equal to the length of the trace."
+                )
+                maximum_time = self.sgy.max_time_ms
+            else:
+                maximum_time = min(maximum_time, self.sgy.max_time_ms)
         return maximum_time
 
     def validate_and_parse_traces_to_inverse(self, traces_to_inverse: Sequence[int]) -> Sequence[int]:
         self.validate_traces_to_inverse(traces_to_inverse)
         # to python indices
         traces_to_inverse = [tr - 1 for tr in traces_to_inverse if tr <= self.traces_per_gather_parsed]
         traces_to_inverse = sorted(set(traces_to_inverse))
@@ -112,76 +123,93 @@
         return float(gain)
 
     @classmethod
     def validate_and_parse_clip(cls, clip: float) -> float:
         cls.validate_clip(clip)
         return float(clip)
 
-    def _convert_maximum_time_to_index(self) -> int:
-        if self.maximum_time_parsed == 0.0:
-            return self.sgy.shape[0]
-        else:
-            return int(self.maximum_time_parsed / (self.sgy.dt_ms))
-
     def get_gathers_ids(self) -> List[Tuple[int]]:
         return list(chunk_iterable(list(range(self.sgy.shape[1])), self.traces_per_gather_parsed))  # type: ignore
 
     @property
     def num_gathers(self) -> int:
         return len(self.get_gathers_ids())
 
     @property
     def picks_in_ms(self) -> Optional[List[float]]:
         if self.picks_in_samples is not None:
-            return sample2ms(self.picks_in_samples, self.sgy.dt_ms)  # type: ignore
+            return multiply_iterable_by(self.picks_in_samples, self.sgy.dt_ms)  # type: ignore
+        else:
+            return None
+
+    @property
+    def picks_in_mcs(self) -> Optional[List[int]]:
+        if self.picks_in_samples is not None:
+            return multiply_iterable_by(self.picks_in_samples, self.sgy.dt_mcs, cast_to=int)  # type: ignore
         else:
             return None
 
-    def export_result(self, filename: Union[str, Path], as_plain: bool = False) -> None:
+    def export_result(
+        self, filename: Union[str, Path], as_plain: bool = False, as_json: bool = False, as_sgy: bool = False
+    ) -> None:
         if self.picks_in_samples is None:
-            raise RuntimeError("There are no picks. Put them manually or process the task first")
+            raise ValueError("There are no picks. Put them manually or process the task first")
+
+        if sum([as_plain, as_json, as_sgy]) == 0:
+            raise ValueError("One of the options 'as_plain', 'as_json', or 'as_sgy' must be explicitly selected.")
+        elif sum([as_plain, as_json, as_sgy]) > 1:
+            raise ValueError("Only one of the options 'as_plain', 'as_json', or 'as_sgy' can be selected.")
 
         if isinstance(self.picks_in_samples, (tuple, list)):
             picks_in_samples = self.picks_in_samples
         elif isinstance(self.picks_in_samples, np.ndarray):
             picks_in_samples = self.picks_in_samples.tolist()
         else:
             raise TypeError("Only 1D sequence can be saved")
-        picks_in_ms = sample2ms(picks_in_samples, dt_ms=self.sgy.dt_ms)
-        confidence = self.confidence
 
-        is_source_file = isinstance(self.sgy.source, (str, Path))
-        if is_source_file:
-            source_filename = str(Path(self.sgy.source).name)  # type: ignore
-            source_full_name = str(Path(self.sgy.source).resolve())  # type: ignore
+        if as_sgy:
+            self.sgy.export_sgy_with_picks(filename, picks_in_samples)  # type: ignore
         else:
-            source_filename = None
-            source_full_name = None
+            picks_in_ms = multiply_iterable_by(picks_in_samples, multiplier=self.sgy.dt_ms)
+            confidence = self.confidence
 
-        meta = {
-            "is_source_file": is_source_file,
-            "is_source_ndarray": self.sgy.is_source_ndarray,
-            "filename": source_filename,
-            "full_name": source_full_name,
-            "hash": self.sgy.get_hash(),
-            "dt_ms": self.sgy.dt_ms,
-            "is_picked_with_model": bool(self.success),
-            "model_hash": self.model_hash,
-            "traces_per_gather": self.traces_per_gather_parsed,
-            "maximum_time": self.maximum_time_parsed,
-            "traces_to_inverse": self.traces_to_inverse_parsed,
-            "gain": self.gain_parsed,
-            "clip": self.clip_parsed,
-        }
-        data = {"picks_in_samples": picks_in_samples, "picks_in_ms": picks_in_ms, "confidence": confidence}
-
-        Path(filename).parent.mkdir(parents=True, exist_ok=True)
-
-        with open(filename, "w") as fout:
-            if as_plain:
-                content = [f"{k}={v}" for k, v in meta.items()]
-                data_str = pd.DataFrame(data).to_string(index=False, justify="right")
-                content.append(data_str)
-                content = "\n".join(content)
-                fout.write(content)
+            is_source_file = isinstance(self.sgy.source, (str, Path))
+            if is_source_file:
+                source_filename = str(Path(self.sgy.source).name)  # type: ignore
+                source_full_name = str(Path(self.sgy.source).resolve())  # type: ignore
             else:
-                json.dump({**meta, **data}, fout)
+                source_filename = None
+                source_full_name = None
+
+            meta = {
+                "is_source_file": is_source_file,
+                "is_source_ndarray": self.sgy.is_source_ndarray,
+                "filename": source_filename,
+                "full_name": source_full_name,
+                "hash": self.sgy.get_hash(),
+                "dt_ms": self.sgy.dt_ms,
+                "is_picked_with_model": bool(self.success),
+                "model_hash": self.model_hash,
+                "traces_per_gather": self.traces_per_gather_parsed,
+                "maximum_time": self.maximum_time_parsed,
+                "traces_to_inverse": self.traces_to_inverse_parsed,
+                "gain": self.gain_parsed,
+                "clip": self.clip_parsed,
+            }
+            data = {
+                "trace": list(range(1, len(picks_in_samples) + 1)),
+                "picks_in_samples": picks_in_samples,
+                "picks_in_ms": picks_in_ms,
+                "confidence": confidence,
+            }
+
+            Path(filename).parent.mkdir(parents=True, exist_ok=True)
+
+            with open(filename, "w") as fout:
+                if as_plain:
+                    content = [f"{k}={v}" for k, v in meta.items()]
+                    data_str = pd.DataFrame(data).to_string(index=False, justify="right")
+                    content.append(data_str)
+                    content = "\n".join(content)
+                    fout.write(content)
+                else:
+                    json.dump({**meta, **data}, fout)
```

### Comparing `first-breaks-picking-0.1.0/first_breaks/sgy/headers.py` & `first-breaks-picking-0.2.0/first_breaks/sgy/headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,16 @@
             (3504, "number_of_textual_headers", "H"),
             (3506, "unassigned2", "94s"),
         ]
         self.validate()
 
 
 class TraceHeaders(Headers):
+    fb_pick_default = "FB_PICK"
+
     def __init__(self) -> None:
         self.headers_schema = [
             (0, "TRACENO", "i"),
             (4, "trace_sequence_file", "i"),
             (8, "FFID", "i"),
             (12, "CHAN", "i"),
             (16, "SOURCE", "i"),
@@ -204,10 +206,10 @@
             (216, "source_type", "h"),
             (218, "source_energy_direction_mantissa", "i"),
             (222, "source_energy_direction_exponent", "H"),
             (224, "source_measurement_mantissa", "i"),
             (228, "source_measurement_exponent", "H"),
             (230, "source_measurement_unit", "h"),
             (232, "unassigned1", "i"),
-            (236, "FB_PICK", "i"),
+            (236, self.fb_pick_default, "I"),
         ]
         self.validate()
```

### Comparing `first-breaks-picking-0.1.0/first_breaks/sgy/reader.py` & `first-breaks-picking-0.2.0/first_breaks/sgy/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from __future__ import annotations
 
 import io
+import shutil
 import struct
 from pathlib import Path
-from typing import Any, Dict, Generator, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, Generator, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from first_breaks.sgy.headers import FileHeaders, TraceHeaders
-from first_breaks.utils.utils import calc_hash, chunk_iterable, get_io
+from first_breaks.utils.utils import (
+    calc_hash,
+    chunk_iterable,
+    get_io,
+    ms2index,
+    multiply_iterable_by,
+)
 
 SizeHW = Tuple[int, int]
 
 
 class NotImplementedReader(Exception):
     pass
 
@@ -68,21 +75,27 @@
     def num_traces(self) -> int:
         return self.ntr
 
     @property
     def shape(self) -> SizeHW:
         return self.ns, self.ntr
 
+    def ms2index(self, ms_value: float) -> int:
+        return ms2index(ms_value, self.dt_ms)
+
+    @property
+    def max_time_ms(self) -> float:
+        return self.num_samples * self.dt_ms
+
     def __init__(
         self,
         source: Union[str, Path, bytes, np.ndarray],
         dt_mcs: Optional[Union[int, float]] = None,
         general_headers_schema: FileHeaders = FileHeaders(),
         traces_headers_schema: TraceHeaders = TraceHeaders(),
-        use_delayed_init: bool = False,
     ):
         self.source = source
         self._dt_mcs_input = dt_mcs
 
         # data
         self._traces: Optional[np.ndarray] = None
         self._dt: Optional[int] = None
@@ -99,47 +112,30 @@
 
         # other
         self._descriptor: Optional[Union[io.BytesIO, io.FileIO]] = None
         self.is_source_ndarray: Optional[bool] = None
         self._endianess: Optional[str] = None
         self._bps: Optional[int] = None
         self._data_fmt: Optional[int] = None
-        self._initialized = False
         self._hash_value: Optional[str] = None
 
-        if not use_delayed_init:
-            self._delayed_init()
+        self.__init()
 
     def get_hash(self) -> Optional[str]:
         if self.is_source_ndarray:
             return None
         else:
             if self._hash_value is None:
                 self._descriptor = get_io(self.source, mode="rb")
                 self._hash_value = calc_hash(self._descriptor)
                 self._descriptor.close()
+                self._descriptor = None
             return self._hash_value
 
-    def __getattribute__(self, item: str) -> Any:
-        _initialized_name = "_initialized"
-        _delayed_init_name = "_delayed_init"
-        _initialized_value = super().__getattribute__(_initialized_name)
-
-        # We run `_delayed_init` if
-        # 1. Try to get any attr with another name
-        # 2. Not initialized yet
-        if item not in (_initialized_name, _delayed_init_name) and not _initialized_value:
-            self._delayed_init()
-        return super().__getattribute__(item)
-
-    def _delayed_init(self) -> None:
-        if self._initialized:
-            return
-        self._initialized = True
-
+    def __init(self) -> None:
         if isinstance(self.source, (str, Path, bytes)):
             if self._dt_mcs_input is not None:
                 raise SGYInitParamsError("Argument 'dt_mcs' must be empty if SGY created from external sources")
             self._init_from_external()
             self.is_source_ndarray = False
         elif isinstance(self.source, np.ndarray):
             if self._dt_mcs_input is None:
@@ -164,14 +160,15 @@
 
     def _init_from_external(self) -> None:
         self._descriptor = get_io(self.source, mode="rb")
         self._read_endianess()
         self._read_general_headers()
         self._read_traces_headers()
         self._descriptor.close()
+        self._descriptor = None
 
     def _read_endianess(self) -> None:
         num_bytes = self._descriptor.seek(0, 2)
         if num_bytes < 3600 + 240 + 1:  # at least general headers, 1 trace headers block and byte for 1 sample
             raise InvalidSGY("Invalid structure of SGY file. File is small")
 
         self._descriptor.seek(3224)
@@ -285,14 +282,15 @@
 
         self._descriptor = get_io(self.source, mode="rb")
         for idx in ids:
             pointer = 3600 + 240 + (240 + self._ns * self._bps) * idx + min_sample
             self._descriptor.seek(pointer)
             buffer.append(self._descriptor.read(length_slice * self._bps))
         self._descriptor.close()
+        self._descriptor = None
 
         buffer_tr = b"".join(buffer)
         traces = self._read_traces_from_buffer(buffer_tr, (length_slice, len(ids)))
         return traces
 
     def _read_traces_from_buffer(self, buffer: bytes, shape: SizeHW) -> np.ndarray:
         if self._data_fmt == 1:
@@ -347,7 +345,40 @@
         return reader(array, 16)
 
     def _read_traces_float(self, buffer: bytes, shape: SizeHW) -> np.ndarray:
         return np.ndarray(shape, f"{self._endianess}f4", buffer, order="F")
 
     def _read_traces_double(self, buffer: bytes, shape: SizeHW) -> np.ndarray:
         return np.ndarray(shape, f"{self._endianess}f8", buffer, order="F")
+
+    def export_sgy_with_picks(
+        self, output_fname: Union[str, Path], picks_in_samples: List[int], byte_to_write: int = 236
+    ) -> None:
+        assert not self.is_source_ndarray, "Only true SGY can be used for importing picks"
+        assert 0 <= byte_to_write <= 236, "Only 0-236 bytes can be ised for writing"
+        assert len(picks_in_samples) == self.num_traces, "Number of traces and picks differs"
+
+        Path(output_fname).parent.mkdir(exist_ok=True, parents=True)
+
+        if isinstance(self.source, (str, Path)):
+            shutil.copyfile(str(self.source), str(output_fname))
+        elif isinstance(self.source, bytes):
+            with open(output_fname, "wb+") as f_output:
+                f_output.write(self.source)
+        else:
+            raise TypeError("Invalid type of source data")
+
+        picks_in_mcs = multiply_iterable_by(picks_in_samples, self.dt_mcs, cast_to=int)
+
+        pack_type = [
+            pack_type
+            for _, header, pack_type in self._traces_headers_schema.headers_schema
+            if header == self._traces_headers_schema.fb_pick_default
+        ][0]
+
+        self._descriptor = get_io(output_fname, mode="r+b")
+        for idx, pick in enumerate(picks_in_mcs):  # type: ignore
+            pointer = 3600 + (240 + self.num_samples * self._bps) * idx + byte_to_write
+            pick_byte = struct.pack(f"{self._endianess}{pack_type}", int(pick))
+            self._descriptor.seek(pointer)
+            self._descriptor.write(pick_byte)
+        self._descriptor.close()
```

### Comparing `first-breaks-picking-0.1.0/first_breaks/utils/debug.py` & `first-breaks-picking-0.2.0/first_breaks/utils/debug.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.1.0/first_breaks/utils/utils.py` & `first-breaks-picking-0.2.0/first_breaks/utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import hashlib
+import inspect
 import io
 from itertools import islice
 from pathlib import Path
-from typing import Any, Iterable, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
+import onnxruntime as ort
 import requests
 
 from first_breaks.const import (
     DEMO_SGY_HASH,
     DEMO_SGY_PATH,
     DEMO_SGY_URL,
     MODEL_ONNX_HASH,
@@ -85,16 +87,40 @@
 
 def download_model_onnx(
     fname: Union[str, Path] = MODEL_ONNX_PATH, url: str = MODEL_ONNX_URL, md5: str = MODEL_ONNX_HASH
 ) -> Union[str, Path]:
     return download_and_validate_file(fname=fname, url=url, md5=md5)
 
 
-def sample2ms(sample: TTimeType, dt_ms: float) -> TTimeType:
-    if isinstance(sample, (int, float, (np.number, np.ndarray))):
-        return sample * dt_ms
+def multiply_iterable_by(
+    sample: TTimeType, multiplier: float, cast_to: Optional[Callable[[Any], Any]] = None
+) -> TTimeType:
+    if isinstance(sample, (int, float, str)):
+        result = sample * multiplier  # type: ignore
+        return cast_to(result) if cast_to else result
+    elif isinstance(sample, (np.number, np.ndarray)):
+        result = sample * multiplier
+        return result.astype(cast_to) if cast_to else result
     elif isinstance(sample, list):
-        return list(sample2ms(val, dt_ms) for val in sample)
+        return list(multiply_iterable_by(val, multiplier, cast_to) for val in sample)
     elif isinstance(sample, tuple):
-        return tuple(sample2ms(val, dt_ms) for val in sample)
+        return tuple(multiply_iterable_by(val, multiplier, cast_to) for val in sample)
     else:
         raise TypeError("Invalid type for samples")
+
+
+def ms2index(ms: float, sgy_ms: float) -> int:
+    return int(ms / sgy_ms)
+
+
+def remove_unused_kwargs(kwargs: Dict[str, Any], constructor: Any) -> Dict[str, Any]:
+    return {k: v for k, v in kwargs.items() if k in inspect.signature(constructor).parameters}
+
+
+ONNX_DEVICE2PROVIDER = {"cuda": "CUDAExecutionProvider", "cpu": "CPUExecutionProvider"}
+
+
+def is_onnx_cuda_available() -> bool:
+    try:
+        return ONNX_DEVICE2PROVIDER["cuda"] in ort.get_available_providers()
+    except Exception:
+        return False
```

### Comparing `first-breaks-picking-0.1.0/first_breaks/utils/visualizations.py` & `first-breaks-picking-0.2.0/first_breaks/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-0.1.0/first_breaks_picking.egg-info/PKG-INFO` & `first-breaks-picking-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: first-breaks-picking
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tool for picking first breaks in seismic gather
 Home-page: https://github.com/DaloroAT/first_breaks_picking
 Author: Aleksei Tarasov
 Author-email: aleksei.v.tarasov@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/DaloroAT/first_breaks_picking
 Keywords: seismic,first-breaks,computer-vision,deep-learning,segmentation,data-science
@@ -17,16 +17,17 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Description-Content-Type: text/markdown
+Provides-Extra: gpu
 License-File: LICENSE
 
 # First breaks picking
 This project is devoted to pick waves that are the first to be detected on a seismogram (first breaks, first arrivals).
 Traditionally, this procedure is performed manually. When processing field data, the number of picks reaches hundreds of
 thousands. Existing analytical methods allow you to automate picking only on high-quality data with a high
 signal / noise ratio.
@@ -98,58 +99,80 @@
 
 ![](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/docs/examples/noisy/noisy_6.png)
 
 </details>
 
 # Installation
 
-Library is available in PyPI:
+Library is available in [PyPI](https://pypi.org/project/first-breaks-picking/):
 ```shell
 pip install -U first-breaks-picking
 ```
 
+### GPU support
+
+You can use the capabilities of GPU to significantly reduce picking time. Before started, check
+[here](https://developer.nvidia.com/cuda-gpus) that your GPU is CUDA compatible.
+
+Install GPU supported version of library:
+```shell
+pip install -U first-breaks-picking[gpu]
+```
+
+The following steps are operating system dependent and must be performed manually:
+
+- Install [latest NVIDIA drivers](https://www.nvidia.com/Download/index.aspx).
+- Install [CUDA toolkit](https://developer.nvidia.com/cuda-downloads).
+**The version must be between 11.x, starting with 11.6. Version 12 is not supported**.
+- Install ZLib and CuDNN:
+[Windows](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html#install-windows) and
+[Linux](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html#install-linux).
+
 ### Extra data
 
 - To pick first breaks you need
 to [download model](https://oml.daloroserver.com/download/seis/fb.onnx).
 
 - If you have no seismic data, you can also
 [download small SGY file](https://raw.githubusercontent.com/DaloroAT/first_breaks_picking/main/data/real_gather.sgy).
 
 It's also possible to download them with Python using the following snippet:
 
+[code-block-start]:downloading-extra
 ```python
 from first_breaks.utils.utils import (download_demo_sgy,
                                       download_model_onnx)
 
 sgy_filename = 'data.sgy'
 model_filename = 'model.onnx'
 
 download_demo_sgy(sgy_filename)
 download_model_onnx(model_filename)
 ```
+[code-block-end]:downloading-extra
 
 # How to use it
 
 The library can be used in Python, or you can use the desktop application.
 
 ## Python
 
 Programmatic way has more flexibility for building your own picking scenario and processing multiple files.
 
 ### Minimal example
 
 The following snippet implements the picking process of the demo file. As a result, you can get an image from
 the project preview.
 
+[code-block-start]:e2e-example
 ```python
 from first_breaks.utils.utils import download_demo_sgy
 from first_breaks.sgy.reader import SGY
 from first_breaks.picking.task import Task
-from first_breaks.picking.picker import PickerONNX
+from first_breaks.picking.picker_onnx import PickerONNX
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 download_demo_sgy(fname=sgy_filename)
 sgy = SGY(sgy_filename)
 
 task = Task(sgy_filename,
@@ -170,67 +193,91 @@
              traces_window=(79.5, 90.5),
              show_processing_region=False,
              headers_total_pixels=80,
              height=500,
              width=700,
              hide_traces_axis=True)
 ```
+[code-block-end]:e2e-example
 
 For a better understanding of the steps taken, expand and read the next section.
 
 ### Detailed examples
 
 <details>
 
 <summary>Show examples</summary>
 
+### Download demo SGY
+
+Let's download the demo file. All the following examples assume that the file is downloaded and saved as `data.sgy`.
+You can also put your own SGY file.
+
+```python
+from first_breaks.utils.utils import download_demo_sgy
+
+sgy_filename = 'data.sgy'
+download_demo_sgy(fname=sgy_filename)
+```
+
 ### Create SGY
 We provide several ways to create `SGY` object: from file, `bytes` or `numpy` array.
 
 From file:
+
+[code-block-start]:init-from-path
 ```python
 from first_breaks.sgy.reader import SGY
 
-sgy_filename = ...  # put path to your file.
+sgy_filename = 'data.sgy'
 sgy = SGY(sgy_filename)
 ```
+[code-block-end]:init-from-path
 
 From `bytes`:
+
+[code-block-start]:init-from-bytes
 ```python
 from first_breaks.sgy.reader import SGY
 
-sgy_filename = ...  # put path to your file.
+sgy_filename = 'data.sgy'
 
 with open(sgy_filename, 'rb') as fin:
     sgy_bytes = fin.read()
 
 sgy = SGY(sgy_bytes)
 ```
+[code-block-end]:init-from-bytes
 
 If you want to create from `numpy` array, extra argument `dt_mcs` is required:
+
+[code-block-start]:init-from-np
 ```python
 import numpy as np
 from first_breaks.sgy.reader import SGY
 
 num_samples = 1000
 num_traces = 48
 dt_mcs = 1e3
 
 traces = np.random.random((num_samples, num_traces))
 sgy = SGY(traces, dt_mcs=dt_mcs)
 ```
+[code-block-end]:init-from-np
 
 ### Content of SGY
 
 Created `SGY` allows you to read traces, get observation parameters and view headers (empty if created from `numpy`)
 
+[code-block-start]:sgy-content
 ```python
 from first_breaks.sgy.reader import SGY
 
-sgy: SGY = ...  # put here previously created SGY
+sgy_filename = 'data.sgy'
+sgy = SGY(sgy_filename)
 
 # get all traces or specific traces limited by time
 all_traces = sgy.read()
 block_of_data = sgy.read_traces_by_ids(ids=[1, 2, 3, 10],
                                        min_sample=100,
                                        max_sample=500)
 
@@ -244,64 +291,114 @@
 print(sgy.dt, sgy.dt_mcs, sgy.dt_ms)
 
 # dict with headers in the first 3600 bytes of the file
 print(sgy.general_headers)
 # pandas DataFrame with headers for each trace
 print(sgy.traces_headers.head())
 ```
+[code-block-end]:sgy-content
 
 ### Create task for picking
 
 Next, we create a task for picking and pass the picking parameters to it. They have default values, but for the
 best quality, they must be matched to specific data. You can use the desktop application to evaluate the parameters.
 A detailed description of the parameters can be found  in the `Picking process` chapter.
 
+[code-block-start]:create-task
 ```python
 from first_breaks.sgy.reader import SGY
 from first_breaks.picking.task import Task
 
-sgy: SGY = ...  # put here previously created SGY
+sgy_filename = 'data.sgy'
+sgy = SGY(sgy_filename)
+
 task = Task(sgy,
             traces_per_gather=24,
             maximum_time=200)
 ```
+[code-block-end]:create-task
+
+
+### Create Picker
+In this step, we instantiate the neural network for picking. If you downloaded the model according to the
+installation section, then pass the path to it. Or leave the path to the model empty so that we can download it
+automatically.
+
+It's also possible to use GPU/CUDA to accelerate computation. By default `cuda` is selected if you have finished
+all steps regarding GPU in `Installation` section. Otherwise, it's `cpu`.
+
+You can also set the value of parameter `batch_size`, which can further speed up the calculations on the GPU.
+However, this will require additional video memory (VRAM).
+
+NOTE: When using the CPU, increasing `batch_size` does not speed up the calculation at all, but it may
+require additional memory costs (RAM). So don't increase this parameter when using CPU.
+
+[code-block-start]:create-picker
+```python
+from first_breaks.picking.picker_onnx import PickerONNX
+
+# the library will determine the best available device
+picker_default = PickerONNX()
+
+# create picker explicitly on CPU
+picker_cpu = PickerONNX(device='cpu')
+
+# create picker explicitly on GPU
+picker_gpu = PickerONNX(device='cuda', batch_size=2)
+
+# transfer model to another device
+picker_cpu.change_settings(device='cuda', batch_size=3)
+picker_gpu.change_settings(device='cpu', batch_size=1)
+```
+[code-block-end]:create-picker
 
 ### Pick first breaks
 
-In this step, we use the neural network for picking. If you downloaded the model according to the installation section,
-then pass the path to it. Or leave the path to the model empty so that we can download it automatically.
+Now, using all the created components, we can pick the first breaks and export the results.
 
+[code-block-start]:pick-fb
 ```python
 from first_breaks.picking.task import Task
-from first_breaks.picking.picker import PickerONNX
+from first_breaks.picking.picker_onnx import PickerONNX
+from first_breaks.sgy.reader import SGY
 
-task: Task = ...  # put here previously created task
+sgy_filename = 'data.sgy'
+sgy = SGY(sgy_filename)
+
+task = Task(sgy,
+            traces_per_gather=24,
+            maximum_time=200)
 picker = PickerONNX()
 task = picker.process_task(task)
 
 # you can see results of picking
 print(task.picks_in_samples)
 print(task.picks_in_ms)
 print(task.confidence)
 
 # you can export picks to file as plain text
 task.export_result('result.txt', as_plain=True)
 # or save as json file
-task.export_result('result.json', as_plain=False)
+task.export_result('result.json', as_json=True)
+# or make a copy of source SGY and put picks to 236 byte
+task.export_result('result.segy', as_sgy=True)
 ```
+[code-block-end]:pick-fb
 
 ### Visualizations
 
 You can save the seismogram and picks as an image. We use Qt backend for visualizations. Here we describe some usage
 scenarios.
 
 We've added named arguments to various scenarios for demonstration purposes, but in practice you can
 use them all. See the function arguments for more visualization options.
 
 Plot `SGY` only:
+
+[code-block-start]:plot-sgy
 ```python
 from first_breaks.sgy.reader import SGY
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 image_filename = 'image.png'
 
@@ -309,16 +406,19 @@
 export_image(sgy, image_filename,
              normalize=False,
              traces_window=(5, 10),
              time_window=(0, 200),
              height=300,
              width_per_trace=30)
 ```
+[code-block-end]:plot-sgy
 
 Plot `numpy` traces:
+
+[code-block-start]:plot-np
 ```python
 import numpy as np
 from first_breaks.sgy.reader import SGY
 from first_breaks.desktop.graph import export_image
 
 image_filename = 'image.png'
 num_traces = 48
@@ -331,16 +431,19 @@
              clip=0.5)
 
 # or create SGY as discussed before
 sgy = SGY(traces, dt_mcs=dt_mcs)
 export_image(sgy, image_filename,
              gain=2)
 ```
+[code-block-end]:plot-np
 
 Plot `SGY` with custom picks:
+
+[code-block-start]:plot-sgy-custom-picks
 ```python
 import numpy as np
 from first_breaks.sgy.reader import SGY
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 image_filename = 'image.png'
@@ -349,51 +452,63 @@
 picks_ms = np.random.uniform(low=0,
                              high=sgy.ns * sgy.dt_ms,
                              size=sgy.ntr)
 export_image(sgy, image_filename,
              picks_ms=picks_ms,
              picks_color=(0, 100, 100))
 ```
+[code-block-end]:plot-sgy-custom-picks
 
 Plot result of picking:
+
+[code-block-start]:plot-sgy-real-picks
 ```python
 from first_breaks.picking.task import Task
+from first_breaks.picking.picker_onnx import PickerONNX
 from first_breaks.desktop.graph import export_image
+from first_breaks.sgy.reader import SGY
 
+sgy_filename = 'data.sgy'
 image_filename = 'image.png'
 
-task: Task = ...  # put here previously created task
-# if the task was not finished, then picks will not be drawn
+sgy = SGY(sgy_filename)
+task = Task(sgy,
+            traces_per_gather=24,
+            maximum_time=200)
+picker = PickerONNX()
+task = picker.process_task(task)
 
 export_image(task, image_filename,
              show_processing_region=False,
              fill_black_left=False,
              width=1000)
 ```
+[code-block-end]:plot-sgy-real-picks
 
 ### *Limit processing region
 
 Unfortunately, processing of a part of a file is not currently supported natively. We will add this functionality soon!
 
 However, you can use the following workaround to do this:
 
+[code-block-start]:pick-limited
 ```python
 from first_breaks.sgy.reader import SGY
 
 sgy_filename = 'data.sgy'
-
 sgy = SGY(sgy_filename)
 
 interesting_traces = sgy.read_traces_by_ids(ids=list(range(20, 40)),
                                             min_sample=100,
                                             max_sample=200)
 
 # we create new SGY based on region of interests
 sgy = SGY(interesting_traces, dt_mcs=sgy.dt_mcs)
 ```
+[code-block-end]:pick-limited
 
 </details>
 
 ## Desktop application
 
 ***Application under development***
 
@@ -417,14 +532,15 @@
 Click on 2 button to select SGY. After successful reading you can analyze SGY file.
 
 The following mouse interactions are available:
 - Left button drag / Middle button drag: Pan the scene.
 - Right button drag: Scales the scene. Dragging left/right scales horizontally; dragging up/down scales vertically.
 - Right button click: Open dialog with extra options, such as limit by X/Y axes and export.
 - Wheel spin: Zooms the scene in and out.
+- Left click: *After picking with model*, you can manually change picks.
 
 You can also use slider in toolbar to change gain of traces. **The gain value for the slider is only used for
 visualization, it is not used in picking process**.
 
 ### Load model
 
 To use picker in desktop app you have to download model. See the `Installation` section for instructions
@@ -437,24 +553,36 @@
 
 Click on 3 button to open window with picking parameters. A detailed description of the parameters can be found
 in the `Picking process` chapter. Then run picking process. After some time, a line will appear connecting the first
 arrivals.
 
 Run again with different parameters to achieve optimal values of the picking parameters for your data.
 
+If you have CUDA compatible GPU and installed GPU supported version of library (see `Installation` section), you can
+select `CUDA/GPU` device  to use GPU acceleration. It can drastically decrease computation time.
+
+Parameter `Batch size` determine how many gathers will be processed simultaneously on GPU. It also can decrease
+computation time, but make sure that you have enough free GPU memory (`Batch size=10` requires > 10 Gb VRAM on Windows).
+
 ### Processing grid
 
 Click on 4 button to toggle the display of the processing grid on or off. Horizontal line
 shows `Maximum time` and vertical lines are drawn at intervals equal to `Traces per gather`. The neural network
 processes blocks independently, as separate images.
 
 ### Save results
 
-Click on 5 button to save picks, picking parameters and info about SGY file into plain `.txt` file.
+Click on 5 button to save picks into file. Depending on file extension, results will be saved as `json`,
+as plain `txt`, or as `segy` file.
+
+For extensions `txt` and `json`, picking parameters and model confidence for each peak are additionally saved.
 
+When choosing an extension `segy`, the copy of original SGY file is saved with the values of the first breaks in the
+trace headers. They are stored in the last 4 bytes (236 byte if counting from 0) to be decoded as an unsigned integer.
+Values are in microseconds.
 # Picking process
 
 Neural network process file as series of **images**. There is why **the traces should not be random**,
 since we are using information about adjacent traces.
 
 To obtain the first breaks we do the following steps:
 1) Read all traces in the file.
```

### Comparing `first-breaks-picking-0.1.0/setup.py` & `first-breaks-picking-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,26 @@
 
 def load_requirements(filename: str) -> List[str]:
     with open(filename, "r") as f:
         reqs = f.read().splitlines()
     return reqs
 
 
+basic_reqs = load_requirements("requirements/basic.txt")
+cpu_reqs = load_requirements("requirements/cpu.txt")
+gpu_extra_reqs = load_requirements("requirements/gpu.txt")
+
+
 setup(
     # technical things
-    version="0.1.0",
-    packages=find_packages(exclude=['data', 'docs', 'legacy']),
-    python_requires=">=3.7,<4.0",
-    install_requires=load_requirements("requirements.txt"),
+    version="0.2.0",
+    packages=find_packages(exclude=['data', 'docs', 'legacy', 'first_breaks._pytorch', 'tests', "requirements"]),
+    python_requires=">=3.8,<4.0",
+    install_requires=basic_reqs + cpu_reqs,
+    extras_require={'gpu': gpu_extra_reqs},
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     entry_points={
             "console_scripts": [
                 "first-breaks-picking=first_breaks.cli:cli_commands"
             ],
         },
```

