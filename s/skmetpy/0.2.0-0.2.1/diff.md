# Comparing `tmp/skmetpy-0.2.0.tar.gz` & `tmp/skmetpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.2.0.tar", last modified: Mon Jun 19 22:45:49 2023, max compression
+gzip compressed data, was "skmetpy-0.2.1.tar", last modified: Tue Jun 20 09:13:09 2023, max compression
```

## Comparing `skmetpy-0.2.0.tar` & `skmetpy-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 22:45:49.272636 skmetpy-0.2.0/
--rw-rw-rw-   0        0        0      259 2023-06-19 22:45:49.271991 skmetpy-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 22:45:49.265981 skmetpy-0.2.0/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.2.0/nunpy/__init__.py
--rw-rw-rw-   0        0        0    26428 2023-06-19 22:43:38.000000 skmetpy-0.2.0/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-19 22:45:49.272636 skmetpy-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-19 22:45:47.000000 skmetpy-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 22:45:49.270989 skmetpy-0.2.0/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-19 22:45:49.000000 skmetpy-0.2.0/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-19 22:45:49.000000 skmetpy-0.2.0/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 22:45:49.000000 skmetpy-0.2.0/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 22:45:49.000000 skmetpy-0.2.0/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 09:13:09.687473 skmetpy-0.2.1/
+-rw-rw-rw-   0        0        0      259 2023-06-20 09:13:09.687473 skmetpy-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 09:13:09.681468 skmetpy-0.2.1/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.2.1/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    26376 2023-06-20 09:09:33.000000 skmetpy-0.2.1/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 09:13:09.687473 skmetpy-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-20 09:13:07.000000 skmetpy-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:13:09.685471 skmetpy-0.2.1/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-20 09:13:09.000000 skmetpy-0.2.1/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-20 09:13:09.000000 skmetpy-0.2.1/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 09:13:09.000000 skmetpy-0.2.1/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 09:13:09.000000 skmetpy-0.2.1/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.2.0/nunpy/rechape.py` & `skmetpy-0.2.1/nunpy/rechape.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,27 +124,26 @@
       '''
 
     print(string)
 
 
 def norm1():
     string = '''
+        # Main
+        X_train, mean, std = normalize(X, X_train)
+        # Funcion
         def normalize(X, X_training):
-            # Obtenemos la media por columnas
             mean = np.mean(X, axis=0)
             std = np.std(X, axis=0)
-        
             normal = []
-        
-            # Calculamos por filas los nuevos valores de las X
             for i in range(X_training.shape[0]):
                 x = X_training[i] - mean
                 x = x / std
                 normal.append(x)
-        
+
             return normal, mean, std
       '''
 
     print(string)
 
 
 def ini1():
```

