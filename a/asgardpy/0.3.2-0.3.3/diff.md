# Comparing `tmp/asgardpy-0.3.2.tar.gz` & `tmp/asgardpy-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgardpy-0.3.2.tar", last modified: Fri Apr 28 15:55:32 2023, max compression
+gzip compressed data, was "asgardpy-0.3.3.tar", last modified: Tue Jun 20 14:25:41 2023, max compression
```

## Comparing `asgardpy-0.3.2.tar` & `asgardpy-0.3.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:55:31.999454 asgardpy-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-28 15:55:14.000000 asgardpy-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-28 15:55:32.003454 asgardpy-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-28 15:55:14.000000 asgardpy-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:55:31.999454 asgardpy-0.3.2/asgardpy/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:55:31.999454 asgardpy-0.3.2/asgardpy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/analysis/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:55:31.999454 asgardpy-0.3.2/asgardpy/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/base/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/base/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/base/reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:55:31.999454 asgardpy-0.3.2/asgardpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/config/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:55:31.999454 asgardpy-0.3.2/asgardpy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/data/dataset_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/data/dataset_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/data/dl4.py
--rw-r--r--   0 runner    (1001) docker     (123)    32564 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/data/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:55:31.999454 asgardpy-0.3.2/asgardpy/io/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-28 15:55:14.000000 asgardpy-0.3.2/asgardpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:55:31.999454 asgardpy-0.3.2/asgardpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-28 15:55:31.000000 asgardpy-0.3.2/asgardpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-28 15:55:31.000000 asgardpy-0.3.2/asgardpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:55:31.000000 asgardpy-0.3.2/asgardpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-28 15:55:31.000000 asgardpy-0.3.2/asgardpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 15:55:31.000000 asgardpy-0.3.2/asgardpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 15:55:14.000000 asgardpy-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-28 15:55:32.003454 asgardpy-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-28 15:55:14.000000 asgardpy-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.810742 asgardpy-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-20 14:25:11.000000 asgardpy-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-20 14:25:41.810742 asgardpy-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-20 14:25:11.000000 asgardpy-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.806741 asgardpy-0.3.3/asgardpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.806741 asgardpy-0.3.3/asgardpy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/analysis/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.806741 asgardpy-0.3.3/asgardpy/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/base/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/base/reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.806741 asgardpy-0.3.3/asgardpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/config/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.810742 asgardpy-0.3.3/asgardpy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/data/dataset_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/data/dataset_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/data/dl4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32564 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/data/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.810742 asgardpy-0.3.3/asgardpy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.806741 asgardpy-0.3.3/asgardpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-20 14:25:41.000000 asgardpy-0.3.3/asgardpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-20 14:25:41.000000 asgardpy-0.3.3/asgardpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:25:41.000000 asgardpy-0.3.3/asgardpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-20 14:25:41.000000 asgardpy-0.3.3/asgardpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 14:25:41.000000 asgardpy-0.3.3/asgardpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 14:25:12.000000 asgardpy-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-20 14:25:41.810742 asgardpy-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-20 14:25:12.000000 asgardpy-0.3.3/setup.py
```

### Comparing `asgardpy-0.3.2/LICENSE` & `asgardpy-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.2/PKG-INFO` & `asgardpy-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgardpy
-Version: 0.3.2
+Version: 0.3.3
 Summary: Gammapy-based pipeline for easy joint analysis of different gamma-ray datasets
 Home-page: https://github.com/chaimain/asgardpy
 Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.1.tar.gz
 Author: Chaitanya Priyadarshi
 Author-email: chaitanya.p.astrphys@gmail.com
 License: Apache
 Classifier: Intended Audience :: Science/Research
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
+# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
 Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent selection cut MAGIC/LST [PointSkyRegion geometry for ON region] + 1D fixed-cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
