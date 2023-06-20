# Comparing `tmp/AlgoMaster-0.0.8.tar.gz` & `tmp/AlgoMaster-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgoMaster-0.0.8.tar", last modified: Mon Jun 19 17:09:34 2023, max compression
+gzip compressed data, was "AlgoMaster-0.0.9.tar", last modified: Mon Jun 19 17:17:35 2023, max compression
```

## Comparing `AlgoMaster-0.0.8.tar` & `AlgoMaster-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 17:09:34.745559 AlgoMaster-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-06-19 17:09:34.486052 AlgoMaster-0.0.8/AlgoMaster/
--rw-rw-rw-   0        0        0       39 2023-06-19 16:54:03.000000 AlgoMaster-0.0.8/AlgoMaster/__init__.py
--rw-rw-rw-   0        0        0     8848 2023-06-19 17:08:09.000000 AlgoMaster-0.0.8/AlgoMaster/classifier.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:09:34.740562 AlgoMaster-0.0.8/AlgoMaster.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-19 17:09:34.000000 AlgoMaster-0.0.8/AlgoMaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-19 17:09:34.000000 AlgoMaster-0.0.8/AlgoMaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 17:09:34.000000 AlgoMaster-0.0.8/AlgoMaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-19 17:09:34.000000 AlgoMaster-0.0.8/AlgoMaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 17:09:34.000000 AlgoMaster-0.0.8/AlgoMaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      534 2023-06-19 17:09:34.744564 AlgoMaster-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-17 16:12:45.000000 AlgoMaster-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 17:09:34.745559 AlgoMaster-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1329 2023-06-19 17:08:57.000000 AlgoMaster-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:17:35.430731 AlgoMaster-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-06-19 17:17:35.255718 AlgoMaster-0.0.9/AlgoMaster/
+-rw-rw-rw-   0        0        0       39 2023-06-19 16:54:03.000000 AlgoMaster-0.0.9/AlgoMaster/__init__.py
+-rw-rw-rw-   0        0        0     8866 2023-06-19 17:17:22.000000 AlgoMaster-0.0.9/AlgoMaster/classifier.py
+drwxrwxrwx   0        0        0        0 2023-06-19 17:17:35.306723 AlgoMaster-0.0.9/AlgoMaster.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-19 17:17:35.000000 AlgoMaster-0.0.9/AlgoMaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-19 17:17:35.000000 AlgoMaster-0.0.9/AlgoMaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 17:17:35.000000 AlgoMaster-0.0.9/AlgoMaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-19 17:17:35.000000 AlgoMaster-0.0.9/AlgoMaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 17:17:35.000000 AlgoMaster-0.0.9/AlgoMaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      534 2023-06-19 17:17:35.313722 AlgoMaster-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-17 16:12:45.000000 AlgoMaster-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 17:17:35.431739 AlgoMaster-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1329 2023-06-19 17:17:30.000000 AlgoMaster-0.0.9/setup.py
```

### Comparing `AlgoMaster-0.0.8/AlgoMaster/classifier.py` & `AlgoMaster-0.0.9/AlgoMaster/classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,17 @@
         return {'model name': model_name, 'accuracy': acc, 'confusion': confusion, 'roc': roc, 'f1': f1, 'recall': recall, 'precision': precision}
 
     def model_training(self):
         model_results = []
         for model, model_name in zip(self.model, self.model_name):
             model.fit(self.X_train, self.Y_train)
             y_pred = model.predict(self.X_test)
-            model_result = self.model_accuracy(self.Y_test, y_pred, model_name)
+            model_result = pd.DataFrame([self.model_accuracy(self.Y_test, y_pred, model_name)])
             model_results.append(model_result)
+
         self.model_table = pd.concat(model_results, ignore_index=True)
         self.model_table = self.model_table.sort_values('accuracy', ascending=False)
         self.model_table.reset_index(drop=True, inplace=True)
         return self.model_table
     
     def ensemble_prediction(self, count):
         top_models = nlargest(count, self.model_table.iterrows(), key=lambda x: x[1]['accuracy'])
```

### Comparing `AlgoMaster-0.0.8/AlgoMaster.egg-info/PKG-INFO` & `AlgoMaster-0.0.9/AlgoMaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgoMaster
-Version: 0.0.8
+Version: 0.0.9
 Summary: Learning models make simple
 Author: sajo sam
 Author-email: <sajosamambalakara@gmail.com>
 Keywords: python,classification,regression,machine learning models,hyper parameter turning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AlgoMaster-0.0.8/PKG-INFO` & `AlgoMaster-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgoMaster
-Version: 0.0.8
+Version: 0.0.9
 Summary: Learning models make simple
 Author: sajo sam
 Author-email: <sajosamambalakara@gmail.com>
 Keywords: python,classification,regression,machine learning models,hyper parameter turning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AlgoMaster-0.0.8/setup.py` & `AlgoMaster-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Learning models make simple'
 # LONG_DESCRIPTION = '''
 #                                         Learning models
 #                                     (single-file, easy-to-use)'''
 
 # Setting up
 setup(
```

