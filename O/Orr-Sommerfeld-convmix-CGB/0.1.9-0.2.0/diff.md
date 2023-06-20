# Comparing `tmp/orr_sommerfeld_convmix_cgb-0.1.9.tar.gz` & `tmp/orr_sommerfeld_convmix_cgb-0.2.0.tar.gz`

## Comparing `orr_sommerfeld_convmix_cgb-0.1.9.tar` & `orr_sommerfeld_convmix_cgb-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.9/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.9/src/Orr_Sommerfeld_convmix_CGB/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.9/LICENSE
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.9/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.0/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.0/src/Orr_Sommerfeld_convmix_CGB/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.0/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.0/PKG-INFO
```

### Comparing `orr_sommerfeld_convmix_cgb-0.1.9/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py` & `orr_sommerfeld_convmix_cgb-0.2.0/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.1.9/LICENSE` & `orr_sommerfeld_convmix_cgb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.1.9/pyproject.toml` & `orr_sommerfeld_convmix_cgb-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "Orr_Sommerfeld_convmix_CGB"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Pablo Szuban", email="pablo.szuban@ib.edu.ar" },
 ]
 description = "Paquete para cálculo de autovalores y autofunciones."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -15,7 +15,8 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+"Source Code" = "https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb"
```

