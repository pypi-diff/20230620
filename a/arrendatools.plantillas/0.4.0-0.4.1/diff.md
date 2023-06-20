# Comparing `tmp/arrendatools.plantillas-0.4.0.tar.gz` & `tmp/arrendatools.plantillas-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrendatools.plantillas-0.4.0.tar", last modified: Wed Jun 14 18:56:35 2023, max compression
+gzip compressed data, was "arrendatools.plantillas-0.4.1.tar", last modified: Tue Jun 20 16:57:25 2023, max compression
```

## Comparing `arrendatools.plantillas-0.4.0.tar` & `arrendatools.plantillas-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1201 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:56:35.320671 arrendatools.plantillas-0.4.0/arrendatools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/arrendatools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/arrendatools/plantillas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/arrendatools/plantillas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/arrendatools/plantillas/filters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/arrendatools/plantillas/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3922 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/arrendatools/plantillas/filters/fechas.py
--rw-r--r--   0 root         (0) root         (0)     3175 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/arrendatools/plantillas/filters/numeros.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/arrendatools/plantillas/plantilla.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-14 18:56:35.000000 arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      538 2023-06-14 18:56:35.000000 arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 18:56:35.000000 arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-14 18:56:35.000000 arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 18:56:35.000000 arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1355 2023-06-14 18:56:32.000000 arrendatools.plantillas-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 18:56:35.324671 arrendatools.plantillas-0.4.0/test/
--rw-r--r--   0 root         (0) root         (0)     1798 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/test/test_fechas.py
--rw-r--r--   0 root         (0) root         (0)     1149 2023-06-14 18:56:31.000000 arrendatools.plantillas-0.4.0/test/test_numeros.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:57:25.114716 arrendatools.plantillas-0.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-06-20 16:57:21.000000 arrendatools.plantillas-0.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-20 16:57:25.114716 arrendatools.plantillas-0.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-06-20 16:57:21.000000 arrendatools.plantillas-0.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:57:25.110716 arrendatools.plantillas-0.4.1/arrendatools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 16:57:21.000000 arrendatools.plantillas-0.4.1/arrendatools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:57:25.114716 arrendatools.plantillas-0.4.1/arrendatools/plantillas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 16:57:21.000000 arrendatools.plantillas-0.4.1/arrendatools/plantillas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:57:25.114716 arrendatools.plantillas-0.4.1/arrendatools/plantillas/filters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 16:57:21.000000 arrendatools.plantillas-0.4.1/arrendatools/plantillas/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4709 2023-06-20 16:57:21.000000 arrendatools.plantillas-0.4.1/arrendatools/plantillas/filters/fechas.py
+-rw-r--r--   0 root         (0) root         (0)     3175 2023-06-20 16:57:21.000000 arrendatools.plantillas-0.4.1/arrendatools/plantillas/filters/numeros.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-06-20 16:57:21.000000 arrendatools.plantillas-0.4.1/arrendatools/plantillas/plantilla.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:57:25.114716 arrendatools.plantillas-0.4.1/arrendatools.plantillas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-20 16:57:25.000000 arrendatools.plantillas-0.4.1/arrendatools.plantillas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      538 2023-06-20 16:57:25.000000 arrendatools.plantillas-0.4.1/arrendatools.plantillas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 16:57:25.000000 arrendatools.plantillas-0.4.1/arrendatools.plantillas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-20 16:57:25.000000 arrendatools.plantillas-0.4.1/arrendatools.plantillas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 16:57:25.000000 arrendatools.plantillas-0.4.1/arrendatools.plantillas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-06-20 16:57:25.114716 arrendatools.plantillas-0.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-06-20 16:57:22.000000 arrendatools.plantillas-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:57:25.114716 arrendatools.plantillas-0.4.1/test/
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-06-20 16:57:21.000000 arrendatools.plantillas-0.4.1/test/test_fechas.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-06-20 16:57:21.000000 arrendatools.plantillas-0.4.1/test/test_numeros.py
```

### Comparing `arrendatools.plantillas-0.4.0/LICENSE` & `arrendatools.plantillas-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.0/PKG-INFO` & `arrendatools.plantillas-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools.plantillas
-Version: 0.4.0
+Version: 0.4.1
 Summary: Módulo de Python que aplica plantillas jinja. Además inlcuye filtros que pueden ser útiles para la generación de recibos de alquiler, facturas, informes,....
 Home-page: https://github.com/hokus15/ArrendaToolsPlantillas
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT License
         
         Copyright (c) 2023 Jordi
