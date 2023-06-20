# Comparing `tmp/ecoengine-0.0.6.tar.gz` & `tmp/ecoengine-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoengine-0.0.6.tar", last modified: Tue May 23 19:02:04 2023, max compression
+gzip compressed data, was "ecoengine-0.0.7.tar", last modified: Tue Jun 20 19:02:34 2023, max compression
```

## Comparing `ecoengine-0.0.6.tar` & `ecoengine-0.0.7.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.918220 ecoengine-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 19:01:31.000000 ecoengine-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-23 19:02:04.918220 ecoengine-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-23 19:01:31.000000 ecoengine-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 19:01:31.000000 ecoengine-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-23 19:02:04.918220 ecoengine-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 19:01:31.000000 ecoengine-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.914220 ecoengine-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.914220 ecoengine-0.0.6/src/ecoengine/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.914220 ecoengine-0.0.6/src/ecoengine/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/constants/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.914220 ecoengine-0.0.6/src/ecoengine/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.918220 ecoengine-0.0.6/src/ecoengine/data/load_shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/apartment.json
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/elementary_school.json
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/food_service_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/food_service_b.json
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/junior_high.json
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/mens_dorm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/motel.json
--rw-r--r--   0 runner    (1001) docker     (123)    47218 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/multi_family.json
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/nursing_home.json
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/office_building.json
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/senior_high.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/data/load_shapes/womens_dorm.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.918220 ecoengine-0.0.6/src/ecoengine/engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/engine/BuildingCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/engine/EcosizerEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/engine/SystemCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.918220 ecoengine-0.0.6/src/ecoengine/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/Building.py
--rw-r--r--   0 runner    (1001) docker     (123)    36036 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/SystemConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/systemConfigUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.918220 ecoengine-0.0.6/src/ecoengine/objects/systems/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/systems/ParallelLoopTank.py
--rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/systems/SwingTank.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 19:01:31.000000 ecoengine-0.0.6/src/ecoengine/objects/systems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:02:04.914220 ecoengine-0.0.6/src/ecoengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-23 19:02:04.000000 ecoengine-0.0.6/src/ecoengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-23 19:02:04.000000 ecoengine-0.0.6/src/ecoengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:02:04.000000 ecoengine-0.0.6/src/ecoengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 19:02:04.000000 ecoengine-0.0.6/src/ecoengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 19:02:04.000000 ecoengine-0.0.6/src/ecoengine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 19:02:31.424986 ecoengine-0.0.7/
+-rw-rw-rw-   0        0        0       45 2023-04-13 18:49:37.000000 ecoengine-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3815 2023-06-20 19:02:34.788000 ecoengine-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3175 2023-04-11 19:29:37.000000 ecoengine-0.0.7/README.md
+-rw-rw-rw-   0        0        0      108 2023-03-28 18:57:57.000000 ecoengine-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      767 2023-06-20 19:02:34.818764 ecoengine-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-04-11 19:29:37.000000 ecoengine-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:02:31.460987 ecoengine-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 19:02:31.532987 ecoengine-0.0.7/src/ecoengine/
+-rw-rw-rw-   0        0        0      915 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:02:31.488987 ecoengine-0.0.7/src/ecoengine/constants/
+-rw-rw-rw-   0        0        0      572 2023-06-19 21:37:33.000000 ecoengine-0.0.7/src/ecoengine/constants/Constants.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/constants/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:02:31.504987 ecoengine-0.0.7/src/ecoengine/data/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:02:31.520987 ecoengine-0.0.7/src/ecoengine/data/load_shapes/
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/__init__.py
+-rw-rw-rw-   0        0        0     1295 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/apartment.json
+-rw-rw-rw-   0        0        0      971 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/elementary_school.json
+-rw-rw-rw-   0        0        0     1127 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/food_service_a.json
+-rw-rw-rw-   0        0        0     1272 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/food_service_b.json
+-rw-rw-rw-   0        0        0     1240 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/junior_high.json
+-rw-rw-rw-   0        0        0     1259 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/mens_dorm.json
+-rw-rw-rw-   0        0        0     1259 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/motel.json
+-rw-rw-rw-   0        0        0   259798 2023-05-26 20:26:21.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/multi_family.json
+-rw-rw-rw-   0        0        0     1273 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/nursing_home.json
+-rw-rw-rw-   0        0        0     1058 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/office_building.json
+-rw-rw-rw-   0        0        0     1120 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/senior_high.json
+-rw-rw-rw-   0        0        0     1219 2023-04-11 19:29:37.000000 ecoengine-0.0.7/src/ecoengine/data/load_shapes/womens_dorm.json
+drwxrwxrwx   0        0        0        0 2023-06-20 19:02:31.532987 ecoengine-0.0.7/src/ecoengine/engine/
+-rw-rw-rw-   0        0        0     8720 2023-06-13 16:15:20.000000 ecoengine-0.0.7/src/ecoengine/engine/BuildingCreator.py
+-rw-rw-rw-   0        0        0    10779 2023-06-20 18:37:08.000000 ecoengine-0.0.7/src/ecoengine/engine/EcosizerEngine.py
+-rw-rw-rw-   0        0        0     4047 2023-06-19 17:36:14.000000 ecoengine-0.0.7/src/ecoengine/engine/Simulator.py
+-rw-rw-rw-   0        0        0     4540 2023-06-15 17:18:04.000000 ecoengine-0.0.7/src/ecoengine/engine/SystemCreator.py
+-rw-rw-rw-   0        0        0      894 2023-04-11 19:29:38.000000 ecoengine-0.0.7/src/ecoengine/engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:02:31.548987 ecoengine-0.0.7/src/ecoengine/objects/
+-rw-rw-rw-   0        0        0    10098 2023-06-20 18:36:29.000000 ecoengine-0.0.7/src/ecoengine/objects/Building.py
+-rw-rw-rw-   0        0        0     4957 2023-06-20 18:12:14.000000 ecoengine-0.0.7/src/ecoengine/objects/PrefMapTracker.py
+-rw-rw-rw-   0        0        0    12246 2023-06-19 17:44:26.000000 ecoengine-0.0.7/src/ecoengine/objects/SimulationRun.py
+-rw-rw-rw-   0        0        0    38112 2023-06-20 18:41:57.000000 ecoengine-0.0.7/src/ecoengine/objects/SystemConfig.py
+-rw-rw-rw-   0        0        0      940 2023-04-11 19:29:38.000000 ecoengine-0.0.7/src/ecoengine/objects/__init__.py
+-rw-rw-rw-   0        0        0     3481 2023-05-30 20:59:48.000000 ecoengine-0.0.7/src/ecoengine/objects/systemConfigUtils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:02:31.568987 ecoengine-0.0.7/src/ecoengine/objects/systems/
+-rw-rw-rw-   0        0        0     4530 2023-06-15 17:19:45.000000 ecoengine-0.0.7/src/ecoengine/objects/systems/ParallelLoopTank.py
+-rw-rw-rw-   0        0        0    22528 2023-06-19 19:13:23.000000 ecoengine-0.0.7/src/ecoengine/objects/systems/SwingTank.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:29:38.000000 ecoengine-0.0.7/src/ecoengine/objects/systems/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:02:31.472987 ecoengine-0.0.7/src/ecoengine.egg-info/
+-rw-rw-rw-   0        0        0     3815 2023-06-20 19:02:30.000000 ecoengine-0.0.7/src/ecoengine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1543 2023-06-20 19:02:31.000000 ecoengine-0.0.7/src/ecoengine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 19:02:31.000000 ecoengine-0.0.7/src/ecoengine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-20 19:02:31.000000 ecoengine-0.0.7/src/ecoengine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-20 19:02:31.000000 ecoengine-0.0.7/src/ecoengine.egg-info/top_level.txt
```

### Comparing `ecoengine-0.0.6/PKG-INFO` & `ecoengine-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-Metadata-Version: 2.1
-Name: ecoengine
-Version: 0.0.6
-Summary: A software for sizing Heat Pump Water Heaters for buildings
-Home-page: https://ecosizer.ecotope.com/sizer/
-Author: Nolan
-Author-email: nolan@ecotope.com
-Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
-# EcosizerEngine
-
-### Requirements:
-
-This software requires a python version greater than or equal to 3.11 to be installed in the environment it is running in.
-
-### Using the package in scripts:
-
-1. Install the package with pip
-
-	$ pip install ecosizer-engine
-
-2. To import and use the tools in this package, add the following import statement to your script:
-
-	from ecosizer_engine_package import *
-
-You should now be able to use the features of EcosizerEngine in your script
-
-### Running locally in a container:
-First, clone the EcosizerEngine repo from github
-
-    $ git clone https://github.com/EcotopeResearch/EcosizerEngine.git
-
-Depending on what type of environment you want to run the code in, please follow the appropriate steps.
-
-Steps for installing in a virtual environment:
-1. Navigate to the EcosizerEngine directory. This should be the same directory level as src/, setup.py, and this README document.
-2. Run the following command:
-
-	$ pip install -e .
-
-This will install the ecosizer-engine package locally in editable format, such that changes you make in the source code here will be reflected in implementation.
-This pip install should also install all dependencies for ecosizer-engine (i.e. numpy, scipy, pytest, and plotly)
-
-Steps for installing using docker container:
-1. Navigate to the EcosizerEngine directory.
-2. Build container with docker file
-
-	$ docker build -t ecosizerengine:latest .
-
-3. Run docker container
-
-	$  docker run -it ecosizerengine bash
-
-4. When you are done messing about in the docker image, just type the command
-
-	$ exit
-
-or press ctrl+c then ctrl+d
-
-Steps for installing conda environment from the Anaconda prompt:
-1. Navigate to the EcosizerEngine directory.
-2. Create new environment from .yml file.
-
-
-	$ conda env create --file EcosizerEngine.yml
-
-If the environment creation doesn't work, make sure Anaconda is up-to-date with
-
-    $ conda update --all
-
-If that doesn't work, you may need to force Anaconda to download and use python 3.11 (it defaults to 3.9) by making another environment
-
-    $ conda create -n py311 python=3.11
-    $ conda activate py311
-    $ conda env create --file EcosizerEngine.yml
-
-3. Check that the environment was created
-
-
-	$ conda env list
-
-4. Activate the new environment
-
-
-	$ conda activate EcosizerEngine
-
-If an environment already exits it can be removed with:
-
-	$ conda remove --name EcosizerEngine --all
-
-
-All the available environment can be found with:
-
-	$ conda env list
-
-### Testing:
-From the parent directory, type
-
-	$ python -m pytest
-
-This will run all unit tests for the package
-
-### Updating Documentation:
-1. If not installed in environment: pip install sphinx and numpydocs
-2. navigate to docs directory and run:
-
-
-	$ make html
-
-### Updating version on pypi
-
-1. If you haven't installed them before, pip install build and twine
-
-	$ python -m pip install --upgrade build
-
-
-	$ python -m pip install --user --upgrade twine
-
-2. Update the version number in setup.cfg
-3. Run the following commands from the project root directory:
-
-	$ python -m build
-
-	$ python -m twine upload dist/*
-
-### Contact Information
-To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
+Metadata-Version: 2.1
+Name: ecoengine
+Version: 0.0.7
+Summary: A software for sizing Heat Pump Water Heaters for buildings
+Home-page: https://ecosizer.ecotope.com/sizer/
+Author: Nolan
+Author-email: nolan@ecotope.com
+Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+
+# EcosizerEngine
+
+### Requirements:
+
+This software requires a python version greater than or equal to 3.11 to be installed in the environment it is running in.
+
+### Using the package in scripts:
+
+1. Install the package with pip
+
+	$ pip install ecosizer-engine
+
+2. To import and use the tools in this package, add the following import statement to your script:
+
+	from ecosizer_engine_package import *
+
+You should now be able to use the features of EcosizerEngine in your script
+
+### Running locally in a container:
+First, clone the EcosizerEngine repo from github
+
+    $ git clone https://github.com/EcotopeResearch/EcosizerEngine.git
+
+Depending on what type of environment you want to run the code in, please follow the appropriate steps.
+
+Steps for installing in a virtual environment:
+1. Navigate to the EcosizerEngine directory. This should be the same directory level as src/, setup.py, and this README document.
+2. Run the following command:
+
+	$ pip install -e .
+
+This will install the ecosizer-engine package locally in editable format, such that changes you make in the source code here will be reflected in implementation.
+This pip install should also install all dependencies for ecosizer-engine (i.e. numpy, scipy, pytest, and plotly)
+
+Steps for installing using docker container:
+1. Navigate to the EcosizerEngine directory.
+2. Build container with docker file
+
+	$ docker build -t ecosizerengine:latest .
+
+3. Run docker container
+
+	$  docker run -it ecosizerengine bash
+
+4. When you are done messing about in the docker image, just type the command
+
+	$ exit
+
+or press ctrl+c then ctrl+d
+
+Steps for installing conda environment from the Anaconda prompt:
+1. Navigate to the EcosizerEngine directory.
+2. Create new environment from .yml file.
+
+
+	$ conda env create --file EcosizerEngine.yml
+
+If the environment creation doesn't work, make sure Anaconda is up-to-date with
+
+    $ conda update --all
+
+If that doesn't work, you may need to force Anaconda to download and use python 3.11 (it defaults to 3.9) by making another environment
+
+    $ conda create -n py311 python=3.11
+    $ conda activate py311
+    $ conda env create --file EcosizerEngine.yml
+
+3. Check that the environment was created
+
+
+	$ conda env list
+
+4. Activate the new environment
+
+
+	$ conda activate EcosizerEngine
+
+If an environment already exits it can be removed with:
+
+	$ conda remove --name EcosizerEngine --all
+
+
+All the available environment can be found with:
+
+	$ conda env list
+
+### Testing:
+From the parent directory, type
+
+	$ python -m pytest
+
+This will run all unit tests for the package
+
+### Updating Documentation:
+1. If not installed in environment: pip install sphinx and numpydocs
+2. navigate to docs directory and run:
+
+
+	$ make html
+
+### Updating version on pypi
+
+1. If you haven't installed them before, pip install build and twine
+
+	$ python -m pip install --upgrade build
+
+
+	$ python -m pip install --user --upgrade twine
+
+2. Update the version number in setup.cfg
+3. Run the following commands from the project root directory:
+
+	$ python -m build
+
+	$ python -m twine upload dist/*
+
+### Contact Information
+To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
```

### Comparing `ecoengine-0.0.6/README.md` & `ecoengine-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/__init__.py` & `ecoengine-0.0.7/src/ecoengine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/data/load_shapes/apartment.json` & `ecoengine-0.0.7/src/ecoengine/data/load_shapes/apartment.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/data/load_shapes/elementary_school.json` & `ecoengine-0.0.7/src/ecoengine/data/load_shapes/elementary_school.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/data/load_shapes/food_service_a.json` & `ecoengine-0.0.7/src/ecoengine/data/load_shapes/food_service_a.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/data/load_shapes/food_service_b.json` & `ecoengine-0.0.7/src/ecoengine/data/load_shapes/food_service_b.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/data/load_shapes/junior_high.json` & `ecoengine-0.0.7/src/ecoengine/data/load_shapes/junior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/data/load_shapes/mens_dorm.json` & `ecoengine-0.0.7/src/ecoengine/data/load_shapes/mens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/data/load_shapes/motel.json` & `ecoengine-0.0.7/src/ecoengine/data/load_shapes/motel.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/data/load_shapes/nursing_home.json` & `ecoengine-0.0.7/src/ecoengine/data/load_shapes/nursing_home.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/data/load_shapes/office_building.json` & `ecoengine-0.0.7/src/ecoengine/data/load_shapes/office_building.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/data/load_shapes/senior_high.json` & `ecoengine-0.0.7/src/ecoengine/data/load_shapes/senior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/data/load_shapes/womens_dorm.json` & `ecoengine-0.0.7/src/ecoengine/data/load_shapes/womens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/engine/BuildingCreator.py` & `ecoengine-0.0.7/src/ecoengine/engine/BuildingCreator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from ecoengine.objects.Building import *
 import numpy as np
+import csv
 
 def createBuilding(incomingT_F, magnitudeStat, supplyT_F, buildingType, loadshape = None, avgLoadshape = None,
-                    returnT_F = 0, flowRate = 0, gpdpp = 0, nBR = None, nApt = 0, Wapt = 0, standardGPD = None):
+                    returnT_F = 0, flowRate = 0, gpdpp = 0, nBR = None, nApt = 0, Wapt = 0, standardGPD = None,
+                    annual = False, zipCode = None, climateZone = None):
     
     """
     Initializes the building in which the HPWH system will be sized for
 
     Attributes
     ----------
     incomingT_F : float 
@@ -33,14 +35,20 @@
         5 bedroom units.
     nApt: integer
         The number of apartments. Use with Qdot_apt to determine total recirculation losses. (For multi-falmily buildings)
     Wapt:  float
         Watts of heat lost in through recirculation piping system. Used with N_apt to determine total recirculation losses. (For multi-falmily buildings)
     standardGPD : string
         indicates whether to use a standard gpdpp specification for multi-family buildings. Set to None if not using a standard gpdpp.
+    annual : boolean
+        indicates whether to use annual loadshape for multi-family buildings
+    zipCode : int
+        the CA zipcode the building resides in to determine the climate zone
+    climateZone : int
+        the CA climate zone the building resides in
 
     Raises
     ----------
     Exception: Error if buildingType is not in list of valid buildingType names.
 
     """
 
@@ -51,78 +59,102 @@
         else:
             if not isinstance(magnitudeStat, list) or len(buildingType) != len(magnitudeStat):
                 raise Exception("Missing values for multi-use building. Collected " + str(len(buildingType)) + " building types but collected " + 
                                 ("1" if not isinstance(magnitudeStat, list) else str(len(magnitudeStat)))+ " magnitude varriables")
             building_list = []
             for i in range(len(buildingType)):
                 building_list.append(createBuilding(incomingT_F, magnitudeStat[i], supplyT_F, buildingType[i], loadshape, avgLoadshape,
-                        returnT_F, flowRate, gpdpp, nBR, nApt, Wapt))
-            return MultiUse(building_list, incomingT_F, supplyT_F, returnT_F, flowRate)
+                        returnT_F, flowRate, gpdpp, nBR, nApt, Wapt, standardGPD, annual, zipCode, climateZone))
+            return MultiUse(building_list, incomingT_F, supplyT_F, returnT_F, flowRate, getClimateZone(zipCode, climateZone))
     
     #only one building type so there should only be one magnitude statistic 
     if isinstance(magnitudeStat, list):
         if len(magnitudeStat) == 1:
             magnitudeStat = magnitudeStat[0]
         else:
             raise Exception("Missing values for multi-use building. Collected 1 building type but collected " + str(len(magnitudeStat)) + " magnitude varriables")
     
     if not isinstance(buildingType, str):
             raise Exception("buildingType must be a string.")
     
     # check custom loadshape or install standard loadshape
-    if(loadshape is None):
-        loadshape = getLoadShape(buildingType)
-    else:
-        checkLoadShape(loadshape)
-    if(avgLoadshape is None):
-        avgLoadshape = getLoadShape(buildingType, 'Stream_Avg')
-    else:
-        checkLoadShape(avgLoadshape)
+    if annual:
+        loadshape = getLoadShape(buildingType, "Annual_Normalized")
+        avgLoadshape = loadshape
+    else: 
+        if(loadshape is None):
+            loadshape = getLoadShape(buildingType)
+        else:
+            checkLoadShape(loadshape)
+        if(avgLoadshape is None):
+            avgLoadshape = getLoadShape(buildingType, 'Stream_Avg')
+        else:
+            checkLoadShape(avgLoadshape, True)
 
     loadshape = np.array(loadshape) # TODO - this changes values of loadshape a bit, show this to scott
     avgLoadshape = np.array(avgLoadshape) # TODO - this changes values of loadshape a bit, show this to scott
 
+    climate = getClimateZone(zipCode, climateZone)
+
     match buildingType:
         case 'apartment':
-            return Apartment(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+            return Apartment(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
         case 'elementary_school':
-            return ElementarySchool(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+            return ElementarySchool(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
         case 'food_service_a':
-            return FoodServiceA(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+            return FoodServiceA(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
         case 'food_service_b':
-            return FoodServiceB(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+            return FoodServiceB(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
         case 'junior_high':
-            return JuniorHigh(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+            return JuniorHigh(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
         case 'mens_dorm':
-            return MensDorm(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+            return MensDorm(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
         case 'motel':
-            return Motel(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+            return Motel(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
         case 'nursing_home':
-            return NursingHome(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+            return NursingHome(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
         case 'office_building':
-            return OfficeBuilding(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+            return OfficeBuilding(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
         case 'senior_high':
-            return SeniorHigh(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+            return SeniorHigh(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
         case 'womens_dorm':
-            return WomensDorm(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+            return WomensDorm(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
         case 'multi_family':
-            return MultiFamily(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, gpdpp, nBR, nApt, Wapt, standardGPD)
+            return MultiFamily(magnitudeStat, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate, gpdpp, nBR, nApt, Wapt, standardGPD)
         case _:
             raise Exception("Unrecognized building type.")
         
 def getLoadShape(file_name, shape = 'Stream'):
-    if shape != 'Stream' and shape != 'Stream_Avg':
+    if shape != 'Stream' and shape != 'Stream_Avg' and shape != "Annual_Normalized":
         raise Exception("Mapping key not found for loadshapes, valid keys are: 'Stream', or 'Stream_Avg'")
+    if file_name != 'multi_family' and shape == "Annual_Normalized":
+        raise Exception("Annual simulation for non-multifamily buildings is not yet available.")
     try:
         with open(os.path.join(os.path.dirname(__file__), '../data/load_shapes/' + file_name + '.json')) as json_file:
             dataDict = json.load(json_file)
             return dataDict['loadshapes'][shape]
     except:
         raise Exception("No default loadshape found for building type " +file_name + ".")
         
-def checkLoadShape(loadshape):
+def checkLoadShape(loadshape, avgLS = False):
     if len(loadshape) != 24:
-        raise Exception("Loadshape must be of length 24 but instead has length of "+str(len(loadshape))+".")
+        raise Exception(("Average loadshape" if avgLS else "Loadshape") + " must be of length 24 but instead has length of "
+                        + str(len(loadshape))+".")
     if sum(loadshape) > 1 + 1e-3 or sum(loadshape) < 1 - 1e-3:
-        raise Exception("Sum of the loadshape does not equal 1. Loadshape needs to be normalized.")
+        raise Exception("Sum of the " + ("average loadshape" if avgLS else "loadshape") + " does not equal 1. Loadshape needs to be normalized.")
     if any(x < 0 for x in loadshape):
-        raise Exception("Can not have negative load shape values in loadshape.")
+        raise Exception("Can not have negative values in " + ("average loadshape" if avgLS else "loadshape") + ".")
+    
+def getClimateZone(zipCode = None, climateZone = None):
+    if not climateZone is None:
+        if not isinstance(climateZone, int) or climateZone < 1 or climateZone > 16:
+            raise Exception("Climate Zone must be a number between 1 and 16.")
+        return climateZone
+    elif not zipCode is None:
+        with open(os.path.join(os.path.dirname(__file__), '../data/climate_data/ZipCode_ClimateZone_Lookup.csv'), 'r') as file:
+            csv_reader = csv.reader(file)                
+            for row in csv_reader:
+                if str(zipCode) == row[0]:
+                    return int(row[1])
+            raise Exception(str(zipCode) + " is not a California zip code.")
+    else:
+        return None
```

### Comparing `ecoengine-0.0.6/src/ecoengine/engine/EcosizerEngine.py` & `ecoengine-0.0.7/src/ecoengine/engine/EcosizerEngine.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from .BuildingCreator import *
 from .SystemCreator import *
+from .Simulator import simulate
+from ecoengine.objects.SimulationRun import *
 
 print("EcosizerEngine Copyright (C) 2023  Ecotope Inc.")
 print("This program comes with ABSOLUTELY NO WARRANTY. This is free software, and you are welcome to redistribute under certain conditions; details check GNU AFFERO GENERAL PUBLIC LICENSE_08102020.docx.")
 
 class EcosizerEngine:
     """
     Initializes and sizes the HPWH system for a building based on the given parameters.
@@ -74,54 +76,85 @@
 
     """
 
     def __init__(self, incomingT_F, magnitudeStat, supplyT_F, storageT_F, percentUseable, aquaFract,
                             schematic, buildingType, loadshape = None, avgLoadshape = None, loadShiftSchedule = None, loadUpHours = None,
                             aquaFractLoadUp = None, aquaFractShed = None, loadUpT_F = None, loadShiftPercent = 1,
                             returnT_F = 0, flowRate = 0, gpdpp = 0, nBR = None, safetyTM = 1.75,
-                            defrostFactor = 1, compRuntime_hr = 16, nApt = 0, Wapt = 0, doLoadShift = False,
-                            setpointTM_F = 135, TMonTemp_F = 120, offTime_hr = 0.333, standardGPD = None):
+                            defrostFactor = 1, compRuntime_hr = 16, nApt = None, Wapt = None, doLoadShift = False,
+                            setpointTM_F = 135, TMonTemp_F = 120, offTime_hr = 0.333, standardGPD = None,
+                            PVol_G_atStorageT = None, PCap_kBTUhr = None, TMVol_G = None, TMCap_kBTUhr = None,
+                            annual = False, zipCode = None, climateZone = None, systemModel = None):
         
-        building = createBuilding( incomingT_F     = incomingT_F,
-                                    magnitudeStat  = magnitudeStat, 
-                                    supplyT_F       = supplyT_F, 
-                                    buildingType   = buildingType,
-                                    loadshape       = loadshape,
-                                    avgLoadshape    = avgLoadshape,
-                                    returnT_F       = returnT_F, 
-                                    flowRate       = flowRate,
-                                    gpdpp           = gpdpp,
-                                    nBR             = nBR,
-                                    nApt            = nApt,
-                                    Wapt            = Wapt,
-                                    standardGPD = standardGPD
+        self.building = createBuilding( 
+                                incomingT_F     = incomingT_F,
+                                magnitudeStat   = magnitudeStat, 
+                                supplyT_F       = supplyT_F, 
+                                buildingType    = buildingType,
+                                loadshape       = loadshape,
+                                avgLoadshape    = avgLoadshape,
+                                returnT_F       = returnT_F, 
+                                flowRate        = flowRate,
+                                gpdpp           = gpdpp,
+                                nBR             = nBR,
+                                nApt            = nApt,
+                                Wapt            = Wapt,
+                                standardGPD     = standardGPD,
+                                annual          = annual,
+                                zipCode         = zipCode, 
+                                climateZone     = climateZone
         )
 
-        system = createSystem(  schematic, 
-                                building, 
+        self.system = createSystem(  
+                                schematic, 
                                 storageT_F, 
                                 defrostFactor, 
                                 percentUseable, 
                                 compRuntime_hr, 
-                                aquaFract, 
+                                aquaFract,
+                                building = self.building if PVol_G_atStorageT is None else None, 
                                 aquaFractLoadUp = aquaFractLoadUp,
                                 aquaFractShed = aquaFractShed,
                                 loadUpT_F = loadUpT_F,
                                 doLoadShift = doLoadShift, 
                                 loadShiftPercent = loadShiftPercent, 
                                 loadShiftSchedule = loadShiftSchedule, 
                                 loadUpHours = loadUpHours,
                                 safetyTM = safetyTM, 
                                 setpointTM_F = setpointTM_F, 
                                 TMonTemp_F = TMonTemp_F, 
-                                offTime_hr = offTime_hr
+                                offTime_hr = offTime_hr,
+                                PVol_G_atStorageT = PVol_G_atStorageT, 
+                                PCap_kBTUhr = PCap_kBTUhr, 
+                                TMVol_G = TMVol_G, 
+                                TMCap_kBTUhr = TMCap_kBTUhr,
+                                systemModel = systemModel
         )
- 
-        self.system = system
     
+    def getSimResult(self, initPV=None, initST=None, minuteIntervals = 1, nDays = 3, kWhCalc = False):
+        """
+        Returns the result of a simulation of a HPWH system in a building
+
+        Inputs
+        ------
+        initPV : float
+            Primary volume at start of the simulation
+        initST : float
+            Swing tank temperature at start of the simulation. Not used in this instance of the function
+        minuteIntervals : int
+            the number of minutes the duration each interval timestep for the simulation will be
+        nDays : int
+            the number of days the for duration of the entire simulation will be
+        hpwhModel : string
+            the real world HPWH model used in the simulation. Used to determina capacity and input power for varrious air temperaturess
+        """
+        simRun = simulate(self.system, self.building, initPV=initPV, initST=initST, minuteIntervals = minuteIntervals, nDays = nDays)
+        return simRun.returnSimResult(kWhCalc = kWhCalc)
+        # return self.system.simulate(self.building)
+
     def getSizingResults(self):
         """
         Returns the minimum primary volume and heating capacity sizing results
 
         Returns
         -------
         list
@@ -144,32 +177,33 @@
             
         heatHours : array
             Array of running hours per day corresponding to primaryHeatHrs2kBTUHR
             
         recIndex : int
             The index of the recommended heating rate. 
         """
-        return self.system.primaryCurve()
+        return self.system.primaryCurve(self.building)
     
-    def plotStorageLoadSim(self, return_as_div=True):
+    def plotStorageLoadSim(self, return_as_div=True, initPV=None, initST=None, minuteIntervals = 1, nDays = 3, kWhCalc = False):
         """
         Returns a plot of the of the simulation for the minimum sized primary
         system as a div or plotly figure. Can plot the minute level simulation
 
         Parameters
         ----------
         return_as_div
             A logical on the output, as a div (true) or as a figure (false)
 
         Returns
         -------
         div/fig
             plot_div
         """
-        return self.system.plotStorageLoadSim(return_as_div)
+        simRun = simulate(self.system, self.building, initPV=initPV, initST=initST, minuteIntervals = minuteIntervals, nDays = nDays)
+        return simRun.plotStorageLoadSim(return_as_div)
     
     def lsSizedPoints(self):
         """
         Returns combinations of storage and capacity based on number of 
         load up hours
 
         Returns 
@@ -177,19 +211,19 @@
         volN : array
             Array of storage volume for each number of load up hours.
         CapN : array
             Array of heating capacity for each number of load up hours.
         N : array
             Array of load up hours tested. Goes from 1 to hour before first shed.
         """
-        return self.system.lsSizedPoints()
+        return self.system.lsSizedPoints(self.building)
 
     def getHWMagnitude(self):
         """
         Returns the total daily hot water for the building the HPWH is being sized for.
         
         Returns
         -------
         magnitude : Float
             The total daily hot water for the building the HPWH is being sized for.
         """
-        return self.system.building.magnitude
+        return self.building.magnitude
```

### Comparing `ecoengine-0.0.6/src/ecoengine/engine/SystemCreator.py` & `ecoengine-0.0.7/src/ecoengine/engine/SystemCreator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from ecoengine.objects.SystemConfig import *
 from ecoengine.objects.systems.SwingTank import *
 from ecoengine.objects.systems.ParallelLoopTank import *
 
-def createSystem(schematic, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift = False, 
+def createSystem(schematic, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, building = None, doLoadShift = False, 
                  aquaFractLoadUp = None, aquaFractShed = None, loadUpT_F = None, loadShiftPercent = 1, loadShiftSchedule = None, loadUpHours = None, safetyTM = 1.75, 
-                 setpointTM_F = 135, TMonTemp_F = 120, offTime_hr = 0.333):
-
+                 setpointTM_F = 135, TMonTemp_F = 120, offTime_hr = 0.333, PVol_G_atStorageT = None, PCap_kBTUhr = None, TMVol_G = None, TMCap_kBTUhr = None,
+                 systemModel = None):
     """
     Initializes and sizes the HPWH system. Both primary and tempurature maintenance (for parrallel loop and swing tank) are set up in this function.
 
     Attributes
     ----------
     schematic : String
         Indicates schematic type. Valid values are 'swingtank', 'paralleltank', and 'primary'
-    building : Building
-        Building object the HPWH system will be sized for.
     storageT_F : float 
         The hot water storage temperature. [°F]
     defrostFactor : float 
         A multipier used to account for defrost in the final heating capacity. Default equals 1.
     percentUseable : float
         The fraction of the storage volume that can be filled with hot water.
     compRuntime_hr : float
         The number of hours the compressor will run on the design day. [Hr]
     aquaFract: float
         The fraction of the total height of the primary hot water tanks at which the Aquastat is located.
+    building : Building
+        Building object the HPWH system will be sized for.
     doLoadShift : boolean
         Set to true if doing loadshift
     aquaFractLoadUp : float
         The fraction of the total height of the primary hot water tanks at which the load up aquastat is located.
     aquaFractShed : float
         The fraction of the total height of the primary hot water tanks at which the shed aquastat is located.
     loadUpT_F : float
@@ -44,27 +44,38 @@
     setpointTM_F : float
         The setpoint of the temprature maintence tank. Defaults to 130 °F.
     TMonTemp_F : float
         The temperature where parallel loop tank will turn on.
         Defaults to 120 °F.
     offTime_hr: integer
         Maximum hours per day the temperature maintenance equipment can run.
+    PVol_G_atStorageT : float
+        For pre-sized systems, the total/maximum storage volume for water at storage temperature for the system in gallons
+    PCap_kBTUhr : float
+        For pre-sized systems, the output capacity for the system in kBTUhr
+    TMVol_G : float
+        For applicable pre-sized systems, the temperature maintenance volume for the system in gallons
+    TMCap_kBTUhr : float
+        For applicable pre-sized systems, the output capacity for temperature maintenance for the system in kBTUhr
 
     Raises
     ----------
     Exception: Error if schematic is not in list of valid schematic names.
 
     """
     
     match schematic:
         case 'swingtank':
-            return SwingTank(safetyTM, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                             doLoadShift, loadShiftPercent, loadShiftSchedule, loadUpHours, aquaFractLoadUp, aquaFractShed, loadUpT_F)        
+            return SwingTank(safetyTM, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, building,
+                doLoadShift, loadShiftPercent, loadShiftSchedule, loadUpHours, aquaFractLoadUp, aquaFractShed, loadUpT_F,
+                systemModel, PVol_G_atStorageT, PCap_kBTUhr, TMVol_G, TMCap_kBTUhr)        
         case 'paralleltank':
-            return ParallelLoopTank(safetyTM, setpointTM_F, TMonTemp_F, offTime_hr, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                 doLoadShift, loadShiftPercent, loadShiftSchedule, loadUpHours, aquaFractLoadUp, aquaFractShed, loadUpT_F)
+            return ParallelLoopTank(safetyTM, setpointTM_F, TMonTemp_F, offTime_hr, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
+                building, doLoadShift, loadShiftPercent, loadShiftSchedule, loadUpHours, aquaFractLoadUp, aquaFractShed, loadUpT_F,
+                systemModel, PVol_G_atStorageT, PCap_kBTUhr, TMVol_G, TMCap_kBTUhr)
         case 'primary':
-            return Primary(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent, loadShiftSchedule, loadUpHours,
-                           aquaFractLoadUp, aquaFractShed, loadUpT_F)
+            return Primary(storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, building, 
+                doLoadShift, loadShiftPercent, loadShiftSchedule, loadUpHours, aquaFractLoadUp, aquaFractShed, loadUpT_F,
+                systemModel, PVol_G_atStorageT, PCap_kBTUhr)
         case _:
             raise Exception("Unknown system schematic type.")
```

### Comparing `ecoengine-0.0.6/src/ecoengine/engine/__init__.py` & `ecoengine-0.0.7/src/ecoengine/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/objects/Building.py` & `ecoengine-0.0.7/src/ecoengine/objects/Building.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,111 +1,108 @@
 import os
 import json
 import numpy as np
+import csv
 
 from ecoengine.constants.Constants import *
 
 class Building:
-    def __init__(self, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         
-        self._checkParams(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
-
+        self._checkParams(incomingT_F, supplyT_F, returnT_F, flowRate)
+        
+        # Does not check loadshape as that is checked in buildingCreator
         self.loadshape = loadshape
         self.avgLoadshape = avgLoadshape
+        
         self.incomingT_F = incomingT_F
         self.supplyT_F = supplyT_F
         self.recirc_loss = (supplyT_F - returnT_F) * flowRate * rhoCp * 60. #BTU/HR
+        if(self.recirc_loss > RECIRC_LOSS_MAX_BTUHR):
+            raise Exception("Error: Recirculation losses may not exceed 108 kW, consider using multiple central plants.")
+        self.climateZone = climate
 
-    def _checkParams(self, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
-        if not isinstance(loadshape, np.ndarray) or len(loadshape) != 24:
-            raise Exception("Error: Loadshape must be a list of length 24.")
-        if sum(loadshape) > 1 + 1e-3 or sum(loadshape) < 1 - 1e-3:
-            raise Exception("Error:  Sum of the loadshape does not equal 1 but "+str(sum(loadshape))+".")
-        if any(x < 0 for x in loadshape):
-            raise Exception("Error:  Can not have negative load shape values in loadshape.")
-        if not isinstance(avgLoadshape, np.ndarray) or len(avgLoadshape) != 24:
-            raise Exception("Error: Average loadshape must be a list of length 24.")
-        if sum(avgLoadshape) > 1 + 1e-3 or sum(avgLoadshape) < 1 - 1e-3:
-            raise Exception("Error:  Sum of the average loadshape does not equal 1 but "+str(sum(loadshape))+".")
-        if any(x < 0 for x in avgLoadshape):
-            raise Exception("Error:  Can not have negative load shape values in average loadshape.")
+    def _checkParams(self, incomingT_F, supplyT_F, returnT_F, flowRate):
         if not (isinstance(supplyT_F, int) or isinstance(supplyT_F, float)):
             raise Exception("Error: Supply temp must be a number.")
         if not (isinstance(returnT_F, int) or isinstance(returnT_F, float)):
             raise Exception("Error: Return temp must be a number.")
         if supplyT_F <= returnT_F:
             raise Exception("Error: Supply temp must be higher than return temp.")
         if not (isinstance(incomingT_F, int) or isinstance(incomingT_F, float)):
             raise Exception("Error: City water temp must be a number.")
         if not (isinstance(flowRate, int) or isinstance(flowRate, float)):
             raise Exception("Error: Flow rate must be a number.")
         if not hasattr(self, 'magnitude'):
             raise Exception("Magnitude has not been set.")
+        
+    def setToAnnualLS(self):
+        raise Exception("Annual loadshape not available for this building type. This feature is only available for multi-family buildings.")
 
 class MensDorm(Building):
-    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         self.magnitude = n_students * 18.9 # ASHREA GPD per student
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
 
 class WomensDorm(Building):
-    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         self.magnitude = n_students * 16.4 # ASHREA GPD per student
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
 
 class Motel(Building):
-    def __init__(self, n_units, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, n_units, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         self.magnitude = n_units * 28.8 # ASHREA GPD per unit
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
 
 class NursingHome(Building):
-    def __init__(self, n_beds, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, n_beds, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         self.magnitude = n_beds * 20.1 # ASHREA GPD per bed
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
 
 class OfficeBuilding(Building):
-    def __init__(self, n_people, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, n_people, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         self.magnitude = n_people * 1.11 # ASHREA GPD per person
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
 
 class FoodServiceA(Building):
-    def __init__(self, n_meals, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, n_meals, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         self.magnitude = n_meals * 11.032 # ASHREA GPD per meal
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
 
 class FoodServiceB(Building):
-    def __init__(self, n_meals, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, n_meals, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         self.magnitude = n_meals * 6.288 # ASHREA GPD per meal
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
 
 class Apartment(Building):
-    def __init__(self, n_units, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, n_units, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         self.magnitude = n_units * 42.8 # ASHREA GPD per unit
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
 
 class ElementarySchool(Building):
-    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         self.magnitude = n_students * 1.081 # ASHREA GPD per student
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
 
 class JuniorHigh(Building):
-    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         self.magnitude = n_students * 3.27 # ASHREA GPD per student
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
 
 class SeniorHigh(Building):
-    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, n_students, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         self.magnitude = n_students * 3.02 # ASHREA GPD per student
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
     
 class MultiFamily(Building):
-    def __init__(self, n_people, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, gpdpp, nBR, nApt, Wapt, standardGPD):
+    def __init__(self, n_people, loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate, gpdpp, nBR, nApt, Wapt, standardGPD):
         # check inputs
-        if not (isinstance(nApt, int)):
+        if not nApt is None and not (isinstance(nApt, int)):
             raise Exception("Error: Number of apartments must be an integer.")
-        if not (isinstance(Wapt, int)):
+        if not Wapt is None and not (isinstance(Wapt, int)):
             raise Exception("Error: WATTs per apt must be an integer.")
         if standardGPD is None:
             if not (isinstance(gpdpp, int) or isinstance(gpdpp, float)):
                 raise Exception("Error: GPDPP must be a number.")
         else:
             if isinstance(standardGPD, str) and standardGPD in possibleStandardGPDs: # if the input here is a string get the appropriate standard gpdpp
                 with open(os.path.join(os.path.dirname(__file__), '../data/load_shapes/multi_family.json')) as json_file:
@@ -127,21 +124,30 @@
                     else:
                         gpdpp = dataDict['gpdpp'][standardGPD][0]
             else:
                 raise Exception("Error: standardGPD must be a String of one of the following values: " + str(possibleStandardGPDs))
             
         self.magnitude = gpdpp * n_people # gpdpp * number_of_people
 
-        super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
         # recalculate recirc_loss with different method if applicable
-        if(nApt > 0 and Wapt > 0):
+        if not nApt is None and not Wapt is None and (nApt > 0 and Wapt > 0):
+            # nApt * Wapt will overwrite recirc_loss so it doesn't matter what numbers we put in for returnT_F, flowRate
+            super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, 1, 1, climate)
             self.recirc_loss = nApt * Wapt * W_TO_BTUHR
+        else:
+            super().__init__(loadshape, avgLoadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
+
+    def setToAnnualLS(self):
+        with open(os.path.join(os.path.dirname(__file__), '../data/load_shapes/multi_family.json')) as json_file:
+            dataDict = json.load(json_file)
+            self.loadshape = dataDict['loadshapes']["Annual_Normalized"]
+            self.avgLoadshape = self.loadshape
 
 class MultiUse(Building):
-    def __init__(self, building_list, incomingT_F, supplyT_F, returnT_F, flowRate):
+    def __init__(self, building_list, incomingT_F, supplyT_F, returnT_F, flowRate, climate):
         # Generates building with loadshape that is combination of multiple loadshapes, one for each use section of the building. Each loadshape is multiplied
         # by the magnitude of that use section of the multi-use building, then all added together and divided by the total magnitude for the whole building
 
         total_magnitude = building_list[0].magnitude
         total_loadshape = [j * building_list[0].magnitude for j in building_list[0].loadshape]
         total_avg_loadshape = [j * building_list[0].magnitude for j in building_list[0].avgLoadshape]
 
@@ -155,8 +161,8 @@
         total_loadshape = [j / total_magnitude for j in total_loadshape]
         total_avg_loadshape = [j / total_magnitude for j in total_avg_loadshape]
         total_loadshape = np.array(total_loadshape)
         total_avg_loadshape = np.array(total_avg_loadshape)
 
         self.magnitude = total_magnitude
 
-        super().__init__(total_loadshape, total_avg_loadshape, incomingT_F, supplyT_F, returnT_F, flowRate)
+        super().__init__(total_loadshape, total_avg_loadshape, incomingT_F, supplyT_F, returnT_F, flowRate, climate)
```

### Comparing `ecoengine-0.0.6/src/ecoengine/objects/SystemConfig.py` & `ecoengine-0.0.7/src/ecoengine/objects/SystemConfig.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,204 +1,214 @@
 from ecoengine.constants.Constants import *
 from .Building import Building
+from .SimulationRun import SimulationRun
+from .PrefMapTracker import PrefMapTracker
 import numpy as np
 from scipy.stats import norm #lognorm
-from plotly.graph_objs import Figure, Scatter
-from plotly.offline import plot
-from .systemConfigUtils import roundList, mixVolume, hrToMinList, getPeakIndices, checkLiqudWater, checkHeatHours
+from .systemConfigUtils import mixVolume, hrToMinList, hrTo15MinList, getPeakIndices, checkLiqudWater, checkHeatHours
 
 class SystemConfig:
-    def __init__(self, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
+    def __init__(self, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, building = None,
                  doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None, loadUpHours = None, aquaFractLoadUp = None, 
-                 aquaFractShed = None, loadUpT_F = None):
+                 aquaFractShed = None, loadUpT_F = None, systemModel = None, PVol_G_atStorageT = None, PCap_kBTUhr = None):
         # check inputs. Schedule not checked because it is checked elsewhere
-        self._checkInputs(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent)
+        self._checkInputs(storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent)
         self.doLoadShift = doLoadShift
-        self.building = building        
         self.storageT_F = storageT_F
         self.defrostFactor = defrostFactor
         self.percentUseable = percentUseable
         self.compRuntime_hr = compRuntime_hr
         self.aquaFract = aquaFract
         self.loadUpHours = None
+        # self.perfMap = None
 
         if doLoadShift and not loadShiftSchedule is None:
             self._setLoadShift(loadShiftSchedule, loadUpHours, aquaFract, aquaFractLoadUp, aquaFractShed, storageT_F, loadUpT_F, loadShiftPercent)
         
         else:
             self.loadShiftSchedule = [1] * 24
             self.fract_total_vol = 1 # fraction of total volume for for load shifting, or 1 if no load shifting
 
         #Check if need to increase sizing to meet lower runtimes for load shift
         self.maxDayRun_hr = min(self.compRuntime_hr, sum(self.loadShiftSchedule))
 
         #size system
-        self.PVol_G_atStorageT, self.effSwingFract = self.sizePrimaryTankVolume(self.maxDayRun_hr, self.loadUpHours)
-        self.PCap_kBTUhr = self._primaryHeatHrs2kBTUHR(heathours = self.maxDayRun_hr, loadUpHours = self.loadUpHours, effSwingVolFract = self.effSwingFract, primaryCurve = False)[0]
+        if not PVol_G_atStorageT is None:
+            if not (isinstance(PVol_G_atStorageT, int) or isinstance(PVol_G_atStorageT, float)) or PVol_G_atStorageT <= 0: 
+                raise Exception('Invalid input given for Primary Storage Volume, it must be a number greater than zero.')
+            if not (isinstance(PCap_kBTUhr, int) or isinstance(PCap_kBTUhr, float)) or PCap_kBTUhr <= 0: 
+                raise Exception('Invalid input given for Primary Output Capacity, it must be a number greater than zero.')
+            self.PVol_G_atStorageT = PVol_G_atStorageT
+            self.PCap_kBTUhr = PCap_kBTUhr
+        else: 
+            #size system based off of building
+            if not isinstance(building, Building):
+                raise Exception("Error: Building is not valid.")
+            self.PVol_G_atStorageT, self.effSwingFract = self.sizePrimaryTankVolume(self.maxDayRun_hr, self.loadUpHours, building)
+            self.PCap_kBTUhr = self._primaryHeatHrs2kBTUHR(self.maxDayRun_hr, self.loadUpHours, building, 
+                effSwingVolFract = self.effSwingFract, primaryCurve = False)[0]
+            
+        self.perfMap = PrefMapTracker(self.PCap_kBTUhr, modelName = systemModel, kBTUhr = True)
 
-    def _checkInputs(self, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent):
-        if not isinstance(building, Building):
-            raise Exception("Error: Building is not valid.")
+    def _checkInputs(self, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, doLoadShift, loadShiftPercent):
         if not (isinstance(storageT_F, int) or isinstance(storageT_F, float)) or not checkLiqudWater(storageT_F): 
             raise Exception('Invalid input given for Storage temp, it must be between 32 and 212F.')
         if not (isinstance(defrostFactor, int) or isinstance(defrostFactor, float)) or defrostFactor < 0 or defrostFactor > 1:
             raise Exception("Invalid input given for Defrost Factor, must be a number between 0 and 1.")
         if not (isinstance(percentUseable, int) or isinstance(percentUseable, float)) or percentUseable > 1 or percentUseable < 0:
             raise Exception("Invalid input given for percentUseable, must be a number between 0 and 1.")
         if not isinstance(compRuntime_hr, int) or compRuntime_hr <= 0 or compRuntime_hr > 24:
             raise Exception("Invalid input given for compRuntime_hr, must be an integer between 0 and 24.")
         if not (isinstance(aquaFract, int) or isinstance(aquaFract, float)) or aquaFract > 1 or aquaFract <= 0:
             raise Exception("Invalid input given for aquaFract must, be a number between 0 and 1.")
-        if not (isinstance(loadShiftPercent, int) or isinstance(loadShiftPercent, float)) or loadShiftPercent > 1 or loadShiftPercent < 0:
-            raise Exception("Invalid input given for loadShiftPercent, must be a number between 0 and 1.")
         if not isinstance(doLoadShift, bool):
             raise Exception("Invalid input given for doLoadShift, must be a boolean.")
-              
+        if doLoadShift and (not (isinstance(loadShiftPercent, int) or isinstance(loadShiftPercent, float)) or loadShiftPercent > 1 or loadShiftPercent < 0):
+            raise Exception("Invalid input given for loadShiftPercent, must be a number between 0 and 1.")
+
+    def setCapacity(self, PCap_kBTUhr = None, oat = None, incomingWater_T = None):
+        if not PCap_kBTUhr is None:
+            self.PCap_kBTUhr = PCap_kBTUhr
+        elif not (oat is None or incomingWater_T is None or self.perfMap is None):
+            self.PCap_kBTUhr = self.perfMap.getCapacity(oat, incomingWater_T, self.storageT_F)
+        else:
+           raise Exception("No capacity given or preformance map has not been set.") 
+
+    def getCapacity(self, kW = False):
+        if kW:
+            return self.PCap_kBTUhr/W_TO_BTUHR
+        return self.PCap_kBTUhr
+
     def getSizingResults(self):
         """
         Returns the minimum primary volume and heating capacity sizing results. Implimented seperatly in Temp Maintenence systems.
 
         Returns
         -------
         list
             self.PVol_G_atStorageT, self.PCap_kBTUhr
         """
         return [self.PVol_G_atStorageT, self.PCap_kBTUhr]
-
-    def simulate(self, initPV=None, initST=None, Pcapacity=None, Pvolume=None):
-        """
-        Implimented seperatly for Swink Tank systems 
-        Inputs
-        ------
-        initPV : float
-            Primary volume at start of the simulation
-        initST : float
-            Primary Swing tank at start of the simulation. Not used in this instance of the function
-        Pcapacity : float
-            The primary heating capacity in kBTUhr to use for the simulation,
-            default is the sized system
-        Pvolume : float
-            The primary storage volume in gallons to  to use for the simulation,
-            default is the sized system
-        
-        Returns
-        -------
-        list [ pV, G_hw, D_hw, prun ]
-        pV : list 
-            Volume of HW in the tank with time at the strorage temperature.
-        G_hw : list 
-            The generation of HW with time at the supply temperature
-        D_hw : list 
-            The hot water demand with time at the tsupply temperature
-        prun : list 
-            The actual output in gallons of the HPWH with time
-        """
-
-        G_hw, D_hw, V0, Vtrig, pV, pheating = self._getInitialSimulationValues(Pcapacity, Pvolume)
-       
-        hw_outSwing = [0] * (len(G_hw))
-        hw_outSwing[0] = D_hw[0]
-        prun = [0] * (len(G_hw))
-
-        if initPV:
-            pV[0] = initPV
-
-        #get mixed storage temp
-        mixedStorT_F = self._mixStorageTemps(pV[0])[0]
-
-        # Run the "simulation"
-        for i in range(1, len(G_hw)):
-            mixedDHW = mixVolume(D_hw[i], mixedStorT_F, self.building.incomingT_F, self.building.supplyT_F) 
-            mixedGHW = mixVolume(G_hw[i], mixedStorT_F, self.building.incomingT_F, self.building.supplyT_F)
-            pheating, pV[i], prun[i] = self.runOnePrimaryStep(pheating, V0, Vtrig[i], pV[i-1], mixedDHW, mixedGHW) 
-            
-        return [roundList(pV, 3),
-                roundList(G_hw, 3),
-                roundList(D_hw, 3),
-                roundList(prun, 3)]
-
-    def _getInitialSimulationValues(self, Pcapacity=None, Pvolume=None):
+    
+    def getInitializedSimulation(self, building : Building, initPV=None, initST=None, minuteIntervals = 1, nDays = 3):
         """
-        Returns initialized arrays needed for 3-day simulation
+        Returns initialized arrays needed for nDay simulation
 
         Parameters
         ----------
-        Pcapacity : float
-            The primary heating capacity in kBTUhr to use for the simulation,
-            default is the sized system
-        Pvolume : float
-            The primary storage volume in gallons to  to use for the simulation,
-            default is the sized system
+        building : Building
+            The building for the simulation
+        initPV : float
+            the initial primary tank volume at the start of the simulation
+        initST : float
+        minuteIntervals : int
+            the number of minutes per time interval for the simulation
+        nDays : int
+            the number of days that will be simulated 
 
         Returns
         -------
-        list [ G_hw, D_hw, V0, V, run, pheating ]
-        G_hw : list
+        list [ hwGenRate, hwDemand, V0, V, run, pheating ]
+        hwGenRate : list
             The generation of HW with time at the supply temperature
-        D_hw : list
+        hwDemand : list
             The hot water demand with time at the tsupply temperature
         V0 : float
             The storage volume of the primary system at the storage temperature
         Vtrig : list
             The remaining volume of the primary storage volume when heating is
             triggered, note this equals V0*(1 - aquaFract[i]) 
         pV : list 
             Volume of HW in the tank with time at the storage temperature. Initialized to array of 0s with pV[0] set to V0
         pheating : boolean 
             set to false. Simulation starts with a full tank so primary heating starts off
+        pGen : list 
+            The actual output in gallons of the HPWH with time
         """
-        if not Pcapacity:
-            Pcapacity =  self.PCap_kBTUhr
-
-        if not Pvolume:
-            Pvolume =  self.PVol_G_atStorageT
         
-        loadShapeN = self.building.loadshape
-        if self.doLoadShift:
-            loadShapeN = self.building.avgLoadshape
+        loadShapeN = building.loadshape
+        if self.doLoadShift and nDays < 365: #Only for non-annual simulations
+            loadShapeN = building.avgLoadshape
         
         # Get the generation rate from the primary capacity
-        G_hw = 1000 * Pcapacity / rhoCp / (self.building.supplyT_F - self.building.incomingT_F) \
-               * self.defrostFactor * np.tile(self.loadShiftSchedule, 3)
-
+        hwGenRate = 1000 * self.PCap_kBTUhr / rhoCp / (building.supplyT_F - building.incomingT_F) \
+               * self.defrostFactor
+        loadshiftSched = np.tile(self.loadShiftSchedule, nDays) # TODO can we get rid of it?
         
         # Define the use of DHW with the normalized load shape
-        D_hw = self.building.magnitude * self.fract_total_vol * np.tile(loadShapeN, 3)
+        hwDemand = building.magnitude * loadShapeN
+        if (len(hwDemand) == 24):
+            hwDemand = np.tile(hwDemand, nDays)
+        if nDays < 365:
+            hwDemand = hwDemand * self.fract_total_vol
+        elif nDays == 365:
+            hwDemand = hwDemand
+        else:
+            raise Exception("Invalid input given for number of days. Must be <= 365.")
 
         # Init the "simulation"
-        V0 = np.ceil(Pvolume * self.percentUseable) 
+        V0 = np.ceil(self.PVol_G_atStorageT * self.percentUseable)
         
-        Vtrig = np.tile(np.ceil(Pvolume * (1 - self.aquaFract)) + 1, 24) # To prevent negatives with any of that rounding math. TODO Nolan and I don't think we need this mysterious + 1
+        Vtrig = np.tile(np.ceil(self.PVol_G_atStorageT * (1 - self.aquaFract)) + 1, 24) # To prevent negatives with any of that rounding math. TODO Nolan and I don't think we need this mysterious + 1
         
         if self.doLoadShift:
             
-            Vtrig = [Pvolume * (1 - self.aquaFractShed) if x == 0 else Pvolume * (1 - self.aquaFract) for x in self.loadShiftSchedule]
+            Vtrig = [self.PVol_G_atStorageT * (1 - self.aquaFractShed) if x == 0 else self.PVol_G_atStorageT * (1 - self.aquaFract) for x in self.loadShiftSchedule]
             
             #set load up hours pre-shed 1
             shedHours = [i for i in range(len(self.loadShiftSchedule)) if self.loadShiftSchedule[i] == 0] 
-            Vtrig = [Pvolume * (1 - self.aquaFractLoadUp) if shedHours[0] - self.loadUpHours <= i <= shedHours[0] - 1 else Vtrig[i] for i, x in enumerate(Vtrig)]
+            Vtrig = [self.PVol_G_atStorageT * (1 - self.aquaFractLoadUp) if shedHours[0] - self.loadUpHours <= i <= shedHours[0] - 1 else Vtrig[i] for i, x in enumerate(Vtrig)]
             
             #check if there are two sheds, if so set all hours inbetween to load up
             try:
                 secondShed = [[shedHours[i-1], shedHours[i]] for i in range(1, len(shedHours)) if shedHours[i] - shedHours[i-1] > 1][0]
-                Vtrig = [Pvolume * (1 - self.aquaFractLoadUp) if secondShed[0] <= i <= secondShed[1] - 1 else Vtrig[i] for i, x in enumerate(Vtrig)]
+                Vtrig = [self.PVol_G_atStorageT * (1 - self.aquaFractLoadUp) if secondShed[0] <= i <= secondShed[1] - 1 else Vtrig[i] for i, x in enumerate(Vtrig)]
             
             except IndexError:
                 pass
         
-        # To per minute from per hour
-        G_hw = np.array(hrToMinList(G_hw)) / 60
-        D_hw = np.array(hrToMinList(D_hw)) / 60
-        Vtrig = np.array(hrToMinList(np.tile(Vtrig, 3))) 
+        if minuteIntervals == 1:
+            # To per minute from per hour
+            hwGenRate = hwGenRate / 60
+            hwDemand = np.array(hrToMinList(hwDemand)) / 60
+            Vtrig = np.array(hrToMinList(np.tile(Vtrig, nDays))) 
+            loadshiftSched = np.array(hrToMinList(loadshiftSched))
+        elif minuteIntervals == 15:
+            # To per 15 minute from per hour
+            hwGenRate = hwGenRate / 4
+            hwDemand = np.array(hrTo15MinList(hwDemand)) / 4
+            Vtrig = np.array(hrTo15MinList(np.tile(Vtrig, nDays)))
+            loadshiftSched = np.array(hrTo15MinList(loadshiftSched))
+        elif minuteIntervals == 60:
+            Vtrig = np.array(np.tile(Vtrig, nDays))
+        else:
+            raise Exception("Invalid input given for granularity. Must be 1, 15, or 60.")
 
-        pV = [V0] + [0] * (len(G_hw) - 1)
+        pV = [0] * (len(hwDemand) - 1) + [V0]
 
         pheating = False
+
+        pGen = [0] * len(hwDemand)
+        pRun = [0] * len(hwDemand)
+
+        mixedStorT_F = self.mixStorageTemps(V0, building.incomingT_F, building.supplyT_F)[0]
+        if initPV:
+            pV[-1] = initPV
+
+        return SimulationRun(hwGenRate, hwDemand, V0, Vtrig, pV, pGen, pRun, pheating, mixedStorT_F, building, loadshiftSched, minuteIntervals, self.doLoadShift)
     
-        return G_hw, D_hw, V0, Vtrig, pV, pheating
+    def runOneSystemStep(self, simRun : SimulationRun, i, minuteIntervals = 1, oat = None):
+        incomingWater_T = simRun.getIncomingWaterT(i)
+        if not (oat is None or self.perfMap is None):
+            # set primary system capacity based on outdoor ait temp and incoming water temp 
+            self.PCap_kBTUhr = self.perfMap.getCapacity(oat, incomingWater_T, self.storageT_F)
+        mixedDHW = mixVolume(simRun.hwDemand[i], simRun.mixedStorT_F, incomingWater_T, simRun.building.supplyT_F) 
+        mixedGHW = mixVolume(simRun.hwGenRate, simRun.mixedStorT_F, incomingWater_T, simRun.building.supplyT_F)
+        simRun.pheating, simRun.pV[i], simRun.pGen[i], simRun.pRun[i] = self.runOnePrimaryStep(simRun.pheating, simRun.V0, simRun.Vtrig[i], simRun.pV[i-1], mixedDHW, mixedGHW, simRun.Vtrig[i-1],
+                                                                                               minuteIntervals = minuteIntervals) 
     
     def _setLoadShift(self, loadShiftSchedule, loadUpHours, aquaFract, aquaFractLoadUp, aquaFractShed, storageT_F, loadUpT_F, loadShiftPercent=1):
         """
         Sets the load shifting schedule from input loadShiftSchedule
 
         Parameters
         ----------
@@ -256,67 +266,78 @@
         else:
             # calculate fraction total hot water required to meet load shift days
             fract = norm_mean + norm_std * norm.ppf(loadShiftPercent) #TODO norm_mean and std are currently from multi-family, need other types eventually. For now, loadshifting will only be available for multi-family
             self.fract_total_vol = fract if fract <= 1. else 1.
         
         self.doLoadShift = True
 
-    def _primaryHeatHrs2kBTUHR(self, heathours, loadUpHours, primaryCurve = False, effSwingVolFract=1):
+    def _primaryHeatHrs2kBTUHR(self, heathours, loadUpHours, building, primaryCurve = False, effSwingVolFract=1):
         """
         Converts from hours of heating in a day to heating capacity. If loadshifting compares this method to capacity needed to load up
         and takes maximum.
 
         Implimented seperatly in Swing Tank systems
 
         Parameters
         ----------
         heathours : float or numpy.ndarray
             The number of hours primary heating equipment can run.
-
+        loadUpHours : float
+            Number of hours spent loading up for first shed.
+        building : Building
+            The building the system being sized for
+        primaryCurve : Bool
+            Indicates that function is being called to generate the priamry
+            sizing curve. This overrides LS sizing and sizes with "normal"
+            sizing (default = False)
         effSwingVolFract : float or numpy.ndarray
             The fractional adjustment to the total hot water load for the
             primary system. Only used in a swing tank system.
 
         Returns
         -------
         heatCap
             The heating capacity in [btu/hr].
         genRate
             The generation rate in [gal/hr] when the heat pump is on. 
             If loadshifting this is the maximum between normal calculation
             and what is necessary to complete first load up.
         """
         checkHeatHours(heathours)
-        genRate = self.building.magnitude * effSwingVolFract / heathours
+        genRate = building.magnitude * effSwingVolFract / heathours
         
         if self.doLoadShift and not primaryCurve:
-            Vshift, VconsumedLU = self._calcPrelimVol(loadUpHours) 
+            Vshift, VconsumedLU = self._calcPrelimVol(loadUpHours, building.avgLoadshape, building) 
             Vload = Vshift * (self.aquaFract - self.aquaFractLoadUp) / (self.aquaFractShed - self.aquaFractLoadUp) #volume in 'load up' portion of tank
             LUgenRate = (Vload + VconsumedLU) / loadUpHours #rate needed to load up tank and offset use during load up period
             
             #compare with original genRate
             genRate = max(LUgenRate, genRate)
             
         heatCap = genRate * rhoCp * \
-            (self.building.supplyT_F - self.building.incomingT_F) / self.defrostFactor / 1000
+            (building.supplyT_F - building.incomingT_F) / self.defrostFactor / 1000
        
         return heatCap, genRate
     
 
-    def sizePrimaryTankVolume(self, heatHrs, loadUpHours, primaryCurve = False):
+    def sizePrimaryTankVolume(self, heatHrs, loadUpHours, building, primaryCurve = False):
         """
         Calculates the primary storage using the Ecotope sizing methodology. Function is also used
         to generate primary sizing curve, which creates a curve with no load shifting and points
         with varying numbers of load up hours.
 
         Parameters
         ----------
         heatHrs : float
             The number of hours primary heating equipment can run in a day.
-        primaryCurve : 
+        loadUpHours : float
+            Number of hours spent loading up for first shed.
+        building : Building
+            the building object the primary tank is being sized for.
+        primaryCurve : Bool
             Indicates that function is being called to generate the priamry
             sizing curve. This overrides LS sizing and sizes with "normal"
             sizing (default = False)
         
         Raises
         ------
         ValueError: aquastat fraction is too low.
@@ -335,58 +356,58 @@
 
         if heatHrs <= 0 or heatHrs > 24:
             raise Exception("Heat hours is not within 1 - 24 hours")
         # Fraction used for adjusting swing tank volume.
         effMixFract = 1.
 
         # Running vol
-        runningVol_G, effMixFract = self._calcRunningVol(heatHrs, np.ones(24), self.building.loadshape, effMixFract)
-        totalVolAtStorage = self._getTotalVolAtStorage(runningVol_G)
+        runningVol_G, effMixFract = self._calcRunningVol(heatHrs, np.ones(24), building.loadshape, building, effMixFract)
+        totalVolAtStorage = self._getTotalVolAtStorage(runningVol_G, building.incomingT_F, building.supplyT_F)
         totalVolAtStorage *=  thermalStorageSF
 
         if self.doLoadShift and not primaryCurve:
-            LSrunningVol_G, LSeffMixFract = self._calcRunningVolLS(loadUpHours, effMixFract)
+            LSrunningVol_G, LSeffMixFract = self._calcRunningVolLS(loadUpHours, building.avgLoadshape, building, effMixFract)
             LSrunningVol_G *= self.fract_total_vol 
 
             # Get total volume from max of primary method or load shift method
             if LSrunningVol_G > runningVol_G:
                 runningVol_G = LSrunningVol_G
                 effMixFract = LSeffMixFract
                 
                 #get the average tank volume
-                totalVolAtStorage = self._mixStorageTemps(runningVol_G)[1]
+                totalVolAtStorage = self.mixStorageTemps(runningVol_G, building.incomingT_F, building.supplyT_F)[1]
                 
                 #multiply computed storage by efficiency safety factor (currently set to 1)
                 totalVolAtStorage *=  thermalStorageSF 
         
             # Check the Cycling Volume 
             LUcyclingVol_G = totalVolAtStorage * (self.aquaFractLoadUp - (1 - self.percentUseable))
-            minRunVol_G = pCompMinimumRunTime * (self.building.magnitude / heatHrs) # (generation rate - no usage) #REMOVED EFFMIXFRACT
+            minRunVol_G = pCompMinimumRunTime * (building.magnitude / heatHrs) # (generation rate - no usage) #REMOVED EFFMIXFRACT
             
             if minRunVol_G > LUcyclingVol_G:
                 min_AF = minRunVol_G / totalVolAtStorage + (1 - self.percentUseable)
                 if min_AF < 1:
-                    raise ValueError("01", "The load up aquastat fraction is too low in the storge system recommend increasing the maximum run hours in the day or increasing to a minimum of: ", round(min_AF,3))
-                raise ValueError("02", "The minimum aquastat fraction is greater than 1. This is due to the storage efficency and/or the maximum run hours in the day may be too low. Try increasing these values, we reccomend 0.8 and 16 hours for these variables respectively." )
+                    raise Exception("The load up aquastat fraction is too low in the storge system recommend increasing the maximum run hours in the day or increasing to a minimum of: " + str(round(min_AF,3)))
+                raise Exception("The minimum load up aquastat fraction is greater than 1. This is due to the storage efficency and/or the maximum run hours in the day may be too low. Try increasing these values, we reccomend 0.8 and 16 hours for these variables respectively." )
 
         cyclingVol_G = totalVolAtStorage * (self.aquaFract - (1 - self.percentUseable))
-        minRunVol_G = pCompMinimumRunTime * (self.building.magnitude / heatHrs) # (generation rate - no usage)  #REMOVED EFFMIXFRACT
+        minRunVol_G = pCompMinimumRunTime * (building.magnitude / heatHrs) # (generation rate - no usage)  #REMOVED EFFMIXFRACT
 
         if minRunVol_G > cyclingVol_G:
             min_AF = minRunVol_G / totalVolAtStorage + (1 - self.percentUseable)
             if min_AF < 1:
                 raise ValueError("01", "The aquastat fraction is too low in the storge system recommend increasing the maximum run hours in the day or increasing to a minimum of: ", round(min_AF,3))
             raise ValueError("02", "The minimum aquastat fraction is greater than 1. This is due to the storage efficency and/or the maximum run hours in the day may be too low. Try increasing these values, we reccomend 0.8 and 16 hours for these variables respectively." )
 
         
         # Return the temperature adjusted total volume ########################
         
         return totalVolAtStorage, effMixFract
     
-    def _calcRunningVol(self, heatHrs, onOffArr, loadshape, effMixFract = 0):
+    def _calcRunningVol(self, heatHrs, onOffArr, loadshape, building, effMixFract = 0):
         """
         Function to find the running volume for the hot water storage tank, which
         is needed for calculating the total volume for primary sizing and in the event of load shift sizing
         represents the entire volume.
 
         Implimented seperatly for Swing Tank systems
 
@@ -394,14 +415,16 @@
         ----------
         heatHrs : float
             The number of hours primary heating equipment can run in a day.
         onOffArr : ndarray
             array of 1/0's where 1's allow heat pump to run and 0's dissallow. of length 24.
         loadshape : ndarray
             normalized array of length 24 representing the daily loadshape for this calculation.
+        building : Building
+            The building the system is being sized for
         effMixFract: Int
             unused value in this instance of the function. Used in Swing Tank implimentation
 
         Raises
         ------
         Exception: Error if oversizing system.
 
@@ -411,92 +434,101 @@
             The running volume in gallons at supply temp.
         effMixFract: int
             Needed for swing tank implementation.
         """          
         genRate = np.tile(onOffArr,2) / heatHrs #hourly
         diffN = genRate - np.tile(loadshape,2) #hourly
         diffInd = getPeakIndices(diffN[0:24]) #Days repeat so just get first day!
-        diffN *= self.building.magnitude
+        diffN *= building.magnitude
         
         # Get the running volume ##############################################
         if len(diffInd) == 0:
-            #TODO but what if it is undersized? Also can this ever be hit? users currently do not have power to change num hours from interface
             raise Exception("ERROR ID 03","The heating rate is greater than the peak volume the system is oversized! Try increasing the hours the heat pump runs in a day",)
         runV_G = 0
         for peakInd in diffInd:
             #Get the rest of the day from the start of the peak
             diffCum = np.cumsum(diffN[peakInd:])  #hourly
             runV_G = max(runV_G, -min(diffCum[diffCum<0.])) #Minimum value less than 0 or 0.
         return runV_G, effMixFract
     
-    def _calcRunningVolLS(self, loadUpHours, effMixFract = 1):
+    def _calcRunningVolLS(self, loadUpHours, loadshape, building, effMixFract = 1):
         """
         Function to calculate the running volume if load shifting. Using the max generation rate between normal sizing
         and preliminary volume, the deficit between generation and hot water use is then added to the preliminary volume.
 
         Implemented separately for swing tank system.
 
         Parameters
         ------   
         loadUpHours : float
             Number of hours of scheduled load up before first shed. If sizing, this is set by user. If creating sizing
-            plot, number may vary.   
+            plot, number may vary.  
+        loadshape : ndarray
+            normalized array of length 24 representing the daily loadshape for this calculation.
+        building : Building
+            The building the system is being sized for
         effMixFract : float
             Only used in swing tank implementation.
 
         Returns
         ------
         LSrunV_G : float
             Volume needed between primary shed aquastat and load up aquastat at supply temp.
         effMixFract : float
             Used for swing tank implementation.
         """
-        Vshift = self._calcPrelimVol(loadUpHours)[0] #volume to make it through first shed
+        Vshift = self._calcPrelimVol(loadUpHours, loadshape, building)[0] #volume to make it through first shed
         
-        genRateON = self._primaryHeatHrs2kBTUHR(self.maxDayRun_hr, loadUpHours, effSwingVolFract = effMixFract, primaryCurve = False)[1] #max generation rate from both methods
+        genRateON = self._primaryHeatHrs2kBTUHR(self.maxDayRun_hr, loadUpHours, building, effSwingVolFract = effMixFract, primaryCurve = False)[1] #max generation rate from both methods
         genRate = [genRateON if x != 0 else 0 for x in self.loadShiftSchedule] #set generation rate during shed to 0
         
-        diffN = np.tile(genRate, 2) - np.tile(self.building.avgLoadshape,2) * self.building.magnitude
+        diffN = np.tile(genRate, 2) - np.tile(loadshape,2) * building.magnitude
         
         #get first index after shed
         shedEnd = [i for i,x in enumerate(genRate[1:],1) if x > genRate[i-1]][0] #start at beginning of first shed, fully loaded up equivalent to starting at the end of shed completely "empty"
         diffCum = np.cumsum(diffN[shedEnd:]) 
         LSrunV_G = -min(diffCum[diffCum<0.], default = 0) #numbers less than 0 are a hot water deficit, find the biggest deficit. if no deficit then 0.
         
         #add running volume to preliminary shifted volume
         LSrunV_G += Vshift
         
         return LSrunV_G, effMixFract 
 
-    def _getTotalVolAtStorage(self, runningVol_G):
+    def _getTotalVolAtStorage(self, runningVol_G, incomingT_F, supplyT_F):
         """
         Calculates the maximum primary storage using the Ecotope sizing methodology. Swing Tanks implement sperately.
 
         Parameters
         ----------
         runningVol_G : float
             The running volume in gallons
-        avgStorageT_F : float
-            Average storage temperature. If not load shifting this is the storage temp. If load shifting this is the 
-            average between load up and normal setpoint based on aquastat locations.
+        incomingT_F : float
+            Incoming temp (in Fahrenhiet) of city water
+        supplyT_F : float
+            Supply temp (in Fahrenhiet) of water distributed to those in the building
 
         Returns
         -------
         totalVolMax : float
             The total storage volume in gallons adjusted to the storage tempreature.
         
         """
         
-        return mixVolume(runningVol_G, self.storageT_F, self.building.incomingT_F, self.building.supplyT_F) / (1 - self.aquaFract)
+        return mixVolume(runningVol_G, self.storageT_F, incomingT_F, supplyT_F) / (1 - self.aquaFract)
     
-    def primaryCurve(self):
+    def primaryCurve(self, building):
         """
         Sizes the primary system curve. Will catch the point at which the aquatstat
         fraction is too small for system and cuts the return arrays to match cutoff point.
 
+        Parameters
+        ----------
+        building : Building
+            the building this primary system curve is being sized for
+
         Returns
         -------
         volN : array
             Array of volume in the tank at each hour.
 
         primaryHeatHrs2kBTUHR : array
             Array of heating capacity in kBTU/hr
@@ -505,221 +537,189 @@
             Array of running hours per day corresponding to primaryHeatHrs2kBTUHR
             
         recIndex : int
             The index of the recommended heating rate. 
         """
         # Define the heating hours we'll check
         delta = -0.25
-        maxHeatHours = 1/(max(self.building.loadshape))*1.001   
+        maxHeatHours = 1/(max(building.loadshape))*1.001   
         arr1 = np.arange(24, self.maxDayRun_hr, delta) #TODO why are we going all the way to 24 hours ???
         recIndex = len(arr1)
         heatHours = np.concatenate((arr1, np.arange(self.maxDayRun_hr, maxHeatHours, delta)))
         
         volN = np.zeros(len(heatHours))
         effMixFract = np.ones(len(heatHours))
         for i in range(0,len(heatHours)):
             try:
-                volN[i], effMixFract[i] = self.sizePrimaryTankVolume(heatHours[i], self.loadUpHours, primaryCurve = True)
+                volN[i], effMixFract[i] = self.sizePrimaryTankVolume(heatHours[i], self.loadUpHours, building, primaryCurve = True)
                 
             except ValueError:
                 break
         # Cut to the point the aquastat fraction was too small
         volN        = volN[:i]
         heatHours   = heatHours[:i]
         effMixFract = effMixFract[:i]
 
-        return [volN, self._primaryHeatHrs2kBTUHR(heatHours, self.loadUpHours, effSwingVolFract = effMixFract, primaryCurve = True)[0], heatHours, recIndex]
+        return [volN, self._primaryHeatHrs2kBTUHR(heatHours, self.loadUpHours, building, 
+            effSwingVolFract = effMixFract, primaryCurve = True)[0], heatHours, recIndex]
 
-    def lsSizedPoints(self):
+    def lsSizedPoints(self, building):
         """
         Creates points for sizing curve plot based on number of hours in first load up period. If "regular" sizing 
         drives algorithmn, regular sizing will be used. This prevents user from oversizing system by putting 
         ill-informed number of load up hours.
 
+        Parameters
+        ----------
+        building : Building
+            The building the system being sized for
+
         Returns
         lsSizingCombos : array
             Array of volume and capacity combinations sized based on the number of load up hours.
         """
         
         volN = np.zeros(5)
         capN = np.zeros(5)
         effMixN = np.zeros(5)
         N = np.zeros(5)
 
         #load up hours to loop through
         for i in range(1, 6): #arbitrary stopping point, anything more than this will not result in different sizing
             #size the primary system based on the number of load up hours
             volN[i-1], effMixN[i-1] = self.sizePrimaryTankVolume(heatHrs = self.maxDayRun_hr, loadUpHours = i, primaryCurve = False)
-            capN[i-1] = self._primaryHeatHrs2kBTUHR(heathours = self.maxDayRun_hr, loadUpHours = i, effSwingVolFract = effMixN[i-1], primaryCurve = False)[0]
+            capN[i-1] = self._primaryHeatHrs2kBTUHR(self.maxDayRun_hr, i, building, effSwingVolFract = effMixN[i-1], primaryCurve = False)[0]
             N[i-1] = i
 
         volN, capN = zip(*set(zip(volN, capN)))
         N = N[:len(volN)]
     
         return [volN, capN, N]
 
     
-    def runOnePrimaryStep(self, pheating, V0, Vtrig, Vcurr, hw_out, hw_in):
+    def runOnePrimaryStep(self, pheating, V0, Vtrig, Vcurr, hw_out, hw_in, Vtrig_previous, minuteIntervals = 1):
         """
         Runs one step on the primary system. This changes the volume of the primary system
         by assuming there is hot water removed at a volume of hw_out and hot water
         generated or added at a volume of hw_in. This is assuming the system is perfectly
         stratified and all of the hot water above the cold temperature is at the storage temperature.
 
         Parameters
         ----------
         pheating : boolean
             indicates whether system is heating at the beginning of this step
         V0 : float
             The storage volume of the primary system at the storage temperature
         Vtrig : float
             The remaining volume of the primary storage volume when heating is
-            triggered, note this equals V0*(1 - aquaFract) TODO is that true tho? 
+            triggered, note this equals V0*(1 - aquaFract) 
         Vcurr : float
             The primary volume at the timestep.
         hw_out : float
             The volume of DHW removed from the primary system, assumed that
             100% of what of what is removed is replaced
         hw_in : float
             The volume of hot water generated in a time step
+        Vtrig_previous : float
+            Trigger from last time step to see if we missed any heating (may have changed if doing load shifting)
 
         Returns
         -------
         pheating : boolean
             Boolean indicating if the primary system is heating at the end of this step in the simulation 
         Vnew : float
             The new primary volume at the timestep.
-        did_run : float
+        hw_generated : float
             The volume of hot water generated during the time step.
 
         """
-        did_run = 0
+        hw_generated = 0
         Vnew = 0
+        time_ran = 0
+        Vtrig_normal = np.ceil(self.PVol_G_atStorageT * (1 - self.aquaFract))
         if pheating:
             Vnew = Vcurr + hw_in - hw_out # If heating, generate HW and lose HW
-            did_run = hw_in
+            hw_generated = hw_in
+            time_ran = 1
 
-        else:  # Else not heating, REMOVED TIME MISSED HERE
+        else:
             Vnew = Vcurr - hw_out # So lose HW
             if Vnew < Vtrig: # If should heat
-                Vnew += hw_in # # Start heating
-                did_run = hw_in 
                 pheating = True
-
-        if Vnew > V0: # If overflow
+            if Vnew < Vtrig_previous:
+                time_ran = min((Vtrig_previous - Vnew)/hw_out, 1) # Volume below turn on / rate of draw gives time below tigger (aquastat)
+                Vnew += hw_in * time_ran
+                hw_generated = hw_in * time_ran
+
+        if self.doLoadShift and Vtrig == np.ceil(self.PVol_G_atStorageT * (1 - self.aquaFractShed)) and Vnew > Vtrig_normal:
+            # stop heating if hw has met the normal aquastat fraction during a shed period
+            time_over = (Vnew - Vtrig_normal) / (hw_in - hw_out) # Volume over generated / rate of generation gives time above full
+            Vnew = Vtrig_normal - hw_out * time_over # Make full with missing volume
+            time_ran = 1-time_over
+            hw_generated = hw_in * time_ran
+            pheating = False # Stop heating
+        elif Vnew > V0: # If overflow
             time_over = (Vnew - V0) / (hw_in - hw_out) # Volume over generated / rate of generation gives time above full
             Vnew = V0 - hw_out * time_over # Make full with missing volume
-            did_run = hw_in * (1-time_over)
+            time_ran = 1-time_over
+            hw_generated = hw_in * time_ran
             pheating = False # Stop heating
+        elif Vtrig < Vtrig_previous and Vnew > Vtrig: # turn off heating if aquastat changes and we find we are above it.
+            pheating = False
 
         if Vnew < 0:
            raise Exception("Primary storage ran out of Volume!") 
 
-        return pheating, Vnew, did_run
+        return pheating, Vnew, hw_generated, time_ran * minuteIntervals
     
-    def plotStorageLoadSim(self, return_as_div=True):
-        """
-        Returns a plot of the of the simulation for the minimum sized primary
-        system as a div or plotly figure. Can plot the minute level simulation
-
-        Implimented seperatly for Swing Tank systems
-
-        Parameters
-        ----------
-        return_as_div
-            A logical on the output, as a div (true) or as a figure (false)
-
-        Returns
-        -------
-        div/fig
-            plot_div
-        """
-        [V, G_hw, D_hw, run] = self.simulate()
-        
-        hrind_fromback = 24 # Look at the last 24 hours of the simulation not the whole thing
-        run = np.array(run[-(60*hrind_fromback):])*60
-        G_hw = np.array(G_hw[-(60*hrind_fromback):])*60
-        D_hw = np.array(D_hw[-(60*hrind_fromback):])*60
-        V = np.array(V[-(60*hrind_fromback):])
-
-        if any(i < 0 for i in V):
-            raise Exception("Primary storage ran out of Volume!") 
-        
-        fig = Figure()
-
-        # Do primary components
-        x_data = list(range(len(V)))
-
-        if self.doLoadShift:
-            ls_off = [int(not x)* max(V)*2 for x in G_hw]
-            fig.add_trace(Scatter(x=x_data, y=ls_off, name='Load Shift Off Period',
-                                  mode='lines', line_shape='hv',
-                                  opacity=0.5, marker_color='grey',
-                                  fill='tonexty'))
-
-        fig.add_trace(Scatter(x=x_data, y=V, name='Useful Storage Volume at Storage Temperature',
-                              mode='lines', line_shape='hv',
-                              opacity=0.8, marker_color='green'))
-        fig.add_trace(Scatter(x=x_data, y=run, name = "Hot Water Generation at Storage Temperature",
-                              mode='lines', line_shape='hv',
-                              opacity=0.8, marker_color='red'))
-        fig.add_trace(Scatter(x=x_data, y=D_hw, name='Hot Water Demand at Supply Temperature',
-                              mode='lines', line_shape='hv',
-                              opacity=0.8, marker_color='blue'))
-        fig.update_yaxes(range=[0, np.ceil(max(np.append(V,D_hw))/100)*100])
-
-        fig.update_layout(title="Hot Water Simulation",
-                          xaxis_title= "Minute of Day",
-                          yaxis_title="Gallons or\nGallons per Hour",
-                          width=900,
-                          height=700)
-
-        if return_as_div:
-            plot_div = plot(fig, output_type='div', show_link=False, link_text="",
-                        include_plotlyjs = False)
-            return plot_div
-        return fig
-    
-    def _calcPrelimVol(self, loadUpHours):
+    def _calcPrelimVol(self, loadUpHours, loadshape, building):
         '''
         Function to calculate volume shifted during first shed period, which is used to calculated generation rate
         needed for load up.
 
         Parameters
         ----------
         loadUpHours : float
             Number of hours of scheduled load up before first shed. If sizing, this is set by user. If creating sizing
             plot, number may vary. 
+        loadshape : ndarray
+            normalized array of length 24 representing the daily loadshape for this calculation.
+        building : Building
+            The building object being sized for 
 
         Returns 
         ----------
         Vshift : float
             Volume at supply temp between normal and load up AQ fract needed to make it through first shed period.
         VconsumedLU : float
             Volume at supply temp consumed during first load up period.
         '''
         shedHours = [i for i in range(len(self.loadShiftSchedule)) if self.loadShiftSchedule[i] == 0] #get all scheduled shed hours
         firstShed = [x for i,x in enumerate(shedHours) if x == shedHours[0] + i] #get first shed
-        Vshift = sum([self.building.avgLoadshape[i]*self.building.magnitude for i in firstShed])#calculate vol used during first shed
-        VconsumedLU = sum(self.building.avgLoadshape[firstShed[0] - loadUpHours : firstShed[0]]) * self.building.magnitude
+        Vshift = sum([loadshape[i]*building.magnitude for i in firstShed])#calculate vol used during first shed
+        VconsumedLU = sum(loadshape[firstShed[0] - loadUpHours : firstShed[0]]) * building.magnitude
         
         return Vshift, VconsumedLU 
         
         
 
-    def _mixStorageTemps(self, runningVol_G):
+    def mixStorageTemps(self, runningVol_G, incomingT_F, supplyT_F):
         """
         Calculates average tank temperature using load up and normal setpoints according to locations of aquastats. 
         Used for load shifting when there are two setpoints. Returns normal storage setpoint if load up and normal
         setpoint are equal or if not loadshifting.
 
         Parameters
         ----------
         runningVol_G : float
             Volume of water to be mixed. 
+        incomingT_F : float
+            Incoming temp (in Fahrenhiet) of city water
+        supplyT_F : float
+            Supply temp (in Fahrenhiet) of water distributed to those in the building
 
         Returns
         ----------
         mixStorageT_F: float
             Average storage temperature calcuated with normal setpoint and load up setpoint.
         totalVolMax : float
             The total storage volume in gallons adjusted to the average storage temperature.
@@ -729,20 +729,19 @@
         if self.doLoadShift:
             f = (self.aquaFract - self.aquaFractLoadUp) / (self.aquaFractShed - self.aquaFractLoadUp) 
             normV = (1 - f) * runningVol_G
             loadV = f * runningVol_G
 
             mixStorageT_F = (self.storageT_F * normV + self.loadUpT_F * loadV) / (normV + loadV)
 
-            return mixStorageT_F, mixVolume(runningVol_G, mixStorageT_F, self.building.incomingT_F, self.building.supplyT_F) / (self.aquaFractShed - self.aquaFractLoadUp)
+            return mixStorageT_F, mixVolume(runningVol_G, mixStorageT_F, incomingT_F, supplyT_F) / (self.aquaFractShed - self.aquaFractLoadUp)
         
         return [mixStorageT_F]
-
     
 class Primary(SystemConfig):
-    def __init__(self, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
+    def __init__(self, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, building,
                  doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None, loadUpHours = None, aquaFractLoadUp = None, 
-                 aquaFractShed = None, loadUpT_F = None):
-        super().__init__(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
-                 doLoadShift, loadShiftPercent, loadShiftSchedule, loadUpHours, aquaFractLoadUp, aquaFractShed, loadUpT_F)
+                 aquaFractShed = None, loadUpT_F = None, systemModel = None, PVol_G_atStorageT = None, PCap_kBTUhr = None):
+        super().__init__(storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, building, doLoadShift, 
+                loadShiftPercent, loadShiftSchedule, loadUpHours, aquaFractLoadUp, aquaFractShed, loadUpT_F, systemModel, PVol_G_atStorageT, PCap_kBTUhr)
```

### Comparing `ecoengine-0.0.6/src/ecoengine/objects/__init__.py` & `ecoengine-0.0.7/src/ecoengine/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.6/src/ecoengine/objects/systemConfigUtils.py` & `ecoengine-0.0.7/src/ecoengine/objects/systemConfigUtils.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,14 +77,35 @@
 
     """
     out_list = []
     for num in a_list:
         out_list += [num]*60
     return out_list
 
+def hrTo15MinList(a_list):
+    """
+    Repeats each element of a_list 4 times to go from hourly to 15 minute intervals.
+    Still may need other unit conversions to get data from per hour to per 15 minute
+
+    Parameters
+    ----------
+    a_list : list
+        A list in of values per hour.
+
+    Returns
+    -------
+    out_list : list
+        A list in of values per 15 minute interval created by repeating values per hour 4 times.
+
+    """
+    out_list = []
+    for num in a_list:
+        out_list += [num]*4
+    return out_list
+
 def getPeakIndices(diff1):
     """
     Finds the points of an array where the values go from positive to negative
 
     Parameters
     ----------
     diff1 : array_like
```

### Comparing `ecoengine-0.0.6/src/ecoengine.egg-info/PKG-INFO` & `ecoengine-0.0.7/src/ecoengine.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-Metadata-Version: 2.1
-Name: ecoengine
-Version: 0.0.6
-Summary: A software for sizing Heat Pump Water Heaters for buildings
-Home-page: https://ecosizer.ecotope.com/sizer/
-Author: Nolan
-Author-email: nolan@ecotope.com
-Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
-# EcosizerEngine
-
-### Requirements:
-
-This software requires a python version greater than or equal to 3.11 to be installed in the environment it is running in.
-
-### Using the package in scripts:
-
-1. Install the package with pip
-
-	$ pip install ecosizer-engine
-
-2. To import and use the tools in this package, add the following import statement to your script:
-
-	from ecosizer_engine_package import *
-
-You should now be able to use the features of EcosizerEngine in your script
-
-### Running locally in a container:
-First, clone the EcosizerEngine repo from github
-
-    $ git clone https://github.com/EcotopeResearch/EcosizerEngine.git
-
-Depending on what type of environment you want to run the code in, please follow the appropriate steps.
-
-Steps for installing in a virtual environment:
-1. Navigate to the EcosizerEngine directory. This should be the same directory level as src/, setup.py, and this README document.
-2. Run the following command:
-
-	$ pip install -e .
-
-This will install the ecosizer-engine package locally in editable format, such that changes you make in the source code here will be reflected in implementation.
-This pip install should also install all dependencies for ecosizer-engine (i.e. numpy, scipy, pytest, and plotly)
-
-Steps for installing using docker container:
-1. Navigate to the EcosizerEngine directory.
-2. Build container with docker file
-
-	$ docker build -t ecosizerengine:latest .
-
-3. Run docker container
-
-	$  docker run -it ecosizerengine bash
-
-4. When you are done messing about in the docker image, just type the command
-
-	$ exit
-
-or press ctrl+c then ctrl+d
-
-Steps for installing conda environment from the Anaconda prompt:
-1. Navigate to the EcosizerEngine directory.
-2. Create new environment from .yml file.
-
-
-	$ conda env create --file EcosizerEngine.yml
-
-If the environment creation doesn't work, make sure Anaconda is up-to-date with
-
-    $ conda update --all
-
-If that doesn't work, you may need to force Anaconda to download and use python 3.11 (it defaults to 3.9) by making another environment
-
-    $ conda create -n py311 python=3.11
-    $ conda activate py311
-    $ conda env create --file EcosizerEngine.yml
-
-3. Check that the environment was created
-
-
-	$ conda env list
-
-4. Activate the new environment
-
-
-	$ conda activate EcosizerEngine
-
-If an environment already exits it can be removed with:
-
-	$ conda remove --name EcosizerEngine --all
-
-
-All the available environment can be found with:
-
-	$ conda env list
-
-### Testing:
-From the parent directory, type
-
-	$ python -m pytest
-
-This will run all unit tests for the package
-
-### Updating Documentation:
-1. If not installed in environment: pip install sphinx and numpydocs
-2. navigate to docs directory and run:
-
-
-	$ make html
-
-### Updating version on pypi
-
-1. If you haven't installed them before, pip install build and twine
-
-	$ python -m pip install --upgrade build
-
-
-	$ python -m pip install --user --upgrade twine
-
-2. Update the version number in setup.cfg
-3. Run the following commands from the project root directory:
-
-	$ python -m build
-
-	$ python -m twine upload dist/*
-
-### Contact Information
-To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
+Metadata-Version: 2.1
+Name: ecoengine
+Version: 0.0.7
+Summary: A software for sizing Heat Pump Water Heaters for buildings
+Home-page: https://ecosizer.ecotope.com/sizer/
+Author: Nolan
+Author-email: nolan@ecotope.com
+Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+
+# EcosizerEngine
+
+### Requirements:
+
+This software requires a python version greater than or equal to 3.11 to be installed in the environment it is running in.
+
+### Using the package in scripts:
+
+1. Install the package with pip
+
+	$ pip install ecosizer-engine
+
+2. To import and use the tools in this package, add the following import statement to your script:
+
+	from ecosizer_engine_package import *
+
+You should now be able to use the features of EcosizerEngine in your script
+
+### Running locally in a container:
+First, clone the EcosizerEngine repo from github
+
+    $ git clone https://github.com/EcotopeResearch/EcosizerEngine.git
+
+Depending on what type of environment you want to run the code in, please follow the appropriate steps.
+
+Steps for installing in a virtual environment:
+1. Navigate to the EcosizerEngine directory. This should be the same directory level as src/, setup.py, and this README document.
+2. Run the following command:
+
+	$ pip install -e .
+
+This will install the ecosizer-engine package locally in editable format, such that changes you make in the source code here will be reflected in implementation.
+This pip install should also install all dependencies for ecosizer-engine (i.e. numpy, scipy, pytest, and plotly)
+
+Steps for installing using docker container:
+1. Navigate to the EcosizerEngine directory.
+2. Build container with docker file
+
+	$ docker build -t ecosizerengine:latest .
+
+3. Run docker container
+
+	$  docker run -it ecosizerengine bash
+
+4. When you are done messing about in the docker image, just type the command
+
+	$ exit
+
+or press ctrl+c then ctrl+d
+
+Steps for installing conda environment from the Anaconda prompt:
+1. Navigate to the EcosizerEngine directory.
+2. Create new environment from .yml file.
+
+
+	$ conda env create --file EcosizerEngine.yml
+
+If the environment creation doesn't work, make sure Anaconda is up-to-date with
+
+    $ conda update --all
+
+If that doesn't work, you may need to force Anaconda to download and use python 3.11 (it defaults to 3.9) by making another environment
+
+    $ conda create -n py311 python=3.11
+    $ conda activate py311
+    $ conda env create --file EcosizerEngine.yml
+
+3. Check that the environment was created
+
+
+	$ conda env list
+
+4. Activate the new environment
+
+
+	$ conda activate EcosizerEngine
+
+If an environment already exits it can be removed with:
+
+	$ conda remove --name EcosizerEngine --all
+
+
+All the available environment can be found with:
+
+	$ conda env list
+
+### Testing:
+From the parent directory, type
+
+	$ python -m pytest
+
+This will run all unit tests for the package
+
+### Updating Documentation:
+1. If not installed in environment: pip install sphinx and numpydocs
+2. navigate to docs directory and run:
+
+
+	$ make html
+
+### Updating version on pypi
+
+1. If you haven't installed them before, pip install build and twine
+
+	$ python -m pip install --upgrade build
+
+
+	$ python -m pip install --user --upgrade twine
+
+2. Update the version number in setup.cfg
+3. Run the following commands from the project root directory:
+
+	$ python -m build
+
+	$ python -m twine upload dist/*
+
+### Contact Information
+To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
```

### Comparing `ecoengine-0.0.6/src/ecoengine.egg-info/SOURCES.txt` & `ecoengine-0.0.7/src/ecoengine.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,19 @@
 src/ecoengine/data/load_shapes/multi_family.json
 src/ecoengine/data/load_shapes/nursing_home.json
 src/ecoengine/data/load_shapes/office_building.json
 src/ecoengine/data/load_shapes/senior_high.json
 src/ecoengine/data/load_shapes/womens_dorm.json
 src/ecoengine/engine/BuildingCreator.py
 src/ecoengine/engine/EcosizerEngine.py
+src/ecoengine/engine/Simulator.py
 src/ecoengine/engine/SystemCreator.py
 src/ecoengine/engine/__init__.py
 src/ecoengine/objects/Building.py
+src/ecoengine/objects/PrefMapTracker.py
+src/ecoengine/objects/SimulationRun.py
 src/ecoengine/objects/SystemConfig.py
 src/ecoengine/objects/__init__.py
 src/ecoengine/objects/systemConfigUtils.py
 src/ecoengine/objects/systems/ParallelLoopTank.py
 src/ecoengine/objects/systems/SwingTank.py
 src/ecoengine/objects/systems/__init__.py
```

