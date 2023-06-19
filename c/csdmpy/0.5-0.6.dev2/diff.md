# Comparing `tmp/csdmpy-0.5.tar.gz` & `tmp/csdmpy-0.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdmpy-0.5.tar", last modified: Sat Jul  9 21:57:21 2022, max compression
+gzip compressed data, was "csdmpy-0.6.dev2.tar", last modified: Mon Jun 19 22:16:24 2023, max compression
```

## Comparing `csdmpy-0.5.tar` & `csdmpy-0.6.dev2.tar`

### file list

```diff
@@ -1,165 +1,167 @@
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.342937 csdmpy-0.5/
--rw-r--r--   0 deepansh   (501) staff       (20)     6649 2022-07-09 21:55:19.000000 csdmpy-0.5/CHANGELOG
--rw-r--r--   0 deepansh   (501) staff       (20)     1519 2020-06-23 22:39:49.000000 csdmpy-0.5/LICENSE
--rw-r--r--   0 deepansh   (501) staff       (20)      309 2020-06-23 22:39:49.000000 csdmpy-0.5/MANIFEST.in
--rw-r--r--   0 deepansh   (501) staff       (20)    10587 2022-07-09 21:57:21.343669 csdmpy-0.5/PKG-INFO
--rw-r--r--   0 deepansh   (501) staff       (20)     8741 2022-07-09 21:55:19.000000 csdmpy-0.5/README.md
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.170920 csdmpy-0.5/csdmpy/
--rw-r--r--   0 deepansh   (501) staff       (20)     9922 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/__init__.py
--rw-r--r--   0 deepansh   (501) staff       (20)      352 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/__main__.py
--rw-r--r--   0 deepansh   (501) staff       (20)     2862 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/abstract_list.py
--rw-r--r--   0 deepansh   (501) staff       (20)    59492 2022-07-09 21:55:19.000000 csdmpy-0.5/csdmpy/csdm.py
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.176853 csdmpy-0.5/csdmpy/dependent_variable/
--rw-r--r--   0 deepansh   (501) staff       (20)    27612 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dependent_variable/__init__.py
--rw-r--r--   0 deepansh   (501) staff       (20)    10966 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dependent_variable/base_class.py
--rw-r--r--   0 deepansh   (501) staff       (20)     2147 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dependent_variable/decoder.py
--rw-r--r--   0 deepansh   (501) staff       (20)     2802 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dependent_variable/download.py
--rw-r--r--   0 deepansh   (501) staff       (20)     1805 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dependent_variable/external.py
--rw-r--r--   0 deepansh   (501) staff       (20)     2096 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dependent_variable/internal.py
--rw-r--r--   0 deepansh   (501) staff       (20)     5120 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dependent_variable/sparse.py
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.181714 csdmpy-0.5/csdmpy/dimension/
--rw-r--r--   0 deepansh   (501) staff       (20)    29252 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dimension/__init__.py
--rw-r--r--   0 deepansh   (501) staff       (20)     3829 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dimension/base.py
--rw-r--r--   0 deepansh   (501) staff       (20)     3919 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dimension/labeled.py
--rw-r--r--   0 deepansh   (501) staff       (20)    10092 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dimension/linear.py
--rw-r--r--   0 deepansh   (501) staff       (20)     7904 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dimension/monotonic.py
--rw-r--r--   0 deepansh   (501) staff       (20)     6388 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/dimension/quantitative.py
--rw-r--r--   0 deepansh   (501) staff       (20)    18300 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/helper_functions.py
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.182629 csdmpy-0.5/csdmpy/numpy_wrapper/
--rw-r--r--   0 deepansh   (501) staff       (20)     4574 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/numpy_wrapper/__init__.py
--rw-r--r--   0 deepansh   (501) staff       (20)     5366 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/numpy_wrapper/apodize.py
--rw-r--r--   0 deepansh   (501) staff       (20)     4165 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/statistics.py
--rw-r--r--   0 deepansh   (501) staff       (20)      352 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/tests.py
--rw-r--r--   0 deepansh   (501) staff       (20)     8074 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/units.py
--rw-r--r--   0 deepansh   (501) staff       (20)    10188 2022-07-09 01:12:01.000000 csdmpy-0.5/csdmpy/utils.py
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.172622 csdmpy-0.5/csdmpy.egg-info/
--rw-r--r--   0 deepansh   (501) staff       (20)    10587 2022-07-09 21:57:20.000000 csdmpy-0.5/csdmpy.egg-info/PKG-INFO
--rw-r--r--   0 deepansh   (501) staff       (20)     4319 2022-07-09 21:57:20.000000 csdmpy-0.5/csdmpy.egg-info/SOURCES.txt
--rw-r--r--   0 deepansh   (501) staff       (20)        1 2022-07-09 21:57:20.000000 csdmpy-0.5/csdmpy.egg-info/dependency_links.txt
--rw-r--r--   0 deepansh   (501) staff       (20)      104 2022-07-09 21:57:20.000000 csdmpy-0.5/csdmpy.egg-info/requires.txt
--rw-r--r--   0 deepansh   (501) staff       (20)        7 2022-07-09 21:57:20.000000 csdmpy-0.5/csdmpy.egg-info/top_level.txt
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.191452 csdmpy-0.5/docs/
--rw-r--r--   0 deepansh   (501) staff       (20)     6148 2021-05-07 11:54:04.000000 csdmpy-0.5/docs/.DS_Store
--rw-r--r--   0 deepansh   (501) staff       (20)    53248 2022-07-04 09:23:08.000000 csdmpy-0.5/docs/.coverage
--rw-r--r--   0 deepansh   (501) staff       (20)     2599 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/CSD_model.rst
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.195495 csdmpy-0.5/docs/CSDmodel_uml/
--rw-r--r--   0 deepansh   (501) staff       (20)     6148 2019-07-25 14:55:02.000000 csdmpy-0.5/docs/CSDmodel_uml/.DS_Store
--rw-r--r--   0 deepansh   (501) staff       (20)     1501 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/CSDmodel_uml/csdm.rst
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.197904 csdmpy-0.5/docs/CSDmodel_uml/dependent_variables/
--rw-r--r--   0 deepansh   (501) staff       (20)     2249 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/CSDmodel_uml/dependent_variables/dependent_variable.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      787 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/CSDmodel_uml/dependent_variables/external.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     1436 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/CSDmodel_uml/dependent_variables/internal.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     1745 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/CSDmodel_uml/dependent_variables/sparse_sampling.rst
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.199737 csdmpy-0.5/docs/CSDmodel_uml/dimensions/
--rw-r--r--   0 deepansh   (501) staff       (20)     1424 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/CSDmodel_uml/dimensions/dimension.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     1145 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/CSDmodel_uml/dimensions/labeled.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     3526 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/CSDmodel_uml/dimensions/linear.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     2289 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/CSDmodel_uml/dimensions/monotonic.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     3761 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/CSDmodel_uml/enumeration.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      348 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/CSDmodel_uml/scalarQuantity.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      709 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/Makefile
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.200229 csdmpy-0.5/docs/_images/
--rw-r--r--   0 deepansh   (501) staff       (20)     6148 2021-05-06 13:27:37.000000 csdmpy-0.5/docs/_images/.DS_Store
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.206505 csdmpy-0.5/docs/_static/
--rw-r--r--   0 deepansh   (501) staff       (20)     6148 2020-06-23 22:36:23.000000 csdmpy-0.5/docs/_static/.DS_Store
--rw-r--r--   0 deepansh   (501) staff       (20)     1622 2021-04-09 14:10:50.000000 csdmpy-0.5/docs/_static/button.css
--rw-r--r--   0 deepansh   (501) staff       (20)   376691 2022-07-09 21:55:19.000000 csdmpy-0.5/docs/_static/csdm.png
--rw-r--r--   0 deepansh   (501) staff       (20)    16811 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/_static/csdmpy.png
--rw-r--r--   0 deepansh   (501) staff       (20)     8143 2021-04-09 14:10:50.000000 csdmpy-0.5/docs/_static/style.css
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.208861 csdmpy-0.5/docs/_templates/
--rw-r--r--   0 deepansh   (501) staff       (20)     6148 2021-05-07 11:54:04.000000 csdmpy-0.5/docs/_templates/.DS_Store
--rw-r--r--   0 deepansh   (501) staff       (20)     1766 2021-04-09 14:10:50.000000 csdmpy-0.5/docs/_templates/layout.html
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.215235 csdmpy-0.5/docs/api/
--rw-r--r--   0 deepansh   (501) staff       (20)     6148 2021-05-07 08:42:55.000000 csdmpy-0.5/docs/api/.DS_Store
--rw-r--r--   0 deepansh   (501) staff       (20)     2345 2022-07-09 21:55:19.000000 csdmpy-0.5/docs/api/CSDM.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     1638 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/api/DependentVariable.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     2025 2021-04-09 14:10:50.000000 csdmpy-0.5/docs/api/Dimensions.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     1448 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/api/csdmpy.rst
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.216692 csdmpy-0.5/docs/api/dimension/
--rw-r--r--   0 deepansh   (501) staff       (20)      149 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/api/dimension/labeled.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      145 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/api/dimension/linear.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      157 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/api/dimension/monotonic.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      123 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/api/numpy_wrappers.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      517 2021-05-07 15:45:58.000000 csdmpy-0.5/docs/api/plotting_function.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      321 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/api/statistics.rst
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.219352 csdmpy-0.5/docs/api/wrappers/
--rw-r--r--   0 deepansh   (501) staff       (20)      827 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/api/wrappers/apodization.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     8499 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/api/wrappers/element_wise_operation.rst
--rw-r--r--   0 deepansh   (501) staff       (20)       57 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/changelog.rst
--rw-r--r--   0 deepansh   (501) staff       (20)    11195 2022-07-09 16:43:43.000000 csdmpy-0.5/docs/conf.py
--rw-r--r--   0 deepansh   (501) staff       (20)     7374 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/getting_started.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     5955 2022-07-09 21:55:19.000000 csdmpy-0.5/docs/index.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     1827 2020-07-25 22:12:57.000000 csdmpy-0.5/docs/installation.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      797 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/make.bat
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.222245 csdmpy-0.5/docs/plotting_with_pyplot/
--rw-r--r--   0 deepansh   (501) staff       (20)      866 2020-07-25 22:12:57.000000 csdmpy-0.5/docs/plotting_with_pyplot/one_D_plots.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      892 2020-07-25 22:12:57.000000 csdmpy-0.5/docs/plotting_with_pyplot/two_D_plots.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      322 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/referenceAPI.rst
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.233727 csdmpy-0.5/docs/startFromScratch/
--rw-r--r--   0 deepansh   (501) staff       (20)     2925 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/startFromScratch/A fun example.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     2628 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/startFromScratch/add_dependent_variable_object.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     1896 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/startFromScratch/add_dimension_object.rst
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.159222 csdmpy-0.5/docs/startFromScratch/dimension/
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.238793 csdmpy-0.5/docs/startFromScratch/dimension/generate/
--rw-r--r--   0 deepansh   (501) staff       (20)      198 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/startFromScratch/dimension/generate/dimension_objects.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      918 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/startFromScratch/dimension/generate/labeled.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     2853 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/startFromScratch/dimension/generate/linear.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     2527 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/startFromScratch/dimension/generate/monotonic.rst
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.245903 csdmpy-0.5/docs/startFromScratch/dimension/interact/
--rw-r--r--   0 deepansh   (501) staff       (20)      158 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/startFromScratch/dimension/interact/dimension_objects.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     6093 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/startFromScratch/dimension/interact/linear.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     4434 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/startFromScratch/dimension/interact/monotonic.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     4647 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/startFromScratch/generating_csdm_object.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     5837 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/startFromScratch/generating_dependent_variable_object.rst
--rw-r--r--   0 deepansh   (501) staff       (20)    11628 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/startFromScratch/interacting_with_csdm.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      195 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/startFromScratch/interacting_with_csdmpy_objects.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     3265 2022-07-09 01:12:01.000000 csdmpy-0.5/docs/startFromScratch/save_dataset.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      494 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/startFromScratch/start.rst
--rw-r--r--   0 deepansh   (501) staff       (20)     1326 2020-06-23 22:39:50.000000 csdmpy-0.5/docs/using_csdm_with_pyplot.rst
--rw-r--r--   0 deepansh   (501) staff       (20)      174 2020-06-23 22:39:50.000000 csdmpy-0.5/pyproject.toml
--rw-r--r--   0 deepansh   (501) staff       (20)      427 2021-04-09 14:10:50.000000 csdmpy-0.5/requirements-dev.txt
--rw-r--r--   0 deepansh   (501) staff       (20)      174 2021-04-09 14:10:50.000000 csdmpy-0.5/requirements.txt
--rw-r--r--   0 deepansh   (501) staff       (20)      352 2022-07-09 21:57:21.344651 csdmpy-0.5/setup.cfg
--rw-r--r--   0 deepansh   (501) staff       (20)     2321 2022-07-09 01:12:01.000000 csdmpy-0.5/setup.py
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.270571 csdmpy-0.5/tests/
--rw-r--r--   0 deepansh   (501) staff       (20)     6148 2022-07-09 21:02:58.000000 csdmpy-0.5/tests/.DS_Store
--rw-r--r--   0 deepansh   (501) staff       (20)     4404 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/csdm_indexing_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)     1125 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/csdm_new_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)    17957 2022-07-09 21:55:19.000000 csdmpy-0.5/tests/csdm_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)     8789 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/dependent_variable_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)    23240 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/dimension_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)     3735 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/fft_test.py
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.273007 csdmpy-0.5/tests/file_read/
--rw-r--r--   0 deepansh   (501) staff       (20)     6148 2021-05-06 18:55:00.000000 csdmpy-0.5/tests/file_read/.DS_Store
--rw-r--r--   0 deepansh   (501) staff       (20)     3070 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/file_read/fileread_test.py
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.332818 csdmpy-0.5/tests/file_read/test_files/
--rw-r--r--   0 deepansh   (501) staff       (20)     6148 2021-05-06 15:57:45.000000 csdmpy-0.5/tests/file_read/test_files/.DS_Store
--rw-r--r--   0 deepansh   (501) staff       (20)      750 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/1.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      773 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/10.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      788 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/11.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      715 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/12.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      716 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/13.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      713 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/14.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      711 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/15.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      511 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/16.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      728 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/2.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      752 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/3.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      750 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/4.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      878 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/5.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      876 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/6.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      879 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/7.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      852 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/8.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)      802 2021-05-07 15:45:58.000000 csdmpy-0.5/tests/file_read/test_files/9.csdfe
--rw-r--r--   0 deepansh   (501) staff       (20)     2295 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/import_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)     1327 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/nmr_freq_test.py
-drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2022-07-09 21:57:21.340068 csdmpy-0.5/tests/numpy_wrapper/
--rw-r--r--   0 deepansh   (501) staff       (20)     3539 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/numpy_wrapper/apodization_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)     1930 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/numpy_wrapper/change_shape_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)     4070 2022-07-09 21:55:19.000000 csdmpy-0.5/tests/numpy_wrapper/dimension_reduction_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)     5842 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/numpy_wrapper/element_wise_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)      883 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/save_file_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)      903 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/serialization_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)     2029 2022-07-09 21:55:19.000000 csdmpy-0.5/tests/sparse_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)     2166 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/statistics_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)     1631 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/unit_test.py
--rw-r--r--   0 deepansh   (501) staff       (20)     3205 2022-07-09 01:12:01.000000 csdmpy-0.5/tests/utils_test.py
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.914766 csdmpy-0.6.dev2/
+-rw-r--r--   0 deepansh   (501) staff       (20)     7403 2023-06-19 13:54:12.000000 csdmpy-0.6.dev2/CHANGELOG
+-rw-r--r--   0 deepansh   (501) staff       (20)     1519 2020-06-23 22:39:49.000000 csdmpy-0.6.dev2/LICENSE
+-rw-r--r--   0 deepansh   (501) staff       (20)      309 2020-06-23 22:39:49.000000 csdmpy-0.6.dev2/MANIFEST.in
+-rw-r--r--   0 deepansh   (501) staff       (20)     9445 2023-06-19 22:16:24.914971 csdmpy-0.6.dev2/PKG-INFO
+-rw-r--r--   0 deepansh   (501) staff       (20)     8458 2023-05-07 13:07:00.000000 csdmpy-0.6.dev2/README.md
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.694921 csdmpy-0.6.dev2/csdmpy/
+-rw-r--r--   0 deepansh   (501) staff       (20)     9498 2023-06-19 13:54:12.000000 csdmpy-0.6.dev2/csdmpy/__init__.py
+-rw-r--r--   0 deepansh   (501) staff       (20)      352 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/csdmpy/__main__.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     2862 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/csdmpy/abstract_list.py
+-rw-r--r--   0 deepansh   (501) staff       (20)    62475 2023-06-19 13:54:12.000000 csdmpy-0.6.dev2/csdmpy/csdm.py
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.708795 csdmpy-0.6.dev2/csdmpy/dependent_variable/
+-rw-r--r--   0 deepansh   (501) staff       (20)    26662 2023-06-19 13:54:12.000000 csdmpy-0.6.dev2/csdmpy/dependent_variable/__init__.py
+-rw-r--r--   0 deepansh   (501) staff       (20)    10965 2022-07-27 23:27:45.000000 csdmpy-0.6.dev2/csdmpy/dependent_variable/base_class.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     2179 2022-09-24 12:45:46.000000 csdmpy-0.6.dev2/csdmpy/dependent_variable/decoder.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     2802 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/csdmpy/dependent_variable/download.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     1805 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/csdmpy/dependent_variable/external.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     2114 2022-07-27 23:57:36.000000 csdmpy-0.6.dev2/csdmpy/dependent_variable/internal.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     4882 2022-09-24 12:45:46.000000 csdmpy-0.6.dev2/csdmpy/dependent_variable/sparse.py
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.717848 csdmpy-0.6.dev2/csdmpy/dimension/
+-rw-r--r--   0 deepansh   (501) staff       (20)    30278 2023-06-19 13:54:12.000000 csdmpy-0.6.dev2/csdmpy/dimension/__init__.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     3942 2023-05-15 22:44:58.000000 csdmpy-0.6.dev2/csdmpy/dimension/base.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     3918 2022-09-24 12:45:46.000000 csdmpy-0.6.dev2/csdmpy/dimension/labeled.py
+-rw-r--r--   0 deepansh   (501) staff       (20)    10284 2023-06-19 22:11:53.000000 csdmpy-0.6.dev2/csdmpy/dimension/linear.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     8099 2022-10-05 00:34:42.000000 csdmpy-0.6.dev2/csdmpy/dimension/monotonic.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     6386 2022-07-27 23:27:45.000000 csdmpy-0.6.dev2/csdmpy/dimension/quantitative.py
+-rw-r--r--   0 deepansh   (501) staff       (20)    18297 2023-06-18 23:44:56.000000 csdmpy-0.6.dev2/csdmpy/helper_functions.py
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.720709 csdmpy-0.6.dev2/csdmpy/numpy_wrapper/
+-rw-r--r--   0 deepansh   (501) staff       (20)     6210 2023-06-19 13:54:12.000000 csdmpy-0.6.dev2/csdmpy/numpy_wrapper/__init__.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     5358 2023-06-19 13:54:12.000000 csdmpy-0.6.dev2/csdmpy/numpy_wrapper/apodize.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     4165 2023-06-18 23:44:56.000000 csdmpy-0.6.dev2/csdmpy/statistics.py
+-rw-r--r--   0 deepansh   (501) staff       (20)      352 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/csdmpy/tests.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     8051 2023-06-18 23:44:56.000000 csdmpy-0.6.dev2/csdmpy/units.py
+-rw-r--r--   0 deepansh   (501) staff       (20)    11943 2023-06-19 13:54:12.000000 csdmpy-0.6.dev2/csdmpy/utils.py
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.699097 csdmpy-0.6.dev2/csdmpy.egg-info/
+-rw-r--r--   0 deepansh   (501) staff       (20)     9445 2023-06-19 22:16:24.000000 csdmpy-0.6.dev2/csdmpy.egg-info/PKG-INFO
+-rw-r--r--   0 deepansh   (501) staff       (20)     4398 2023-06-19 22:16:24.000000 csdmpy-0.6.dev2/csdmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 deepansh   (501) staff       (20)        1 2023-06-19 22:16:24.000000 csdmpy-0.6.dev2/csdmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 deepansh   (501) staff       (20)       91 2023-06-19 22:16:24.000000 csdmpy-0.6.dev2/csdmpy.egg-info/requires.txt
+-rw-r--r--   0 deepansh   (501) staff       (20)        7 2023-06-19 22:16:24.000000 csdmpy-0.6.dev2/csdmpy.egg-info/top_level.txt
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.748400 csdmpy-0.6.dev2/docs/
+-rw-r--r--   0 deepansh   (501) staff       (20)     6148 2021-05-07 11:54:04.000000 csdmpy-0.6.dev2/docs/.DS_Store
+-rw-r--r--   0 deepansh   (501) staff       (20)    53248 2022-07-04 09:23:08.000000 csdmpy-0.6.dev2/docs/.coverage
+-rw-r--r--   0 deepansh   (501) staff       (20)     2599 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/CSD_model.rst
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.754561 csdmpy-0.6.dev2/docs/CSDmodel_uml/
+-rw-r--r--   0 deepansh   (501) staff       (20)     6148 2019-07-25 14:55:02.000000 csdmpy-0.6.dev2/docs/CSDmodel_uml/.DS_Store
+-rw-r--r--   0 deepansh   (501) staff       (20)     1501 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/CSDmodel_uml/csdm.rst
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.761260 csdmpy-0.6.dev2/docs/CSDmodel_uml/dependent_variables/
+-rw-r--r--   0 deepansh   (501) staff       (20)     2249 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/CSDmodel_uml/dependent_variables/dependent_variable.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      787 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/CSDmodel_uml/dependent_variables/external.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     1436 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/CSDmodel_uml/dependent_variables/internal.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     1745 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/CSDmodel_uml/dependent_variables/sparse_sampling.rst
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.766995 csdmpy-0.6.dev2/docs/CSDmodel_uml/dimensions/
+-rw-r--r--   0 deepansh   (501) staff       (20)     1424 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/CSDmodel_uml/dimensions/dimension.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     1145 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/CSDmodel_uml/dimensions/labeled.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     3526 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/CSDmodel_uml/dimensions/linear.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     2289 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/CSDmodel_uml/dimensions/monotonic.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     3761 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/CSDmodel_uml/enumeration.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      348 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/CSDmodel_uml/scalarQuantity.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      709 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/Makefile
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.767857 csdmpy-0.6.dev2/docs/_images/
+-rw-r--r--   0 deepansh   (501) staff       (20)     6148 2021-05-06 13:27:37.000000 csdmpy-0.6.dev2/docs/_images/.DS_Store
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.778104 csdmpy-0.6.dev2/docs/_static/
+-rw-r--r--   0 deepansh   (501) staff       (20)     6148 2020-06-23 22:36:23.000000 csdmpy-0.6.dev2/docs/_static/.DS_Store
+-rw-r--r--   0 deepansh   (501) staff       (20)     1622 2021-04-09 14:10:50.000000 csdmpy-0.6.dev2/docs/_static/button.css
+-rw-r--r--   0 deepansh   (501) staff       (20)   376691 2022-07-09 21:55:19.000000 csdmpy-0.6.dev2/docs/_static/csdm.png
+-rw-r--r--   0 deepansh   (501) staff       (20)    16811 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/_static/csdmpy.png
+-rw-r--r--   0 deepansh   (501) staff       (20)     8143 2021-04-09 14:10:50.000000 csdmpy-0.6.dev2/docs/_static/style.css
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.781228 csdmpy-0.6.dev2/docs/_templates/
+-rw-r--r--   0 deepansh   (501) staff       (20)     6148 2021-05-07 11:54:04.000000 csdmpy-0.6.dev2/docs/_templates/.DS_Store
+-rw-r--r--   0 deepansh   (501) staff       (20)     1766 2021-04-09 14:10:50.000000 csdmpy-0.6.dev2/docs/_templates/layout.html
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.793664 csdmpy-0.6.dev2/docs/api/
+-rw-r--r--   0 deepansh   (501) staff       (20)     6148 2021-05-07 08:42:55.000000 csdmpy-0.6.dev2/docs/api/.DS_Store
+-rw-r--r--   0 deepansh   (501) staff       (20)     2513 2023-05-28 18:04:12.000000 csdmpy-0.6.dev2/docs/api/CSDM.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     1638 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/api/DependentVariable.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     2025 2021-04-09 14:10:50.000000 csdmpy-0.6.dev2/docs/api/Dimensions.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     1448 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/api/csdmpy.rst
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.797366 csdmpy-0.6.dev2/docs/api/dimension/
+-rw-r--r--   0 deepansh   (501) staff       (20)      149 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/api/dimension/labeled.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      145 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/api/dimension/linear.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      157 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/api/dimension/monotonic.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      123 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/api/numpy_wrappers.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      517 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/docs/api/plotting_function.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      321 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/api/statistics.rst
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.799194 csdmpy-0.6.dev2/docs/api/wrappers/
+-rw-r--r--   0 deepansh   (501) staff       (20)      827 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/api/wrappers/apodization.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     8499 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/api/wrappers/element_wise_operation.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)       57 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/changelog.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)    11195 2022-07-09 16:43:43.000000 csdmpy-0.6.dev2/docs/conf.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     7374 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/getting_started.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     5593 2023-05-07 13:07:00.000000 csdmpy-0.6.dev2/docs/index.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     1827 2023-05-28 17:56:43.000000 csdmpy-0.6.dev2/docs/installation.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      797 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/make.bat
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.801826 csdmpy-0.6.dev2/docs/plotting_with_pyplot/
+-rw-r--r--   0 deepansh   (501) staff       (20)      866 2020-07-25 22:12:57.000000 csdmpy-0.6.dev2/docs/plotting_with_pyplot/one_D_plots.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      892 2020-07-25 22:12:57.000000 csdmpy-0.6.dev2/docs/plotting_with_pyplot/two_D_plots.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      322 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/referenceAPI.rst
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.813329 csdmpy-0.6.dev2/docs/startFromScratch/
+-rw-r--r--   0 deepansh   (501) staff       (20)     2925 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/startFromScratch/A fun example.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     2628 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/startFromScratch/add_dependent_variable_object.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     1896 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/startFromScratch/add_dimension_object.rst
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.672328 csdmpy-0.6.dev2/docs/startFromScratch/dimension/
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.817379 csdmpy-0.6.dev2/docs/startFromScratch/dimension/generate/
+-rw-r--r--   0 deepansh   (501) staff       (20)      198 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/startFromScratch/dimension/generate/dimension_objects.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      918 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/startFromScratch/dimension/generate/labeled.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     2853 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/startFromScratch/dimension/generate/linear.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     2527 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/startFromScratch/dimension/generate/monotonic.rst
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.821410 csdmpy-0.6.dev2/docs/startFromScratch/dimension/interact/
+-rw-r--r--   0 deepansh   (501) staff       (20)      158 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/startFromScratch/dimension/interact/dimension_objects.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     6093 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/startFromScratch/dimension/interact/linear.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     4434 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/startFromScratch/dimension/interact/monotonic.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     4647 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/startFromScratch/generating_csdm_object.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     5837 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/startFromScratch/generating_dependent_variable_object.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)    11628 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/startFromScratch/interacting_with_csdm.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      195 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/startFromScratch/interacting_with_csdmpy_objects.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     3265 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/docs/startFromScratch/save_dataset.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      494 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/startFromScratch/start.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)     1326 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/docs/using_csdm_with_pyplot.rst
+-rw-r--r--   0 deepansh   (501) staff       (20)      174 2020-06-23 22:39:50.000000 csdmpy-0.6.dev2/pyproject.toml
+-rw-r--r--   0 deepansh   (501) staff       (20)      426 2023-06-19 01:29:45.000000 csdmpy-0.6.dev2/requirements-dev.txt
+-rw-r--r--   0 deepansh   (501) staff       (20)      173 2023-06-19 01:29:49.000000 csdmpy-0.6.dev2/requirements.txt
+-rw-r--r--   0 deepansh   (501) staff       (20)      352 2023-06-19 22:16:24.917372 csdmpy-0.6.dev2/setup.cfg
+-rw-r--r--   0 deepansh   (501) staff       (20)     2302 2023-06-18 23:44:50.000000 csdmpy-0.6.dev2/setup.py
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.862887 csdmpy-0.6.dev2/tests/
+-rw-r--r--   0 deepansh   (501) staff       (20)     6148 2023-05-26 09:51:40.000000 csdmpy-0.6.dev2/tests/.DS_Store
+-rw-r--r--   0 deepansh   (501) staff       (20)     4316 2023-06-18 23:44:56.000000 csdmpy-0.6.dev2/tests/csdm_indexing_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     1125 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/tests/csdm_new_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)    19530 2023-06-18 23:44:56.000000 csdmpy-0.6.dev2/tests/csdm_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     9353 2022-09-24 12:45:46.000000 csdmpy-0.6.dev2/tests/dependent_variable_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)    23594 2023-06-19 22:11:53.000000 csdmpy-0.6.dev2/tests/dimension_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     4472 2023-05-29 18:30:47.000000 csdmpy-0.6.dev2/tests/fft_test.py
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.876170 csdmpy-0.6.dev2/tests/file_read/
+-rw-r--r--   0 deepansh   (501) staff       (20)     6148 2021-05-06 18:55:00.000000 csdmpy-0.6.dev2/tests/file_read/.DS_Store
+-rw-r--r--   0 deepansh   (501) staff       (20)     3070 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/tests/file_read/fileread_test.py
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.902040 csdmpy-0.6.dev2/tests/file_read/test_files/
+-rw-r--r--   0 deepansh   (501) staff       (20)     6148 2021-05-06 15:57:45.000000 csdmpy-0.6.dev2/tests/file_read/test_files/.DS_Store
+-rw-r--r--   0 deepansh   (501) staff       (20)      750 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/1.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      773 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/10.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      788 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/11.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      715 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/12.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      716 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/13.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      713 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/14.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      711 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/15.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      511 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/16.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      728 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/2.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      752 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/3.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      750 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/4.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      878 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/5.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      876 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/6.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      879 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/7.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      852 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/8.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)      802 2021-05-07 15:45:58.000000 csdmpy-0.6.dev2/tests/file_read/test_files/9.csdfe
+-rw-r--r--   0 deepansh   (501) staff       (20)     2295 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/tests/import_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     1327 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/tests/nmr_freq_test.py
+drwxr-xr-x   0 deepansh   (501) staff       (20)        0 2023-06-19 22:16:24.913805 csdmpy-0.6.dev2/tests/numpy_wrapper/
+-rw-r--r--   0 deepansh   (501) staff       (20)     3539 2023-05-11 00:22:23.000000 csdmpy-0.6.dev2/tests/numpy_wrapper/apodization_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     2468 2023-06-19 13:54:12.000000 csdmpy-0.6.dev2/tests/numpy_wrapper/change_shape_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     4070 2023-05-11 00:22:08.000000 csdmpy-0.6.dev2/tests/numpy_wrapper/dimension_reduction_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     5842 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/tests/numpy_wrapper/element_wise_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     2047 2023-06-19 13:54:12.000000 csdmpy-0.6.dev2/tests/numpy_wrapper/np_pad_flip_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     1846 2023-06-18 23:44:56.000000 csdmpy-0.6.dev2/tests/numpy_wrapper/numpy_csdm_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)      883 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/tests/save_file_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)      903 2022-07-09 01:12:01.000000 csdmpy-0.6.dev2/tests/serialization_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     2029 2022-07-09 21:55:19.000000 csdmpy-0.6.dev2/tests/sparse_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     2179 2023-06-18 23:44:56.000000 csdmpy-0.6.dev2/tests/statistics_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     1724 2023-06-18 23:44:56.000000 csdmpy-0.6.dev2/tests/unit_test.py
+-rw-r--r--   0 deepansh   (501) staff       (20)     3701 2023-06-19 13:54:12.000000 csdmpy-0.6.dev2/tests/utils_test.py
```

### Comparing `csdmpy-0.5/CHANGELOG` & `csdmpy-0.6.dev2/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+v0.6.0
+------
+
+Feature
+'''''''
+
+- Convert negative increment CSDM object to positive increment CSDM object.
+- Accepts both C and F contiguous numpy array to convert to CSDM object. #57
+- Add `csdm.reshape(dim1, dim2)` to CSDM object to reshape a CSDM object to the
+  given list dimension object---`dim1`, `dim2`.
+- Numpy broadcasing mulipllication can now be applied to csdm objects.
+- Support for additional numpy methods `np.pad` and `np.flip`.
+
+Bugfix
+''''''
+
+- fft and ifft scale the first point by 2 when the dimension is non-periodic.
+- Bugfix in serializing csdm #54
+- You can multiply CSDM objects by a scalar to the right (`csdm * scalar`). The fix
+  now allows the multiplication of CSDM objects by a scalar to the left (`scalar * csdm`). #62
+
 v0.5.0
 ------
 
 What's new
 ''''''''''
 
 - Add support for ``np.cumsum``, ``np.cumprod``, ``np.argmin``, ``np.argmax`` functions to CSDM objects.
```

### Comparing `csdmpy-0.5/LICENSE` & `csdmpy-0.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/PKG-INFO` & `csdmpy-0.6.dev2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,132 @@
 Metadata-Version: 2.1
 Name: csdmpy
-Version: 0.5
+Version: 0.6.dev2
 Summary: A python module for the core scientific dataset model.
 Home-page: https://github.com/DeepanshS/csdmpy/
 Author: Deepansh Srivastava
 Author-email: srivastava.89@osu.edu
 License: BSD-3-Clause
-Description: 
-        # The csdmpy project
-        
-        |              |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
-        | ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-        | Deployment   | [![PyPI version](https://img.shields.io/pypi/v/csdmpy.svg?style=flat&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/csdmpy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/csdmpy)                                                                                                                                                                                                                                                                                                                                                                |
-        | Build Status | [![Github workflow](<https://img.shields.io/github/workflow/status/deepanshs/csdmpy/CI%20(pip)?logo=GitHub>)](https://github.com/DeepanshS/csdmpy/actions) [![Documentation Status](https://readthedocs.org/projects/csdmpy/badge/?version=stable)](https://csdmpy.readthedocs.io/en/stable/?badge=stable)                                                                                                                                        |
-        | License      | [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
-        | Metrics      | [![Total alerts](https://img.shields.io/lgtm/alerts/g/DeepanshS/csdmpy.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/DeepanshS/csdmpy/alerts/) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/DeepanshS/csdmpy.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/DeepanshS/csdmpy/context:python) [![codecov](https://codecov.io/gh/DeepanshS/csdmpy/branch/master/graph/badge.svg)](https://codecov.io/gh/DeepanshS/csdmpy) |
-        | GitHub       | ![GitHub issues](https://img.shields.io/github/issues-raw/deepanshs/csdmpy)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-        | Citations    | [![DOI](<https://img.shields.io/badge/DOI-PLOS%20ONE%2015(1):%20e0225953-blueviolet>)](https://doi.org/10.1371/journal.pone.0225953)                                                                                                                                                                                                                                                                                                                               |
-        
-        The _csdmpy_ package is a Python support for the core scientific
-        dataset (CSD) model file exchange-format.
-        The package is based on the core scientific dataset (CSD) model which is
-        designed as a building block in the development of a more sophisticated
-        portable scientific dataset file standard.
-        The CSD model is capable of handling a wide variety of
-        scientific datasets both within and across disciplinary fields.
-        
-        The main objective of this python package is to facilitate an easy import and
-        export of the CSD model serialized JSON files for Python users. The
-        package utilizes Numpy library and, therefore, offers the end users versatility
-        to process or visualize the imported datasets with any third party package(s)
-        compatible with Numpy.
-        
-        For further reading, refer to the [documentation](https://csdmpy.readthedocs.io/en/latest/).
-        
-        > **See example gallery**
-        >
-        > [![View](https://img.shields.io/badge/View-Example%20Gallery-Purple?size=large)](https://csdmpy.readthedocs.io/en/latest/auto_examples/index.html)
-        
-        ## The core scientific dataset (CSD) model
-        
-        The core scientific dataset (CSD) model is a _light-weight_, _portable_,
-        _versatile_, and _standalone_ data model capable of handling a variety of
-        scientific datasets. The model only encapsulates
-        data values and the minimum metadata, to accurately represent a **_p_-component
-        dependent variable,
-        discretely sampled at _M_ unique points in a _d_-dimensional coordinate space**.
-        The model is not intended to encapsulate
-        any information on how the data might be acquired, processed, or visualized.
-        
-        ---
-        ### Use cases
-        The data model is _versatile_ in allowing many **use cases for most spectroscopy,
-        diffraction, and imaging techniques**.
-        
-        ![](/docs/_static/csdm.png "")
-        
-        ### Data Model
-        
-        The model supports multi-component datasets associated with continuous
-        physical quantities that are discretely sampled in a multi-dimensional space
-        associated with other carefully controlled quantities, for e.g., a mass as a
-        function of temperature, a current as a function of voltage and time, a signal
-        voltage as a function of magnetic field gradient strength, a color image with
-        a red, green, and blue (RGB) light intensity components as a function of two
-        independent spatial dimensions, or the six components of the symmetric
-        second-rank diffusion tensor MRI as a function of three independent spatial
-        dimensions. Additionally, the model supports multiple dependent variables
-        sharing the same _d_-dimensional coordinate space. For instance,
-        the simultaneous measurement of current and voltage as a function of time.
-        Another example would be the simultaneous acquisition of air temperature,
-        pressure, wind velocity, and
-        solar-flux as a function of Earth’s latitude and longitude coordinates. We
-        refer to these dependent variables as _correlated-datasets_.
-        
-        **Example**
-        ```py
-        "csdm": {
-          "version": "1.0",
-          # A list of Linear, Monotonic, or Labeled dimensions of the multi-dimensional space.
-          "dimensions": [{
-            "type": "linear",
-            "count": 1608,
-            "increment": "0.08333333333 yr",
-            "coordinates_offset": "1880.0416666667 yr",
-          }],
-          # A list of dependent variables sampling the multi-dimensional space.
-          "dependent_variables": [{
-            "type": "internal",
-            "unit": "mm",
-            "numeric_type": "float32",
-            "quantity_type": "scalar",
-            "component_labels": ["GMSL"],
-            "components": [
-              ["-183.0, -171.125, ..., 59.6875, 58.5"]
-            ]
-          }]
-        }
-        ```
-        ## Installing _csdmpy_ package
-        
-            $ pip install csdmpy
-        
-        ## How to cite
-        
-        Please cite the following when used in publication.
-        
-        1. Srivastava D.J., Vosegaard T., Massiot D., Grandinetti P.J. (2020) Core Scientific Dataset Model: A lightweight and portable model and file format for multi-dimensional scientific data. [PLOS ONE 15(1): e0225953.](https://doi.org/10.1371/journal.pone.0225953)
-        
-        ## Check out the media coverage.
-        
-        - [<img src="https://inc.cnrs.fr/sites/institut_inc/files/styles/top_left/public/image/cnrs_20180120_0025%20%281%29.jpg?itok=i3wlyGBq" height="64" width="64"> Des chimistes élaborent un nouveau format pour le partage de données scientifiques](https://inc.cnrs.fr/fr/cnrsinfo/des-chimistes-elaborent-un-nouveau-format-pour-le-partage-de-donnees-scientifiques)
-        
-        - [<img src="https://www.technology.org/texorgwp/wp-content/uploads/2020/01/1920_data-1536x1024.jpg" height="64" width="64"> Simplifying how scientists share data](https://www.technology.org/2020/01/03/simplifying-how-scientists-share-data/)
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: matplotlib
+License-File: LICENSE
+
+
+# The csdmpy project
+
+|              |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Deployment   | [![PyPI version](https://img.shields.io/pypi/v/csdmpy.svg?style=flat&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/csdmpy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/csdmpy)                                                                                                                                                                                                                                                                                                                                                                |
+| Build Status | [![Github workflow](<https://img.shields.io/github/actions/workflow/status/deepanshs/csdmpy/continuous-integration-pip.yml?logo=GitHub>)](https://github.com/DeepanshS/csdmpy/actions/workflow/continuous-integration-pip.yml) [![Documentation Status](https://readthedocs.org/projects/csdmpy/badge/?version=stable)](https://csdmpy.readthedocs.io/en/stable/?badge=stable)                                                                                                                                        |
+| License      | [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| Metrics      | [![codecov](https://codecov.io/gh/DeepanshS/csdmpy/branch/master/graph/badge.svg)](https://codecov.io/gh/DeepanshS/csdmpy) ![GitHub issues](https://img.shields.io/github/issues-raw/deepanshs/csdmpy)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+| Citation    | [![DOI](<https://img.shields.io/badge/DOI-PLOS%20ONE%2015(1):%20e0225953-blueviolet>)](https://doi.org/10.1371/journal.pone.0225953)                                                                                                                                                                                                                                                                                                                               |
+
+The _csdmpy_ package is a Python support for the core scientific
+dataset (CSD) model file exchange-format.
+The package is based on the core scientific dataset (CSD) model which is
+designed as a building block in the development of a more sophisticated
+portable scientific dataset file standard.
+The CSD model is capable of handling a wide variety of
+scientific datasets both within and across disciplinary fields.
+
+The main objective of this python package is to facilitate an easy import and
+export of the CSD model serialized JSON files for Python users. The
+package utilizes Numpy library and, therefore, offers the end users versatility
+to process or visualize the imported datasets with any third party package(s)
+compatible with Numpy.
+
+For further reading, refer to the [documentation](https://csdmpy.readthedocs.io/en/latest/).
+
+> **See example gallery**
+>
+> [![View](https://img.shields.io/badge/View-Example%20Gallery-Purple?size=large)](https://csdmpy.readthedocs.io/en/latest/auto_examples/index.html)
+
+## The core scientific dataset (CSD) model
+
+The core scientific dataset (CSD) model is a _light-weight_, _portable_,
+_versatile_, and _standalone_ data model capable of handling a variety of
+scientific datasets. The model only encapsulates
+data values and the minimum metadata, to accurately represent a **_p_-component
+dependent variable,
+discretely sampled at _M_ unique points in a _d_-dimensional coordinate space**.
+The model is not intended to encapsulate
+any information on how the data might be acquired, processed, or visualized.
+
+---
+### Use cases
+The data model is _versatile_ in allowing many **use cases for most spectroscopy,
+diffraction, and imaging techniques**.
+
+![](/docs/_static/csdm.png "")
+
+### Data Model
+
+The model supports multi-component datasets associated with continuous
+physical quantities that are discretely sampled in a multi-dimensional space
+associated with other carefully controlled quantities, for e.g., a mass as a
+function of temperature, a current as a function of voltage and time, a signal
+voltage as a function of magnetic field gradient strength, a color image with
+a red, green, and blue (RGB) light intensity components as a function of two
+independent spatial dimensions, or the six components of the symmetric
+second-rank diffusion tensor MRI as a function of three independent spatial
+dimensions. Additionally, the model supports multiple dependent variables
+sharing the same _d_-dimensional coordinate space. For instance,
+the simultaneous measurement of current and voltage as a function of time.
+Another example would be the simultaneous acquisition of air temperature,
+pressure, wind velocity, and
+solar-flux as a function of Earth’s latitude and longitude coordinates. We
+refer to these dependent variables as _correlated-datasets_.
+
+**Example**
+```py
+"csdm": {
+  "version": "1.0",
+  # A list of Linear, Monotonic, or Labeled dimensions of the multi-dimensional space.
+  "dimensions": [{
+    "type": "linear",
+    "count": 1608,
+    "increment": "0.08333333333 yr",
+    "coordinates_offset": "1880.0416666667 yr",
+  }],
+  # A list of dependent variables sampling the multi-dimensional space.
+  "dependent_variables": [{
+    "type": "internal",
+    "unit": "mm",
+    "numeric_type": "float32",
+    "quantity_type": "scalar",
+    "component_labels": ["GMSL"],
+    "components": [
+      ["-183.0, -171.125, ..., 59.6875, 58.5"]
+    ]
+  }]
+}
+```
+## Installing _csdmpy_ package
+
+    $ pip install csdmpy
+
+## How to cite
+
+Please cite the following when used in publication.
+
+1. Srivastava D.J., Vosegaard T., Massiot D., Grandinetti P.J. (2020) Core Scientific Dataset Model: A lightweight and portable model and file format for multi-dimensional scientific data. [PLOS ONE 15(1): e0225953.](https://doi.org/10.1371/journal.pone.0225953)
+
+## Check out the media coverage.
+
+- [<img src="https://inc.cnrs.fr/sites/institut_inc/files/styles/top_left/public/image/cnrs_20180120_0025%20%281%29.jpg?itok=i3wlyGBq" height="64" width="64"> Des chimistes élaborent un nouveau format pour le partage de données scientifiques](https://inc.cnrs.fr/fr/cnrsinfo/des-chimistes-elaborent-un-nouveau-format-pour-le-partage-de-donnees-scientifiques)
+
+- [<img src="https://www.technology.org/texorgwp/wp-content/uploads/2020/01/1920_data-1536x1024.jpg" height="64" width="64"> Simplifying how scientists share data](https://www.technology.org/2020/01/03/simplifying-how-scientists-share-data/)
```

### Comparing `csdmpy-0.5/README.md` & `csdmpy-0.6.dev2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # The csdmpy project
 
 |              |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 | ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | Deployment   | [![PyPI version](https://img.shields.io/pypi/v/csdmpy.svg?style=flat&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/csdmpy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/csdmpy)                                                                                                                                                                                                                                                                                                                                                                |
-| Build Status | [![Github workflow](<https://img.shields.io/github/workflow/status/deepanshs/csdmpy/CI%20(pip)?logo=GitHub>)](https://github.com/DeepanshS/csdmpy/actions) [![Documentation Status](https://readthedocs.org/projects/csdmpy/badge/?version=stable)](https://csdmpy.readthedocs.io/en/stable/?badge=stable)                                                                                                                                        |
+| Build Status | [![Github workflow](<https://img.shields.io/github/actions/workflow/status/deepanshs/csdmpy/continuous-integration-pip.yml?logo=GitHub>)](https://github.com/DeepanshS/csdmpy/actions/workflow/continuous-integration-pip.yml) [![Documentation Status](https://readthedocs.org/projects/csdmpy/badge/?version=stable)](https://csdmpy.readthedocs.io/en/stable/?badge=stable)                                                                                                                                        |
 | License      | [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
-| Metrics      | [![Total alerts](https://img.shields.io/lgtm/alerts/g/DeepanshS/csdmpy.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/DeepanshS/csdmpy/alerts/) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/DeepanshS/csdmpy.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/DeepanshS/csdmpy/context:python) [![codecov](https://codecov.io/gh/DeepanshS/csdmpy/branch/master/graph/badge.svg)](https://codecov.io/gh/DeepanshS/csdmpy) |
-| GitHub       | ![GitHub issues](https://img.shields.io/github/issues-raw/deepanshs/csdmpy)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-| Citations    | [![DOI](<https://img.shields.io/badge/DOI-PLOS%20ONE%2015(1):%20e0225953-blueviolet>)](https://doi.org/10.1371/journal.pone.0225953)                                                                                                                                                                                                                                                                                                                               |
+| Metrics      | [![codecov](https://codecov.io/gh/DeepanshS/csdmpy/branch/master/graph/badge.svg)](https://codecov.io/gh/DeepanshS/csdmpy) ![GitHub issues](https://img.shields.io/github/issues-raw/deepanshs/csdmpy)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+| Citation    | [![DOI](<https://img.shields.io/badge/DOI-PLOS%20ONE%2015(1):%20e0225953-blueviolet>)](https://doi.org/10.1371/journal.pone.0225953)                                                                                                                                                                                                                                                                                                                               |
 
 The _csdmpy_ package is a Python support for the core scientific
 dataset (CSD) model file exchange-format.
 The package is based on the core scientific dataset (CSD) model which is
 designed as a building block in the development of a more sophisticated
 portable scientific dataset file standard.
 The CSD model is capable of handling a wide variety of
```

### Comparing `csdmpy-0.5/csdmpy/__init__.py` & `csdmpy-0.6.dev2/csdmpy/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 """The data model build on the Core Scientific Dataset Model."""
 import datetime
 import json
 from urllib.parse import urlparse
 
 import numpy as np
 
-from .csdm import as_dependent_variable  # lgtm [py/import-own-module] # NOQA
-from .csdm import as_dimension  # lgtm [py/import-own-module] # NOQA
-from .csdm import CSDM  # lgtm [py/import-own-module] # NOQA
-from .csdm import DependentVariable  # lgtm [py/import-own-module] # NOQA
-from .csdm import Dimension  # lgtm [py/import-own-module] # NOQA
-from .csdm import LabeledDimension  # lgtm [py/import-own-module] # NOQA
-from .csdm import LinearDimension  # lgtm [py/import-own-module] # NOQA
-from .csdm import MonotonicDimension  # lgtm [py/import-own-module] # NOQA
-from .dependent_variable import download  # lgtm [py/import-own-module] # NOQA
-from .helper_functions import _preview  # lgtm [py/import-own-module] # NOQA
-from .numpy_wrapper import apodize  # lgtm [py/import-own-module] # NOQA
-from .tests import *  # lgtm [py/import-own-module] # NOQA
-from .units import ScalarQuantity  # lgtm [py/import-own-module] # NOQA
-from .units import string_to_quantity  # lgtm [py/import-own-module] # NOQA
-from .utils import QuantityType  # lgtm [py/import-own-module] # NOQA
-from .utils import validate  # lgtm [py/import-own-module] # NOQA
+from .csdm import as_dependent_variable  # NOQA
+from .csdm import as_dimension  # NOQA
+from .csdm import CSDM  # NOQA
+from .csdm import DependentVariable  # NOQA
+from .csdm import Dimension  # NOQA
+from .csdm import LabeledDimension  # NOQA
+from .csdm import LinearDimension  # NOQA
+from .csdm import MonotonicDimension  # NOQA
+from .dependent_variable import download  # NOQA
+from .helper_functions import _preview  # NOQA
+from .numpy_wrapper import apodize  # NOQA
+from .tests import *  # NOQA
+from .units import Quantity  # NOQA
+from .units import ScalarQuantity  # NOQA
+from .units import string_to_quantity  # NOQA
+from .utils import QuantityType  # NOQA
+from .utils import validate  # NOQA
 
 now = datetime.datetime.now()
 year = now.year
 
 __author__ = "Deepansh J. Srivastava"
 __email__ = "srivastava.89@osu.edu"
 __copyright__ = f"Copyright 2019-{year}, The CSDMpy Project."
 __credits__ = ["Deepansh J. Srivastava"]
 __license__ = "BSD License"
 __maintainer__ = "Deepansh J. Srivastava"
 __status__ = "Beta"
-__version__ = "0.5"
+__version__ = "0.6.dev2"
 
 __all__ = [
     "parse_dict",
     "load",
     "loads",
     "new",
     "as_csdm",
@@ -235,16 +236,16 @@
     if q_type.p != array.shape[0]:
         raise ValueError(
             f"Expecting exactly {q_type.p} components for quantity type, "
             f"`{quantity_type}`, found {array.shape[0]}. Make sure `array.shape[0]` "
             f"is equal to the number of components supported by {quantity_type}."
         )
 
-    shape = array.shape[::-1][:-1]
-    dim = [LinearDimension(count=i, increment="1") for i in shape]
+    ar_shape = array.shape[::-1][:-1]
+    dim = [Dimension(type="linear", count=i, increment="1") for i in ar_shape]
     dv = DependentVariable(
         type="internal",
         components=array,
         unit=unit,
         quantity_type=quantity_type,
     )
     return CSDM(dimensions=dim, dependent_variables=[dv])
```

### Comparing `csdmpy-0.5/csdmpy/abstract_list.py` & `csdmpy-0.6.dev2/csdmpy/abstract_list.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/csdmpy/csdm.py` & `csdmpy-0.6.dev2/csdmpy/csdm.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,85 +3,43 @@
 import json
 import warnings
 from copy import deepcopy
 
 import numpy as np
 from astropy.units.quantity import Quantity
 
-from .abstract_list import __dimensions_list__  # lgtm [py/import-own-module]
-from .abstract_list import DependentVariableList  # lgtm [py/import-own-module]
-from .abstract_list import DimensionList  # lgtm [py/import-own-module]
+from .abstract_list import __dimensions_list__
+from .abstract_list import DependentVariableList
+from .abstract_list import DimensionList
 from .dependent_variable import as_dependent_variable  # noqa: F401
-from .dependent_variable import DependentVariable  # lgtm [py/import-own-module]
-from .dimension import as_dimension  # lgtm [py/import-own-module]
-from .dimension import Dimension  # lgtm [py/import-own-module] # noqa: F401
-from .dimension import LabeledDimension  # lgtm [py/import-own-module] # noqa: F401
-from .dimension import LinearDimension  # lgtm [py/import-own-module] # noqa: F401
-from .dimension import MonotonicDimension  # lgtm [py/import-own-module] # noqa: F401
-from .helper_functions import _preview  # lgtm [py/import-own-module]
+from .dependent_variable import DependentVariable
+from .dimension import as_dimension
+from .dimension import Dimension  # noqa: F401
+from .dimension import LabeledDimension  # noqa: F401
+from .dimension import LinearDimension  # noqa: F401
+from .dimension import MonotonicDimension  # noqa: F401
+from .helper_functions import _preview
+from .numpy_wrapper import __array_manipulation__
+from .numpy_wrapper import __function_reduction_list__
+from .numpy_wrapper import __other_functions__
+from .numpy_wrapper import __shape_manipulation_functions__
+from .numpy_wrapper import __ufunc_list_applies_to_unit__
+from .numpy_wrapper import __ufunc_list_dimensionless_unit__
+from .numpy_wrapper import __ufunc_list_unit_independent__
 from .numpy_wrapper import fft
-from .units import string_to_quantity  # lgtm [py/import-own-module]
-from .utils import _check_dimension_indices  # lgtm [py/import-own-module]
-from .utils import _get_broadcast_shape  # lgtm [py/import-own-module]
-from .utils import check_scalar_object  # lgtm [py/import-own-module]
-from .utils import validate  # lgtm [py/import-own-module]
+from .units import string_to_quantity
+from .utils import _check_dimension_indices
+from .utils import _get_broadcast_shape
+from .utils import check_scalar_object
+from .utils import get_CSDM_object__args__axes
+from .utils import np_check_for_out
+from .utils import np_check_pads
+from .utils import validate
 
 __all__ = ["CSDM"]
-__ufunc_list_dimensionless_unit__ = [
-    np.sin,
-    np.cos,
-    np.tan,
-    np.arcsin,
-    np.arccos,
-    np.arctan,
-    np.sinh,
-    np.cosh,
-    np.tanh,
-    np.arcsinh,
-    np.arccosh,
-    np.arctanh,
-    np.exp,
-    np.exp2,
-    np.log,
-    np.log2,
-    np.log10,
-    np.expm1,
-    np.log1p,
-]
-
-__ufunc_list_unit_independent__ = [
-    np.negative,
-    np.positive,
-    np.absolute,
-    np.fabs,
-    np.rint,
-    np.sign,
-    np.conj,
-    np.conjugate,
-]
-
-__ufunc_list_applies_to_unit__ = [np.sqrt, np.square, np.cbrt, np.reciprocal, np.power]
-
-__function_reduction_list__ = [
-    np.max,
-    np.min,
-    np.sum,
-    np.mean,
-    np.var,
-    np.std,
-    np.prod,
-    np.cumsum,
-    np.cumprod,
-    np.argmin,
-    np.argmax,
-]
-
-__other_functions__ = [np.round, np.real, np.imag, np.clip, np.around, np.angle]
-
-__shape_manipulation_functions__ = [np.transpose]
 
 
 class CSDM:
     """Create an instance of a CSDM class.
 
     This class is based on the root CSDM object of the core scientific dataset
     (CSD) model. The class is a composition of the :ref:`dv_api` and
@@ -134,30 +92,30 @@
             for k, v in kwargs.items()
             if f"_{k}" in CSDM.__slots__
         ]
 
         self._dimensions = DimensionList([])
         if "dimensions" in kwargs_keys:
             if not isinstance(kwargs["dimensions"], (list, DimensionList)):
-                t_ = type(kwargs["dimensions"])
+                dim_type = type(kwargs["dimensions"])
                 raise ValueError(
                     "A list of valid Dimension or equivalent dictionary objects is "
-                    f"required, found {t_}."
+                    f"required, found {dim_type}."
                 )
             _ = [self.dimensions.append(item) for item in kwargs["dimensions"]]
 
         self._dependent_variables = DependentVariableList([])
         if "dependent_variables" in kwargs_keys:
-            t_ = type(kwargs["dependent_variables"])
+            dv_type = type(kwargs["dependent_variables"])
             if not isinstance(
                 kwargs["dependent_variables"], (list, DependentVariableList)
             ):
                 raise ValueError(
                     "A list of valid DependentVariable or equivalent dictionary "
-                    f"objects is required, found {t_}."
+                    f"objects is required, found {dv_type}."
                 )
             for item in kwargs["dependent_variables"]:
                 if isinstance(item, dict):
                     item.update({"filename": self.filename})
                 self.dependent_variables.append(item)
                 if self.shape != ():
                     shape = self.shape[::-1]
@@ -293,15 +251,14 @@
     # def __rshift__(self, other):
     #     raise NotImplementedError()
 
     # def __irshift__(self, other):
     #     raise NotImplementedError()
 
     def __ifunction__(self, function, symbol, other):
-
         if isinstance(other, CSDM):
             self.__check_csdm_object_additive_compatibility(other)
 
             for i, item in enumerate(self.dependent_variables):
                 factor = other.dependent_variables[i].unit.to(item.unit)
                 f_n = getattr(item.components, function)
                 f_n(factor * other.dependent_variables[i].components)
@@ -314,68 +271,68 @@
             if not isinstance(other, Quantity):
                 f_n(other)
             else:
                 factor = other.unit.to(item.unit)
                 f_n(factor * other.value)
         return self
 
-    def _default_addition_(self, other, fn, operation):
+    def _default_addition_(self, other, f_n, operation):
         """Operate on two objects (z=x+/-y), if the other object is a
             1) csdm or scalar object,
             2) with identical dimension objects,
             3) same number of dependent-variables, and
             4) each dependent variables with identical dimensionality.
 
         Args:
             other: the object to add/subtract
-            fn: addition/subtraction function
+            f_n: addition/subtraction function
             operation: "+" or "-"
         """
         if isinstance(other, CSDM):
             self.__check_csdm_object_additive_compatibility(other)
 
-            d1 = self.copy()
-            for i, item in enumerate(d1.dependent_variables):
+            obj = self.copy()
+            for i, item in enumerate(obj.dependent_variables):
                 factor = other.dependent_variables[i].unit.to(item.unit)
-                item.components = item.components + fn(
+                item.components = item.components + f_n(
                     factor, other.dependent_variables[i].components
                 )
-            return d1
+            return obj
 
         other = check_scalar_object(other, operation)
-        d1 = self.copy()
-        for i, item in enumerate(d1.dependent_variables):
+        obj = self.copy()
+        for i, item in enumerate(obj.dependent_variables):
             item.components = (
-                item.components + fn(1, other)
+                item.components + f_n(1, other)
                 if not isinstance(other, Quantity)
-                else item.components + fn(1, other.unit.to(item.unit) * other.value)
+                else item.components + f_n(1, other.unit.to(item.unit) * other.value)
             )
-        return d1
+        return obj
 
     def __add__(self, other):
         """Add two objects (z=x+y)"""
 
-        def function(a, b):
-            return a * b
+        def function(val_1, val_2):
+            return val_1 * val_2
 
         return self._default_addition_(other, function, "+")
 
     def __radd__(self, other):
         """Right add two objects. See __add__ for details."""
         return self.__add__(other)
 
     def __iadd__(self, other):
         """Add two objects in-place (y+=x).  See __add__ for details."""
         return self.__ifunction__("__iadd__", "+", other)
 
     def __sub__(self, other):
         """Subtract two objects (z=x+y)"""
 
-        def function(a, b):
-            return -a * b
+        def function(val_1, val_2):
+            return -val_1 * val_2
 
         return self._default_addition_(other, function, "-")
 
     def __rsub__(self, other):
         """Right subtract two objects. See __sub__ for details."""
         return -self.__sub__(other)
 
@@ -383,23 +340,23 @@
         """Subtract two objects in-lace (y-=x). See __sub__ for details."""
         return self.__ifunction__("__isub__", "-", other)
 
     def __mul__(self, other):
         """Multiply the components of the CSDM object by a scalar."""
         other = check_scalar_object(other, "*")
 
-        d1 = self.copy()
-        for item in d1.dependent_variables:
+        obj = self.copy()
+        for item in obj.dependent_variables:
             if not isinstance(other, Quantity):
                 item.components = item.components * other
             else:
                 value = 1 * item.subtype._unit * other
                 item.subtype._unit = value.unit
                 item.components = item.components * value.value
-        return d1
+        return obj
 
     def __rmul__(self, other):
         """Right multiply the components of the CSDM object by a scalar."""
         return self.__mul__(other)
 
     def __imul__(self, other):
         """In place multiplication of the components of the CSDM object by a scalar."""
@@ -415,23 +372,23 @@
                 item.components.__imul__(value.value)
         return self
 
     def __truediv__(self, other):
         """Divide the components of the CSDM object by a scalar."""
         other = check_scalar_object(other, "/")
 
-        d1 = self.copy()
-        for item in d1.dependent_variables:
+        obj = self.copy()
+        for item in obj.dependent_variables:
             if not isinstance(other, Quantity):
                 item.components = item.components / other
             else:
                 value = (1 * item.subtype._unit) / other
                 item.subtype._unit = value.unit
                 item.components = item.components * value.value
-        return d1
+        return obj
 
     def __rtruediv__(self, other):
         """Right divide the components of the CSDM object by a scalar."""
         return np.reciprocal(self) * other
 
     def __itruediv__(self, other):
         """In place division of the components of the CSDM object by a scalar."""
@@ -457,17 +414,17 @@
         for item in self.dependent_variables:
             item.components.__ipow__(other)
             item.subtype._unit = item.subtype._unit**other
         return self
 
     def _get_indices(self, indices):
         if isinstance(indices, tuple):
-            l_ = len(indices)
+            size = len(indices)
             indices = indices + tuple(
-                slice(0, _.count, 1) for _ in self.dimensions[l_:]
+                slice(0, _.count, 1) for _ in self.dimensions[size:]
             )
         if isinstance(indices, (int, slice)):
             indices = (indices,) + tuple(
                 slice(0, _.count, 1) for _ in self.dimensions[1:]
             )
         for item in indices:
             if isinstance(item, (tuple, list)):
@@ -486,50 +443,38 @@
             variable.components[section] = values
 
     def __getitem__(self, indices):
         """Return a csdm object corresponding to given indices."""
         indices = self._get_indices(indices)
         csdm = CSDM()
         for i, dim in enumerate(self.dimensions):
-            s_ = indices[i]
-
-            dim_ = dim.subtype if hasattr(dim, "subtype") else dim
-
-            length_ = dim.coordinates[s_].size
-            if length_ > 1:
-                if hasattr(dim_, "_equivalencies"):
-                    equivalencies_ = dim_._equivalencies
-                    dim_._equivalencies = None
-                    x = dim.coordinates[s_]
-                    new_dim = as_dimension(x.value, unit=str(x.unit))
-                    dim_._equivalencies = equivalencies_
-                    new_dim._equivalencies = equivalencies_
-
-                else:
-                    x = dim.coordinates[s_]
-                    new_dim = as_dimension(x)
-
-                new_dim._copy_metadata(dim_)
-                if hasattr(new_dim, "complex_fft"):
-                    new_dim.complex_fft = False
-
+            dim_ = Dimension(**dim.dict()) if not hasattr(self, "subtype") else dim
+            dim_.copy_metadata(dim)
+            new_dim = dim_[indices[i]]
+            if new_dim.size > 1:
                 csdm._dimensions += [new_dim]
 
         for variable in self.dependent_variables:
             section = (slice(0, len(variable.components), 1),) + indices[::-1]
-            y = variable.components[section]
-            dv = empty_dependent_variable(variable.numeric_type, variable.quantity_type)
-            dv.subtype._components = y
-            dv._copy_metadata(variable)
-            csdm._dependent_variables += [dv]
-
-        csdm._copy_metadata(self)
+            components = variable.components[section]
+            dv_obj = empty_dependent_variable(
+                variable.numeric_type, variable.quantity_type
+            )
+            dv_obj.subtype._components = components
+            dv_obj.copy_metadata(variable)
+            csdm._dependent_variables += [dv_obj]
+
+        csdm.copy_metadata(self)
+        if len(csdm.dimensions) == 0 and len(csdm.dependent_variables) == 1:
+            value = np.squeeze(csdm.dependent_variables[0].components)
+            unit = csdm.dependent_variables[0].unit
+            return value * unit
         return csdm
 
-    def _copy_metadata(self, other):
+    def copy_metadata(self, other):
         self._version = other._version
         self._description = other._description
         self._read_only = other._read_only
         self._tags = other._tags
         self._timestamp = other._timestamp
         self._geographic_coordinate = other._geographic_coordinate
         self._application = other._application
@@ -719,22 +664,22 @@
         components."""
         return np.imag(self)
 
     @property
     def T(self):
         """Return a csdm object with a transpose of the dataset."""
         new = CSDM()
-        new._copy_metadata(self)
+        new.copy_metadata(self)
         new._dimensions += self._dimensions[::-1]
 
         for item in self.dependent_variables:
-            dv = empty_dependent_variable(item.numeric_type, item.quantity_type)
-            dv._copy_metadata(item)
-            dv.subtype._components = np.moveaxis(item.subtype._components.T, -1, 0)
-            new._dependent_variables += [dv]
+            dv_obj = empty_dependent_variable(item.numeric_type, item.quantity_type)
+            dv_obj.copy_metadata(item)
+            dv_obj.subtype._components = np.moveaxis(item.subtype._components.T, -1, 0)
+            new._dependent_variables += [dv_obj]
 
         return new
 
     @property
     def shape(self):
         """Return the count along each dimension of the csdm object."""
         return tuple(item.count for item in self._dimensions)
@@ -745,14 +690,42 @@
         return np.prod([item.count for item in self.dimensions])
 
     @property
     def ndim(self):
         """Return the total number of dimensions."""
         return len(self.dimensions)
 
+    def reshape(self, shape):
+        """Reshape the csdm object to shape.
+
+        Args:
+            shape: A list of dimension objects or integers.
+        """
+        size = self.y[0].components[0].size
+
+        shape_int = [item if isinstance(item, int) else item.size for item in shape]
+        new_dim = []
+        for index in shape:
+            sh = int(-size / np.prod(shape_int)) if index == -1 else index
+            dim = (
+                Dimension(type="linear", count=sh, increment="1")
+                if isinstance(sh, int)
+                else sh
+            )
+            new_dim.append(dim)
+
+        for d_v in self.y:
+            new_shape = (d_v.components.shape[0],) + tuple(shape_int[::-1])
+            new_dv = as_dependent_variable(array=d_v.components.reshape(new_shape))
+            new_dv.copy_metadata(d_v)
+
+        new_csdm = CSDM(dimensions=new_dim, dependent_variables=[new_dv])
+        new_csdm.copy_metadata(self)
+        return new_csdm
+
     # ----------------------------------------------------------------------- #
     #                                  Methods                                #
     # ----------------------------------------------------------------------- #
     # deprecated
     def add_dimension(self, *args, **kwargs):
         """Add a new :ref:`dim_api` instance to the :ref:`csdm_api` object.
 
@@ -1098,16 +1071,16 @@
 
     # csdm dimension order manipulation
     def transpose(self):
         """Return a transpose of the CSDM object."""
         return self.T
 
     def fft(self, axis=0):
-        """Perform a FFT along the given `dimension=axis`, for linear dimension, assuming
-        Nyquist-Shannon relation.
+        """Perform a FFT along the given `dimension=axis`, for linear dimension,
+        assuming Nyquist-Shannon relation.
 
         Args:
             axis: dimension index along which the FFT is performed.
 
         The FFT method uses the :attr:`~csdmpy.Dimension.complex_fft` attribute of the
         Dimension object to decide whether a forward or inverse Fourier transform is
         performed. If the value of the `complex_fft` is True, an inverse FFT is
@@ -1318,80 +1291,109 @@
                 per dependent variable.
         Return:
             A CSDM object with `m` dimensions removed, or a list when `axis` is None.
         """
         return np.cumprod(self, axis=axis)
 
     def __array_ufunc__(self, function, method, *inputs, **kwargs):
+        if function == np.multiply:
+            return inputs[1] * inputs[0]
+        if function == np.divide:
+            return (1.0 / inputs[1]) * inputs[0]
+
         csdm = inputs[0]
         input_ = []
         if len(inputs) > 1:
             input_ = inputs[1:]
 
         if function in __ufunc_list_dimensionless_unit__:
             factor = np.ones(len(csdm.dependent_variables))
             for i, variable in enumerate(csdm.dependent_variables):
                 if variable.unit.physical_type != "dimensionless":
                     raise ValueError(
                         f"Cannot apply `{function.__name__}` to quantity with physical "
                         f"type `{variable.unit.physical_type}`."
                     )
                 factor[i] = variable.unit.to("")
-            return _get_new_csdm_object_after_applying_ufunc(
-                inputs[0], function, method, factor, *input_, **kwargs
+            return get_new_csdm_object_after_applying_ufunc(
+                csdm, function, method, factor, *input_, **kwargs
             )
 
         if function in __ufunc_list_unit_independent__:
-            return _get_new_csdm_object_after_applying_ufunc(
-                inputs[0], function, method, None, *input_, **kwargs
+            return get_new_csdm_object_after_applying_ufunc(
+                csdm, function, method, None, *input_, **kwargs
             )
 
         if function in __ufunc_list_applies_to_unit__:
-            obj = _get_new_csdm_object_after_applying_ufunc(
-                inputs[0], function, method, None, *input_, **kwargs
+            obj = get_new_csdm_object_after_applying_ufunc(
+                csdm, function, method, None, *input_, **kwargs
             )
             for i, variable in enumerate(obj.dependent_variables):
                 scalar = function(1 * variable.unit, *input_)
                 variable.components *= scalar.value
                 variable.subtype._unit = scalar.unit
             return obj
 
         raise NotImplementedError(f"Function {function} is not implemented.")
 
     def __array_function__(self, function, _, *args, **kwargs):
         if function in __function_reduction_list__:
-            return _get_new_csdm_object_after_dimension_reduction_func(
+            return get_new_csdm_object_after_dimension_reduction_func(
                 function, *args[0], **args[1], **kwargs
             )
         if function in __other_functions__:
-            return _get_new_csdm_object_after_applying_function(
+            return get_new_csdm_object_after_applying_function(
                 function, *args[0], **args[1], **kwargs
             )
+        if function in __array_manipulation__:
+            csdm = args[0][0]
+            args_ = ()
+            if len(args[0]) > 1:
+                args_ = args[0][1:]
+            args_kw = args[1]
+            return get_new_csdm_object_after_applying_ufunc(
+                csdm, function, None, None, *args_, **args_kw
+            )
+        if function in [np.pad]:
+            return apply_np_padding(function, *args, **kwargs)
+
         if function in __shape_manipulation_functions__:
+            dim_len = len(args[0][0].dimensions)
             if "axes" in args[1].keys():
-                args[1]["axes"] = (0,) + tuple(np.asarray(args[1]["axes"]) + 1)
+                axes = (0,) + tuple(-np.asarray(args[1]["axes"]) - 1)
+                axes_dim = args[1]["axes"]
+                args[1]["axes"] = axes
+
+            elif len(args[0]) == 2:
+                args = list(args)
+                args[0] = list(args[0])
+                axes = (0,) + tuple(-np.asarray(args[0][1]) - 1)
+                axes_dim = args[0][1]
+                args[0][1] = axes
             else:
-                dim_len = len(args[0][0].dimensions)
-                args[1]["axes"] = (0,) + tuple(-i - 1 for i in range(dim_len))
+                axes = (0,) + tuple(-i - 1 for i in range(dim_len))
+                axes_dim = np.arange(dim_len)[::-1]
+                args[1]["axes"] = axes
 
-            csdm = _get_new_csdm_object_after_applying_function(
+            csdm = get_new_csdm_object_after_applying_function(
                 function, *args[0], **args[1], **kwargs
             )
+
             csdm._dimensions = tuple(
-                csdm.dimensions[args[1]["axes"][1:][i]]
-                for i in range(len(csdm.dimensions))
+                csdm.dimensions[axes_dim[i]] for i in range(len(csdm.dimensions))
             )
+            return csdm
 
         # if function in __return_np__:
         #     if len(self.y) > 1:
         #         raise NotImplementedError(
         #             f"Function {function.__name__} is not implemented for multi "
         #              "dependent variable csdm object."
         #         )
-        #     csdm, args_, axis, kwargs = _get_CSDM_object__args__axes(
+        #     csdm, args_, axis, kwargs = get_CSDM_object__args__axes(
         #         *args[0], **args[1], **kwargs
         #     )
         #     nd_array = csdm.y[0].components
         #     return function(nd_array, *args_, **kwargs)
 
         raise NotImplementedError(f"Function {function.__name__} is not implemented.")
 
@@ -1429,93 +1431,124 @@
             A matplotlib figure instance.
 
         Example:
             >>> cp.plot(data_object) # doctest: +SKIP
         """
         return _preview(self, reverse_axis, range, **kwargs)
 
+    def to_positive_inc(self):
+        """Convert the csdm object with negative increment dimensions to positive
+        increments.
 
-def _check_for_out(csdm, **kwargs):
-    out = kwargs.get("out", None)
-    if out is not None:
-        if len(csdm.dependent_variables) > 1:
-            raise NotImplementedError(
-                "Keyword `out` is not implemented for csdm objects with more that "
-                "one dependent variables."
+        Args:
+            csdm_obj: CSDM object
+        """
+        reverse_index = []
+        new_dimensions = []
+        for i, dim in enumerate(self.dimensions):
+            if dim.type in ["linear", "monotonic"]:
+                diff = dim.coordinates[1] - dim.coordinates[0]
+                if diff.value < 0:
+                    reverse_index.append(-i - 1)
+                    coords = dim.coordinates
+                    array, unit = coords.value[::-1], coords.unit
+                    new_axis = as_dimension(array=array, unit=str(unit))
+                    new_axis.copy_metadata(dim)
+                    new_dimensions.append(new_axis)
+                else:
+                    new_dimensions.append(dim)
+            else:
+                new_dimensions.append(dim)
+
+        new_dvs = []
+        for d_v in self.dependent_variables:
+            datum = d_v.components
+            datum = (
+                datum
+                if reverse_index == []
+                else np.flip(datum, axis=tuple(reverse_index))
             )
+            new_dv = as_dependent_variable(array=datum)
+            new_dv.copy_metadata(d_v)
+            new_dvs.append(new_dv)
 
+        new_csdm = CSDM(dimensions=new_dimensions, dependent_variables=new_dvs)
+        new_csdm.copy_metadata(self)
 
-def _get_new_csdm_object_after_applying_ufunc(
+        return new_csdm
+
+
+def get_new_csdm_object_after_applying_ufunc(
     csdm, func, method=None, factor=None, *inputs, **kwargs
 ):
     """Perform the operation, func, on the components of the dependent variables, and
     return the corresponding CSDM object.
     """
     if factor is None:
         factor = np.ones(len(csdm.dependent_variables))
     axis = kwargs.get("axis", None)
     if axis is not None:
         kwargs["axis"] = _check_dimension_indices(len(csdm.dimensions), axis)
 
-    _check_for_out(csdm, **kwargs)
+    np_check_for_out(csdm, **kwargs)
 
     new = CSDM()
 
     # dimension should be added first so that the dependent variables can be
     # shaped appropriately.
     new._dimensions = deepcopy(csdm.dimensions)
 
     for i, variable in enumerate(csdm.dependent_variables):
         res = func(variable.components * factor[i], *inputs, **kwargs)
 
         obj = empty_dependent_variable(
             numeric_type=res.dtype, quantity_type=variable.quantity_type
         )
-        obj._copy_metadata(variable)
+        obj.copy_metadata(variable)
         obj.subtype._components = res
         new._dependent_variables += [obj]
         # obj = as_dependent_variable(y, quantity_type=variable.quantity_type)
-        # obj._copy_metadata(variable)
+        # obj.copy_metadata(variable)
         # new.add_dependent_variable(obj)
 
-    new._copy_metadata(csdm)
+    new.copy_metadata(csdm)
     return new
 
 
-def _get_new_csdm_object_after_applying_function(func, *args, **kwargs):
+def get_new_csdm_object_after_applying_function(func, *args, **kwargs):
     """Perform the operation, func, on the components of the dependent variables, and
     return the corresponding CSDM object.
     """
     args_ = []
     csdm = args[0]
     if len(args) > 1:
         args_ = args[1:]
 
-    _check_for_out(csdm, **kwargs)
+    np_check_for_out(csdm, **kwargs)
 
     new = CSDM()
 
     # dimension should be added first so that the dependent variables can be
     # shaped appropriately.
     new._dimensions = deepcopy(csdm.dimensions)
 
     for variable in csdm.dependent_variables:
-        y = func(variable.components, *args_, **kwargs)
+        components = func(variable.components, *args_, **kwargs)
         obj = empty_dependent_variable(
-            numeric_type=y.dtype, quantity_type=variable.quantity_type
+            numeric_type=components.dtype, quantity_type=variable.quantity_type
         )
-        obj._copy_metadata(variable)
-        obj.subtype._components = y
+        obj.copy_metadata(variable)
+        obj.subtype._components = components
         new._dependent_variables += [obj]
 
-    new._copy_metadata(csdm)
+    new.copy_metadata(csdm)
     return new
 
 
-def _get_new_csdm_object_after_apodization(csdm, func, arg, index=-1):
+def get_new_csdm_object_after_apodization(csdm, func, arg, index=-1):
     """Perform the operation, func, on the components of the dependent variables, and
     return the corresponding CSDM object.
     """
     index = _check_dimension_indices(len(csdm.dimensions), index)
     index = [index] if isinstance(index, int) else index
 
     quantity = string_to_quantity(arg)
@@ -1541,97 +1574,113 @@
     new = CSDM()
 
     # dimension should be added first so that the dependent variables can be
     # shaped appropriately.
     new._dimensions = deepcopy(csdm.dimensions)
 
     for variable in csdm.dependent_variables:
-        y = variable.components * apodization_vector_nd
+        components = variable.components * apodization_vector_nd
 
         obj = empty_dependent_variable(
-            numeric_type=y.dtype, quantity_type=variable.quantity_type
+            numeric_type=components.dtype, quantity_type=variable.quantity_type
         )
-        obj._copy_metadata(variable)
-        obj.subtype._components = y
+        obj.copy_metadata(variable)
+        obj.subtype._components = components
         new._dependent_variables += [obj]
 
         # obj = as_dependent_variable(y, quantity_type=variable.quantity_type)
-        # obj._copy_metadata(variable)
+        # obj.copy_metadata(variable)
         # new.add_dependent_variable(obj)
 
-    new._copy_metadata(csdm)
+    new.copy_metadata(csdm)
     return new
 
 
-def _get_CSDM_object__args__axes(*args, **kwargs):
-    # print(args)
-    axis = None
-    args_ = []
-    if args != ():
-        csdm = args[0]
-        args_ = list(args[1:])
-        if len(args) > 1:
-            args_[0] = _check_dimension_indices(len(csdm.dimensions), args[1])
-            axis = args_[0]
-    if "a" in kwargs.keys():
-        csdm = kwargs["a"]
-        kwargs.pop("a")
-    if "axis" in kwargs.keys():
-        if kwargs["axis"] is not None:
-            axis = _check_dimension_indices(len(csdm.dimensions), kwargs["axis"])
-            kwargs["axis"] = axis
-
-    _check_for_out(csdm, **kwargs)
-    return csdm, args_, axis, kwargs
-
-
-def _get_new_csdm_object_after_dimension_reduction_func(func, *args, **kwargs):
+def get_new_csdm_object_after_dimension_reduction_func(func, *args, **kwargs):
     """Perform the operation, func, on the components of the dependent variables, and
     return the corresponding CSDM object.
     """
-    csdm, args_, axis, kwargs = _get_CSDM_object__args__axes(*args, **kwargs)
+    csdm, args_, axis, kwargs = get_CSDM_object__args__axes(*args, **kwargs)
 
     new = CSDM()
     lst = []
 
     axis = [axis] if isinstance(axis, int) else axis
     # dimension should be added first so that the dependent variables can be
     # shaped appropriately.
     if axis is not None:
         for i, variable in enumerate(csdm.dimensions):
             if -1 - i not in axis:
                 new.dimensions.append(variable.copy())
 
     for variable in csdm.dependent_variables:
-        y = func(variable.components, *args_, **kwargs)
+        components = func(variable.components, *args_, **kwargs)
 
         if axis is not None:
             obj = empty_dependent_variable(
-                numeric_type=y.dtype, quantity_type=variable.quantity_type
+                numeric_type=components.dtype, quantity_type=variable.quantity_type
             )
-            obj._copy_metadata(variable)
-            obj.subtype._components = y
+            obj.copy_metadata(variable)
+            obj.subtype._components = components
             new._dependent_variables += [obj]
 
             # obj = as_dependent_variable(y, quantity_type=variable.quantity_type)
-            # obj._copy_metadata(variable)
+            # obj.copy_metadata(variable)
             # new.add_dependent_variable(obj)
         else:
-            lst.append(y * variable.unit)
+            lst.append(components * variable.unit)
 
     if axis is None:
         del new
-        # if len(lst) > 1:
-        #     return lst
         return lst if len(lst) > 1 else lst[0]
 
-    new._copy_metadata(csdm)
+    new.copy_metadata(csdm)
     return new
 
 
 def empty_dependent_variable(numeric_type, quantity_type="scalar"):
+    """Create an empty dependent variable object"""
     return DependentVariable(
         type="internal",
         components=np.empty(0),
         quantity_type=quantity_type,
         numeric_type=numeric_type,
     )
+
+
+def apply_np_padding(function, *args, **kwargs):
+    """Apply numpy padding"""
+    args0 = list(args[0])
+    n_dims = len(args0[0].x)
+    if "pad_width" in args[1].keys():
+        pads = np_check_pads(args[1]["pad_width"], n_dims)
+        pads = ((0, 0),) + tuple(pads)[::-1]
+        args[1]["pad_width"] = pads
+    else:
+        pads = np_check_pads(args0[1], n_dims)
+        pads = ((0, 0),) + tuple(pads)[::-1]
+        args0[1] = pads
+
+    for key, val in args[1].items():
+        if key in ["stat_length", "constant_values", "end_values"]:
+            args[1][key] = ((0, 0),) + tuple(np_check_pads(val, n_dims))[::-1]
+
+    csdm = get_new_csdm_object_after_applying_function(
+        function, *args0, **args[1], **kwargs
+    )
+    for dim, pads in zip(csdm.dimensions, pads[::-1][:-1]):
+        if dim.type == "linear":
+            dim.count += int(np.sum(pads))
+            offset = int(pads[0] / 2 - 1) if dim.complex_fft else pads[0]
+            dim.coordinates_offset -= dim.increment * offset
+        if dim.type == "monotonic":
+            inc = dim.coordinates[1] - dim.coordinates[0]
+            left = inc * (np.arange(pads[0]) - pads[0]) + dim.coordinates[0]
+            right = inc * np.arange(pads[1]) + dim.coordinates[0]
+            coords = np.concatenate((left, dim.coordinates, right))
+            dim.coordinates = coords
+        if dim.type == "labeled":
+            left = ["0"] * pads[0]
+            right = ["0"] * pads[1]
+            coords = left + list(dim.labels) + right
+            dim.labels = coords
+    return csdm
```

### Comparing `csdmpy-0.5/csdmpy/dependent_variable/__init__.py` & `csdmpy-0.6.dev2/csdmpy/dependent_variable/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import warnings
 from copy import deepcopy
 
 import numpy as np
 
 from csdmpy.dependent_variable.external import ExternalDataset
 from csdmpy.dependent_variable.internal import InternalDataset
-from csdmpy.utils import _axis_label  # lgtm [py/import-own-module]
-from csdmpy.utils import _get_dictionary  # lgtm [py/import-own-module]
+from csdmpy.utils import _axis_label
+from csdmpy.utils import _get_dictionary
 
 __author__ = "Deepansh J. Srivastava"
 __email__ = "srivastava.89@osu.edu"
 __all__ = ["DependentVariable"]
 
 
 class DependentVariable:
@@ -188,19 +188,14 @@
         model, however, it is a convenient supplementary attribute that provides
         formatted string ready for labeling the components of the dependent variable.
         The string at index `i` is formatted as `component_labels[i] / unit` if
         `component_labels[i]` is a non-empty string, otherwise, `quantity_name / unit`.
         Here, `quantity_name`, `component_labels`, and `unit`are the attributes of the
         :ref:`dv_api` instance. For example,
 
-        .. doctest::
-
-            >>> y.axis_label
-            ['energy / (s W)', 'energy / (s W)', 'energy / (s W)']
-
         Returns:
             A list of formatted component label strings.
 
         Raises:
             AttributeError: When assigned a value.
         """
         labels = []
@@ -344,38 +339,14 @@
         """Json serialized string describing the DependentVariable class instance.
 
         This supplementary attribute is useful for a quick preview of the dependent
         variable object. For convenience, the values from the `components` attribute
         are truncated to the first and the last two numbers per component.
         The `encoding` keyword is also hidden from this view.
 
-        .. doctest::
-
-            >>> print(y.data_structure)
-            {
-              "type": "internal",
-              "description": "A test image",
-              "name": "star",
-              "unit": "s * W",
-              "quantity_name": "energy",
-              "numeric_type": "float32",
-              "quantity_type": "pixel_3",
-              "components": [
-                [
-                  "0.0, 1.0, ..., 8.0, 9.0"
-                ],
-                [
-                  "10.0, 11.0, ..., 18.0, 19.0"
-                ],
-                [
-                  "20.0, 21.0, ..., 28.0, 29.0"
-                ]
-              ]
-            }
-
         Returns:
             A json serialized string of the dependent variable object.
 
         Raises:
             AttributeError: When modified.
         """
         return json.dumps(
@@ -629,19 +600,14 @@
         """Unit associated with the dependent variable.
 
         .. note::
             The attribute cannot be modified. To convert the unit, use the
             :meth:`~csdmpy.DependentVariable.to` method of
             the class instance.
 
-        .. doctest::
-
-            >>> y.unit
-            Unit("s W")
-
         Returns:
             A `Unit` object from astropy.unit package.
 
         Raises:
             AttributeError: When assigned a value.
         """
         return self.subtype.unit
@@ -662,16 +628,14 @@
 
         Args:
             unit: A string containing a unit with the same dimensionality as the
                   components of the dependent variable.
 
         .. doctest::
 
-            >>> y.unit
-            Unit("s W")
             >>> print(y.components[0, 5])
             5.0
             >>> y.to("mJ")
             >>> y.unit
             Unit("mJ")
             >>> print(y.components[0, 5])
             5000.0
@@ -739,15 +703,15 @@
         if item._sparse_sampling == {}:
             item._components = np.asarray(
                 item._components[:, :grid_points].reshape(sub_shape), dtype=dtype
             )
         else:
             item._components = fill_sparse_space(item, sub_shape, dtype)
 
-    def _copy_metadata(self, obj, copy=False):
+    def copy_metadata(self, obj, copy=False):
         """Copy DependentVariable metadata"""
 
         self.type = obj.type
         self.subtype._description = obj.subtype._description
         self.subtype._name = obj.subtype._name
         self.subtype._unit = obj.subtype._unit
         self.subtype._quantity_name = obj.subtype._quantity_name
```

### Comparing `csdmpy-0.5/csdmpy/dependent_variable/base_class.py` & `csdmpy-0.6.dev2/csdmpy/dependent_variable/base_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         obj["description"] = self._description.strip()
         obj["name"] = self._name.strip()
         obj["unit"] = (
             ScalarQuantity(1.0 * self._unit).__format__("unit")
             if str(self._unit) != ""
             else ""
         )
-        obj["quantity_name"] = self._quantity_name
+        obj["quantity_name"] = self.quantity_name
         obj["encoding"] = str(self._encoding)
         obj["numeric_type"] = str(self._numeric_type)
         obj["quantity_type"] = str(self._quantity_type)
 
         for label in self._component_labels:
             if label.strip() != "":
                 obj["component_labels"] = self._component_labels
```

### Comparing `csdmpy-0.5/csdmpy/dependent_variable/decoder.py` & `csdmpy-0.6.dev2/csdmpy/dependent_variable/decoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 __email__ = "srivastava.89@osu.edu"
 __all__ = ["Decoder"]
 
 
 class Decoder:
     """Decoder class"""
 
-    def __new__(self, encoding, quantity_type, components, dtype):
+    def __new__(cls, encoding, quantity_type, components, dtype):
         """Decode the components based on the encoding key value.
 
         The valid encodings are 'base64', 'none' (text), and 'raw' (binary).
         """
         if encoding != "raw":
             check_number_of_components_and_encoding_type(len(components), quantity_type)
         component_len = quantity_type.p
-        method = getattr(self, "decode_" + encoding)
+        method = getattr(cls, "decode_" + encoding)
         return method(components, dtype, component_len)
 
     @staticmethod
     def decode_base64(components, dtype, component_len=None):
         """Read components form a base64 buffer"""
         components = np.asarray(
             [np.frombuffer(base64.b64decode(item), dtype=dtype) for item in components]
@@ -46,15 +46,16 @@
             else np.asarray(components, dtype=dtype)
         )
 
     @staticmethod
     def decode_raw(components, dtype, component_len=None):
         """Read components form a binary buffer"""
         components = np.frombuffer(components, dtype=dtype)
-        components.shape = component_len, int(components.size / component_len)
+        size = int(components.size / component_len)
+        components = components.reshape(component_len, size)
         return components
 
 
 def check_number_of_components_and_encoding_type(length, quantity_type):
     """Verify the consistency of encoding wrt the number of components."""
     if length != quantity_type.p:
         raise Exception(
```

### Comparing `csdmpy-0.5/csdmpy/dependent_variable/download.py` & `csdmpy-0.6.dev2/csdmpy/dependent_variable/download.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/csdmpy/dependent_variable/external.py` & `csdmpy-0.6.dev2/csdmpy/dependent_variable/external.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/csdmpy/dependent_variable/internal.py` & `csdmpy-0.6.dev2/csdmpy/dependent_variable/internal.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 self._quantity_type,
                 components,
                 self._numeric_type.dtype,
             )
 
         size = self._components.size
         p_1 = self.quantity_type.p
-        self._components.shape = (p_1, int(size / p_1))
+        self._components = self._components.reshape(p_1, int(size / p_1))
 
     def dict(self, filename=None, dataset_index=None, for_display=False):
         """Return InternalDataset object as a python dictionary."""
         dictionary = {}
         dictionary["type"] = "internal"
         dictionary.update(super().dict(filename, dataset_index, for_display))
         return dictionary
```

### Comparing `csdmpy-0.5/csdmpy/dependent_variable/sparse.py` & `csdmpy-0.6.dev2/csdmpy/dependent_variable/sparse.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,25 +23,15 @@
         "_encoding",
         "_quantity_type",
         "_unsigned_integer_type",
         "_description",
         "_application",
     )
 
-    def __init__(
-        self,
-        # dimension_indexes,
-        # sparse_grid_vertexes,
-        # encoding="none",
-        # quantity_type="scalar",
-        # unsigned_integer_type="int64",
-        # description="",
-        # application={},
-        **kwargs,
-    ):
+    def __init__(self, **kwargs):
         """Initialize a SparseDimension class."""
         default = {
             "encoding": "none",
             "quantity_type": "scalar",
             "unsigned_integer_type": "uint64",
             "description": "",
             "application": None,
```

### Comparing `csdmpy-0.5/csdmpy/dimension/__init__.py` & `csdmpy-0.6.dev2/csdmpy/dimension/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from copy import deepcopy
 
 import numpy as np
 
 from csdmpy.dimension.labeled import LabeledDimension
 from csdmpy.dimension.linear import LinearDimension
 from csdmpy.dimension.monotonic import MonotonicDimension
-from csdmpy.units import string_to_quantity  # lgtm [py/import-own-module]
-from csdmpy.utils import _get_dictionary  # lgtm [py/import-own-module]
-from csdmpy.utils import validate  # lgtm [py/import-own-module]
+from csdmpy.units import string_to_quantity
+from csdmpy.utils import _get_dictionary
+from csdmpy.utils import validate
 
 __author__ = "Deepansh J. Srivastava"
 __email__ = "srivastava.89@osu.edu"
 __all__ = ["Dimension"]
 
 
 functional_dimension = ["linear"]
@@ -171,29 +171,58 @@
 
     def __eq__(self, other):
         """Overrides the default implementation."""
         other = other.subtype if isinstance(other, Dimension) else other
         return True if self.subtype == other else False
 
     def __mul__(self, other):
-        """Multiply the Dimension object by a scalar."""
+        """Multiply the Dimension object by a right scalar."""
         return self.subtype.__mul__(other)
 
+    def __rmul__(self, other):
+        """Multiply the Dimension object by a left scalar."""
+        return self.subtype.__rmul__(other)
+
     def __imul__(self, other):
         """Multiply the Dimension object by a scalar, in-place."""
         return self.subtype.__imul__(other)
 
     def __truediv__(self, other):
         """Divide the Dimension object by a scalar."""
         return self.subtype.__truediv__(other)
 
     def __itruediv__(self, other):
         """Divide the Dimension object by a scalar, in-place."""
         return self.subtype.__itruediv__(other)
 
+    def __getitem__(self, indices):
+        """Return a dimension object corresponding to given indices."""
+        dim_ = self.subtype if hasattr(self, "subtype") else self
+
+        length_ = self.coordinates[indices].size
+        if length_ <= 1:
+            return self.coordinates[indices]
+
+        if hasattr(dim_, "_equivalencies"):
+            equivalencies_ = dim_._equivalencies
+            dim_._equivalencies = None
+            coordinates = self.coordinates[indices]
+            new_dim = as_dimension(coordinates.value, unit=str(coordinates.unit))
+            dim_._equivalencies = equivalencies_
+            new_dim._equivalencies = equivalencies_
+
+        else:
+            coordinates = self.coordinates[indices]
+            new_dim = as_dimension(coordinates)
+
+        new_dim.copy_metadata(dim_)
+        if hasattr(new_dim, "complex_fft"):
+            new_dim.complex_fft = False
+        return new_dim
+
     # ======================================================================= #
     #                          Dimension Attributes                           #
     # ======================================================================= #
     @property
     def absolute_coordinates(self):
         r"""Absolute coordinates, :math:`\bf X_k^{\rm{abs}}`, along the dimension.
 
@@ -529,14 +558,19 @@
         return self.subtype.label
 
     @label.setter
     def label(self, label=""):
         self.subtype.label = label
 
     @property
+    def size(self):
+        """Return the dimension count"""
+        return self.count
+
+    @property
     def count(self):
         r"""Number of coordinates, :math:`N_k \ge 1`, along the dimension.
 
         Example:
             >>> print(x.count)
             10
             >>> x.count = 5
@@ -722,18 +756,17 @@
         """
         return self.subtype.reciprocal
 
     # ======================================================================= #
     #                           Dimension Methods                             #
     # ======================================================================= #
 
-    def _copy_metadata(self, obj):
+    def copy_metadata(self, obj):
         """Copy Dimension metadata"""
-        self.subtype._type = obj.subtype._type
-        self.subtype._copy_metadata(obj)
+        self.subtype.copy_metadata(obj)
 
     def to_dict(self):
         """Alias to the `dict()` method of the class."""
         return self.dict()
 
     def dict(self):
         """Return Dimension object as a python dictionary.
```

### Comparing `csdmpy-0.5/csdmpy/dimension/base.py` & `csdmpy-0.6.dev2/csdmpy/dimension/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,19 @@
         return self.coordinates
 
     @coords.setter
     def coords(self, value):
         self.coordinates = value
 
     @property
+    def size(self):
+        """Return the dimension count"""
+        return self.coordinates.size
+
+    @property
     def axis_label(self):
         """Return a formatted string for displaying label along the dimension axis."""
         return self.label
 
     def to_dict(self):
         """Alias to the `dict()` method of the class."""
         return self.dict()
```

### Comparing `csdmpy-0.5/csdmpy/dimension/labeled.py` & `csdmpy-0.6.dev2/csdmpy/dimension/labeled.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     def coordinates(self, value):
         self.labels = value
 
     # ----------------------------------------------------------------------- #
     #                                 Methods                                 #
     # ----------------------------------------------------------------------- #
 
-    def _copy_metadata(self, obj):
+    def copy_metadata(self, obj):
         """Copy LabeledDimension metadata."""
         obj = obj.subtype if hasattr(obj, "subtype") else obj
         if isinstance(obj, LabeledDimension):
             _copy_core_metadata(self, obj, "labeled")
 
     def dict(self):
         """Return the LabeledDimension as a python dictionary."""
```

### Comparing `csdmpy-0.5/csdmpy/dimension/linear.py` & `csdmpy-0.6.dev2/csdmpy/dimension/linear.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,19 @@
         if not isinstance(other, LinearDimension):
             return False
         check = [getattr(self, _) == getattr(other, _) for _ in __class__.__slots__[:4]]
         check += [super().__eq__(other)]
         return np.all(check)
 
     def __mul__(self, other):
-        """Multiply the LinearDimension object by a scalar."""
+        """Multiply the LinearDimension object by a right scalar."""
+        return _update_linear_dimension_object_by_scalar(self.copy(), other, "mul")
+
+    def __rmul__(self, other):
+        """Multiply the LinearDimension object by a left scalar."""
         return _update_linear_dimension_object_by_scalar(self.copy(), other, "mul")
 
     def __imul__(self, other):
         """Multiply the LinearDimension object by a scalar, in-place."""
         return _update_linear_dimension_object_by_scalar(self, other, "mul")
 
     def __truediv__(self, other):
@@ -163,15 +167,15 @@
         equivalent_fn = self._equivalencies
         equivalent_unit = self._equivalent_unit
 
         if equivalent_fn is None or equivalent_unit is None:
             return coordinates.to(self._unit)
 
         if equivalent_fn == "nmr_frequency_ratio":
-            denominator = self.origin_offset - self.get_nmr_reference_offset()
+            denominator = self.origin_offset  # - self.get_nmr_reference_offset()
             if denominator.value == 0:
                 raise ZeroDivisionError("Cannot convert the coordinates to ppm.")
             return coordinates.to(equivalent_unit, frequency_ratio(denominator))
 
         return coordinates.to(equivalent_unit, equivalent_fn)
 
     @coordinates.setter
@@ -198,15 +202,15 @@
         # negative increment
         return self.coordinates_offset + (count - 1) * self.increment
 
     # ----------------------------------------------------------------------- #
     #                                 Methods                                 #
     # ----------------------------------------------------------------------- #
 
-    def _copy_metadata(self, obj):
+    def copy_metadata(self, obj):
         """Copy LinearDimension metadata."""
         obj = obj.subtype if hasattr(obj, "subtype") else obj
         if isinstance(obj, LinearDimension):
             _copy_core_metadata(self, obj, "linear")
 
     def dict(self):
         """Return the LinearDimension as a python dictionary."""
```

### Comparing `csdmpy-0.5/csdmpy/dimension/monotonic.py` & `csdmpy-0.6.dev2/csdmpy/dimension/monotonic.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,19 @@
         properties = ", ".join([f"coordinates={self._coordinates.__str__()}", *meta])
         return f"MonotonicDimension({properties})"
 
     def __str__(self):
         return f"MonotonicDimension({self.coordinates.__str__()})"
 
     def __mul__(self, other):
-        """Multiply the MonotonicDimension object by a scalar."""
+        """Multiply the MonotonicDimension object by a right scalar."""
+        return _update_monotonic_dimension_object_by_scalar(self.copy(), other, "mul")
+
+    def __rmul__(self, other):
+        """Multiply the MonotonicDimension object by a left scalar."""
         return _update_monotonic_dimension_object_by_scalar(self.copy(), other, "mul")
 
     def __imul__(self, other):
         """Multiply the MonotonicDimension object by a scalar, in-place."""
         return _update_monotonic_dimension_object_by_scalar(self, other, "mul")
 
     def __truediv__(self, other):
@@ -162,15 +166,15 @@
     def coordinates(self, value):
         self._get_coordinates(value)
 
     # ------------------------------------------------------------------------------- #
     #                                     Methods                                     #
     # ------------------------------------------------------------------------------- #
 
-    def _copy_metadata(self, obj):
+    def copy_metadata(self, obj):
         """Copy MonotonicDimension metadata."""
         obj = obj.subtype if hasattr(obj, "subtype") else obj
         if isinstance(obj, MonotonicDimension):
             _copy_core_metadata(self, obj, "monotonic")
 
     def dict(self):
         """Return the MonotonicDimension as a python dictionary."""
```

### Comparing `csdmpy-0.5/csdmpy/dimension/quantitative.py` & `csdmpy-0.6.dev2/csdmpy/dimension/quantitative.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,16 +140,16 @@
 
         if self._coordinates_offset.value != 0.0:
             obj["coordinates_offset"] = str(ScalarQuantity(self._coordinates_offset))
 
         if self._origin_offset.value != 0.0:
             obj["origin_offset"] = str(ScalarQuantity(self._origin_offset))
 
-        if self._quantity_name not in [None, "unknown", "dimensionless"]:
-            obj["quantity_name"] = self._quantity_name
+        if self.quantity_name not in [None, "unknown", "dimensionless"]:
+            obj["quantity_name"] = self.quantity_name
 
         if self._period.value not in [0.0, np.inf]:
             obj["period"] = str(ScalarQuantity(self._period))
 
         obj.update(super().dict())
         return obj
```

### Comparing `csdmpy-0.5/csdmpy/helper_functions.py` & `csdmpy-0.6.dev2/csdmpy/helper_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,15 @@
         cs = ax.imshow(y00, **kwargs)
     else:
         if "interpolation" not in kwargs.keys():
             kwargs["interpolation"] = "nearest"
 
         cs = NonUniformImage(ax, **kwargs)
         cs.set_data(x0, x1, y00)
-        ax.images.append(cs)
+        ax.add_artist(cs)
 
     cbar = ax.figure.colorbar(cs, ax=ax)
     cbar.ax.minorticks_off()
     cbar.set_label(y.axis_label[0])
     ax.set_xlim([extent[0], extent[1]])
     ax.set_ylim([extent[2], extent[3]])
     ax.set_xlabel(f"{x[0].axis_label} - 0")
```

### Comparing `csdmpy-0.5/csdmpy/numpy_wrapper/apodize.py` & `csdmpy-0.6.dev2/csdmpy/numpy_wrapper/apodize.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 The list of supported functions are:
     - sin
     - cos
     - ...
 """
 import numpy as np
 
-from csdmpy.csdm import _get_new_csdm_object_after_apodization
+from csdmpy.csdm import get_new_csdm_object_after_apodization
 
 __all__ = ("sin", "cos", "tan", "arcsin", "arccos", "arctan", "exp")
 
 
 # Trigonometric functions
 
 
@@ -33,15 +33,15 @@
         dimension: An integer or tuple of `m` integers cooresponding to the
                    index/indices of the dimensions along which the sine of the
                    dependent variable components is performed.
     Return:
         A CSDM object with `d-m` dimensions, where `d` is the total
         number of dimensions from the original `csdm` object.
     """
-    return _get_new_csdm_object_after_apodization(csdm, np.sin, arg, dimension)
+    return get_new_csdm_object_after_apodization(csdm, np.sin, arg, dimension)
 
 
 def cos(csdm, arg, dimension=0):
     r"""Apodize the components along the `dimension` with :math:`\cos(a x)`.
 
     Args:
         csdm: A CSDM object.
@@ -49,15 +49,15 @@
         dimension: An integer or tuple of `m` integers cooresponding to the
                    index/indices of the dimensions along which the cosine of the
                    dependent variable components is performed.
     Return:
         A CSDM object with `d-m` dimensions, where `d` is the total
         number of dimensions from the original `csdm` object.
     """
-    return _get_new_csdm_object_after_apodization(csdm, np.cos, arg, dimension)
+    return get_new_csdm_object_after_apodization(csdm, np.cos, arg, dimension)
 
 
 def tan(csdm, arg, dimension=0):
     r"""Apodize the components along the `dimension` with :math:`\tan(a x)`.
 
     Args:
         csdm: A CSDM object.
@@ -65,15 +65,15 @@
         dimension: An integer or tuple of `m` integers cooresponding to the
                    index/indices of the dimensions along which the tangent of the
                    dependent variable components is performed.
     Return:
         A CSDM object with `d-m` dimensions, where `d` is the total
         number of dimensions from the original `csdm` object.
     """
-    return _get_new_csdm_object_after_apodization(csdm, np.tan, arg, dimension)
+    return get_new_csdm_object_after_apodization(csdm, np.tan, arg, dimension)
 
 
 def arcsin(csdm, arg, dimension=0):
     r"""Apodize the components along the `dimension` with :math:`\arcsin(a x)`.
 
     Args:
         csdm: A CSDM object.
@@ -81,15 +81,15 @@
         dimension: An integer or tuple of `m` integers cooresponding to the
                    index/indices of the dimensions along which the inverse sine of the
                    dependent variable components is performed.
     Return:
         A CSDM object with `d-m` dimensions, where `d` is the total
         number of dimensions from the original `csdm` object.
     """
-    return _get_new_csdm_object_after_apodization(csdm, np.arcsin, arg, dimension)
+    return get_new_csdm_object_after_apodization(csdm, np.arcsin, arg, dimension)
 
 
 def arccos(csdm, arg, dimension=0):
     r"""Apodize the components along the `dimension` with :math:`\arccos(a x)`.
 
     Args:
         csdm: A CSDM object.
@@ -97,15 +97,15 @@
         dimension: An integer or tuple of `m` integers cooresponding to the
                    index/indices of the dimensions along which the inverse cosine of
                    the dependent variable components is performed.
     Return:
         A CSDM object with `d-m` dimensions, where `d` is the total
         number of dimensions from the original `csdm` object.
     """
-    return _get_new_csdm_object_after_apodization(csdm, np.arccos, arg, dimension)
+    return get_new_csdm_object_after_apodization(csdm, np.arccos, arg, dimension)
 
 
 def arctan(csdm, arg, dimension=0):
     r"""Apodize the components along the `dimension` with :math:`\arctan(a x)`.
 
     Args:
         csdm: A CSDM object.
@@ -113,15 +113,15 @@
         dimension: An integer or tuple of `m` integers cooresponding to the
                    index/indices of the dimensions along which the inverse tangent of
                    the dependent variable components is performed.
     Return:
         A CSDM object with `d-m` dimensions, where `d` is the total
         number of dimensions from the original `csdm` object.
     """
-    return _get_new_csdm_object_after_apodization(csdm, np.arctan, arg, dimension)
+    return get_new_csdm_object_after_apodization(csdm, np.arctan, arg, dimension)
 
 
 def exp(csdm, arg, dimension=0):
     r"""Apodize the components along the `dimension` with :math:`\exp(a x)`.
 
     Args:
         csdm: A CSDM object.
@@ -129,8 +129,8 @@
         dimension: An integer or tuple of `m` integers cooresponding to the
                    index/indices of the dimensions along which the exp of the
                    dependent variable components is performed.
     Return:
         A CSDM object with `d-m` dimensions, where `d` is the total
         number of dimensions from the original `csdm` object.
     """
-    return _get_new_csdm_object_after_apodization(csdm, np.exp, arg, dimension)
+    return get_new_csdm_object_after_apodization(csdm, np.exp, arg, dimension)
```

### Comparing `csdmpy-0.5/csdmpy/statistics.py` & `csdmpy-0.6.dev2/csdmpy/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,18 @@
         A list of integrals corresponding to the list of the dependent variables. If
         only one dependent variable is present, return a quantity instead.
 
     Example:
         >>> import csdmpy.statistics as stat
         >>> x = np.arange(100) * 2 - 100.0
         >>> gauss = np.exp(-((x - 5.) ** 2) / (2 * 4. ** 2))
-        >>> csdm = cp.as_csdm(gauss, unit='T')
+        >>> csdm = cp.as_csdm(gauss, unit='T/m')
         >>> csdm.dimensions[0] = cp.as_dimension(x, unit="m")
         >>> stat.integral(csdm)
-        <Quantity 10.0265131 m T>
+        <Quantity 10.0265131 T>
     """
     dim_l = len(csdm.dimensions)
     _check_dimension_type(csdm)
 
     intervals = [item.coordinates[1] - item.coordinates[0] for item in csdm.dimensions]
     i = 1.0
     for _ in range(dim_l):
```

### Comparing `csdmpy-0.5/csdmpy/units.py` & `csdmpy-0.6.dev2/csdmpy/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,21 +209,21 @@
     def __format__(self, format="quantity"):
         """Format the units according to csdmpy recommendation.
 
         :ivar: format: The value can either be 'quantity' or 'unit'
 
         .. doctest::
 
-            >>> a = ScalarQuantity("5 kg m^2 /s")
+            >>> a = ScalarQuantity("5 m /s")
             >>> print(a.quantity)
-            5.0 kg m2 / s
+            5.0 m / s
             >>> print(str(ScalarQuantity(a.quantity)))
-            5.0 kg * m^2 * s^-1
+            5.0 m * s^-1
             >>> print(ScalarQuantity(a.quantity).__format__("unit"))
-            kg * m^2 * s^-1
+            m * s^-1
         """
 
         element = _default_units(self.quantity)
         if format == "unit":
             return scalar_quantity_format(element, numerical_value=False)
         if format == "quantity":
             return scalar_quantity_format(element)
```

### Comparing `csdmpy-0.5/csdmpy/utils.py` & `csdmpy-0.6.dev2/csdmpy/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -317,24 +317,32 @@
     ScalarQuantity.
 
     Returns: The other object.
     """
     if isinstance(other, numpy_scalars):
         return other
 
+    if other.__class__.__name__ == "CSDM":
+        if len(other.y) > 1:
+            raise TypeError(
+                f"unsupported operand type(s) {operator}: 'CSDM' and "
+                f"multi dependent variable CSDM."
+            )
+        return other.y[0].components
+
+    if isinstance(other, np.ndarray):
+        return other.T[np.newaxis]
+
     if not isinstance(
         other, (int, float, complex, np.ndarray, Quantity, ScalarQuantity)
     ):
         raise TypeError(
             f"unsupported operand type(s) {operator}: 'CSDM' and "
             f"'{other.__class__.__name__}'."
         )
-    if isinstance(other, np.ndarray):
-        if other.ndim != 0:
-            raise ValueError("Only scalar multiplication or division is allowed.")
 
     if isinstance(other, ScalarQuantity):
         return other.quantity
 
     return other
 
 
@@ -370,7 +378,56 @@
     if isinstance(index, (tuple, list, np.ndarray)):
         for i, item in enumerate(index):
             index[i] = _correct_index(item, d)
         return tuple(index)
     if isinstance(index, int):
         return _correct_index(index, d)
     raise TypeError(f"{message}, found {type(index)}")
+
+
+def np_check_for_out(csdm, **kwargs):
+    out = kwargs.get("out", None)
+    if out is not None:
+        if len(csdm.dependent_variables) > 1:
+            raise NotImplementedError(
+                "Keyword `out` is not implemented for csdm objects with more than "
+                "one dependent variables."
+            )
+
+
+def get_CSDM_object__args__axes(*args, **kwargs):
+    axis = None
+    args_ = []
+    if args != ():
+        csdm = args[0]
+        args_ = list(args[1:])
+        if len(args) > 1:
+            args_[0] = _check_dimension_indices(len(csdm.dimensions), args[1])
+            axis = args_[0]
+    if "a" in kwargs.keys():
+        csdm = kwargs["a"]
+        kwargs.pop("a")
+    if "axis" in kwargs.keys():
+        if kwargs["axis"] is not None:
+            axis = _check_dimension_indices(len(csdm.dimensions), kwargs["axis"])
+            kwargs["axis"] = axis
+
+    np_check_for_out(csdm, **kwargs)
+    return csdm, args_, axis, kwargs
+
+
+def np_check_pads(pads, n_dims):
+    """Check and fix pads compatible with csdm"""
+    if isinstance(pads, int):
+        return tuple([(pads, pads) for _ in range(n_dims)])
+
+    if isinstance(pads, tuple):
+        if len(pads) == 2:
+            if isinstance(pads[0], int):
+                return tuple([pads for _ in range(n_dims)])
+        if len(pads) == 1:
+            if isinstance(pads[0], int):
+                return tuple([(pads[0], pads[0]) for _ in range(n_dims)])
+            if isinstance(pads[0], tuple):
+                return tuple([pads[0] for _ in range(n_dims)])
+
+    return pads
```

### Comparing `csdmpy-0.5/csdmpy.egg-info/PKG-INFO` & `csdmpy-0.6.dev2/csdmpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,132 @@
 Metadata-Version: 2.1
 Name: csdmpy
-Version: 0.5
+Version: 0.6.dev2
 Summary: A python module for the core scientific dataset model.
 Home-page: https://github.com/DeepanshS/csdmpy/
 Author: Deepansh Srivastava
 Author-email: srivastava.89@osu.edu
 License: BSD-3-Clause
-Description: 
-        # The csdmpy project
-        
-        |              |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
-        | ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-        | Deployment   | [![PyPI version](https://img.shields.io/pypi/v/csdmpy.svg?style=flat&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/csdmpy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/csdmpy)                                                                                                                                                                                                                                                                                                                                                                |
-        | Build Status | [![Github workflow](<https://img.shields.io/github/workflow/status/deepanshs/csdmpy/CI%20(pip)?logo=GitHub>)](https://github.com/DeepanshS/csdmpy/actions) [![Documentation Status](https://readthedocs.org/projects/csdmpy/badge/?version=stable)](https://csdmpy.readthedocs.io/en/stable/?badge=stable)                                                                                                                                        |
-        | License      | [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
-        | Metrics      | [![Total alerts](https://img.shields.io/lgtm/alerts/g/DeepanshS/csdmpy.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/DeepanshS/csdmpy/alerts/) [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/DeepanshS/csdmpy.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/DeepanshS/csdmpy/context:python) [![codecov](https://codecov.io/gh/DeepanshS/csdmpy/branch/master/graph/badge.svg)](https://codecov.io/gh/DeepanshS/csdmpy) |
-        | GitHub       | ![GitHub issues](https://img.shields.io/github/issues-raw/deepanshs/csdmpy)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-        | Citations    | [![DOI](<https://img.shields.io/badge/DOI-PLOS%20ONE%2015(1):%20e0225953-blueviolet>)](https://doi.org/10.1371/journal.pone.0225953)                                                                                                                                                                                                                                                                                                                               |
-        
-        The _csdmpy_ package is a Python support for the core scientific
-        dataset (CSD) model file exchange-format.
-        The package is based on the core scientific dataset (CSD) model which is
-        designed as a building block in the development of a more sophisticated
-        portable scientific dataset file standard.
-        The CSD model is capable of handling a wide variety of
-        scientific datasets both within and across disciplinary fields.
-        
-        The main objective of this python package is to facilitate an easy import and
-        export of the CSD model serialized JSON files for Python users. The
-        package utilizes Numpy library and, therefore, offers the end users versatility
-        to process or visualize the imported datasets with any third party package(s)
-        compatible with Numpy.
-        
-        For further reading, refer to the [documentation](https://csdmpy.readthedocs.io/en/latest/).
-        
-        > **See example gallery**
-        >
-        > [![View](https://img.shields.io/badge/View-Example%20Gallery-Purple?size=large)](https://csdmpy.readthedocs.io/en/latest/auto_examples/index.html)
-        
-        ## The core scientific dataset (CSD) model
-        
-        The core scientific dataset (CSD) model is a _light-weight_, _portable_,
-        _versatile_, and _standalone_ data model capable of handling a variety of
-        scientific datasets. The model only encapsulates
-        data values and the minimum metadata, to accurately represent a **_p_-component
-        dependent variable,
-        discretely sampled at _M_ unique points in a _d_-dimensional coordinate space**.
-        The model is not intended to encapsulate
-        any information on how the data might be acquired, processed, or visualized.
-        
-        ---
-        ### Use cases
-        The data model is _versatile_ in allowing many **use cases for most spectroscopy,
-        diffraction, and imaging techniques**.
-        
-        ![](/docs/_static/csdm.png "")
-        
-        ### Data Model
-        
-        The model supports multi-component datasets associated with continuous
-        physical quantities that are discretely sampled in a multi-dimensional space
-        associated with other carefully controlled quantities, for e.g., a mass as a
-        function of temperature, a current as a function of voltage and time, a signal
-        voltage as a function of magnetic field gradient strength, a color image with
-        a red, green, and blue (RGB) light intensity components as a function of two
-        independent spatial dimensions, or the six components of the symmetric
-        second-rank diffusion tensor MRI as a function of three independent spatial
-        dimensions. Additionally, the model supports multiple dependent variables
-        sharing the same _d_-dimensional coordinate space. For instance,
-        the simultaneous measurement of current and voltage as a function of time.
-        Another example would be the simultaneous acquisition of air temperature,
-        pressure, wind velocity, and
-        solar-flux as a function of Earth’s latitude and longitude coordinates. We
-        refer to these dependent variables as _correlated-datasets_.
-        
-        **Example**
-        ```py
-        "csdm": {
-          "version": "1.0",
-          # A list of Linear, Monotonic, or Labeled dimensions of the multi-dimensional space.
-          "dimensions": [{
-            "type": "linear",
-            "count": 1608,
-            "increment": "0.08333333333 yr",
-            "coordinates_offset": "1880.0416666667 yr",
-          }],
-          # A list of dependent variables sampling the multi-dimensional space.
-          "dependent_variables": [{
-            "type": "internal",
-            "unit": "mm",
-            "numeric_type": "float32",
-            "quantity_type": "scalar",
-            "component_labels": ["GMSL"],
-            "components": [
-              ["-183.0, -171.125, ..., 59.6875, 58.5"]
-            ]
-          }]
-        }
-        ```
-        ## Installing _csdmpy_ package
-        
-            $ pip install csdmpy
-        
-        ## How to cite
-        
-        Please cite the following when used in publication.
-        
-        1. Srivastava D.J., Vosegaard T., Massiot D., Grandinetti P.J. (2020) Core Scientific Dataset Model: A lightweight and portable model and file format for multi-dimensional scientific data. [PLOS ONE 15(1): e0225953.](https://doi.org/10.1371/journal.pone.0225953)
-        
-        ## Check out the media coverage.
-        
-        - [<img src="https://inc.cnrs.fr/sites/institut_inc/files/styles/top_left/public/image/cnrs_20180120_0025%20%281%29.jpg?itok=i3wlyGBq" height="64" width="64"> Des chimistes élaborent un nouveau format pour le partage de données scientifiques](https://inc.cnrs.fr/fr/cnrsinfo/des-chimistes-elaborent-un-nouveau-format-pour-le-partage-de-donnees-scientifiques)
-        
-        - [<img src="https://www.technology.org/texorgwp/wp-content/uploads/2020/01/1920_data-1536x1024.jpg" height="64" width="64"> Simplifying how scientists share data](https://www.technology.org/2020/01/03/simplifying-how-scientists-share-data/)
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: matplotlib
+License-File: LICENSE
+
+
+# The csdmpy project
+
+|              |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Deployment   | [![PyPI version](https://img.shields.io/pypi/v/csdmpy.svg?style=flat&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/csdmpy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/csdmpy)                                                                                                                                                                                                                                                                                                                                                                |
+| Build Status | [![Github workflow](<https://img.shields.io/github/actions/workflow/status/deepanshs/csdmpy/continuous-integration-pip.yml?logo=GitHub>)](https://github.com/DeepanshS/csdmpy/actions/workflow/continuous-integration-pip.yml) [![Documentation Status](https://readthedocs.org/projects/csdmpy/badge/?version=stable)](https://csdmpy.readthedocs.io/en/stable/?badge=stable)                                                                                                                                        |
+| License      | [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| Metrics      | [![codecov](https://codecov.io/gh/DeepanshS/csdmpy/branch/master/graph/badge.svg)](https://codecov.io/gh/DeepanshS/csdmpy) ![GitHub issues](https://img.shields.io/github/issues-raw/deepanshs/csdmpy)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+| Citation    | [![DOI](<https://img.shields.io/badge/DOI-PLOS%20ONE%2015(1):%20e0225953-blueviolet>)](https://doi.org/10.1371/journal.pone.0225953)                                                                                                                                                                                                                                                                                                                               |
+
+The _csdmpy_ package is a Python support for the core scientific
+dataset (CSD) model file exchange-format.
+The package is based on the core scientific dataset (CSD) model which is
+designed as a building block in the development of a more sophisticated
+portable scientific dataset file standard.
+The CSD model is capable of handling a wide variety of
+scientific datasets both within and across disciplinary fields.
+
+The main objective of this python package is to facilitate an easy import and
+export of the CSD model serialized JSON files for Python users. The
+package utilizes Numpy library and, therefore, offers the end users versatility
+to process or visualize the imported datasets with any third party package(s)
+compatible with Numpy.
+
+For further reading, refer to the [documentation](https://csdmpy.readthedocs.io/en/latest/).
+
+> **See example gallery**
+>
+> [![View](https://img.shields.io/badge/View-Example%20Gallery-Purple?size=large)](https://csdmpy.readthedocs.io/en/latest/auto_examples/index.html)
+
+## The core scientific dataset (CSD) model
+
+The core scientific dataset (CSD) model is a _light-weight_, _portable_,
+_versatile_, and _standalone_ data model capable of handling a variety of
+scientific datasets. The model only encapsulates
+data values and the minimum metadata, to accurately represent a **_p_-component
+dependent variable,
+discretely sampled at _M_ unique points in a _d_-dimensional coordinate space**.
+The model is not intended to encapsulate
+any information on how the data might be acquired, processed, or visualized.
+
+---
+### Use cases
+The data model is _versatile_ in allowing many **use cases for most spectroscopy,
+diffraction, and imaging techniques**.
+
+![](/docs/_static/csdm.png "")
+
+### Data Model
+
+The model supports multi-component datasets associated with continuous
+physical quantities that are discretely sampled in a multi-dimensional space
+associated with other carefully controlled quantities, for e.g., a mass as a
+function of temperature, a current as a function of voltage and time, a signal
+voltage as a function of magnetic field gradient strength, a color image with
+a red, green, and blue (RGB) light intensity components as a function of two
+independent spatial dimensions, or the six components of the symmetric
+second-rank diffusion tensor MRI as a function of three independent spatial
+dimensions. Additionally, the model supports multiple dependent variables
+sharing the same _d_-dimensional coordinate space. For instance,
+the simultaneous measurement of current and voltage as a function of time.
+Another example would be the simultaneous acquisition of air temperature,
+pressure, wind velocity, and
+solar-flux as a function of Earth’s latitude and longitude coordinates. We
+refer to these dependent variables as _correlated-datasets_.
+
+**Example**
+```py
+"csdm": {
+  "version": "1.0",
+  # A list of Linear, Monotonic, or Labeled dimensions of the multi-dimensional space.
+  "dimensions": [{
+    "type": "linear",
+    "count": 1608,
+    "increment": "0.08333333333 yr",
+    "coordinates_offset": "1880.0416666667 yr",
+  }],
+  # A list of dependent variables sampling the multi-dimensional space.
+  "dependent_variables": [{
+    "type": "internal",
+    "unit": "mm",
+    "numeric_type": "float32",
+    "quantity_type": "scalar",
+    "component_labels": ["GMSL"],
+    "components": [
+      ["-183.0, -171.125, ..., 59.6875, 58.5"]
+    ]
+  }]
+}
+```
+## Installing _csdmpy_ package
+
+    $ pip install csdmpy
+
+## How to cite
+
+Please cite the following when used in publication.
+
+1. Srivastava D.J., Vosegaard T., Massiot D., Grandinetti P.J. (2020) Core Scientific Dataset Model: A lightweight and portable model and file format for multi-dimensional scientific data. [PLOS ONE 15(1): e0225953.](https://doi.org/10.1371/journal.pone.0225953)
+
+## Check out the media coverage.
+
+- [<img src="https://inc.cnrs.fr/sites/institut_inc/files/styles/top_left/public/image/cnrs_20180120_0025%20%281%29.jpg?itok=i3wlyGBq" height="64" width="64"> Des chimistes élaborent un nouveau format pour le partage de données scientifiques](https://inc.cnrs.fr/fr/cnrsinfo/des-chimistes-elaborent-un-nouveau-format-pour-le-partage-de-donnees-scientifiques)
+
+- [<img src="https://www.technology.org/texorgwp/wp-content/uploads/2020/01/1920_data-1536x1024.jpg" height="64" width="64"> Simplifying how scientists share data](https://www.technology.org/2020/01/03/simplifying-how-scientists-share-data/)
```

### Comparing `csdmpy-0.5/csdmpy.egg-info/SOURCES.txt` & `csdmpy-0.6.dev2/csdmpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -132,8 +132,10 @@
 tests/file_read/test_files/6.csdfe
 tests/file_read/test_files/7.csdfe
 tests/file_read/test_files/8.csdfe
 tests/file_read/test_files/9.csdfe
 tests/numpy_wrapper/apodization_test.py
 tests/numpy_wrapper/change_shape_test.py
 tests/numpy_wrapper/dimension_reduction_test.py
-tests/numpy_wrapper/element_wise_test.py
+tests/numpy_wrapper/element_wise_test.py
+tests/numpy_wrapper/np_pad_flip_test.py
+tests/numpy_wrapper/numpy_csdm_test.py
```

### Comparing `csdmpy-0.5/docs/.DS_Store` & `csdmpy-0.6.dev2/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/.coverage` & `csdmpy-0.6.dev2/docs/.coverage`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/CSD_model.rst` & `csdmpy-0.6.dev2/docs/CSD_model.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/CSDmodel_uml/.DS_Store` & `csdmpy-0.6.dev2/docs/CSDmodel_uml/.DS_Store`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/CSDmodel_uml/csdm.rst` & `csdmpy-0.6.dev2/docs/CSDmodel_uml/csdm.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/CSDmodel_uml/dependent_variables/dependent_variable.rst` & `csdmpy-0.6.dev2/docs/CSDmodel_uml/dependent_variables/dependent_variable.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/CSDmodel_uml/dependent_variables/external.rst` & `csdmpy-0.6.dev2/docs/CSDmodel_uml/dependent_variables/external.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/CSDmodel_uml/dependent_variables/internal.rst` & `csdmpy-0.6.dev2/docs/CSDmodel_uml/dependent_variables/internal.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/CSDmodel_uml/dependent_variables/sparse_sampling.rst` & `csdmpy-0.6.dev2/docs/CSDmodel_uml/dependent_variables/sparse_sampling.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/CSDmodel_uml/dimensions/dimension.rst` & `csdmpy-0.6.dev2/docs/CSDmodel_uml/dimensions/dimension.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/CSDmodel_uml/dimensions/labeled.rst` & `csdmpy-0.6.dev2/docs/CSDmodel_uml/dimensions/labeled.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/CSDmodel_uml/dimensions/linear.rst` & `csdmpy-0.6.dev2/docs/CSDmodel_uml/dimensions/linear.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/CSDmodel_uml/dimensions/monotonic.rst` & `csdmpy-0.6.dev2/docs/CSDmodel_uml/dimensions/monotonic.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/CSDmodel_uml/enumeration.rst` & `csdmpy-0.6.dev2/docs/CSDmodel_uml/enumeration.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/Makefile` & `csdmpy-0.6.dev2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/_images/.DS_Store` & `csdmpy-0.6.dev2/docs/_images/.DS_Store`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/_static/.DS_Store` & `csdmpy-0.6.dev2/docs/_static/.DS_Store`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/_static/button.css` & `csdmpy-0.6.dev2/docs/_static/button.css`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/_static/csdm.png` & `csdmpy-0.6.dev2/docs/_static/csdm.png`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/_static/csdmpy.png` & `csdmpy-0.6.dev2/docs/_static/csdmpy.png`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/_static/style.css` & `csdmpy-0.6.dev2/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/_templates/.DS_Store` & `csdmpy-0.6.dev2/docs/_templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/_templates/layout.html` & `csdmpy-0.6.dev2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/api/.DS_Store` & `csdmpy-0.6.dev2/docs/api/.DS_Store`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/api/CSDM.rst` & `csdmpy-0.6.dev2/docs/api/CSDM.rst`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,22 @@
    .. autosummary::
       :nosignatures:
 
       ~CSDM.dict
       ~CSDM.to_dict
       ~CSDM.dumps
       ~CSDM.astype
+      ~CSDM.to_list
       ~CSDM.save
       ~CSDM.copy
       ~CSDM.split
+      ~CSDM.reshape
+      ~CSDM.transpose
+      ~CSDM.fft
+      ~CSDM.to_positive_inc
 
    .. rubric:: Numpy compatible attributes summary
    .. autosummary::
       :nosignatures:
 
       ~CSDM.real
       ~CSDM.imag
@@ -95,14 +100,16 @@
    .. automethod:: save
    .. automethod:: to_list
    .. automethod:: astype
    .. automethod:: copy
    .. automethod:: split
    .. automethod:: transpose
    .. automethod:: fft
+   .. automethod:: reshape
+   .. automethod:: to_positive_inc
 
    .. rubric:: Numpy compatible method documentation
 
    .. automethod:: max
    .. automethod:: min
    .. automethod:: clip
    .. automethod:: conj
```

### Comparing `csdmpy-0.5/docs/api/DependentVariable.rst` & `csdmpy-0.6.dev2/docs/api/DependentVariable.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/api/Dimensions.rst` & `csdmpy-0.6.dev2/docs/api/Dimensions.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/api/csdmpy.rst` & `csdmpy-0.6.dev2/docs/api/csdmpy.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/api/plotting_function.rst` & `csdmpy-0.6.dev2/docs/api/plotting_function.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/api/wrappers/apodization.rst` & `csdmpy-0.6.dev2/docs/api/wrappers/apodization.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/api/wrappers/element_wise_operation.rst` & `csdmpy-0.6.dev2/docs/api/wrappers/element_wise_operation.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/conf.py` & `csdmpy-0.6.dev2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/getting_started.rst` & `csdmpy-0.6.dev2/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/index.rst` & `csdmpy-0.6.dev2/docs/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -15,41 +15,32 @@
             :target: https://pypi.python.org/pypi/csdmpy
             :alt: PyPI version
 
           .. image:: https://img.shields.io/pypi/pyversions/csdmpy
             :alt: PyPI - Python Version
 
       * - Build Status
-        - .. image:: https://img.shields.io/github/workflow/status/deepanshs/csdmpy/CI%20(pip)?logo=GitHub
-            :target: https://github.com/DeepanshS/csdmpy/actions
+        - .. image:: https://img.shields.io/github/actions/workflow/status/deepanshs/csdmpy/continuous-integration-pip.yml?logo=GitHub
+            :target: https://github.com/DeepanshS/csdmpy/actions/workflow/continuous-integration-pip.yml
             :alt: GitHub Workflow Status
 
           .. image:: https://readthedocs.org/projects/csdmpy/badge/?version=stable
             :target: https://csdmpy.readthedocs.io/en/stable/
             :alt: Documentation Status
 
       * - License
         - .. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
             :target: https://opensource.org/licenses/BSD-3-Clause
             :alt: License
 
       * - Metrics
-        - .. image:: https://img.shields.io/lgtm/alerts/g/DeepanshS/csdmpy.svg?logo=lgtm
-            :target: https://lgtm.com/projects/g/DeepanshS/csdmpy/alerts/
-            :alt: Total alerts
-
-          .. image:: https://img.shields.io/lgtm/grade/python/g/DeepanshS/csdmpy.svg?logo=lgtm
-            :target: https://lgtm.com/projects/g/DeepanshS/csdmpy/context:python
-            :alt: Language grade: Python
-
-          .. image:: https://codecov.io/gh/DeepanshS/csdmpy/branch/master/graph/badge.svg
+        - .. image:: https://codecov.io/gh/DeepanshS/csdmpy/branch/master/graph/badge.svg
             :target: https://codecov.io/gh/DeepanshS/csdmpy
 
-      * - GitHub
-        - .. image:: https://img.shields.io/github/issues-raw/deepanshs/csdmpy?logo=github
+          .. image:: https://img.shields.io/github/issues-raw/deepanshs/csdmpy?logo=github
             :target: https://github.com/DeepanshS/csdmpy/issues
             :alt: GitHub issues
 
       * - Citation
         - .. image:: https://img.shields.io/badge/DOI-PLOS%20ONE%2015(1):%20e0225953-Purple?size=large
             :target: https://doi.org/10.1371/journal.pone.0225953
```

### Comparing `csdmpy-0.5/docs/installation.rst` & `csdmpy-0.6.dev2/docs/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ============
 
 Requirements
 ------------
 
 ``csdmpy`` has the following strict requirements:
 
-- `Python <https://www.python.org>`_ 3.6 or later
-- `Numpy <https://numpy.org>`_ 1.17 or later
+- `Python <https://www.python.org>`_ 3.7 or later
+- `Numpy <https://numpy.org>`_ 1.20 or later
 
 Other requirements include:
 
 - `requests>=2.21.0 <http://docs.python-requests.org/en/master/>`_
   (for downloading files from server)
 - `astropy>=3.0 <http://www.astropy.org>`_ (for astropy units module)
 - `matplotlib>=3.0 <https://matplotlib.org>`_ (for rendering plots)
```

### Comparing `csdmpy-0.5/docs/make.bat` & `csdmpy-0.6.dev2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/plotting_with_pyplot/one_D_plots.rst` & `csdmpy-0.6.dev2/docs/plotting_with_pyplot/one_D_plots.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/plotting_with_pyplot/two_D_plots.rst` & `csdmpy-0.6.dev2/docs/plotting_with_pyplot/two_D_plots.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/startFromScratch/A fun example.rst` & `csdmpy-0.6.dev2/docs/startFromScratch/A fun example.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/startFromScratch/add_dependent_variable_object.rst` & `csdmpy-0.6.dev2/docs/startFromScratch/add_dependent_variable_object.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/startFromScratch/add_dimension_object.rst` & `csdmpy-0.6.dev2/docs/startFromScratch/add_dimension_object.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/startFromScratch/dimension/generate/labeled.rst` & `csdmpy-0.6.dev2/docs/startFromScratch/dimension/generate/labeled.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/startFromScratch/dimension/generate/linear.rst` & `csdmpy-0.6.dev2/docs/startFromScratch/dimension/generate/linear.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/startFromScratch/dimension/generate/monotonic.rst` & `csdmpy-0.6.dev2/docs/startFromScratch/dimension/generate/monotonic.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/startFromScratch/dimension/interact/linear.rst` & `csdmpy-0.6.dev2/docs/startFromScratch/dimension/interact/linear.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/startFromScratch/dimension/interact/monotonic.rst` & `csdmpy-0.6.dev2/docs/startFromScratch/dimension/interact/monotonic.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/startFromScratch/generating_csdm_object.rst` & `csdmpy-0.6.dev2/docs/startFromScratch/generating_csdm_object.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/startFromScratch/generating_dependent_variable_object.rst` & `csdmpy-0.6.dev2/docs/startFromScratch/generating_dependent_variable_object.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/startFromScratch/interacting_with_csdm.rst` & `csdmpy-0.6.dev2/docs/startFromScratch/interacting_with_csdm.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/startFromScratch/save_dataset.rst` & `csdmpy-0.6.dev2/docs/startFromScratch/save_dataset.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/docs/using_csdm_with_pyplot.rst` & `csdmpy-0.6.dev2/docs/using_csdm_with_pyplot.rst`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/setup.py` & `csdmpy-0.6.dev2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,16 @@
         if "__version__" in line:
             before_keyword, keyword, after_keyword = line.partition("=")
             version = after_keyword.strip()[1:-1]
 
 
 # What packages are required for this module to be executed?
 required = [
-    "numpy>=1.17",
+    "numpy>=1.20",
     "setuptools>=27.3",
-    "astropy>=3.0",
     "requests>=2.21.0",
     "numexpr>=2.7.0",
 ]
 extras = {"matplotlib": ["matplotlib>=3.0"]}
 setup_requires = ["setuptools>=27.3"]
 
 here = os.path.abspath(os.path.dirname(__file__))
@@ -38,15 +37,15 @@
     name="csdmpy",
     version=version,
     description="A python module for the core scientific dataset model.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Deepansh Srivastava",
     author_email="srivastava.89@osu.edu",
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     url="https://github.com/DeepanshS/csdmpy/",
     packages=find_packages(),
     install_requires=required,
     setup_requires=setup_requires,
     extras_require=extras,
     tests_require=["pytest", "pytest-runner"],
     include_package_data=True,
@@ -57,15 +56,15 @@
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
     ],
 )
```

### Comparing `csdmpy-0.5/tests/.DS_Store` & `csdmpy-0.6.dev2/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/csdm_indexing_test.py` & `csdmpy-0.6.dev2/tests/csdm_indexing_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,22 +126,20 @@
     assert str(l_test.y[0].unit) == "A"
     save_and_load(l_test)
 
 
 def test_index_7():
     l_test = a_obj[1, 3, 9]
     assert l_test.shape == ()
-    assert np.allclose(l_test.y[0].components[0], array[9, 3, 1])
-    assert str(l_test.y[0].unit) == "A"
-    save_and_load(l_test)
+    assert np.allclose(l_test.value, array[9, 3, 1])
+    assert str(l_test.unit) == "A"
 
     l_test = a_obj[(1, 3, 19)]
     assert l_test.shape == ()
-    assert np.allclose(l_test.y[0].components[0], array[19, 3, 1])
-    assert str(l_test.y[0].unit) == "A"
-    save_and_load(l_test)
+    assert np.allclose(l_test.value, array[19, 3, 1])
+    assert str(l_test.unit) == "A"
 
 
 def test_index_8():
     error = "Fancy indexing using tuples or lists may result in"
     with pytest.raises(NotImplementedError, match=f".*{error}.*"):
         _ = a_obj[(1, 3, 9), 10]
```

### Comparing `csdmpy-0.5/tests/csdm_new_test.py` & `csdmpy-0.6.dev2/tests/csdm_new_test.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/csdm_test.py` & `csdmpy-0.6.dev2/tests/csdm_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,16 +65,15 @@
         data.tags = "23"
 
     # version
     assert data.version == cp.csdm.CSDM.__latest_CSDM_version__
 
     # geographic_coordinate
     assert data.geographic_coordinate is None
-    error = "can't set attribute"
-    with pytest.raises(AttributeError, match=f".*{error}.*"):
+    with pytest.raises(AttributeError):
         data.geographic_coordinate = {}
 
     # description
     assert data.description == "This is a test"
     data.description = "Enough with the tests"
     assert data.description == "Enough with the tests"
     error = "Expecting an instance of type"
@@ -385,26 +384,18 @@
     res = cp.ScalarQuantity("1.324 s") / (b_test + 1)
     assert np.allclose(res.y[0].components, 1.324 / (out + 1))
 
     error = r"unsupported operand type\(s\) \*: 'CSDM' and 'str'."
     with pytest.raises(TypeError, match=f".*{error}.*"):
         res = a_test * "3"
 
-    error = "Only scalar multiplication or division is allowed."
-    with pytest.raises(ValueError, match=f".*{error}.*"):
-        res = a_test * np.asarray([1, 2])
-
     error = r"unsupported operand type\(s\) /: 'CSDM' and 'str'."
     with pytest.raises(TypeError, match=f".*{error}.*"):
         res = a_test / "3"
 
-    error = "Only scalar multiplication or division is allowed."
-    with pytest.raises(ValueError, match=f".*{error}.*"):
-        res = a_test / np.asarray([1, 2])
-
     # pow
     res = b1_test**2
     out = b1_test.y[0].components
     assert np.allclose(res.y[0].components, np.power(out, 2))
     assert str(res.y[0].unit) == "km2"
 
     res **= 2
@@ -605,7 +596,62 @@
     np_fn = [np.ptp, np.trace]
     cp_fn = ["ptp", "trace"]
     for fn_n, fn_c in zip(np_fn, cp_fn):
         with pytest.raises(NotImplementedError, match=""):
             _ = fn_n(a_test)
         with pytest.raises(NotImplementedError, match=""):
             a_test.__getattribute__(fn_c)()
+
+
+def test_reshape():
+    out, test_csdm = get_test_2d(int)
+    new_test = test_csdm.reshape(shape=(25, 2))
+    np.testing.assert_allclose(new_test.y[0].components[0], out.reshape(2, 25))
+
+    d1 = cp.as_dimension(array=np.arange(2))
+    d2 = cp.as_dimension(array=np.arange(25) - 12)
+    new_test = test_csdm.reshape(shape=(d1, d2))
+    np.testing.assert_allclose(new_test.y[0].components[0], out.reshape(25, 2))
+
+
+def test_neg_to_pos_inc1():
+    x = [
+        cp.MonotonicDimension(coordinates=["1m", "10m", "100m"]),
+        cp.LinearDimension(count=10, increment="-1", coordinates_offset="2"),
+        cp.LinearDimension(count=5, increment="-3", coordinates_offset="2"),
+        cp.LabeledDimension(labels=["a", "b", "c"]),
+    ]
+    y = [cp.as_dependent_variable(array=[np.random.rand(3, 5, 10, 3)])]
+    obj = cp.CSDM(dimensions=x, dependent_variables=y)
+
+    new_obj = obj.to_positive_inc()
+    for i in [1, 2]:
+        np.testing.assert_allclose(
+            new_obj.x[i].coordinates.value[::-1], obj.x[i].coordinates.value
+        )
+    for i in [0, 4]:
+        np.testing.assert_allclose(
+            new_obj.x[0].coordinates.value, obj.x[0].coordinates.value
+        )
+    np.testing.assert_allclose(
+        new_obj.y[0].components[0][:, ::-1, ::-1, :], obj.y[0].components[0]
+    )
+
+
+def test_neg_to_pos_inc2():
+    x = [
+        cp.MonotonicDimension(coordinates=["1", "-10", "-100"]),
+        cp.LinearDimension(count=5, increment="3", coordinates_offset="2"),
+    ]
+    y = [cp.as_dependent_variable(array=[np.random.rand(5, 3)])]
+    obj = cp.CSDM(dimensions=x, dependent_variables=y)
+
+    new_obj = obj.to_positive_inc()
+    np.testing.assert_allclose(
+        new_obj.x[0].coordinates.value[::-1], obj.x[0].coordinates.value
+    )
+    np.testing.assert_allclose(
+        new_obj.x[1].coordinates.value, obj.x[1].coordinates.value
+    )
+    np.testing.assert_allclose(
+        new_obj.y[0].components[0][:, ::-1], obj.y[0].components[0]
+    )
```

### Comparing `csdmpy-0.5/tests/dependent_variable_test.py` & `csdmpy-0.6.dev2/tests/dependent_variable_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,65 +167,65 @@
 
     assert dim1 != 21
 
 
 def test_external_new():
     domain = "https://www.ssnmr.org/sites/default/files/CSDM"
 
-    d_v = cp.DependentVariable(
+    dv_obj = cp.DependentVariable(
         type="external",
         components_url=f"{domain}/GC/cinnamon_raw_cinnamon stick.dat",
         component_labels=["monotonic"],
         name="Headspace from cinnamon stick",
         numeric_type="float32",
         quantity_type="scalar",
     )
-    data = cp.CSDM(dependent_variables=[d_v, d_v.copy()])
+    data = cp.CSDM(dependent_variables=[dv_obj, dv_obj.copy()])
 
-    for dv in data.y:
+    for dv_obj in data.y:
         # check type
-        assert dv.type == "internal"
-        dv.type = "external"
-        assert dv.type == "external"
+        assert dv_obj.type == "internal"
+        dv_obj.type = "external"
+        assert dv_obj.type == "external"
 
         # check components
-        assert dv.numeric_type == "float32"
+        assert dv_obj.numeric_type == "float32"
 
         # assign and check components
-        dv.numeric_type = "int32"
-        assert dv.numeric_type == "int32"
-        assert dv.components.dtype == "int32"
+        dv_obj.numeric_type = "int32"
+        assert dv_obj.numeric_type == "int32"
+        assert dv_obj.components.dtype == "int32"
 
         # check name
-        assert dv.name == "Headspace from cinnamon stick"
+        assert dv_obj.name == "Headspace from cinnamon stick"
 
         # check unit
-        assert dv.unit == ""
+        assert dv_obj.unit == ""
 
         # check component_url
-        assert dv.components_url == f"{domain}/GC/cinnamon_raw_cinnamon stick.dat"
+        assert dv_obj.components_url == f"{domain}/GC/cinnamon_raw_cinnamon stick.dat"
 
         # component names
-        assert dv.component_labels == ["monotonic"]
+        assert dv_obj.component_labels == ["monotonic"]
 
         # quantity type
-        assert dv.quantity_type == "scalar"
+        assert dv_obj.quantity_type == "scalar"
 
         # encoding
-        assert dv.encoding == "base64"
-        dv.encoding = "raw"
-        assert dv.encoding == "raw"
+        assert dv_obj.encoding == "base64"
+        dv_obj.encoding = "raw"
+        assert dv_obj.encoding == "raw"
 
         # description
-        assert dv.description == ""
-        dv.description = "This is also a test"
-        assert dv.description == "This is also a test"
+        assert dv_obj.description == ""
+        dv_obj.description = "This is also a test"
+        assert dv_obj.description == "This is also a test"
 
         # application
-        assert dv.application is None
+        assert dv_obj.application is None
 
     dict_1 = {
         "type": "internal",
         "description": "This is also a test",
         "name": "Headspace from cinnamon stick",
         "numeric_type": "int32",
         "quantity_type": "scalar",
@@ -279,7 +279,22 @@
 
 
 def test_missing_component_url():
     d_v = {"type": "external", "numeric_type": "float32", "quantity_type": "scalar"}
     error = "Missing a required `components_url` key"
     with pytest.raises(KeyError, match=f".*{error}.*"):
         _ = cp.CSDM(dependent_variables=[d_v])
+
+
+def test_c_f_contiguous_array():
+    arr_c = np.random.rand(1028 * 1028).reshape(1028, 1028)
+    arr_f = np.asfortranarray(arr_c.copy())
+
+    assert arr_c.flags["C_CONTIGUOUS"] is True
+    assert arr_c.flags["F_CONTIGUOUS"] is False
+    assert arr_f.flags["C_CONTIGUOUS"] is False
+    assert arr_f.flags["F_CONTIGUOUS"] is True
+
+    dv_c = cp.as_dependent_variable(arr_c)
+    dv_f = cp.as_dependent_variable(arr_f)
+
+    assert np.allclose(dv_c.components, dv_f.components)
```

### Comparing `csdmpy-0.5/tests/dimension_test.py` & `csdmpy-0.6.dev2/tests/dimension_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,15 @@
     # test for attributes
     assert data.dependent_variables == data.y
     assert data.dimensions == data.x
 
     # type
     assert data.dimensions[0].type == "linear"
 
-    error = "can't set attribute"
-    with pytest.raises(AttributeError, match=f".*{error}.*"):
+    with pytest.raises(AttributeError):
         data.dimensions[0].type = "monotonic"
 
     # increment
     assert str(data.dimensions[0].increment) == "10.0 m / s"
     data.dimensions[0].increment = ScalarQuantity("20.0 m / s")
     assert str(data.dimensions[0].increment) == "20.0 m / s"
     data.dimensions[0].increment = 20.0 * u.Unit("m / s")
@@ -68,16 +67,18 @@
     assert str(data.dimensions[0].period) == "inf m / s"
     assert data.dimensions[0].complex_fft is False
     assert np.all(data.dimensions[0].coordinates.value == np.arange(10) * 10.0 + 5.0)
     assert np.all(data.x[0].coords.value == np.arange(10) * 10.0 + 5.0)
 
     # count
     assert data.dimensions[0].count == 10
+    assert data.dimensions[0].size == 10
     data.dimensions[0].count = 12
     assert data.dimensions[0].count == 12
+    assert data.dimensions[0].size == 12
     assert np.all(data.dimensions[0].coordinates.value == np.arange(12) * 10.0 + 5.0)
     assert np.all(data.x[0].coords.value == np.arange(12) * 10.0 + 5.0)
     assert np.all(
         data.dimensions[0].absolute_coordinates.value == np.arange(12) * 10.0 + 5.0
     )
 
     # origin offset
@@ -232,15 +233,15 @@
     )
 
     freq.to("kHz")
     assert np.allclose(freq.coordinates.value, (np.arange(10) * 0.1 + 1))
     assert np.allclose(freq.coords.value, (np.arange(10) * 0.1 + 1))
 
     freq.to("ppm", "nmr_frequency_ratio")
-    values = (np.arange(10) * 100 + 1000) / (1 - (0.001 + 0.0005))
+    values = (np.arange(10) * 100 + 1000) / 1
     assert np.allclose(freq.coordinates.value, values)
     assert np.allclose(freq.coords.value, values)
 
     freq.origin_offset = "0 Hz"
     assert str(freq.origin_offset) == "0.0 Hz"
 
     freq.coordinates_offset = "0 Hz"
@@ -261,14 +262,21 @@
 # monotonic dimension
 def test_monotonic_new():
     dim_x = cp.Dimension(
         type="monotonic",
         description="Far far away.",
         coordinates=["1 m", "100 m", "1 km", "1 Gm", "0.25 lyr"],
     )
+    # mult
+    dim_x2 = dim_x * 4
+    assert np.allclose(dim_x2.coordinates, 4 * dim_x.coordinates)
+
+    dim_x2 = 4 * dim_x
+    assert np.allclose(dim_x2.coordinates, 4 * dim_x.coordinates)
+
     data = cp.CSDM(dimensions=[dim_x, dim_x.copy()])
 
     for dim in data.dimensions:
         assert dim.is_quantitative() is True
 
         # description
         assert dim.description == "Far far away."
@@ -303,29 +311,29 @@
 
         error = "Expecting an instance of type"
         with pytest.raises(TypeError, match=f".*{error}.*"):
             dim.label = {}
 
         # count
         assert dim.count == 5
+        assert dim.size == 5
         error = "Cannot set the count,"
         with pytest.raises(ValueError, match=f".*{error}.*"):
             dim.count = 12
 
         error = "Expecting an instance of type"
         with pytest.raises(TypeError, match=f".*{error}.*"):
             dim.count = "12"
 
         # coordinates_offset
         error = "`MonotonicDimension` has no attribute `coordinates_offset`."
         with pytest.raises(AttributeError, match=f".*{error}.*"):
             _ = dim.coordinates_offset
 
-        error = "can't set attribute"
-        with pytest.raises(AttributeError, match=f".*{error}.*"):
+        with pytest.raises(AttributeError):
             dim.coordinates_offset = "1"
 
         # origin offset
         assert str(dim.origin_offset) == "0.0 m"
 
         dim.origin_offset = ScalarQuantity("3.1415 m")
         assert str(dim.origin_offset) == "3.1415 m"
@@ -521,14 +529,15 @@
         "type": "labeled",
         "description": "Far far away.",
         "labels": ["m", "s", "t", "a"],
     }
     data.dimensions.append(dim)
 
     assert data.dimensions[0].is_quantitative() is False
+    assert data.dimensions[0].size == 4
 
     # description
     assert data.dimensions[0].description == "Far far away."
     data.dimensions[0].description = "A galaxy far far away."
     assert data.dimensions[0].description == "A galaxy far far away."
 
     error = "Expecting an instance of type"
@@ -619,14 +628,21 @@
     rand = np.random.rand(10)
     monotonic = 10**array / 10
 
     dim = cp.as_dimension(array, unit="s")
     assert np.allclose(dim.coordinates.value, array)
     assert np.allclose(dim.coords.value, array)
 
+    # dim mult
+    dim2 = 4 * dim
+    assert dim2.increment == dim.increment * 4
+
+    dim2 = dim * 4
+    assert dim2.increment == dim.increment * 4
+
     # linear
     error = "Invalid array for Dimension object."
     with pytest.raises(ValueError, match=f".*{error}.*"):
         cp.as_dimension(one, unit="s")
 
     dim = cp.as_dimension(array, unit="s", type="linear")
     assert np.allclose(dim.coordinates.value, array)
```

### Comparing `csdmpy-0.5/tests/fft_test.py` & `csdmpy-0.6.dev2/tests/fft_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,65 @@
+from copy import deepcopy
+
 import numpy as np
 
 import csdmpy as cp
 
 
 def fft_process(csdm):
     y = csdm.y[0].components[0]
 
     # fft
     coordinates_offset = csdm.dimensions[0].coordinates_offset
     reciprocal_coordinates = csdm.dimensions[0].reciprocal_coordinates()
 
+    scale = 1.0 if np.isfinite(csdm.dimensions[0].period) else 2.0
     phase = np.exp(-2j * np.pi * coordinates_offset * reciprocal_coordinates)
-    y_fft = np.fft.fftshift(np.fft.fft(y)) * phase
+    y_copy = deepcopy(y)
+    y_copy[0] /= scale
+    y_fft = np.fft.fftshift(np.fft.fft(y_copy)) * phase
     csdm_fft = csdm.fft(axis=0)
     assert np.allclose(y_fft, csdm_fft.y[0].components[0])
 
     # inverse fft
     reciprocal_coordinates_offset = csdm_fft.dimensions[0].reciprocal.coordinates_offset
     coordinates = csdm_fft.dimensions[0].coordinates
 
     phase = np.exp(2j * np.pi * reciprocal_coordinates_offset * coordinates)
     y2 = np.fft.ifft(np.fft.ifftshift(y_fft * phase))
+    y2[0] *= scale
     csdm_2 = csdm_fft.fft(axis=0)
 
     assert np.allclose(y, y2)
     assert np.allclose(y2, csdm_2.y[0].components[0])
     assert csdm == csdm_2
 
 
 def ifft_process(csdm):
     y = csdm.y[0].components[0]
 
     # inverse fft
     reciprocal_coordinates_offset = csdm.dimensions[0].reciprocal.coordinates_offset
     coordinates = csdm.dimensions[0].coordinates - csdm.dimensions[0].coordinates_offset
 
+    scale = 1.0 if np.isfinite(csdm.dimensions[0].period) else 2.0
     phase = np.exp(2j * np.pi * reciprocal_coordinates_offset * coordinates)
+
     y_fft = np.fft.ifft(np.fft.ifftshift(y * phase))
+    y_fft[0] *= scale
     csdm_fft = csdm.fft(axis=0)
 
     assert np.allclose(y_fft, csdm_fft.y[0].components[0])
 
     # fft
     coordinates_offset = csdm_fft.dimensions[0].coordinates_offset
     reciprocal_coordinates = csdm_fft.dimensions[0].reciprocal_coordinates()
 
     phase = np.exp(-2j * np.pi * coordinates_offset * reciprocal_coordinates)
+    y_fft[0] /= scale
     y2 = np.fft.fftshift(np.fft.fft(y_fft)) * phase
     csdm_2 = csdm_fft.fft(axis=0)
 
     assert np.allclose(y, y2)
     assert np.allclose(y2, csdm_2.y[0].components[0])
     assert csdm == csdm_2
 
@@ -80,21 +90,36 @@
                 cp.as_dependent_variable(vals, quantity_type="scalar")
             ],
         )
 
         ifft_process(csdm)
 
 
+def test_fft_3():
+    for _ in range(10):
+        coordinates = np.arange(64, dtype=np.float64) - (np.random.rand() * 64)
+        vals = np.random.rand(64).astype(np.complex128)
+
+        csdm = cp.CSDM(
+            dimensions=[cp.as_dimension(coordinates, period="1")],
+            dependent_variables=[
+                (cp.as_dependent_variable(vals, quantity_type="scalar"))
+            ],
+        )
+
+        fft_process(csdm)
+
+
 def test_fft_2D_1():
     test_data = np.ones((40, 50))
     csdm_object = cp.CSDM(
         dependent_variables=[cp.as_dependent_variable(test_data)],
         dimensions=[
             cp.LinearDimension(count=50, increment="1 m"),
-            cp.LinearDimension(count=40, increment="1 s"),
+            cp.LinearDimension(count=40, increment="1 s", period="5 s"),
         ],
     )
     csdm_object_fft = csdm_object.fft(axis=0)
     csdm_object_2 = cp.CSDM(
         dependent_variables=[cp.as_dependent_variable(np.ones(50))],
         dimensions=[cp.LinearDimension(count=50, increment="1 m")],
     )
@@ -105,15 +130,15 @@
         csdm_object_2_fft.y[0].components,
     )
 
     csdm_object_fft = csdm_object.fft(axis=1)
 
     csdm_object_1 = cp.CSDM(
         dependent_variables=[cp.as_dependent_variable(np.ones(40))],
-        dimensions=[cp.LinearDimension(count=40, increment="1 s")],
+        dimensions=[cp.LinearDimension(count=40, increment="1 s", period="5 s")],
     )
     csdm_object_1_fft = csdm_object_1.fft()
 
     assert np.allclose(
         csdm_object_fft[0].y[0].components,
         csdm_object_1_fft.y[0].components,
     )
```

### Comparing `csdmpy-0.5/tests/file_read/.DS_Store` & `csdmpy-0.6.dev2/tests/file_read/.DS_Store`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/fileread_test.py` & `csdmpy-0.6.dev2/tests/file_read/fileread_test.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/.DS_Store` & `csdmpy-0.6.dev2/tests/file_read/test_files/.DS_Store`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/1.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/1.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/10.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/10.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/11.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/11.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/12.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/12.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/13.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/13.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/14.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/14.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/15.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/15.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/2.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/2.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/3.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/3.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/4.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/4.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/5.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/5.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/6.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/6.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/7.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/7.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/8.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/8.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/file_read/test_files/9.csdfe` & `csdmpy-0.6.dev2/tests/file_read/test_files/9.csdfe`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/import_test.py` & `csdmpy-0.6.dev2/tests/import_test.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/nmr_freq_test.py` & `csdmpy-0.6.dev2/tests/nmr_freq_test.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/numpy_wrapper/apodization_test.py` & `csdmpy-0.6.dev2/tests/numpy_wrapper/apodization_test.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/numpy_wrapper/dimension_reduction_test.py` & `csdmpy-0.6.dev2/tests/numpy_wrapper/dimension_reduction_test.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/numpy_wrapper/element_wise_test.py` & `csdmpy-0.6.dev2/tests/numpy_wrapper/element_wise_test.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/save_file_test.py` & `csdmpy-0.6.dev2/tests/save_file_test.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/serialization_test.py` & `csdmpy-0.6.dev2/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/sparse_test.py` & `csdmpy-0.6.dev2/tests/sparse_test.py`

 * *Files identical despite different names*

### Comparing `csdmpy-0.5/tests/statistics_test.py` & `csdmpy-0.6.dev2/tests/statistics_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     csdm.dimensions[0] = cp.as_dimension(x, unit="deg")
 
     gauss_integral = 4.0 * 2 * np.pi * 0.4
 
     # integration
     int_csdm = stat.integral(csdm)
     assert np.allclose(int_csdm.value, gauss_integral)
-    assert str(int_csdm.unit) == "deg K s"
+    assert str(int_csdm.unit) in ["deg K s", "K deg s"]
 
     # mean
     mean_csdm = stat.mean(csdm)
     assert np.allclose(mean_csdm[0].value, 5.0)
     assert np.allclose(mean_csdm[1].value, 0.5)
     assert str(mean_csdm[0].unit) == "deg"
     assert str(mean_csdm[1].unit) == "s"
```

### Comparing `csdmpy-0.5/tests/unit_test.py` & `csdmpy-0.6.dev2/tests/unit_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,23 +18,26 @@
 
     a = ScalarQuantity("(54.3/2) ppm").quantity
     assert str(a) == "27.15 ppm"
     assert str(ScalarQuantity(a)) == "27.15 ppm"
 
     a = ScalarQuantity("(54.3/2) (µHz/Hz)").quantity
     assert str(a) == "27.15 uHz / Hz"
-    assert str(ScalarQuantity(a)) == "27.15 Hz^-1 * µHz"
+    assert str(ScalarQuantity(a)) in ["27.15 Hz^-1 * µHz", "27.15 µHz * Hz^-1"]
     assert str(a.to("ppm")) == "27.15 ppm"
 
     a = ScalarQuantity("5 kg * m / s").quantity
     b = a * ScalarQuantity("1 m / s").quantity
     assert str(a) == "5.0 kg m / s"
     assert str(ScalarQuantity(a)) == "5.0 kg * m * s^-1"
-    assert str(ScalarQuantity(b)) == "5.0 kg * m^2 * s^-2"
-    assert ScalarQuantity(b).__format__("unit") == "kg * m^2 * s^-2"
+    assert str(ScalarQuantity(b)) in ["5.0 kg * m^2 * s^-2", "5.0 m^2 * kg * s^-2"]
+    assert ScalarQuantity(b).__format__("unit") in [
+        "kg * m^2 * s^-2",
+        "m^2 * kg * s^-2",
+    ]
     assert str(b.to("J")) == "5.0 J"
 
     a = ScalarQuantity("5e-7 s").quantity
     assert str(a) == "5e-07 s"
     assert str(ScalarQuantity(a)) == "5e-07 s"
     assert str(ScalarQuantity(a.to("us"))) == "0.5 µs"
     assert ScalarQuantity(a.to("us")).__format__("unit") == "µs"
```

