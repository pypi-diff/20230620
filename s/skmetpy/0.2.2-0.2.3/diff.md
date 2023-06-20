# Comparing `tmp/skmetpy-0.2.2.tar.gz` & `tmp/skmetpy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.2.2.tar", last modified: Tue Jun 20 10:10:02 2023, max compression
+gzip compressed data, was "skmetpy-0.2.3.tar", last modified: Tue Jun 20 10:11:53 2023, max compression
```

## Comparing `skmetpy-0.2.2.tar` & `skmetpy-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 10:10:02.044241 skmetpy-0.2.2/
--rw-rw-rw-   0        0        0      259 2023-06-20 10:10:02.043241 skmetpy-0.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 10:10:02.038236 skmetpy-0.2.2/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.2.2/nunpy/__init__.py
--rw-rw-rw-   0        0        0    30811 2023-06-20 10:09:36.000000 skmetpy-0.2.2/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-20 10:10:02.044241 skmetpy-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-20 10:09:55.000000 skmetpy-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:10:02.042239 skmetpy-0.2.2/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-20 10:10:01.000000 skmetpy-0.2.2/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-20 10:10:01.000000 skmetpy-0.2.2/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 10:10:01.000000 skmetpy-0.2.2/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 10:10:01.000000 skmetpy-0.2.2/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 10:11:53.198480 skmetpy-0.2.3/
+-rw-rw-rw-   0        0        0      259 2023-06-20 10:11:53.197877 skmetpy-0.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 10:11:53.189470 skmetpy-0.2.3/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.2.3/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    30825 2023-06-20 10:11:41.000000 skmetpy-0.2.3/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 10:11:53.198480 skmetpy-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-20 10:11:51.000000 skmetpy-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:11:53.196874 skmetpy-0.2.3/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-20 10:11:53.000000 skmetpy-0.2.3/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-20 10:11:53.000000 skmetpy-0.2.3/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:11:53.000000 skmetpy-0.2.3/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 10:11:53.000000 skmetpy-0.2.3/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.2.2/nunpy/rechape.py` & `skmetpy-0.2.3/nunpy/rechape.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     list2()
     list3()
     list4()
     listplot()
 
 
 def list1():
-    print(f"REDES NEURONALES"
+    print(f"REDES NEURONALES\n"
           f"0 - list1()\n"
           f"1 - pasos1()\n"
           f"2 - carga1()\n"
           f"3 - hold1()\n"
           f"4 - norm1()\n"
           f"5 - ini1()\n"
           f"6 - fordw1()\n"
@@ -21,50 +21,50 @@
           f"10 - unroll1()\n"
           f"11 - pred1()\n"
           f"12 - nnsk1()\n"
           )
 
 
 def list2():
-    print(f"RECOMENDACION"
+    print(f"RECOMENDACION\n"
           f"0 - list2()\n"
           f"1 - pasos2()\n"
           f"2 - carga2()\n"
           f"3 - rank2()\n"
           f"4 - cost2()\n"
           f"5 - grad2()\n"
           f"6 - fmin2()\n"
           f"7 - recom2()\n"
           f"8 - simi2()\n"
           f"9 - km2()\n"
           f"10 - checkG2()\n")
 
 def list3():
-    print(f"CLUSTERING"
+    print(f"CLUSTERING\n"
           f"0 - list3()\n"
           f"1 - pasos3()\n"
           f"2 - carga3()\n"
           f"3 - fcc3()\n"
           f"4 - compc3()\n"
           f"5 - kmean3()\n"
           f"6 - randini3()\n"
           f"7 - elbow3()\n"
           f"8 - clustsk3()\n")
 
 def list4():
-    print(f"Lineal y Logistica"
+    print(f"Lineal y Logistica\n"
           f"0 - list4()\n"
           f"1 - rlineal4()\n"
           f"2 - rlogi4()\n")
 
 
 def listplot():
-    print(f"PLOT"
-          f"0 - listplot()"
-          f"1 - plot()"
+    print(f"PLOT\n"
+          f"0 - listplot()\n"
+          f"1 - plot()\n"
           f"2 - frontera()\n"
           f"3 - seaborn()\n")
 
 def pasos1():
     print("1 - Carga de datos\n"
           "2 - Holdout\n"
           "3 - Normaliza\n"
```

