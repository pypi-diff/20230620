# Comparing `tmp/optunizer-0.1.8.tar.gz` & `tmp/optunizer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optunizer-0.1.8.tar", last modified: Tue Nov  8 14:52:21 2022, max compression
+gzip compressed data, was "optunizer-0.1.9.tar", last modified: Fri Nov 11 16:08:42 2022, max compression
```

## Comparing `optunizer-0.1.8.tar` & `optunizer-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bra      (10011) Users    (10000)        0 2022-11-08 14:49:12.427505 optunizer-0.1.8/
--rw-r--r--   0 bra      (10011) Users    (10000)     1073 2022-10-02 15:55:29.000000 optunizer-0.1.8/LICENSE
--rw-r--r--   0 bra      (10011) Users    (10000)     3054 2022-11-08 14:49:12.431505 optunizer-0.1.8/PKG-INFO
--rw-r--r--   0 bra      (10011) Users    (10000)     2520 2022-10-11 21:39:26.000000 optunizer-0.1.8/README.md
--rw-r--r--   0 bra      (10011) Users    (10000)       84 2022-10-02 16:13:29.000000 optunizer-0.1.8/pyproject.toml
--rw-r--r--   0 bra      (10011) Users    (10000)      690 2022-11-08 14:49:12.463505 optunizer-0.1.8/setup.cfg
-drwxr-xr-x   0 bra      (10011) Users    (10000)        0 2022-11-08 14:49:11.535512 optunizer-0.1.8/src/
-drwxr-xr-x   0 bra      (10011) Users    (10000)        0 2022-11-08 14:49:12.063508 optunizer-0.1.8/src/optunizer/
--rw-r--r--   0 bra      (10011) Users    (10000)        0 2022-10-02 15:56:49.000000 optunizer-0.1.8/src/optunizer/__init__.py
--rw-r--r--   0 bra      (10011) Users    (10000)      522 2022-10-11 21:39:31.000000 optunizer-0.1.8/src/optunizer/__main__.py
--rw-r--r--   0 bra      (10011) Users    (10000)      492 2022-10-02 16:10:37.000000 optunizer-0.1.8/src/optunizer/factory.py
--rw-r--r--   0 bra      (10011) Users    (10000)    14565 2022-11-08 14:48:30.000000 optunizer-0.1.8/src/optunizer/optimizer.py
-drwxr-xr-x   0 bra      (10011) Users    (10000)        0 2022-11-08 14:49:12.399505 optunizer-0.1.8/src/optunizer.egg-info/
--rw-r--r--   0 bra      (10011) Users    (10000)     3054 2022-11-08 14:49:11.000000 optunizer-0.1.8/src/optunizer.egg-info/PKG-INFO
--rw-r--r--   0 bra      (10011) Users    (10000)      348 2022-11-08 14:49:11.000000 optunizer-0.1.8/src/optunizer.egg-info/SOURCES.txt
--rw-r--r--   0 bra      (10011) Users    (10000)        1 2022-11-08 14:49:11.000000 optunizer-0.1.8/src/optunizer.egg-info/dependency_links.txt
--rw-r--r--   0 bra      (10011) Users    (10000)       28 2022-11-08 14:49:11.000000 optunizer-0.1.8/src/optunizer.egg-info/requires.txt
--rw-r--r--   0 bra      (10011) Users    (10000)       10 2022-11-08 14:49:11.000000 optunizer-0.1.8/src/optunizer.egg-info/top_level.txt
+drwxr-xr-x   0 bra      (10011) Users    (10000)        0 2022-11-11 16:05:28.593830 optunizer-0.1.9/
+-rw-r--r--   0 bra      (10011) Users    (10000)     1073 2022-10-02 15:55:29.000000 optunizer-0.1.9/LICENSE
+-rw-r--r--   0 bra      (10011) Users    (10000)     3054 2022-11-11 16:05:28.593830 optunizer-0.1.9/PKG-INFO
+-rw-r--r--   0 bra      (10011) Users    (10000)     2520 2022-10-11 21:39:26.000000 optunizer-0.1.9/README.md
+-rw-r--r--   0 bra      (10011) Users    (10000)       84 2022-10-02 16:13:29.000000 optunizer-0.1.9/pyproject.toml
+-rw-r--r--   0 bra      (10011) Users    (10000)      690 2022-11-11 16:05:28.621829 optunizer-0.1.9/setup.cfg
+drwxr-xr-x   0 bra      (10011) Users    (10000)        0 2022-11-11 16:05:28.285832 optunizer-0.1.9/src/
+drwxr-xr-x   0 bra      (10011) Users    (10000)        0 2022-11-11 16:05:28.373831 optunizer-0.1.9/src/optunizer/
+-rw-r--r--   0 bra      (10011) Users    (10000)        0 2022-10-02 15:56:49.000000 optunizer-0.1.9/src/optunizer/__init__.py
+-rw-r--r--   0 bra      (10011) Users    (10000)      522 2022-10-11 21:39:31.000000 optunizer-0.1.9/src/optunizer/__main__.py
+-rw-r--r--   0 bra      (10011) Users    (10000)      492 2022-10-02 16:10:37.000000 optunizer-0.1.9/src/optunizer/factory.py
+-rw-r--r--   0 bra      (10011) Users    (10000)    14596 2022-11-11 16:04:34.000000 optunizer-0.1.9/src/optunizer/optimizer.py
+drwxr-xr-x   0 bra      (10011) Users    (10000)        0 2022-11-11 16:05:28.585830 optunizer-0.1.9/src/optunizer.egg-info/
+-rw-r--r--   0 bra      (10011) Users    (10000)     3054 2022-11-11 16:05:28.000000 optunizer-0.1.9/src/optunizer.egg-info/PKG-INFO
+-rw-r--r--   0 bra      (10011) Users    (10000)      348 2022-11-11 16:05:28.000000 optunizer-0.1.9/src/optunizer.egg-info/SOURCES.txt
+-rw-r--r--   0 bra      (10011) Users    (10000)        1 2022-11-11 16:05:28.000000 optunizer-0.1.9/src/optunizer.egg-info/dependency_links.txt
+-rw-r--r--   0 bra      (10011) Users    (10000)       28 2022-11-11 16:05:28.000000 optunizer-0.1.9/src/optunizer.egg-info/requires.txt
+-rw-r--r--   0 bra      (10011) Users    (10000)       10 2022-11-11 16:05:28.000000 optunizer-0.1.9/src/optunizer.egg-info/top_level.txt
```

### Comparing `optunizer-0.1.8/LICENSE` & `optunizer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `optunizer-0.1.8/PKG-INFO` & `optunizer-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optunizer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Optuna extension for JSON and YAML configuration files
 Home-page: https://github.com/romanzes637/optunizer
 Author: Roman Pashkovsky
 Author-email: romapasky@gmail.com
 Project-URL: Bug Tracker, https://github.com/romanzes637/optunizer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `optunizer-0.1.8/README.md` & `optunizer-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `optunizer-0.1.8/setup.cfg` & `optunizer-0.1.9/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = optunizer
-version = 0.1.8
+version = 0.1.9
 author = Roman Pashkovsky
 author_email = romapasky@gmail.com
 description = Optuna extension for JSON and YAML configuration files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/romanzes637/optunizer
 project_urls =
```