-Follow the [Gammapy v1.0](https://docs.gammapy.org/1.0/) documentation for understanding the core Gammapy objects.
+Follow the [Gammapy v1.1](https://docs.gammapy.org/1.1/) documentation for understanding the core Gammapy objects.
 
 The various Data Levels	used here follow the descriptions suggested by [GADF v0.3](https://gamma-astro-data-formats.readthedocs.io/en/latest/) and CTAO Data Model
 
 # Pipeline development
 
-The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent selection cuts) for point-like sources. 
+The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent selection cuts) for point-like sources.
 The pipeline can be further expanded to support more types of DL3 files of gamma-ray instruments.
 
 An example of configuration file that can be used with asgardpy can be found at ``asgardpy/config/template.yaml``
 Examples of usage of asgardpy is shown in jupyter notebooks in ``notebooks/`` but as there are no public test data included with the pipeline yet, the results are empty.
 
 # Pipeline Template
```

### Comparing `asgardpy-0.3.2/README.md` & `asgardpy-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
+# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
 Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent selection cut MAGIC/LST [PointSkyRegion geometry for ON region] + 1D fixed-cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
-Follow the [Gammapy v1.0](https://docs.gammapy.org/1.0/) documentation for understanding the core Gammapy objects.
+Follow the [Gammapy v1.1](https://docs.gammapy.org/1.1/) documentation for understanding the core Gammapy objects.
 
 The various Data Levels	used here follow the descriptions suggested by [GADF v0.3](https://gamma-astro-data-formats.readthedocs.io/en/latest/) and CTAO Data Model
 
 # Pipeline development
 
-The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent selection cuts) for point-like sources. 
+The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent selection cuts) for point-like sources.
 The pipeline can be further expanded to support more types of DL3 files of gamma-ray instruments.
 
 An example of configuration file that can be used with asgardpy can be found at ``asgardpy/config/template.yaml``
 Examples of usage of asgardpy is shown in jupyter notebooks in ``notebooks/`` but as there are no public test data included with the pipeline yet, the results are empty.
 
 # Pipeline Template
```

### Comparing `asgardpy-0.3.2/asgardpy/analysis/analysis.py` & `asgardpy-0.3.3/asgardpy/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.2/asgardpy/base/__init__.py` & `asgardpy-0.3.3/asgardpy/base/__init__.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.2/asgardpy/base/base.py` & `asgardpy-0.3.3/asgardpy/base/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,16 +156,14 @@
 
 
 class AnalysisStepEnum(str, Enum):
     datasets_1d = "datasets-1d"
     datasets_3d = "datasets-3d"
     fit = "fit"
     flux_points = "flux-points"
-    excess_map = "excess-map"
-    light_curve = "light-curve"
 
 
 # Basic Quantity ranges Type for building the Config
 class TimeRangeConfig(BaseConfig):
     start: TimeType = Time("0", format="mjd")
     stop: TimeType = Time("0", format="mjd")
```

### Comparing `asgardpy-0.3.2/asgardpy/base/geom.py` & `asgardpy-0.3.3/asgardpy/base/geom.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.2/asgardpy/base/reduction.py` & `asgardpy-0.3.3/asgardpy/base/reduction.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.2/asgardpy/config/generator.py` & `asgardpy-0.3.3/asgardpy/config/generator.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.2/asgardpy/data/__init__.py` & `asgardpy-0.3.3/asgardpy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.2/asgardpy/data/dataset_1d.py` & `asgardpy-0.3.3/asgardpy/data/dataset_1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from asgardpy.io import DL3Files, InputConfig
 
 __all__ = [
     "Datasets1DAnalysisStep",
     "Dataset1DBaseConfig",
     "Dataset1DConfig",
     "Dataset1DGeneration",
+    "Dataset1DInfoConfig",
 ]
 
 log = logging.getLogger(__name__)
 
 
 # Defining various components of 1D Dataset Config section
 class Dataset1DInfoConfig(BaseConfig):
```

### Comparing `asgardpy-0.3.2/asgardpy/data/dataset_3d.py` & `asgardpy-0.3.3/asgardpy/data/dataset_3d.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.2/asgardpy/data/dl4.py` & `asgardpy-0.3.3/asgardpy/data/dl4.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,25 +21,32 @@
 
 # Defining various components of High-level Analysis Config
 class BackendEnum(str, Enum):
     minuit = "minuit"
     scipy = "scipy"
 
 
+class ParallelBackendEnum(str, Enum):
+    multi = "multiprocessing"
+    ray = "ray"
+
+
 class FitConfig(BaseConfig):
     fit_range: EnergyRangeConfig = EnergyRangeConfig()
     backend: BackendEnum = BackendEnum.minuit
     optimize_opts: dict = {}
     covariance_opts: dict = {}
     confidence_opts: dict = {}
     store_trace: bool = True
 
 
 class FluxPointsConfig(BaseConfig):
     parameters: dict = {"selection_optional": "all"}
+    parallel_backend: ParallelBackendEnum = ParallelBackendEnum.multi
+    reoptimize: bool = False
 
 
 # The main Analysis Steps
 class FitAnalysisStep(AnalysisStepBase):
     """
     Using the Fitting parameters as defined in the Config, with the given
     datasets perform the fit of the models to the updated list of datasets.
@@ -110,15 +117,20 @@
         """
         Setup the Gammapy FluxPointsEstimator function with all the
         provided parameters.
         """
         fpe_settings = self.config.flux_points_params.parameters
 
         self.fpe = FluxPointsEstimator(
-            energy_edges=energy_bin_edges, source=self.config.target.source_name, **fpe_settings
+            energy_edges=energy_bin_edges,
+            source=self.config.target.source_name,
+            n_jobs=self.config.general.n_jobs,
+            parallel_backend=self.config.flux_points_params.parallel_backend,
+            reoptimize=self.config.flux_points_params.reoptimize,
+            **fpe_settings
         )
 
     def _sort_datasets_info(self):
         """
         The given list of datasets may contain sub-instrument level datasets.
         With the help of the dict information for instrument specific name and
         spectral energy edges, this function, sorts the datasets and returns
```

### Comparing `asgardpy-0.3.2/asgardpy/data/target.py` & `asgardpy-0.3.3/asgardpy/data/target.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.2/asgardpy/io/io.py` & `asgardpy-0.3.3/asgardpy/io/io.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.2/asgardpy.egg-info/PKG-INFO` & `asgardpy-0.3.3/asgardpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgardpy
-Version: 0.3.2
+Version: 0.3.3
 Summary: Gammapy-based pipeline for easy joint analysis of different gamma-ray datasets
 Home-page: https://github.com/chaimain/asgardpy
 Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.1.tar.gz
 Author: Chaitanya Priyadarshi
 Author-email: chaitanya.p.astrphys@gmail.com
 License: Apache
 Classifier: Intended Audience :: Science/Research
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
+# asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
 Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent selection cut MAGIC/LST [PointSkyRegion geometry for ON region] + 1D fixed-cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
-Follow the [Gammapy v1.0](https://docs.gammapy.org/1.0/) documentation for understanding the core Gammapy objects.
+Follow the [Gammapy v1.1](https://docs.gammapy.org/1.1/) documentation for understanding the core Gammapy objects.
 
 The various Data Levels	used here follow the descriptions suggested by [GADF v0.3](https://gamma-astro-data-formats.readthedocs.io/en/latest/) and CTAO Data Model
 
 # Pipeline development
 
-The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent selection cuts) for point-like sources. 
+The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent selection cuts) for point-like sources.
 The pipeline can be further expanded to support more types of DL3 files of gamma-ray instruments.
 
 An example of configuration file that can be used with asgardpy can be found at ``asgardpy/config/template.yaml``
 Examples of usage of asgardpy is shown in jupyter notebooks in ``notebooks/`` but as there are no public test data included with the pipeline yet, the results are empty.
 
 # Pipeline Template
```

### Comparing `asgardpy-0.3.2/asgardpy.egg-info/SOURCES.txt` & `asgardpy-0.3.3/asgardpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.2/setup.py` & `asgardpy-0.3.3/setup.py`

 * *Files identical despite different names*

