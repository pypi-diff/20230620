# Comparing `tmp/s2and-0.15.tar.gz` & `tmp/s2and-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2and-0.15.tar", last modified: Tue Jun 20 19:59:31 2023, max compression
+gzip compressed data, was "s2and-0.16.tar", last modified: Tue Jun 20 21:54:47 2023, max compression
```

## Comparing `s2and-0.15.tar` & `s2and-0.16.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 19:59:31.474113 s2and-0.15/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13134 2023-06-05 12:41:33.000000 s2and-0.15/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-20 19:59:31.473942 s2and-0.15/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9477 2023-06-14 16:26:22.000000 s2and-0.15/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 19:59:31.471235 s2and-0.15/s2and/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      272 2023-06-05 12:41:33.000000 s2and-0.15/s2and/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1762 2023-06-05 12:41:33.000000 s2and-0.15/s2and/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    63074 2023-06-18 17:05:48.000000 s2and-0.15/s2and/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    42585 2023-06-18 18:44:33.000000 s2and-0.15/s2and/eval.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    29361 2023-06-13 11:14:21.000000 s2and-0.15/s2and/featurizer.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4866 2023-06-05 12:41:33.000000 s2and-0.15/s2and/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      942 2023-06-20 19:15:14.000000 s2and-0.15/s2and/inference.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    48434 2023-06-18 16:18:01.000000 s2and-0.15/s2and/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8210 2023-06-05 12:41:33.000000 s2and-0.15/s2and/plotting_utils.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9806 2023-06-05 12:41:33.000000 s2and-0.15/s2and/s2_funcs.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3969 2023-06-05 12:41:33.000000 s2and-0.15/s2and/sampling.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    16550 2023-06-05 12:41:33.000000 s2and-0.15/s2and/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 19:59:31.471815 s2and-0.15/s2and.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-20 19:59:31.000000 s2and-0.15/s2and.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      578 2023-06-20 19:59:31.000000 s2and-0.15/s2and.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-06-20 19:59:31.000000 s2and-0.15/s2and.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       12 2023-06-20 19:59:31.000000 s2and-0.15/s2and.egg-info/top_level.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-06-20 19:59:31.474159 s2and-0.15/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      445 2023-06-20 19:59:20.000000 s2and-0.15/setup.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 19:59:31.473684 s2and-0.15/tests/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 12:41:33.000000 s2and-0.15/tests/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3035 2023-06-05 12:41:33.000000 s2and-0.15/tests/test_cluster.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2437 2023-06-05 12:41:33.000000 s2and-0.15/tests/test_cluster_incremental.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3368 2023-06-05 12:41:33.000000 s2and-0.15/tests/test_cluster_incremental_incompatible.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7541 2023-06-05 12:41:33.000000 s2and-0.15/tests/test_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-06-05 12:41:33.000000 s2and-0.15/tests/test_eval.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4757 2023-06-05 12:41:33.000000 s2and-0.15/tests/test_featurizer.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2981 2023-06-05 12:41:33.000000 s2and-0.15/tests/test_s2_funcs.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4725 2023-06-05 12:41:33.000000 s2and-0.15/tests/test_text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 21:54:47.171021 s2and-0.16/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13134 2023-06-05 12:41:33.000000 s2and-0.16/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-20 21:54:47.170869 s2and-0.16/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9477 2023-06-14 16:26:22.000000 s2and-0.16/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 21:54:47.168238 s2and-0.16/s2and/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      272 2023-06-05 12:41:33.000000 s2and-0.16/s2and/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1762 2023-06-05 12:41:33.000000 s2and-0.16/s2and/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    63074 2023-06-18 17:05:48.000000 s2and-0.16/s2and/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    42587 2023-06-20 21:51:56.000000 s2and-0.16/s2and/eval.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    29361 2023-06-13 11:14:21.000000 s2and-0.16/s2and/featurizer.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4866 2023-06-05 12:41:33.000000 s2and-0.16/s2and/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      942 2023-06-20 19:15:14.000000 s2and-0.16/s2and/inference.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    48439 2023-06-20 21:51:36.000000 s2and-0.16/s2and/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8210 2023-06-05 12:41:33.000000 s2and-0.16/s2and/plotting_utils.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9806 2023-06-05 12:41:33.000000 s2and-0.16/s2and/s2_funcs.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3969 2023-06-05 12:41:33.000000 s2and-0.16/s2and/sampling.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    16550 2023-06-05 12:41:33.000000 s2and-0.16/s2and/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 21:54:47.169012 s2and-0.16/s2and.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      114 2023-06-20 21:54:47.000000 s2and-0.16/s2and.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      578 2023-06-20 21:54:47.000000 s2and-0.16/s2and.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-06-20 21:54:47.000000 s2and-0.16/s2and.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       12 2023-06-20 21:54:47.000000 s2and-0.16/s2and.egg-info/top_level.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-06-20 21:54:47.171065 s2and-0.16/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      445 2023-06-20 21:53:18.000000 s2and-0.16/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-06-20 21:54:47.170655 s2and-0.16/tests/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-06-05 12:41:33.000000 s2and-0.16/tests/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3035 2023-06-05 12:41:33.000000 s2and-0.16/tests/test_cluster.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2437 2023-06-05 12:41:33.000000 s2and-0.16/tests/test_cluster_incremental.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3368 2023-06-05 12:41:33.000000 s2and-0.16/tests/test_cluster_incremental_incompatible.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7541 2023-06-05 12:41:33.000000 s2and-0.16/tests/test_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-06-05 12:41:33.000000 s2and-0.16/tests/test_eval.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4757 2023-06-05 12:41:33.000000 s2and-0.16/tests/test_featurizer.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2981 2023-06-05 12:41:33.000000 s2and-0.16/tests/test_s2_funcs.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4725 2023-06-05 12:41:33.000000 s2and-0.16/tests/test_text.py
```

### Comparing `s2and-0.15/LICENSE` & `s2and-0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `s2and-0.15/README.md` & `s2and-0.16/README.md`

 * *Files identical despite different names*

