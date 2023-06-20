# Comparing `tmp/pdr-1.0.0.tar.gz` & `tmp/pdr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdr-1.0.0.tar", last modified: Mon Jun  5 15:59:17 2023, max compression
+gzip compressed data, was "pdr-1.0.1.tar", last modified: Tue Jun 20 17:24:19 2023, max compression
```

## Comparing `pdr-1.0.0.tar` & `pdr-1.0.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:59:17.171064 pdr-1.0.0/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1524 2023-05-02 18:30:59.000000 pdr-1.0.0/LICENSE
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    10893 2023-06-05 15:59:17.171064 pdr-1.0.0/PKG-INFO
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    10315 2023-06-05 15:54:39.000000 pdr-1.0.0/README.md
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:59:17.167063 pdr-1.0.0/pdr/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      560 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3956 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/_scaling.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5212 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/bit_handling.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    11544 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/browsify.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7128 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/datatypes.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       97 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/errors.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:59:17.167063 pdr-1.0.0/pdr/formats/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      602 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3846 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/cassini.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    12685 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/checkers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      940 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/clementine.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      650 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/diviner.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      993 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/galileo.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      884 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/juno.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1940 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/lro.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      125 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/lroc.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      335 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/mex_marsis.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2039 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/mgn.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      420 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/mgs.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      214 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/msl_apxs.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      210 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/msl_ccam.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      518 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/msl_cmn.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      530 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/pvo.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      221 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/rosetta.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1053 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/formats/themis.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5457 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/func.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:59:17.171064 pdr-1.0.0/pdr/loaders/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2039 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/_helpers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4623 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/datawrap.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     4398 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/dispatch.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2767 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/handlers.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     5219 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/image.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    17607 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/queries.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     6429 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/table.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     2473 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/text.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1516 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/loaders/utility.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     3493 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/np_utils.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:59:17.171064 pdr-1.0.0/pdr/parselabel/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-05-02 18:30:59.000000 pdr-1.0.0/pdr/parselabel/__init__.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    11104 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/parselabel/pds3.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1397 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/parselabel/pds4.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      731 2023-05-02 18:30:59.000000 pdr-1.0.0/pdr/parselabel/utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     7294 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/pd_utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    26437 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/pdr.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      208 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/pdrtypes.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      490 2023-05-02 18:30:59.000000 pdr-1.0.0/pdr/pvl_utils.py
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     6652 2023-06-05 15:54:44.000000 pdr-1.0.0/pdr/utils.py
-drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:59:17.167063 pdr-1.0.0/pdr.egg-info/
--rw-rw-r--   0 sierra    (1000) sierra    (1000)    10893 2023-06-05 15:59:17.000000 pdr-1.0.0/pdr.egg-info/PKG-INFO
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1086 2023-06-05 15:59:17.000000 pdr-1.0.0/pdr.egg-info/SOURCES.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2023-06-05 15:59:17.000000 pdr-1.0.0/pdr.egg-info/dependency_links.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)      177 2023-06-05 15:59:17.000000 pdr-1.0.0/pdr.egg-info/requires.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)        4 2023-06-05 15:59:17.000000 pdr-1.0.0/pdr.egg-info/top_level.txt
--rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2023-06-05 15:59:17.171064 pdr-1.0.0/setup.cfg
--rw-rw-r--   0 sierra    (1000) sierra    (1000)     1076 2023-06-05 15:54:44.000000 pdr-1.0.0/setup.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-20 17:24:19.648991 pdr-1.0.1/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1524 2023-05-02 18:30:59.000000 pdr-1.0.1/LICENSE
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    10893 2023-06-20 17:24:19.648991 pdr-1.0.1/PKG-INFO
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    10315 2023-06-20 17:15:41.000000 pdr-1.0.1/README.md
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-20 17:24:19.644991 pdr-1.0.1/pdr/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      595 2023-06-20 17:15:58.000000 pdr-1.0.1/pdr/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3956 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/_scaling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5212 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/bit_handling.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    11544 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/browsify.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     7128 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/datatypes.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       97 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/errors.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-20 17:24:19.648991 pdr-1.0.1/pdr/formats/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      602 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3846 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/cassini.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    12685 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/formats/checkers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      940 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/clementine.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      650 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/diviner.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      993 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/formats/galileo.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      884 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/juno.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1940 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/lro.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      125 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/lroc.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      335 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/mex_marsis.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2039 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/formats/mgn.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      420 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/mgs.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      214 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/msl_apxs.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      210 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/msl_ccam.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      518 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/msl_cmn.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      530 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/pvo.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      221 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/rosetta.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1053 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/formats/themis.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5457 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/func.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-20 17:24:19.648991 pdr-1.0.1/pdr/loaders/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2039 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/_helpers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4623 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/datawrap.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     4398 2023-06-13 19:04:43.000000 pdr-1.0.1/pdr/loaders/dispatch.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2767 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/handlers.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     5219 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/image.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    17607 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/loaders/queries.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     6429 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/loaders/table.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     2473 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/text.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1516 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/loaders/utility.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     3493 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/np_utils.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-20 17:24:19.648991 pdr-1.0.1/pdr/parselabel/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        0 2023-05-02 18:30:59.000000 pdr-1.0.1/pdr/parselabel/__init__.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    11104 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/parselabel/pds3.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1397 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/parselabel/pds4.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      731 2023-05-02 18:30:59.000000 pdr-1.0.1/pdr/parselabel/utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     7294 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/pd_utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    26437 2023-06-20 17:15:41.000000 pdr-1.0.1/pdr/pdr.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      208 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/pdrtypes.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      490 2023-05-02 18:30:59.000000 pdr-1.0.1/pdr/pvl_utils.py
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     6652 2023-06-05 15:54:44.000000 pdr-1.0.1/pdr/utils.py
+drwxrwxr-x   0 sierra    (1000) sierra    (1000)        0 2023-06-20 17:24:19.644991 pdr-1.0.1/pdr.egg-info/
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)    10893 2023-06-20 17:24:19.000000 pdr-1.0.1/pdr.egg-info/PKG-INFO
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1086 2023-06-20 17:24:19.000000 pdr-1.0.1/pdr.egg-info/SOURCES.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        1 2023-06-20 17:24:19.000000 pdr-1.0.1/pdr.egg-info/dependency_links.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)      177 2023-06-20 17:24:19.000000 pdr-1.0.1/pdr.egg-info/requires.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)        4 2023-06-20 17:24:19.000000 pdr-1.0.1/pdr.egg-info/top_level.txt
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)       38 2023-06-20 17:24:19.648991 pdr-1.0.1/setup.cfg
+-rw-rw-r--   0 sierra    (1000) sierra    (1000)     1076 2023-06-20 17:15:58.000000 pdr-1.0.1/setup.py
```

### Comparing `pdr-1.0.0/LICENSE` & `pdr-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/PKG-INFO` & `pdr-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr
-Version: 1.0.0
+Version: 1.0.1
 Summary: Planetary Data Reader
 Home-page: https://github.com/MillionConcepts/pdr
 Author: Chase Million
 Author-email: chase@millionconcepts.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pdr-1.0.0/README.md` & `pdr-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/_scaling.py` & `pdr-1.0.1/pdr/_scaling.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/bit_handling.py` & `pdr-1.0.1/pdr/bit_handling.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/browsify.py` & `pdr-1.0.1/pdr/browsify.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/datatypes.py` & `pdr-1.0.1/pdr/datatypes.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/formats/__init__.py` & `pdr-1.0.1/pdr/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/formats/cassini.py` & `pdr-1.0.1/pdr/formats/cassini.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/formats/checkers.py` & `pdr-1.0.1/pdr/formats/checkers.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/formats/clementine.py` & `pdr-1.0.1/pdr/formats/clementine.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/formats/diviner.py` & `pdr-1.0.1/pdr/formats/diviner.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/formats/galileo.py` & `pdr-1.0.1/pdr/formats/galileo.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/formats/juno.py` & `pdr-1.0.1/pdr/formats/juno.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/formats/lro.py` & `pdr-1.0.1/pdr/formats/lro.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/formats/mgn.py` & `pdr-1.0.1/pdr/formats/mgn.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/formats/msl_cmn.py` & `pdr-1.0.1/pdr/formats/msl_cmn.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/formats/pvo.py` & `pdr-1.0.1/pdr/formats/pvo.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/formats/themis.py` & `pdr-1.0.1/pdr/formats/themis.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/func.py` & `pdr-1.0.1/pdr/func.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/loaders/_helpers.py` & `pdr-1.0.1/pdr/loaders/_helpers.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/loaders/datawrap.py` & `pdr-1.0.1/pdr/loaders/datawrap.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/loaders/dispatch.py` & `pdr-1.0.1/pdr/loaders/dispatch.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/loaders/handlers.py` & `pdr-1.0.1/pdr/loaders/handlers.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/loaders/image.py` & `pdr-1.0.1/pdr/loaders/image.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/loaders/queries.py` & `pdr-1.0.1/pdr/loaders/queries.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/loaders/table.py` & `pdr-1.0.1/pdr/loaders/table.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/loaders/text.py` & `pdr-1.0.1/pdr/loaders/text.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/loaders/utility.py` & `pdr-1.0.1/pdr/loaders/utility.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/np_utils.py` & `pdr-1.0.1/pdr/np_utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/parselabel/pds3.py` & `pdr-1.0.1/pdr/parselabel/pds3.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/parselabel/pds4.py` & `pdr-1.0.1/pdr/parselabel/pds4.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/parselabel/utils.py` & `pdr-1.0.1/pdr/parselabel/utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/pd_utils.py` & `pdr-1.0.1/pdr/pd_utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/pdr.py` & `pdr-1.0.1/pdr/pdr.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr/utils.py` & `pdr-1.0.1/pdr/utils.py`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/pdr.egg-info/PKG-INFO` & `pdr-1.0.1/pdr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdr
-Version: 1.0.0
+Version: 1.0.1
 Summary: Planetary Data Reader
 Home-page: https://github.com/MillionConcepts/pdr
 Author: Chase Million
 Author-email: chase@millionconcepts.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pdr-1.0.0/pdr.egg-info/SOURCES.txt` & `pdr-1.0.1/pdr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdr-1.0.0/setup.py` & `pdr-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pdr",
-    version="1.0.0",
+    version="1.0.1",
     author="Chase Million",
     author_email="chase@millionconcepts.com",
     description="Planetary Data Reader",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MillionConcepts/pdr",
     packages=setuptools.find_packages(),
```

