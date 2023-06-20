# Comparing `tmp/m1nx4s_calculator-1.1.0.tar.gz` & `tmp/m1nx4s_calculator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m1nx4s_calculator-1.1.0.tar", last modified: Mon Jun 19 11:01:25 2023, max compression
+gzip compressed data, was "m1nx4s_calculator-1.2.0.tar", last modified: Tue Jun 20 08:49:05 2023, max compression
```

## Comparing `m1nx4s_calculator-1.1.0.tar` & `m1nx4s_calculator-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 11:01:25.984609 m1nx4s_calculator-1.1.0/
--rw-rw-rw-   0        0        0     1091 2023-06-14 08:21:18.000000 m1nx4s_calculator-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      339 2023-06-19 11:01:25.985608 m1nx4s_calculator-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2025 2023-06-19 10:46:20.000000 m1nx4s_calculator-1.1.0/README.md
--rw-rw-rw-   0        0        0      121 2023-06-19 11:01:25.991061 m1nx4s_calculator-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-06-15 08:15:16.000000 m1nx4s_calculator-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:01:25.881019 m1nx4s_calculator-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 11:01:25.941225 m1nx4s_calculator-1.1.0/src/calculator/
--rw-rw-rw-   0        0        0       50 2023-06-19 11:00:50.000000 m1nx4s_calculator-1.1.0/src/calculator/__init__.py
--rw-rw-rw-   0        0        0     1341 2023-06-19 07:09:46.000000 m1nx4s_calculator-1.1.0/src/calculator/calculator.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:01:25.972775 m1nx4s_calculator-1.1.0/src/m1nx4s_calculator.egg-info/
--rw-rw-rw-   0        0        0      339 2023-06-19 11:01:25.000000 m1nx4s_calculator-1.1.0/src/m1nx4s_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-19 11:01:25.000000 m1nx4s_calculator-1.1.0/src/m1nx4s_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 11:01:25.000000 m1nx4s_calculator-1.1.0/src/m1nx4s_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 11:01:25.000000 m1nx4s_calculator-1.1.0/src/m1nx4s_calculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 08:49:05.539943 m1nx4s_calculator-1.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-14 08:21:18.000000 m1nx4s_calculator-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      340 2023-06-20 08:49:05.540530 m1nx4s_calculator-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1324 2023-06-20 08:29:38.000000 m1nx4s_calculator-1.2.0/README.md
+-rw-rw-rw-   0        0        0      121 2023-06-20 08:49:05.553067 m1nx4s_calculator-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      457 2023-06-20 08:38:45.000000 m1nx4s_calculator-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:49:05.471213 m1nx4s_calculator-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 08:49:05.495368 m1nx4s_calculator-1.2.0/src/calculator/
+-rw-rw-rw-   0        0        0       50 2023-06-20 08:48:06.000000 m1nx4s_calculator-1.2.0/src/calculator/__init__.py
+-rw-rw-rw-   0        0        0     1284 2023-06-20 08:38:45.000000 m1nx4s_calculator-1.2.0/src/calculator/calculator.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:49:05.531069 m1nx4s_calculator-1.2.0/src/m1nx4s_calculator.egg-info/
+-rw-rw-rw-   0        0        0      340 2023-06-20 08:49:05.000000 m1nx4s_calculator-1.2.0/src/m1nx4s_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-20 08:49:05.000000 m1nx4s_calculator-1.2.0/src/m1nx4s_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:49:05.000000 m1nx4s_calculator-1.2.0/src/m1nx4s_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-20 08:49:05.000000 m1nx4s_calculator-1.2.0/src/m1nx4s_calculator.egg-info/top_level.txt
```

### Comparing `m1nx4s_calculator-1.1.0/LICENSE` & `m1nx4s_calculator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `m1nx4s_calculator-1.1.0/src/calculator/calculator.py` & `m1nx4s_calculator-1.2.0/src/calculator/calculator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 class Calculator:
     """
-    The main package file should contain a class Calculator that should be able to perform these actions:
+    The main package file contains a class Calculator that perform these actions:
     Addition / Subtraction.
     Multiplication / Division.
-    Take (n) root of a number.
     Reset memory (Calculator must have its own memory, meaning it will manipulate starting number 0 until it is reset.).
     """
 
     def __init__(self):
         self.memory = 0
 
     def add(self, num: int | float) -> float:
@@ -24,15 +23,15 @@
         """multiplication operation"""
         self.memory = self.memory * num
         return self.memory
 
     def div(self, num: int | float) -> float:
         """
         division operation
-        if num2 has digit = 0 operation, it will provide message that this operation is not possible
+        if num has digit = 0 operation, it will provide message that this operation is not possible
         """
         if num == 0:
             print("Divide by 0 Error is not possible")
         else:
             self.memory = round(self.memory / num, 2)
             return self.memory
```