```

### Comparing `arrendatools.plantillas-0.4.0/README.md` & `arrendatools.plantillas-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.0/arrendatools/plantillas/filters/numeros.py` & `arrendatools.plantillas-0.4.1/arrendatools/plantillas/filters/numeros.py`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.0/arrendatools/plantillas/plantilla.py` & `arrendatools.plantillas-0.4.1/arrendatools/plantillas/plantilla.py`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/PKG-INFO` & `arrendatools.plantillas-0.4.1/arrendatools.plantillas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools.plantillas
-Version: 0.4.0
+Version: 0.4.1
 Summary: Módulo de Python que aplica plantillas jinja. Además inlcuye filtros que pueden ser útiles para la generación de recibos de alquiler, facturas, informes,....
 Home-page: https://github.com/hokus15/ArrendaToolsPlantillas
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT License
         
         Copyright (c) 2023 Jordi
```

### Comparing `arrendatools.plantillas-0.4.0/arrendatools.plantillas.egg-info/SOURCES.txt` & `arrendatools.plantillas-0.4.1/arrendatools.plantillas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.4.0/setup.py` & `arrendatools.plantillas-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 import pkg_resources
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 with open('LICENSE', encoding='utf-8') as f:
     license = f.read()
```

### Comparing `arrendatools.plantillas-0.4.0/test/test_fechas.py` & `arrendatools.plantillas-0.4.1/test/test_fechas.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,15 +24,21 @@
 
     def test_trimestre(self):
         self.assertEqual(trimestre('2023-01-01'), '1T 2023')
         self.assertEqual(trimestre('2023-05-01', delta=1), '3T 2023')
         self.assertEqual(trimestre('2023-12-31', delta=-2), '3T 2023')
 
     def test_dias_entre(self):
-        self.assertEqual(dias_entre('2023-01-01', '2023-12-31'), 364)
-        self.assertEqual(dias_entre('2023-01-01', '2024-01-01'), 365)
-        self.assertEqual(dias_entre('2023-06-01', '2024-01-01'), 214)
-        self.assertEqual(dias_entre('2024-01-01', '2025-01-01'), 366)
+        self.assertEqual(dias_entre('2023-01-01', '2023-12-31', '%Y-%m-%d', '%Y-%m-%d'), 364)
+        self.assertEqual(dias_entre('2023-12-01', '2023-12-31', '%Y-%m-%d', '%Y-%m-%d'), 30)
+        self.assertEqual(dias_entre('2023-12-01', '2024-01-01', '%Y-%m-%d', '%Y-%m-%d'), 31)
+        self.assertEqual(dias_entre('2023-01-01', '2024-01-01', '%Y-%m-%d', '%Y-%m-%d'), 365)
+        self.assertEqual(dias_entre('2023-06-01', '2024-01-01', '%Y-%m-%d', '%Y-%m-%d'), 214)
+        self.assertEqual(dias_entre('2024-01-01', '2025-01-01', '%Y-%m-%d', '%Y-%m-%d'), 366)
+        self.assertEqual(dias_entre('2022-06-01T22:00:00.000Z', '2022-12-31T23:00:00.000Z'), 213)
+        self.assertEqual(dias_entre('2022-06-01T22:00:00.000Z', '2023-01-01', formato_fin='%Y-%m-%d'), 213)
+        self.assertEqual(dias_entre('2022-06-02', '2023-01-01', '%Y-%m-%d', '%Y-%m-%d'), 213)
+        self.assertEqual(dias_entre('2022-06-02', '2022-12-31T23:00:00.000Z', formato_inicio='%Y-%m-%d'), 213)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arrendatools.plantillas-0.4.0/test/test_numeros.py` & `arrendatools.plantillas-0.4.1/test/test_numeros.py`

 * *Files identical despite different names*

