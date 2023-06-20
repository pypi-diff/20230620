# Comparing `tmp/vssource-0.9.4.tar.gz` & `tmp/vssource-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vssource-0.9.4.tar", last modified: Tue Jun 20 14:23:46 2023, max compression
+gzip compressed data, was "vssource-0.9.5.tar", last modified: Tue Jun 20 15:36:33 2023, max compression
```

## Comparing `vssource-0.9.4.tar` & `vssource-0.9.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.891149 vssource-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 14:23:16.000000 vssource-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-20 14:23:46.891149 vssource-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-20 14:23:16.000000 vssource-0.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-20 14:23:46.891149 vssource-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-20 14:23:16.000000 vssource-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.887149 vssource-0.9.4/vssource/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/dataclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.887149 vssource-0.9.4/vssource/formats/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.887149 vssource-0.9.4/vssource/formats/bd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/bd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.887149 vssource-0.9.4/vssource/formats/dvd/
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/dvd/IsoFile.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/dvd/IsoFileCore.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/dvd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.891149 vssource-0.9.4/vssource/formats/dvd/parsedvd/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/dvd/parsedvd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/dvd/parsedvd/sector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/formats/dvd/parsedvd/vts_pgci.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.891149 vssource-0.9.4/vssource/indexers/
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/indexers/D2VWitch.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/indexers/DGIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/indexers/DGIndexNV.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/indexers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/indexers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/indexers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-20 14:23:16.000000 vssource-0.9.4/vssource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:46.887149 vssource-0.9.4/vssource.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-20 14:23:46.000000 vssource-0.9.4/vssource.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-20 14:23:46.000000 vssource-0.9.4/vssource.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:23:46.000000 vssource-0.9.4/vssource.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 14:23:46.000000 vssource-0.9.4/vssource.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 14:23:46.000000 vssource-0.9.4/vssource.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.526875 vssource-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 15:36:10.000000 vssource-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-20 15:36:33.526875 vssource-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-20 15:36:10.000000 vssource-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-20 15:36:33.530876 vssource-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-20 15:36:10.000000 vssource-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.526875 vssource-0.9.5/vssource/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/dataclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.526875 vssource-0.9.5/vssource/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/formats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.526875 vssource-0.9.5/vssource/formats/bd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/formats/bd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.526875 vssource-0.9.5/vssource/formats/dvd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/formats/dvd/IsoFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/formats/dvd/IsoFileCore.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/formats/dvd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.526875 vssource-0.9.5/vssource/formats/dvd/parsedvd/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/formats/dvd/parsedvd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/formats/dvd/parsedvd/sector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/formats/dvd/parsedvd/vts_pgci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.526875 vssource-0.9.5/vssource/indexers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/indexers/D2VWitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/indexers/DGIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/indexers/DGIndexNV.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/indexers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/indexers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/indexers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-20 15:36:10.000000 vssource-0.9.5/vssource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.526875 vssource-0.9.5/vssource.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-20 15:36:33.000000 vssource-0.9.5/vssource.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-20 15:36:33.000000 vssource-0.9.5/vssource.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:36:33.000000 vssource-0.9.5/vssource.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 15:36:33.000000 vssource-0.9.5/vssource.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 15:36:33.000000 vssource-0.9.5/vssource.egg-info/top_level.txt
```

### Comparing `vssource-0.9.4/LICENSE` & `vssource-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/PKG-INFO` & `vssource-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vssource
-Version: 0.9.4
+Version: 0.9.5
 Summary: Vapoursynth Wrapper for DVDs stuff
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-source
 Project-URL: Documentation, https://vssource.encode.moe/en/latest/
```

### Comparing `vssource-0.9.4/README.md` & `vssource-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/setup.cfg` & `vssource-0.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/setup.py` & `vssource-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/vssource/dataclasses.py` & `vssource-0.9.5/vssource/dataclasses.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/vssource/formats/dvd/IsoFile.py` & `vssource-0.9.5/vssource/formats/dvd/IsoFile.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/vssource/formats/dvd/IsoFileCore.py` & `vssource-0.9.5/vssource/formats/dvd/IsoFileCore.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/vssource/formats/dvd/parsedvd/sector.py` & `vssource-0.9.5/vssource/formats/dvd/parsedvd/sector.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/vssource/formats/dvd/parsedvd/vts_pgci.py` & `vssource-0.9.5/vssource/formats/dvd/parsedvd/vts_pgci.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/vssource/funcs.py` & `vssource-0.9.5/vssource/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
             indexer_kwargs = dict[str, Any]()
             if idx_info.film >= film_thr:
                 indexer_kwargs |= dict(fieldop=1)
                 props |= dict(dgi_fieldop=1, _FieldBased=0)
 
             clip = indexer.source_func(filepath, **indexer_kwargs)
-        except (RuntimeError, AttributeError):
+        except (RuntimeError, AttributeError, FileNotFoundError):
             indexers = list[type[Indexer]]([LSMAS, D2VWitch, DGIndex])
 
             try:
                 from vspreview import is_preview
 
                 best_last = is_preview()
             except BaseException:
```

### Comparing `vssource-0.9.4/vssource/indexers/D2VWitch.py` & `vssource-0.9.5/vssource/indexers/D2VWitch.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/vssource/indexers/DGIndex.py` & `vssource-0.9.5/vssource/indexers/DGIndex.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/vssource/indexers/DGIndexNV.py` & `vssource-0.9.5/vssource/indexers/DGIndexNV.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/vssource/indexers/base.py` & `vssource-0.9.5/vssource/indexers/base.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/vssource/utils.py` & `vssource-0.9.5/vssource/utils.py`

 * *Files identical despite different names*

### Comparing `vssource-0.9.4/vssource.egg-info/PKG-INFO` & `vssource-0.9.5/vssource.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vssource
-Version: 0.9.4
+Version: 0.9.5
 Summary: Vapoursynth Wrapper for DVDs stuff
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-source
 Project-URL: Documentation, https://vssource.encode.moe/en/latest/
```

### Comparing `vssource-0.9.4/vssource.egg-info/SOURCES.txt` & `vssource-0.9.5/vssource.egg-info/SOURCES.txt`

 * *Files identical despite different names*