### Comparing `s2and-0.15/s2and/consts.py` & `s2and-0.16/s2and/consts.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/s2and/data.py` & `s2and-0.16/s2and/data.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/s2and/eval.py` & `s2and-0.16/s2and/eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,16 +492,16 @@
 
     if nameless_classifier is not None:
         y_prob = (classifier.predict_proba(X)[:, 1] + nameless_classifier.predict_proba(nameless_X)[:, 1]) / 2
     else:
         y_prob = classifier.predict_proba(X)[:, 1]
 
     # plot AUROC
-    np.savetxt('y.txt', y, fmt='%.2f', delimiter=',')
-    np.savetxt('y_p.txt', y_prob, fmt='%.2f', delimiter=',')
+    #np.savetxt('y.txt', y, fmt='%.2f', delimiter=',')
+    #np.savetxt('y_p.txt', y_prob, fmt='%.2f', delimiter=',')
     # Calculate the mode of the array without nan values
     mode = stats.mode(y[~np.isnan(y)])[0][0]
 
     # Replace nan values with the mode
     y[np.isnan(y)] = mode
     fpr, tpr, _ = roc_curve(y, y_prob)
     roc_auc = auc(fpr, tpr)
```

### Comparing `s2and-0.15/s2and/featurizer.py` & `s2and-0.16/s2and/featurizer.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/s2and/file_cache.py` & `s2and-0.16/s2and/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/s2and/inference.py` & `s2and-0.16/s2and/inference.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/s2and/model.py` & `s2and-0.16/s2and/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -865,21 +865,21 @@
 
                 # Calculate the mode of the array without nan values
                 mode = stats.mode(y_train[~np.isnan(y_train)])[0][0]
 
                 # Replace nan values with the mode
                 y_train[np.isnan(y_train)] = mode
 
-                np.savetxt('x_train.txt', X_train, fmt='%.2f', delimiter=',')
-                np.savetxt('y_train.txt', y_train, fmt='%.2f', delimiter=',')
+                #np.savetxt('x_train.txt', X_train, fmt='%.2f', delimiter=',')
+                #np.savetxt('y_train.txt', y_train, fmt='%.2f', delimiter=',')
                 self.estimator.fit(X_train, y_train)
                 y_pred_proba = self.estimator.predict_proba(X_val)[:, 1]
-                np.savetxt('x_val.txt', X_val, fmt='%.2f', delimiter=',')
-                np.savetxt('y_prob.txt', y_pred_proba, fmt='%.2f', delimiter=',')
-                np.savetxt('y_val.txt', y_val, fmt='%.2f', delimiter=',')
+                #np.savetxt('x_val.txt', X_val, fmt='%.2f', delimiter=',')
+                #np.savetxt('y_prob.txt', y_pred_proba, fmt='%.2f', delimiter=',')
+                #np.savetxt('y_val.txt', y_val, fmt='%.2f', delimiter=',')
                 # Calculate the mode of the array without nan values
                 mode = stats.mode(y_val[~np.isnan(y_val)])[0][0]
 
                 # Replace nan values with the mode
                 y_val[np.isnan(y_val)] = mode
                 return -roc_auc_score(y_val, y_pred_proba)
```

### Comparing `s2and-0.15/s2and/plotting_utils.py` & `s2and-0.16/s2and/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/s2and/s2_funcs.py` & `s2and-0.16/s2and/s2_funcs.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/s2and/sampling.py` & `s2and-0.16/s2and/sampling.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/s2and/text.py` & `s2and-0.16/s2and/text.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/s2and.egg-info/SOURCES.txt` & `s2and-0.16/s2and.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2and-0.15/tests/test_cluster.py` & `s2and-0.16/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/tests/test_cluster_incremental.py` & `s2and-0.16/tests/test_cluster_incremental.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/tests/test_cluster_incremental_incompatible.py` & `s2and-0.16/tests/test_cluster_incremental_incompatible.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/tests/test_data.py` & `s2and-0.16/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/tests/test_eval.py` & `s2and-0.16/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/tests/test_featurizer.py` & `s2and-0.16/tests/test_featurizer.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/tests/test_s2_funcs.py` & `s2and-0.16/tests/test_s2_funcs.py`

 * *Files identical despite different names*

### Comparing `s2and-0.15/tests/test_text.py` & `s2and-0.16/tests/test_text.py`

 * *Files identical despite different names*

