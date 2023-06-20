# Comparing `tmp/weaver-core-0.4.3.tar.gz` & `tmp/weaver-core-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaver-core-0.4.3.tar", last modified: Wed Jun 14 15:23:18 2023, max compression
+gzip compressed data, was "weaver-core-0.4.4.tar", last modified: Tue Jun 20 14:44:26 2023, max compression
```

## Comparing `weaver-core-0.4.3.tar` & `weaver-core-0.4.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.529950 weaver-core-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 15:22:35.000000 weaver-core-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-14 15:23:18.529950 weaver-core-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-06-14 15:22:35.000000 weaver-core-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 15:23:18.529950 weaver-core-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-14 15:22:35.000000 weaver-core-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/loss/focal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/nn/model/
--rw-r--r--   0 runner    (1001) docker     (123)    35306 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/model/ParticleNeXt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/model/ParticleNet.py
--rw-r--r--   0 runner    (1001) docker     (123)    30175 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/model/ParticleTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/nn/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45296 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/data/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/data/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/data/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/import_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/lr_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/utils/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver/utils/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/optimizer/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/optimizer/radam.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/optimizer/ranger.py
--rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-06-14 15:22:35.000000 weaver-core-0.4.3/weaver/utils/nn/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:23:18.525951 weaver-core-0.4.3/weaver_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 15:23:18.000000 weaver-core-0.4.3/weaver_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.742385 weaver-core-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 14:43:35.000000 weaver-core-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-20 14:44:26.742385 weaver-core-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-06-20 14:43:35.000000 weaver-core-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:44:26.742385 weaver-core-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-20 14:43:35.000000 weaver-core-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.734385 weaver-core-0.4.4/weaver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.734385 weaver-core-0.4.4/weaver/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.734385 weaver-core-0.4.4/weaver/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/loss/focal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.734385 weaver-core-0.4.4/weaver/nn/model/
+-rw-r--r--   0 runner    (1001) docker     (123)    35306 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/model/ParticleNeXt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/model/ParticleNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30175 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/model/ParticleTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/nn/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45296 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.738385 weaver-core-0.4.4/weaver/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.738385 weaver-core-0.4.4/weaver/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/data/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/data/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/data/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17989 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/import_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/lr_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.738385 weaver-core-0.4.4/weaver/utils/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.738385 weaver-core-0.4.4/weaver/utils/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/optimizer/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/optimizer/radam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/optimizer/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-06-20 14:43:35.000000 weaver-core-0.4.4/weaver/utils/nn/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:44:26.742385 weaver-core-0.4.4/weaver_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 14:44:26.000000 weaver-core-0.4.4/weaver_core.egg-info/top_level.txt
```

### Comparing `weaver-core-0.4.3/LICENSE` & `weaver-core-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/PKG-INFO` & `weaver-core-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaver-core
-Version: 0.4.3
+Version: 0.4.4
 Summary: A streamlined deep-learning framework for high energy physics
 Home-page: https://github.com/hqucms/weaver-core
 Author: H. Qu, C. Li
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `weaver-core-0.4.3/README.md` & `weaver-core-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/setup.py` & `weaver-core-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         if not line:
             continue
         if line.startswith('#'):
             continue
         install_requires.append(line)
 
 setup(name="weaver-core",
-      version='0.4.3',
+      version='0.4.4',
       description="A streamlined deep-learning framework for high energy physics",
       long_description_content_type="text/markdown",
       author="H. Qu, C. Li",
       url="https://github.com/hqucms/weaver-core",
       long_description=long_desc,
       entry_points={'console_scripts':
                     ['weaver = weaver.train:main']},
```

### Comparing `weaver-core-0.4.3/weaver/nn/loss/focal.py` & `weaver-core-0.4.4/weaver/nn/loss/focal.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/nn/model/ParticleNeXt.py` & `weaver-core-0.4.4/weaver/nn/model/ParticleNeXt.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/nn/model/ParticleNet.py` & `weaver-core-0.4.4/weaver/nn/model/ParticleNet.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/nn/model/ParticleTransformer.py` & `weaver-core-0.4.4/weaver/nn/model/ParticleTransformer.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/train.py` & `weaver-core-0.4.4/weaver/train.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/utils/data/config.py` & `weaver-core-0.4.4/weaver/utils/data/config.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/utils/data/fileio.py` & `weaver-core-0.4.4/weaver/utils/data/fileio.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/utils/data/preprocess.py` & `weaver-core-0.4.4/weaver/utils/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/utils/data/tools.py` & `weaver-core-0.4.4/weaver/utils/data/tools.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/utils/dataset.py` & `weaver-core-0.4.4/weaver/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/utils/flops_counter.py` & `weaver-core-0.4.4/weaver/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/utils/logger.py` & `weaver-core-0.4.4/weaver/utils/logger.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/utils/lr_finder.py` & `weaver-core-0.4.4/weaver/utils/lr_finder.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/utils/nn/metrics.py` & `weaver-core-0.4.4/weaver/utils/nn/metrics.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/utils/nn/optimizer/lookahead.py` & `weaver-core-0.4.4/weaver/utils/nn/optimizer/lookahead.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/utils/nn/optimizer/radam.py` & `weaver-core-0.4.4/weaver/utils/nn/optimizer/radam.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver/utils/nn/tools.py` & `weaver-core-0.4.4/weaver/utils/nn/tools.py`

 * *Files identical despite different names*

### Comparing `weaver-core-0.4.3/weaver_core.egg-info/PKG-INFO` & `weaver-core-0.4.4/weaver_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaver-core
-Version: 0.4.3
+Version: 0.4.4
 Summary: A streamlined deep-learning framework for high energy physics
 Home-page: https://github.com/hqucms/weaver-core
 Author: H. Qu, C. Li
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `weaver-core-0.4.3/weaver_core.egg-info/SOURCES.txt` & `weaver-core-0.4.4/weaver_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