### Comparing `optunizer-0.1.8/src/optunizer/__main__.py` & `optunizer-0.1.9/src/optunizer/__main__.py`

 * *Files identical despite different names*

### Comparing `optunizer-0.1.8/src/optunizer/optimizer.py` & `optunizer-0.1.9/src/optunizer/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,16 @@
       d = {'platform': platform.system(),
            'release': platform.release(),
            'version': platform.version(),
            'architecture': platform.machine(),
            'processor': platform.processor(),
            'hostname': socket.gethostname(),
            'fqdn': socket.getfqdn(),
-           'ip': Optimizer.Logger.get_ip()}
+           'ip': Optimizer.Logger.get_ip(),
+           'cwd': os.getcwd()}
       return d
     
     @staticmethod
     def get_best_trial(study):
       d = {}
       if study._is_multi_objective():
         t = study.best_trials[0]
```

### Comparing `optunizer-0.1.8/src/optunizer.egg-info/PKG-INFO` & `optunizer-0.1.9/src/optunizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optunizer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Optuna extension for JSON and YAML configuration files
 Home-page: https://github.com/romanzes637/optunizer
 Author: Roman Pashkovsky
 Author-email: romapasky@gmail.com
 Project-URL: Bug Tracker, https://github.com/romanzes637/optunizer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

