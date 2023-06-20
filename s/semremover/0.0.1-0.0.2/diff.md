# Comparing `tmp/semremover-0.0.1.tar.gz` & `tmp/semremover-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semremover-0.0.1.tar", last modified: Tue Jun 20 12:51:41 2023, max compression
+gzip compressed data, was "semremover-0.0.2.tar", last modified: Tue Jun 20 13:11:27 2023, max compression
```

## Comparing `semremover-0.0.1.tar` & `semremover-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:41.560748 semremover-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 12:51:33.000000 semremover-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-20 12:51:41.560748 semremover-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-20 12:51:33.000000 semremover-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-20 12:51:33.000000 semremover-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:41.560748 semremover-0.0.1/semremover/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 12:51:33.000000 semremover-0.0.1/semremover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-20 12:51:33.000000 semremover-0.0.1/semremover/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:41.560748 semremover-0.0.1/semremover/models/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 12:51:33.000000 semremover-0.0.1/semremover/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-20 12:51:33.000000 semremover-0.0.1/semremover/models/lama.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-20 12:51:33.000000 semremover-0.0.1/semremover/models/maskformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-20 12:51:33.000000 semremover-0.0.1/semremover/models/semremover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:41.560748 semremover-0.0.1/semremover.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-20 12:51:41.000000 semremover-0.0.1/semremover.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-20 12:51:41.000000 semremover-0.0.1/semremover.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:51:41.000000 semremover-0.0.1/semremover.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 12:51:41.000000 semremover-0.0.1/semremover.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 12:51:41.560748 semremover-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-20 12:51:38.000000 semremover-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:11:27.265416 semremover-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 13:11:22.000000 semremover-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-20 13:11:27.265416 semremover-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-20 13:11:22.000000 semremover-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-20 13:11:25.000000 semremover-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:11:27.265416 semremover-0.0.2/semremover/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 13:11:22.000000 semremover-0.0.2/semremover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-20 13:11:22.000000 semremover-0.0.2/semremover/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:11:27.265416 semremover-0.0.2/semremover/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 13:11:22.000000 semremover-0.0.2/semremover/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-20 13:11:22.000000 semremover-0.0.2/semremover/models/lama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-20 13:11:22.000000 semremover-0.0.2/semremover/models/maskformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-20 13:11:22.000000 semremover-0.0.2/semremover/models/semremover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:11:27.265416 semremover-0.0.2/semremover.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-20 13:11:27.000000 semremover-0.0.2/semremover.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-20 13:11:27.000000 semremover-0.0.2/semremover.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:11:27.000000 semremover-0.0.2/semremover.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 13:11:27.000000 semremover-0.0.2/semremover.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:11:27.265416 semremover-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 13:11:22.000000 semremover-0.0.2/setup.py
```

### Comparing `semremover-0.0.1/LICENSE` & `semremover-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `semremover-0.0.1/PKG-INFO` & `semremover-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semremover
-Version: 0.0.1
+Version: 0.0.2
 Summary: semantic object removal made easy.
 Author-email: Jesse Visser <jssvssr2000@gmail.com>
 Project-URL: Homepage, https://github.com/Jessseee/semantic-object-removal
 Project-URL: Bug Tracker, https://github.com/Jessseee/semantic-object-removal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,17 +23,15 @@
 ```
 Be sure to download the model weights for [LaMa](https://github.com/advimman/lama) (e.g., [big-lama](https://disk.yandex.ru/d/ouP6l8VJ0HpMZg)). Download the directory and put it in `./semremover/models/weights`.
 
 ## Usage
 To use the script you can call it with various options. The first positional argument is the input path, which can point to either an image or a directory of images. To remove objects from a picture add them to the labels option when running the script. The default labels can be found in `./semremover/models/config/ade20k_labels.json`.
 
 ## Example
-**input**
+### input
 ```
     python -m semremover example/paris.jpg --labels car minibike van
 ```
+![A picture of a street lined with cars in Paris.](https://github.com/Jessseee/semantic-object-removal/blob/main/example/paris.jpg?raw=true)
 
-![A picture of a street lined with cars in Paris.](example/paris.jpg)
-
-**output**
-
-![A picture of the same street in paris with the cars digitally removed.](example/paris-inpainted.jpg)
+### Output
+![A picture of the same street in paris with the cars digitally removed.](https://github.com/Jessseee/semantic-object-removal/blob/main/example/paris-inpainted.jpg?raw=true)
```

### Comparing `semremover-0.0.1/README.md` & `semremover-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 ```
 Be sure to download the model weights for [LaMa](https://github.com/advimman/lama) (e.g., [big-lama](https://disk.yandex.ru/d/ouP6l8VJ0HpMZg)). Download the directory and put it in `./semremover/models/weights`.
 
 ## Usage
 To use the script you can call it with various options. The first positional argument is the input path, which can point to either an image or a directory of images. To remove objects from a picture add them to the labels option when running the script. The default labels can be found in `./semremover/models/config/ade20k_labels.json`.
 
 ## Example
-**input**
+### input
 ```
     python -m semremover example/paris.jpg --labels car minibike van
 ```
+![A picture of a street lined with cars in Paris.](https://github.com/Jessseee/semantic-object-removal/blob/main/example/paris.jpg?raw=true)
 
-![A picture of a street lined with cars in Paris.](example/paris.jpg)
-
-**output**
-
-![A picture of the same street in paris with the cars digitally removed.](example/paris-inpainted.jpg)
+### Output
+![A picture of the same street in paris with the cars digitally removed.](https://github.com/Jessseee/semantic-object-removal/blob/main/example/paris-inpainted.jpg?raw=true)
```

### Comparing `semremover-0.0.1/pyproject.toml` & `semremover-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "semremover"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jesse Visser", email="jssvssr2000@gmail.com" },
 ]
 description = "semantic object removal made easy."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `semremover-0.0.1/semremover/__main__.py` & `semremover-0.0.2/semremover/__main__.py`

 * *Files identical despite different names*

### Comparing `semremover-0.0.1/semremover/models/lama.py` & `semremover-0.0.2/semremover/models/lama.py`

 * *Files identical despite different names*

### Comparing `semremover-0.0.1/semremover/models/maskformer.py` & `semremover-0.0.2/semremover/models/maskformer.py`

 * *Files identical despite different names*

### Comparing `semremover-0.0.1/semremover/models/semremover.py` & `semremover-0.0.2/semremover/models/semremover.py`

 * *Files identical despite different names*

### Comparing `semremover-0.0.1/semremover.egg-info/PKG-INFO` & `semremover-0.0.2/semremover.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semremover
-Version: 0.0.1
+Version: 0.0.2
 Summary: semantic object removal made easy.
 Author-email: Jesse Visser <jssvssr2000@gmail.com>
 Project-URL: Homepage, https://github.com/Jessseee/semantic-object-removal
 Project-URL: Bug Tracker, https://github.com/Jessseee/semantic-object-removal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,17 +23,15 @@
 ```
 Be sure to download the model weights for [LaMa](https://github.com/advimman/lama) (e.g., [big-lama](https://disk.yandex.ru/d/ouP6l8VJ0HpMZg)). Download the directory and put it in `./semremover/models/weights`.
 
 ## Usage
 To use the script you can call it with various options. The first positional argument is the input path, which can point to either an image or a directory of images. To remove objects from a picture add them to the labels option when running the script. The default labels can be found in `./semremover/models/config/ade20k_labels.json`.
 
 ## Example
-**input**
+### input
 ```
     python -m semremover example/paris.jpg --labels car minibike van
 ```
+![A picture of a street lined with cars in Paris.](https://github.com/Jessseee/semantic-object-removal/blob/main/example/paris.jpg?raw=true)
 
-![A picture of a street lined with cars in Paris.](example/paris.jpg)
-
-**output**
-
-![A picture of the same street in paris with the cars digitally removed.](example/paris-inpainted.jpg)
+### Output
+![A picture of the same street in paris with the cars digitally removed.](https://github.com/Jessseee/semantic-object-removal/blob/main/example/paris-inpainted.jpg?raw=true)
```

