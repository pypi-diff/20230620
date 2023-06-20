# Comparing `tmp/geodata-harvester-1.0.1.tar.gz` & `tmp/geodata-harvester-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodata-harvester-1.0.1.tar", last modified: Fri May 19 06:20:41 2023, max compression
+gzip compressed data, was "geodata-harvester-1.1.0.tar", last modified: Tue Jun 20 05:12:04 2023, max compression
```

## Comparing `geodata-harvester-1.0.1.tar` & `geodata-harvester-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-19 06:20:41.110603 geodata-harvester-1.0.1/
--rw-r--r--   0 seb        (504) staff       (20)     7652 2023-01-10 23:44:41.000000 geodata-harvester-1.0.1/LICENSE.txt
--rw-r--r--   0 seb        (504) staff       (20)    12790 2023-05-19 06:20:41.110365 geodata-harvester-1.0.1/PKG-INFO
--rw-r--r--   0 seb        (504) staff       (20)    12376 2023-05-09 05:44:57.000000 geodata-harvester-1.0.1/README.md
--rw-r--r--   0 seb        (504) staff       (20)       38 2023-05-19 06:20:41.110643 geodata-harvester-1.0.1/setup.cfg
--rw-r--r--   0 seb        (504) staff       (20)     1981 2023-05-19 06:10:22.000000 geodata-harvester-1.0.1/setup.py
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-19 06:20:41.105059 geodata-harvester-1.0.1/src/
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-19 06:20:41.108245 geodata-harvester-1.0.1/src/geodata_harvester/
--rw-r--r--   0 seb        (504) staff       (20)     1030 2023-05-19 06:10:00.000000 geodata-harvester-1.0.1/src/geodata_harvester/__init__.py
--rw-r--r--   0 seb        (504) staff       (20)     1040 2022-03-23 04:23:00.000000 geodata-harvester-1.0.1/src/geodata_harvester/arc2meter.py
--rw-r--r--   0 seb        (504) staff       (20)    35525 2023-01-23 03:29:23.000000 geodata-harvester-1.0.1/src/geodata_harvester/getdata_dea.py
--rw-r--r--   0 seb        (504) staff       (20)    10787 2023-01-18 01:59:45.000000 geodata-harvester-1.0.1/src/geodata_harvester/getdata_dem.py
--rw-r--r--   0 seb        (504) staff       (20)     8655 2023-01-18 01:54:54.000000 geodata-harvester-1.0.1/src/geodata_harvester/getdata_landscape.py
--rw-r--r--   0 seb        (504) staff       (20)    11275 2023-01-18 01:55:09.000000 geodata-harvester-1.0.1/src/geodata_harvester/getdata_radiometric.py
--rw-r--r--   0 seb        (504) staff       (20)    18323 2023-05-08 08:11:38.000000 geodata-harvester-1.0.1/src/geodata_harvester/getdata_silo.py
--rw-r--r--   0 seb        (504) staff       (20)    15851 2023-02-06 06:20:02.000000 geodata-harvester-1.0.1/src/geodata_harvester/getdata_slga.py
--rw-r--r--   0 seb        (504) staff       (20)    23169 2023-05-09 01:43:38.000000 geodata-harvester-1.0.1/src/geodata_harvester/harvest.py
--rw-r--r--   0 seb        (504) staff       (20)      738 2023-01-15 23:19:22.000000 geodata-harvester-1.0.1/src/geodata_harvester/settingshandler.py
--rw-r--r--   0 seb        (504) staff       (20)     6228 2023-01-27 00:29:41.000000 geodata-harvester-1.0.1/src/geodata_harvester/spatial.py
--rw-r--r--   0 seb        (504) staff       (20)    13346 2023-05-19 06:07:38.000000 geodata-harvester-1.0.1/src/geodata_harvester/temporal.py
--rw-r--r--   0 seb        (504) staff       (20)    30584 2023-05-09 01:49:21.000000 geodata-harvester-1.0.1/src/geodata_harvester/utils.py
--rw-r--r--   0 seb        (504) staff       (20)    11604 2023-01-18 02:18:57.000000 geodata-harvester-1.0.1/src/geodata_harvester/validate_settings.py
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-19 06:20:41.109500 geodata-harvester-1.0.1/src/geodata_harvester/widgets/
--rw-rw-r--   0 seb        (504) staff       (20)       40 2016-10-31 16:56:29.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/__init__.py
--rw-r--r--   0 seb        (504) staff       (20)    25214 2023-02-16 02:40:52.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/harvesterwidgets.py
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-19 06:20:41.110082 geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/
--rwxr-xr-x   0 seb        (504) staff       (20)       60 2021-09-15 22:24:00.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/__init__.py
--rw-rw-r--   0 seb        (504) staff       (20)     1056 2021-09-15 22:24:00.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/errors.py
--rw-rw-r--   0 seb        (504) staff       (20)    22928 2022-06-09 00:48:28.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/filechooser.py
--rw-rw-r--   0 seb        (504) staff       (20)     3976 2021-09-15 22:24:00.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/utils.py
--rw-rw-r--   0 seb        (504) staff       (20)     1996 2016-10-31 16:56:29.000000 geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipywidgets_file_selector.py
--rw-r--r--   0 seb        (504) staff       (20)     3703 2022-07-14 05:17:29.000000 geodata-harvester-1.0.1/src/geodata_harvester/write_logs.py
-drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-05-19 06:20:41.109005 geodata-harvester-1.0.1/src/geodata_harvester.egg-info/
--rw-r--r--   0 seb        (504) staff       (20)    12790 2023-05-19 06:20:41.000000 geodata-harvester-1.0.1/src/geodata_harvester.egg-info/PKG-INFO
--rw-r--r--   0 seb        (504) staff       (20)     1188 2023-05-19 06:20:41.000000 geodata-harvester-1.0.1/src/geodata_harvester.egg-info/SOURCES.txt
--rw-r--r--   0 seb        (504) staff       (20)        1 2023-05-19 06:20:41.000000 geodata-harvester-1.0.1/src/geodata_harvester.egg-info/dependency_links.txt
--rw-r--r--   0 seb        (504) staff       (20)      217 2023-05-19 06:20:41.000000 geodata-harvester-1.0.1/src/geodata_harvester.egg-info/requires.txt
--rw-r--r--   0 seb        (504) staff       (20)       18 2023-05-19 06:20:41.000000 geodata-harvester-1.0.1/src/geodata_harvester.egg-info/top_level.txt
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-06-20 05:12:04.054672 geodata-harvester-1.1.0/
+-rw-r--r--   0 seb        (504) staff       (20)     7652 2023-01-10 23:44:41.000000 geodata-harvester-1.1.0/LICENSE.txt
+-rw-r--r--   0 seb        (504) staff       (20)    17330 2023-06-20 05:12:04.054421 geodata-harvester-1.1.0/PKG-INFO
+-rw-r--r--   0 seb        (504) staff       (20)    16916 2023-06-20 05:06:02.000000 geodata-harvester-1.1.0/README.md
+-rw-r--r--   0 seb        (504) staff       (20)       38 2023-06-20 05:12:04.054727 geodata-harvester-1.1.0/setup.cfg
+-rw-r--r--   0 seb        (504) staff       (20)     1981 2023-06-20 05:02:13.000000 geodata-harvester-1.1.0/setup.py
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-06-20 05:12:04.041934 geodata-harvester-1.1.0/src/
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-06-20 05:12:04.049393 geodata-harvester-1.1.0/src/geodata_harvester/
+-rw-r--r--   0 seb        (504) staff       (20)     1030 2023-06-20 03:03:38.000000 geodata-harvester-1.1.0/src/geodata_harvester/__init__.py
+-rw-r--r--   0 seb        (504) staff       (20)     1040 2022-03-23 04:23:00.000000 geodata-harvester-1.1.0/src/geodata_harvester/arc2meter.py
+-rw-r--r--   0 seb        (504) staff       (20)    32251 2023-06-20 00:37:59.000000 geodata-harvester-1.1.0/src/geodata_harvester/getdata_dea.py
+-rw-r--r--   0 seb        (504) staff       (20)    12480 2023-06-06 02:44:48.000000 geodata-harvester-1.1.0/src/geodata_harvester/getdata_dem.py
+-rw-r--r--   0 seb        (504) staff       (20)     8655 2023-01-18 01:54:54.000000 geodata-harvester-1.1.0/src/geodata_harvester/getdata_landscape.py
+-rw-r--r--   0 seb        (504) staff       (20)     9576 2023-06-20 00:54:07.000000 geodata-harvester-1.1.0/src/geodata_harvester/getdata_radiometric.py
+-rw-r--r--   0 seb        (504) staff       (20)    18323 2023-05-08 08:11:38.000000 geodata-harvester-1.1.0/src/geodata_harvester/getdata_silo.py
+-rw-r--r--   0 seb        (504) staff       (20)    15851 2023-02-06 06:20:02.000000 geodata-harvester-1.1.0/src/geodata_harvester/getdata_slga.py
+-rw-r--r--   0 seb        (504) staff       (20)    23589 2023-06-14 01:56:07.000000 geodata-harvester-1.1.0/src/geodata_harvester/harvest.py
+-rw-r--r--   0 seb        (504) staff       (20)     2902 2023-06-15 02:21:58.000000 geodata-harvester-1.1.0/src/geodata_harvester/settingshandler.py
+-rw-r--r--   0 seb        (504) staff       (20)     6228 2023-01-27 00:29:41.000000 geodata-harvester-1.1.0/src/geodata_harvester/spatial.py
+-rw-r--r--   0 seb        (504) staff       (20)    13887 2023-06-20 01:31:00.000000 geodata-harvester-1.1.0/src/geodata_harvester/temporal.py
+-rw-r--r--   0 seb        (504) staff       (20)    30625 2023-06-15 05:14:35.000000 geodata-harvester-1.1.0/src/geodata_harvester/utils.py
+-rw-r--r--   0 seb        (504) staff       (20)    11604 2023-01-18 02:18:57.000000 geodata-harvester-1.1.0/src/geodata_harvester/validate_settings.py
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-06-20 05:12:04.051886 geodata-harvester-1.1.0/src/geodata_harvester/widgets/
+-rw-rw-r--   0 seb        (504) staff       (20)       40 2016-10-31 16:56:29.000000 geodata-harvester-1.1.0/src/geodata_harvester/widgets/__init__.py
+-rw-r--r--   0 seb        (504) staff       (20)    25818 2023-06-14 05:19:31.000000 geodata-harvester-1.1.0/src/geodata_harvester/widgets/harvesterwidgets.py
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-06-20 05:12:04.053235 geodata-harvester-1.1.0/src/geodata_harvester/widgets/ipyfilechooser/
+-rwxr-xr-x   0 seb        (504) staff       (20)       60 2021-09-15 22:24:00.000000 geodata-harvester-1.1.0/src/geodata_harvester/widgets/ipyfilechooser/__init__.py
+-rw-rw-r--   0 seb        (504) staff       (20)     1056 2021-09-15 22:24:00.000000 geodata-harvester-1.1.0/src/geodata_harvester/widgets/ipyfilechooser/errors.py
+-rw-rw-r--   0 seb        (504) staff       (20)    22928 2022-06-09 00:48:28.000000 geodata-harvester-1.1.0/src/geodata_harvester/widgets/ipyfilechooser/filechooser.py
+-rw-rw-r--   0 seb        (504) staff       (20)     3976 2021-09-15 22:24:00.000000 geodata-harvester-1.1.0/src/geodata_harvester/widgets/ipyfilechooser/utils.py
+-rw-rw-r--   0 seb        (504) staff       (20)     1996 2016-10-31 16:56:29.000000 geodata-harvester-1.1.0/src/geodata_harvester/widgets/ipywidgets_file_selector.py
+-rw-r--r--   0 seb        (504) staff       (20)     3703 2022-07-14 05:17:29.000000 geodata-harvester-1.1.0/src/geodata_harvester/write_logs.py
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-06-20 05:12:04.050674 geodata-harvester-1.1.0/src/geodata_harvester.egg-info/
+-rw-r--r--   0 seb        (504) staff       (20)    17330 2023-06-20 05:12:04.000000 geodata-harvester-1.1.0/src/geodata_harvester.egg-info/PKG-INFO
+-rw-r--r--   0 seb        (504) staff       (20)     1297 2023-06-20 05:12:04.000000 geodata-harvester-1.1.0/src/geodata_harvester.egg-info/SOURCES.txt
+-rw-r--r--   0 seb        (504) staff       (20)        1 2023-06-20 05:12:04.000000 geodata-harvester-1.1.0/src/geodata_harvester.egg-info/dependency_links.txt
+-rw-r--r--   0 seb        (504) staff       (20)      217 2023-06-20 05:12:04.000000 geodata-harvester-1.1.0/src/geodata_harvester.egg-info/requires.txt
+-rw-r--r--   0 seb        (504) staff       (20)       18 2023-06-20 05:12:04.000000 geodata-harvester-1.1.0/src/geodata_harvester.egg-info/top_level.txt
+drwxr-xr-x   0 seb        (504) staff       (20)        0 2023-06-20 05:12:04.054106 geodata-harvester-1.1.0/tests/
+-rw-r--r--   0 seb        (504) staff       (20)     3630 2023-06-20 00:20:43.000000 geodata-harvester-1.1.0/tests/test_getdata_dea.py
+-rw-r--r--   0 seb        (504) staff       (20)     2238 2023-06-20 00:51:15.000000 geodata-harvester-1.1.0/tests/test_getdata_radiometric.py
+-rw-r--r--   0 seb        (504) staff       (20)     1239 2023-06-20 01:00:37.000000 geodata-harvester-1.1.0/tests/test_getdata_silo.py
+-rw-r--r--   0 seb        (504) staff       (20)     1245 2023-06-20 01:46:08.000000 geodata-harvester-1.1.0/tests/test_harvest.py
```

### Comparing `geodata-harvester-1.0.1/LICENSE.txt` & `geodata-harvester-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.1/PKG-INFO` & `geodata-harvester-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodata-harvester
-Version: 1.0.1
+Version: 1.1.0
 Summary: An automation tool for harvesting and processing geodata from the web
 Home-page: https://github.com/Sydney-Informatics-Hub/geodata-harvester
 License: LGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -39,16 +39,18 @@
 - [Key Features](#-key-features)
 - [Installation](#-installation)
     - [Conda or Mamba](#conda-or-mamba)
     - [PyPI](#pypi)
     - [Google Earth Engine extension](#google-earth-engine-extension)
     - [Local development](#local-development)
     - [Workshop Cloud Sandbox](#workshop-cloud-sandbox)
+- [Settings Overview](#-settings-overview)
 - [How to get started](#-how-to-get-started)
 - [How to add new data source modules](#-how-to-add-new-data-source-modules)
+- [Testing](#-testing)
 - [Code reference API](#-code-reference-api)
 - [Contributions](#-contributions)
 - [Attribution and Acknowledgments](#-attribution-and-acknowledgments)
 - [License](#-license)
 
 
 ## 💡 Introduction
@@ -67,40 +69,38 @@
 - SILO Climate Database
 - National Digital Elevation Model (DEM) 1 Second Hydrologically Enforced
 - Digital Earth Australia (DEA) Geoscience Earth Observations
 - GSKY Data Server for DEA Geoscience Earth Observations
 - Radiometric Data
 - Google Earth Engine Data (GEE account needed), see for overview [Earth_Engine_Data_Overview](quarto/docs/Earth_Engine_Data_Overview.md).
 
-## Functionality
+## 🔄 Functionality
 
 The main goal of the Data Harvester is to enable researchers with reusable workflows for automatic data extraction and processing:
 
 1. Retrieve: given set of locations, automatically access and download multiple data sources (APIs) from a diverse range of geospatial and soil data sources
 2. Process: Spatial and temporal processing, conversion to dataframes and custom raster-files
 3. Output: Ready-made dataset for machine learning (training set and prediction mapping)
 
 Geodata-Harvester is designed as a modular and maintainable project in the form of a multi-stage pipeline by providing explicit boundaries among tasks. To encourage interaction and experimentation with the pipeline, multiple frontend notebooks and use case scenarios are provided.
 
 ## 🌟 Key Features
 
-Below is a list of features available for the geodata-harvester package. Please check the project Github webpage and notebooks for examples, data selection, and other settings.
+The geodata-harvester package provides the following core features:
 
-- enabling reproducible workflows via YAML settings files.
-- automatic data retrieval from geodata APIs for given locations and dates.
-- automatic download and spatiotemporal processing of geo-spatial maps for user-specified bounding box, resolution, and time-scale.
-- support for time-series data extraction for multiple time slices. 
-- automatic extraction of retrieved data into ready-made dataframes for ML training.
-- automatic generation of ready-made aligned maps in GeoTiff format.
-- preview of downloaded and aligned maps.
-- support for saving and loading settings via interactive widgets.
-- with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices.
-- example notebooks and use-cases are provided for the user to get started.
+- enabling reproducible workflows via YAML settings files (see for settings example [settings_harvest.yaml](notebooks/settings/settings_harvest.yaml)).
+- interactive widgets for settings selection (see for example notebook [example_harvest_with_widgets.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_with_widgets.ipynb)).
+- automated download and processing pipeline for multiple data sources (supported by the `harvest.run()` function as demonstrated in the example notebook [example_harvest.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest.ipynb)).
+- automatic data retrieval from geodata APIs and spatiotemporal processing for given locations, bounding box, resoultion, and time-scales into ready-made aligned and geo-referenced maps in GeoTiff format (see [notebook API download and process step](https://nbviewer.jupyter.org/github/Sydney-Informatics-Hub/geodata-harvester/blob/main/notebooks/example_harvest_stepwise.ipynb#Download-and-process-data-from-API-sources)).
+- support for time-series data extraction for multiple time slices (see example notebook [example_harvest_temporal1.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_temporal1.ipynb) and [example_harvest_temporal2.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_temporal2.ipynb)). 
+- automatic extraction of retrieved data into ready-made dataframes for ML training ([see notebook point extraction process](https://nbviewer.jupyter.org/github/Sydney-Informatics-Hub/geodata-harvester/blob/main/notebooks/example_harvest_stepwise.ipynb#Points-extraction-from-downloaded/processed-data))).
+- preview of downloaded and aligned maps (see [notebook preview example](https://nbviewer.jupyter.org/github/Sydney-Informatics-Hub/geodata-harvester/blob/main/notebooks/example_harvest_stepwise.ipynb#Overview-plot-of-all-processed-rasters)).
+- with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices (see pipeline notebook [example_harvest_withGEE.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_withGEE.ipynb)) or the [step-by-step GEE process instructions](https://nbviewer.jupyter.org/github/Sydney-Informatics-Hub/geodata-harvester/blob/main/notebooks/example_harvest_stepwise.ipynb#Google-Earth-Engine).
 
-For more features, please see the [API reference documentation](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
+For more details about all functionalities, please consult the [API reference documentation](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
 
 ## 🔧 Installation
 
 Geodata-Harvester can be run on cloud-servers (e.g., in JupyterHub environment) or on your local machine. 
 Example notebooks for importing and using the package can be found in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks). The package can be installed via PyPI or Conda:
 
 ### Conda or Mamba
@@ -150,33 +150,65 @@
 
 As play-ground for workshop training sessions and testing of the Geodata-Harvester we provide a pre-installed cloud Python Jupyterlab environment, which does not require any local installation. For login instructions and how to access the sandbox, please visit our [Python workshop page](https://sydney-informatics-hub.github.io/AgReFed-Workshop/pydocs/py00-workshop.html).
 
 The Jupyter environment is hosted on the ARDC Nectar Research Cloud in partnership with AgReFed and Australian Research Data Commons (ARDC). Note that this sandbox is currently hosted for test purposes only and generated data is not permanently stored.
 
 The Geodata-Harvester can be easily installed also on other cloud services (e.g., Google Colab, Azure Notebooks).
 
+## ⚙️ Settings Overview
+
+The Geodata-Harvester is controlled by a settings file in YAML format. The settings file contains all user-defined settings for the data extraction and processing. A detailed settings overview is provided in [Settings_Overview](quarto/docs/Settings_Overview.md). Example settings files are provided along the notebooks in the folder [notebooks/settings](notebooks/settings).  
+
+Alternatively a settings file can be also created via the interactive widget-panels as demonstrated in the notebook [example_harvest_with_widgets.ipynb](notebooks/example_harvest_with_widgets.ipynb).
+
 
 ## 🚀 How to get started
 
 You may now invoke the geodata-harvester directly from a python terminal with:
 
 ```python
 import geodata_harvester as gdh
 gdh.harvest.run(PATH_TO_SETTINGS_YAMLFILE)
 ```
 
 **Note the subtle but important difference in use of an underscore `_` to import the package and the use of a dash `-` to install it!**
 
 To get started, some example workflows are provided as Jupyter notebooks:
 
-1. Options and user settings are defined by the user in the settings; see for settings documentation [Settings_Overview](quarto/docs/Settings_Overview.md)
+1. Clone the geodata-harvester repo to your local machine or cloud server. Alternatively, download the package as zip folder from the [geodata-harvester Github page](https://github.com/Sydney-Informatics-Hub/geodata-harvester/archive/refs/heads/main.zip) and unzip the folder. This will download the geodata-harvester package including the example notebooks, settings files and example input data.
+
+2. Options and user settings are defined by the user in the settings; see for example settings file [settings_harvest.yaml](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/settings/settings_harvest.yaml)
+
+3. Run a jupyter notebook in the notebooks folder, such as  [example_harvest.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest.ipynb).
+
+4. The notebook will run the geodata-harvester with the settings file and download/process all the requested data. The final data is saved in the folder `results_example_harvest` in the current working directory as specified in the settings file. There you can find the generated data table `results.csv` and the downloaded georeferenced .tif files (open with, e.g., rasterio, QGIS or ArcGIS). A summary of all generated images is provided in the table `download_summary.csv`.
+
+A step-by-step tutorial on how to use the individual modules of the Geodata-Harvester is provided in the notebook [example_harvest_stepwise.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_stepwise.ipynb).
+
+To include Google Earth Engine (GEE) data in Geodata-Harvester, please follow the instructions in the notebook [example_harvest_withGEE.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_withGEE.ipynb). Note that this requires a GEE account and authorisation (see [Google Earth Engine extension](#google-earth-engine-extension)).
 
-2. Run the jupyter notebook in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks).
+If you would like to learn more about the Geodata-Harvester, please also visit our [Workshop webpage](https://sydney-informatics-hub.github.io/AgReFed-Workshop/).
+
+## ✅ Testing
+
+Test functions are included in the [tests](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/tests) folder. Note that due to the nature of this package, these tests require an internet connection and may fail if the data source API servers are not available or the data source API has changed. To run automated tests with `pytest`, you need to install the package with
+```bash
+pip install pytest
+```
+and then run:
+```bash
+cd tests
+pytest ./
+```
+or test individual modules with, e.g.,
+```bash
+cd tests
+pytest test_getdata_dea.py
+```
 
-If you would like to learn more about the Geodata-Harvester, please visit our [Workshop webpage](https://sydney-informatics-hub.github.io/AgReFed-Workshop/).
 
 ## ➕ How to add new data source modules
 
 The Geodata-Harvester is designed to be extendable and new data source modules can be added as Python modules (for examples, see `getdata_*.py` modules). If you would like to add a new data source, please follow the [adding new data source guidelines](quarto/docs/How_to_add_DataSources.md)  
 
 We recommend to fork the geodata-harvester repo and develop new modules in a local environment. If you would like to contribute your data source module to the geodata-harvester package, please visit the [geodata-harvester contribution guidelines](quarto/docs/Contributing.md).
```

### Comparing `geodata-harvester-1.0.1/README.md` & `geodata-harvester-1.1.0/src/geodata_harvester.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: geodata-harvester
+Version: 1.1.0
+Summary: An automation tool for harvesting and processing geodata from the web
+Home-page: https://github.com/Sydney-Informatics-Hub/geodata-harvester
+License: LGPL-3.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Geodata-Harvester
 
 <h3><em>Automate geodata harvesting from the web and jumpstart your analysis with a ready-made set of spatiotemporal processed maps and data tables.</em></h3> 
 
 <center><a><img src="quarto/images/dataharvester_logo.png" alt="Geodata-Harvester logo" width="100%"/></a></center>
 
 
@@ -27,16 +39,18 @@
 - [Key Features](#-key-features)
 - [Installation](#-installation)
     - [Conda or Mamba](#conda-or-mamba)
     - [PyPI](#pypi)
     - [Google Earth Engine extension](#google-earth-engine-extension)
     - [Local development](#local-development)
     - [Workshop Cloud Sandbox](#workshop-cloud-sandbox)
+- [Settings Overview](#-settings-overview)
 - [How to get started](#-how-to-get-started)
 - [How to add new data source modules](#-how-to-add-new-data-source-modules)
+- [Testing](#-testing)
 - [Code reference API](#-code-reference-api)
 - [Contributions](#-contributions)
 - [Attribution and Acknowledgments](#-attribution-and-acknowledgments)
 - [License](#-license)
 
 
 ## 💡 Introduction
@@ -55,40 +69,38 @@
 - SILO Climate Database
 - National Digital Elevation Model (DEM) 1 Second Hydrologically Enforced
 - Digital Earth Australia (DEA) Geoscience Earth Observations
 - GSKY Data Server for DEA Geoscience Earth Observations
 - Radiometric Data
 - Google Earth Engine Data (GEE account needed), see for overview [Earth_Engine_Data_Overview](quarto/docs/Earth_Engine_Data_Overview.md).
 
-## Functionality
+## 🔄 Functionality
 
 The main goal of the Data Harvester is to enable researchers with reusable workflows for automatic data extraction and processing:
 
 1. Retrieve: given set of locations, automatically access and download multiple data sources (APIs) from a diverse range of geospatial and soil data sources
 2. Process: Spatial and temporal processing, conversion to dataframes and custom raster-files
 3. Output: Ready-made dataset for machine learning (training set and prediction mapping)
 
 Geodata-Harvester is designed as a modular and maintainable project in the form of a multi-stage pipeline by providing explicit boundaries among tasks. To encourage interaction and experimentation with the pipeline, multiple frontend notebooks and use case scenarios are provided.
 
 ## 🌟 Key Features
 
-Below is a list of features available for the geodata-harvester package. Please check the project Github webpage and notebooks for examples, data selection, and other settings.
+The geodata-harvester package provides the following core features:
 
-- enabling reproducible workflows via YAML settings files.
-- automatic data retrieval from geodata APIs for given locations and dates.
-- automatic download and spatiotemporal processing of geo-spatial maps for user-specified bounding box, resolution, and time-scale.
-- support for time-series data extraction for multiple time slices. 
-- automatic extraction of retrieved data into ready-made dataframes for ML training.
-- automatic generation of ready-made aligned maps in GeoTiff format.
-- preview of downloaded and aligned maps.
-- support for saving and loading settings via interactive widgets.
-- with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices.
-- example notebooks and use-cases are provided for the user to get started.
+- enabling reproducible workflows via YAML settings files (see for settings example [settings_harvest.yaml](notebooks/settings/settings_harvest.yaml)).
+- interactive widgets for settings selection (see for example notebook [example_harvest_with_widgets.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_with_widgets.ipynb)).
+- automated download and processing pipeline for multiple data sources (supported by the `harvest.run()` function as demonstrated in the example notebook [example_harvest.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest.ipynb)).
+- automatic data retrieval from geodata APIs and spatiotemporal processing for given locations, bounding box, resoultion, and time-scales into ready-made aligned and geo-referenced maps in GeoTiff format (see [notebook API download and process step](https://nbviewer.jupyter.org/github/Sydney-Informatics-Hub/geodata-harvester/blob/main/notebooks/example_harvest_stepwise.ipynb#Download-and-process-data-from-API-sources)).
+- support for time-series data extraction for multiple time slices (see example notebook [example_harvest_temporal1.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_temporal1.ipynb) and [example_harvest_temporal2.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_temporal2.ipynb)). 
+- automatic extraction of retrieved data into ready-made dataframes for ML training ([see notebook point extraction process](https://nbviewer.jupyter.org/github/Sydney-Informatics-Hub/geodata-harvester/blob/main/notebooks/example_harvest_stepwise.ipynb#Points-extraction-from-downloaded/processed-data))).
+- preview of downloaded and aligned maps (see [notebook preview example](https://nbviewer.jupyter.org/github/Sydney-Informatics-Hub/geodata-harvester/blob/main/notebooks/example_harvest_stepwise.ipynb#Overview-plot-of-all-processed-rasters)).
+- with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices (see pipeline notebook [example_harvest_withGEE.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_withGEE.ipynb)) or the [step-by-step GEE process instructions](https://nbviewer.jupyter.org/github/Sydney-Informatics-Hub/geodata-harvester/blob/main/notebooks/example_harvest_stepwise.ipynb#Google-Earth-Engine).
 
-For more features, please see the [API reference documentation](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
+For more details about all functionalities, please consult the [API reference documentation](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
 
 ## 🔧 Installation
 
 Geodata-Harvester can be run on cloud-servers (e.g., in JupyterHub environment) or on your local machine. 
 Example notebooks for importing and using the package can be found in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks). The package can be installed via PyPI or Conda:
 
 ### Conda or Mamba
@@ -138,33 +150,65 @@
 
 As play-ground for workshop training sessions and testing of the Geodata-Harvester we provide a pre-installed cloud Python Jupyterlab environment, which does not require any local installation. For login instructions and how to access the sandbox, please visit our [Python workshop page](https://sydney-informatics-hub.github.io/AgReFed-Workshop/pydocs/py00-workshop.html).
 
 The Jupyter environment is hosted on the ARDC Nectar Research Cloud in partnership with AgReFed and Australian Research Data Commons (ARDC). Note that this sandbox is currently hosted for test purposes only and generated data is not permanently stored.
 
 The Geodata-Harvester can be easily installed also on other cloud services (e.g., Google Colab, Azure Notebooks).
 
+## ⚙️ Settings Overview
+
+The Geodata-Harvester is controlled by a settings file in YAML format. The settings file contains all user-defined settings for the data extraction and processing. A detailed settings overview is provided in [Settings_Overview](quarto/docs/Settings_Overview.md). Example settings files are provided along the notebooks in the folder [notebooks/settings](notebooks/settings).  
+
+Alternatively a settings file can be also created via the interactive widget-panels as demonstrated in the notebook [example_harvest_with_widgets.ipynb](notebooks/example_harvest_with_widgets.ipynb).
+
 
 ## 🚀 How to get started
 
 You may now invoke the geodata-harvester directly from a python terminal with:
 
 ```python
 import geodata_harvester as gdh
 gdh.harvest.run(PATH_TO_SETTINGS_YAMLFILE)
 ```
 
 **Note the subtle but important difference in use of an underscore `_` to import the package and the use of a dash `-` to install it!**
 
 To get started, some example workflows are provided as Jupyter notebooks:
 
-1. Options and user settings are defined by the user in the settings; see for settings documentation [Settings_Overview](quarto/docs/Settings_Overview.md)
+1. Clone the geodata-harvester repo to your local machine or cloud server. Alternatively, download the package as zip folder from the [geodata-harvester Github page](https://github.com/Sydney-Informatics-Hub/geodata-harvester/archive/refs/heads/main.zip) and unzip the folder. This will download the geodata-harvester package including the example notebooks, settings files and example input data.
+
+2. Options and user settings are defined by the user in the settings; see for example settings file [settings_harvest.yaml](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/settings/settings_harvest.yaml)
+
+3. Run a jupyter notebook in the notebooks folder, such as  [example_harvest.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest.ipynb).
+
+4. The notebook will run the geodata-harvester with the settings file and download/process all the requested data. The final data is saved in the folder `results_example_harvest` in the current working directory as specified in the settings file. There you can find the generated data table `results.csv` and the downloaded georeferenced .tif files (open with, e.g., rasterio, QGIS or ArcGIS). A summary of all generated images is provided in the table `download_summary.csv`.
+
+A step-by-step tutorial on how to use the individual modules of the Geodata-Harvester is provided in the notebook [example_harvest_stepwise.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_stepwise.ipynb).
+
+To include Google Earth Engine (GEE) data in Geodata-Harvester, please follow the instructions in the notebook [example_harvest_withGEE.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_withGEE.ipynb). Note that this requires a GEE account and authorisation (see [Google Earth Engine extension](#google-earth-engine-extension)).
 
-2. Run the jupyter notebook in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks).
+If you would like to learn more about the Geodata-Harvester, please also visit our [Workshop webpage](https://sydney-informatics-hub.github.io/AgReFed-Workshop/).
+
+## ✅ Testing
+
+Test functions are included in the [tests](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/tests) folder. Note that due to the nature of this package, these tests require an internet connection and may fail if the data source API servers are not available or the data source API has changed. To run automated tests with `pytest`, you need to install the package with
+```bash
+pip install pytest
+```
+and then run:
+```bash
+cd tests
+pytest ./
+```
+or test individual modules with, e.g.,
+```bash
+cd tests
+pytest test_getdata_dea.py
+```
 
-If you would like to learn more about the Geodata-Harvester, please visit our [Workshop webpage](https://sydney-informatics-hub.github.io/AgReFed-Workshop/).
 
 ## ➕ How to add new data source modules
 
 The Geodata-Harvester is designed to be extendable and new data source modules can be added as Python modules (for examples, see `getdata_*.py` modules). If you would like to add a new data source, please follow the [adding new data source guidelines](quarto/docs/How_to_add_DataSources.md)  
 
 We recommend to fork the geodata-harvester repo and develop new modules in a local environment. If you would like to contribute your data source module to the geodata-harvester package, please visit the [geodata-harvester contribution guidelines](quarto/docs/Contributing.md).
```

### Comparing `geodata-harvester-1.0.1/setup.py` & `geodata-harvester-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 from os import path
 import io
 
-PYPI_VERSION = '1.0.1'
+PYPI_VERSION = '1.1.0'
 
 this_directory = path.abspath(path.dirname(__file__))
 with io.open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 packages = find_packages('src')
 package_dir = {'': 'src'}
```

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/__init__.py` & `geodata-harvester-1.1.0/src/geodata_harvester/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 - SILO Climate Database, see getdata_silo.py
 - National Digital Elevation Model (DEM), see getdata_dem.py
 - Digital Earth Australia (DEA) Geoscience Earth Observations, see getdata_dea.py
 - Radiometric Data, see getdata_radiometric.py
 - Google Earth Engine Data (GEE account needed), see docs for eeharvest
 """
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 __title__ = "Geodata-Harvester"
 __description__ = """
 This Python package provides automation tools for harvesting and processing geodata from the web.
 """
 __uri__ = "https://github.com/Sydney-Informatics-Hub/geodata-harvester"
 __doc__ = __description__ + " <" + __uri__ + ">"
```

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/arc2meter.py` & `geodata-harvester-1.1.0/src/geodata_harvester/arc2meter.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/getdata_dea.py` & `geodata-harvester-1.1.0/src/geodata_harvester/getdata_dea.py`

 * *Files 3% similar despite different names*

```diff
@@ -783,31 +783,30 @@
             fname_out = f"{layername}{fname_end}"
             outfname = os.path.join(outpath, fname_out)
         else:
             datestring = datetime.fromisoformat(
                 date[:-1]).astimezone(timezone.utc)
             fname_out = f"{layername}_{datestring.year}-{datestring.month}-{datestring.day}{fname_end}"
         outfname = os.path.join(outpath, fname_out)
-        if os.path.exists(outfname):
-            outfnames.append(outfname)
+        #if os.path.exists(outfname):
+        #    outfnames.append(outfname)
         # Get data
         download_ok = get_wcsmap(
             outfname,
             layername,
             bbox,
             date,
             resolution,
             url,
             crs=crs,
             format_out=format_out,
         )
         # Log download success message if file does not already exist
         if download_ok:
-            # outfnames.append(outfname)
-            pass
+            outfnames.append(outfname)
         else:
             cprint(f"✘ {layername} for date {date} failed to download", "red")
     # return [item for sublist in outfnames for item in sublist]
     return outfnames
 
 
 def get_dea_images_daterange(
@@ -907,118 +906,8 @@
             format_out=format_out,
         )
         # Log download success message if file does not already exist
         if download_ok:
             outfnames.append(outfname)
         else:
             cprint(f"✘ {layername} for date {date} failed to download", "red")
-    return outfnames
-
-
-### Some test functions ###
-
-
-def test_get_capabilities():
-    """
-    Test script to retrieve WCS capabilities
-    """
-    # DEA layer
-    url = "https://ows.dea.ga.gov.au/?version=1.3.0"
-    # Get capabilities
-    keys, title_list, description_list, bbox_list, timelimits, nbands = get_capabilities(url)
-    assert len(keys) > 0
-    print('Test passed')
-
-
-def test_get_times():
-    """
-    Test script to retrieve available times for a layer
-    """
-    layername = "ga_ls8c_ard_3"
-    url = "https://ows.dea.ga.gov.au/?version=1.3.0"
-    times = get_times(url, layername)
-    assert len(times) > 0
-    print('Test passed')
-
-
-def test_get_times_startend():
-    """
-    Test script to retrieve available times for a layer
-    """
-    layername = "ga_ls8c_ard_3"
-    url = "https://ows.dea.ga.gov.au/?version=1.3.0"
-    dt_start = "2020-01-01"
-    dt_end = "2020-02-20"
-    times = get_times_startend(url, layername, dt_start, dt_end)
-    assert len(times) > 0
-    print('Test passed')
-
-
-def test_get_wcsmap():
-    """
-    Test script to retrieve and save image for one layer and date
-    """
-    url = "https://ows.dea.ga.gov.au/?version=1.3.0"
-    layername = "ga_ls8c_ard_3"
-    times = get_times(url, layername)
-    crs = "EPSG:4326"  # WGS84
-    # define bounding box for retrieval (simple test here for entire Australia)
-    bbox = [130, -40, 150, -20]
-    # define resolution (in arcsecs per pixel since crs is in WGS84)
-    resolution = 100
-    # get latest image
-    time = times[-1]
-    # define output file name
-    fname_out = f"test_{layername}_{time}.tif"
-    # Get data
-    download_ok = get_wcsmap(fname_out, layername, bbox, time, resolution, url)
-    assert download_ok
-    print('Test passed')
-
-
-def test_get_dea_images():
-    """
-    Test script to retrieve and save images for a given year
-    """
-    url = "https://ows.dea.ga.gov.au/?version=1.3.0"
-    # Get data (here only for first layer)
-    layername = "ga_ls8c_ard_3"
-    # Crs for output
-    crs = "EPSG:4326"  # WGS84
-    # define bounding box for retrieval (simple test here for entire Australia)
-    bbox = [120, -40, 140, -20]
-    # define resolution (in arcsecs per pixel since crs is in WGS84)
-    resolution = 100
-    # define year
-    year = 2019
-    # define outpath
-    outpath = "test_dea"
-    # Get data
-    outfnames = get_dea_images(
-        layername, year, bbox, resolution, outpath, crs=crs)
-    assert len(outfnames) > 0
-    print('Test passed')
-
-
-def test_get_dea_images_daterange():
-    """
-    Test script to retrieve and save images for a given year
-    """
-    url = "https://ows.dea.ga.gov.au/?version=1.3.0"
-    # Get data (here only for first layer)
-    layername = "ga_ls8c_ard_3"
-    # Crs for output
-    crs = "EPSG:4326"  # WGS84
-    # define bounding box for retrieval (simple test here for entire Australia)
-    bbox = [120, -40, 140, -20]
-    # define resolution (in arcsecs per pixel since crs is in WGS84)
-    resolution = 100
-    # define daterange
-    date_min = '2019-01-01'
-    date_max = '2019-01-10'
-    # define outpath
-    outpath = "test_dea"
-    # Get data
-    outfnames = get_dea_images_daterange(
-        layername, date_min, date_max, bbox, resolution, outpath, crs=crs)
-    assert len(outfnames) > 0
-    print('Test passed')
+    return outfnames
```

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/getdata_dem.py` & `geodata-harvester-1.1.0/src/geodata_harvester/getdata_dem.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,39 +20,37 @@
 https://ecat.ga.gov.au/geonetwork/srv/eng/catalog.search#/metadata/72759
 
 WCS url:
 https://services.ga.gov.au/site_9/services/DEM_SRTM_1Second_Hydro_Enforced/MapServer/WCSServer?request=GetCapabilities&service=WCS
 
 This package is part of the Data Harvester project developed for the Agricultural Research Federation (AgReFed).
 
-Copyright 2022 Sydney Informatics Hub (SIH), The University of Sydney
+Copyright 2023 Sydney Informatics Hub (SIH), The University of Sydney
 
 This open-source software is released under the LGPL-3.0 License.
 
 Author: Sebastian Haan
 """
 
 import logging
 import os
 from datetime import datetime, timezone
 from geodata_harvester import utils
 from geodata_harvester.utils import spin
+from geodata_harvester import arc2meter
 
 import rasterio
 
 # logger setup
 from geodata_harvester import write_logs
 from owslib.wcs import WebCoverageService
 from rasterio.plot import show
 from termcolor import cprint
-
-try:
-    from osgeo import gdal
-except ImportError:
-    import gdal
+import rioxarray
+import numpy as np
 
 
 def get_demdict():
     """
     Get dictionary of meta data
 
     OUTPUT:
@@ -280,29 +278,80 @@
     infname : str
     """
     data = rasterio.open(infname)
     # show image
     show(data)
 
 
+
+def calculate_slope_aspect(fname_dem, fname_out, type='slope'):
+    """
+    Calculate slope or aspect from DEM and save as geotiff.
+
+    Parameters
+    ----------
+    fname_dem : str
+        DEM file name
+    fname_out : str
+        output filename
+    type : str
+        'slope' or 'aspect'
+    """
+    # check if type is valid
+    if type not in ['slope', 'aspect']:
+        raise ValueError(f"Type {type} not recognised, must be 'slope' or 'aspect'")
+
+    # Open the DEM file
+    dem = rioxarray.open_rasterio(fname_dem, masked=True)
+
+    # convert dem  to meters if necessary
+    if dem.rio.crs != 'EPSG:4326':
+        dem = dem.rio.reproject('EPSG:4326')
+    # caculate factor for converting degrees to meter based on Latitude
+    deg2meter_x = arc2meter.calc_arc2meter(3600, dem.y)[0] # this is an array (due to Latitude dependency in conversion)
+    deg2meter_y = arc2meter.calc_arc2meter(3600, dem.y)[1] # ths is a constant
+
+    # Calculate the gradient in the x and y directions
+    gradient_x = dem.differentiate("x") / deg2meter_x
+    gradient_y = dem.differentiate("y") / deg2meter_y
+
+    # Calculate slope:
+    if type == 'slope':
+        gradient_magnitude = np.sqrt(gradient_x**2 + gradient_y**2)
+        result = np.arctan(gradient_magnitude) * 180 / np.pi
+
+    if type == 'aspect':
+        result = np.arctan2(gradient_x, gradient_y) * 180 / np.pi + 180
+
+    # mask out values where dem has zero
+    result = result.where(dem != 0, 0)
+
+    # Assign the coordinate reference system of the original DEM to the new raster
+    result = result.rio.write_crs(dem.rio.crs)
+
+    # Save the result as a new GeoTIFF file
+    result.rio.to_raster(fname_out)
+
+
+
 def dem2slope(fname_dem):
     """
     Calculate slope from DEM and save as geotiff
 
     Parameters
     ----------
     fname_dem : str
         DEM path + file name
     """
     # Get filename
     fname = os.path.basename(fname_dem)
     # Get path for output
     path = os.path.dirname(fname_dem)
     fname_out = os.path.join(path, "Slope_" + fname)
-    gdal.DEMProcessing(fname_out, fname_dem, "slope")
+    calculate_slope_aspect(fname_dem, fname_out, type='slope')
     logging.info(f"✔  DEM slope from: {fname_dem}")
     utils.msg_success(f"DEM slope generated at: {fname_out}")
     return fname_out
 
 
 def dem2aspect(fname_dem):
     """
@@ -314,15 +363,15 @@
         DEM file name
     """
     # Get filename
     fname = os.path.basename(fname_dem)
     # Get path for output
     path = os.path.dirname(fname_dem)
     fname_out = os.path.join(path, "Aspect_" + fname)
-    gdal.DEMProcessing(fname_out, fname_dem, "aspect")
+    calculate_slope_aspect(fname_dem, fname_out, type='aspect')
     logging.info(f"✓ | DEM aspect from: {fname_dem}")
     utils.msg_success(f"Aspect (from DEM) generated at: {fname_out}")
     return fname_out
 
 
 def test_getwcs_dem(outpath="./test_DEM/"):
     """
```

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/getdata_landscape.py` & `geodata-harvester-1.1.0/src/geodata_harvester/getdata_landscape.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/getdata_radiometric.py` & `geodata-harvester-1.1.0/src/geodata_harvester/getdata_radiometric.py`

 * *Files 10% similar despite different names*

```diff
@@ -280,62 +280,7 @@
     else:
         year = int(year)
         dates = []
         for time in times:
             if datetime.fromisoformat(time[:-1]).astimezone(timezone.utc).year == year:
                 dates.append(time)
         return dates
-
-
-### Some test functions ###
-
-
-def test_get_capabilities():
-    """
-    Test script to retrieve WCS capabilities
-    """
-    # Get capabilities
-    keys, titles, descriptions, bboxs = get_capabilities()
-    assert len(keys) > 0
-
-
-def test_get_times():
-    """
-    Test script to retrieve available times for a layer
-    """
-    url = "https://gsky.nci.org.au/ows/national_geophysical_compilations?service=WCS"
-    times = get_times(url, layername)
-    assert len(times) > 0
-
-
-def test_times():
-    """
-    Check that there is only one time per layers.
-    """
-    url = "https://gsky.nci.org.au/ows/national_geophysical_compilations?service=WCS"
-    radiometricdict = get_radiometricdict()
-    layernames = radiometricdict["layernames"]
-    for key in layernames:
-        times = get_times(url, key)
-        print(f"{key}: {times}")
-        assert len(times) == 1
-
-
-def test_get_radiometric_image():
-    """
-    Test script to retrieve and save image for one layer
-    """
-    url = "https://gsky.nci.org.au/ows/national_geophysical_compilations?service=WCS"
-    # "radmap2019_grid_dose_terr_awags_rad_2019"  # for some layers readout time of 30s is exceeding (server limited)
-    layername = "radmap2019_grid_dose_terr_filtered_awags_rad_2019"
-    crs = "EPSG:4326"  # WGS84
-    # define bounding box for retrieval (simple test here for entire Australia)
-    bbox = (114, -44, 153.9, -11)
-    # define resolution (in arcsecs per pixel since crs is in WGS84)
-    resolution = 100
-    # define output file name
-    fname_out = f"test_{layername}.tif"
-    # Get data
-    download_ok = get_radiometric_image(
-        fname_out, layername, bbox, url, resolution=resolution
-    )
-    assert download_ok
```

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/getdata_silo.py` & `geodata-harvester-1.1.0/src/geodata_harvester/getdata_silo.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/getdata_slga.py` & `geodata-harvester-1.1.0/src/geodata_harvester/getdata_slga.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/harvest.py` & `geodata-harvester-1.1.0/src/geodata_harvester/harvest.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,20 @@
                 config['date_max'] = date_end_list[i].date() #.strftime("%Y-%m-%d")
                 if config['target_sources']['GEE']['preprocess']['reduce'] is None:
                     config['target_sources']['GEE']['preprocess']['reduce'] = agg_type
                 with open(tmp_config, "w") as f:
                     yaml.dump(config, f)
                 # run eeharvest
                 gee_outpath = os.path.join(settings.outpath,'ee')
-                gee = eeharvester.auto(config=tmp_config, outpath=gee_outpath)
+                try:
+                    # Try to download gee images for the time interval. If no images available, skip.
+                    gee = eeharvester.auto(config=tmp_config, outpath=gee_outpath)
+                except Exception as e:
+                    print(e)
+                    continue
                 if not isinstance(gee.filenames, list):
                     # convert to list
                     gee.filenames = [gee.filenames]
                 gee_filenames = []
                 # Walk through the directory and its subdirectories to find full paths
                 for root, _, files in os.walk(gee_outpath):
                     for file in files:
@@ -216,29 +221,30 @@
                 agg_list += [agg_type] * len(gee_filenames)
                 layer_titles += [layer + "_" + agg_type + "_" + date_start_list[i].strftime("%Y-%m-%d") + 
                 "-to-" + date_end_list[i].strftime("%Y-%m-%d") for layer in layers]
                 
                 # remove temporary config file
                 os.remove(tmp_config)
 
-        # rename outfname files to layer_titles + .tif
-        for i in range(len(outfnames)):
-            os.rename(outfnames[i], os.path.join(os.path.dirname(outfnames[i]), layer_titles[i] + ".tif"))
-            outfnames[i] = os.path.join(os.path.dirname(outfnames[i]), layer_titles[i] + ".tif")
+        if len(outfnames) > 0:
+            # rename outfname files to layer_titles + .tif
+            for i in range(len(outfnames)):
+                os.rename(outfnames[i], os.path.join(os.path.dirname(outfnames[i]), layer_titles[i] + ".tif"))
+                outfnames[i] = os.path.join(os.path.dirname(outfnames[i]), layer_titles[i] + ".tif")
 
-        download_log = update_logtable(
-            download_log,
-            outfnames,
-            layernames,
-            "GEE",
-            settings,
-            layertitles=layer_titles,
-            agfunctions=agg_list,
-            loginfos="downloaded",
-        )
+            download_log = update_logtable(
+                download_log,
+                outfnames,
+                layernames,
+                "GEE",
+                settings,
+                layertitles=layer_titles,
+                agfunctions=agg_list,
+                loginfos="downloaded",
+            )
 
     # DEA
     if "DEA" in list_sources:
         cprint("\n⌛ Downloading DEA data...", attrs=["bold"])
         # get data from DEA
         dea_layernames = settings.target_sources["DEA"]
         outpath_dea = os.path.join(settings.outpath, "dea")
@@ -254,14 +260,15 @@
             format_out="GeoTIFF",
         )
         if period_days is not None:
             # aggregate temporal data
             outfname_dea_list = []
             layer_list = []
             layer_titles = []
+            agg_list = []
             for layername in dea_layernames:
                 # get files for layername 
                 #files_layer = [os.path.basename(x) for x in files_dea if layername in x]
                 files_layer = [x for x in files_dea if layername in x]
 
                 # Check if there are multiple files for the same layer, 
                 # if not assume no temporal aggregation and skip loop
@@ -400,15 +407,16 @@
                 settings,
                 layertitles=layernames,
                 loginfos="downloaded",
             )
         else:
             pass
     if "SILO" in list_sources:
-        cprint("\n⌛ Downloading SILO data...", attrs=["bold"])
+        cprint("\n⌛ Downloading SILO data.\
+            This will take a couple of minutes, depending on your internet speed...", attrs=["bold"])
         # get data from SILO
         fnames_out_silo = []
         silo_layernames = list(settings.target_sources["SILO"].keys())
         # print(silo_layernames)
         try:
             # run the download
             files_silo = os.path.join(settings.outpath, "silo")
```

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/spatial.py` & `geodata-harvester-1.1.0/src/geodata_harvester/spatial.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/temporal.py` & `geodata-harvester-1.1.0/src/geodata_harvester/temporal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-#!/bin/python
 """
+Utility functions for temporal processing.
 
-Utility functions for for temporal processing.
-
---Function List, in order of appearence--
+--Main function list--
 
 combine_rasters_temporal: Concatenates files by time returns xarray.
 aggregate_temporal: Aggregates xarrays by specified function and time period.
+temporal_crop: Cuts an xarray object by start and end times.
+aggregate_temporal: Make a data aggregation (mean, median, sum, etc) through time on an xarray.
+
+--Helper function list--
 
+get_date_after_last_underscore: Extract the date from the file name after the last underscore.
+get_mask_array: Return mask of the data, e.g. for cloud-cover.
 """
 
 import numpy as np
 import pandas as pd
 import rioxarray
 import xarray as xr
 import datetime
@@ -74,15 +78,18 @@
                 + " Options are",
                 [t for t in xds.attrs],
             )
             return None
 
         array_list.append(xds)
         #print("attrs", xds.attrs[attribute_name])
-        attrs = attrs + xds.attrs[attribute_name]
+        try:
+            attrs = attrs + xds.attrs[attribute_name]
+        except:
+            attrs = attrs + (xds.attrs[attribute_name],)
         if first == True:
             coords = xds[channel_name].values
 
             first = False
         else:
             coords = np.append(coords, xds[channel_name].values + coords[-1])
 
@@ -201,16 +208,14 @@
         # Check for case-insensitive nodata names
         if not nodata_name_found:
             for key, value in xdr.attrs.items():
                 if key.lower() in [attr.lower() for attr in nodata_names]:
                     xdr = xdr.where(xdr != value, np.nan)
                     nodata_name_found = True
                     break
-        if not nodata_name_found:
-            print("No nodata value found in attributes. Will not fill nan values.")
 
 
     # Check the aggregation methods are okay
     agg_types = ["mean", "median", "sum", "perc95", "perc5", "max", "min"]
     aggcheck = [a for a in agg if a in agg_types]
     if aggcheck is None:
         raise ValueError("Invalid Aggregation type. Expected any of: %s" % agg_types)
@@ -294,14 +299,25 @@
 
             print(a, "of", label, "saved in:", outfile + "_" + a + "_" + label + ".tif")
 
     return outfname_list, agg_list
 
 
 def get_date_after_last_underscore(file_list):
+    """
+    Extract the date from the file name after the last underscore.
+
+    Parameters
+    ----------
+    file_list : list of filename strings in date order to concatenate.
+
+    Returns
+    -------
+    result : list of dates in date order to concatenate.
+    """
     result = []
 
     for filename in file_list:
         split_string = filename.rsplit('_', 1)  # Split the string from the right side, keeping only the last part
 
         # Check if the string was split
         if len(split_string) > 1:
@@ -363,8 +379,7 @@
             if len(mask_band) > 1:
                 if verbose: print(f"Multiple mask bands found in attributes. Proceeding with mask band: {xdr.attrs['long_name'][mask_band[0]]}")
             mask_band = mask_band[0] + 1
             if verbose: print(f"Masking values with Nan where mask band {xdr.attrs['long_name'][mask_band[0]]} is valid")
             mask = xdr.sel(band=mask_band).values != 0
 
     return mask
-
```

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/utils.py` & `geodata-harvester-1.1.0/src/geodata_harvester/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,17 @@
         meta = src.meta
 
     meta.update(dtype=rasterio.float32)
 
     # Stack all data/channels as a list of numpy arrays
     array_list = []
     for x in file_list:
-        array_list.extend(_read_file(x))
+        array_list.append(_read_file(x))
+
+    array_list = np.asarray(array_list)
 
     # Perform aggregation over channels axis
     mean_array = np.nanmean(array_list, axis=0)
     median_array = np.nanmedian(array_list, axis=0)
     sum_array = np.nansum(array_list, axis=0)
     mean_array95 = np.nanpercentile(array_list, 95, axis=0)
     mean_array5 = np.nanpercentile(array_list, 5, axis=0)
```

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/validate_settings.py` & `geodata-harvester-1.1.0/src/geodata_harvester/validate_settings.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/widgets/harvesterwidgets.py` & `geodata-harvester-1.1.0/src/geodata_harvester/widgets/harvesterwidgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import os
 import ast
 import yaml
 import sys
 import ipywidgets as widgets
 from IPython.display import display
 import datetime
+import geopandas as gpd
 from types import SimpleNamespace
 
 # import data dictionaries
 #sys.path.append("../")
 from .ipyfilechooser import FileChooser
 from geodata_harvester.getdata_slga import get_slgadict
 from geodata_harvester.getdata_silo import get_silodict
@@ -99,15 +100,15 @@
 
     Input:
         None
     
     Output:
         w_load: widget for loading settings
     """
-    w_yamlfile = FileChooser(os.getcwd(), title="Settings File:")
+    w_yamlfile = FileChooser(os.getcwd(), title="Settings File (.yaml or .yml):")
     return w_yamlfile
 
 
 def gen_maintab():
     """
     Generate New Settings Tab
 
@@ -178,15 +179,15 @@
         None
 
     Output:
         panel_io: panel for input and output settings
         w_io: widget for input path
         w_names: list of names of widgets
     """ 
-    w_inpath = FileChooser(os.getcwd(), title="Input File:")
+    w_inpath = FileChooser(os.getcwd(), title="Input File (.csv):")
 
     # Write name relative output path
     w_outpath = widgets.Text(
         value="../../dataresults/",
         placeholder="Type name of output path",
         description="Output Path:",
         disabled=False,
@@ -234,15 +235,15 @@
     Output:
         panel_st: panel for spatial-temporal settings
         settings_st: list of settings
         settings_names: list of names of settings
     """
     w_target_bbox = widgets.Text(
         value="",
-        placeholder="[Lng_min, Lat_min, Lng_max, Lat_max]",
+        placeholder="[Long_min, Lat_min, Long_max, Lat_max]",
         description="",
         disabled=False,
     )
 
     w_target_res = widgets.FloatSlider(
         value=3,
         min=0.3,
@@ -261,15 +262,15 @@
     disabled=False
 )
     w_date_max = widgets.DatePicker(
     description='',
     disabled=False
 )
 
-    w_temp_intervals = widgets.IntSlider(
+    w_time_intervals = widgets.IntSlider(
         value=1,
         min=1,
         max=365,
         step=1,
         description="",
         disabled=False,
         continuous_update=False,
@@ -291,23 +292,23 @@
         slider_color="white",
     )
 
     items = [
         widgets.GridBox([widgets.Label("Bounding Box :"), w_target_bbox], layout=widgets.Layout(grid_template_columns="1fr 2fr")),
         widgets.GridBox([widgets.Label("Spatial Resolution [arcsec]:"), w_target_res], layout=widgets.Layout(grid_template_columns="1fr 2fr")),
         widgets.GridBox([widgets.Label(f"Start Date:".rjust(2)), w_date_min], layout=widgets.Layout(grid_template_columns="1fr 2fr")),
-        widgets.GridBox([widgets.Label(f"Number of Temporal Slices:".rjust(3)), w_temp_intervals], layout=widgets.Layout(grid_template_columns="1fr 2fr")),
+        widgets.GridBox([widgets.Label(f"Number of Temporal Slices:".rjust(3)), w_time_intervals], layout=widgets.Layout(grid_template_columns="1fr 2fr")),
         widgets.GridBox([widgets.Label(f"End Date:".rjust(4)), w_date_max], layout=widgets.Layout(grid_template_columns="1fr 2fr")),
         widgets.GridBox([widgets.Label(f"Temporal Buffer Window in Days:"), w_temp_buffer], layout=widgets.Layout(grid_template_columns="1fr 2fr")),
         # widgets.Box([widgets.Label("Select years:"), w_target_dates]),
         # widgets.Box([widgets.Label("Temporal Resolution [days]:"), w_temp_res]),
         ]
 
-    settings_st = [w_target_bbox, w_target_res, w_date_min, w_temp_intervals, w_date_max, w_temp_buffer]
-    settings_names = ["target_bbox", "target_res", "date_min", "temp_intervals", "date_max", "temp_buffer"]
+    settings_st = [w_target_bbox, w_target_res, w_date_min, w_time_intervals, w_date_max, w_temp_buffer]
+    settings_names = ["target_bbox", "target_res", "date_min", "time_intervals", "date_max", "temp_buffer"]
     panel_st = widgets.GridBox(
         items, layout=widgets.Layout(grid_template_columns="6fr 6fr")
     )
     return panel_st, settings_st, settings_names
 
 
 def gen_panel_slga():
@@ -367,18 +368,18 @@
     box_silo = []
     for i in range(len(options_silo)):
         option = options_silo[i]
         desc = desc_silo[i]
         w_sel = widgets.Checkbox(
             value=False, description=option, disabled=False, indent=False
         )
-        w_temp = widgets.SelectMultiple(
+        w_temp = widgets.Select(
             # options=['Total','Median','Mean','Std','5pct','10pct','15pct','25pct','75pct','85pct','90pct','95pct'],
             options=["mean", "median", "sum", "std", "perc95", "perc5", "max", "min"],
-            value=["median"],
+            value="median",
             rows=2,
             description="",
             disabled=False,
         )
         w_silo.append([w_sel, w_temp])
         items = [
             w_sel,
@@ -745,29 +746,31 @@
     assert len(names_io) == len(w_io)
     for i in range(len(w_io)):
         dict_settings[names_io[i]] = w_io[i].value
     # ST settings
     assert len(names_st) == len(w_st)
     for i in range(len(w_st)):
         dict_settings[names_st[i]] = w_st[i].value
+    # correct potential floating error
+    dict_settings["target_res"] = round(dict_settings["target_res"], 4)
     # target sources settings
     # define for target source a dictionary
     # Loop over all settings and add the ones that are selected
     dict_sources = {}
     # SLGA
     slist = {}
     for i in range(len(w_slga)):
         if w_slga[i][0].value:
             slist[names_slga[i]] = list(w_slga[i][1].value)
     dict_sources["SLGA"] = slist
     # SILO
     slist = {}
     for i in range(len(w_silo)):
         if w_silo[i][0].value:
-            slist[names_silo[i]] = list(w_silo[i][1].value)
+            slist[names_silo[i]] = w_silo[i][1].value
     dict_sources["SILO"] = slist
     # DEA
     slist = []
     for i in range(len(w_dea)):
         if w_dea[i][0].value:
             # slist.append({names_dea[i]: list(w_dea[i][1].value)})
             slist.append(names_dea[i])
@@ -827,15 +830,22 @@
     dict_sources["GEE"] = slist
     # Add here any new settings or data sources
     dict_settings["target_sources"] = dict_sources
 
     # Check bounding box:
     if type(dict_settings["target_bbox"]) == str:
         # remove string from list
+        if dict_settings["target_bbox"] == "":
+             # set bounding box around input data with padding +/- 0.05 deg
+            gdfpoints = gpd.read_file(dict_settings["infile"])
+            longs = gdfpoints[dict_settings["colname_lng"]].astype(float)
+            lats = gdfpoints[dict_settings["colname_lat"]].astype(float)
+            dict_settings["target_bbox"] = f"[{min(longs) - 0.05},{min(lats) - 0.05},{max(longs) + 0.05},{max(lats) + 0.05}]"
         dict_settings["target_bbox"] = ast.literal_eval(dict_settings["target_bbox"])
+
     return dict_settings
 
 
 def print_settings(settings):
     """
     print settings
```

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/errors.py` & `geodata-harvester-1.1.0/src/geodata_harvester/widgets/ipyfilechooser/errors.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/filechooser.py` & `geodata-harvester-1.1.0/src/geodata_harvester/widgets/ipyfilechooser/filechooser.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipyfilechooser/utils.py` & `geodata-harvester-1.1.0/src/geodata_harvester/widgets/ipyfilechooser/utils.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/widgets/ipywidgets_file_selector.py` & `geodata-harvester-1.1.0/src/geodata_harvester/widgets/ipywidgets_file_selector.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester/write_logs.py` & `geodata-harvester-1.1.0/src/geodata_harvester/write_logs.py`

 * *Files identical despite different names*

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester.egg-info/PKG-INFO` & `geodata-harvester-1.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: geodata-harvester
-Version: 1.0.1
-Summary: An automation tool for harvesting and processing geodata from the web
-Home-page: https://github.com/Sydney-Informatics-Hub/geodata-harvester
-License: LGPL-3.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Geodata-Harvester
 
 <h3><em>Automate geodata harvesting from the web and jumpstart your analysis with a ready-made set of spatiotemporal processed maps and data tables.</em></h3> 
 
 <center><a><img src="quarto/images/dataharvester_logo.png" alt="Geodata-Harvester logo" width="100%"/></a></center>
 
 
@@ -39,16 +27,18 @@
 - [Key Features](#-key-features)
 - [Installation](#-installation)
     - [Conda or Mamba](#conda-or-mamba)
     - [PyPI](#pypi)
     - [Google Earth Engine extension](#google-earth-engine-extension)
     - [Local development](#local-development)
     - [Workshop Cloud Sandbox](#workshop-cloud-sandbox)
+- [Settings Overview](#-settings-overview)
 - [How to get started](#-how-to-get-started)
 - [How to add new data source modules](#-how-to-add-new-data-source-modules)
+- [Testing](#-testing)
 - [Code reference API](#-code-reference-api)
 - [Contributions](#-contributions)
 - [Attribution and Acknowledgments](#-attribution-and-acknowledgments)
 - [License](#-license)
 
 
 ## 💡 Introduction
@@ -67,40 +57,38 @@
 - SILO Climate Database
 - National Digital Elevation Model (DEM) 1 Second Hydrologically Enforced
 - Digital Earth Australia (DEA) Geoscience Earth Observations
 - GSKY Data Server for DEA Geoscience Earth Observations
 - Radiometric Data
 - Google Earth Engine Data (GEE account needed), see for overview [Earth_Engine_Data_Overview](quarto/docs/Earth_Engine_Data_Overview.md).
 
-## Functionality
+## 🔄 Functionality
 
 The main goal of the Data Harvester is to enable researchers with reusable workflows for automatic data extraction and processing:
 
 1. Retrieve: given set of locations, automatically access and download multiple data sources (APIs) from a diverse range of geospatial and soil data sources
 2. Process: Spatial and temporal processing, conversion to dataframes and custom raster-files
 3. Output: Ready-made dataset for machine learning (training set and prediction mapping)
 
 Geodata-Harvester is designed as a modular and maintainable project in the form of a multi-stage pipeline by providing explicit boundaries among tasks. To encourage interaction and experimentation with the pipeline, multiple frontend notebooks and use case scenarios are provided.
 
 ## 🌟 Key Features
 
-Below is a list of features available for the geodata-harvester package. Please check the project Github webpage and notebooks for examples, data selection, and other settings.
+The geodata-harvester package provides the following core features:
 
-- enabling reproducible workflows via YAML settings files.
-- automatic data retrieval from geodata APIs for given locations and dates.
-- automatic download and spatiotemporal processing of geo-spatial maps for user-specified bounding box, resolution, and time-scale.
-- support for time-series data extraction for multiple time slices. 
-- automatic extraction of retrieved data into ready-made dataframes for ML training.
-- automatic generation of ready-made aligned maps in GeoTiff format.
-- preview of downloaded and aligned maps.
-- support for saving and loading settings via interactive widgets.
-- with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices.
-- example notebooks and use-cases are provided for the user to get started.
+- enabling reproducible workflows via YAML settings files (see for settings example [settings_harvest.yaml](notebooks/settings/settings_harvest.yaml)).
+- interactive widgets for settings selection (see for example notebook [example_harvest_with_widgets.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_with_widgets.ipynb)).
+- automated download and processing pipeline for multiple data sources (supported by the `harvest.run()` function as demonstrated in the example notebook [example_harvest.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest.ipynb)).
+- automatic data retrieval from geodata APIs and spatiotemporal processing for given locations, bounding box, resoultion, and time-scales into ready-made aligned and geo-referenced maps in GeoTiff format (see [notebook API download and process step](https://nbviewer.jupyter.org/github/Sydney-Informatics-Hub/geodata-harvester/blob/main/notebooks/example_harvest_stepwise.ipynb#Download-and-process-data-from-API-sources)).
+- support for time-series data extraction for multiple time slices (see example notebook [example_harvest_temporal1.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_temporal1.ipynb) and [example_harvest_temporal2.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_temporal2.ipynb)). 
+- automatic extraction of retrieved data into ready-made dataframes for ML training ([see notebook point extraction process](https://nbviewer.jupyter.org/github/Sydney-Informatics-Hub/geodata-harvester/blob/main/notebooks/example_harvest_stepwise.ipynb#Points-extraction-from-downloaded/processed-data))).
+- preview of downloaded and aligned maps (see [notebook preview example](https://nbviewer.jupyter.org/github/Sydney-Informatics-Hub/geodata-harvester/blob/main/notebooks/example_harvest_stepwise.ipynb#Overview-plot-of-all-processed-rasters)).
+- with connectivity support to the Google Earth Engine API, perform petabyte-scale operations which include temporal cloud/shadow masking and automatic calculation of spectral indices (see pipeline notebook [example_harvest_withGEE.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_withGEE.ipynb)) or the [step-by-step GEE process instructions](https://nbviewer.jupyter.org/github/Sydney-Informatics-Hub/geodata-harvester/blob/main/notebooks/example_harvest_stepwise.ipynb#Google-Earth-Engine).
 
-For more features, please see the [API reference documentation](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
+For more details about all functionalities, please consult the [API reference documentation](https://sydney-informatics-hub.github.io/geodata-harvester/API/geodata_harvester/index.html).
 
 ## 🔧 Installation
 
 Geodata-Harvester can be run on cloud-servers (e.g., in JupyterHub environment) or on your local machine. 
 Example notebooks for importing and using the package can be found in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks). The package can be installed via PyPI or Conda:
 
 ### Conda or Mamba
@@ -150,33 +138,65 @@
 
 As play-ground for workshop training sessions and testing of the Geodata-Harvester we provide a pre-installed cloud Python Jupyterlab environment, which does not require any local installation. For login instructions and how to access the sandbox, please visit our [Python workshop page](https://sydney-informatics-hub.github.io/AgReFed-Workshop/pydocs/py00-workshop.html).
 
 The Jupyter environment is hosted on the ARDC Nectar Research Cloud in partnership with AgReFed and Australian Research Data Commons (ARDC). Note that this sandbox is currently hosted for test purposes only and generated data is not permanently stored.
 
 The Geodata-Harvester can be easily installed also on other cloud services (e.g., Google Colab, Azure Notebooks).
 
+## ⚙️ Settings Overview
+
+The Geodata-Harvester is controlled by a settings file in YAML format. The settings file contains all user-defined settings for the data extraction and processing. A detailed settings overview is provided in [Settings_Overview](quarto/docs/Settings_Overview.md). Example settings files are provided along the notebooks in the folder [notebooks/settings](notebooks/settings).  
+
+Alternatively a settings file can be also created via the interactive widget-panels as demonstrated in the notebook [example_harvest_with_widgets.ipynb](notebooks/example_harvest_with_widgets.ipynb).
+
 
 ## 🚀 How to get started
 
 You may now invoke the geodata-harvester directly from a python terminal with:
 
 ```python
 import geodata_harvester as gdh
 gdh.harvest.run(PATH_TO_SETTINGS_YAMLFILE)
 ```
 
 **Note the subtle but important difference in use of an underscore `_` to import the package and the use of a dash `-` to install it!**
 
 To get started, some example workflows are provided as Jupyter notebooks:
 
-1. Options and user settings are defined by the user in the settings; see for settings documentation [Settings_Overview](quarto/docs/Settings_Overview.md)
+1. Clone the geodata-harvester repo to your local machine or cloud server. Alternatively, download the package as zip folder from the [geodata-harvester Github page](https://github.com/Sydney-Informatics-Hub/geodata-harvester/archive/refs/heads/main.zip) and unzip the folder. This will download the geodata-harvester package including the example notebooks, settings files and example input data.
+
+2. Options and user settings are defined by the user in the settings; see for example settings file [settings_harvest.yaml](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/settings/settings_harvest.yaml)
+
+3. Run a jupyter notebook in the notebooks folder, such as  [example_harvest.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest.ipynb).
+
+4. The notebook will run the geodata-harvester with the settings file and download/process all the requested data. The final data is saved in the folder `results_example_harvest` in the current working directory as specified in the settings file. There you can find the generated data table `results.csv` and the downloaded georeferenced .tif files (open with, e.g., rasterio, QGIS or ArcGIS). A summary of all generated images is provided in the table `download_summary.csv`.
+
+A step-by-step tutorial on how to use the individual modules of the Geodata-Harvester is provided in the notebook [example_harvest_stepwise.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_stepwise.ipynb).
+
+To include Google Earth Engine (GEE) data in Geodata-Harvester, please follow the instructions in the notebook [example_harvest_withGEE.ipynb](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks/example_harvest_withGEE.ipynb). Note that this requires a GEE account and authorisation (see [Google Earth Engine extension](#google-earth-engine-extension)).
 
-2. Run the jupyter notebook in the folder [notebooks](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/notebooks).
+If you would like to learn more about the Geodata-Harvester, please also visit our [Workshop webpage](https://sydney-informatics-hub.github.io/AgReFed-Workshop/).
+
+## ✅ Testing
+
+Test functions are included in the [tests](https://github.com/Sydney-Informatics-Hub/geodata-harvester/tree/main/tests) folder. Note that due to the nature of this package, these tests require an internet connection and may fail if the data source API servers are not available or the data source API has changed. To run automated tests with `pytest`, you need to install the package with
+```bash
+pip install pytest
+```
+and then run:
+```bash
+cd tests
+pytest ./
+```
+or test individual modules with, e.g.,
+```bash
+cd tests
+pytest test_getdata_dea.py
+```
 
-If you would like to learn more about the Geodata-Harvester, please visit our [Workshop webpage](https://sydney-informatics-hub.github.io/AgReFed-Workshop/).
 
 ## ➕ How to add new data source modules
 
 The Geodata-Harvester is designed to be extendable and new data source modules can be added as Python modules (for examples, see `getdata_*.py` modules). If you would like to add a new data source, please follow the [adding new data source guidelines](quarto/docs/How_to_add_DataSources.md)  
 
 We recommend to fork the geodata-harvester repo and develop new modules in a local environment. If you would like to contribute your data source module to the geodata-harvester package, please visit the [geodata-harvester contribution guidelines](quarto/docs/Contributing.md).
```

### Comparing `geodata-harvester-1.0.1/src/geodata_harvester.egg-info/SOURCES.txt` & `geodata-harvester-1.1.0/src/geodata_harvester.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,8 +23,12 @@
 src/geodata_harvester.egg-info/top_level.txt
 src/geodata_harvester/widgets/__init__.py
 src/geodata_harvester/widgets/harvesterwidgets.py
 src/geodata_harvester/widgets/ipywidgets_file_selector.py
 src/geodata_harvester/widgets/ipyfilechooser/__init__.py
 src/geodata_harvester/widgets/ipyfilechooser/errors.py
 src/geodata_harvester/widgets/ipyfilechooser/filechooser.py
-src/geodata_harvester/widgets/ipyfilechooser/utils.py
+src/geodata_harvester/widgets/ipyfilechooser/utils.py
+tests/test_getdata_dea.py
+tests/test_getdata_radiometric.py
+tests/test_getdata_silo.py
+tests/test_harvest.py
```

