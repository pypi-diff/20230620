# Comparing `tmp/DeepLogTimedelta-0.2.1.tar.gz` & `tmp/DeepLogTimedelta-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLogTimedelta-0.2.1.tar", last modified: Tue Jun 20 07:17:27 2023, max compression
+gzip compressed data, was "DeepLogTimedelta-0.2.2.tar", last modified: Tue Jun 20 07:47:06 2023, max compression
```

## Comparing `DeepLogTimedelta-0.2.1.tar` & `DeepLogTimedelta-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 07:17:27.672398 DeepLogTimedelta-0.2.1/
-drwxrwxrwx   0        0        0        0 2023-06-20 07:17:27.604555 DeepLogTimedelta-0.2.1/DeepLogTimedelta/
--rw-rw-rw-   0        0        0     3466 2023-06-20 07:16:43.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta/DeepLogTimedelta.py
--rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta/__init__.py
--rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta/main.py
--rw-rw-rw-   0        0        0     2311 2023-06-19 13:46:57.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta/preproccesing.py
-drwxrwxrwx   0        0        0        0 2023-06-20 07:17:27.664398 DeepLogTimedelta-0.2.1/DeepLogTimedelta.egg-info/
--rw-rw-rw-   0        0        0      207 2023-06-20 07:17:27.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-20 07:17:27.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 07:17:27.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-20 07:17:27.000000 DeepLogTimedelta-0.2.1/DeepLogTimedelta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      207 2023-06-20 07:17:27.664398 DeepLogTimedelta-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-20 07:17:27.672398 DeepLogTimedelta-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      335 2023-06-20 07:17:19.000000 DeepLogTimedelta-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:47:06.888362 DeepLogTimedelta-0.2.2/
+drwxrwxrwx   0        0        0        0 2023-06-20 07:47:06.839049 DeepLogTimedelta-0.2.2/DeepLogTimedelta/
+-rw-rw-rw-   0        0        0     3505 2023-06-20 07:46:49.000000 DeepLogTimedelta-0.2.2/DeepLogTimedelta/DeepLogTimedelta.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.2.2/DeepLogTimedelta/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.2.2/DeepLogTimedelta/main.py
+-rw-rw-rw-   0        0        0     2311 2023-06-19 13:46:57.000000 DeepLogTimedelta-0.2.2/DeepLogTimedelta/preproccesing.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:47:06.888362 DeepLogTimedelta-0.2.2/DeepLogTimedelta.egg-info/
+-rw-rw-rw-   0        0        0      207 2023-06-20 07:47:06.000000 DeepLogTimedelta-0.2.2/DeepLogTimedelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-20 07:47:06.000000 DeepLogTimedelta-0.2.2/DeepLogTimedelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:47:06.000000 DeepLogTimedelta-0.2.2/DeepLogTimedelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 07:47:06.000000 DeepLogTimedelta-0.2.2/DeepLogTimedelta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      207 2023-06-20 07:47:06.888362 DeepLogTimedelta-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:47:06.888362 DeepLogTimedelta-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      335 2023-06-20 07:47:02.000000 DeepLogTimedelta-0.2.2/setup.py
```

### Comparing `DeepLogTimedelta-0.2.1/DeepLogTimedelta/DeepLogTimedelta.py` & `DeepLogTimedelta-0.2.2/DeepLogTimedelta/DeepLogTimedelta.py`

 * *Files 9% similar despite different names*

```diff
@@ -98,11 +98,12 @@
                         ).predict(X, y, epochs, batch_size, learning_rate, criterion, optimizer, by_method='abs')
 
     def result_abs(self, y_true, y_pred):
         result = np.abs(y_true - y_pred)
         return result
 
     def result_std(self, y_true, y_pred):
-        std_2 = np.std(y_true, axis=0) * 2
+        flatten_y = y_true.flatten()
+        std_2 = torch.std(flatten_y)[0] * 2
         vfunc = np.vectorize(lambda x: 1 if x in range(x - std_2, x + std_2 + 1) else 0)
         result = vfunc(y_pred)
         return result
```

### Comparing `DeepLogTimedelta-0.2.1/DeepLogTimedelta/preproccesing.py` & `DeepLogTimedelta-0.2.2/DeepLogTimedelta/preproccesing.py`

 * *Files identical despite different names*

