# Comparing `tmp/heat-1.2.2.tar.gz` & `tmp/heat-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heat-1.2.2.tar", last modified: Thu Jan 19 08:33:43 2023, max compression
+gzip compressed data, was "heat-1.3.0.tar", last modified: Tue Jun 20 14:17:33 2023, max compression
```

## Comparing `heat-1.2.2.tar` & `heat-1.3.0.tar`

### file list

```diff
@@ -1,103 +1,112 @@
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:43.029401 heat-1.2.2/
--rw-r--r--   0 c.comito   (501) staff       (20)     1192 2022-07-21 04:14:34.000000 heat-1.2.2/LICENSE
--rw-r--r--   0 c.comito   (501) staff       (20)     7196 2023-01-19 08:33:43.029486 heat-1.2.2/PKG-INFO
--rw-r--r--   0 c.comito   (501) staff       (20)     6412 2023-01-19 08:23:06.000000 heat-1.2.2/README.md
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:42.991288 heat-1.2.2/heat/
--rw-r--r--   0 c.comito   (501) staff       (20)      352 2023-01-19 08:23:06.000000 heat-1.2.2/heat/__init__.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:42.993531 heat-1.2.2/heat/classification/
--rw-r--r--   0 c.comito   (501) staff       (20)       79 2022-07-21 04:14:34.000000 heat-1.2.2/heat/classification/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)     4820 2022-07-21 04:14:34.000000 heat-1.2.2/heat/classification/kneighborsclassifier.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:42.995893 heat-1.2.2/heat/cluster/
--rw-r--r--   0 c.comito   (501) staff       (20)      185 2022-07-21 04:14:34.000000 heat-1.2.2/heat/cluster/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)     9604 2022-07-21 04:14:34.000000 heat-1.2.2/heat/cluster/_kcluster.py
--rw-r--r--   0 c.comito   (501) staff       (20)     5342 2022-07-21 04:14:34.000000 heat-1.2.2/heat/cluster/kmeans.py
--rw-r--r--   0 c.comito   (501) staff       (20)     5398 2022-07-21 04:14:34.000000 heat-1.2.2/heat/cluster/kmedians.py
--rw-r--r--   0 c.comito   (501) staff       (20)     6093 2022-07-21 04:14:34.000000 heat-1.2.2/heat/cluster/kmedoids.py
--rw-r--r--   0 c.comito   (501) staff       (20)     8189 2022-11-04 11:46:24.000000 heat-1.2.2/heat/cluster/spectral.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:43.016340 heat-1.2.2/heat/core/
--rw-r--r--   0 c.comito   (501) staff       (20)      761 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    19964 2023-01-19 08:23:06.000000 heat-1.2.2/heat/core/_operations.py
--rw-r--r--   0 c.comito   (501) staff       (20)    34923 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/arithmetics.py
--rw-r--r--   0 c.comito   (501) staff       (20)     7455 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/base.py
--rw-r--r--   0 c.comito   (501) staff       (20)    71029 2023-01-19 08:23:12.000000 heat-1.2.2/heat/core/communication.py
--rw-r--r--   0 c.comito   (501) staff       (20)     3166 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/complex_math.py
--rw-r--r--   0 c.comito   (501) staff       (20)     1072 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/constants.py
--rw-r--r--   0 c.comito   (501) staff       (20)     4467 2022-11-28 04:52:03.000000 heat-1.2.2/heat/core/devices.py
--rw-r--r--   0 c.comito   (501) staff       (20)    68607 2023-01-19 08:23:12.000000 heat-1.2.2/heat/core/dndarray.py
--rw-r--r--   0 c.comito   (501) staff       (20)    10997 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/exponential.py
--rw-r--r--   0 c.comito   (501) staff       (20)    50421 2023-01-16 06:08:23.000000 heat-1.2.2/heat/core/factories.py
--rw-r--r--   0 c.comito   (501) staff       (20)     5439 2023-01-14 06:32:48.000000 heat-1.2.2/heat/core/indexing.py
--rw-r--r--   0 c.comito   (501) staff       (20)    44078 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/io.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:43.018117 heat-1.2.2/heat/core/linalg/
--rw-r--r--   0 c.comito   (501) staff       (20)      136 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/linalg/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    89679 2023-01-19 08:23:12.000000 heat-1.2.2/heat/core/linalg/basics.py
--rw-r--r--   0 c.comito   (501) staff       (20)    45178 2022-08-29 02:49:58.000000 heat-1.2.2/heat/core/linalg/qr.py
--rw-r--r--   0 c.comito   (501) staff       (20)    10452 2023-01-16 06:08:23.000000 heat-1.2.2/heat/core/linalg/solver.py
--rw-r--r--   0 c.comito   (501) staff       (20)       58 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/linalg/svd.py
--rw-r--r--   0 c.comito   (501) staff       (20)    17923 2023-01-19 08:23:12.000000 heat-1.2.2/heat/core/logical.py
--rw-r--r--   0 c.comito   (501) staff       (20)   149205 2023-01-19 08:23:12.000000 heat-1.2.2/heat/core/manipulations.py
--rw-r--r--   0 c.comito   (501) staff       (20)     2851 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/memory.py
--rw-r--r--   0 c.comito   (501) staff       (20)    10729 2022-12-12 08:04:57.000000 heat-1.2.2/heat/core/printing.py
--rw-r--r--   0 c.comito   (501) staff       (20)    37457 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/random.py
--rw-r--r--   0 c.comito   (501) staff       (20)    13189 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/relational.py
--rw-r--r--   0 c.comito   (501) staff       (20)    15411 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/rounding.py
--rw-r--r--   0 c.comito   (501) staff       (20)    12667 2022-11-29 10:05:10.000000 heat-1.2.2/heat/core/sanitation.py
--rw-r--r--   0 c.comito   (501) staff       (20)     5135 2022-12-23 05:59:47.000000 heat-1.2.2/heat/core/signal.py
--rw-r--r--   0 c.comito   (501) staff       (20)    75631 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/statistics.py
--rw-r--r--   0 c.comito   (501) staff       (20)     6792 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/stride_tricks.py
--rw-r--r--   0 c.comito   (501) staff       (20)    52486 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/tiling.py
--rw-r--r--   0 c.comito   (501) staff       (20)    16274 2022-07-21 04:14:34.000000 heat-1.2.2/heat/core/trigonometrics.py
--rw-r--r--   0 c.comito   (501) staff       (20)    28163 2022-12-26 06:55:14.000000 heat-1.2.2/heat/core/types.py
--rw-r--r--   0 c.comito   (501) staff       (20)      559 2023-01-19 08:23:44.000000 heat-1.2.2/heat/core/version.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:43.022881 heat-1.2.2/heat/datasets/
--rw-r--r--   0 c.comito   (501) staff       (20)       50 2022-07-21 04:14:34.000000 heat-1.2.2/heat/datasets/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    25312 2022-07-21 04:14:34.000000 heat-1.2.2/heat/datasets/diabetes.h5
--rw-r--r--   0 c.comito   (501) staff       (20)     2400 2022-07-21 04:14:34.000000 heat-1.2.2/heat/datasets/iris.csv
--rw-r--r--   0 c.comito   (501) staff       (20)     6944 2022-07-21 04:14:34.000000 heat-1.2.2/heat/datasets/iris.h5
--rw-r--r--   0 c.comito   (501) staff       (20)    11040 2022-07-21 04:14:34.000000 heat-1.2.2/heat/datasets/iris.nc
--rw-r--r--   0 c.comito   (501) staff       (20)     1800 2022-07-21 04:14:34.000000 heat-1.2.2/heat/datasets/iris_X_test.csv
--rw-r--r--   0 c.comito   (501) staff       (20)     1800 2022-07-21 04:14:34.000000 heat-1.2.2/heat/datasets/iris_X_train.csv
--rw-r--r--   0 c.comito   (501) staff       (20)      300 2022-07-21 04:14:34.000000 heat-1.2.2/heat/datasets/iris_labels.csv
--rw-r--r--   0 c.comito   (501) staff       (20)     5669 2022-07-21 04:14:34.000000 heat-1.2.2/heat/datasets/iris_y_pred_proba.csv
--rw-r--r--   0 c.comito   (501) staff       (20)      150 2022-07-21 04:14:34.000000 heat-1.2.2/heat/datasets/iris_y_test.csv
--rw-r--r--   0 c.comito   (501) staff       (20)      150 2022-07-21 04:14:34.000000 heat-1.2.2/heat/datasets/iris_y_train.csv
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:43.024092 heat-1.2.2/heat/graph/
--rw-r--r--   0 c.comito   (501) staff       (20)       86 2022-07-21 04:14:34.000000 heat-1.2.2/heat/graph/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)     4962 2022-07-21 04:14:34.000000 heat-1.2.2/heat/graph/laplacian.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:43.024506 heat-1.2.2/heat/naive_bayes/
--rw-r--r--   0 c.comito   (501) staff       (20)       88 2022-07-21 04:14:34.000000 heat-1.2.2/heat/naive_bayes/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    22418 2022-07-21 04:14:34.000000 heat-1.2.2/heat/naive_bayes/gaussianNB.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:43.025240 heat-1.2.2/heat/nn/
--rw-r--r--   0 c.comito   (501) staff       (20)     2265 2022-07-21 04:14:34.000000 heat-1.2.2/heat/nn/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    16594 2022-07-21 04:14:34.000000 heat-1.2.2/heat/nn/data_parallel.py
--rw-r--r--   0 c.comito   (501) staff       (20)     1558 2022-07-21 04:14:34.000000 heat-1.2.2/heat/nn/functional.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:43.026501 heat-1.2.2/heat/optim/
--rw-r--r--   0 c.comito   (501) staff       (20)     2507 2022-07-21 04:14:34.000000 heat-1.2.2/heat/optim/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    38332 2022-07-21 04:14:34.000000 heat-1.2.2/heat/optim/dp_optimizer.py
--rw-r--r--   0 c.comito   (501) staff       (20)     1083 2022-07-21 04:14:34.000000 heat-1.2.2/heat/optim/lr_scheduler.py
--rw-r--r--   0 c.comito   (501) staff       (20)     7171 2022-07-21 04:14:34.000000 heat-1.2.2/heat/optim/utils.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:43.026942 heat-1.2.2/heat/regression/
--rw-r--r--   0 c.comito   (501) staff       (20)       80 2022-07-21 04:14:34.000000 heat-1.2.2/heat/regression/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)     5653 2022-07-21 04:14:34.000000 heat-1.2.2/heat/regression/lasso.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:43.027375 heat-1.2.2/heat/spatial/
--rw-r--r--   0 c.comito   (501) staff       (20)       93 2022-07-21 04:14:34.000000 heat-1.2.2/heat/spatial/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    18389 2022-07-21 04:14:34.000000 heat-1.2.2/heat/spatial/distance.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:43.027888 heat-1.2.2/heat/utils/
--rw-r--r--   0 c.comito   (501) staff       (20)      112 2022-07-21 04:14:34.000000 heat-1.2.2/heat/utils/__init__.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:43.029234 heat-1.2.2/heat/utils/data/
--rw-r--r--   0 c.comito   (501) staff       (20)      171 2022-07-21 04:14:34.000000 heat-1.2.2/heat/utils/data/__init__.py
--rw-r--r--   0 c.comito   (501) staff       (20)    13358 2022-07-21 04:14:34.000000 heat-1.2.2/heat/utils/data/_utils.py
--rw-r--r--   0 c.comito   (501) staff       (20)    17539 2022-07-21 04:14:34.000000 heat-1.2.2/heat/utils/data/datatools.py
--rw-r--r--   0 c.comito   (501) staff       (20)     2425 2022-07-21 04:14:34.000000 heat-1.2.2/heat/utils/data/matrixgallery.py
--rw-r--r--   0 c.comito   (501) staff       (20)     4853 2022-07-21 04:14:34.000000 heat-1.2.2/heat/utils/data/mnist.py
--rw-r--r--   0 c.comito   (501) staff       (20)    15496 2022-07-21 04:14:34.000000 heat-1.2.2/heat/utils/data/partial_dataset.py
--rw-r--r--   0 c.comito   (501) staff       (20)     1661 2022-07-21 04:14:34.000000 heat-1.2.2/heat/utils/vision_transforms.py
-drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-01-19 08:33:42.992686 heat-1.2.2/heat.egg-info/
--rw-r--r--   0 c.comito   (501) staff       (20)     7196 2023-01-19 08:33:42.000000 heat-1.2.2/heat.egg-info/PKG-INFO
--rw-r--r--   0 c.comito   (501) staff       (20)     2108 2023-01-19 08:33:42.000000 heat-1.2.2/heat.egg-info/SOURCES.txt
--rw-r--r--   0 c.comito   (501) staff       (20)        1 2023-01-19 08:33:42.000000 heat-1.2.2/heat.egg-info/dependency_links.txt
--rw-r--r--   0 c.comito   (501) staff       (20)      245 2023-01-19 08:33:42.000000 heat-1.2.2/heat.egg-info/requires.txt
--rw-r--r--   0 c.comito   (501) staff       (20)        5 2023-01-19 08:33:42.000000 heat-1.2.2/heat.egg-info/top_level.txt
--rw-r--r--   0 c.comito   (501) staff       (20)       31 2022-07-21 04:14:34.000000 heat-1.2.2/pyproject.toml
--rw-r--r--   0 c.comito   (501) staff       (20)      327 2023-01-19 08:33:43.029834 heat-1.2.2/setup.cfg
--rw-r--r--   0 c.comito   (501) staff       (20)     1623 2023-01-19 08:23:12.000000 heat-1.2.2/setup.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.525972 heat-1.3.0/
+-rw-r--r--   0 c.comito   (501) staff       (20)     1192 2022-07-21 04:14:34.000000 heat-1.3.0/LICENSE
+-rw-r--r--   0 c.comito   (501) staff       (20)     9939 2023-06-20 14:17:33.526068 heat-1.3.0/PKG-INFO
+-rw-r--r--   0 c.comito   (501) staff       (20)     9085 2023-06-13 08:37:46.000000 heat-1.3.0/README.md
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.495159 heat-1.3.0/heat/
+-rw-r--r--   0 c.comito   (501) staff       (20)      373 2023-05-18 06:09:45.000000 heat-1.3.0/heat/__init__.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.497814 heat-1.3.0/heat/classification/
+-rw-r--r--   0 c.comito   (501) staff       (20)       79 2022-07-21 04:14:34.000000 heat-1.3.0/heat/classification/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     4716 2023-06-20 13:15:54.000000 heat-1.3.0/heat/classification/kneighborsclassifier.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.500846 heat-1.3.0/heat/cluster/
+-rw-r--r--   0 c.comito   (501) staff       (20)      185 2022-07-21 04:14:34.000000 heat-1.3.0/heat/cluster/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     9597 2023-06-20 13:15:54.000000 heat-1.3.0/heat/cluster/_kcluster.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     5336 2023-06-20 13:15:54.000000 heat-1.3.0/heat/cluster/kmeans.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     5391 2023-06-20 13:15:54.000000 heat-1.3.0/heat/cluster/kmedians.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     6087 2023-06-20 13:15:54.000000 heat-1.3.0/heat/cluster/kmedoids.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     8174 2023-06-20 13:15:54.000000 heat-1.3.0/heat/cluster/spectral.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.510192 heat-1.3.0/heat/core/
+-rw-r--r--   0 c.comito   (501) staff       (20)      761 2022-07-21 04:14:34.000000 heat-1.3.0/heat/core/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    19854 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/_operations.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    35615 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/arithmetics.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     7395 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/base.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    70818 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/communication.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     3166 2022-07-21 04:14:34.000000 heat-1.3.0/heat/core/complex_math.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     1072 2022-07-21 04:14:34.000000 heat-1.3.0/heat/core/constants.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     4951 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/devices.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    73359 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/dndarray.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    10997 2022-07-21 04:14:34.000000 heat-1.3.0/heat/core/exponential.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    56979 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/factories.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     5399 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/indexing.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    43828 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/io.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.511888 heat-1.3.0/heat/core/linalg/
+-rw-r--r--   0 c.comito   (501) staff       (20)      160 2023-06-16 09:52:23.000000 heat-1.3.0/heat/core/linalg/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    89467 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/linalg/basics.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    44959 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/linalg/qr.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    10320 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/linalg/solver.py
+-rw-r--r--   0 c.comito   (501) staff       (20)      566 2023-06-16 09:52:23.000000 heat-1.3.0/heat/core/linalg/svd.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    25597 2023-06-20 08:05:54.000000 heat-1.3.0/heat/core/linalg/svdtools.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    17929 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/logical.py
+-rw-r--r--   0 c.comito   (501) staff       (20)   152131 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/manipulations.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     2942 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/memory.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    10383 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/printing.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    37382 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/random.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    13166 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/relational.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    15182 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/rounding.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    12399 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/sanitation.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     7345 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/signal.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    75639 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/statistics.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     6688 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/stride_tricks.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    52201 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/tiling.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    16274 2022-07-21 04:14:34.000000 heat-1.3.0/heat/core/trigonometrics.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    28107 2023-06-20 13:15:54.000000 heat-1.3.0/heat/core/types.py
+-rw-r--r--   0 c.comito   (501) staff       (20)      534 2023-06-20 13:17:10.000000 heat-1.3.0/heat/core/version.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.514982 heat-1.3.0/heat/datasets/
+-rw-r--r--   0 c.comito   (501) staff       (20)       50 2022-07-21 04:14:34.000000 heat-1.3.0/heat/datasets/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    25312 2022-07-21 04:14:34.000000 heat-1.3.0/heat/datasets/diabetes.h5
+-rw-r--r--   0 c.comito   (501) staff       (20)     2400 2022-07-21 04:14:34.000000 heat-1.3.0/heat/datasets/iris.csv
+-rw-r--r--   0 c.comito   (501) staff       (20)     6944 2022-07-21 04:14:34.000000 heat-1.3.0/heat/datasets/iris.h5
+-rw-r--r--   0 c.comito   (501) staff       (20)    11040 2022-07-21 04:14:34.000000 heat-1.3.0/heat/datasets/iris.nc
+-rw-r--r--   0 c.comito   (501) staff       (20)     1800 2022-07-21 04:14:34.000000 heat-1.3.0/heat/datasets/iris_X_test.csv
+-rw-r--r--   0 c.comito   (501) staff       (20)     1800 2022-07-21 04:14:34.000000 heat-1.3.0/heat/datasets/iris_X_train.csv
+-rw-r--r--   0 c.comito   (501) staff       (20)      300 2022-07-21 04:14:34.000000 heat-1.3.0/heat/datasets/iris_labels.csv
+-rw-r--r--   0 c.comito   (501) staff       (20)     5669 2022-07-21 04:14:34.000000 heat-1.3.0/heat/datasets/iris_y_pred_proba.csv
+-rw-r--r--   0 c.comito   (501) staff       (20)      150 2022-07-21 04:14:34.000000 heat-1.3.0/heat/datasets/iris_y_test.csv
+-rw-r--r--   0 c.comito   (501) staff       (20)      150 2022-07-21 04:14:34.000000 heat-1.3.0/heat/datasets/iris_y_train.csv
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.515426 heat-1.3.0/heat/graph/
+-rw-r--r--   0 c.comito   (501) staff       (20)       86 2022-07-21 04:14:34.000000 heat-1.3.0/heat/graph/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     4962 2022-07-21 04:14:34.000000 heat-1.3.0/heat/graph/laplacian.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.515900 heat-1.3.0/heat/naive_bayes/
+-rw-r--r--   0 c.comito   (501) staff       (20)       88 2022-07-21 04:14:34.000000 heat-1.3.0/heat/naive_bayes/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    22124 2023-06-20 13:15:54.000000 heat-1.3.0/heat/naive_bayes/gaussianNB.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.518556 heat-1.3.0/heat/nn/
+-rw-r--r--   0 c.comito   (501) staff       (20)     2265 2022-07-21 04:14:34.000000 heat-1.3.0/heat/nn/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    16357 2023-06-20 13:15:54.000000 heat-1.3.0/heat/nn/data_parallel.py
+-rw-r--r--   0 c.comito   (501) staff       (20)      630 2023-06-16 09:52:23.000000 heat-1.3.0/heat/nn/functional.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.519922 heat-1.3.0/heat/optim/
+-rw-r--r--   0 c.comito   (501) staff       (20)     2507 2022-07-21 04:14:34.000000 heat-1.3.0/heat/optim/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    38305 2023-06-20 13:15:54.000000 heat-1.3.0/heat/optim/dp_optimizer.py
+-rw-r--r--   0 c.comito   (501) staff       (20)      380 2023-06-16 09:52:23.000000 heat-1.3.0/heat/optim/lr_scheduler.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     7171 2022-07-21 04:14:34.000000 heat-1.3.0/heat/optim/utils.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.520381 heat-1.3.0/heat/regression/
+-rw-r--r--   0 c.comito   (501) staff       (20)       80 2022-07-21 04:14:34.000000 heat-1.3.0/heat/regression/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     5607 2023-06-20 13:15:54.000000 heat-1.3.0/heat/regression/lasso.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.522101 heat-1.3.0/heat/sparse/
+-rw-r--r--   0 c.comito   (501) staff       (20)      194 2023-05-18 06:09:45.000000 heat-1.3.0/heat/sparse/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     5681 2023-05-18 06:09:45.000000 heat-1.3.0/heat/sparse/_operations.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     3276 2023-05-18 06:09:45.000000 heat-1.3.0/heat/sparse/arithmetics.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     9922 2023-05-18 06:09:45.000000 heat-1.3.0/heat/sparse/dcsr_matrix.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    10088 2023-06-20 13:15:54.000000 heat-1.3.0/heat/sparse/factories.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     3000 2023-05-18 06:09:45.000000 heat-1.3.0/heat/sparse/manipulations.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.522556 heat-1.3.0/heat/spatial/
+-rw-r--r--   0 c.comito   (501) staff       (20)       93 2022-07-21 04:14:34.000000 heat-1.3.0/heat/spatial/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    18018 2023-06-20 13:15:54.000000 heat-1.3.0/heat/spatial/distance.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.523351 heat-1.3.0/heat/utils/
+-rw-r--r--   0 c.comito   (501) staff       (20)      112 2022-07-21 04:14:34.000000 heat-1.3.0/heat/utils/__init__.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.525667 heat-1.3.0/heat/utils/data/
+-rw-r--r--   0 c.comito   (501) staff       (20)      195 2023-06-13 08:37:46.000000 heat-1.3.0/heat/utils/data/__init__.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    13358 2023-06-20 13:15:54.000000 heat-1.3.0/heat/utils/data/_utils.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    17539 2022-07-21 04:14:34.000000 heat-1.3.0/heat/utils/data/datatools.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     6354 2023-06-16 09:52:23.000000 heat-1.3.0/heat/utils/data/matrixgallery.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     4849 2023-06-20 13:15:54.000000 heat-1.3.0/heat/utils/data/mnist.py
+-rw-r--r--   0 c.comito   (501) staff       (20)    15496 2023-06-20 13:15:54.000000 heat-1.3.0/heat/utils/data/partial_dataset.py
+-rw-r--r--   0 c.comito   (501) staff       (20)     1994 2023-06-13 08:37:46.000000 heat-1.3.0/heat/utils/data/spherical.py
+-rw-r--r--   0 c.comito   (501) staff       (20)      606 2023-06-16 09:52:23.000000 heat-1.3.0/heat/utils/vision_transforms.py
+drwxr-xr-x   0 c.comito   (501) staff       (20)        0 2023-06-20 14:17:33.497032 heat-1.3.0/heat.egg-info/
+-rw-r--r--   0 c.comito   (501) staff       (20)     9939 2023-06-20 14:17:33.000000 heat-1.3.0/heat.egg-info/PKG-INFO
+-rw-r--r--   0 c.comito   (501) staff       (20)     2325 2023-06-20 14:17:33.000000 heat-1.3.0/heat.egg-info/SOURCES.txt
+-rw-r--r--   0 c.comito   (501) staff       (20)        1 2023-06-20 14:17:33.000000 heat-1.3.0/heat.egg-info/dependency_links.txt
+-rw-r--r--   0 c.comito   (501) staff       (20)      263 2023-06-20 14:17:33.000000 heat-1.3.0/heat.egg-info/requires.txt
+-rw-r--r--   0 c.comito   (501) staff       (20)        5 2023-06-20 14:17:33.000000 heat-1.3.0/heat.egg-info/top_level.txt
+-rw-r--r--   0 c.comito   (501) staff       (20)       31 2022-07-21 04:14:34.000000 heat-1.3.0/pyproject.toml
+-rw-r--r--   0 c.comito   (501) staff       (20)      327 2023-06-20 14:17:33.526446 heat-1.3.0/setup.cfg
+-rw-r--r--   0 c.comito   (501) staff       (20)     1704 2023-06-16 09:52:23.000000 heat-1.3.0/setup.py
```

### Comparing `heat-1.2.2/LICENSE` & `heat-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/PKG-INFO` & `heat-1.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,174 @@
-Metadata-Version: 2.1
-Name: heat
-Version: 1.2.2
-Summary: A framework for high-performance data analytics and machine learning.
-Home-page: https://github.com/helmholtz-analytics/heat
-Author: Helmholtz Association
-Author-email: martin.siggel@dlr.de
-Keywords: data,analytics,tensors,distributed,gpu
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: docutils
-Provides-Extra: hdf5
-Provides-Extra: netcdf
-Provides-Extra: dev
-Provides-Extra: examples
-License-File: LICENSE
-
 <div align="center">
   <img src="https://raw.githubusercontent.com/helmholtz-analytics/heat/main/doc/images/logo.png">
 </div>
 
 ---
 
 Heat is a distributed tensor framework for high performance data analytics.
 
-Project Status
---------------
-[![Mirror and run GitLab CI](https://github.com/helmholtz-analytics/heat/actions/workflows/ci_cpu.yml/badge.svg)](https://github.com/helmholtz-analytics/heat/actions/workflows/ci_cpu.yml)
+# Project Status
+
+[![pipeline status](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/badges/heat/base/pipeline.svg)](https://codebase.helmholtz.cloud/helmholtz-analytics/ci/-/commits/heat/base)
 [![Documentation Status](https://readthedocs.org/projects/heat/badge/?version=latest)](https://heat.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/helmholtz-analytics/heat/branch/main/graph/badge.svg)](https://codecov.io/gh/helmholtz-analytics/heat)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![license: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![Downloads](https://pepy.tech/badge/heat)](https://pepy.tech/project/heat)
+[![Github-Pages - Benchmarks](https://img.shields.io/badge/Github--Pages-Benchmarks-2ea44f)](https://helmholtz-analytics.github.io/heat/dev/bench)
 
-Goals
------
+# Goals
 
 Heat is a flexible and seamless open-source software for high performance data
 analytics and machine learning. It provides highly optimized algorithms and data
 structures for tensor computations using CPUs, GPUs and distributed cluster
 systems on top of MPI. The goal of Heat is to fill the gap between data
 analytics and machine learning libraries with a strong focus on single-node
 performance, and traditional high-performance computing (HPC). Heat's generic
 Python-first programming interface integrates seamlessly with the existing data
 science ecosystem and makes it as effortless as using numpy to write scalable
 scientific and data science applications.
 
 Heat allows you to tackle your actual Big Data challenges that go beyond the
 computational and memory needs of your laptop and desktop.
 
-Features
---------
+# Features
 
 * High-performance n-dimensional tensors
 * CPU, GPU and distributed computation using MPI
 * Powerful data analytics and machine learning methods
 * Abstracted communication via split tensors
 * Python API
 
-Getting Started
----------------
-
-Check out our Jupyter Notebook [tutorial](https://github.com/helmholtz-analytics/heat/blob/main/scripts/tutorial.ipynb)
-right here on Github or in the /scripts directory.
-
-The complete documentation of the latest version is always deployed on
-[Read the Docs](https://heat.readthedocs.io/).
+# Support Channels
 
-Support Channels
-----------------
+We use [GitHub Discussions](https://github.com/helmholtz-analytics/heat/discussions) as a forum for questions about Heat.
+If you found a bug or miss a feature, then please file a new [issue](https://github.com/helmholtz-analytics/heat/issues/new/choose).
 
-We use [StackOverflow](https://stackoverflow.com/tags/pyheat/) as a forum for questions about Heat.
-If you do not find an answer to your question, then please ask a new question there and be sure to
-tag it with "pyheat".
-
-You can also reach us on [GitHub Discussions](https://github.com/helmholtz-analytics/heat/discussions).
-
-Requirements
-------------
+# Requirements
 
 Heat requires Python 3.7 or newer.
 Heat is based on [PyTorch](https://pytorch.org/). Specifically, we are exploiting
 PyTorch's support for GPUs *and* MPI parallelism. For MPI support we utilize
 [mpi4py](https://mpi4py.readthedocs.io). Both packages can be installed via pip
 or automatically using the setup.py.
 
-
-Installation
-------------
+# Installation
 
 Tagged releases are made available on the
 [Python Package Index (PyPI)](https://pypi.org/project/heat/). You can typically
 install the latest version with
 
-> $ pip install heat[hdf5,netcdf]
+```
+$ pip install heat[hdf5,netcdf]
+```
 
 where the part in brackets is a list of optional dependencies. You can omit
 it, if you do not need HDF5 or NetCDF support.
 
 **It is recommended to use the most recent supported version of PyTorch!**
 
-It is also very important to ensure that the PyTorch version is compatible with the local CUDA installation.
+**It is also very important to ensure that the PyTorch version is compatible with the local CUDA installation.**
 More information can be found [here](https://pytorch.org/get-started/locally/).
 
-Hacking
--------
+# Hacking
 
 If you want to work with the development version, you can check out the sources using
 
-> $ git clone https://github.com/helmholtz-analytics/heat.git
+```
+$ git clone <https://github.com/helmholtz-analytics/heat.git>
+```
 
 The installation can then be done from the checked-out sources with
 
-> $ pip install .[hdf5,netcdf,dev]
+```
+$ pip install heat[hdf5,netcdf,dev]
+```
+
+# Getting Started
+
+TL;DR: [Quick Start](quick_start.md) (Read this to get a quick overview of Heat).
+
+Check out our Jupyter Notebook [**Tutorial**](https://github.com/helmholtz-analytics/heat/blob/main/scripts/)
+right here on Github or in the /scripts directory, to learn and understand about the basics and working of Heat.
+
+The complete documentation of the latest version is always deployed on
+[Read the Docs](https://heat.readthedocs.io/).
+
+***Try your first Heat program***
+
+```shell
+$ python
+```
+
+```python
+>>> import heat as ht
+>>> x = ht.arange(10,split=0)
+>>> print(x)
+DNDarray([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=ht.int32, device=cpu:0, split=0)
+>>> y = ht.ones(10,split=0)
+>>> print(y)
+DNDarray([1., 1., 1., 1., 1., 1., 1., 1., 1., 1.], dtype=ht.float32, device=cpu:0, split=0)
+>>> print(x + y)
+DNDarray([ 1.,  2.,  3.,  4.,  5.,  6.,  7.,  8.,  9., 10.], dtype=ht.float32, device=cpu:0, split=0)
+```
+
+### Also, you can test your setup by running the [`heat_test.py`](https://github.com/helmholtz-analytics/heat/blob/main/scripts/heat_test.py) script:
+
+```shell
+mpirun -n 2 python heat_test.py
+```
+
+### It should print something like this:
+
+```shell
+x is distributed:  True
+Global DNDarray x:  DNDarray([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=ht.int32, device=cpu:0, split=0)
+Global DNDarray x:
+Local torch tensor on rank  0 :  tensor([0, 1, 2, 3, 4], dtype=torch.int32)
+Local torch tensor on rank  1 :  tensor([5, 6, 7, 8, 9], dtype=torch.int32)
+```
+
+## Resources:
+
+* [Heat Tutorials](https://heat.readthedocs.io/en/latest/tutorials.html)
+* [Heat API Reference](https://heat.readthedocs.io/en/latest/autoapi/index.html)
+
+### Parallel Computing and MPI:
+
+* @davidhenty's [course](https://www.archer2.ac.uk/training/courses/200514-mpi/)
+* Wes Kendall's [Tutorials](https://mpitutorial.com/tutorials/)
+
+### mpi4py
+
+* [mpi4py docs](https://mpi4py.readthedocs.io/en/stable/tutorial.html)
+* [Tutorial](https://www.kth.se/blogs/pdc/2019/08/parallel-programming-in-python-mpi4py-part-1/)
+
+# Contribution guidelines
+
+**We welcome contributions from the community, if you want to contribute to Heat, be sure to review the [Contribution Guidelines](contributing.md) before getting started!**
+
+We use [GitHub issues](https://github.com/helmholtz-analytics/heat/issues) for tracking requests and bugs, please see [Discussions](https://github.com/helmholtz-analytics/heat/discussions) for general questions and discussion, and You can also get in touch with us on [Mattermost](https://mattermost.hzdr.de/signup_user_complete/?id=3sixwk9okpbzpjyfrhen5jpqfo). You can sign up with your GitHub credentials. Once you log in, you can introduce yourself on the `Town Square` channel.
+
+Small improvements or fixes are always appreciated; issues labeled as **"good first issue"** may be a good starting point.
+
+If you’re unsure where to start or how your skills fit in, reach out! You can ask us here on GitHub, by leaving a comment on a relevant issue that is already open.
 
-We welcome contributions from the community, please check out our [Contribution Guidelines](contributing.md) before getting started!
+**If you are new to contributing to open source, [this guide](https://opensource.guide/how-to-contribute/) helps explain why, what, and how to get involved.**
 
-License
--------
+# License
 
 Heat is distributed under the MIT license, see our
 [LICENSE](LICENSE) file.
 
-Citing Heat
------------
+# Citing Heat
 
 If you find Heat helpful for your research, please mention it in your publications. You can cite:
 
-- Götz, M., Debus, C., Coquelin, D., Krajsek, K., Comito, C., Knechtges, P., Hagemeier, B., Tarnawa, M., Hanselmann, S., Siggel, S., Basermann, A. & Streit, A. (2020). HeAT - a Distributed and GPU-accelerated Tensor Framework for Data Analytics. In 2020 IEEE International Conference on Big Data (Big Data) (pp. 276-287). IEEE, DOI: 10.1109/BigData50022.2020.9378050.
+* Götz, M., Debus, C., Coquelin, D., Krajsek, K., Comito, C., Knechtges, P., Hagemeier, B., Tarnawa, M., Hanselmann, S., Siggel, S., Basermann, A. & Streit, A. (2020). HeAT - a Distributed and GPU-accelerated Tensor Framework for Data Analytics. In 2020 IEEE International Conference on Big Data (Big Data) (pp. 276-287). IEEE, DOI: 10.1109/BigData50022.2020.9378050.
 
 ```
 @inproceedings{heat2020,
     title={{HeAT -- a Distributed and GPU-accelerated Tensor Framework for Data Analytics}},
     author={
       Markus Götz and
       Charlotte Debus and
@@ -156,16 +188,15 @@
     pages={276-287},
     month={December},
     publisher={IEEE},
     doi={10.1109/BigData50022.2020.9378050}
 }
 ```
 
-Acknowledgements
-----------------
+## Acknowledgements
 
 *This work is supported by the [Helmholtz Association Initiative and
 Networking Fund](https://www.helmholtz.de/en/about_us/the_association/initiating_and_networking/)
 under project number ZT-I-0003 and the Helmholtz AI platform grant.*
 
 ---
```

### Comparing `heat-1.2.2/heat/classification/kneighborsclassifier.py` & `heat-1.3.0/heat/classification/kneighborsclassifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,41 +82,37 @@
         --------
         >>> samples = ht.rand(10, 3)
         >>> knn = KNeighborsClassifier(n_neighbors=1)
         >>> knn.fit(samples)
         """
         # check for type consistency
         if not isinstance(x, DNDarray) or not isinstance(y, DNDarray):
-            raise TypeError("x and y must be DNDarrays but were {} {}".format(type(x), type(y)))
+            raise TypeError(f"x and y must be DNDarrays but were {type(x)} {type(y)}")
 
         # ensure that x is a two-dimensional matrix
         if len(x.shape) != 2:
-            raise ValueError("x must be two-dimensional, but was {}".format(len(x.shape)))
+            raise ValueError(f"x must be two-dimensional, but was {len(x.shape)}")
         self.x = x
         self.n_samples_fit_ = x.shape[0]
 
         # ensure that x and y have the same number of samples
         if x.shape[0] != y.shape[0]:
             raise ValueError(
-                "Number of samples x and y samples mismatch, got {}, {}".format(
-                    x.shape[0], y.shape[0]
-                )
+                f"Number of samples x and y samples mismatch, got {x.shape[0]}, {y.shape[0]}"
             )
 
         # checks the labels for correct dimensionality and encode one-hot
         if len(y.shape) == 1:
             self.y = self.one_hot_encoding(y)
             self.outputs_2d_ = False
         elif len(y.shape) == 2:
             self.y = y
             self.outputs_2d_ = True
         else:
-            raise ValueError(
-                "y needs to be one- or two-dimensional, but was {}".format(len(y.shape))
-            )
+            raise ValueError(f"y needs to be one- or two-dimensional, but was {len(y.shape)}")
 
     def predict(self, x: DNDarray) -> DNDarray:
         """
         Predict the class labels for the provided data.
 
         Parameters
         ----------
```

### Comparing `heat-1.2.2/heat/cluster/_kcluster.py` & `heat-1.3.0/heat/cluster/_kcluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         Parameters
         ----------
         x : DNDarray
             Data points, Shape = (n_samples, n_features)
         """
         # calculate the distance matrix and determine the closest centroid
         distances = self._metric(x, self._cluster_centers)
-        matching_centroids = distances.argmin(axis=1, keepdim=True)
+        matching_centroids = distances.argmin(axis=1, keepdims=True)
 
         return matching_centroids
 
     def _update_centroids(self, x: DNDarray, matching_centroids: DNDarray):
         """
         The Update strategy is algorithm specific (e.g. calculate mean of assigned points for kmeans, median for kmedians, etc.)
 
@@ -244,11 +244,11 @@
         Parameters
         ----------
         x : DNDarray
             New data to predict. Shape = (n_samples, n_features)
         """
         # input sanitation
         if not isinstance(x, DNDarray):
-            raise ValueError("input needs to be a ht.DNDarray, but was {}".format(type(x)))
+            raise ValueError(f"input needs to be a ht.DNDarray, but was {type(x)}")
 
         # determine the centroids
         return self._assign_to_cluster(x)
```

### Comparing `heat-1.2.2/heat/cluster/kmeans.py` & `heat-1.3.0/heat/cluster/kmeans.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,21 +84,21 @@
         """
         new_cluster_centers = self._cluster_centers.copy()
         for i in range(self.n_clusters):
             # points in current cluster
             selection = (matching_centroids == i).astype(ht.int64)
             # accumulate points and total number of points in cluster
             assigned_points = x * selection
-            points_in_cluster = selection.sum(axis=0, keepdim=True).clip(
+            points_in_cluster = selection.sum(axis=0, keepdims=True).clip(
                 1.0, ht.iinfo(ht.int64).max
             )
 
             # compute the new centroids
             new_cluster_centers[i : i + 1, :] = (assigned_points / points_in_cluster).sum(
-                axis=0, keepdim=True
+                axis=0, keepdims=True
             )
 
         return new_cluster_centers
 
     def fit(self, x: DNDarray) -> self:
         """
         Computes the centroid of a k-means clustering.
@@ -107,15 +107,15 @@
         ----------
         x : DNDarray
             Training instances to cluster. Shape = (n_samples, n_features)
 
         """
         # input sanitation
         if not isinstance(x, DNDarray):
-            raise ValueError("input needs to be a ht.DNDarray, but was {}".format(type(x)))
+            raise ValueError(f"input needs to be a ht.DNDarray, but was {type(x)}")
 
         # initialize the clustering
         self._initialize_cluster_centers(x)
         self._n_iter = 0
         matching_centroids = ht.zeros((x.shape[0]), split=x.split, device=x.device, comm=x.comm)
 
         # iteratively fit the points to the centroids
```

### Comparing `heat-1.2.2/heat/cluster/kmedians.py` & `heat-1.3.0/heat/cluster/kmedians.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                     idx = sample - displ[proc]
                     xi = ht.array(x.lloc[idx, :], device=x.device, comm=x.comm)
                 xi.comm.Bcast(xi, root=proc)
                 new_cluster_centers[i, :] = xi
             else:
                 if clean.shape[0] <= ht.MPI_WORLD.size:
                     clean.resplit_(axis=None)
-                median = ht.median(clean, axis=0, keepdim=True)
+                median = ht.median(clean, axis=0, keepdims=True)
                 new_cluster_centers[i : i + 1, :] = median
 
         return new_cluster_centers
 
     def fit(self, x: DNDarray):
         """
         Computes the centroid of a k-medians clustering.
@@ -107,15 +107,15 @@
         Parameters
         ----------
         x : DNDarray
             Training instances to cluster. Shape = (n_samples, n_features)
         """
         # input sanitation
         if not isinstance(x, ht.DNDarray):
-            raise ValueError("input needs to be a ht.DNDarray, but was {}".format(type(x)))
+            raise ValueError(f"input needs to be a ht.DNDarray, but was {type(x)}")
 
         # initialize the clustering
         self._initialize_cluster_centers(x)
         self._n_iter = 0
         matching_centroids = ht.zeros((x.shape[0]), split=x.split, device=x.device, comm=x.comm)
         # iteratively fit the points to the centroids
         for epoch in range(self.max_iter):
```

### Comparing `heat-1.2.2/heat/cluster/kmedoids.py` & `heat-1.3.0/heat/cluster/kmedoids.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,19 +90,19 @@
                     xi = ht.array(x.lloc[idx, :], device=x.device, comm=x.comm)
                 xi.comm.Bcast(xi, root=proc)
                 new_cluster_centers[i, :] = xi
 
             else:
                 if clean.shape[0] <= ht.MPI_WORLD.size:
                     clean.resplit_(axis=None)
-                median = ht.median(clean, axis=0, keepdim=True)
+                median = ht.median(clean, axis=0, keepdims=True)
 
                 dist = self._metric(x, median)
                 _, displ, _ = x.comm.counts_displs_shape(shape=x.shape, axis=0)
-                idx = dist.argmin(axis=0, keepdim=False).item()
+                idx = dist.argmin(axis=0, keepdims=False).item()
                 proc = 0
                 for p in range(x.comm.size):
                     if displ[p] > idx:
                         break
                     proc = p
                 closest_point = ht.zeros(x.shape[1], dtype=x.dtype)
                 if x.comm.rank == proc:
@@ -120,15 +120,15 @@
         Parameters
         ----------
         x : DNDarray
             Training instances to cluster. Shape = (n_samples, n_features)
         """
         # input sanitation
         if not isinstance(x, DNDarray):
-            raise ValueError("input needs to be a ht.DNDarray, but was {}".format(type(x)))
+            raise ValueError(f"input needs to be a ht.DNDarray, but was {type(x)}")
 
         # initialize the clustering
         self._initialize_cluster_centers(x)
         self._n_iter = 0
         matching_centroids = ht.zeros((x.shape[0]), split=x.split, device=x.device, comm=x.comm)
         # iteratively fit the points to the centroids
         for epoch in range(self.max_iter):
```

### Comparing `heat-1.2.2/heat/cluster/spectral.py` & `heat-1.3.0/heat/cluster/spectral.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         gamma: float = 1.0,
         metric: str = "rbf",
         laplacian: str = "fully_connected",
         threshold: float = 1.0,
         boundary: str = "upper",
         n_lanczos: int = 300,
         assign_labels: str = "kmeans",
-        **params
+        **params,
     ):
         self.n_clusters = n_clusters
         self.gamma = gamma
         self.metric = metric
         self.laplacian = laplacian
         self.threshold = threshold
         self.boundary = boundary
@@ -160,15 +160,15 @@
         Parameters
         ----------
         x : DNDarray
             Training instances to cluster. Shape = (n_samples, n_features)
         """
         # 1. input sanitation
         if not isinstance(x, DNDarray):
-            raise ValueError("input needs to be a ht.DNDarray, but was {}".format(type(x)))
+            raise ValueError(f"input needs to be a ht.DNDarray, but was {type(x)}")
         if x.split is not None and x.split != 0:
             raise NotImplementedError("Not implemented for other splitting-axes")
         # 2. Embed Dataset into lower-dimensional Eigenvector space
         eigenvalues, eigenvectors = self._spectral_embedding(x)
 
         # 3. Find the spectral gap, if number of clusters is not defined from the outside
         if self.n_clusters is None:
@@ -202,15 +202,15 @@
         Warning
         -------
         Caution: Calculation of the low-dim representation requires some time!
 
         """
         # input sanitation
         if not isinstance(x, DNDarray):
-            raise ValueError("input needs to be a ht.DNDarray, but was {}".format(type(x)))
+            raise ValueError(f"input needs to be a ht.DNDarray, but was {type(x)}")
         if x.split is not None and x.split != 0:
             raise NotImplementedError("Not implemented for other splitting-axes")
 
         _, eigenvectors = self._spectral_embedding(x)
 
         components = eigenvectors[:, : self.n_clusters].copy()
```

### Comparing `heat-1.2.2/heat/core/__init__.py` & `heat-1.3.0/heat/core/__init__.py`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/core/_operations.py` & `heat-1.3.0/heat/core/_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Generalized MPI operations. i.e. element-wise binary operations
-"""
+"""Generalized operations for DNDarray"""
 
 import builtins
 import numpy as np
 import torch
 import warnings
 
 from .communication import MPI, MPI_WORLD
@@ -74,41 +72,39 @@
     1) split is preferred to no split
     2) no (shape)-broadcasting in the split dimension if not necessary
     3) t1 is preferred to t2
     """
     # Check inputs
     if not np.isscalar(t1) and not isinstance(t1, DNDarray):
         raise TypeError(
-            "Only DNDarrays and numeric scalars are supported, but input was {}".format(type(t1))
+            f"Only DNDarrays and numeric scalars are supported, but input was {type(t1)}"
         )
     if not np.isscalar(t2) and not isinstance(t2, DNDarray):
         raise TypeError(
-            "Only DNDarrays and numeric scalars are supported, but input was {}".format(type(t2))
+            f"Only DNDarrays and numeric scalars are supported, but input was {type(t2)}"
         )
     promoted_type = types.result_type(t1, t2).torch_type()
 
     # Make inputs Dndarrays
     if np.isscalar(t1) and np.isscalar(t2):
         try:
             t1 = factories.array(t1)
             t2 = factories.array(t2)
         except (ValueError, TypeError):
-            raise TypeError(
-                "Data type not supported, inputs were {} and {}".format(type(t1), type(t2))
-            )
+            raise TypeError(f"Data type not supported, inputs were {type(t1)} and {type(t2)}")
     elif np.isscalar(t1) and isinstance(t2, DNDarray):
         try:
             t1 = factories.array(t1, device=t2.device, comm=t2.comm)
         except (ValueError, TypeError):
-            raise TypeError("Data type not supported, input was {}".format(type(t1)))
+            raise TypeError(f"Data type not supported, input was {type(t1)}")
     elif isinstance(t1, DNDarray) and np.isscalar(t2):
         try:
             t2 = factories.array(t2, device=t1.device, comm=t1.comm)
         except (ValueError, TypeError):
-            raise TypeError("Data type not supported, input was {}".format(type(t2)))
+            raise TypeError(f"Data type not supported, input was {type(t2)}")
 
     # Make inputs have the same dimensionality
     output_shape = stride_tricks.broadcast_shape(t1.shape, t2.shape)
     if where is not None:
         output_shape = stride_tricks.broadcast_shape(where.shape, output_shape)
         while len(where.shape) < len(output_shape):
             where = where.expand_dims(axis=0)
@@ -294,24 +290,28 @@
         x.comm.Exscan(send, recv, exscan_op)
         final_op(cumop, recv, out=cumop)
 
     if out is not None:
         return out
 
     return factories.array(
-        cumop, dtype=x.dtype if dtype is None else dtype, is_split=x.split, device=x.device
+        cumop,
+        dtype=x.dtype if dtype is None else dtype,
+        is_split=x.split,
+        device=x.device,
+        comm=x.comm,
     )
 
 
 def __local_op(
     operation: Callable,
     x: DNDarray,
     out: Optional[DNDarray] = None,
     no_cast: Optional[bool] = False,
-    **kwargs
+    **kwargs,
 ) -> DNDarray:
     """
     Generic wrapper for local operations, which do not require communication. Accepts the actual operation function as
     argument and takes only care of buffer allocation/writing. This function is intended to work on an element-wise bases
 
     Parameters
     ----------
@@ -333,15 +333,15 @@
     -------
     TypeError
         If the input is not a tensor or the output is not a tensor or None.
     """
     # perform sanitation
     sanitation.sanitize_in(x)
     if out is not None and not isinstance(out, DNDarray):
-        raise TypeError("expected out to be None or an ht.DNDarray, but was {}".format(type(out)))
+        raise TypeError(f"expected out to be None or an ht.DNDarray, but was {type(out)}")
 
     # infer the output type of the tensor
     # we need floating point numbers here, due to PyTorch only providing sqrt() implementation for float32/64
     if not no_cast:
         promoted_type = types.promote_types(x.dtype, types.float32)
         torch_type = promoted_type.torch_type()
     else:
@@ -377,15 +377,15 @@
 
 
 def __reduce_op(
     x: DNDarray,
     partial_op: Callable,
     reduction_op: Callable,
     neutral: Optional[Union[int, float]] = None,
-    **kwargs
+    **kwargs,
 ) -> DNDarray:
     """
     Generic wrapper for reduction operations, e.g. :func:`sum() <heat.arithmetics.sum>`, :func:`prod() <heat.arithmetics.prod>`
     etc. Performs a two-stage reduction. First, a partial reduction is performed node-local that is combined into a
     global reduction result via an MPI_Op.
 
     Parameters
@@ -412,15 +412,15 @@
     # perform sanitation
     sanitation.sanitize_in(x)
 
     # no further checking needed, sanitize axis will raise the proper exceptions
     axis = stride_tricks.sanitize_axis(x.shape, kwargs.get("axis"))
     if isinstance(axis, int):
         axis = (axis,)
-    keepdim = kwargs.get("keepdim")
+    keepdims = kwargs.get("keepdims")
     out = kwargs.get("out")
     split = x.split
     balanced = x.balanced
 
     # if local tensor is empty, replace it with the identity element
     if x.is_distributed() and 0 in x.lshape and (axis is None or split in axis):
         if neutral is None:
@@ -444,15 +444,15 @@
         output_shape = x.gshape
         for dim in axis:
             if not (
                 partial.shape.numel() == 0 and partial_op.__name__ in ("local_max", "local_min")
             ):  # no neutral element for max/min
                 partial = partial_op(partial, dim=dim, keepdim=True)
             output_shape = output_shape[:dim] + (1,) + output_shape[dim + 1 :]
-        if not keepdim and not len(partial.shape) == 1:
+        if not keepdims and len(partial.shape) != 1:
             gshape_losedim = tuple(x.gshape[dim] for dim in range(len(x.gshape)) if dim not in axis)
             lshape_losedim = tuple(x.lshape[dim] for dim in range(len(x.lshape)) if dim not in axis)
             output_shape = gshape_losedim
             # Take care of special cases argmin and argmax: keep partial.shape[0]
             if 0 in axis and partial.shape[0] != 1:
                 lshape_losedim = (partial.shape[0],) + lshape_losedim
             if 0 not in axis and partial.shape[0] != x.lshape[0]:
@@ -462,15 +462,15 @@
     # perform a reduction operation in case the tensor is distributed across the reduction axis
     if x.split is not None:
         if axis is None or (x.split in axis):
             split = None
             balanced = True
             if x.comm.is_distributed():
                 x.comm.Allreduce(MPI.IN_PLACE, partial, reduction_op)
-        elif axis is not None and not keepdim:
+        elif axis is not None and not keepdims:
             down_dims = len(tuple(dim for dim in axis if dim < x.split))
             split -= down_dims
             balanced = x.balanced
 
     ARG_OPS = [statistics.MPI_ARGMAX, statistics.MPI_ARGMIN]
     arg_op = False
     if reduction_op in ARG_OPS:
@@ -483,17 +483,15 @@
     tensor_type = bool if reduction_op in __BOOLEAN_OPS else partial.dtype
 
     if out is not None:
         # sanitize out
         sanitation.sanitize_out(out, output_shape, split, x.device)
         if arg_op and out.dtype != types.canonical_heat_type(partial.dtype):
             raise TypeError(
-                "Data type mismatch: out.dtype should be {}, is {}".format(
-                    types.canonical_heat_type(partial.dtype), out.dtype
-                )
+                f"Data type mismatch: out.dtype should be {types.canonical_heat_type(partial.dtype)}, is {out.dtype}"
             )
         out._DNDarray__array = partial
         return out
 
     return DNDarray(
         partial,
         output_shape,
```

### Comparing `heat-1.2.2/heat/core/arithmetics.py` & `heat-1.3.0/heat/core/arithmetics.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     """
     dtypes = (heat_type_of(t1), heat_type_of(t2))
 
     for dt in dtypes:
         if heat_type_is_inexact(dt):
             raise TypeError("Operation is not supported for float types")
 
-    return _operations.__binary_op(torch.Tensor.__and__, t1, t2)
+    return _operations.__binary_op(torch.bitwise_and, t1, t2)
 
 
 DNDarray.__and__ = lambda self, other: bitwise_and(self, other)
 DNDarray.__and__.__doc__ = bitwise_and.__doc__
 
 
 def bitwise_or(t1: Union[DNDarray, float], t2: Union[DNDarray, float]) -> DNDarray:
@@ -171,15 +171,15 @@
     """
     dtypes = (heat_type_of(t1), heat_type_of(t2))
 
     for dt in dtypes:
         if heat_type_is_inexact(dt):
             raise TypeError("Operation is not supported for float types")
 
-    return _operations.__binary_op(torch.Tensor.__or__, t1, t2)
+    return _operations.__binary_op(torch.bitwise_or, t1, t2)
 
 
 DNDarray.__or__ = lambda self, other: bitwise_or(self, other)
 DNDarray.__or__.__doc__ = bitwise_or.__doc__
 
 
 def bitwise_xor(t1: Union[DNDarray, float], t2: Union[DNDarray, float]) -> DNDarray:
@@ -210,15 +210,15 @@
     """
     dtypes = (heat_type_of(t1), heat_type_of(t2))
 
     for dt in dtypes:
         if heat_type_is_inexact(dt):
             raise TypeError("Operation is not supported for float types")
 
-    return _operations.__binary_op(torch.Tensor.__xor__, t1, t2)
+    return _operations.__binary_op(torch.bitwise_xor, t1, t2)
 
 
 DNDarray.__xor__ = lambda self, other: bitwise_xor(self, other)
 DNDarray.__xor__.__doc__ = bitwise_xor.__doc__
 
 
 def cumprod(a: DNDarray, axis: int, dtype: datatype = None, out=None) -> DNDarray:
@@ -323,15 +323,15 @@
         Scalar values are expanded to arrays with length 1 in the direction of axis and
         the shape of the input array in along all other axes. Otherwise the dimension and
         shape must match a except along axis.
     """
     if n == 0:
         return a
     if n < 0:
-        raise ValueError("diff requires that n be a positive number, got {}".format(n))
+        raise ValueError(f"diff requires that n be a positive number, got {n}")
     if not isinstance(a, DNDarray):
         raise TypeError("'a' must be a DNDarray")
 
     axis = stride_tricks.sanitize_axis(a.gshape, axis)
 
     if prepend is not None or append is not None:
         pend_shape = a.gshape[:axis] + (1,) + a.gshape[axis + 1 :]
@@ -349,21 +349,19 @@
                         device=a.device,
                         comm=a.comm,
                     )
                 elif isinstance(p_el, DNDarray) and p_el.gshape == pend_shape:
                     pass
                 elif not isinstance(p_el, DNDarray):
                     raise TypeError(
-                        "prepend/append should be a scalar or a DNDarray, was {}".format(type(p_el))
+                        f"prepend/append should be a scalar or a DNDarray, was {type(p_el)}"
                     )
                 elif p_el.gshape != pend_shape:
                     raise ValueError(
-                        "shape mismatch: expected prepend/append to be {}, got {}".format(
-                            pend_shape, p_el.gshape
-                        )
+                        f"shape mismatch: expected prepend/append to be {pend_shape}, got {p_el.gshape}"
                     )
                 if p == 0:
                     # prepend
                     a = manipulations.concatenate((p_el, a), axis=axis)
                 else:
                     # append
                     a = manipulations.concatenate((a, p_el), axis=axis)
@@ -527,18 +525,15 @@
     DNDarray([[1., 2.],
               [1., 4.]], dtype=ht.float64, device=cpu:0, split=None)
     >>> T2 = ht.float32([1.5, 2.5])
     >>> ht.floordiv(T1, T2)
     DNDarray([[1., 0.],
               [1., 1.]], dtype=ht.float32, device=cpu:0, split=None)
     """
-    if int(torch.__version__.split(".")[1]) > 7:
-        return _operations.__binary_op(torch.div, t1, t2, fn_kwargs={"rounding_mode": "floor"})
-    else:
-        return _operations.__binary_op(torch.floor_divide, t1, t2)
+    return _operations.__binary_op(torch.div, t1, t2, fn_kwargs={"rounding_mode": "floor"})
 
 
 DNDarray.__floordiv__ = lambda self, other: floordiv(self, other)
 DNDarray.__floordiv__.__doc__ = floordiv.__doc__
 DNDarray.__rfloordiv__ = lambda self, other: floordiv(other, self)
 DNDarray.__rfloordiv__.__doc__ = floordiv.__doc__
 
@@ -746,15 +741,15 @@
     >>> +ht.array([-1., 1.])
     DNDarray([-1.,  1.], dtype=ht.float32, device=cpu:0, split=None)
     """
     sanitation.sanitize_in(a)
 
     def torch_pos(torch_tensor, out=None):
         if not torch.is_tensor(torch_tensor):
-            raise TypeError("Input is not a torch tensor but {}".format(type(torch_tensor)))
+            raise TypeError(f"Input is not a torch tensor but {type(torch_tensor)}")
         return out.copy_(torch_tensor)
 
     if out is not None:
         return _operations.__local_op(torch_pos, a, out, no_cast=True)
 
     return a.copy()
 
@@ -789,14 +784,45 @@
     DNDarray([[ 1.,  8.],
             [ 9., 16.]], dtype=ht.float32, device=cpu:0, split=None)
     >>> s = 3.0
     >>> ht.pow(T1, s)
     DNDarray([[ 1.,  8.],
             [27., 64.]], dtype=ht.float32, device=cpu:0, split=None)
     """
+    # early exit for integer scalars
+    if isinstance(t2, int):
+        try:
+            result = torch.pow(t1.larray, t2)
+            return DNDarray(
+                result,
+                gshape=t1.gshape,
+                dtype=t1.dtype,
+                device=t1.device,
+                split=t1.split,
+                comm=t1.comm,
+                balanced=t1.balanced,
+            )
+        except AttributeError:
+            # t1 is no DNDarray
+            pass
+    elif isinstance(t1, int):
+        try:
+            result = torch.pow(t1, t2.larray)
+            return DNDarray(
+                result,
+                gshape=t2.gshape,
+                dtype=t2.dtype,
+                device=t2.device,
+                split=t2.split,
+                comm=t2.comm,
+                balanced=t2.balanced,
+            )
+        except AttributeError:
+            # t2 is no DNDarray
+            pass
     return _operations.__binary_op(torch.pow, t1, t2)
 
 
 DNDarray.__pow__ = lambda self, other: pow(self, other)
 DNDarray.__pow__.__doc__ = pow.__doc__
 DNDarray.__rpow__ = lambda self, other: pow(other, self)
 DNDarray.__rpow__.__doc__ = pow.__doc__
@@ -867,15 +893,15 @@
 DNDarray.__rshift__.__doc__ = right_shift.__doc__
 
 
 def prod(
     a: DNDarray,
     axis: Union[int, Tuple[int, ...]] = None,
     out: DNDarray = None,
-    keepdim: bool = None,
+    keepdims: bool = None,
 ) -> DNDarray:
     """
     Return the product of array elements over a given axis in form of a DNDarray shaped as a but with the specified axis removed.
 
     Parameters
     ----------
     a : DNDarray
@@ -884,15 +910,15 @@
         Axis or axes along which a product is performed. The default, ``axis=None``, will calculate the product of all the
         elements in the input array. If axis is negative it counts from the last to the first axis.
         If axis is a tuple of ints, a product is performed on all of the axes specified in the tuple instead of a single
         axis or all the axes as before.
     out : DNDarray, optional
         Alternative output array in which to place the result. It must have the same shape as the expected output, but
         the datatype of the output values will be cast if necessary.
-    keepdim : bool, optional
+    keepdims : bool, optional
         If this is set to ``True``, the axes which are reduced are left in the result as dimensions with size one. With this
         option, the result will broadcast correctly against the input array.
 
     Examples
     --------
     >>> ht.prod(ht.array([1.,2.]))
     DNDarray([2.], dtype=ht.float32, device=cpu:0, split=None)
@@ -903,19 +929,19 @@
     >>> ht.prod(ht.array([
         [1.,2.],
         [3.,4.]
     ]), axis=1)
     DNDarray([ 2., 12.], dtype=ht.float32, device=cpu:0, split=None)
     """
     return _operations.__reduce_op(
-        a, torch.prod, MPI.PROD, axis=axis, out=out, neutral=1, keepdim=keepdim
+        a, torch.prod, MPI.PROD, axis=axis, out=out, neutral=1, keepdims=keepdims
     )
 
 
-DNDarray.prod = lambda self, axis=None, out=None, keepdim=None: prod(self, axis, out, keepdim)
+DNDarray.prod = lambda self, axis=None, out=None, keepdims=None: prod(self, axis, out, keepdims)
 DNDarray.prod.__doc__ = prod.__doc__
 
 
 def sub(t1: Union[DNDarray, float], t2: Union[DNDarray, float]) -> DNDarray:
     """
     Element-wise subtraction of values of operand ``t2`` from values of operands ``t1`` (i.e ``t1-t2``)
     Operation is not commutative.
@@ -957,15 +983,15 @@
 """
 
 
 def sum(
     a: DNDarray,
     axis: Union[int, Tuple[int, ...]] = None,
     out: DNDarray = None,
-    keepdim: bool = None,
+    keepdims: bool = None,
 ) -> DNDarray:
     """
     Sum of array elements over a given axis. An array with the same shape as ``self.__array`` except for the specified
     axis which becomes one, e.g. ``a.shape=(1, 2, 3)`` => ``ht.ones((1, 2, 3)).sum(axis=1).shape=(1, 1, 3)``
 
     Parameters
     ----------
@@ -974,15 +1000,15 @@
     axis : None or int or Tuple[int,...], optional
         Axis along which a sum is performed. The default, ``axis=None``, will sum all of the elements of the input array.
         If ``axis`` is negative it counts from the last to the first axis. If ``axis`` is a tuple of ints, a sum is performed
         on all of the axes specified in the tuple instead of a single axis or all the axes as before.
     out : DNDarray, optional
         Alternative output array in which to place the result. It must have the same shape as the expected output, but
         the datatype of the output values will be cast if necessary.
-    keepdim : bool, optional
+    keepdims : bool, optional
         If this is set to ``True``, the axes which are reduced are left in the result as dimensions with size one. With this
         option, the result will broadcast correctly against the input array.
 
     Examples
     --------
     >>> ht.sum(ht.ones(2))
     DNDarray([2.], dtype=ht.float32, device=cpu:0, split=None)
@@ -992,12 +1018,12 @@
     DNDarray([9], dtype=ht.int64, device=cpu:0, split=None)
     >>> ht.sum(ht.ones((3,2,1)), axis=-3)
     DNDarray([[3.],
               [3.]], dtype=ht.float32, device=cpu:0, split=None)
     """
     # TODO: make me more numpy API complete Issue #101
     return _operations.__reduce_op(
-        a, torch.sum, MPI.SUM, axis=axis, out=out, neutral=0, keepdim=keepdim
+        a, torch.sum, MPI.SUM, axis=axis, out=out, neutral=0, keepdims=keepdims
     )
 
 
-DNDarray.sum = lambda self, axis=None, out=None, keepdim=None: sum(self, axis, out, keepdim)
+DNDarray.sum = lambda self, axis=None, out=None, keepdims=None: sum(self, axis, out, keepdims)
```

### Comparing `heat-1.2.2/heat/core/base.py` & `heat-1.3.0/heat/core/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         Get parameters for this estimator.
 
         Parameters
         ----------
         deep : bool, default: True
             If ``True``, will return the parameters for this estimator and contained sub-objects that are estimators.
         """
-        params = dict()
+        params = {}
 
         for key in self._parameter_names():
             value = getattr(self, key)
 
             if deep and hasattr(value, "get_params"):
                 value = value.get_params()
 
@@ -78,17 +78,15 @@
         if not params:
             return self
 
         parameter_names = self._parameter_names()
         for key, value in params.items():
             if key not in parameter_names:
                 raise ValueError(
-                    "Invalid parameter {} for estimator {}. Check the list of available parameters with `estimator.get_params().keys()`.".format(
-                        key, self
-                    )
+                    f"Invalid parameter {key} for estimator {self}. Check the list of available parameters with `estimator.get_params().keys()`."
                 )
 
             if isinstance(value, dict):
                 getattr(self, key).set_params(value)
             else:
                 setattr(self, key, value)
```

### Comparing `heat-1.2.2/heat/core/communication.py` & `heat-1.3.0/heat/core/communication.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,20 @@
     def is_distributed(self) -> bool:
         """
         Determines whether the communicator is distributed, i.e. handles more than one node.
         """
         return self.size > 1
 
     def chunk(
-        self, shape: Tuple[int], split: int, rank: int = None, w_size: int = None
+        self,
+        shape: Tuple[int],
+        split: int,
+        rank: int = None,
+        w_size: int = None,
+        sparse: bool = False,
     ) -> Tuple[int, Tuple[int], Tuple[slice]]:
         """
         Calculates the chunk of data that will be assigned to this compute node given a global data shape and a split
         axis.
         Returns ``(offset, local_shape, slices)``: the offset in the split dimension, the resulting local shape if the
         global input shape is chunked on the split axis and the chunk slices with respect to the given shape
 
@@ -175,15 +180,16 @@
             The axis along which to chunk the data
         rank : int, optional
             Process for which the chunking is calculated for, defaults to ``self.rank``.
             Intended for creating chunk maps without communication
         w_size : int, optional
             The MPI world size, defaults to ``self.size``.
             Intended for creating chunk maps without communication
-
+        sparse : bool, optional
+            Specifies whether the array is a sparse matrix
         """
         # ensure the split axis is valid, we actually do not need it
         split = sanitize_axis(shape, split)
         if split is None:
             return 0, shape, tuple(slice(0, end) for end in shape)
         rank = self.rank if rank is None else rank
         w_size = self.size if w_size is None else w_size
@@ -198,14 +204,17 @@
         if remainder > rank:
             chunk += 1
             start = rank * chunk
         else:
             start = rank * chunk + remainder
         end = start + chunk
 
+        if sparse:
+            return start, end
+
         return (
             start,
             tuple(shape[i] if i != split else end - start for i in range(dims)),
             tuple(slice(0, shape[i]) if i != split else slice(start, end) for i in range(dims)),
         )
 
     def counts_displs_shape(
@@ -269,23 +278,22 @@
         if is_contiguous is None:
             # determine local contiguity
             is_contiguous = obj.is_contiguous()
 
         if is_contiguous:
             if counts is None:
                 return mpi_type, elements
-            else:
-                factor = np.prod(obj.shape[1:])
-                return (
-                    mpi_type,
-                    (
-                        tuple(factor * ele for ele in counts),
-                        (tuple(factor * ele for ele in displs)),
-                    ),
-                )
+            factor = np.prod(obj.shape[1:])
+            return (
+                mpi_type,
+                (
+                    tuple(factor * ele for ele in counts),
+                    (tuple(factor * ele for ele in displs)),
+                ),
+            )
 
         # non-contiguous memory, e.g. after a transpose, has to be packed in derived MPI types
         elements = obj.shape[0]
         shape = obj.shape[1:]
         strides = [1] * len(shape)
         strides[0] = obj.stride()[-1]
         strides = strides[::-1]
@@ -1042,33 +1050,27 @@
         send_counts, send_displs, recv_counts, recv_displs = None, None, None, None
 
         # unpack the send buffer
         if isinstance(sendbuf, tuple):
             sendbuf, send_counts, send_displs = sendbuf
         if isinstance(sendbuf, DNDarray):
             sendbuf = sendbuf.larray
-        if not isinstance(sendbuf, torch.Tensor):
-            if axis != 0:
-                raise TypeError(
-                    "sendbuf of type {} does not support concatenation axis != 0".format(
-                        type(sendbuf)
-                    )
-                )
+        if not isinstance(sendbuf, torch.Tensor) and axis != 0:
+            raise TypeError(
+                f"sendbuf of type {type(sendbuf)} does not support concatenation axis != 0"
+            )
         # unpack the receive buffer
         if isinstance(recvbuf, tuple):
             recvbuf, recv_counts, recv_displs = recvbuf
         if isinstance(recvbuf, DNDarray):
             recvbuf = recvbuf.larray
-        if not isinstance(recvbuf, torch.Tensor):
-            if axis != 0:
-                raise TypeError(
-                    "recvbuf of type {} does not support concatenation axis != 0".format(
-                        type(recvbuf)
-                    )
-                )
+        if not isinstance(recvbuf, torch.Tensor) and axis != 0:
+            raise TypeError(
+                f"recvbuf of type {type(recvbuf)} does not support concatenation axis != 0"
+            )
 
         # keep a reference to the original buffer object
         original_recvbuf = recvbuf
         sbuf_is_contiguous, rbuf_is_contiguous = None, None
         # permute the send_axis order so that the split send_axis is the first to be transmitted
         if axis != 0:
             send_axis_permutation = list(range(sendbuf.ndimension()))
@@ -1236,44 +1238,38 @@
                 - if ``send_axis==recv_axis``, an error will be thrown
                 - if ``send_axis`` or ``recv_axis`` are ``None``, an error will be thrown
         recv_axis: int
             Prior split axis, along which blocks are received from the individual ranks
         """
         if send_axis is None:
             raise NotImplementedError(
-                "AllToAll needs send_axis and recv_axis to be specified but was send_axis = {}, recv_axis = {}. Please set send_axis and recv_axis".format(
-                    send_axis, recv_axis
-                )
+                f"AllToAll needs send_axis and recv_axis to be specified but was send_axis = {send_axis}, recv_axis = {recv_axis}. Please set send_axis and recv_axis"
             )
         # align the output buffer in the same way as the input buffer by default
         if recv_axis is None:
             recv_axis = send_axis
 
         # dummy allocation for *v calls
         send_counts, send_displs, recv_counts, recv_displs = None, None, None, None
 
         # unpack the send buffer
         if isinstance(sendbuf, tuple):
             sendbuf, send_counts, send_displs = sendbuf
         if isinstance(sendbuf, DNDarray):
             sendbuf = sendbuf.larray
         if not isinstance(sendbuf, torch.Tensor) and send_axis != 0:
-            raise TypeError(
-                "sendbuf of type {} does not support send_axis != 0".format(type(sendbuf))
-            )
+            raise TypeError(f"sendbuf of type {type(sendbuf)} does not support send_axis != 0")
 
         # unpack the receive buffer
         if isinstance(recvbuf, tuple):
             recvbuf, recv_counts, recv_displs = recvbuf
         if isinstance(recvbuf, DNDarray):
             recvbuf = recvbuf.larray
         if not isinstance(recvbuf, torch.Tensor) and send_axis != 0:
-            raise TypeError(
-                "recvbuf of type {} does not support send_axis != 0".format(type(recvbuf))
-            )
+            raise TypeError(f"recvbuf of type {type(recvbuf)} does not support send_axis != 0")
 
         # keep a reference to the original buffer object
         original_recvbuf = recvbuf
 
         # Simple case, contiguous buffers can be transmitted as is
         if send_axis < 2 and recv_axis < 2:
             send_axis_permutation = list(range(recvbuf.ndimension()))
@@ -1529,27 +1525,23 @@
 
         # unpack the send buffer
         if isinstance(sendbuf, tuple):
             sendbuf, send_counts, send_displs = sendbuf
         if isinstance(sendbuf, DNDarray):
             sendbuf = sendbuf.larray
         if not isinstance(sendbuf, torch.Tensor) and send_axis != 0:
-            raise TypeError(
-                "sendbuf of type {} does not support send_axis != 0".format(type(sendbuf))
-            )
+            raise TypeError(f"sendbuf of type {type(sendbuf)} does not support send_axis != 0")
 
         # unpack the receive buffer
         if isinstance(recvbuf, tuple):
             recvbuf, recv_counts, recv_displs = recvbuf
         if isinstance(recvbuf, DNDarray):
             recvbuf = recvbuf.larray
         if not isinstance(recvbuf, torch.Tensor) and send_axis != 0:
-            raise TypeError(
-                "recvbuf of type {} does not support send_axis != 0".format(type(recvbuf))
-            )
+            raise TypeError(f"recvbuf of type {type(recvbuf)} does not support send_axis != 0")
 
         # keep a reference to the original buffer object
         original_recvbuf = recvbuf
 
         # permute the send_axis order so that the split send_axis is the first to be transmitted
         send_axis_permutation = list(range(recvbuf.ndimension()))
         send_axis_permutation[0], send_axis_permutation[send_axis] = send_axis, 0
@@ -1931,15 +1923,15 @@
         If the given communication is not the proper type
     """
     if comm is None:
         return get_comm()
     elif isinstance(comm, Communication):
         return comm
 
-    raise TypeError("Unknown communication, must be instance of {}".format(Communication))
+    raise TypeError(f"Unknown communication, must be instance of {Communication}")
 
 
 def use_comm(comm: Communication = None):
     """
     Sets the globally used default communicator.
 
     Parameters
```

### Comparing `heat-1.2.2/heat/core/complex_math.py` & `heat-1.3.0/heat/core/complex_math.py`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/core/constants.py` & `heat-1.3.0/heat/core/constants.py`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/core/devices.py` & `heat-1.3.0/heat/core/devices.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 handle different devices. Current options: CPU (default), GPU
 """
 
 from __future__ import annotations
 
 import torch
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
 from . import communication
 
 
 __all__ = ["Device", "cpu", "get_device", "sanitize_device", "use_device"]
 
 
@@ -62,21 +62,37 @@
         """
         return self.__torch_device
 
     def __repr__(self) -> str:
         """
         Return the unambiguous information of :class:`~heat.core.device.Device`.
         """
-        return "device({})".format(self.__str__())
+        return f"device({self.__str__()})"
 
     def __str__(self) -> str:
         """
         Return the descriptive information of :class:`~heat.core.device.Device`.
         """
-        return "{}:{}".format(self.device_type, self.device_id)
+        return f"{self.device_type}:{self.device_id}"
+
+    def __eq__(self, other: Any) -> bool:
+        """
+        Overloads the `==` operator for local equal check.
+
+        Parameters
+        ----------
+        other : Any
+            The object to compare with
+        """
+        if isinstance(other, Device):
+            return self.device_type == other.device_type and self.device_id == other.device_id
+        elif isinstance(other, torch.device):
+            return self.device_type == other.type and self.device_id == other.index
+        else:
+            return NotImplemented
 
 
 # create a CPU device singleton
 cpu = Device("cpu", 0, "cpu")
 """
 The standard CPU Device
 
@@ -95,15 +111,15 @@
 __device_mapping = {cpu.device_type: cpu}
 
 # add gpu support if available
 if torch.cuda.device_count() > 0:
     # GPUs are assigned round-robin to the MPI processes
     gpu_id = communication.MPI_WORLD.rank % torch.cuda.device_count()
     # create a new GPU device
-    gpu = Device("gpu", gpu_id, "cuda:{}".format(gpu_id))
+    gpu = Device("gpu", gpu_id, f"cuda:{gpu_id}")
     """
     The standard GPU Device
 
     Examples
     --------
     >>> ht.cpu
     device(cpu:0)
@@ -145,17 +161,15 @@
 
     if isinstance(device, Device):
         return device
 
     try:
         return __device_mapping[device.strip().lower()]
     except (AttributeError, KeyError, TypeError):
-        raise ValueError(
-            "Unknown device, must be one of {}".format(", ".join(__device_mapping.keys()))
-        )
+        raise ValueError(f'Unknown device, must be one of {", ".join(__device_mapping.keys())}')
 
 
 def use_device(device: Optional[Union[str, Device]] = None) -> None:
     """
     Sets the globally used default :class:`~heat.core.device.Device`.
 
     Parameters
```

### Comparing `heat-1.2.2/heat/core/dndarray.py` & `heat-1.3.0/heat/core/dndarray.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         self.__split = split
         self.__device = device
         self.__comm = comm
         self.__balanced = balanced
         self.__ishalo = False
         self.__halo_next = None
         self.__halo_prev = None
+        self.__partitions_dict__ = None
         self.__lshape_map = None
 
         # check for inconsistencies between torch and heat devices
         assert str(array.device) == device.torch_device
 
     @property
     def balanced(self) -> bool:
@@ -180,21 +181,43 @@
     def ndim(self) -> int:
         """
         Number of dimensions of the ``DNDarray``
         """
         return len(self.__gshape)
 
     @property
+    def __partitioned__(self) -> dict:
+        """
+        This will return a dictionary containing information useful for working with the partitioned
+        data. These items include the shape of the data on each process, the starting index of the data
+        that a process has, the datatype of the data, the local devices, as well as the global
+        partitioning scheme.
+
+        An example of the output and shape is shown in :func:`ht.core.DNDarray.create_partition_interface <ht.core.DNDarray.create_partition_interface>`.
+
+        Returns
+        -------
+        dictionary with the partition interface
+        """
+        if self.__partitions_dict__ is None:
+            self.__partitions_dict__ = self.create_partition_interface()
+        return self.__partitions_dict__
+
+    @property
     def size(self) -> int:
         """
         Number of total elements of the ``DNDarray``
         """
-        return torch.prod(
-            torch.tensor(self.gshape, dtype=torch.int, device=self.device.torch_device)
-        ).item()
+        return (
+            torch.prod(
+                torch.tensor(self.gshape, dtype=torch.float64, device=self.device.torch_device)
+            )
+            .long()
+            .item()
+        )
 
     @property
     def gnbytes(self) -> int:
         """
         Returns the number of bytes consumed by the global ``DNDarray``
 
         Note
@@ -364,19 +387,19 @@
         Parameters
         ----------
         halo_size : int
             Size of the halo.
         """
         if not isinstance(halo_size, int):
             raise TypeError(
-                "halo_size needs to be of Python type integer, {} given".format(type(halo_size))
+                f"halo_size needs to be of Python type integer, {type(halo_size)} given"
             )
         if halo_size < 0:
             raise ValueError(
-                "halo_size needs to be a positive Python integer, {} given".format(type(halo_size))
+                f"halo_size needs to be a positive Python integer, {type(halo_size)} given"
             )
 
         if self.is_distributed() and halo_size > 0:
             # gather lshapes
             lshape_map = self.lshape_map
             rank = self.comm.rank
 
@@ -391,25 +414,23 @@
             else:
                 # if process has no data we ignore it
                 return
 
             if (halo_size > self.lshape_map[:, self.split][populated_ranks]).any():
                 # halo_size is larger than the local size on at least one process
                 raise ValueError(
-                    "halo_size {} needs to be smaller than chunk-size {} )".format(
-                        halo_size, self.lshape[self.split]
-                    )
+                    f"halo_size {halo_size} needs to be smaller than chunk-size {self.lshape[self.split]} )"
                 )
 
             a_prev = self.__prephalo(0, halo_size)
             a_next = self.__prephalo(-halo_size, None)
             res_prev = None
             res_next = None
 
-            req_list = list()
+            req_list = []
 
             # exchange data with next populated process
             if rank != last_rank:
                 self.comm.Isend(a_next, next_rank)
                 res_prev = torch.zeros(
                     a_prev.size(), dtype=a_prev.dtype, device=self.device.torch_device
                 )
@@ -436,24 +457,30 @@
         if not self.is_distributed():
             return self.__array
         return torch.cat(
             [_ for _ in (self.__halo_prev, self.__array, self.__halo_next) if _ is not None],
             dim=self.split,
         )
 
+    def __array__(self) -> np.ndarray:
+        """
+        Returns a view of the process-local slice of the :class:`DNDarray` as a numpy ndarray, if the ``DNDarray`` resides on CPU. Otherwise, it returns a copy, on CPU, of the process-local slice of ``DNDarray`` as numpy ndarray.
+        """
+        return self.larray.cpu().__array__()
+
     def astype(self, dtype, copy=True) -> DNDarray:
         """
         Returns a casted version of this array.
         Casted array is a new array of the same shape but with given type of this array. If copy is ``True``, the
         same array is returned instead.
 
         Parameters
         ----------
         dtype : datatype
-            HeAT type to which the array is cast
+            Heat type to which the array is cast
         copy : bool, optional
             By default the operation returns a copy of this array. If copy is set to ``False`` the cast is performed
             in-place and this array is returned
 
         """
         dtype = canonical_heat_type(dtype)
         casted_array = self.__array.type(dtype.torch_type())
@@ -577,15 +604,15 @@
             if False (default) and the lshape map has already been created, use the previous
             result. Otherwise, create the lshape_map
         """
         if not force_check and self.__lshape_map is not None:
             return self.__lshape_map.clone()
 
         lshape_map = torch.zeros(
-            (self.comm.size, self.ndim), dtype=torch.int, device=self.device.torch_device
+            (self.comm.size, self.ndim), dtype=torch.int64, device=self.device.torch_device
         )
         if not self.is_distributed:
             lshape_map[:] = torch.tensor(self.gshape, device=self.device.torch_device)
             return lshape_map
         if self.is_balanced(force_check=True):
             for i in range(self.comm.size):
                 _, lshape, _ = self.comm.chunk(self.gshape, self.split, rank=i)
@@ -595,14 +622,112 @@
                 self.lshape, device=self.device.torch_device
             )
             self.comm.Allreduce(MPI.IN_PLACE, lshape_map, MPI.SUM)
 
         self.__lshape_map = lshape_map
         return lshape_map.clone()
 
+    def create_partition_interface(self):
+        """
+        Create a partition interface in line with the DPPY proposal. This is subject to change.
+        The intention of this to facilitate the usage of a general format for the referencing of
+        distributed datasets.
+
+        An example of the output and shape is shown below.
+
+        __partitioned__ = {
+            'shape': (27, 3, 2),
+            'partition_tiling': (4, 1, 1),
+            'partitions': {
+                (0, 0, 0): {
+                    'start': (0, 0, 0),
+                    'shape': (7, 3, 2),
+                    'data': tensor([...], dtype=torch.int32),
+                    'location': [0],
+                    'dtype': torch.int32,
+                    'device': 'cpu'
+                },
+                (1, 0, 0): {
+                    'start': (7, 0, 0),
+                    'shape': (7, 3, 2),
+                    'data': None,
+                    'location': [1],
+                    'dtype': torch.int32,
+                    'device': 'cpu'
+                },
+                (2, 0, 0): {
+                    'start': (14,  0,  0),
+                    'shape': (7, 3, 2),
+                    'data': None,
+                    'location': [2],
+                    'dtype': torch.int32,
+                    'device': 'cpu'
+                },
+                (3, 0, 0): {
+                    'start': (21,  0,  0),
+                    'shape': (6, 3, 2),
+                    'data': None,
+                    'location': [3],
+                    'dtype': torch.int32,
+                    'device': 'cpu'
+                }
+            },
+            'locals': [(rank, 0, 0)],
+            'get': lambda x: x,
+        }
+
+        Returns
+        -------
+        dictionary containing the partition interface as shown above.
+        """
+        lshape_map = self.create_lshape_map()
+        start_idx_map = torch.zeros_like(lshape_map)
+
+        part_tiling = [1] * self.ndim
+        lcls = [0] * self.ndim
+
+        z = torch.tensor([0], device=self.device.torch_device, dtype=self.dtype.torch_type())
+        if self.split is not None:
+            starts = torch.cat((z, torch.cumsum(lshape_map[:, self.split], dim=0)[:-1]), dim=0)
+            lcls[self.split] = self.comm.rank
+            part_tiling[self.split] = self.comm.size
+        else:
+            starts = torch.zeros(self.ndim, dtype=torch.int, device=self.device.torch_device)
+
+        start_idx_map[:, self.split] = starts
+
+        partitions = {}
+        base_key = [0] * self.ndim
+        for r in range(self.comm.size):
+            if self.split is not None:
+                base_key[self.split] = r
+                dat = None if r != self.comm.rank else self.larray
+            else:
+                dat = self.larray
+            partitions[tuple(base_key)] = {
+                "start": tuple(start_idx_map[r].tolist()),
+                "shape": tuple(lshape_map[r].tolist()),
+                "data": dat,
+                "location": [r],
+                "dtype": self.dtype.torch_type(),
+                "device": self.device.torch_device,
+            }
+
+        partition_dict = {
+            "shape": self.gshape,
+            "partition_tiling": tuple(part_tiling),
+            "partitions": partitions,
+            "locals": [tuple(lcls)],
+            "get": lambda x: x,
+        }
+
+        self.__partitions_dict__ = partition_dict
+
+        return partition_dict
+
     def __float__(self) -> DNDarray:
         """
         Float scalar casting.
 
         See Also
         ---------
         :func:`~heat.core.manipulations.flatten`
@@ -693,15 +818,15 @@
             if key.larray.dtype in [torch.bool, torch.uint8]:
                 key = indexing.nonzero(key)
 
             if key.ndim > 1:
                 key = list(key.larray.split(1, dim=1))
                 # key is now a list of tensors with dimensions (key.ndim, 1)
                 # squeeze singleton dimension:
-                key = list(key[i].squeeze_(1) for i in range(len(key)))
+                key = [key[i].squeeze_(1) for i in range(len(key))]
             else:
                 key = [key]
             advanced_ind = True
         elif not isinstance(key, tuple):
             """this loop handles all other cases. DNDarrays which make it to here refer to
             advanced indexing slices, as do the torch tensors. Both DNDaarrys and torch.Tensors
             are cast into lists here by PyTorch. lists mean advanced indexing will be used"""
@@ -805,30 +930,28 @@
             if isinstance(key[self.split], DNDarray):
                 lkey[self.split] = key[self.split].larray
 
             if not isinstance(lkey[self.split], torch.Tensor):
                 inds = torch.tensor(
                     lkey[self.split], dtype=torch.long, device=self.device.torch_device
                 )
+            elif lkey[self.split].dtype in [torch.bool, torch.uint8]:  # or torch.byte?
+                # need to convert the bools to indices
+                inds = torch.nonzero(lkey[self.split])
             else:
-                if lkey[self.split].dtype in [torch.bool, torch.uint8]:  # or torch.byte?
-                    # need to convert the bools to indices
-                    inds = torch.nonzero(lkey[self.split])
-                else:
-                    inds = lkey[self.split]
+                inds = lkey[self.split]
             # todo: remove where in favor of nonzero? might be a speed upgrade. testing required
             loc_inds = torch.where((inds >= chunk_start) & (inds < chunk_end))
             # if there are no local indices on a process, then `arr` is empty
             # if local indices exist:
             if len(loc_inds[0]) != 0:
                 # select same local indices for other (non-split) dimensions if necessary
                 for i, k in enumerate(lkey):
-                    if isinstance(k, (list, torch.Tensor, DNDarray)):
-                        if i != self.split:
-                            lkey[i] = k[loc_inds]
+                    if isinstance(k, (list, torch.Tensor, DNDarray)) and i != self.split:
+                        lkey[i] = k[loc_inds]
                 # correct local indices for offset
                 inds = inds[loc_inds] - chunk_start
                 lkey[self.split] = inds
                 lout[new_split] = len(inds)
                 arr = self.__array[tuple(lkey)].reshape(tuple(lout))
             elif len(loc_inds[0]) == 0:
                 if new_split is not None:
@@ -976,26 +1099,31 @@
         Examples
         -------
         >>> import heat as ht
         >>> x = ht.zeros((1))
         >>> x.item()
         0.0
         """
+        if self.size > 1:
+            raise ValueError("only one-element DNDarrays can be converted to Python scalars")
+        # make sure the element is on every process
+        self.resplit_(None)
         return self.__array.item()
 
     def __len__(self) -> int:
         """
         The length of the ``DNDarray``, i.e. the number of items in the first dimension.
         """
         return self.shape[0]
 
     def numpy(self) -> np.array:
         """
-        Convert :class:`DNDarray` to numpy array. If the ``DNDarray`` is distributed it will be merged beforehand. If the ``DNDarray``
-        resides on the GPU, it will be copied to the CPU first.
+        Returns a copy of the :class:`DNDarray` as numpy ndarray. If the ``DNDarray`` resides on the GPU, the underlying data will be copied to the CPU first.
+
+        If the ``DNDarray`` is distributed, an MPI Allgather operation will be performed before converting to np.ndarray, i.e. each MPI process will end up holding a copy of the entire array in memory.  Make sure process memory is sufficient!
 
         Examples
         --------
         >>> import heat as ht
         T1 = ht.random.randn((10,8))
         T1.numpy()
         """
@@ -1044,15 +1172,15 @@
             Units are ``[rank, target lshape]``.
             Note: the only important parts of the target map are the values along the split axis,
             values which are not along this axis are there to mimic the shape of the ``lshape_map``.
 
         Examples
         --------
         >>> st = ht.ones((50, 81, 67), split=2)
-        >>> target_map = torch.zeros((st.comm.size, 3), dtype=torch.int)
+        >>> target_map = torch.zeros((st.comm.size, 3), dtype=torch.int64)
         >>> target_map[0, 2] = 67
         >>> print(target_map)
         [0/2] tensor([[ 0,  0, 67],
         [0/2]         [ 0,  0,  0],
         [0/2]         [ 0,  0,  0]], dtype=torch.int32)
         [1/2] tensor([[ 0,  0, 67],
         [1/2]         [ 0,  0,  0],
@@ -1075,44 +1203,37 @@
         snd_dtype = self.dtype.torch_type()
         # units -> {pr, 1st index, 2nd index}
         if lshape_map is None:
             # NOTE: giving an lshape map which is incorrect will result in an incorrect distribution
             lshape_map = self.create_lshape_map(force_check=True)
         else:
             if not isinstance(lshape_map, torch.Tensor):
-                raise TypeError(
-                    "lshape_map must be a torch.Tensor, currently {}".format(type(lshape_map))
-                )
+                raise TypeError(f"lshape_map must be a torch.Tensor, currently {type(lshape_map)}")
             if lshape_map.shape != (self.comm.size, len(self.gshape)):
                 raise ValueError(
-                    "lshape_map must have the shape ({}, {}), currently {}".format(
-                        self.comm.size, len(self.gshape), lshape_map.shape
-                    )
+                    f"lshape_map must have the shape ({self.comm.size}, {len(self.gshape)}), currently {lshape_map.shape}"
                 )
         if target_map is None:  # if no target map is given then it will balance the tensor
             _, _, chk = self.comm.chunk(self.shape, self.split)
             target_map = lshape_map.clone()
             target_map[..., self.split] = 0
             for pr in range(self.comm.size):
                 target_map[pr, self.split] = self.comm.chunk(self.shape, self.split, rank=pr)[1][
                     self.split
                 ]
             self.__balanced = True
         else:
             sanitation.sanitize_in_tensor(target_map)
             if target_map[..., self.split].sum() != self.shape[self.split]:
                 raise ValueError(
-                    "Sum along the split axis of the target map must be equal to the "
-                    "shape in that dimension, currently {}".format(target_map[..., self.split])
+                    f"Sum along the split axis of the target map must be equal to the shape in that dimension, currently {target_map[..., self.split]}"
                 )
             if target_map.shape != (self.comm.size, len(self.gshape)):
                 raise ValueError(
-                    "target_map must have the shape {}, currently {}".format(
-                        (self.comm.size, len(self.gshape)), target_map.shape
-                    )
+                    f"target_map must have the shape {(self.comm.size, len(self.gshape))}, currently {target_map.shape}"
                 )
             # no info on balanced status
             self.__balanced = False
         lshape_cumsum = torch.cumsum(lshape_map[..., self.split], dim=0)
         chunk_cumsum = torch.cat(
             (
                 torch.tensor([0], device=self.device.torch_device),
@@ -1266,17 +1387,21 @@
         """
         # sanitize the axis to check whether it is in range
         axis = sanitize_axis(self.shape, axis)
 
         # early out for unchanged content
         if self.comm.size == 1:
             self.__split = axis
+            if axis is None:
+                self.__partitions_dict__ = None
         if axis == self.split:
             return self
 
+        self.__partitions_dict__ = None
+
         if axis is None:
             gathered = torch.empty(
                 self.shape, dtype=self.dtype.torch_type(), device=self.device.torch_device
             )
             counts, displs = self.counts_displs()
             self.comm.Allgatherv(self.__array, (gathered, counts, displs), recv_axis=self.split)
             self.__array = gathered
@@ -1310,15 +1435,15 @@
             for i in range(new_locs.shape[0]):
                 key = tuple(new_locs[i].tolist())
                 spr = tiles.tile_locations[key].item()
                 to_send = tiles[key]
                 if spr == rank and spr != rpr:
                     self.comm.Send(to_send.clone(), dest=rpr, tag=rank)
                     del to_send
-                elif spr == rpr and rpr == rank:
+                elif spr == rpr == rank:
                     rcv[key] = [None, to_send]
                 elif rank == rpr:
                     sz = tiles.get_tile_size(key)
                     buf = torch.zeros(
                         sz, dtype=self.dtype.torch_type(), device=self.device.torch_device
                     )
                     w = self.comm.Irecv(buf=buf, source=spr, tag=spr)
@@ -1420,15 +1545,15 @@
             if key.larray.dtype in [torch.bool, torch.uint8]:
                 key = indexing.nonzero(key)
 
             if key.ndim > 1:
                 key = list(key.larray.split(1, dim=1))
                 # key is now a list of tensors with dimensions (key.ndim, 1)
                 # squeeze singleton dimension:
-                key = list(key[i].squeeze_(1) for i in range(len(key)))
+                key = [key[i].squeeze_(1) for i in range(len(key))]
             else:
                 key = [key]
         elif not isinstance(key, tuple):
             """this loop handles all other cases. DNDarrays which make it to here refer to
             advanced indexing slices, as do the torch tensors. Both DNDaarrys and torch.Tensors
             are cast into lists here by PyTorch. lists mean advanced indexing will be used"""
             h = [slice(None, None, None)] * self.ndim
@@ -1480,15 +1605,15 @@
             slices = [slice(None)] * (self.ndim - (len(kst) + len(kend)))
             key = kst + slices + kend
         # ---------- end ellipsis stuff -------------
 
         for c, k in enumerate(key):
             try:
                 key[c] = k.item()
-            except (AttributeError, ValueError):
+            except (AttributeError, ValueError, RuntimeError):
                 pass
 
         rank = self.comm.rank
         if self.split is not None:
             counts, chunk_starts = self.counts_displs()
         else:
             counts, chunk_starts = 0, [0] * self.comm.size
@@ -1560,15 +1685,15 @@
                 and value.shape[self.split] != self.shape[self.split]
             ):
                 # setting elements in self with a DNDarray which is not the same size in the
                 # split dimension
                 local_keys = []
                 # below is used if the target needs to be reshaped
                 target_reshape_map = torch.zeros(
-                    (self.comm.size, self.ndim), dtype=torch.int, device=self.device.torch_device
+                    (self.comm.size, self.ndim), dtype=torch.int64, device=self.device.torch_device
                 )
                 for r in range(self.comm.size):
                     if r not in actives:
                         loc_key = key.copy()
                         loc_key[self.split] = slice(0, 0, 0)
                     else:
                         key_start_l = 0 if r != actives[0] else key_start - chunk_starts[r]
@@ -1592,18 +1717,17 @@
                     return  # non-active ranks can exit here
 
                 chunk_starts_v = target_reshape_map[:, self.split]
                 value_slice = [slice(None, None, None)] * value.ndim
                 step2 = key_step if key_step is not None else 1
                 key_start = (chunk_starts_v[rank] - og_key_start).item()
 
-                if key_start < 0:
-                    key_start = 0
+                key_start = max(key_start, 0)
                 key_stop = key_start + key_stop
-                slice_loc = value.ndim - 1 if self.split > value.ndim - 1 else self.split
+                slice_loc = min(self.split, value.ndim - 1)
                 value_slice[slice_loc] = slice(
                     key_start, math.ceil(torch.true_divide(key_stop, step2)), 1
                 )
 
                 self.__setter(tuple(key), value.larray)
                 return
 
@@ -1619,18 +1743,17 @@
 
             # todo: need to slice the values to be the right size...
             if isinstance(value, (torch.Tensor, type(self))):
                 # if its a torch tensor, it is assumed to exist on all processes
                 value_slice = [slice(None, None, None)] * value.ndim
                 step2 = key_step if key_step is not None else 1
                 key_start = (chunk_starts[rank] - og_key_start).item()
-                if key_start < 0:
-                    key_start = 0
+                key_start = max(key_start, 0)
                 key_stop = key_start + key_stop
-                slice_loc = value.ndim - 1 if self.split > value.ndim - 1 else self.split
+                slice_loc = min(self.split, value.ndim - 1)
                 value_slice[slice_loc] = slice(
                     key_start, math.ceil(torch.true_divide(key_stop, step2)), 1
                 )
                 self.__setter(tuple(key), value[tuple(value_slice)])
             else:
                 self.__setter(tuple(key), value)
         elif isinstance(key[self.split], (torch.Tensor, list)):
@@ -1672,15 +1795,15 @@
         elif isinstance(value, (list, tuple)):
             value = torch.tensor(value, device=self.device.torch_device)
             self.__array.__setitem__(key, value.data)
         elif isinstance(value, np.ndarray):
             value = torch.from_numpy(value)
             self.__array.__setitem__(key, value.data)
         else:
-            raise NotImplementedError("Not implemented for {}".format(value.__class__.__name__))
+            raise NotImplementedError(f"Not implemented for {value.__class__.__name__}")
 
     def __str__(self) -> str:
         """
         Computes a string representation of the passed ``DNDarray``.
         """
         return printing.__str__(self)
```

### Comparing `heat-1.2.2/heat/core/exponential.py` & `heat-1.3.0/heat/core/exponential.py`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/core/factories.py` & `heat-1.3.0/heat/core/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 from .sanitation import sanitize_in, sanitize_sequence
 from .stride_tricks import sanitize_axis, sanitize_shape
 from .types import datatype
 
 from . import devices
 from . import types
 
-
 __all__ = [
     "arange",
     "array",
     "asarray",
     "empty",
     "empty_like",
     "eye",
+    "from_partitioned",
+    "from_partition_dict",
     "full",
     "full_like",
     "linspace",
     "logspace",
     "meshgrid",
     "ones",
     "ones_like",
@@ -38,15 +39,15 @@
 
 
 def arange(
     *args: Union[int, float],
     dtype: Optional[Type[datatype]] = None,
     split: Optional[int] = None,
     device: Optional[Union[str, Device]] = None,
-    comm: Optional[Communication] = None
+    comm: Optional[Communication] = None,
 ) -> DNDarray:
     """
     Return evenly spaced values within a given interval.
 
     Values are generated within the half-open interval ``[start, stop)`` (in other words, the interval including `start`
     but excluding `stop`). For integer arguments the function is equivalent to the Python built-in `range
     <http://docs.python.org/lib/built-in-funcs.html>`_ function, but returns a array rather than a list.
@@ -118,17 +119,15 @@
             dtype = types.int32 if all_ints else types.float32
         start = args[0]
         stop = args[1]
         step = args[2]
         num = int(np.ceil((stop - start) / step))
     else:
         raise TypeError(
-            "function takes minimum one and at most 3 positional arguments ({} given)".format(
-                num_of_param
-            )
+            f"function takes minimum one and at most 3 positional arguments ({num_of_param} given)"
         )
 
     # sanitize device and comm
     device = devices.sanitize_device(device)
     comm = sanitize_comm(comm)
 
     gshape = (num,)
@@ -146,15 +145,15 @@
 
     return DNDarray(data, gshape, htype, split, device, comm, balanced)
 
 
 def array(
     obj: Iterable,
     dtype: Optional[Type[datatype]] = None,
-    copy: bool = True,
+    copy: Optional[bool] = None,
     ndmin: int = 0,
     order: str = "C",
     split: Optional[int] = None,
     is_split: Optional[int] = None,
     device: Optional[Device] = None,
     comm: Optional[Communication] = None,
 ) -> DNDarray:
@@ -167,16 +166,17 @@
         A tensor or array, any object exposing the array interface, an object whose ``__array__`` method returns an
         array, or any (nested) sequence.
     dtype : datatype, optional
         The desired data-type for the array. If not given, then the type will be determined as the minimum type required
         to hold the objects in the sequence. This argument can only be used to ‘upcast’ the array. For downcasting, use
         the :func:`~heat.core.dndarray.astype` method.
     copy : bool, optional
-        If ``True`` (default), then the object is copied. Otherwise, a copy will only be made if obj is a nested
-        sequence or if a copy is needed to satisfy any of the other requirements, e.g. ``dtype``.
+        If ``True``, the input object is copied.
+        If ``False``, input which supports the buffer protocol is never copied.
+        If ``None`` (default), the function reuses the existing memory buffer if possible, and copies otherwise.
     ndmin : int, optional
         Specifies the minimum number of dimensions that the resulting array should have. Ones will, if needed, be
         attached to the shape if ``ndim > 0`` and prefaced in case of ``ndim < 0`` to meet the requirement.
     order: str, optional
         Options: ``'C'`` or ``'F'``. Specifies the memory layout of the newly created array. Default is ``order='C'``,
         meaning the array will be stored in row-major order (C-like). If ``order=‘F’``, the array will be stored in
         column-major order (Fortran-like).
@@ -193,14 +193,18 @@
     comm : Communication, optional
         Handle to the nodes holding distributed array chunks.
 
     Raises
     ------
     NotImplementedError
         If order is one of the NumPy options ``'K'`` or ``'A'``.
+    ValueError
+        If ``copy`` is False but a copy is necessary to satisfy other requirements (e.g. different dtype, device, etc.).
+    TypeError
+        If the input object cannot be converted to a torch.Tensor, hence it cannot be converted to a :class:`~heat.core.dndarray.DNDarray`.
 
     Examples
     --------
     >>> ht.array([1, 2, 3])
     DNDarray([1, 2, 3], dtype=ht.int64, device=cpu:0, split=None)
     >>> ht.array([1, 2, 3.0])
     DNDarray([1., 2., 3.], dtype=ht.float32, device=cpu:0, split=None)
@@ -280,26 +284,24 @@
           7
           10
           8
           11
          [torch.LongStorage of size 6]
     """
     # array already exists; no copy
-    if (
-        isinstance(obj, DNDarray)
-        and not copy
-        and (dtype is None or dtype == obj.dtype)
-        and (split is None or split == obj.split)
-        and (is_split is None or is_split == obj.split)
-        and (device is None or device == obj.device)
-    ):
-        return obj
-
-    # extract the internal tensor in case of a heat tensor
     if isinstance(obj, DNDarray):
+        if not copy:
+            if (
+                (dtype is None or dtype == obj.dtype)
+                and (split is None or split == obj.split)
+                and (is_split is None or is_split == obj.split)
+                and (device is None or device == obj.device)
+            ):
+                return obj
+        # extract the internal tensor
         obj = obj.larray
 
     # sanitize the data type
     if dtype is not None:
         dtype = types.canonical_heat_type(dtype)
 
     # sanitize device
@@ -319,21 +321,36 @@
                     device=device.torch_device
                     if device is not None
                     else devices.get_device().torch_device,
                 )
             except RuntimeError:
                 raise TypeError("invalid data of type {}".format(type(obj)))
     else:
-        if not isinstance(obj, DNDarray):
+        if copy is False and not np.isscalar(obj) and not isinstance(obj, (Tuple, List)):
+            # Python array-API compliance, cf. https://data-apis.org/array-api/2022.12/API_specification/generated/array_api.asarray.html
+            if not (
+                (dtype is None or dtype == types.canonical_heat_type(obj.dtype))
+                and (
+                    device is None
+                    or device.torch_device
+                    == str(getattr(obj, "device", devices.get_device().torch_device))
+                )
+            ):
+                raise ValueError(
+                    "argument `copy` is set to False, but copy of input object is necessary. \n Set copy=None to reuse the memory buffer whenever possible and allow for copies otherwise."
+                )
+        try:
             obj = torch.as_tensor(
                 obj,
                 device=device.torch_device
                 if device is not None
                 else devices.get_device().torch_device,
             )
+        except RuntimeError:
+            raise TypeError("invalid data of type {}".format(type(obj)))
 
     # infer dtype from obj if not explicitly given
     if dtype is None:
         dtype = types.canonical_heat_type(obj.dtype)
     else:
         torch_dtype = dtype.torch_type()
         if obj.dtype != torch_dtype:
@@ -341,21 +358,22 @@
 
     # infer device from obj if not explicitly given
     if device is None:
         device = devices.sanitize_device(obj.device.type)
 
     if str(obj.device) != device.torch_device:
         warnings.warn(
-            "Array 'obj' is not on device '{}'. It will be moved to it.".format(device), UserWarning
+            f"Array 'obj' is not on device '{device}'. It will be moved to it.",
+            UserWarning,
         )
         obj = obj.to(device.torch_device)
 
     # sanitize minimum number of dimensions
     if not isinstance(ndmin, int):
-        raise TypeError("expected ndmin to be int, but was {}".format(type(ndmin)))
+        raise TypeError(f"expected ndmin to be int, but was {type(ndmin)}")
 
     # reshape the object to encompass additional dimensions
     ndmin_abs = abs(ndmin) - len(obj.shape)
     if ndmin_abs > 0 and ndmin > 0:
         obj = obj.reshape(obj.shape + ndmin_abs * (1,))
     if ndmin_abs > 0 > ndmin:
         obj = obj.reshape(ndmin_abs * (1,) + obj.shape)
@@ -371,18 +389,26 @@
 
     # determine the local and the global shape. If split is None, they are identical
     gshape = list(obj.shape)
     lshape = gshape.copy()
     balanced = True
 
     # content shall be split, chunk the passed data object up
-    if split is not None:
-        _, _, slices = comm.chunk(gshape, split)
-        obj = obj[slices].clone()
+    if comm.size == 1 or split is None and is_split is None:
         obj = sanitize_memory_layout(obj, order=order)
+        split = is_split if is_split is not None else split
+
+    elif split is not None:
+        # only keep local slice
+        _, _, slices = comm.chunk(gshape, split)
+        _ = obj[slices].clone()
+        del obj
+
+        obj = sanitize_memory_layout(_, order=order)
+
     # check with the neighboring rank whether the local shape would fit into a global shape
     elif is_split is not None:
         obj = sanitize_memory_layout(obj, order=order)
 
         # Check whether the shape of distributed data
         # matches in all dimensions except the split axis
         neighbour_shape = np.array(gshape)
@@ -391,59 +417,55 @@
         if comm.rank < comm.size - 1:
             comm.Isend(lshape, dest=comm.rank + 1)
         if comm.rank != 0:
             # look into the message of the neighbor to see whether the shape length fits
             status = MPI.Status()
             comm.Probe(source=comm.rank - 1, status=status)
             length = status.Get_count() // lshape.dtype.itemsize
+            del status
             # the number of shape elements does not match with the 'left' rank
             if length != len(lshape):
                 discard_buffer = np.empty(length)
                 comm.Recv(discard_buffer, source=comm.rank - 1)
-                neighbour_shape[is_split] = np.iinfo(neighbour_shape.dtype).min
+                lshape[is_split] = np.iinfo(lshape.dtype).min
             else:
                 # check whether the individual shape elements match
                 comm.Recv(neighbour_shape, source=comm.rank - 1)
                 for i in range(length):
-                    if i == is_split:
-                        continue
-                    elif lshape[i] != neighbour_shape[i]:
-                        neighbour_shape[is_split] = np.iinfo(neighbour_shape.dtype).min
+                    if i != is_split:
+                        if lshape[i] != neighbour_shape[i]:
+                            lshape[is_split] = np.iinfo(lshape.dtype).min
+            del neighbour_shape
 
         # sum up the elements along the split dimension
-        reduction_buffer = np.array(neighbour_shape[is_split])
+        reduction_buffer = np.array(lshape[is_split])
         comm.Allreduce(MPI.IN_PLACE, reduction_buffer, MPI.MIN)
         if reduction_buffer < 0:
             raise ValueError(
                 "Unable to construct DNDarray. Local data slices have inconsistent shapes or dimensions."
             )
-        ttl_shape = np.array(obj.shape)
-        ttl_shape[is_split] = lshape[is_split]
-        comm.Allreduce(MPI.IN_PLACE, ttl_shape, MPI.SUM)
-        gshape[is_split] = ttl_shape[is_split]
+
+        total_split_shape = np.array(lshape[is_split])
+        comm.Allreduce(MPI.IN_PLACE, total_split_shape, MPI.SUM)
+        gshape[is_split] = total_split_shape.item()
         split = is_split
         # compare to calculated balanced lshape (cf. dndarray.is_balanced())
-        gshape = tuple(int(ele) for ele in gshape)
-        lshape = tuple(int(ele) for ele in lshape)
-        _, _, chk = comm.chunk(gshape, split)
-        test_lshape = tuple([x.stop - x.start for x in chk])
-        match = 1 if test_lshape == lshape else 0
+        _, test_lshape, _ = comm.chunk(gshape, split)
+        match = (test_lshape == lshape).all().astype(int)
         gmatch = comm.allreduce(match, MPI.SUM)
         if gmatch != comm.size:
             balanced = False
 
-    elif split is None and is_split is None:
-        obj = sanitize_memory_layout(obj, order=order)
-
     return DNDarray(obj, tuple(gshape), dtype, split, device, comm, balanced)
 
 
 def asarray(
     obj: Iterable,
     dtype: Optional[Type[datatype]] = None,
+    copy: Optional[bool] = None,
     order: str = "C",
     is_split: Optional[bool] = None,
     device: Optional[Union[str, Device]] = None,
 ) -> DNDarray:
     """
     Convert ``obj`` to a DNDarray. If ``obj`` is a `DNDarray` or `Tensor` with the same `dtype` and `device` or if the
     data is an `ndarray` of the corresponding ``dtype`` and the ``device`` is the CPU, no copy will be performed.
@@ -451,18 +473,22 @@
     Parameters
     ----------
     obj : iterable
         Input data, in any form that can be converted to an array. This includes e.g. lists, lists of tuples, tuples,
         tuples of tuples, tuples of lists and ndarrays.
     dtype : dtype, optional
         By default, the data-type is inferred from the input data.
+    copy : bool, optional
+        If ``True``, then the object is copied.  If ``False``, the object is not copied and a ``ValueError`` is
+        raised in the case a copy would be necessary. If ``None``, a copy will only be made if `obj` is a nested
+        sequence or if a copy is needed to satisfy any of the other requirements, e.g. ``dtype``.
     order: str, optional
         Whether to use row-major (C-style) or column-major (Fortran-style) memory representation. Defaults to ‘C’.
     is_split : None or int, optional
-        Specifies the axis along which the local data portions, passed in obj, are split across all machines. Useful for
+        Specifies the axis along which the local data portions, passed in obj, are split across all MPI processes. Useful for
         interfacing with other HPC code. The shape of the global tensor is automatically inferred.
     device : str, ht.Device or None, optional
         Specifies the device the tensor shall be allocated on. By default, it is inferred from the input data.
 
     Examples
     --------
     >>> a = [1,2]
@@ -484,15 +510,15 @@
     DNDarray([0, 2, 3], dtype=ht.int64, device=cpu:0, split=None)
     >>> a = ht.array([1,2,3,4], dtype=ht.float32)
     >>> ht.asarray(a, dtype=ht.float32) is a
     True
     >>> ht.asarray(a, dtype=ht.float64) is a
     False
     """
-    return array(obj, dtype=dtype, copy=False, order=order, is_split=is_split, device=device)
+    return array(obj, dtype=dtype, copy=copy, order=order, is_split=is_split, device=device)
 
 
 def empty(
     shape: Union[int, Sequence[int]],
     dtype: Type[datatype] = types.float32,
     split: Optional[int] = None,
     device: Optional[Device] = None,
@@ -726,15 +752,15 @@
     a: DNDarray,
     dtype: Type[datatype],
     split: Optional[int],
     factory: Callable,
     device: Device,
     comm: Communication,
     order: str = "C",
-    **kwargs
+    **kwargs,
 ) -> DNDarray:
     """
     Abstracted '...-like' factory function for HeAT :class:`~heat.core.dndarray.DNDarray` initialization
 
     Parameters
     ----------
     a : DNDarray
@@ -777,25 +803,175 @@
             dtype = types.heat_type_of(a)
         except TypeError:
             dtype = types.float32
 
     # infer split axis
     if split is None:
         try:
-            split = a.split if not isinstance(a, str) else None
+            split = None if isinstance(a, str) else a.split
         except AttributeError:
             # do not split at all
             pass
 
     # use the default communicator, if not set
     comm = sanitize_comm(comm)
 
     return factory(shape, dtype=dtype, split=split, device=device, comm=comm, order=order, **kwargs)
 
 
+def from_partitioned(x, comm: Optional[Communication] = None) -> DNDarray:
+    """
+    Return a newly created DNDarray constructed from the '__partitioned__' attributed of the input object.
+    Memory of local partitions will be shared (zero-copy) as long as supported by data objects.
+    Currently supports numpy ndarrays and torch tensors as data objects.
+    Current limitations:
+      * Partitions must be ordered in the partition-grid by rank
+      * Only one split-axis
+      * Only one partition per rank
+      * Only SPMD-style __partitioned__
+
+    Parameters
+    ----------
+    x : object
+        Requires x.__partitioned__
+    comm: Communication, optional
+        Handle to the nodes holding distributed parts or copies of this array.
+
+    See also
+    --------
+    :func:`ht.core.DNDarray.create_partition_interface <ht.core.DNDarray.create_partition_interface>`.
+
+    Raises
+    ------
+    AttributeError
+        If not hasattr(x, "__partitioned__") or if underlying data has no dtype.
+    TypeError
+        If it finds an unsupported array types
+    RuntimeError
+        If other unsupported content is found.
+
+    Examples
+    --------
+    >>> import heat as ht
+    >>> a = ht.ones((44,55), split=0)
+    >>> b = ht.from_partitioned(a)
+    >>> assert (a==b).all()
+    >>> a[40] = 4711
+    >>> assert (a==b).all()
+    """
+    comm = sanitize_comm(comm)
+    parted = x.__partitioned__
+    return __from_partition_dict_helper(parted, comm)
+
+
+def from_partition_dict(parted: dict, comm: Optional[Communication] = None) -> DNDarray:
+    """
+    Return a newly created DNDarray constructed from the '__partitioned__' attributed of the input object.
+    Memory of local partitions will be shared (zero-copy) as long as supported by data objects.
+    Currently supports numpy ndarrays and torch tensors as data objects.
+    Current limitations:
+      * Partitions must be ordered in the partition-grid by rank
+      * Only one split-axis
+      * Only one partition per rank
+      * Only SPMD-style __partitioned__
+
+    Parameters
+    ----------
+    parted : dict
+        A partition dictionary used to create the new DNDarray
+    comm: Communication, optional
+        Handle to the nodes holding distributed parts or copies of this array.
+
+    See also
+    --------
+    :func:`ht.core.DNDarray.create_partition_interface <ht.core.DNDarray.create_partition_interface>`.
+
+    Raises
+    ------
+    AttributeError
+        If not hasattr(x, "__partitioned__") or if underlying data has no dtype.
+    TypeError
+        If it finds an unsupported array types
+    RuntimeError
+        If other unsupported content is found.
+
+    Examples
+    --------
+    >>> import heat as ht
+    >>> a = ht.ones((44,55), split=0)
+    >>> b = ht.from_partition_dict(a.__partitioned__)
+    >>> assert (a==b).all()
+    >>> a[40] = 4711
+    >>> assert (a==b).all()
+    """
+    comm = sanitize_comm(comm)
+    return __from_partition_dict_helper(parted, comm)
+
+
+def __from_partition_dict_helper(parted: dict, comm: Communication):
+    # helper to create a DNDarray from a partition table (dictionary)
+    # the dictionary must be in the same form as the DNDarray.__partitioned__ property creates
+    if "locals" not in parted:
+        raise RuntimeError("Non-SPMD __partitioned__ not supported")
+    try:
+        gshape = parted["shape"]
+    except KeyError:
+        raise RuntimeError(
+            "partition dictionary must have a 'shape' entry, see DNDarray.create_partition_interface for more details"
+        )
+    try:
+        lparts = parted["locals"]
+    except KeyError:
+        raise RuntimeError(
+            "partition dictionary must have a 'local' entry, see DNDarray.create_partition_interface for more details"
+        )
+    if len(lparts) != 1:
+        raise RuntimeError("Only exactly one partition per rank supported (yet)")
+    parts = parted["partitions"]
+    lpart = parted["get"](parts[lparts[0]]["data"])
+    if isinstance(lpart, np.ndarray):
+        data = torch.from_numpy(lpart)
+    elif isinstance(lpart, torch.Tensor):
+        data = lpart
+    else:
+        raise TypeError(f"Only numpy arrays and torch tensors supported (not {type(lpart)}")
+    htype = types.canonical_heat_type(data.dtype)
+
+    # get split axis
+    gshape_list = list(gshape)
+    lshape_list = list(data.shape)
+    shape_diff = torch.tensor(
+        [g - l for g, l in zip(gshape_list, lshape_list)]
+    )  # dont care about device
+    nz = torch.nonzero(shape_diff)
+
+    if nz.numel() > 1:
+        raise RuntimeError("only one split axis allowed, check the ")
+    elif nz.numel() == 1:
+        split = nz[0].item()
+    else:
+        split = None
+
+    expected = {
+        int(x["location"][0]): (
+            comm.chunk(gshape, split, x["location"][0])[1:],
+            (x["shape"], x["start"]),
+        )
+        for x in parts.values()
+    }
+    balanced = all(x[0][0] == x[1][0] for x in expected.values())
+
+    ret = DNDarray(
+        data, gshape, htype, split, devices.sanitize_device(None), sanitize_comm(comm), balanced
+    )
+    ret.__partitions_dict__ = parted
+
+    return ret
+
+
 def full(
     shape: Union[int, Sequence[int]],
     fill_value: Union[int, float],
     dtype: Type[datatype] = types.float32,
     split: Optional[int] = None,
     device: Optional[Device] = None,
     comm: Optional[Communication] = None,
@@ -949,17 +1125,15 @@
     (DNDarray([2.0000, 2.2500, 2.5000, 2.7500, 3.0000], dtype=ht.float32, device=cpu:0, split=None), 0.25)
     """
     # sanitize input parameters
     start = float(start)
     stop = float(stop)
     num = int(num)
     if num < 0:
-        raise ValueError(
-            "number of samples 'num' must be non-negative integer, but was {}".format(num)
-        )
+        raise ValueError(f"number of samples 'num' must be non-negative integer, but was {num}")
     step = (stop - start) / max(1, num - 1 if endpoint else num)
 
     # sanitize device and comm
     device = devices.sanitize_device(device)
     comm = sanitize_comm(comm)
 
     # infer local and global shapes
@@ -1113,26 +1287,26 @@
     # pytorch does not support indexing keyword: switch back
     if indexing == "xy" and len(arrays) > 1:
         grids = list(grids)
         grids[0], grids[1] = grids[1], grids[0]
 
     shape = tuple(array.size for array in arrays)
 
-    return list(
+    return [
         DNDarray(
             array=grid,
             gshape=shape,
             dtype=types.heat_type_of(grid),
             split=splitted,
             device=devices.sanitize_device(grid.device.type),
             comm=sanitize_comm(None),
             balanced=True,
         )
         for grid in grids
-    )
+    ]
 
 
 def ones(
     shape: Union[int, Sequence[int]],
     dtype: Type[datatype] = types.float32,
     split: Optional[int] = None,
     device: Optional[Device] = None,
```

### Comparing `heat-1.2.2/heat/core/indexing.py` & `heat-1.3.0/heat/core/indexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,11 +141,9 @@
             if isinstance(var, int):
                 var = float(var)
         return cond.dtype(cond == 0) * y + cond * x
     elif x is None and y is None:
         return nonzero(cond)
     else:
         raise TypeError(
-            "either both or neither x and y must be given and both must be DNDarrays or numerical scalars({}, {})".format(
-                type(x), type(y)
-            )
+            f"either both or neither x and y must be given and both must be DNDarrays or numerical scalars({type(x)}, {type(y)})"
         )
```

### Comparing `heat-1.2.2/heat/core/io.py` & `heat-1.3.0/heat/core/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,19 +99,19 @@
         [0/2] (5,)
         [1/2] (5,)
         >>> b.lshape
         [0/2] (3,)
         [1/2] (2,)
         """
         if not isinstance(path, str):
-            raise TypeError("path must be str, not {}".format(type(path)))
+            raise TypeError(f"path must be str, not {type(path)}")
         elif not isinstance(dataset, str):
             raise TypeError("dataset must be str, not {}".format(type(dataset)))
         elif split is not None and not isinstance(split, int):
-            raise TypeError("split must be None or int, not {}".format(type(split)))
+            raise TypeError(f"split must be None or int, not {type(split)}")
 
         # infer the type and communicator for the loaded array
         dtype = types.canonical_heat_type(dtype)
         # determine the comm and device the data will be placed on
         device = devices.sanitize_device(device)
         comm = sanitize_comm(comm)
 
@@ -174,25 +174,23 @@
 
         Examples
         --------
         >>> x = ht.arange(100, split=0)
         >>> ht.save_hdf5(x, 'data.h5', dataset='DATA')
         """
         if not isinstance(data, DNDarray):
-            raise TypeError("data must be heat tensor, not {}".format(type(data)))
+            raise TypeError(f"data must be heat tensor, not {type(data)}")
         if not isinstance(path, str):
-            raise TypeError("path must be str, not {}".format(type(path)))
+            raise TypeError(f"path must be str, not {type(path)}")
         if not isinstance(dataset, str):
-            raise TypeError("dataset must be str, not {}".format(type(path)))
+            raise TypeError(f"dataset must be str, not {type(path)}")
 
         # we only support a subset of possible modes
         if mode not in __VALID_WRITE_MODES:
-            raise ValueError(
-                "mode was {}, not in possible modes {}".format(mode, __VALID_WRITE_MODES)
-            )
+            raise ValueError(f"mode was {mode}, not in possible modes {__VALID_WRITE_MODES}")
 
         # chunk the data, if no split is set maximize parallel I/O and chunk first axis
         is_split = data.split is not None
         _, _, slices = data.comm.chunk(data.gshape, data.split if is_split else 0)
 
         # attempt to perform parallel I/O if possible
         if h5py.get_config().mpi:
@@ -310,19 +308,19 @@
         [0/2] (5,)
         [1/2] (5,)
         >>> b.lshape
         [0/2] (3,)
         [1/2] (2,)
         """
         if not isinstance(path, str):
-            raise TypeError("path must be str, not {}".format(type(path)))
+            raise TypeError(f"path must be str, not {type(path)}")
         if not isinstance(variable, str):
-            raise TypeError("dataset must be str, not {}".format(type(variable)))
+            raise TypeError(f"dataset must be str, not {type(variable)}")
         if split is not None and not isinstance(split, int):
-            raise TypeError("split must be None or int, not {}".format(type(split)))
+            raise TypeError(f"split must be None or int, not {type(split)}")
 
         # infer the canonical heat datatype
         dtype = types.canonical_heat_type(dtype)
         # determine the device and comm the data will be placed on
         device = devices.sanitize_device(device)
         comm = sanitize_comm(comm)
 
@@ -687,31 +685,31 @@
     --------
     >>> ht.load('data.h5', dataset='DATA')
     DNDarray([ 1.0000,  2.7183,  7.3891, 20.0855, 54.5981], dtype=ht.float32, device=cpu:0, split=None)
     >>> ht.load('data.nc', variable='DATA')
     DNDarray([ 1.0000,  2.7183,  7.3891, 20.0855, 54.5981], dtype=ht.float32, device=cpu:0, split=None)
     """
     if not isinstance(path, str):
-        raise TypeError("Expected path to be str, but was {}".format(type(path)))
+        raise TypeError(f"Expected path to be str, but was {type(path)}")
     extension = os.path.splitext(path)[-1].strip().lower()
 
     if extension in __CSV_EXTENSION:
         return load_csv(path, *args, **kwargs)
     elif extension in __HDF5_EXTENSIONS:
         if supports_hdf5():
             return load_hdf5(path, *args, **kwargs)
         else:
-            raise RuntimeError("hdf5 is required for file extension {}".format(extension))
+            raise RuntimeError(f"hdf5 is required for file extension {extension}")
     elif extension in __NETCDF_EXTENSIONS:
         if supports_netcdf():
             return load_netcdf(path, *args, **kwargs)
         else:
-            raise RuntimeError("netcdf is required for file extension {}".format(extension))
+            raise RuntimeError(f"netcdf is required for file extension {extension}")
     else:
-        raise ValueError("Unsupported file extension {}".format(extension))
+        raise ValueError(f"Unsupported file extension {extension}")
 
 
 def load_csv(
     path: str,
     header_lines: int = 0,
     sep: str = ",",
     dtype: datatype = types.float32,
@@ -771,21 +769,21 @@
     >>> b.lshape
     [0/3] (35, 4)
     [1/3] (35, 4)
     [2/3] (35, 4)
     [3/3] (35, 4)
     """
     if not isinstance(path, str):
-        raise TypeError("path must be str, not {}".format(type(path)))
+        raise TypeError(f"path must be str, not {type(path)}")
     if not isinstance(sep, str):
-        raise TypeError("separator must be str, not {}".format(type(sep)))
+        raise TypeError(f"separator must be str, not {type(sep)}")
     if not isinstance(header_lines, int):
-        raise TypeError("header_lines must int, not {}".format(type(header_lines)))
+        raise TypeError(f"header_lines must int, not {type(header_lines)}")
     if split not in [None, 0, 1]:
-        raise ValueError("split must be in [None, 0, 1], but is {}".format(split))
+        raise ValueError(f"split must be in [None, 0, 1], but is {split}")
 
     # infer the type and communicator for the loaded array
     dtype = types.canonical_heat_type(dtype)
     # determine the comm and device the data will be placed on
     device = devices.sanitize_device(device)
     comm = sanitize_comm(comm)
 
@@ -794,15 +792,15 @@
     size = comm.size
 
     if split is None:
         with open(path) as f:
             data = f.readlines()
             data = data[header_lines:]
             result = []
-            for i, line in enumerate(data):
+            for line in data:
                 values = line.replace("\n", "").replace("\r", "").split(sep)
                 values = [float(val) for val in values]
                 result.append(values)
             resulting_tensor = factories.array(
                 result, dtype=dtype, split=split, device=device, comm=comm
             )
 
@@ -814,15 +812,15 @@
         with open(path, "rb") as f:
             f.seek(displs[rank], 0)
             line_starts = []
             r = f.read(counts[rank])
             for pos, l in enumerate(r):
                 if chr(l) == "\n":
                     # Check if it is part of '\r\n'
-                    if not chr(r[pos - 1]) == "\r":
+                    if chr(r[pos - 1]) != "\r":
                         line_starts.append(pos + 1)
                 elif chr(l) == "\r":
                     # check if file line is terminated by '\r\n'
                     if pos + 1 < len(r) and chr(r[pos + 1]) == "\n":
                         line_starts.append(pos + 2)
                         lineter_len = 2
                     else:
@@ -955,22 +953,22 @@
         An optional object of type Communication to be used.
     truncate : bool
         Whether to truncate an existing file before writing, i.e. fully overwrite it.
         The sane default is True. Setting it to False will not shorten files if
         needed and thus may leave garbage at the end of existing files.
     """
     if not isinstance(path, str):
-        raise TypeError("path must be str, not {}".format(type(path)))
+        raise TypeError(f"path must be str, not {type(path)}")
     if not isinstance(sep, str):
-        raise TypeError("separator must be str, not {}".format(type(sep)))
+        raise TypeError(f"separator must be str, not {type(sep)}")
     # check this to allow None
     if not isinstance(header_lines, Iterable) and header_lines is not None:
-        raise TypeError("header_lines must Iterable[str], not {}".format(type(header_lines)))
+        raise TypeError(f"header_lines must Iterable[str], not {type(header_lines)}")
     if data.split not in [None, 0, 1]:
-        raise ValueError("split must be in [None, 0, 1], but is {}".format(data.split))
+        raise ValueError(f"split must be in [None, 0, 1], but is {data.split}")
 
     if os.path.exists(path) and truncate:
         if data.comm.rank == 0:
             os.truncate(path, 0)
         # avoid truncating and writing at the same time
         data.comm.handle.Barrier()
 
@@ -1084,28 +1082,28 @@
 
     Examples
     --------
     >>> x = ht.arange(100, split=0)
     >>> ht.save(x, 'data.h5', 'DATA', mode='a')
     """
     if not isinstance(path, str):
-        raise TypeError("Expected path to be str, but was {}".format(type(path)))
+        raise TypeError(f"Expected path to be str, but was {type(path)}")
     extension = os.path.splitext(path)[-1].strip().lower()
 
     if extension in __HDF5_EXTENSIONS:
         if supports_hdf5():
             save_hdf5(data, path, *args, **kwargs)
         else:
-            raise RuntimeError("hdf5 is required for file extension {}".format(extension))
+            raise RuntimeError(f"hdf5 is required for file extension {extension}")
     elif extension in __NETCDF_EXTENSIONS:
         if supports_netcdf():
             save_netcdf(data, path, *args, **kwargs)
         else:
-            raise RuntimeError("netcdf is required for file extension {}".format(extension))
+            raise RuntimeError(f"netcdf is required for file extension {extension}")
     elif extension in __CSV_EXTENSION:
         save_csv(data, path, *args, **kwargs)
     else:
-        raise ValueError("Unsupported file extension {}".format(extension))
+        raise ValueError(f"Unsupported file extension {extension}")
 
 
 DNDarray.save = lambda self, path, *args, **kwargs: save(self, path, *args, **kwargs)
 DNDarray.save.__doc__ = save.__doc__
```

### Comparing `heat-1.2.2/heat/core/linalg/basics.py` & `heat-1.3.0/heat/core/linalg/basics.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,24 +81,22 @@
               [1., 0., 0.],
               [0., 1., 0.]], dtype=ht.float32, device=cpu:0, split=None)
     """
     sanitation.sanitize_in(a)
     sanitation.sanitize_in(b)
 
     if a.device != b.device:
-        raise ValueError(
-            "'a' and 'b' must have the same device type, {} != {}".format(a.device, b.device)
-        )
+        raise ValueError(f"'a' and 'b' must have the same device type, {a.device} != {b.device}")
     if a.comm != b.comm:  # pragma: no cover
-        raise ValueError("'a' and 'b' must have the same comm, {} != {}".format(a.comm, b.comm))
+        raise ValueError(f"'a' and 'b' must have the same comm, {a.comm} != {b.comm}")
 
     a_2d, b_2d = False, False
     a_shape, b_shape = list(a.shape), list(b.shape)
 
-    if not axis == -1 or torch.unique(torch.tensor([axisa, axisb, axisc, axis])).numel() == 1:
+    if axis != -1 or torch.unique(torch.tensor([axisa, axisb, axisc, axis])).numel() == 1:
         axis = stride_tricks.sanitize_axis(a.shape, axis)
         axisa, axisb, axisc = (axis,) * 3
     else:
         axisa = stride_tricks.sanitize_axis(a.shape, axisa)
         axisb = stride_tricks.sanitize_axis(b.shape, axisb)
         axisc = stride_tricks.sanitize_axis(a.shape, axisc)
 
@@ -112,15 +110,15 @@
     output_shape = stride_tricks.broadcast_shape(a_shape, b_shape)
 
     # 2d -> 3d vector
     if a.shape[axisa] == 2:
         a_2d = True
         shape = tuple(1 if i == axisa else j for i, j in enumerate(a.shape))
         a = manipulations.concatenate(
-            [a, factories.zeros(shape, dtype=a.dtype, device=a.device)], axis=axisa
+            [a, factories.zeros(shape, dtype=a.dtype, device=a.device, comm=a.comm)], axis=axisa
         )
     if b.shape[axisb] == 2:
         b_2d = True
         shape = tuple(1 if i == axisb else j for i, j in enumerate(b.shape))
         b = manipulations.concatenate(
             [b, factories.zeros(shape, dtype=b.dtype, device=b.device)], axis=axisb
         )
@@ -131,15 +129,15 @@
     if axisc != axisb:
         b = manipulations.moveaxis(b, axisb, axisc)
 
     axis = axisc
 
     # by now split axes must be aligned
     if a.split != b.split:
-        raise ValueError("'a' and 'b' must have the same split, {} != {}".format(a.split, b.split))
+        raise ValueError(f"'a' and 'b' must have the same split, {a.split} != {b.split}")
 
     if not (a.is_balanced and b.is_balanced):
         # TODO: replace with sanitize_redistribute after #888 is merged
         b = manipulations.redistribute(b, b.lshape_map, a.lshape_map)
 
     promoted = torch.promote_types(a.larray.dtype, b.larray.dtype)
 
@@ -190,28 +188,28 @@
 
     if types.heat_type_is_exact(a.dtype):
         raise RuntimeError("dtype of DNDarray must be floating-point.")
 
     # no split in the square matrices
     if not a.is_distributed() or a.split < a.ndim - 2:
         data = torch.linalg.det(a.larray)
-        sp = None if not a.is_distributed() else a.split
+        sp = a.split if a.is_distributed() else None
         return DNDarray(
             data,
             a.shape[:-2],
             types.heat_type_of(data),
             split=sp,
             device=a.device,
             comm=a.comm,
             balanced=a.balanced,
         )
 
     acopy = a.copy()
     acopy = manipulations.reshape(acopy, (-1, m, m), new_split=a.split - a.ndim + 3)
-    adet = factories.ones(acopy.shape[0], dtype=a.dtype, device=a.device)
+    adet = factories.ones(acopy.shape[0], dtype=a.dtype, device=a.device, comm=a.comm)
 
     for k in range(adet.shape[0]):
         m = 0
         for i in range(n):
             # partial pivoting
             if np.isclose(acopy[k, i, i].item(), 0):
                 abord = True
@@ -392,17 +390,16 @@
                 if abord:
                     raise RuntimeError("Inverse does not exist")
 
             scale = acopy[k, i, i].item()
 
             # Circumvent an issue with DNDarray setter and getter that caused precision errors
             if a.split == a.ndim - 2:
-                if rank < acopy.comm.size - 1:
-                    if i >= displs[rank + 1]:
-                        rank += 1
+                if rank < acopy.comm.size - 1 and i >= displs[rank + 1]:
+                    rank += 1
                 if acopy.comm.rank == rank:
                     ainv.larray[k, i - displs[rank], :] /= scale
                     acopy.larray[k, i - displs[rank], :] /= scale
             else:
                 ainv[k, i, :].larray /= scale
                 acopy[k, i, :].larray /= scale
 
@@ -471,30 +468,29 @@
     >>> b[0] = ht.arange(1, k + 1)
     >>> b[:, 0] = ht.arange(1, j + 1).larray
     [0/1] tensor([[1., 2., 3., 4., 5., 6., 7.],
                   [2., 1., 1., 1., 1., 1., 1.]])
     [1/1] tensor([[3., 1., 1., 1., 1., 1., 1.],
                   [4., 1., 1., 1., 1., 1., 1.]])
     >>> linalg.matmul(a, b).larray
+
     [0/1] tensor([[18.,  8.,  9., 10.],
                   [14.,  6.,  7.,  8.],
                   [18.,  7.,  8.,  9.],
                   [22.,  8.,  9., 10.],
                   [26.,  9., 10., 11.]])
     [1/1] tensor([[11., 12., 13.],
                   [ 9., 10., 11.],
                   [10., 11., 12.],
                   [11., 12., 13.],
                   [12., 13., 14.]])
     """
     if a.gshape[-1] != b.gshape[0]:
         raise ValueError(
-            "If the last dimension of a ({}) is not the same size as the second-to-last dimension of b. ({})".format(
-                a.gshape[-1], b.gshape[-2]
-            )
+            f"If the last dimension of a ({a.gshape[-1]}) is not the same size as the second-to-last dimension of b. ({b.gshape[-2]})"
         )
 
     # determine if a larger type is needed for c
     c_type = types.promote_types(a.dtype, b.dtype)
     gpu_int_flag = False
     if str(a.device)[:3] == "gpu":
         og_type = c_type
@@ -516,39 +512,39 @@
         if gpu_int_flag:
             ret = og_type(ret, device=a.device)
         return ret
 
     if a.split is None and b.split is None:  # matmul from torch
         if len(a.gshape) < 2 or len(b.gshape) < 2 or not allow_resplit:
             # if either of A or B is a vector
-            ret = factories.array(torch.matmul(a.larray, b.larray), device=a.device)
+            ret = factories.array(torch.matmul(a.larray, b.larray), device=a.device, comm=a.comm)
             if gpu_int_flag:
                 ret = og_type(ret, device=a.device)
             return ret
 
         a.resplit_(0)
         slice_0 = a.comm.chunk(a.shape, a.split)[2][0]
         hold = a.larray @ b.larray
 
-        c = factories.zeros((a.gshape[-2], b.gshape[1]), dtype=c_type, device=a.device)
+        c = factories.zeros((a.gshape[-2], b.gshape[1]), dtype=c_type, device=a.device, comm=a.comm)
         c.larray[slice_0.start : slice_0.stop, :] += hold
         c.comm.Allreduce(MPI.IN_PLACE, c, MPI.SUM)
         if gpu_int_flag:
             c = og_type(c, device=a.device)
         return c
 
     # if they are vectors they need to be expanded to be the proper dimensions
     vector_flag = False  # flag to run squeeze at the end of the function
     if len(a.gshape) < 2 and len(b.gshape) < 2:
         # make both split 0, do a local mm then a sum
         a.resplit_(0)
         b.resplit_(0)
         res = a.larray @ b.larray
         a.comm.Allreduce(MPI.IN_PLACE, res, MPI.SUM)
-        ret = factories.array(res, split=None, device=a.device)
+        ret = factories.array(res, split=None, device=a.device, comm=a.comm)
         if gpu_int_flag:
             ret = og_type(ret, device=a.device)
         return ret
     elif len(a.gshape) < 2:
         a = manipulations.expand_dims(a, axis=0)
         vector_flag = True
     elif len(b.gshape) < 2:
@@ -563,67 +559,73 @@
     tdev = a.device.torch_device
 
     if (
         (a.split == 0 and b.split is None) or (a.split is None and b.split == 1)
     ) and not vector_flag:
         split = a.split if a.split is not None else b.split
         split = split if not vector_flag else 0
-        c = factories.zeros((a.gshape[-2], b.gshape[1]), split=split, dtype=c_type, device=a.device)
+        c = factories.zeros(
+            (a.gshape[-2], b.gshape[1]), split=split, dtype=c_type, device=a.device, comm=a.comm
+        )
         c.larray += a.larray @ b.larray
 
         ret = c if not vector_flag else c.squeeze()
         if gpu_int_flag:
             ret = og_type(ret, device=a.device)
         return ret
 
     elif a.split == 1 and b.split is None:
         c = torch.zeros((a.gshape[-2], b.gshape[1]), dtype=c_type.torch_type(), device=tdev)
 
         a_idx = a.comm.chunk(a.shape, a.split)[2]
         c += a.larray @ b.larray[a_idx[1].start : a_idx[1].start + a.lshape[-1], :]
         a.comm.Allreduce(MPI.IN_PLACE, c, MPI.SUM)
         c = c if not vector_flag else c.squeeze()
-        ret = factories.array(c, split=a.split if b.gshape[1] > 1 else 0, device=a.device)
+        ret = factories.array(
+            c, split=a.split if b.gshape[1] > 1 else 0, device=a.device, comm=a.comm
+        )
         if gpu_int_flag:
             ret = og_type(ret, device=a.device)
         return ret
 
     elif a.split is None and b.split == 0:
         c = torch.zeros((a.gshape[-2], b.gshape[1]), dtype=c_type.torch_type(), device=tdev)
         b_idx = b.comm.chunk(b.shape, b.split)[2]
         c += a.larray[:, b_idx[0].start : b_idx[0].start + b.lshape[0]] @ b.larray
         b.comm.Allreduce(MPI.IN_PLACE, c, MPI.SUM)
         c = c if not vector_flag else c.squeeze()
-        ret = factories.array(c, split=b.split if a.gshape[-2] > 1 else 0, device=a.device)
+        ret = factories.array(
+            c, split=b.split if a.gshape[-2] > 1 else 0, device=a.device, comm=a.comm
+        )
         if gpu_int_flag:
             ret = og_type(ret, device=a.device)
         return ret
 
     elif (
         a.split == 0 and b.split is None
     ):  # this case and the one below will only be reaching if one of them is a vector
         c = torch.zeros((a.gshape[-2], b.lshape[1]), dtype=c_type.torch_type(), device=tdev)
         a_idx = a.comm.chunk(a.shape, a.split)[2]
         c[a_idx[0]] += a.larray @ b.larray
         a.comm.Allreduce(MPI.IN_PLACE, c, MPI.SUM)
         c = c if not vector_flag else c.squeeze()
         split = a.split if b.gshape[1] > 1 else 0
         split = split if not vector_flag else 0
-        ret = factories.array(c, split=split, device=a.device)
+        ret = factories.array(c, split=split, device=a.device, comm=a.comm)
         if gpu_int_flag:
             ret = og_type(ret, device=a.device)
         return ret
 
     elif a.split is None and b.split == 1:
         c = torch.zeros((a.gshape[-2], b.lshape[1]), dtype=c_type.torch_type(), device=tdev)
         c += a.larray @ b.larray
         c = c if not vector_flag else c.squeeze()
         split = b.split if a.gshape[1] > 1 else 0
         split = split if not vector_flag else 0
-        ret = factories.array(c, is_split=split, device=a.device)
+        ret = factories.array(c, is_split=split, device=a.device, comm=a.comm)
         if gpu_int_flag:
             ret = og_type(ret, device=a.device)
         return ret
 
     elif a.split == 0 and b.split == 0:
         split_0_flag = True
     elif a.split == 1 and b.split == 1:
@@ -645,15 +647,15 @@
         kB = min([a.gshape[-1] // a.comm.size, b.gshape[0] // b.comm.size])
     elif a.split == len(a.gshape) - 2 and b.split == len(a.gshape) - 1:
         kB = a.gshape[-1]
     elif a.split == len(a.gshape) - 1:
         kB = a.gshape[-1] // a.comm.size
     elif b.split == len(a.gshape) - 2:
         kB = b.gshape[0] // b.comm.size
-        kB = kB if kB < a.gshape[-1] else a.gshape[-1]
+        kB = min(kB, a.gshape[-1])
 
     if a.lshape[-1] % kB != 0 or (kB == 1 and a.lshape[-1] != 1):
         rem_a = 1
     if b.lshape[0] % kB != 0 or (kB == 1 and b.lshape[-2] != 1):
         rem_b = 1
 
     # get the lshape map to determine what needs to be sent where as well as M and N
@@ -691,18 +693,18 @@
     index_map[b.comm.rank, 1, 0] = torch.tensor((b_idx[0].start, b_idx[0].stop), device=tdev)
     index_map[b.comm.rank, 1, 1] = torch.tensor((b_idx[1].start, b_idx[1].stop), device=tdev)
 
     index_map_comm = a.comm.Iallreduce(MPI.IN_PLACE, index_map, MPI.SUM)
 
     # for the communication scheme, the output array needs to be created
     c_shape = (a.gshape[-2], b.gshape[1])
-    c = factories.zeros(c_shape, split=a.split, dtype=c_type, device=a.device)
+    c = factories.zeros(c_shape, split=a.split, dtype=c_type, device=a.device, comm=a.comm)
 
     # get the index map for c
-    c_index_map = factories.zeros((c.comm.size, 2, 2), device=a.device)
+    c_index_map = factories.zeros((c.comm.size, 2, 2), device=a.device, comm=a.comm)
     c_idx = c.comm.chunk(c.shape, c.split)[2]
     c_index_map[c.comm.rank, 0, :] = (c_idx[0].start, c_idx[0].stop)
     c_index_map[c.comm.rank, 1, :] = (c_idx[1].start, c_idx[1].stop)
     c_wait = c.comm.Iallreduce(MPI.IN_PLACE, c_index_map, MPI.SUM)
 
     if a.split == 0:
         a_block_map = torch.zeros(
@@ -862,19 +864,18 @@
                 # check if there is a remainder on b in the previous node
                 # this loop is intended to get the remainders of b since it is the one being passed
                 if pr - 1 in b_rem_locs0:
                     # takes care of the remainders in b as well as dim0 of a
                     b_rem[pr - 1] = b_lp_data[pr - 1][-1]
 
                 # this loop is to take care of the remainders in dim0 of A
-                if a_rem_locs0.nelement() != 0:
-                    if r_loc is not None:
-                        st = index_map[pr - 1, 1, 0, 0].item()
-                        sp = index_map[pr - 1, 1, 0, 1].item()
-                        c.larray[r_loc.item(), :] += r[st:sp] @ b_lp_data[pr - 1]
+                if a_rem_locs0.nelement() != 0 and r_loc is not None:
+                    st = index_map[pr - 1, 1, 0, 0].item()
+                    sp = index_map[pr - 1, 1, 0, 1].item()
+                    c.larray[r_loc.item(), :] += r[st:sp] @ b_lp_data[pr - 1]
                 del b_lp_data[pr - 1]
 
             # need to wait if its the last loop, also need to collect the remainders
             if pr == b.comm.size - 1:
                 req[pr].Wait()
                 __mm_c_block_setter(
                     b_proc=pr,
@@ -892,38 +893,37 @@
                 )
                 # check if there is a remainder on b on the last node (there shouldnt be)
                 if pr in b_rem_locs0:
                     # this is to save the data from B required by the remainders from dim1 of A
                     b_rem[pr] = b_lp_data[pr][-1]
 
                 # this loop is to take care of the remainders in the 0th dimension of A
-                if a_rem_locs0.nelement() != 0:
-                    if r_loc is not None:
-                        st = index_map[pr, 1, 0, 0].item()
-                        sp = index_map[pr, 1, 0, 1].item()
-
-                        if split_01_flag:
-                            st1 = index_map[pr, 1, 1, 0].item()
-                            sp1 = index_map[pr, 1, 1, 1].item()
-                            c.larray[r_loc.item(), st1:sp1] += r[st:sp] @ b_lp_data[pr]
-                        else:
-                            c.larray[r_loc.item(), :] += r[st:sp] @ b_lp_data[pr]
+                if a_rem_locs0.nelement() != 0 and r_loc is not None:
+                    st = index_map[pr, 1, 0, 0].item()
+                    sp = index_map[pr, 1, 0, 1].item()
+
+                    if split_01_flag:
+                        st1 = index_map[pr, 1, 1, 0].item()
+                        sp1 = index_map[pr, 1, 1, 1].item()
+                        c.larray[r_loc.item(), st1:sp1] += r[st:sp] @ b_lp_data[pr]
+                    else:
+                        c.larray[r_loc.item(), :] += r[st:sp] @ b_lp_data[pr]
 
                 # set the final blocks on the last loop, then adjust for the
                 # the remainders which were collected in b_rem
                 if b_rem_locs0.numel():
                     c.larray[: a_node_rem_s0.shape[0]] += a_node_rem_s0 @ b_rem
                 del b_lp_data[pr]
 
         if vector_flag:
             c_loc = c.larray.squeeze()
             if c_loc.nelement() == 1:
                 c_loc = torch.tensor(c_loc, device=tdev)
 
-            c = factories.array(c_loc, is_split=0, device=a.device)
+            c = factories.array(c_loc, is_split=0, device=a.device, comm=a.comm)
         if gpu_int_flag:
             c = og_type(c, device=a.device)
         return c
 
     elif split_1_flag:
         # for this case, a is sent to b
         #   this is because 'b' has complete columns and the rows of 'a' are split
@@ -978,20 +978,19 @@
                 )
                 # check if there is a remainder on b in the previous node
                 # this loop is intended to get the remainders of b since it is the one being passed
                 if pr - 1 in a_rem_locs1:
                     # takes care of the remainders in b as well as dim0 of a
                     a_rem[:, pr - 1] = a_lp_data[pr - 1][:, -1]
                 # this loop is to take care of the remainders in dim1 of B
-                if b_rem_locs1.nelement() != 0:
-                    if r_loc is not None:
-                        st = index_map[pr - 1, 0, 1, 0].item()
-                        sp = index_map[pr - 1, 0, 1, 1].item()
+                if b_rem_locs1.nelement() != 0 and r_loc is not None:
+                    st = index_map[pr - 1, 0, 1, 0].item()
+                    sp = index_map[pr - 1, 0, 1, 1].item()
 
-                        c.larray[:, r_loc.item()] += (a_lp_data[pr - 1] @ r[st:sp, None]).flatten()
+                    c.larray[:, r_loc.item()] += (a_lp_data[pr - 1] @ r[st:sp, None]).flatten()
 
                 del a_lp_data[pr - 1]
 
             # need to wait if its the last loop, also need to collect the remainders
             if pr == b.comm.size - 1:
                 req[pr].Wait()
                 __mm_c_block_setter(
@@ -1009,25 +1008,24 @@
                     c=c.larray,
                 )
                 # check if there is a remainder on b on the last node (there shouldnt be)
                 if pr in a_rem_locs1:
                     # this is to save the data from B required by the remainders from dim1 of A
                     a_rem[:, pr] = a_lp_data[pr][:, -1]
                 # this loop is to take care of the remainders in the 0th dimension of A
-                if b_rem_locs1.nelement() != 0:
-                    if r_loc is not None:
-                        st = index_map[pr, 0, 1, 0].item()
-                        sp = index_map[pr, 0, 1, 1].item()
-                        c.larray[:, r_loc.item()] += (a_lp_data[pr] @ r[st:sp, None]).flatten()
+                if b_rem_locs1.nelement() != 0 and r_loc is not None:
+                    st = index_map[pr, 0, 1, 0].item()
+                    sp = index_map[pr, 0, 1, 1].item()
+                    c.larray[:, r_loc.item()] += (a_lp_data[pr] @ r[st:sp, None]).flatten()
                 # set the final blocks on the last loop, then adjust for the the remainders which were collected in b_rem
                 if a_rem_locs1.numel():
                     c.larray[:, : b_node_rem_s1.shape[1]] += a_rem @ b_node_rem_s1
                 del a_lp_data[pr]
         if vector_flag:
-            c = factories.array(c.larray.squeeze(), is_split=0, device=a.device)
+            c = factories.array(c.larray.squeeze(), is_split=0, device=a.device, comm=a.comm)
         if gpu_int_flag:
             c = og_type(c, device=a.device)
         return c
 
     elif split_01_flag:
         # for this case there are no remainders which need to be taken care of
         req = {}
@@ -1062,15 +1060,15 @@
                 st0 = index_map[pr, 0, 0, 0].item()
                 sp0 = index_map[pr, 0, 0, 1].item() + 1
                 st1 = index_map[pr, 1, 1, 0].item()
                 sp1 = index_map[pr, 1, 1, 1].item()
                 c.larray[: sp0 - st0, st1:sp1] += a.larray @ b_lp_data[pr]
                 del b_lp_data[pr]
         if vector_flag:
-            c = factories.array(c.larray.squeeze(), is_split=0, device=a.device)
+            c = factories.array(c.larray.squeeze(), is_split=0, device=a.device, comm=a.comm)
         if gpu_int_flag:
             c = og_type(c, device=a.device)
 
         return c
 
     elif split_10_flag:
         # todo: this may create the full matrix on evey process, issue #360
@@ -1086,15 +1084,15 @@
             res += a.larray[:, -1, None] @ b.larray[None, -1, :]
 
         a.comm.Allreduce(MPI.IN_PLACE, res, MPI.SUM)
         split = a.split if b.gshape[1] > 1 else 0
         if vector_flag:
             split = 0
             res = res.squeeze()
-        c = factories.array(res, split=split, device=a.device)
+        c = factories.array(res, split=split, device=a.device, comm=a.comm)
         if gpu_int_flag:
             c = og_type(c, device=a.device)
         return c
 
 
 DNDarray.__matmul__ = lambda self, other: matmul(self, other)
 
@@ -1181,49 +1179,49 @@
 
     row_axis, col_axis = axis
 
     if ord == 1:
         if col_axis > row_axis and not keepdims:
             col_axis -= 1
         return statistics.max(
-            arithmetics.sum(rounding.abs(x), axis=row_axis, keepdim=keepdims),
+            arithmetics.sum(rounding.abs(x), axis=row_axis, keepdims=keepdims),
             axis=col_axis,
-            keepdim=keepdims,
+            keepdims=keepdims,
         )
     elif ord == -1:
         if col_axis > row_axis and not keepdims:
             col_axis -= 1
         return statistics.min(
-            arithmetics.sum(rounding.abs(x), axis=row_axis, keepdim=keepdims),
+            arithmetics.sum(rounding.abs(x), axis=row_axis, keepdims=keepdims),
             axis=col_axis,
-            keepdim=keepdims,
+            keepdims=keepdims,
         )
     elif ord == 2:
         raise NotImplementedError("The largest singular value can't be computed yet.")
     elif ord == -2:
         raise NotImplementedError("The smallest singular value can't be computed yet.")
     elif ord == constants.inf:
         if row_axis > col_axis and not keepdims:
             row_axis -= 1
         return statistics.max(
-            arithmetics.sum(rounding.abs(x), axis=col_axis, keepdim=keepdims),
+            arithmetics.sum(rounding.abs(x), axis=col_axis, keepdims=keepdims),
             axis=row_axis,
-            keepdim=keepdims,
+            keepdims=keepdims,
         )
     elif ord == -constants.inf:
         if row_axis > col_axis and not keepdims:
             row_axis -= 1
         return statistics.min(
-            arithmetics.sum(rounding.abs(x), axis=col_axis, keepdim=keepdims),
+            arithmetics.sum(rounding.abs(x), axis=col_axis, keepdims=keepdims),
             axis=row_axis,
-            keepdim=keepdims,
+            keepdims=keepdims,
         )
     elif ord in [None, "fro"]:
         return exponential.sqrt(
-            arithmetics.sum((complex_math.conj(x) * x).real, axis=axis, keepdim=keepdims)
+            arithmetics.sum((complex_math.conj(x) * x).real, axis=axis, keepdims=keepdims)
         )
     elif ord == "nuc":
         raise NotImplementedError("The nuclear norm can't be computed yet.")
     else:
         raise ValueError("Invalid norm order for matrices.")
 
 
@@ -1487,29 +1485,25 @@
     for array in [a, b]:
         sanitation.sanitize_in(array)
         devices.append(array.device)
     if devices.count(devices[0]) == 2:
         device = devices[0]
     else:
         raise RuntimeError(
-            "input arrays on different devices: input 0 on {}, input 1 on {}".format(
-                devices[0], devices[1]
-            )
+            f"input arrays on different devices: input 0 on {devices[0]}, input 1 on {devices[1]}"
         )
 
     # sanitize dimensions
     # TODO implement is_1D in sanitation module #468
     if a.ndim > 1:
         a = manipulations.flatten(a)
     if b.ndim > 1:
         b = manipulations.flatten(b)
     if a.ndim == 0 or b.ndim == 0:
-        raise RuntimeError(
-            "a, b must be 1-D DNDarrays, but were {}-D and {}-D".format(a.ndim, b.ndim)
-        )
+        raise RuntimeError(f"a, b must be 1-D DNDarrays, but were {a.ndim}-D and {b.ndim}-D")
 
     outer_gshape = (a.gshape[0], b.gshape[0])
     t_a = a.larray
     t_b = b.larray
     t_outer_dtype = torch.promote_types(t_a.dtype, t_b.dtype)
     t_a, t_b = t_a.type(t_outer_dtype), t_b.type(t_outer_dtype)
     outer_dtype = types.canonical_heat_type(t_outer_dtype)
@@ -1617,21 +1611,19 @@
     ----------
     a : DNDarray
         The vector to be projected. Must be a 1D ``DNDarray``
     b : DNDarray
         The vector to project onto. Must be a 1D ``DNDarray``
     """
     if not isinstance(a, DNDarray) or not isinstance(b, DNDarray):
-        raise TypeError(
-            "a, b must be of type ht.DNDarray, but were {}, {}".format(type(a), type(b))
-        )
+        raise TypeError(f"a, b must be of type ht.DNDarray, but were {type(a)}, {type(b)}")
 
     if len(a.shape) != 1 or len(b.shape) != 1:
         raise RuntimeError(
-            "a, b must be vectors of length 1, but were {}, {}".format(len(a.shape), len(b.shape))
+            f"a, b must be vectors of length 1, but were {len(a.shape)}, {len(b.shape)}"
         )
 
     return (dot(a, b) / dot(b, b)) * b
 
 
 def trace(
     a: DNDarray,
@@ -1827,18 +1819,15 @@
 
     # -------------------------------
     # CASE > 2D => DNDArray
     # -------------------------------
 
     # sanitize axis1, axis2 (make sure axis1 < axis2)
     if axis1 > axis2:
-        tmp = axis1
-        axis1 = axis2
-        axis2 = tmp
-
+        axis1, axis2 = axis2, axis1
     # ----------------------------------
     # CASE split axis NOT IN trace axes
     # ----------------------------------
     # compute each diagonal sum
     if not (a.is_distributed() and a.split in (axis1, axis2)):
         # extract diagonals
         diag_t = torch.diagonal(a.larray, offset=offset, dim1=axis1, dim2=axis2)
@@ -1902,19 +1891,15 @@
             sanitation.sanitize_out(out, tuple(res_shape), out.split, out.device)
             out.larray = sum_along_diagonals.larray
 
         return sum_along_diagonals
 
     if a.is_distributed():
         # (...and a.split not in (axis1, axis2))
-        if a.split < axis2:
-            gather_axis = a.split
-        else:
-            gather_axis = a.split - 2
-
+        gather_axis = a.split if a.split < axis2 else a.split - 2
         # check if gather_axis is in range of result
         if gather_axis >= sum_along_diagonals_t.ndim:
             gather_axis = sum_along_diagonals_t.ndim - 1
 
         # Stack all partial results back together along the correct axis
         sum_along_diagonals = factories.array(
             sum_along_diagonals_t, dtype=dtype, is_split=gather_axis, comm=a.comm, device=a.device
@@ -2081,15 +2066,15 @@
         except TypeError:
             raise ValueError("axes must be an iterable containing ints")
 
         if len(axes) != dimensions:
             raise ValueError("axes do not match tensor shape")
         for index, axis in enumerate(axes):
             if not isinstance(axis, int):
-                raise TypeError("axis must be an integer, but was {}".format(type(axis)))
+                raise TypeError(f"axis must be an integer, but was {type(axis)}")
             elif axis < 0:
                 axes[index] = axis + dimensions
 
     # infer the new split axis, it is the position of the split axis within the new axes permutation
     try:
         transposed_split = axes.index(a.split) if a.split is not None else None
     except ValueError:
@@ -2145,15 +2130,15 @@
         If the input is not a tensor or the diagonal offset cannot be converted to an integral value.
     """
     sanitation.sanitize_in(m)
 
     try:
         k = int(k)
     except ValueError:
-        raise TypeError("Expected k to be integral, but was {}".format(type(k)))
+        raise TypeError(f"Expected k to be integral, but was {type(k)}")
 
     # chunk the global shape of the tensor to obtain the offset compared to the other ranks
     offset, _, _ = m.comm.chunk(m.shape, m.split)
     dimensions = len(m.shape)
 
     # manually repeat the input for vectors
     if dimensions == 1:
@@ -2273,28 +2258,28 @@
     x1 = manipulations.flatten(x1)
     x2 = manipulations.flatten(x2)
 
     return arithmetics.sum(arithmetics.multiply(complex_math.conjugate(x1), x2))
 
 
 def vecdot(
-    x1: DNDarray, x2: DNDarray, axis: Optional[int] = None, keepdim: Optional[bool] = None
+    x1: DNDarray, x2: DNDarray, axis: Optional[int] = None, keepdims: Optional[bool] = None
 ) -> DNDarray:
     """
     Computes the (vector) dot product of two DNDarrays.
 
     Parameters
     ----------
     x1 : DNDarray
         first input array.
     x2 : DNDarray
         second input array. Must be compatible with x1.
     axis : int, optional
         axis over which to compute the dot product. The last dimension is used if 'None'.
-    keepdim : bool, optional
+    keepdims : bool, optional
         If this is set to 'True', the axes which are reduced are left in the result as dimensions with size one.
 
     See Also
     --------
     dot
         NumPy-like dot function.
 
@@ -2306,15 +2291,15 @@
               [9., 9., 9.]], dtype=ht.float32, device=cpu:0, split=None)
     """
     m = arithmetics.mul(x1, x2)
 
     if axis is None:
         axis = m.ndim - 1
 
-    return arithmetics.sum(m, axis=axis, keepdim=keepdim)
+    return arithmetics.sum(m, axis=axis, keepdims=keepdims)
 
 
 def vector_norm(
     x: DNDarray,
     axis: Optional[Union[int, Tuple[int]]] = None,
     keepdims=False,
     ord: Optional[Union[int, float]] = None,
@@ -2382,24 +2367,24 @@
     else:
         try:
             axis = int(axis)
         except Exception:
             raise TypeError("'axis' must be an integer or 1-tuple for vectors.")
 
     if ord == constants.INF:
-        return statistics.max(rounding.abs(x), axis=axis, keepdim=keepdims)
+        return statistics.max(rounding.abs(x), axis=axis, keepdims=keepdims)
     elif ord == -constants.INF:
-        return statistics.min(rounding.abs(x), axis=axis, keepdim=keepdims)
+        return statistics.min(rounding.abs(x), axis=axis, keepdims=keepdims)
     elif ord == 0:
-        return arithmetics.sum(x != 0, axis=axis, keepdim=keepdims).astype(types.float)
+        return arithmetics.sum(x != 0, axis=axis, keepdims=keepdims).astype(types.float)
     elif ord == 1:
-        return arithmetics.sum(rounding.abs(x), axis=axis, keepdim=keepdims)
+        return arithmetics.sum(rounding.abs(x), axis=axis, keepdims=keepdims)
     elif ord is None or ord == 2:
         s = (complex_math.conj(x) * x).real
-        return exponential.sqrt(arithmetics.sum(s, axis=axis, keepdim=keepdims))
+        return exponential.sqrt(arithmetics.sum(s, axis=axis, keepdims=keepdims))
     elif isinstance(ord, str):
-        raise ValueError("Norm order {} is invalid for vectors".format(ord))
+        raise ValueError(f"Norm order {ord} is invalid for vectors")
     else:
         ret = arithmetics.pow(rounding.abs(x), ord)
-        ret = arithmetics.sum(ret, axis=axis, keepdim=keepdims)
+        ret = arithmetics.sum(ret, axis=axis, keepdims=keepdims)
         ret = arithmetics.pow(ret, 1.0 / ord)
         return ret
```

### Comparing `heat-1.2.2/heat/core/linalg/qr.py` & `heat-1.3.0/heat/core/linalg/qr.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,39 +72,37 @@
     [0/1] True
     [1/1] True
     """
     if not isinstance(a, DNDarray):
         raise TypeError("'a' must be a DNDarray")
     if not isinstance(tiles_per_proc, (int, torch.Tensor)):
         raise TypeError(
-            "tiles_per_proc must be an int or a torch.Tensor, "
-            "currently {}".format(type(tiles_per_proc))
+            f"tiles_per_proc must be an int or a torch.Tensor, currently {type(tiles_per_proc)}"
         )
     if not isinstance(calc_q, bool):
-        raise TypeError("calc_q must be a bool, currently {}".format(type(calc_q)))
+        raise TypeError(f"calc_q must be a bool, currently {type(calc_q)}")
     if not isinstance(overwrite_a, bool):
-        raise TypeError("overwrite_a must be a bool, currently {}".format(type(overwrite_a)))
+        raise TypeError(f"overwrite_a must be a bool, currently {type(overwrite_a)}")
     if isinstance(tiles_per_proc, torch.Tensor):
         raise ValueError(
-            "tiles_per_proc must be a single element torch.Tenor or int, "
-            "currently has {} entries".format(tiles_per_proc.numel())
+            f"tiles_per_proc must be a single element torch.Tenor or int, currently has {tiles_per_proc.numel()} entries"
         )
     if len(a.shape) != 2:
         raise ValueError("Array 'a' must be 2 dimensional")
 
     QR = collections.namedtuple("QR", "Q, R")
 
     if a.split is None:
         try:
             q, r = torch.linalg.qr(a.larray, mode="complete")
         except AttributeError:
             q, r = a.larray.qr(some=False)
 
-        q = factories.array(q, device=a.device)
-        r = factories.array(r, device=a.device)
+        q = factories.array(q, device=a.device, comm=a.comm)
+        r = factories.array(r, device=a.device, comm=a.comm)
         ret = QR(q if calc_q else None, r)
         return ret
     # =============================== Prep work ====================================================
     r = a if overwrite_a else a.copy()
     # r.create_square_diag_tiles(tiles_per_proc=tiles_per_proc)
     r_tiles = SquareDiagTiles(arr=r, tiles_per_proc=tiles_per_proc)
     tile_columns = r_tiles.tile_columns
@@ -247,18 +245,15 @@
         # todo: modify this so that it will get what is needed from the process,
         #  instead of gathering all the qs
         top_left = lp_q[: base_size[0], : base_size[0]]
         top_right = lp_q[: base_size[0], base_size[0] :]
         bottom_left = lp_q[base_size[0] :, : base_size[0]]
         bottom_right = lp_q[base_size[0] :, base_size[0] :]
         # need to adjust the keys to be the global row
-        if diag_proc == r0:
-            col1 = col
-        else:
-            col1 = proc_tile_start[r0].item()
+        col1 = col if diag_proc == r0 else proc_tile_start[r0].item()
         col2 = proc_tile_start[r1].item()
         # col0 and col1 are the columns numbers
         # r0 and r1 are the ranks
         jdim = (col1, col1)
         kdim = (col1, col2)
         ldim = (col2, col1)
         mdim = (col2, col2)
@@ -367,33 +362,30 @@
         loc_rest = torch.matmul(q1.T, base_rest)
         r_tiles.local_set(key=(slice(lcl_tile_row, None), slice(col_num + 1, None)), value=loc_rest)
     # --------------- global QR calc (binary merge) -------------------------------------
     rem1 = None
     rem2 = None
     offset = not_completed_prs[0]
     loop_size_remaining = not_completed_prs.clone()
-    completed = False if loop_size_remaining.size()[0] > 1 else True
+    completed = bool(loop_size_remaining.size()[0] <= 1)
     procs_remaining = loop_size_remaining.size()[0]
     loop = 0
     while not completed:
         if procs_remaining % 2 == 1:
             # if the number of processes active is odd need to save the remainders
             if rem1 is None:
                 rem1 = loop_size_remaining[-1]
                 loop_size_remaining = loop_size_remaining[:-1]
             elif rem2 is None:
                 rem2 = loop_size_remaining[-1]
                 loop_size_remaining = loop_size_remaining[:-1]
         if rank not in loop_size_remaining and rank not in [rem1, rem2]:
             break  # if the rank is done then exit the loop
         # send the data to the corresponding processes
-        try:
-            half_prs_rem = torch.div(procs_remaining, 2, rounding_mode="floor")
-        except TypeError:  # torch 1.7 version
-            half_prs_rem = torch.floor_divide(procs_remaining, 2)
+        half_prs_rem = torch.div(procs_remaining, 2, rounding_mode="floor")
 
         zipped = zip(
             loop_size_remaining.flatten()[:half_prs_rem],
             loop_size_remaining.flatten()[half_prs_rem:],
         )
         for pr in zipped:
             pr0, pr1 = int(pr[0].item()), int(pr[1].item())
```

### Comparing `heat-1.2.2/heat/core/linalg/solver.py` & `heat-1.3.0/heat/core/linalg/solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,39 +24,37 @@
     x0 : DNDarray
         Arbitrary 1D starting vector
     out : DNDarray, optional
         Output Vector
     """
     if not isinstance(A, DNDarray) or not isinstance(b, DNDarray) or not isinstance(x0, DNDarray):
         raise TypeError(
-            "A, b and x0 need to be of type ht.DNDarray, but were {}, {}, {}".format(
-                type(A), type(b), type(x0)
-            )
+            f"A, b and x0 need to be of type ht.DNDarray, but were {type(A)}, {type(b)}, {type(x0)}"
         )
 
-    if not A.ndim == 2:
+    if A.ndim != 2:
         raise RuntimeError("A needs to be a 2D matrix")
-    if not b.ndim == 1:
+    if b.ndim != 1:
         raise RuntimeError("b needs to be a 1D vector")
-    if not x0.ndim == 1:
+    if x0.ndim != 1:
         raise RuntimeError("c needs to be a 1D vector")
 
     r = b - ht.matmul(A, x0)
     p = r
     rsold = ht.matmul(r, r)
     x = x0
 
     for i in range(len(b)):
         Ap = ht.matmul(A, p)
         alpha = rsold / ht.matmul(p, Ap)
         x = x + alpha * p
         r = r - alpha * Ap
         rsnew = ht.matmul(r, r)
         if ht.sqrt(rsnew).item() < 1e-10:
-            print("Residual reaches tolerance in it = {}".format(i))
+            print(f"Residual reaches tolerance in it = {i}")
             if out is not None:
                 out = x
                 return out
             return x
         p = r + ((rsnew / rsold) * p)
         rsold = rsnew
 
@@ -94,21 +92,21 @@
         1D starting vector of Euclidean norm 1. If not provided, a random vector will be used to start the algorithm
     V_out : DNDarray, optional
         Output Matrix for the Krylow vectors, Shape = (n, m), dtype=A.dtype, must be initialized to zero
     T_out : DNDarray, optional
         Output Matrix for the Tridiagonal matrix, Shape = (m, m), must be initialized to zero
     """
     if not isinstance(A, DNDarray):
-        raise TypeError("A needs to be of type ht.dndarray, but was {}".format(type(A)))
-    if not (A.ndim == 2):
+        raise TypeError(f"A needs to be of type ht.dndarray, but was {type(A)}")
+    if A.ndim != 2:
         raise RuntimeError("A needs to be a 2D matrix")
     if A.dtype is ht.int32 or A.dtype is ht.int64:
-        raise TypeError("A can be float or complex, got {}".format(A.dtype))
+        raise TypeError(f"A can be float or complex, got {A.dtype}")
     if not isinstance(m, (int, float)):
-        raise TypeError("m must be int, got {}".format(type(m)))
+        raise TypeError(f"m must be int, got {type(m)}")
 
     n, column = A.shape
     if n != column:
         raise TypeError("Input Matrix A needs to be symmetric positive-definite.")
 
     # output data types: T is always Real
     A_is_complex = A.dtype is ht.complex128 or A.dtype is ht.complex64
@@ -157,17 +155,16 @@
     if A_is_complex:
         if v0 is None:
             vr = (
                 ht.random.rand(n, split=V.split, dtype=T_dtype, device=V.device, comm=V.comm)
                 + ht.random.rand(n, split=V.split, dtype=T_dtype, device=V.device, comm=V.comm) * 1j
             )
             v0 = vr / ht.norm(vr)
-        else:
-            if v0.split != V.split:
-                v0.resplit_(axis=V.split)
+        elif v0.split != V.split:
+            v0.resplit_(axis=V.split)
         # # 0th iteration
         # # vector v0 has Euclidean norm = 1
         w = ht.matmul(A, v0)
         alpha = ht.dot(ht.conj(w).T, v0)
         w = w - alpha * v0
         T[0, 0] = alpha.real
         V[:, 0] = v0
@@ -214,17 +211,16 @@
             T[i, i - 1] = beta.real
             T[i, i] = alpha.real
             V[:, i] = vi
     else:
         if v0 is None:
             vr = ht.random.rand(n, split=V.split, dtype=T_dtype, device=V.device, comm=V.comm)
             v0 = vr / ht.norm(vr)
-        else:
-            if v0.split != V.split:
-                v0.resplit_(axis=V.split)
+        elif v0.split != V.split:
+            v0.resplit_(axis=V.split)
         # # 0th iteration
         # # vector v0 has Euclidean norm = 1
         w = ht.matmul(A, v0)
         alpha = ht.dot(w, v0)
         w = w - alpha * v0
         T[0, 0] = alpha
         V[:, 0] = v0
```

### Comparing `heat-1.2.2/heat/core/logical.py` & `heat-1.3.0/heat/core/logical.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ]
 
 
 def all(
     x: DNDarray,
     axis: Union[int, Tuple[int], None] = None,
     out: Optional[DNDarray] = None,
-    keepdim: bool = False,
+    keepdims: bool = False,
 ) -> Union[DNDarray, bool]:
     """
     Test whether all array elements along a given axis evaluate to ``True``.
     A new boolean or :class:`~heat.core.dndarray.DNDarray` is returned unless out is specified, in which case a
     reference to ``out`` is returned.
 
     Parameters
@@ -53,15 +53,15 @@
     axis : None or int or Tuple[int,...], optional
         Axis or axes along which a logical AND reduction is performed. The default (``axis=None``) is to perform a
         logical AND over all the dimensions of the input array. ``axis`` may be negative, in which case it counts
         from the last to the first axis.
     out : DNDarray, optional
         Alternate output array in which to place the result. It must have the same shape as the expected output
         and its type is preserved.
-    keepdim : bool, optional
+    keepdims : bool, optional
         If this is set to ``True``, the axes which are reduced are left in the result as dimensions with size one.
         With this option, the result will broadcast correctly against the original array.
 
     Examples
     ---------
     >>> x = ht.random.randn(4, 5)
     >>> x
@@ -87,25 +87,25 @@
     >>> out
     DNDarray([False, False, False, False, False], dtype=ht.float32, device=cpu:0, split=None)
     """
 
     def local_all(t, *args, **kwargs):
         return torch.all(t != 0, *args, **kwargs)
 
-    if keepdim and axis is None:
+    if keepdims and axis is None:
         axis = tuple(range(x.ndim))
 
     return _operations.__reduce_op(
-        x, local_all, MPI.LAND, axis=axis, out=out, neutral=1, keepdim=keepdim
+        x, local_all, MPI.LAND, axis=axis, out=out, neutral=1, keepdims=keepdims
     )
 
 
 DNDarray.all: Callable[
     [Union[int, Tuple[int], None], Optional[DNDarray], bool], Union[DNDarray, bool]
-] = lambda self, axis=None, out=None, keepdim=False: all(self, axis, out, keepdim)
+] = lambda self, axis=None, out=None, keepdims=False: all(self, axis, out, keepdims)
 DNDarray.all.__doc__ = all.__doc__
 
 
 def allclose(
     x: DNDarray, y: DNDarray, rtol: float = 1e-05, atol: float = 1e-08, equal_nan: bool = False
 ) -> bool:
     """
@@ -166,15 +166,15 @@
 ] = lambda self, other, rtol=1e-05, atol=1e-08, equal_nan=False: allclose(
     self, other, rtol, atol, equal_nan
 )
 DNDarray.allclose.__doc__ = all.__doc__
 
 
 def any(
-    x, axis: Optional[int] = None, out: Optional[DNDarray] = None, keepdim: bool = False
+    x, axis: Optional[int] = None, out: Optional[DNDarray] = None, keepdims: bool = False
 ) -> DNDarray:
     """
     Returns a :class:`~heat.core.dndarray.DNDarray` containing the result of the test whether any array elements along a
     given axis evaluate to ``True``.
     The returning array is one dimensional unless axis is not ``None``.
 
     Parameters
@@ -183,15 +183,15 @@
         Input tensor
     axis : int, optional
         Axis along which a logic OR reduction is performed. With ``axis=None``, the logical OR is performed over all
         dimensions of the array.
     out : DNDarray, optional
         Alternative output tensor in which to place the result. It must have the same shape as the expected output.
         The output is a array with ``datatype=bool``.
-    keepdim : bool, optional
+    keepdims : bool, optional
         If this is set to ``True``, the axes which are reduced are left in the result as dimensions with size one.
         With this option, the result will broadcast correctly against the original array.
 
     Examples
     ---------
     >>> x = ht.float32([[0.3, 0, 0.5]])
     >>> x.any()
@@ -207,25 +207,25 @@
     >>> res
     DNDarray([False, False,  True], dtype=ht.bool, device=cpu:0, split=None)
     """
 
     def local_any(t, *args, **kwargs):
         return torch.any(t != 0, *args, **kwargs)
 
-    if keepdim and axis is None:
+    if keepdims and axis is None:
         axis = tuple(range(x.ndim))
 
     return _operations.__reduce_op(
-        x, local_any, MPI.LOR, axis=axis, out=out, neutral=0, keepdim=keepdim
+        x, local_any, MPI.LOR, axis=axis, out=out, neutral=0, keepdims=keepdims
     )
 
 
 DNDarray.any: Callable[
     [DNDarray, Optional[int], Optional[DNDarray], bool], DNDarray
-] = lambda self, axis=None, out=None, keepdim=False: any(self, axis, out, keepdim)
+] = lambda self, axis=None, out=None, keepdims=False: any(self, axis, out, keepdims)
 DNDarray.any.__doc__ = any.__doc__
 
 
 def isclose(
     x: DNDarray, y: DNDarray, rtol: float = 1e-05, atol: float = 1e-08, equal_nan: bool = False
 ) -> DNDarray:
     """
@@ -501,15 +501,15 @@
         Raises
         ------
         TypeError
             If ``x`` or ``y`` are not
         """
         if not isinstance(x, DNDarray):
             if np.ndim(x) != 0:
-                raise TypeError("Expected DNDarray or numeric scalar, input was {}".format(type(x)))
+                raise TypeError(f"Expected DNDarray or numeric scalar, input was {type(x)}")
 
             dtype = getattr(x, "dtype", float)
             device = getattr(y, "device", None)
             x = factories.array(x, dtype=dtype, device=device)
 
         return x
```

### Comparing `heat-1.2.2/heat/core/manipulations.py` & `heat-1.3.0/heat/core/manipulations.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from . import stride_tricks
 from . import tiling
 from . import types
 from . import _operations
 
 __all__ = [
     "balance",
+    "broadcast_arrays",
+    "broadcast_to",
     "column_stack",
     "concatenate",
     "diag",
     "diagonal",
     "dsplit",
     "expand_dims",
     "flatten",
@@ -70,29 +72,182 @@
     array : DNDarray
         the DNDarray to be balanced
     copy : bool, optional
         if the DNDarray should be copied before being balanced. If false (default) this will balance
         the original array and return that array. Otherwise (true), a balanced copy of the array
         will be returned.
         Default: False
-
-    Returns
-    -------
-    balanced : DNDarray
-        The balanced DNDarray
     """
     cpy = array.copy() if copy else array
     cpy.balance_()
     return cpy
 
 
 DNDarray.balance = lambda self, copy=False: balance(self, copy)
 DNDarray.balance.__doc__ = balance.__doc__
 
 
+def broadcast_arrays(*arrays: DNDarray) -> List[DNDarray]:
+    """
+    Broadcasts one or more arrays against one another. Returns the broadcasted arrays, distributed along the split dimension of the first array in the list. If the first array is not distributed, the output will not be distributed.
+
+    Parameters
+    ----------
+    arrays : DNDarray
+        An arbitrary number of to-be broadcasted ``DNDarray``s.
+
+    Notes
+    -----
+    Broadcasted arrays are a view of the original arrays if possible, otherwise a copy is made.
+
+    Examples
+    --------
+    >>> import heat as ht
+    >>> a = ht.ones((100, 10), split=0)
+    >>> b = ht.ones((10,), split=None)
+    >>> c = ht.ones((1, 10), split=1)
+    >>> d, e, f = ht.broadcast_arrays(a, b, c)
+    >>> d.shape
+    (100, 10)
+    >>> e.shape
+    (100, 10)
+    >>> f.shape
+    (100, 10)
+    >>> d.split
+    0
+    >>> e.split
+    0
+    >>> f.split
+    0
+    """
+    if len(arrays) <= 1:
+        return arrays
+
+    try:
+        arrays = sanitation.sanitize_distribution(*arrays, target=arrays[0])
+        output_split, output_comm, output_balanced = (
+            arrays[0].split,
+            arrays[0].comm,
+            arrays[0].balanced,
+        )
+    except NotImplementedError as e:
+        raise ValueError(e)
+
+    gshapes = []
+    t_arrays = []
+    for array in arrays:
+        # extract global shapes
+        gshapes.append(array.gshape)
+        # extract local torch tensors
+        t_arrays.append(array.larray)
+    t_arrays = tuple(t_arrays)
+
+    # broadcast the global shapes
+    try:
+        output_shape = tuple(torch.broadcast_shapes(*gshapes))
+    except RuntimeError:
+        raise ValueError(
+            f"Shape mismatch: objects cannot be broadcast to a single shape. Original shapes: {gshapes}"
+        )
+
+    # broadcast the local torch tensors: this is a view of the original data
+    broadcasted = torch.broadcast_tensors(*t_arrays)
+
+    out = []
+    for i in range(len(broadcasted)):
+        out.append(
+            DNDarray(
+                broadcasted[i],
+                gshape=output_shape,
+                dtype=arrays[i].dtype,
+                split=output_split,
+                device=arrays[i].device,
+                comm=output_comm,
+                balanced=output_balanced,
+            )
+        )
+
+    return out
+
+
+def broadcast_to(x: DNDarray, shape: Tuple[int, ...]) -> DNDarray:
+    """
+    Broadcasts an array to a specified shape. Returns a view of ``x`` if ``x`` is not distributed, otherwise it returns a broadcasted, distributed, load-balanced copy of ``x``.
+
+    Parameters
+    ----------
+    x : DNDarray
+        `DNDarray` to broadcast.
+    shape : Tuple[int, ...]
+        Array shape. Must be compatible with ``x``.
+
+    Raises
+    ------
+    ValueError
+        If the array is not compatible with the new shape according to PyTorch's broadcasting rules.
+
+    Examples
+    --------
+    >>> import heat as ht
+    >>> a = ht.arange(100, split=0)
+    >>> b = ht.broadcast_to(a, (10,100))
+    >>> b.shape
+    (10, 100)
+    >>> b.split
+    1
+    >>> c = ht.broadcast_to(a, (100, 10))
+    ValueError: Shape mismatch: object cannot be broadcast to the given shape. Original shape: (100,), target shape: (100, 10)
+    """
+    sanitation.sanitize_in(x)
+
+    # figure out the output split axis via dndarray.__torch_proxy__ and named tensors functionality
+    torch_proxy = x.__torch_proxy__()
+    split_tags = [None] * x.ndim
+    if x.split is not None:
+        split_tags[x.split] = "split"
+        torch_proxy = torch.tensor(torch_proxy, names=split_tags)
+        try:
+            torch_proxy = torch_proxy.broadcast_to(shape)
+        except RuntimeError:
+            raise ValueError(
+                f"Shape mismatch: object cannot be broadcast to the given shape. Original shape: {x.shape}, target shape: {shape}"
+            )
+        output_split = torch_proxy.names.index("split")
+    else:
+        try:
+            torch_proxy = torch_proxy.broadcast_to(shape)
+        except RuntimeError:
+            raise ValueError(
+                f"Shape mismatch: object cannot be broadcast to the given shape. Original shape: {x.shape}, target shape: {shape}"
+            )
+        output_split = None
+
+    if not x.is_distributed():
+        # return a view of the input data
+        broadcasted = DNDarray(
+            x.larray.broadcast_to(shape),
+            gshape=shape,
+            dtype=x.dtype,
+            split=output_split,
+            device=x.device,
+            comm=x.comm,
+            balanced=True,
+        )
+    else:
+        # input is distributed, return a broadcasted copy of input
+        # exploit binary operations broadcasting
+        broadcasted = factories.zeros(
+            shape, dtype=x.dtype, split=output_split, device=x.device, comm=x.comm
+        )
+        broadcasted += x
+        del x
+
+    return broadcasted
+
+
 def column_stack(arrays: Sequence[DNDarray, ...]) -> DNDarray:
     """
     Stack 1-D or 2-D `DNDarray`s as columns into a 2-D `DNDarray`.
     If the input arrays are 1-D, they will be stacked as columns. If they are 2-D,
     they will be concatenated along the second axis.
 
     Parameters
@@ -269,24 +424,23 @@
             res = concatenate((res, arrays[a]), axis=axis)
         return res
 
     # unpack the arrays
     arr0, arr1 = arrays
 
     if not isinstance(axis, int):
-        raise TypeError("axis must be an integer, currently: {}".format(type(axis)))
+        raise TypeError(f"axis must be an integer, currently: {type(axis)}")
     axis = stride_tricks.sanitize_axis(arr0.gshape, axis)
 
     if arr0.ndim != arr1.ndim:
         raise ValueError("DNDarrays must have the same number of dimensions")
 
-    if not all([arr0.gshape[i] == arr1.gshape[i] for i in range(len(arr0.gshape)) if i != axis]):
+    if any(arr0.gshape[i] != arr1.gshape[i] for i in range(len(arr0.gshape)) if i != axis):
         raise ValueError(
-            "Arrays cannot be concatenated, shapes must be the same in every axis "
-            "except the selected axis: {}, {}".format(arr0.gshape, arr1.gshape)
+            f"Arrays cannot be concatenated, shapes must be the same in every axis except the selected axis: {arr0.gshape}, {arr1.gshape}"
         )
 
     # different communicators may not be concatenated
     if arr0.comm != arr1.comm:
         raise RuntimeError("Communicators of passed arrays mismatch.")
 
     # identify common data type
@@ -301,34 +455,31 @@
     if s0 is None and s1 is None:
         return factories.array(
             torch.cat((arr0.larray, arr1.larray), dim=axis), device=arr0.device, comm=arr0.comm
         )
 
     # non-matching splits when both arrays are split
     elif s0 != s1 and all([s is not None for s in [s0, s1]]):
-        raise RuntimeError(
-            "DNDarrays given have differing split axes, arr0 {} arr1 {}".format(s0, s1)
-        )
+        raise RuntimeError(f"DNDarrays given have differing split axes, arr0 {s0} arr1 {s1}")
 
-    # unsplit and split array
     elif (s0 is None and s1 != axis) or (s1 is None and s0 != axis):
         _, _, arr0_slice = arr1.comm.chunk(arr0.shape, arr1.split)
         _, _, arr1_slice = arr0.comm.chunk(arr1.shape, arr0.split)
         out = factories.array(
             torch.cat((arr0.larray[arr0_slice], arr1.larray[arr1_slice]), dim=axis),
             dtype=out_dtype,
             is_split=s1 if s1 is not None else s0,
             device=arr1.device,
             comm=arr0.comm,
         )
 
         return out
 
-    elif s0 == s1 or any([s is None for s in [s0, s1]]):
-        if s0 != axis and all([s is not None for s in [s0, s1]]):
+    elif s0 == s1 or any(s is None for s in [s0, s1]):
+        if s0 != axis and all(s is not None for s in [s0, s1]):
             # the axis is different than the split axis, this case can be easily implemented
             # torch cat arrays together and return a new array that is_split
 
             out = factories.array(
                 torch.cat((arr0.larray, arr1.larray), dim=axis),
                 dtype=out_dtype,
                 is_split=s0,
@@ -646,19 +797,21 @@
         split = a.split - 1
     elif x < y < a.split:
         split = a.split - 2
     else:
         split = len(shape) - 1
 
     if a.split is None or a.split not in (dim1, dim2):
-        result = torch.diagonal(a.larray, offset=offset, dim1=dim1, dim2=dim2)
+        result = torch.diagonal(a.larray, offset=offset, dim1=dim1, dim2=dim2).contiguous()
     else:
         vz = 1 if a.split == dim1 else -1
         off, _, _ = a.comm.chunk(a.shape, a.split)
-        result = torch.diagonal(a.larray, offset=offset + vz * off, dim1=dim1, dim2=dim2)
+        result = torch.diagonal(
+            a.larray, offset=offset + vz * off, dim1=dim1, dim2=dim2
+        ).contiguous()
     return factories.array(result, dtype=a.dtype, is_split=split, device=a.device, comm=a.comm)
 
 
 def dsplit(x: Sequence[DNDarray, ...], indices_or_sections: Iterable) -> List[DNDarray, ...]:
     """
     Split array into multiple sub-DNDarrays along the 3rd axis (depth).
     Returns a list of sub-DNDarrays as copies of parts of `x`.
@@ -1223,39 +1376,35 @@
                [ 0,  0,  0,  0,  0,  0,  0]]], dtype=ht.int64, device=cpu:0, split=0)
     """
     # early out if pad width is 0
     if pad_width == 0:
         return array
 
     if not isinstance(array, DNDarray):
-        raise TypeError("expected array to be a ht.DNDarray, but was {}".format(type(array)))
+        raise TypeError(f"expected array to be a ht.DNDarray, but was {type(array)}")
 
     if not isinstance(mode, str):
-        raise TypeError("expected mode to be a string, but was {}".format(type(mode)))
+        raise TypeError(f"expected mode to be a string, but was {type(mode)}")
 
     # shortcut int for all dimensions
     if isinstance(pad_width, int):
         pad = (pad_width,) * 2 * len(array.shape)
 
     elif not isinstance(pad_width, (tuple, list)):
         raise TypeError(
-            "expected pad_width to be an integer or a sequence (tuple or list), but was {}".format(
-                type(pad_width)
-            )
+            f"expected pad_width to be an integer or a sequence (tuple or list), but was {type(pad_width)}"
         )
 
     # shortcut one sequence within a sequence for all dimensions - ((before,after), ) = pad_width
     elif len(pad_width) == 1:
         if isinstance(pad_width[0], int):
             pad = (pad_width[0],) * 2 * len(array.shape)
-        elif not (isinstance(pad_width[0], tuple) or isinstance(pad_width[0], list)):
+        elif not (isinstance(pad_width[0], (tuple, list))):
             raise TypeError(
-                "For shortcut option '1 sequence for all dimensions', expected element within pad_width to be a tuple or list, but was {}".format(
-                    type(pad_width[0])
-                )
+                f"For shortcut option '1 sequence for all dimensions', expected element within pad_width to be a tuple or list, but was {type(pad_width[0])}"
             )
         elif len(pad_width[0]) == 2:
             pad = pad_width[0] * len(array.shape)
         else:
             raise ValueError(
                 f"Pad_width {pad_width} invalid.\n Apart from shortcut options (--> documentation), "
                 "each sequence within pad_width must contain 2 elements."
@@ -1263,23 +1412,20 @@
     # shortcut - one sequence for all dimensions - (before,after) = pad_width
     elif len(pad_width) == 2 and isinstance(pad_width[0], int) and isinstance(pad_width[1], int):
         pad_width = tuple(pad_width)
         pad = pad_width * len(array.shape)
 
     # no shortcut - padding of various dimensions
     else:
-        if any(
-            not (isinstance(pad_tuple, tuple) or isinstance(pad_tuple, list))
-            for pad_tuple in pad_width
-        ):
+        if any(not (isinstance(pad_tuple, (tuple, list))) for pad_tuple in pad_width):
             raise TypeError(
                 f"Invalid type for pad_width {pad_width}.\nApart from shortcut options (--> documentation),"
                 "pad_width has to be a sequence of (2 elements) sequences (sequence=tuple or list)."
             )
-        pad = tuple()
+        pad = ()
         # Transform numpy pad_width to torch pad (--> one tuple containing all padding spans)
         for pad_tuple in pad_width:
             if isinstance(pad_tuple, list):
                 pad_tuple = tuple(pad_tuple)
             pad = pad_tuple + pad
 
         if len(pad) % 2 != 0:
@@ -1292,18 +1438,18 @@
             raise ValueError(
                 f"Not enough dimensions to pad.\n"
                 f"Padding a {len(array.shape)}-dimensional tensor for {len(pad) // 2}"
                 f" dimensions is not possible."
             )
 
     # value_tuple = all padding values stored in 1 tuple
-    if isinstance(constant_values, tuple) or isinstance(constant_values, list):
-        value_tuple = tuple()
+    if isinstance(constant_values, (tuple, list)):
+        value_tuple = ()
         # sequences for each dimension defined within one sequence
-        if isinstance(constant_values[0], tuple) or isinstance(constant_values[0], list):
+        if isinstance(constant_values[0], (tuple, list)):
             # one sequence for all dimensions - values = ((before, after),)
             if len(constant_values) == 1:
                 value_tuple = constant_values[0] * (len(pad) // 2)
             else:
                 for value_pair in constant_values:
                     if isinstance(value_pair, tuple):
                         pass
@@ -1530,15 +1676,15 @@
         Units are ``[rank, target lshape]``.
         Note: the only important parts of the target map are the values along the split axis,
         values which are not along this axis are there to mimic the shape of the ``lshape_map``.
 
     Examples
     --------
     >>> st = ht.ones((50, 81, 67), split=2)
-    >>> target_map = torch.zeros((st.comm.size, 3), dtype=torch.int)
+    >>> target_map = torch.zeros((st.comm.size, 3), dtype=torch.int64)
     >>> target_map[0, 2] = 67
     >>> print(target_map)
     [0/2] tensor([[ 0,  0, 67],
     [0/2]         [ 0,  0,  0],
     [0/2]         [ 0,  0,  0]], dtype=torch.int32)
     [1/2] tensor([[ 0,  0, 67],
     [1/2]         [ 0,  0,  0],
@@ -1609,36 +1755,30 @@
     if not isinstance(a, DNDarray):
         if isinstance(a, (int, float)):
             a = factories.array([a])
         elif isinstance(a, (tuple, list, np.ndarray)):
             a = factories.array(a)
         else:
             raise TypeError(
-                "`a` must be a ht.DNDarray, np.ndarray, list, tuple, integer, or float, currently: {}".format(
-                    type(a)
-                )
+                f"`a` must be a ht.DNDarray, np.ndarray, list, tuple, integer, or float, currently: {type(a)}"
             )
 
     # sanitation `axis`
     if axis is not None and not isinstance(axis, int):
-        raise TypeError("`axis` must be an integer or None, currently: {}".format(type(axis)))
+        raise TypeError(f"`axis` must be an integer or None, currently: {type(axis)}")
 
     if axis is not None and (axis >= len(a.shape) or axis < 0):
         raise ValueError(
-            "Invalid input for `axis`. Value has to be either None or between 0 and {}, not {}.".format(
-                len(a.shape) - 1, axis
-            )
+            f"Invalid input for `axis`. Value has to be either None or between 0 and {len(a.shape) - 1}, not {axis}."
         )
 
     # sanitation `repeats`
     if not isinstance(repeats, (int, list, tuple, np.ndarray, DNDarray)):
         raise TypeError(
-            "`repeats` must be an integer, list, tuple, np.ndarray or ht.DNDarray of integers, currently: {}".format(
-                type(repeats)
-            )
+            f"`repeats` must be an integer, list, tuple, np.ndarray or ht.DNDarray of integers, currently: {type(repeats)}"
         )
 
     # no broadcast implied
     if not isinstance(repeats, int):
         # make sure everything inside `repeats` is int
         if isinstance(repeats, DNDarray):
             if repeats.dtype == types.int64:
@@ -1649,59 +1789,53 @@
                     dtype=types.int64,
                     is_split=repeats.split,
                     device=repeats.device,
                     comm=repeats.comm,
                 )
             else:
                 raise TypeError(
-                    "Invalid dtype for ht.DNDarray `repeats`. Has to be integer,"
-                    " but was {}".format(repeats.dtype)
+                    f"Invalid dtype for ht.DNDarray `repeats`. Has to be integer, but was {repeats.dtype}"
                 )
         elif isinstance(repeats, np.ndarray):
             if not types.can_cast(repeats.dtype.type, types.int64):
                 raise TypeError(
-                    "Invalid dtype for np.ndarray `repeats`. Has to be integer,"
-                    " but was {}".format(repeats.dtype.type)
+                    f"Invalid dtype for np.ndarray `repeats`. Has to be integer, but was {repeats.dtype.type}"
                 )
             repeats = factories.array(
                 repeats, dtype=types.int64, is_split=None, device=a.device, comm=a.comm
             )
-        # invalid list/tuple
         elif not all(isinstance(r, int) for r in repeats):
             raise TypeError(
                 "Invalid type within `repeats`. All components of `repeats` must be integers."
             )
-        # valid list/tuple
         else:
             repeats = factories.array(
                 repeats, dtype=types.int64, is_split=None, device=a.device, comm=a.comm
             )
 
         # check `repeats` is not empty
         if repeats.gnumel == 0:
             raise ValueError("Invalid input for `repeats`. `repeats` must contain data.")
 
         # check `repeats` is 1-dimensional
         if len(repeats.shape) != 1:
             raise ValueError(
-                "Invalid input for `repeats`. `repeats` must be a 1d-object or integer, but "
-                "was {}-dimensional.".format(len(repeats.shape))
+                f"Invalid input for `repeats`. `repeats` must be a 1d-object or integer, but was {len(repeats.shape)}-dimensional."
             )
 
     # start of algorithm
 
     if 0 in a.gshape:
         return a
 
     # Broadcast (via int or 1-element DNDarray)
     if isinstance(repeats, int) or repeats.gnumel == 1:
         if axis is None and a.split is not None and a.split != 0:
             warnings.warn(
-                "If axis is None, `a` has to be split along axis 0 (not {}) if distributed.\n`a` will be "
-                "copied with new split axis 0.".format(a.split)
+                f"If axis is None, `a` has to be split along axis 0 (not {a.split}) if distributed.\n`a` will be copied with new split axis 0."
             )
             a = resplit(a, 0)
         if isinstance(repeats, int):
             repeated_array_torch = torch.repeat_interleave(a._DNDarray__array, repeats, axis)
         else:
             if repeats.split is not None:
                 warnings.warn(
@@ -1717,98 +1851,90 @@
     else:
         # check if the data chunks of `repeats` and/or `a` have to be (re)distributed before call of torch function.
 
         # UNDISTRIBUTED CASE (a not distributed)
         if a.split is None:
             if repeats.split is not None:
                 warnings.warn(
-                    "If `a` is undistributed, `repeats` also has to be undistributed (not split along axis {}).\n`repeats` will be copied "
-                    "with new split axis None.".format(repeats.split)
+                    f"If `a` is undistributed, `repeats` also has to be undistributed (not split along axis {repeats.split}).\n`repeats` will be copied "
+                    "with new split axis None."
                 )
                 repeats = resplit(repeats, None)
 
             # Check correct input
             if axis is None:
                 # check matching shapes (repetition defined for every element)
                 if a.gnumel != repeats.gnumel:
                     raise ValueError(
-                        "Invalid input. Sizes of flattened `a` ({}) and `repeats` ({}) are not same. "
-                        "Please revise your definition specifying repetitions for all elements "
-                        "of the DNDarray `a` or replace repeats with a single"
-                        " scalar.".format(a.gnumel, repeats.gnumel)
+                        f"Invalid input. Sizes of flattened `a` ({a.gnumel}) and `repeats` ({repeats.gnumel}) are not same. "
+                        "Please revise your definition specifying repetitions for all elements of the DNDarray `a` "
+                        "or replace repeats with a single scalar."
                     )
             # axis is not None
             elif a.lshape[axis] != repeats.lnumel:
                 raise ValueError(
-                    "Invalid input. Amount of elements of `repeats` ({}) and of `a` in the specified axis ({}) "
+                    f"Invalid input. Amount of elements of `repeats` ({repeats.lnumel}) and of `a` in the specified axis ({a.lshape[axis]}) "
                     "are not the same. Please revise your definition specifying repetitions for all elements "
-                    "of the DNDarray `a` or replace `repeats` with a single scalar".format(
-                        repeats.lnumel, a.lshape[axis]
-                    )
+                    "of the DNDarray `a` or replace `repeats` with a single scalar"
                 )
         # DISTRIBUTED CASE (a distributed)
-        else:
-            if axis is None:
-                if a.gnumel != repeats.gnumel:
-                    raise ValueError(
-                        "Invalid input. Sizes of flattened `a` ({}) and `repeats` ({}) are not same. "
-                        "Please revise your definition specifying repetitions for all elements "
-                        "of the DNDarray `a` or replace `repeats` with a single"
-                        " scalar.".format(a.gnumel, repeats.gnumel)
-                    )
+        elif axis is None:
+            if a.gnumel != repeats.gnumel:
+                raise ValueError(
+                    f"Invalid input. Sizes of flattened `a` ({a.gnumel}) and `repeats` ({repeats.gnumel}) are not same. "
+                    "Please revise your definition specifying repetitions for all elements of the DNDarray `a` "
+                    "or replace `repeats` with a single scalar."
+                )
 
-                if a.split != 0:
-                    warnings.warn(
-                        "If `axis` is None, `a` has to be split along axis 0 (not {}) if distributed.\n`a` will be copied"
-                        " with new split axis 0.".format(a.split)
-                    )
-                    a = resplit(a, 0)
+            if a.split != 0:
+                warnings.warn(
+                    f"If `axis` is None, `a` has to be split along axis 0 (not {a.split}) if distributed.\n`a` will be copied "
+                    "with new split axis 0."
+                )
+                a = resplit(a, 0)
 
-                repeats = repeats.reshape(a.gshape)
-                if repeats.split != 0:
-                    warnings.warn(
-                        "If `axis` is None, `repeats` has to be split along axis 0 (not {}) if distributed.\n`repeats` will be copied"
-                        " with new split axis 0.".format(repeats.split)
-                    )
-                    repeats = resplit(repeats, 0)
-                flatten_repeats_t = torch.flatten(repeats._DNDarray__array)
-                repeats = factories.array(
-                    flatten_repeats_t,
-                    is_split=repeats.split,
-                    device=repeats.device,
-                    comm=repeats.comm,
+            repeats = repeats.reshape(a.gshape)
+            if repeats.split != 0:
+                warnings.warn(
+                    f"If `axis` is None, `repeats` has to be split along axis 0 (not {repeats.split}) if distributed.\n`repeats` will be copied "
+                    "with new split axis 0."
                 )
+                repeats = resplit(repeats, 0)
+            flatten_repeats_t = torch.flatten(repeats._DNDarray__array)
+            repeats = factories.array(
+                flatten_repeats_t,
+                is_split=repeats.split,
+                device=repeats.device,
+                comm=repeats.comm,
+            )
 
-            # axis is not None
-            else:
-                if a.split == axis:
-                    if repeats.split != 0:
-                        warnings.warn(
-                            "If `axis` equals `a.split`, `repeats` has to be split along axis 0 (not {}) if distributed.\n"
-                            "`repeats` will be copied with new split axis 0".format(repeats.split)
-                        )
-                        repeats = resplit(repeats, 0)
+        # axis is not None
+        elif a.split == axis:
+            if repeats.split != 0:
+                warnings.warn(
+                    f"If `axis` equals `a.split`, `repeats` has to be split along axis 0 (not {repeats.split}) if distributed.\n`repeats` will be copied "
+                    "with new split axis 0"
+                )
+                repeats = resplit(repeats, 0)
 
-                # a.split != axis
-                else:
-                    if repeats.split is not None:
-                        warnings.warn(
-                            "If `axis` != `a.split`, `repeast` must not be distributed (along axis {}).\n`repeats` will be copied with new"
-                            " split axis None.".format(repeats.split)
-                        )
-                        repeats = resplit(repeats, None)
+        # a.split != axis
+        else:
+            if repeats.split is not None:
+                warnings.warn(
+                    f"If `axis` != `a.split`, `repeast` must not be distributed (along axis {repeats.split}).\n`repeats` will be copied with new "
+                    "split axis None."
+                )
+                repeats = resplit(repeats, None)
 
-                    if a.lshape[axis] != repeats.lnumel:
-                        raise ValueError(
-                            "Invalid input. Amount of elements of `repeats` ({}) and of `a` in the specified axis ({}) "
-                            "are not the same. Please revise your definition specifying repetitions for all elements "
-                            "of the DNDarray `a` or replace `repeats` with a single scalar".format(
-                                repeats.lnumel, a.lshape[axis]
-                            )
-                        )
+            if a.lshape[axis] != repeats.lnumel:
+                raise ValueError(
+                    f"Invalid input. Amount of elements of `repeats` ({repeats.lnumel}) and of `a` in the specified axis ({a.lshape[axis]}) "
+                    "are not the same. Please revise your definition specifying repetitions for all elements "
+                    "of the DNDarray `a` or replace `repeats` with a single scalar"
+                )
 
         repeated_array_torch = torch.repeat_interleave(
             a._DNDarray__array, repeats._DNDarray__array, axis
         )
 
     repeated_array = factories.array(
         repeated_array_torch, dtype=a.dtype, is_split=a.split, device=a.device, comm=a.comm
@@ -1823,24 +1949,28 @@
     Returns an array with the same data and number of elements as `a`, but with the specified shape.
 
     Parameters
     ----------
     a : DNDarray
         The input array
     shape : Union[int, Tuple[int,...]]
-        Shape of the new array
+        Shape of the new array. Must be compatible with the original shape. If an integer, then the result will be a 1-D array of that length.
+        One shape dimension can be -1. In this case, the value is inferred from the length of the array and remaining dimensions.
     new_split : int, optional
-        The new split axis if `a` is a split DNDarray. None denotes same axis.
-        Default : None
+        The distribution axis of the reshaped array. Default: None (same distribution axis as `a`).
 
     Raises
     ------
     ValueError
         If the number of elements in the new shape is inconsistent with the input data.
 
+    Notes
+    -----
+    `reshape()` might require significant communication among processes. Operating along split axis 0 is recommended.
+
     See Also
     --------
     :func:`ravel`
 
     Examples
     --------
     >>> a = ht.zeros((3,4))
@@ -1873,117 +2003,107 @@
                 shape = shape.numpy()
             else:  # Try to coerce everything else.
                 shape = np.asarray(shape)
         except Exception:
             raise TypeError(e)
     shape = np_proxy.reshape(shape).shape  # sanitized shape according to numpy
 
-    tdtype, tdevice = a.dtype.torch_type(), a.device.torch_device
+    # tdtype, tdevice = a.dtype.torch_type(), a.device.torch_device
+    tdevice = a.device.torch_device
 
-    def reshape_argsort_counts_displs(
-        shape1, lshape1, displs1, axis1, shape2, displs2, axis2, comm
-    ):
-        """
-        Compute the send order, counts, and displacements.
-        """
-        shape1 = torch.tensor(shape1, dtype=torch.int)
-        lshape1 = torch.tensor(lshape1, dtype=torch.int)
-        shape2 = torch.tensor(shape2, dtype=torch.int)
-        # constants
-        width = torch.prod(lshape1[axis1:], dtype=torch.int)
-        height = torch.prod(lshape1[:axis1], dtype=torch.int)
-        global_len = torch.prod(shape1[axis1:])
-        ulen = torch.prod(shape2[axis2 + 1 :])
-        gindex = displs1[comm.rank] * torch.prod(shape1[axis1 + 1 :])
-
-        # Get axis position on new split axis
-        mask = torch.arange(width, device=tdevice) + gindex
-        mask = mask + torch.arange(height, device=tdevice).reshape([height, 1]) * global_len
-        try:
-            mask = (torch.divide(mask, ulen, rounding_mode="floor")) % shape2[axis2]
-        except TypeError:
-            mask = (torch.floor_divide(mask, ulen)) % shape2[axis2]
-        mask = mask.flatten()
+    # always operate along split axis 0
+    orig_split = a.split
+    if a.split is not None:
+        a.resplit_(axis=0)
 
-        # Compute return values
-        counts = torch.zeros(comm.size, dtype=torch.int)
-        displs = torch.zeros_like(counts)
-        argsort = torch.empty_like(mask, dtype=torch.long)
-        plz = 0
-        for i in range(len(displs2) - 1):
-            mat = torch.where((mask >= displs2[i]) & (mask < displs2[i + 1]))[0]
-            counts[i] = mat.numel()
-            argsort[plz : counts[i] + plz] = mat
-            plz += counts[i]
-        displs[1:] = torch.cumsum(counts[:-1], dim=0)
-        return argsort, counts, displs
+    local_a = a.larray
 
     # check new_split parameter
     new_split = kwargs.get("new_split")
     if new_split is None:
-        new_split = a.split
+        new_split = orig_split
     new_split = stride_tricks.sanitize_axis(shape, new_split)
 
-    # Forward to Pytorch directly
-    if a.split is None:
-        local_reshape = torch.reshape(a.larray, shape)
-        if new_split is None:
-            return DNDarray(
-                local_reshape,
-                shape,
-                dtype=a.dtype,
-                split=None,
-                device=a.device,
-                comm=a.comm,
-                balanced=True,
-            )
-        _, _, local_slice = a.comm.chunk(shape, new_split)
-        local_reshape = local_reshape[local_slice]
+    if not a.is_distributed():
+        if a.comm.size > 1 and new_split is not None:
+            # keep local slice only
+            _, _, local_slice = a.comm.chunk(shape, new_split)
+            _ = local_a.reshape(shape)
+            local_a = _[local_slice].contiguous()
+            del _
+        else:
+            local_a = local_a.reshape(shape)
         return DNDarray(
-            local_reshape,
-            shape,
+            local_a,
+            gshape=shape,
             dtype=a.dtype,
             split=new_split,
-            comm=a.comm,
             device=a.device,
+            comm=a.comm,
             balanced=True,
         )
 
-    # Create new flat result tensor
-    _, local_shape, _ = a.comm.chunk(shape, new_split)
-    data = torch.empty(local_shape, dtype=tdtype, device=tdevice).flatten()
-
-    # Calculate the counts and displacements
-    _, old_displs, _ = a.comm.counts_displs_shape(a.shape, a.split)
-    _, new_displs, _ = a.comm.counts_displs_shape(shape, new_split)
-
-    old_displs += (a.shape[a.split],)
-    new_displs += (shape[new_split],)
-
-    sendsort, sendcounts, senddispls = reshape_argsort_counts_displs(
-        a.shape, a.lshape, old_displs, a.split, shape, new_displs, new_split, a.comm
+    lshape_map = a.lshape_map
+    rank = a.comm.rank
+    size = a.comm.size
+
+    # flatten dimensions from split axis on, e.g. if split = 1, (3,4,5) -> (3,20)
+    local_elements_off_split = torch.prod(lshape_map[:, a.split :], dim=1)
+    first_local_shape = tuple(lshape_map[rank, : a.split].tolist()) + (
+        local_elements_off_split[rank].item(),
     )
-    recvsort, recvcounts, recvdispls = reshape_argsort_counts_displs(
-        shape, local_shape, new_displs, new_split, a.shape, old_displs, a.split, a.comm
+    local_a = local_a.reshape(first_local_shape)
+    first_global_shape = tuple(lshape_map[rank, : a.split].tolist()) + (
+        local_elements_off_split.sum().item(),
     )
-
-    # rearrange order
-    send = a.larray.flatten()[sendsort]
-    a.comm.Alltoallv((send, sendcounts, senddispls), (data, recvcounts, recvdispls))
-
-    # original order
-    backsort = torch.argsort(recvsort)
-    data = data[backsort]
-
-    # Reshape local tensor
-    data = data.reshape(local_shape)
-
-    return DNDarray(
-        data, shape, dtype=a.dtype, split=new_split, device=a.device, comm=a.comm, balanced=True
+    reshape_first_pass = DNDarray(
+        local_a,
+        gshape=first_global_shape,
+        dtype=a.dtype,
+        split=a.split,
+        device=a.device,
+        comm=a.comm,
+        balanced=a.balanced,
+    )
+    new_lshape_map = lshape_map[:, : a.split + 1]
+    new_lshape_map[:, a.split] = local_elements_off_split
+    reshape_first_pass.__lshape_map = new_lshape_map
+
+    # redistribute if necessary. All splits but a.split = 0 have been ruled out
+
+    lshape_map = reshape_first_pass.lshape_map
+    current_numel = torch.prod(lshape_map, dim=1)
+    # calculate target number of elements on each rank
+    target_numel = torch.zeros((size, len(shape)), dtype=torch.int64, device=tdevice)
+    for i in range(size):
+        _, local_shape, _ = a.comm.chunk(shape, a.split, rank=i)
+        target_numel[i] = torch.tensor(local_shape)
+        if i == rank:
+            second_local_shape = local_shape
+    target_numel = torch.prod(target_numel, dim=1)
+    if (target_numel == current_numel).all():
+        local_a = local_a.reshape(second_local_shape)
+    else:
+        # redistribution is necessary before reshaping
+        target_map = lshape_map.clone()
+        target_map[:, a.split] = target_numel
+        reshape_first_pass.redistribute_(target_map=target_map)
+        local_a = reshape_first_pass.larray.reshape(second_local_shape)
+    reshape_final = DNDarray(
+        local_a,
+        gshape=shape,
+        dtype=a.dtype,
+        split=0,
+        device=a.device,
+        comm=a.comm,
+        balanced=None,
     )
+    reshape_final.resplit_(axis=new_split)
+
+    return reshape_final
 
 
 DNDarray.reshape = lambda self, *shape, **kwargs: reshape(self, *shape, **kwargs)
 DNDarray.reshape.__doc__ = reshape.__doc__
 
 
 def roll(
@@ -2045,15 +2165,15 @@
                 rank = x.comm.Get_rank()
 
                 # local elements along axis:
                 lshape_map = x.create_lshape_map(force_check=False)[:, x.split]
                 cumsum_map = torch.cumsum(lshape_map, dim=0)  # cumulate along axis
                 indices = torch.arange(size, device=x.device.torch_device)
                 # NOTE Can be removed when min version>=1.9
-                if "1.7." in torch.__version__ or "1.8." in torch.__version__:
+                if "1.8." in torch.__version__:  # pragma: no cover
                     lshape_map = lshape_map.to(torch.int64)
                 index_map = torch.repeat_interleave(indices, lshape_map)  # index -> process
 
                 # compute index positions
                 index_old = torch.arange(lshape_map[rank], device=x.device.torch_device)
                 if rank > 0:
                     index_old += cumsum_map[rank - 1]
@@ -2086,47 +2206,41 @@
 
                 return DNDarray(recv, x.gshape, x.dtype, x.split, x.device, x.comm, x.balanced)
 
         else:  # pytorch does not support int / sequence combo at the time, make shift a list instead
             try:
                 axis = sanitation.sanitize_sequence(axis)
             except TypeError:
-                raise TypeError("axis must be a int, list or a tuple, got {}".format(type(axis)))
+                raise TypeError(f"axis must be a int, list or a tuple, got {type(axis)}")
 
             shift = [shift] * len(axis)
 
             return roll(x, shift, axis)
 
     else:  # input must be tuples now
         try:
             shift = sanitation.sanitize_sequence(shift)
         except TypeError:
-            raise TypeError("shift must be an integer, list or a tuple, got {}".format(type(shift)))
+            raise TypeError(f"shift must be an integer, list or a tuple, got {type(shift)}")
 
         try:
             axis = sanitation.sanitize_sequence(axis)
         except TypeError:
-            raise TypeError("axis must be an integer, list or a tuple, got {}".format(type(axis)))
+            raise TypeError(f"axis must be an integer, list or a tuple, got {type(axis)}")
 
         if len(shift) != len(axis):
             raise ValueError(
-                "shift and axis length must be the same, got {} and {}".format(
-                    len(shift), len(axis)
-                )
+                f"shift and axis length must be the same, got {len(shift)} and {len(axis)}"
             )
 
         for i in range(len(shift)):
             if not isinstance(shift[i], int):
-                raise TypeError(
-                    "Element {} in shift is not an integer, got {}".format(i, type(shift[i]))
-                )
+                raise TypeError(f"Element {i} in shift is not an integer, got {type(shift[i])}")
             if not isinstance(axis[i], int):
-                raise TypeError(
-                    "Element {} in axis is not an integer, got {}".format(i, type(axis[i]))
-                )
+                raise TypeError(f"Element {i} in axis is not an integer, got {type(axis[i])}")
 
         if x.split is not None and (x.split in axis or (x.split - x.ndim) in axis):
             # remove split axis elements
             shift_split = 0
             for y in (x.split, x.split - x.ndim):
                 idx = [i for i in range(len(axis)) if axis[i] == y]
                 for i in idx:
@@ -2205,21 +2319,21 @@
                [4, 6]]], dtype=ht.int32, device=cpu:0, split=None)
     """
     axes = tuple(axes)
     if len(axes) != 2:
         raise ValueError("len(axes) must be 2.")
 
     if not isinstance(m, DNDarray):
-        raise TypeError("expected m to be a ht.DNDarray, but was {}".format(type(m)))
+        raise TypeError(f"expected m to be a ht.DNDarray, but was {type(m)}")
 
     if axes[0] == axes[1] or np.absolute(axes[0] - axes[1]) == m.ndim:
         raise ValueError("Axes must be different.")
 
     if axes[0] >= m.ndim or axes[0] < -m.ndim or axes[1] >= m.ndim or axes[1] < -m.ndim:
-        raise ValueError("Axes={} out of range for array of ndim={}.".format(axes, m.ndim))
+        raise ValueError(f"Axes={axes} out of range for array of ndim={m.ndim}.")
 
     if m.split is None:
         return factories.array(
             torch.rot90(m.larray, k, axes), dtype=m.dtype, device=m.device, comm=m.comm
         )
 
     try:
@@ -2255,15 +2369,15 @@
     Parameters
     ----------
     a : DNDarray
         The input `DNDarray`.
     """
     # sanitize input
     if not isinstance(a, DNDarray):
-        raise TypeError("Expected a to be a DNDarray but was {}".format(type(a)))
+        raise TypeError(f"Expected a to be a DNDarray but was {type(a)}")
 
     return a.gshape
 
 
 def sort(a: DNDarray, axis: int = -1, descending: bool = False, out: Optional[DNDarray] = None):
     """
     Sorts the elements of `a` along the given dimension (by default in ascending order) by their value.
@@ -2333,15 +2447,15 @@
         )
 
         # Only processes with elements should share their pivots
         gather_counts = [int(x > 0) * size for x in counts]
         gather_displs = (0,) + tuple(np.cumsum(gather_counts[:-1]))
 
         pivot_dim = list(transposed.size())
-        pivot_dim[0] = size * sum([1 for x in counts if x > 0])
+        pivot_dim[0] = size * sum(x > 0 for x in counts)
 
         # share the local pivots with root process
         pivot_buffer = torch.empty(
             pivot_dim, dtype=a.dtype.torch_type(), device=a.device.torch_device
         )
         a.comm.Gatherv(local_pivots, (pivot_buffer, gather_counts, gather_displs), root=0)
 
@@ -2588,64 +2702,55 @@
                 [11]])]
     """
     # sanitize x
     sanitation.sanitize_in(x)
 
     # sanitize axis
     if not isinstance(axis, int):
-        raise TypeError("Expected `axis` to be an integer, but was {}".format(type(axis)))
+        raise TypeError(f"Expected `axis` to be an integer, but was {type(axis)}")
     if axis < 0 or axis > len(x.gshape) - 1:
         raise ValueError(
-            "Invalid input for `axis`. Valid range is between 0 and {}, but was {}".format(
-                len(x.gshape) - 1, axis
-            )
+            f"Invalid input for `axis`. Valid range is between 0 and {len(x.gshape) - 1}, but was {axis}"
         )
 
     # sanitize indices_or_sections
     if isinstance(indices_or_sections, int):
         if x.gshape[axis] % indices_or_sections != 0:
             raise ValueError(
-                "DNDarray with shape {} can't be divided equally into {} chunks along axis {}".format(
-                    x.gshape, indices_or_sections, axis
-                )
+                f"DNDarray with shape {x.gshape} can't be divided equally into {indices_or_sections} chunks along axis {axis}"
             )
         # np to torch mapping - calculate size of resulting data chunks
         indices_or_sections_t = x.gshape[axis] // indices_or_sections
 
     elif isinstance(indices_or_sections, (list, tuple, DNDarray)):
         if isinstance(indices_or_sections, (list, tuple)):
             indices_or_sections = factories.array(indices_or_sections)
         if len(indices_or_sections.gshape) != 1:
             raise ValueError(
-                "Expected indices_or_sections to be 1-dimensional, but was {}-dimensional instead.".format(
-                    len(indices_or_sections.gshape) - 1
-                )
+                f"Expected indices_or_sections to be 1-dimensional, but was {len(indices_or_sections.gshape) - 1}-dimensional instead."
             )
     else:
         raise TypeError(
-            "Expected `indices_or_sections` to be array_like (DNDarray, list or tuple), but was {}".format(
-                type(indices_or_sections)
-            )
+            f"Expected `indices_or_sections` to be array_like (DNDarray, list or tuple), but was {type(indices_or_sections)}"
         )
 
     # start of actual algorithm
 
     if x.split == axis and x.is_distributed():
-
         if isinstance(indices_or_sections, int):
             # CASE 1 number of processes == indices_or_selections -> split already done due to distribution
             if x.comm.size == indices_or_sections:
                 new_lshape = list(x.lshape)
                 new_lshape[axis] = 0
                 sub_arrays_t = [
                     torch.empty(new_lshape) if i != x.comm.rank else x._DNDarray__array
                     for i in range(indices_or_sections)
                 ]
 
-            # # CASE 2 number of processes != indices_or_selections -> reorder (and split) chunks correctly
+            # CASE 2 number of processes != indices_or_selections -> reorder (and split) chunks correctly
             else:
                 # no data
                 if x.lshape[axis] == 0:
                     sub_arrays_t = [torch.empty(x.lshape) for i in range(indices_or_sections)]
                 else:
                     offset, local_shape, slices = x.comm.chunk(x.gshape, axis)
                     idx_frst_chunk_affctd = offset // indices_or_sections_t
@@ -2673,18 +2778,16 @@
                         )
 
                     sub_arrays_t = torch.split(x._DNDarray__array, new_indices.tolist(), axis)
         # indices or sections == DNDarray
         else:
             if indices_or_sections.split is not None:
                 warnings.warn(
-                    "`indices_or_sections` might not be distributed (along axis {}) if `x` is not distributed.\n"
-                    "`indices_or_sections` will be copied with new split axis None.".format(
-                        indices_or_sections.split
-                    )
+                    f"`indices_or_sections` might not be distributed (along axis {indices_or_sections.split}) "
+                    "if `x` is not distributed.\n`indices_or_sections` will be copied with new split axis None."
                 )
                 indices_or_sections = resplit(indices_or_sections, None)
 
             offset, local_shape, slices = x.comm.chunk(x.gshape, axis)
             slice_axis = slices[axis]
 
             # reduce information to the (chunk) relevant
@@ -2748,15 +2851,14 @@
                 device=indices_or_sections_t.device,
             )
 
             # 4. transform the result into a list (torch requirement)
             indices_or_sections_t = indices_or_sections_t.tolist()
 
             sub_arrays_t = torch.split(x._DNDarray__array, indices_or_sections_t, axis)
-
     sub_arrays_ht = [
         factories.array(sub_DNDarray, dtype=x.dtype, is_split=x.split, device=x.device, comm=x.comm)
         for sub_DNDarray in sub_arrays_t
     ]
 
     for sub_DNDarray in sub_arrays_ht:
         sub_DNDarray.balance_()
@@ -2827,30 +2929,30 @@
     if axis is not None:
         if isinstance(axis, int):
             dim_is_one = x.shape[axis] == 1
             axis = (axis,)
         elif isinstance(axis, tuple):
             dim_is_one = bool(torch.tensor(list(x.shape[dim] == 1 for dim in axis)).all())
         if not dim_is_one:
-            raise ValueError("Dimension along axis {} is not 1 for shape {}".format(axis, x.shape))
+            raise ValueError(f"Dimension along axis {axis} is not 1 for shape {x.shape}")
 
     if axis is None:
         axis = tuple(i for i, dim in enumerate(x.shape) if dim == 1)
 
     if x.split is not None and x.split in axis:
         # split dimension is about to disappear, set split to None
         x.resplit_(axis=None)
 
     out_lshape = tuple(x.lshape[dim] for dim in range(x.ndim) if dim not in axis)
     out_gshape = tuple(x.gshape[dim] for dim in range(x.ndim) if dim not in axis)
     x_lsqueezed = x.larray.reshape(out_lshape)
 
     # Calculate new split axis according to squeezed shape
     if x.split is not None:
-        split = x.split - len(list(dim for dim in axis if dim < x.split))
+        split = x.split - len([dim for dim in axis if dim < x.split])
     else:
         split = None
 
     return DNDarray(
         x_lsqueezed,
         out_gshape,
         x.dtype,
@@ -2959,18 +3061,18 @@
 
     target = arrays[0]
     try:
         arrays = sanitation.sanitize_distribution(
             *arrays, target=target
         )  # also checks target again
     except NotImplementedError as e:  # transform split axis error to ValueError
-        raise ValueError(e)
+        raise ValueError(e) from e
 
     # extract torch tensors
-    t_arrays = list(array.larray for array in arrays)
+    t_arrays = [array.larray for array in arrays]
 
     # output shape and split
     axis = stride_tricks.sanitize_axis(target.gshape + (len(arrays),), axis)
     stacked_shape = target.gshape[:axis] + (len(arrays),) + target.gshape[axis:]
     if target.split is not None:
         stacked_split = target.split + 1 if axis <= target.split else target.split
     else:
@@ -2978,15 +3080,15 @@
 
     # stack locally
     try:
         t_stacked = torch.stack(t_arrays, dim=axis)
         result_dtype = types.canonical_heat_type(t_stacked.dtype)
     except Exception as e:
         if "size" in e.args[0] or "shape" in e.args[0]:
-            raise ValueError(e)
+            raise ValueError(e) from e
         raise e
 
     # return stacked DNDarrays
     if out is not None:
         sanitation.sanitize_out(out, stacked_shape, stacked_split, target.device)
         out.larray = t_stacked.type(out.larray.dtype)
         return out
@@ -3036,17 +3138,15 @@
                [3, 7]]], dtype=ht.int64, device=cpu:0, split=None)
     """
     axes = list(range(x.ndim))
     try:
         axes[axis1], axes[axis2] = axes[axis2], axes[axis1]
     except TypeError:
         raise TypeError(
-            "'axis1' and 'axis2' must be of type int, found {} and {}".format(
-                type(axis1), type(axis2)
-            )
+            f"'axis1' and 'axis2' must be of type int, found {type(axis1)} and {type(axis2)}"
         )
 
     return linalg.transpose(x, axes)
 
 
 DNDarray.swapaxes = lambda self, axis1, axis2: swapaxes(self, axis1, axis2)
 DNDarray.swapaxes.__doc__ = swapaxes.__doc__
@@ -3088,18 +3188,21 @@
     """
     if a.split is None:
         torch_output = torch.unique(
             a.larray, sorted=sorted, return_inverse=return_inverse, dim=axis
         )
         if isinstance(torch_output, tuple):
             heat_output = tuple(
-                factories.array(i, dtype=a.dtype, split=None, device=a.device) for i in torch_output
+                factories.array(i, dtype=a.dtype, split=None, device=a.device, comm=a.comm)
+                for i in torch_output
             )
         else:
-            heat_output = factories.array(torch_output, dtype=a.dtype, split=None, device=a.device)
+            heat_output = factories.array(
+                torch_output, dtype=a.dtype, split=None, device=a.device, comm=a.comm
+            )
         return heat_output
 
     local_data = a.larray
     unique_axis = None
     inverse_indices = None
 
     if axis is not None:
@@ -3369,26 +3472,27 @@
     # sanitize the axis to check whether it is in range
     axis = stride_tricks.sanitize_axis(arr.shape, axis)
 
     # early out for unchanged content
     if axis == arr.split:
         return arr.copy()
     if not arr.is_distributed():
-        return factories.array(arr.larray, split=axis, device=arr.device, copy=True)
+        return factories.array(arr.larray, split=axis, device=arr.device, comm=arr.comm, copy=True)
 
     if axis is None:
         # new_arr = arr.copy()
         gathered = torch.empty(
             arr.shape, dtype=arr.dtype.torch_type(), device=arr.device.torch_device
         )
         counts, displs = arr.counts_displs()
         arr.comm.Allgatherv(arr.larray, (gathered, counts, displs), recv_axis=arr.split)
-        new_arr = factories.array(gathered, is_split=axis, device=arr.device, dtype=arr.dtype)
+        new_arr = factories.array(
+            gathered, is_split=axis, device=arr.device, comm=arr.comm, dtype=arr.dtype
+        )
         return new_arr
-
     arr_tiles = tiling.SplitTiles(arr)
     new_arr = factories.empty(arr.gshape, split=axis, dtype=arr.dtype, device=arr.device)
     new_tiles = tiling.SplitTiles(new_arr)
     rank = arr.comm.rank
     waits = []
     rcv_waits = {}
     for rpr in range(arr.comm.size):
@@ -3399,15 +3503,15 @@
 
         for i in range(new_locs.shape[0]):
             key = tuple(new_locs[i].tolist())
             spr = arr_tiles.tile_locations[key].item()
             to_send = arr_tiles[key]
             if spr == rank and spr != rpr:
                 waits.append(arr.comm.Isend(to_send.clone(), dest=rpr, tag=rank))
-            elif spr == rpr and rpr == rank:
+            elif spr == rpr == rank:
                 new_tiles[key] = to_send.clone()
             elif rank == rpr:
                 buf = torch.zeros_like(new_tiles[key])
                 rcv_waits[key] = [arr.comm.Irecv(buf=buf, source=spr, tag=spr), buf]
     for w in waits:
         w.Wait()
     for k in rcv_waits.keys():
@@ -3489,15 +3593,15 @@
     >>> b = ht.arange(5, 20, split=0).reshape((3, 5))
     >>> ht.row_stack((a, b)).larray
     [0/2] tensor([[0, 1, 2, 3, 4],
     [0/2]         [5, 6, 7, 8, 9]])
     [1/2] tensor([[10, 11, 12, 13, 14]])
     [2/2] tensor([[15, 16, 17, 18, 19]])
     """
-    arr_dims = list(array.ndim for array in arrays)
+    arr_dims = [array.ndim for array in arrays]
     # sanitation, arrays can be 1-d or 2-d, see sanitation module #468
     over_dims = [i for i, j in enumerate(arr_dims) if j > 2]
     if len(over_dims) > 0:
         raise ValueError("Arrays must be 1-D or 2-D")
     if arr_dims.count(1) == len(arr_dims):
         # all arrays are 1-D, stack
         return stack(arrays, axis=0)
@@ -3624,15 +3728,15 @@
     """
     # x can be DNDarray or scalar
     try:
         _ = x.larray
     except AttributeError:
         try:
             _ = x.shape
-            raise TypeError("Input can be a DNDarray or a scalar, is {}".format(type(x)))
+            raise TypeError(f"Input can be a DNDarray or a scalar, is {type(x)}")
         except AttributeError:
             x = factories.array(x).reshape(1)
 
     x_proxy = x.__torch_proxy__()
 
     # torch-proof args/kwargs:
     # torch `reps`: int or sequence of ints; numpy `reps`: can be array-like
@@ -3646,17 +3750,15 @@
             try:
                 reps = reps.tolist()
             except AttributeError:
                 try:
                     _ = x_proxy.repeat(reps)
                 except TypeError:
                     raise TypeError(
-                        "reps must be a sequence of ints, got {}".format(
-                            list(type(i) for i in reps)
-                        )
+                        f"reps must be a sequence of ints, got {[type(i) for i in reps]}"
                     )
                 except RuntimeError:
                     pass
     except RuntimeError:
         pass
 
     try:
@@ -3715,15 +3817,15 @@
         t_slices_ends = t_slices_starts + torch.tensor(counts, device=local_x.device)
         slices_map.append([t_slices_starts, t_slices_ends])
 
     t_slices_x, t_slices_tiled = slices_map
 
     # keep track of repetitions:
     # local_x_starts.shape, local_x_ends.shape changing from (size,) to (reps[split], size)
-    reps_indices = list(x.gshape[x.split] * rep for rep in (range(reps[x.split])))
+    reps_indices = [x.gshape[x.split] * rep for rep in (range(reps[x.split]))]
     t_reps_indices = torch.tensor(reps_indices, dtype=torch.int32, device=local_x.device).reshape(
         len(reps_indices), 1
     )
     for i, t in enumerate(t_slices_x):
         t = t.repeat((reps[x.split], 1))
         t += t_reps_indices
         t_slices_x[i] = t
@@ -3957,15 +4059,15 @@
         is_split = a.split
         split = None
 
     final_array = factories.array(
         gres, dtype=a.dtype, device=a.device, split=split, is_split=is_split
     )
     final_indices = factories.array(
-        gindices, dtype=types.int64, device=a.device, split=split, is_split=is_split
+        gindices, dtype=types.int64, device=a.device, comm=a.comm, split=split, is_split=is_split
     )
 
     if out is not None:
         if out[0].shape != final_array.shape or out[1].shape != final_indices.shape:
             raise ValueError(
                 "Expecting output buffer tuple of shape ({}, {}), got ({}, {})".format(
                     gres.shape, gindices.shape, out[0].shape, out[1].shape
```

### Comparing `heat-1.2.2/heat/core/memory.py` & `heat-1.3.0/heat/core/memory.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,34 +54,35 @@
     if order == "K":
         raise NotImplementedError(
             "Internal usage of torch.clone() means losing original memory layout for now. \n Please specify order='C' for row-major, order='F' for column-major layout."
         )
     if x.ndim < 2 or x.numel() == 0:
         # do nothing
         return x
-    dims = list(range(x.ndim))
-    stride = torch.tensor(x.stride())
+    stride_diff = torch.as_tensor(x.stride())
     # since strides can get a bit wonky with operations like transpose
     #   we should assume that the tensors are row major or are distributed the default way
-    sdiff = stride[1:] - stride[:-1]
-    column_major = all(sdiff >= 0)
-    row_major = True if not column_major else False
+    stride_diff = stride_diff[1:] - stride_diff[:-1]
+    column_major = torch.all(stride_diff >= 0)
+    row_major = not column_major
+    del stride_diff
     if (order == "C" and row_major) or (order == "F" and column_major):
         # do nothing
+        del column_major, row_major
         return x
-    elif (order == "C" and column_major) or (order == "F" and row_major):
+    if (order == "C" and column_major) or (order == "F" and row_major):
+        dims = list(range(x.ndim))
         dims = tuple(reversed(dims))
         y = torch.empty_like(x)
         permutation = x.permute(dims).contiguous()
         y = y.set_(
             permutation.storage(),
             x.storage_offset(),
             x.shape,
             tuple(reversed(permutation.stride())),
         )
+        del permutation, dims, column_major, row_major, x
         return y
     else:
         raise ValueError(
-            "combination of order and layout not permitted, order: {} column major: {} row major: {}".format(
-                order, column_major, row_major
-            )
+            f"combination of order and layout not permitted, order: {order} column major: {column_major} row major: {row_major}"
         )
```

### Comparing `heat-1.2.2/heat/core/printing.py` & `heat-1.3.0/heat/core/printing.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,19 +169,19 @@
     sci_mode : bool, optional
         Enable (True) or disable (False) scientific notation. If None (default) is specified, the value is automatically
         inferred by HeAT.
     """
     torch.set_printoptions(precision, threshold, edgeitems, linewidth, profile, sci_mode)
 
     # HeAT profiles will print a bit wider than PyTorch does
-    if profile == "default" and linewidth is None:
-        torch._tensor_str.PRINT_OPTS.linewidth = _DEFAULT_LINEWIDTH
-    elif profile == "short" and linewidth is None:
-        torch._tensor_str.PRINT_OPTS.linewidth = _DEFAULT_LINEWIDTH
-    elif profile == "full" and linewidth is None:
+    if (
+        (profile == "default" and linewidth is None)
+        or (profile == "short" and linewidth is None)
+        or (profile == "full" and linewidth is None)
+    ):
         torch._tensor_str.PRINT_OPTS.linewidth = _DEFAULT_LINEWIDTH
 
 
 def __str__(dndarray) -> str:
     """
     Computes a printable representation of the passed DNDarray.
 
@@ -281,15 +281,8 @@
 
     # we will recycle torch's printing features here
     # to do so, we slice up the torch data and forward it to torch internal printing mechanism
     summarize = elements > get_printoptions()["threshold"]
     torch_data = _torch_data(dndarray, summarize)
     formatter = torch._tensor_str._Formatter(torch_data)
 
-    if int(torch.__version__[2]) <= 5 and int(torch.__version__[0]) == 0:
-        return torch._tensor_str._tensor_str_with_formatter(
-            torch_data, indent, formatter, summarize
-        )
-    else:
-        return torch._tensor_str._tensor_str_with_formatter(
-            torch_data, indent, summarize, formatter
-        )
+    return torch._tensor_str._tensor_str_with_formatter(torch_data, indent, summarize, formatter)
```

### Comparing `heat-1.2.2/heat/core/random.py` & `heat-1.3.0/heat/core/random.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,36 +100,34 @@
     rank = comm.Get_rank()
     size = comm.Get_size()
     max_count = 0xFFFFFFFF if dtype == torch.int32 else 0xFFFFFFFFFFFFFFFF
 
     # extract the counter state of the random number generator
     if dtype is torch.int32:
         c_0 = (__counter & (max_count << 32)) >> 32
-        c_1 = __counter & max_count
     else:  # torch.int64
         c_0 = (__counter & (max_count << 64)) >> 64
-        c_1 = __counter & max_count
-
+    c_1 = __counter & max_count
     total_elements = torch.prod(torch.tensor(shape))
     if total_elements.item() > 2 * max_count:
-        raise ValueError("Shape is to big with {} elements".format(total_elements))
+        raise ValueError(f"Shape is to big with {total_elements} elements")
 
     if split is None:
-        values = torch.ceil(total_elements / 2)
-        even_end = total_elements % 2 == 0
+        values = total_elements.item() // 2 + total_elements.item() % 2
+        even_end = total_elements.item() % 2 == 0
         lslice = slice(None) if even_end else slice(None, -1)
         start = c_1
         end = start + int(values)
         lshape = shape
     else:
         offset, lshape, _ = comm.chunk(shape, split)
         counts, displs, _ = comm.counts_displs_shape(shape, split)
 
         # Calculate number of local elements per process
-        local_elements = [total_elements / shape[split] * counts[i] for i in range(size)]
+        local_elements = [total_elements.item() / shape[split] * counts[i] for i in range(size)]
         cum_elements = torch.cumsum(torch.tensor(local_elements, device=device.torch_device), dim=0)
 
         # Calculate the correct borders and slices
         even_start = True if rank == 0 else cum_elements[rank - 1] % 2 == 0
         start = c_1 if rank == 0 else int(cum_elements[rank - 1] / 2) + c_1
         elements = local_elements[rank] / 2
         lslice = slice(None)
@@ -306,17 +304,17 @@
         Uses the standard normal distribution
 
     Examples
     --------
     >>> ht.random.normal(ht.array([-1,2]), ht.array([0.5, 2]), (2,))
     DNDarray([-1.4669,  1.6596], dtype=ht.float64, device=cpu:0, split=None)
     """
-    if not (isinstance(mean, float) or isinstance(mean, int)) and not isinstance(mean, DNDarray):
+    if not (isinstance(mean, (float, int))) and not isinstance(mean, DNDarray):
         raise TypeError("'mean' must be float or DNDarray")
-    if not (isinstance(std, float) or isinstance(std, int)) and not isinstance(std, DNDarray):
+    if not (isinstance(std, (float, int))) and not isinstance(std, DNDarray):
         raise TypeError("'mean' must be float or DNDarray")
 
     if ((isinstance(std, float) or isinstance(std, int)) and std < 0) or (
         isinstance(std, DNDarray) and logical.any(std < 0)
     ):
         raise ValueError("'std' must be non-negative")
 
@@ -441,15 +439,15 @@
     """
     # if args are not set, generate a single sample
     if not args:
         args = (1,)
 
     # ensure that the passed dimensions are positive integer-likes
     shape = tuple(int(ele) for ele in args)
-    if not all(ele > 0 for ele in shape):
+    if any(ele <= 0 for ele in shape):
         raise ValueError("negative dimensions are not allowed")
 
     # make sure the remaining parameters are of proper type
     split = stride_tricks.sanitize_axis(shape, split)
     device = devices.sanitize_device(device)
     comm = communication.sanitize_comm(comm)
     balanced = True
@@ -469,15 +467,15 @@
 
         # combine the values into one tensor and convert them to floats
         values = __int64_to_float64(torch.stack([x_0, x_1], dim=1).flatten()[lslice]).reshape(
             lshape
         )
     else:
         # Unsupported type
-        raise ValueError("dtype is none of ht.float32 or ht.float64 but was {}".format(dtype))
+        raise ValueError(f"dtype is none of ht.float32 or ht.float64 but was {dtype}")
 
     return DNDarray(values, shape, dtype, split, device, comm, balanced)
 
 
 def randint(
     low: int,
     high: Optional[int] = None,
@@ -537,15 +535,15 @@
     if size is None:
         size = ()
     try:
         shape = tuple(int(ele) for ele in size)
     except TypeError:
         shape = (int(size),)
     else:
-        if not all(ele >= 0 for ele in shape):
+        if any(ele < 0 for ele in shape):
             raise ValueError("negative dimensions are not allowed")
 
     # sanitize the data type
     if dtype is None:
         dtype = types.int32
     dtype = types.canonical_heat_type(dtype)
     if dtype not in [types.int64, types.int32]:
@@ -809,15 +807,15 @@
     Raises
     ------
     TypeError
         If and improper state is passed.
     ValueError
         If one of the items in the state tuple is of wrong type or value.
     """
-    if not isinstance(state, tuple) or (len(state) != 3 and len(state) != 5):
+    if not isinstance(state, tuple) or len(state) not in [3, 5]:
         raise TypeError("state needs to be a three- or five-tuple")
 
     if state[0] != "Threefry":
         raise ValueError("algorithm must be 'Threefry'")
 
     global __seed, __counter
     __seed = int(state[1])
```

### Comparing `heat-1.2.2/heat/core/relational.py` & `heat-1.3.0/heat/core/relational.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,17 @@
         return False
         # x = factories.full_like(y, fill_value=x)
     else:  # elif isinstance(x, DNDarray) and isinstance(y, DNDarray):
         if x.gnumel == 1:
             return equal(x.item(), y)
         elif y.gnumel == 1:
             return equal(x, y.item())
-        elif not x.comm == y.comm:
+        elif x.comm != y.comm:
             raise NotImplementedError("Not implemented for other comms")
-        elif not x.gshape == y.gshape:
+        elif x.gshape != y.gshape:
             return False
 
         if x.split is None and y.split is None:
             pass
         elif x.split is None and y.split is not None:
             if y.is_balanced(force_check=False):
                 x = factories.array(x, split=y.split, copy=False, comm=x.comm, device=x.device)
@@ -148,17 +148,17 @@
                 idx[x.split] = slice(
                     target_map[: y.comm.rank, x.split].sum(),
                     target_map[: y.comm.rank + 1, x.split].sum(),
                 )
                 y = factories.array(
                     y.larray[tuple(idx)], is_split=x.split, copy=False, comm=y.comm, device=y.device
                 )
-        elif not x.split == y.split:
+        elif x.split != y.split:
             raise ValueError(
-                "DNDarrays must have the same split axes, found {} and {}".format(x.split, y.split)
+                "DNDarrays must have the same split axes, found {x.split} and {y.split}"
             )
         elif not (x.is_balanced(force_check=False) and y.is_balanced(force_check=False)):
             x_lmap = x.lshape_map
             y_lmap = y.lshape_map
             if not torch.equal(x_lmap, y_lmap):
                 x = x.balance()
                 y = y.balance()
```

### Comparing `heat-1.2.2/heat/core/rounding.py` & `heat-1.3.0/heat/core/rounding.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,33 +244,29 @@
     Examples
     --------
     >>> import heat as ht
     >>> ht.modf(ht.arange(-2.0, 2.0, 0.4))
     (DNDarray([ 0.0000, -0.6000, -0.2000, -0.8000, -0.4000,  0.0000,  0.4000,  0.8000,  0.2000,  0.6000], dtype=ht.float32, device=cpu:0, split=None), DNDarray([-2., -1., -1., -0., -0.,  0.,  0.,  0.,  1.,  1.], dtype=ht.float32, device=cpu:0, split=None))
     """
     if not isinstance(x, DNDarray):
-        raise TypeError("expected x to be a DNDarray, but was {}".format(type(x)))
+        raise TypeError(f"expected x to be a DNDarray, but was {type(x)}")
 
     integralParts = trunc(x)
     fractionalParts = x - integralParts
 
     if out is not None:
         if not isinstance(out, tuple):
-            raise TypeError(
-                "expected out to be None or a tuple of DNDarray, but was {}".format(type(out))
-            )
+            raise TypeError(f"expected out to be None or a tuple of DNDarray, but was {type(out)}")
         if len(out) != 2:
             raise ValueError(
-                "expected out to be a tuple of length 2, but was of length {}".format(len(out))
+                f"expected out to be a tuple of length 2, but was of length {len(out)}"
             )
         if (not isinstance(out[0], DNDarray)) or (not isinstance(out[1], DNDarray)):
             raise TypeError(
-                "expected out to be None or a tuple of DNDarray, but was ({}, {})".format(
-                    type(out[0]), type(out[1])
-                )
+                f"expected out to be None or a tuple of DNDarray, but was ({type(out[0])}, {type(out[1])})"
             )
         out[0].larray = fractionalParts.larray
         out[1].larray = integralParts.larray
         return out
 
     return (fractionalParts, integralParts)
 
@@ -388,44 +384,43 @@
     >>> a = ht.array([-1, -0.5, 0, 0.5, 1])
     >>> ht.sign(a)
     DNDarray([-1., -1.,  0.,  1.,  1.], dtype=ht.float32, device=cpu:0, split=None)
     >>> ht.sign(ht.array([5-2j, 3+4j]))
     DNDarray([(1+0j), (1+0j)], dtype=ht.complex64, device=cpu:0, split=None)
     """
     # special case for complex values
-    if types.heat_type_is_complexfloating(x.dtype):
-        sanitation.sanitize_in(x)
-        if out is not None:
-            sanitation.sanitize_out(out, x.shape, x.split, x.device)
-            out.larray.copy_(x.larray)
-            data = out.larray
-        else:
-            data = torch.clone(x.larray)
-        # NOTE remove when min version >= 1.9
-        if "1.7" in torch.__version__ or "1.8" in torch.__version__:
-            pos = data != 0
-        else:  # pragma: no cover
-            indices = torch.nonzero(data)
-            pos = torch.split(indices, 1, 1)
-        data[pos] = x.larray[pos] / torch.sqrt(torch.square(x.larray[pos]))
-
-        if out is not None:
-            out.__dtype = types.heat_type_of(data)
-            return out
-        return DNDarray(
-            data,
-            gshape=x.shape,
-            dtype=types.heat_type_of(data),
-            split=x.split,
-            device=x.device,
-            comm=x.comm,
-            balanced=x.balanced,
-        )
+    if not types.heat_type_is_complexfloating(x.dtype):
+        return _operations.__local_op(torch.sign, x, out)
+    sanitation.sanitize_in(x)
+    if out is not None:
+        sanitation.sanitize_out(out, x.shape, x.split, x.device)
+        out.larray.copy_(x.larray)
+        data = out.larray
+    else:
+        data = torch.clone(x.larray)
+    # NOTE remove when min version >= 1.9
+    if "1.8" in torch.__version__:  # pragma: no cover
+        pos = data != 0
+    else:
+        indices = torch.nonzero(data)
+        pos = torch.split(indices, 1, 1)
+    data[pos] = x.larray[pos] / torch.sqrt(torch.square(x.larray[pos]))
 
-    return _operations.__local_op(torch.sign, x, out)
+    if out is not None:
+        out.__dtype = types.heat_type_of(data)
+        return out
+    return DNDarray(
+        data,
+        gshape=x.shape,
+        dtype=types.heat_type_of(data),
+        split=x.split,
+        device=x.device,
+        comm=x.comm,
+        balanced=x.balanced,
+    )
 
 
 def trunc(x: DNDarray, out: Optional[DNDarray] = None) -> DNDarray:
     """
     Return the trunc of the input, element-wise.
     The truncated value of the scalar ``x`` is the nearest integer ``i`` which is closer to zero than ``x`` is. In short, the
     fractional part of the signed number ``x`` is discarded.
```

### Comparing `heat-1.2.2/heat/core/sanitation.py` & `heat-1.3.0/heat/core/sanitation.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,21 @@
     See Also
     ---------
     :func:`~heat.core.dndarray.create_lshape_map`
         Function to create the lshape_map.
     """
     out = []
     sanitize_in(target)
+    # early out on 1 process
+    if target.comm.size == 1:
+        for arg in args:
+            sanitize_in(arg)
+            out.append(arg)
+        return tuple(out) if len(out) > 1 else out[0]
+
     target_split = target.split
     if diff_map is not None:
         sanitize_in_tensor(diff_map)
         target_map = diff_map
         if target_split is not None:
             tmap_split = target_map[:, target_split]
             target_size = tmap_split.sum().item()
@@ -79,39 +86,33 @@
     elif target_split is not None:
         target_map = target.lshape_map
         target_size = target.shape[target_split]
         target_balanced = target.is_balanced(force_check=False)
 
     for arg in args:
         sanitize_in(arg)
-        if not target.comm == arg.comm:
+        if target.comm != arg.comm:
             try:
                 raise NotImplementedError(
-                    "Not implemented for other comms, found {} and {}".format(
-                        target.comm.name, arg.comm.name
-                    )
+                    f"Not implemented for other comms, found {target.comm.name} and {arg.comm.name}"
                 )
             except Exception:
                 raise NotImplementedError("Not implemented for other comms")
         elif target_split is None:
             if arg.split is not None:
                 raise NotImplementedError(
-                    "DNDarrays must have the same split axes, found {} and {}".format(
-                        target_split, arg.split
-                    )
+                    f"DNDarrays must have the same split axes, found {target_split} and {arg.split}"
                 )
             else:
                 out.append(arg)
         elif arg.shape[target_split] == 1 and target_size > 1:  # broadcasting in split-dimension
             out.append(arg.resplit(None))
         elif arg.shape[target_split] != target_size:
             raise ValueError(
-                "Cannot distribute to match in split dimension, shapes are {} and {}".format(
-                    target.shape, arg.shape
-                )
+                f"Cannot distribute to match in split dimension, shapes are {target.shape} and {arg.shape}"
             )
         elif arg.split is None:  # undistributed case
             if target_balanced:
                 out.append(
                     factories.array(
                         arg, split=target_split, copy=False, comm=arg.comm, device=arg.device
                     )
@@ -129,17 +130,15 @@
                         copy=False,
                         comm=arg.comm,
                         device=arg.device,
                     )
                 )
         elif arg.split != target_split:
             raise NotImplementedError(
-                "DNDarrays must have the same split axes, found {} and {}".format(
-                    target_split, arg.split
-                )
+                f"DNDarrays must have the same split axes, found {target_split} and {arg.split}"
             )
         elif not (
             # False
             target_balanced
             and arg.is_balanced(force_check=False)
         ):  # Split axes are the same and atleast one is not balanced
             current_map = arg.lshape_map
@@ -167,15 +166,15 @@
 
     Raises
     ------
     TypeError
         When ``x`` is not a ``DNDarray``.
     """
     if not isinstance(x, DNDarray):
-        raise TypeError("Input must be a DNDarray, is {}".format(type(x)))
+        raise TypeError(f"Input must be a DNDarray, is {type(x)}")
 
 
 def sanitize_infinity(x: Union[DNDarray, torch.Tensor]) -> Union[int, float]:
     """
     Returns largest possible value for the ``dtype`` of the input array.
 
     Parameters
@@ -203,15 +202,15 @@
 
     Raises
     ------
     TypeError
         When ``x`` is not a ``torch.Tensor``.
     """
     if not isinstance(x, torch.Tensor):
-        raise TypeError("Input must be a torch.Tensor, is {}".format(type(x)))
+        raise TypeError(f"Input must be a torch.Tensor, is {type(x)}")
 
 
 def sanitize_lshape(array: DNDarray, tensor: torch.Tensor):
     """
     Verify shape consistency when manipulating process-local arrays.
 
     Parameters
@@ -230,33 +229,29 @@
     tshape = tuple(tensor.shape)
     if tshape == array.lshape:
         return
     gshape = array.gshape
     split = array.split
     if split is None:
         # allow for axes with size 0, other axes must match
-        non_zero = list(i for i in range(len(tshape)) if tshape[i] != 0)
-        cond = list(tshape[i] == gshape[i] for i in non_zero).count(True) == len(non_zero)
+        non_zero = [i for i in range(len(tshape)) if tshape[i] != 0]
+        cond = [tshape[i] == gshape[i] for i in non_zero].count(True) == len(non_zero)
         if cond:
             return
         else:
             raise ValueError(
-                "Shape of local tensor is inconsistent with global DNDarray: tensor.shape is {}, should be {}".format(
-                    tshape, gshape
-                )
+                f"Shape of local tensor is inconsistent with global DNDarray: tensor.shape is {tshape}, should be {gshape}"
             )
     # size of non-split dimensions must match global shape
     reduced_gshape = gshape[:split] + gshape[split + 1 :]
     reduced_tshape = tshape[:split] + tshape[split + 1 :]
     if reduced_tshape == reduced_gshape:
         return
     raise ValueError(
-        "Shape of local tensor along non-split axes is inconsistent with global DNDarray: tensor.shape is {}, DNDarray is {}".format(
-            tshape, gshape
-        )
+        f"Shape of local tensor along non-split axes is inconsistent with global DNDarray: tensor.shape is {tshape}, DNDarray is {gshape}"
     )
 
 
 def sanitize_out(
     out: Any,
     output_shape: Tuple,
     output_split: int,
@@ -287,34 +282,32 @@
     ------
     TypeError
         if ``out`` is not a ``DNDarray``.
     ValueError
         if shape, split direction, or device of the output buffer ``out`` do not match the operation result.
     """
     if not isinstance(out, DNDarray):
-        raise TypeError("expected `out` to be None or a DNDarray, but was {}".format(type(out)))
+        raise TypeError(f"expected `out` to be None or a DNDarray, but was {type(out)}")
 
     out_proxy = out.__torch_proxy__()
     out_proxy.names = [
-        "split" if (out.split is not None and i == out.split) else "_{}".format(i)
+        "split" if (out.split is not None and i == out.split) else f"_{i}"
         for i in range(out_proxy.ndim)
     ]
     out_proxy = out_proxy.squeeze()
 
     check_proxy = torch.ones(1).expand(output_shape)
     check_proxy.names = [
-        "split" if (output_split is not None and i == output_split) else "_{}".format(i)
+        "split" if (output_split is not None and i == output_split) else f"_{i}"
         for i in range(check_proxy.ndim)
     ]
     check_proxy = check_proxy.squeeze()
 
     if out_proxy.shape != check_proxy.shape:
-        raise ValueError(
-            "Expecting output buffer of shape {}, got {}".format(output_shape, out.shape)
-        )
+        raise ValueError(f"Expecting output buffer of shape {output_shape}, got {out.shape}")
     count_split = int(out.split is not None) + int(output_split is not None)
     if count_split == 1:
         raise ValueError(
             "Split axis of output buffer is inconsistent with split semantics for this operation."
         )
     elif count_split == 2:
         if out.shape[out.split] > 1:  # split axis is not squeezed out
@@ -329,24 +322,20 @@
             check_num_dim_before_split = len(
                 [name for name in check_proxy.names if int(name[1:]) < output_split]
             )
             if num_dim_before_split != check_num_dim_before_split:
                 raise ValueError(
                     "Split axis of output buffer is inconsistent with split semantics for this operation."
                 )
-    if out.device is not output_device:
-        raise ValueError(
-            "Device mismatch: out is on {}, should be on {}".format(out.device, output_device)
-        )
+    if out.device != output_device:
+        raise ValueError(f"Device mismatch: out is on {out.device}, should be on {output_device}")
     if output_comm is not None and out.comm != output_comm:
         try:
             raise NotImplementedError(
-                "Not implemented for other comms, found {} and {}".format(
-                    out.comm.name, output_comm.name
-                )
+                f"Not implemented for other comms, found {out.comm.name} and {output_comm.name}"
             )
         except Exception:
             raise NotImplementedError("Not implemented for other comms")
 
 
 def sanitize_sequence(
     seq: Union[Sequence[int, ...], Sequence[float, ...], DNDarray, torch.Tensor]
@@ -365,15 +354,15 @@
         if ``seq`` is neither a list nor a tuple
     """
     if isinstance(seq, list):
         return seq
     elif isinstance(seq, tuple):
         return list(seq)
     else:
-        raise TypeError("seq must be a list or a tuple, got {}".format(type(seq)))
+        raise TypeError(f"seq must be a list or a tuple, got {type(seq)}")
 
 
 def scalar_to_1d(x: DNDarray) -> DNDarray:
     """
     Turn a scalar ``DNDarray`` into a 1-D ``DNDarray`` with 1 element.
 
     Parameters
```

### Comparing `heat-1.2.2/heat/core/signal.py` & `heat-1.3.0/heat/core/signal.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Provides a collection of signal-processing operations"""
 
 import torch
-from typing import Union, Tuple, Sequence
+import numpy as np
 
 from .communication import MPI
 from .dndarray import DNDarray
 from .types import promote_types
-from .manipulations import pad
-from .factories import array
+from .manipulations import pad, flip
+from .factories import array, zeros
 import torch.nn.functional as fc
 
 __all__ = ["convolve"]
 
 
 def convolve(a: DNDarray, v: DNDarray, mode: str = "full") -> DNDarray:
     """
-    Returns the discrete, linear convolution of two one-dimensional `DNDarray`s.
+    Returns the discrete, linear convolution of two one-dimensional `DNDarray`s or scalars.
 
     Parameters
     ----------
-    a : DNDarray
-        One-dimensional signal `DNDarray` of shape (N,)
-    v : DNDarray
-        One-dimensional filter weight `DNDarray` of shape (M,).
+    a : DNDarray or scalar
+        One-dimensional signal `DNDarray` of shape (N,) or scalar.
+    v : DNDarray or scalar
+        One-dimensional filter weight `DNDarray` of shape (M,) or scalar.
     mode : str
         Can be 'full', 'valid', or 'same'. Default is 'full'.
         'full':
           Returns the convolution at
           each point of overlap, with an output shape of (N+M-1,). At
           the end-points of the convolution, the signals do not overlap
           completely, and boundary effects may be seen.
@@ -36,113 +36,171 @@
           even-sized filter weights
         'valid':
           Mode 'valid' returns output of length 'N-M+1'. The
           convolution product is only given for points where the signals
           overlap completely. Values outside the signal boundary have no
           effect.
 
-    Notes
-    -----
-        Contrary to the original `numpy.convolve`, this function does not
-        swap the input arrays if the second one is larger than the first one.
-        This is because `a`, the signal, might be memory-distributed,
-        whereas the filter `v` is assumed to be non-distributed,
-        i.e. a copy of `v` will reside on each process.
-
-
     Examples
     --------
     Note how the convolution operator flips the second array
     before "sliding" the two across one another:
 
     >>> a = ht.ones(10)
     >>> v = ht.arange(3).astype(ht.float)
     >>> ht.convolve(a, v, mode='full')
     DNDarray([0., 1., 3., 3., 3., 3., 2.])
     >>> ht.convolve(a, v, mode='same')
     DNDarray([1., 3., 3., 3., 3.])
     >>> ht.convolve(a, v, mode='valid')
     DNDarray([3., 3., 3.])
+    >>> a = ht.ones(10, split = 0)
+    >>> v = ht.arange(3, split = 0).astype(ht.float)
+    >>> ht.convolve(a, v, mode='valid')
+    DNDarray([3., 3., 3., 3., 3., 3., 3., 3.])
+
+    [0/3] DNDarray([3., 3., 3.])
+    [1/3] DNDarray([3., 3., 3.])
+    [2/3] DNDarray([3., 3.])
+    >>> a = ht.ones(10, split = 0)
+    >>> v = ht.arange(3, split = 0)
+    >>> ht.convolve(a, v)
+    DNDarray([0., 1., 3., 3., 3., 3., 3., 3., 3., 3., 3., 2.], dtype=ht.float32, device=cpu:0, split=0)
+
+    [0/3] DNDarray([0., 1., 3., 3.])
+    [1/3] DNDarray([3., 3., 3., 3.])
+    [2/3] DNDarray([3., 3., 3., 2.])
     """
+    if np.isscalar(a):
+        a = array([a])
+    if np.isscalar(v):
+        v = array([v])
     if not isinstance(a, DNDarray):
         try:
             a = array(a)
         except TypeError:
-            raise TypeError("non-supported type for signal: {}".format(type(a)))
+            raise TypeError(f"non-supported type for signal: {type(a)}")
     if not isinstance(v, DNDarray):
         try:
             v = array(v)
         except TypeError:
-            raise TypeError("non-supported type for filter: {}".format(type(v)))
+            raise TypeError(f"non-supported type for filter: {type(v)}")
     promoted_type = promote_types(a.dtype, v.dtype)
     a = a.astype(promoted_type)
     v = v.astype(promoted_type)
 
-    if v.is_distributed():
-        raise TypeError("Distributed filter weights are not supported")
     if len(a.shape) != 1 or len(v.shape) != 1:
         raise ValueError("Only 1-dimensional input DNDarrays are allowed")
-    if a.shape[0] <= v.shape[0]:
-        raise ValueError("Filter size must not be greater than or equal to signal size")
     if mode == "same" and v.shape[0] % 2 == 0:
         raise ValueError("Mode 'same' cannot be used with even-sized kernel")
+    if not v.is_balanced():
+        raise ValueError("Only balanced kernel weights are allowed")
+
+    if v.shape[0] > a.shape[0]:
+        a, v = v, a
 
     # compute halo size
-    halo_size = v.shape[0] // 2
+    halo_size = torch.max(v.lshape_map[:, 0]).item() // 2
 
     # pad DNDarray with zeros according to mode
     if mode == "full":
         pad_size = v.shape[0] - 1
         gshape = v.shape[0] + a.shape[0] - 1
     elif mode == "same":
-        pad_size = halo_size
+        pad_size = v.shape[0] // 2
         gshape = a.shape[0]
     elif mode == "valid":
         pad_size = 0
         gshape = a.shape[0] - v.shape[0] + 1
     else:
-        raise ValueError("Supported modes are 'full', 'valid', 'same', got {}".format(mode))
+        raise ValueError(f"Supported modes are 'full', 'valid', 'same', got {mode}")
 
     a = pad(a, pad_size, "constant", 0)
 
     if a.is_distributed():
-        if (v.shape[0] > a.lshape_map[:, 0]).any():
-            raise ValueError("Filter weight is larger than the local chunks of signal")
+        if (v.lshape_map[:, 0] > a.lshape_map[:, 0]).any():
+            raise ValueError(
+                "Local chunk of filter weight is larger than the local chunks of signal"
+            )
         # fetch halos and store them in a.halo_next/a.halo_prev
         a.get_halo(halo_size)
         # apply halos to local array
         signal = a.array_with_halos
     else:
         signal = a.larray
 
+    # flip filter for convolution as Pytorch conv1d computes correlations
+    v = flip(v, [0])
+    if v.larray.shape != v.lshape_map[0]:
+        # pads weights if input kernel is uneven
+        target = torch.zeros(v.lshape_map[0][0], dtype=v.larray.dtype, device=v.larray.device)
+        pad_size = v.lshape_map[0][0] - v.larray.shape[0]
+        target[pad_size:] = v.larray
+        weight = target
+    else:
+        weight = v.larray
+
+    t_v = weight  # stores temporary weight
+
     # make signal and filter weight 3D for Pytorch conv1d function
     signal = signal.reshape(1, 1, signal.shape[0])
-
-    # flip filter for convolution as Pytorch conv1d computes correlations
-    weight = v.larray.flip(dims=(0,))
     weight = weight.reshape(1, 1, weight.shape[0])
 
     # cast to float if on GPU
     if signal.is_cuda:
         float_type = promote_types(signal.dtype, torch.float32).torch_type()
         signal = signal.to(float_type)
         weight = weight.to(float_type)
+        t_v = t_v.to(float_type)
 
-    # apply torch convolution operator
-    signal_filtered = fc.conv1d(signal, weight)
+    if v.is_distributed():
+        size = v.comm.size
+
+        for r in range(size):
+            rec_v = t_v.clone()
+            v.comm.Bcast(rec_v, root=r)
+            t_v1 = rec_v.reshape(1, 1, rec_v.shape[0])
+            local_signal_filtered = fc.conv1d(signal, t_v1)
+            # unpack 3D result into 1D
+            local_signal_filtered = local_signal_filtered[0, 0, :]
+
+            if a.comm.rank != 0 and v.lshape_map[0][0] % 2 == 0:
+                local_signal_filtered = local_signal_filtered[1:]
+
+            # accumulate filtered signal on the fly
+            global_signal_filtered = array(
+                local_signal_filtered, is_split=0, device=a.device, comm=a.comm
+            )
+            if r == 0:
+                # initialize signal_filtered, starting point of slice
+                signal_filtered = zeros(
+                    gshape, dtype=a.dtype, split=a.split, device=a.device, comm=a.comm
+                )
+                start_idx = 0
+
+            # accumulate relevant slice of filtered signal
+            # note, this is a binary operation between unevenly distributed dndarrays and will require communication, check out _operations.__binary_op()
+            signal_filtered += global_signal_filtered[start_idx : start_idx + gshape]
+            if r != size - 1:
+                start_idx += v.lshape_map[r + 1][0].item()
+        return signal_filtered
+
+    else:
+        # apply torch convolution operator
+        signal_filtered = fc.conv1d(signal, weight)
 
-    # unpack 3D result into 1D
-    signal_filtered = signal_filtered[0, 0, :]
+        # unpack 3D result into 1D
+        signal_filtered = signal_filtered[0, 0, :]
 
-    # if kernel shape along split axis is even we need to get rid of duplicated values
-    if a.comm.rank != 0 and v.shape[0] % 2 == 0:
-        signal_filtered = signal_filtered[1:]
-
-    return DNDarray(
-        signal_filtered.contiguous(),
-        (gshape,),
-        signal_filtered.dtype,
-        a.split,
-        a.device,
-        a.comm,
-        balanced=False,
-    ).astype(a.dtype.torch_type())
+        # if kernel shape along split axis is even we need to get rid of duplicated values
+        if a.comm.rank != 0 and v.shape[0] % 2 == 0:
+            signal_filtered = signal_filtered[1:]
+
+        return DNDarray(
+            signal_filtered.contiguous(),
+            (gshape,),
+            signal_filtered.dtype,
+            a.split,
+            a.device,
+            a.comm,
+            balanced=False,
+        ).astype(a.dtype.torch_type())
```

### Comparing `heat-1.2.2/heat/core/statistics.py` & `heat-1.3.0/heat/core/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,17 +248,17 @@
     >>> ht.average(data, weights=weights)
     Traceback (most recent call last):
         ...
     TypeError: Axis must be specified when shapes of x and weights differ.
     """
     # perform sanitation
     if not isinstance(x, DNDarray):
-        raise TypeError("expected x to be a ht.DNDarray, but was {}".format(type(x)))
+        raise TypeError(f"expected x to be a ht.DNDarray, but was {type(x)}")
     if weights is not None and not isinstance(weights, DNDarray):
-        raise TypeError("expected weights to be a ht.DNDarray, but was {}".format(type(x)))
+        raise TypeError(f"expected weights to be a ht.DNDarray, but was {type(x)}")
     axis = stride_tricks.sanitize_axis(x.shape, axis)
 
     if weights is None:
         result = mean(x, axis)
         num_elements = x.gnumel / result.gnumel
         cumwgt = factories.empty(1, dtype=result.dtype)
         cumwgt.larray = torch.tensor(num_elements)
@@ -302,14 +302,15 @@
 
     if returned:
         if cumwgt.gshape != result.gshape:
             cumwgt = factories.array(
                 torch.broadcast_tensors(cumwgt.larray, result.larray)[0],
                 is_split=result.split,
                 device=result.device,
+                comm=result.comm,
                 copy=False,
             )
         return (result, cumwgt)
 
     return result
 
 
@@ -763,30 +764,30 @@
         res = m4 / arithmetics.pow(m2, 2.0)
         if unbiased:
             res = ((n - 1.0) / ((n - 2.0) * (n - 3.0))) * ((n + 1.0) * res - 3 * (n - 1.0)) + 3.0
         if Fischer:
             res -= 3.0
         return res.item() if res.gnumel == 1 else res
     elif isinstance(axis, (list, tuple)):
-        raise TypeError("axis cannot be a list or a tuple, currently {}".format(type(axis)))
+        raise TypeError(f"axis cannot be a list or a tuple, currently {type(axis)}")
     else:
         return __moment_w_axis(__torch_kurtosis, x, axis, None, unbiased, Fischer)
 
 
 DNDarray.kurtosis: Callable[
     [DNDarray, int, bool, bool], DNDarray
 ] = lambda x, axis=None, unbiased=True, Fischer=True: kurtosis(x, axis, unbiased, Fischer)
 DNDarray.kurtosis.__doc__ = average.__doc__
 
 
 def max(
     x: DNDarray,
     axis: Optional[Union[int, Tuple[int, ...]]] = None,
     out: Optional[DNDarray] = None,
-    keepdim: Optional[bool] = None,
+    keepdims: Optional[bool] = None,
 ) -> DNDarray:
     # TODO: initial : scalar, optional Issue #101
     """
     Return the maximum along a given axis.
 
     Parameters
     ----------
@@ -795,15 +796,15 @@
     axis : None or int or Tuple[int,...], optional
         Axis or axes along which to operate. By default, flattened input is used.
         If this is a tuple of ints, the maximum is selected over multiple axes,
         instead of a single axis or all the axes as before.
     out : DNDarray, optional
         Tuple of two output arrays ``(max, max_indices)``. Must be of the same shape and buffer length as the expected
         output. The minimum value of an output element. Must be present to allow computation on empty slice.
-    keepdim : bool, optional
+    keepdims : bool, optional
         If this is set to ``True``, the axes which are reduced are left in the result as dimensions with size one.
         With this option, the result will broadcast correctly against the original array.
 
     Examples
     --------
     >>> a = ht.float32([
         [1, 2, 3],
@@ -823,21 +824,21 @@
         result = torch.max(*args, **kwargs)
         if isinstance(result, tuple):
             result = result[0]
         return result
 
     smallest_value = -sanitation.sanitize_infinity(x)
     return _operations.__reduce_op(
-        x, local_max, MPI.MAX, axis=axis, out=out, neutral=smallest_value, keepdim=keepdim
+        x, local_max, MPI.MAX, axis=axis, out=out, neutral=smallest_value, keepdims=keepdims
     )
 
 
 DNDarray.max: Callable[
     [DNDarray, Union[int, Tuple[int, ...]], DNDarray, bool], DNDarray
-] = lambda x, axis=None, out=None, keepdim=None: max(x, axis, out, keepdim)
+] = lambda x, axis=None, out=None, keepdims=None: max(x, axis, out, keepdims)
 DNDarray.max.__doc__ = max.__doc__
 
 
 def maximum(x1: DNDarray, x2: DNDarray, out: Optional[DNDarray] = None) -> DNDarray:
     """
     Compares two ``DNDarrays`` and returns a new :class:`~heat.core.dndarray.DNDarray` containing the element-wise maxima.
     The ``DNDarrays`` must have the same shape, or shapes that can be broadcast to a single shape.
@@ -1010,37 +1011,37 @@
 
 DNDarray.mean: Callable[[DNDarray, Union[int, List, Tuple]], DNDarray] = lambda x, axis=None: mean(
     x, axis
 )
 DNDarray.mean.__doc__ = mean.__doc__
 
 
-def median(x: DNDarray, axis: Optional[int] = None, keepdim: bool = False) -> DNDarray:
+def median(x: DNDarray, axis: Optional[int] = None, keepdims: bool = False) -> DNDarray:
     """
     Compute the median of the data along the specified axis.
     Returns the median of the ``DNDarray`` elements.
 
     Parameters
     ----------
     x : DNDarray
         Input tensor
     axis : int, or None, optional
         Axis along which the median is computed. Default is ``None``, i.e.,
         the median is computed along a flattened version of the ``DNDarray``.
 
-    keepdim : bool, optional
+    keepdims : bool, optional
         If True, the axes which are reduced are left in the result as dimensions with size one.
         With this option, the result can broadcast correctly against the original array ``a``.
     """
-    return percentile(x, q=50, axis=axis, keepdim=keepdim)
+    return percentile(x, q=50, axis=axis, keepdims=keepdims)
 
 
 DNDarray.median: Callable[
     [DNDarray, int, bool], DNDarray
-] = lambda x, axis=None, keepdim=False: median(x, axis, keepdim)
+] = lambda x, axis=None, keepdims=False: median(x, axis, keepdims)
 DNDarray.mean.__doc__ = mean.__doc__
 
 
 def __merge_moments(
     m1: torch.Tensor, m2: torch.Tensor, unbiased: bool = True
 ) -> Tuple[torch.Tensor, ...]:
     """
@@ -1063,17 +1064,15 @@
     References
     ----------
     [1] J. Bennett, R. Grout, P. Pebay, D. Roe, D. Thompson, Numerically stable, single-pass, parallel statistics
         algorithms, IEEE International Conference on Cluster Computing and Workshops, 2009, Oct 2009, New Orleans, LA,
         USA.
     """
     if len(m1) != len(m2):
-        raise ValueError(
-            "m1 and m2 must be same length, currently {} and {}".format(len(m1), len(m2))
-        )
+        raise ValueError(f"m1 and m2 must be same length, currently {len(m1)} and {len(m2)}")
     n1, n2 = m1[-1], m2[-1]
     mu1, mu2 = m1[-2], m2[-2]
     n = n1 + n2
     delta = mu2 - mu1
     mu = mu1 + n2 * (delta / n)
     if len(m1) == 2:  # merge means
         return mu, n
@@ -1111,15 +1110,15 @@
     #     return k, skew_m, var_m, mu, n
 
 
 def min(
     x: DNDarray,
     axis: Optional[Union[int, Tuple[int, ...]]] = None,
     out: Optional[DNDarray] = None,
-    keepdim: Optional[bool] = None,
+    keepdims: Optional[bool] = None,
 ) -> DNDarray:
     # TODO: initial : scalar, optional Issue #101
     """
     Return the minimum along a given axis.
 
     Parameters
     ----------
@@ -1128,15 +1127,15 @@
     axis : None or int or Tuple[int,...]
         Axis or axes along which to operate. By default, flattened input is used.
         If this is a tuple of ints, the minimum is selected over multiple axes,
         instead of a single axis or all the axes as before.
     out : Tuple[DNDarray,DNDarray], optional
         Tuple of two output arrays ``(min, min_indices)``. Must be of the same shape and buffer length as the expected
         output. The maximum value of an output element. Must be present to allow computation on empty slice.
-    keepdim : bool, optional
+    keepdims : bool, optional
         If this is set to ``True``, the axes which are reduced are left in the result as dimensions with size one.
         With this option, the result will broadcast correctly against the original array.
 
 
     Examples
     --------
     >>> a = ht.float32([
@@ -1157,21 +1156,21 @@
         result = torch.min(*args, **kwargs)
         if isinstance(result, tuple):
             result = result[0]
         return result
 
     largest_value = sanitation.sanitize_infinity(x)
     return _operations.__reduce_op(
-        x, local_min, MPI.MIN, axis=axis, out=out, neutral=largest_value, keepdim=keepdim
+        x, local_min, MPI.MIN, axis=axis, out=out, neutral=largest_value, keepdims=keepdims
     )
 
 
 DNDarray.min: Callable[
     [DNDarray, Union[int, Tuple[int, ...]], DNDarray, bool], DNDarray
-] = lambda self, axis=None, out=None, keepdim=None: min(self, axis, out, keepdim)
+] = lambda self, axis=None, out=None, keepdims=None: min(self, axis, out, keepdims)
 DNDarray.min.__doc__ = min.__doc__
 
 
 def minimum(x1: DNDarray, x2: DNDarray, out: Optional[DNDarray] = None) -> DNDarray:
     """
     Compares two ``DNDarrays`` and returns a new :class:`~heat.core.dndarray.DNDarray`  containing the element-wise minima.
     If one of the elements being compared is ``NaN``, then that element is returned. They must have the same shape,
@@ -1254,15 +1253,15 @@
         kwargs["unbiased"] = unbiased
     if Fischer:
         kwargs["Fischer"] = Fischer
 
     output_shape = list(x.shape)
     if isinstance(axis, int):
         if axis >= len(x.shape):
-            raise ValueError("axis must be < {}, currently is {}".format(len(x.shape), axis))
+            raise ValueError(f"axis must be < {len(x.shape)}, currently is {axis}")
         axis = stride_tricks.sanitize_axis(x.shape, axis)
         # only one axis given
         output_shape = [output_shape[it] for it in range(len(output_shape)) if it != axis]
         output_shape = output_shape if output_shape else (1,)
 
         if x.split is None:  # x is *not* distributed -> no need to distribute
             ret = function(x.larray, **kwargs)
@@ -1280,14 +1279,15 @@
         # singular axis given (axis) not equal to split direction (x.split)
         lcl = function(x.larray, **kwargs)
         return factories.array(
             lcl,
             is_split=x.split if axis > x.split else x.split - 1,
             dtype=x.dtype,
             device=x.device,
+            comm=x.comm,
             copy=False,
         )
     elif not isinstance(axis, (list, tuple, torch.Tensor)):
         raise TypeError(
             f"axis must be an int, tuple, list, or torch.Tensor; currently it is {type(axis)}."
         )
     # else:
@@ -1324,14 +1324,15 @@
         return elementwise_function(output_shape)
     # multiple dimensions which does *not* include the split axis
     # combine along the split axis
     return factories.array(
         function(x.larray, **kwargs),
         is_split=x.split if x.split < len(output_shape) else len(output_shape) - 1,
         device=x.device,
+        comm=x.comm,
         copy=False,
     )
 
 
 def mpi_argmax(a: str, b: str, _: Any) -> torch.Tensor:
     """
     Create the MPI function for doing argmax, for more info see :func:`argmax <argmax>`
@@ -1405,15 +1406,15 @@
 
 def percentile(
     x: DNDarray,
     q: Union[DNDarray, int, float, Tuple, List],
     axis: Optional[int] = None,
     out: Optional[DNDarray] = None,
     interpolation: str = "linear",
-    keepdim: bool = False,
+    keepdims: bool = False,
 ) -> DNDarray:
     r"""
     Compute the q-th percentile of the data along the specified axis.
     Returns the q-th percentile(s) of the tensor elements.
 
     Parameters
     ----------
@@ -1438,15 +1439,15 @@
 
         - ‘higher’: `j`.
 
         - ‘nearest’: `i` or `j`, whichever is nearest.
 
         - ‘midpoint’: :math:`(i + j) / 2`.
 
-    keepdim : bool, optional
+    keepdims : bool, optional
         If True, the axes which are reduced are left in the result as dimensions with size one.
         With this option, the result can broadcast correctly against the original array x.
     """
 
     def _local_percentile(data: torch.Tensor, axis: int, indices: torch.Tensor) -> torch.Tensor:
         # Process-local percentile calculation.
         axis_slice = data.ndim * (slice(None, None, None),)
@@ -1478,38 +1479,38 @@
 
         if axis != 0:
             # permute to have the number of percentiles at dimension 0
             dims = tuple(range(percentile.ndim))
             permute_dims = (axis,) + dims[:axis] + dims[axis + 1 :]
             percentile = percentile.permute(permute_dims)
 
-        if keepdim:
+        if keepdims:
             # leave reduced dimension as size (1,)
             percentile.unsqueeze_(dim=axis + 1)
 
         return percentile
 
     # SANITATION
     # sanitize input
     if not isinstance(x, DNDarray):
         raise TypeError("expected x to be a DNDarray, but was {}".format(type(x)))
-    if isinstance(axis, list) or isinstance(axis, tuple):
+    if isinstance(axis, (list, tuple)):
         raise NotImplementedError("ht.percentile(), tuple axis not implemented yet")
 
     if axis is None:
         if x.ndim > 1:
             x = x.flatten()
         axis = 0
 
     gshape = x.gshape
     split = x.split
     t_x = x.larray
 
     # sanitize q
-    if isinstance(q, list) or isinstance(q, tuple):
+    if isinstance(q, (list, tuple)):
         t_perc_dtype = torch.promote_types(type(q[0]), torch.float32)
         t_q = torch.tensor(q, dtype=t_perc_dtype, device=t_x.device)
     elif np.isscalar(q):
         t_perc_dtype = torch.promote_types(type(q), torch.float32)
         t_q = torch.tensor([q], dtype=t_perc_dtype, device=t_x.device)
     elif isinstance(q, DNDarray):
         if x.comm.is_distributed() and q.split is not None:
@@ -1524,15 +1525,15 @@
     perc_dtype = types.canonical_heat_type(t_perc_dtype)
 
     # q must be 1-D
     if t_q.ndim > 1:
         t_q = t_q.flatten()
 
     # shape of output DNDarray
-    if keepdim:
+    if keepdims:
         output_shape = (nperc,) + gshape[:axis] + (1,) + gshape[axis + 1 :]
     else:
         output_shape = (nperc,) + gshape[:axis] + gshape[axis + 1 :]
 
     # sanitize out
     if out is not None:
         if not isinstance(out, DNDarray):
@@ -1763,15 +1764,15 @@
         raise ValueError(f"Expected ddof >= 0, got {ddof}")
     else:
         if kwargs.get("bessel"):
             unbiased = kwargs.get("bessel")
         else:
             unbiased = bool(ddof)
         ddof = 1 if unbiased else ddof
-    if not x.is_distributed() and str(x.device)[:3] == "cpu":
+    if not x.is_distributed() and str(x.device).startswith("cpu"):
         loc = np.std(x.larray.numpy(), axis=axis, ddof=ddof)
         if loc.size == 1:
             return loc.item()
         return factories.array(loc, copy=False)
     return exponential.sqrt(var(x, axis, ddof, **kwargs), out=None)
```

### Comparing `heat-1.2.2/heat/core/stride_tricks.py` & `heat-1.3.0/heat/core/stride_tricks.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,25 +50,23 @@
         for i, (a, b) in enumerate(it):
             if a == 0 and b == 1 or b == 0 and a == 1:
                 resulting_shape[i] = 0
             elif a == 1 or b == 1 or a == b:
                 resulting_shape[i] = max(a, b)
             else:
                 raise ValueError(
-                    "operands could not be broadcast, input shapes {} {}".format(shape_a, shape_b)
+                    f"operands could not be broadcast, input shapes {shape_a} {shape_b}"
                 )
         return tuple(resulting_shape[::-1])
     except TypeError:
-        raise TypeError("operand 1 must be tuple of ints, not {}".format(type(shape_a)))
+        raise TypeError(f"operand 1 must be tuple of ints, not {type(shape_a)}")
     except NameError:
-        raise TypeError("operands must be tuples of ints, not {} and {}".format(shape_a, shape_b))
+        raise TypeError(f"operands must be tuples of ints, not {shape_a} and {shape_b}")
     except RuntimeError:
-        raise ValueError(
-            "operands could not be broadcast, input shapes {} {}".format(shape_a, shape_b)
-        )
+        raise ValueError(f"operands could not be broadcast, input shapes {shape_a} {shape_b}")
 
     return tuple(resulting_shape)
 
 
 def sanitize_axis(
     shape: Tuple[int, ...], axis: Union[int, None, Tuple[int, ...]]
 ) -> Union[int, None, Tuple[int, ...]]:
@@ -107,31 +105,30 @@
     TypeError: axis must be None or int or tuple, but was <class 'float'>
 
     """
     # scalars are handled like unsplit matrices
     if len(shape) == 0:
         axis = None
 
-    if axis is not None:
-        if not isinstance(axis, int) and not isinstance(axis, tuple):
-            raise TypeError("axis must be None or int or tuple, but was {}".format(type(axis)))
+    if axis is not None and not isinstance(axis, int) and not isinstance(axis, tuple):
+        raise TypeError(f"axis must be None or int or tuple, but was {type(axis)}")
     if isinstance(axis, tuple):
         axis = tuple(dim + len(shape) if dim < 0 else dim for dim in axis)
         for dim in axis:
             if dim < 0 or dim >= len(shape):
-                raise ValueError("axis {} is out of bounds for shape {}".format(axis, shape))
+                raise ValueError(f"axis {axis} is out of bounds for shape {shape}")
         return axis
 
     if axis is None or 0 <= axis < len(shape):
         return axis
     elif axis < 0:
         axis += len(shape)
 
     if axis < 0 or axis >= len(shape):
-        raise ValueError("axis {} is out of bounds for shape {}".format(axis, shape))
+        raise ValueError(f"axis {axis} is out of bounds for shape {shape}")
 
     return axis
 
 
 def sanitize_shape(shape: Union[int, Tuple[int, ...]], lval: int = 0) -> Tuple[int, ...]:
     """
     Verifies and normalizes the given shape.
@@ -160,15 +157,15 @@
     >>> ht.core.stride_tricks.sanitize_shape(1.0)
     Traceback (most recent call last):
       File "<stdin>", line 1, in <module>
       File "heat/heat/core/stride_tricks.py", line 159, in sanitize_shape
         raise TypeError("expected sequence object with length >= 0 or a single integer")
     TypeError: expected sequence object with length >= 0 or a single integer
     """
-    shape = (shape,) if not hasattr(shape, "__iter__") else tuple(shape)
+    shape = tuple(shape) if hasattr(shape, "__iter__") else (shape,)
 
     for dimension in shape:
         if issubclass(type(dimension), np.integer):
             dimension = int(dimension)
         if not isinstance(dimension, int):
             raise TypeError("expected sequence object with length >= 0 or a single integer")
         if dimension < lval:
```

### Comparing `heat-1.2.2/heat/core/tiling.py` & `heat-1.3.0/heat/core/tiling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 Tiling functions/classes. With these classes, you can classes you can address blocks of data in a DNDarray
 """
 
+
 from __future__ import annotations
+import itertools
 import torch
 from typing import List, Tuple, Union
 
 from .dndarray import DNDarray
 
 __all__ = ["SplitTiles", "SquareDiagTiles"]
 
@@ -82,15 +84,15 @@
         #  3. build tile map
         lshape_map = arr.create_lshape_map()
         tile_dims = torch.zeros((arr.ndim, arr.comm.size), device=arr.device.torch_device)
         if arr.split is not None:
             tile_dims[arr.split] = lshape_map[..., arr.split]
         w_size = arr.comm.size
         for ax in range(arr.ndim):
-            if arr.split is None or not ax == arr.split:
+            if arr.split is None or ax != arr.split:
                 size = arr.gshape[ax]
                 chunk = size // w_size
                 remainder = size % w_size
                 tile_dims[ax] = chunk
                 tile_dims[ax][:remainder] += 1
 
         tile_ends_g = torch.cumsum(tile_dims, dim=1).int()
@@ -210,15 +212,15 @@
         [1/2] tensor([[17., 18.],
         [1/2]         [24., 25.]])
         [2/2] tensor([[19., 20.],
         [2/2]         [26., 27.]])
         """
         # todo: strides can be implemented with using a list of slices for each dimension
         if not isinstance(key, (tuple, slice, int, torch.tensor)):
-            raise TypeError("key type not supported: {}".format(type(key)))
+            raise TypeError(f"key type not supported: {type(key)}")
         arr = self.__DNDarray
         # if arr.comm.rank not in self.tile_locations[key]:
         #     return None
         # This filters out the processes which are not involved
         # next need to get the local indices
         # tile_ends_g has the end points, need to get the start and stop
         if arr.comm.rank not in self.tile_locations[key]:
@@ -287,17 +289,15 @@
 
         Parameters
         ----------
         key : int or slice or tuple
             which tiles to get
         """
         arb_slices = self.__get_tile_slices(key)
-        inds = []
-        for sl in arb_slices:
-            inds.append(sl.stop - sl.start)
+        inds = [sl.stop - sl.start for sl in arb_slices]
         return tuple(inds)
 
     def __setitem__(
         self,
         key: Union[int, slice, Tuple[Union[int, slice], ...]],
         value: Union[int, float, torch.Tensor],
     ) -> None:
@@ -312,17 +312,17 @@
             Value to be set on the tile
 
         Examples
         --------
         see getitem function for this class
         """
         if not isinstance(key, (tuple, slice, int, torch.Tensor)):
-            raise TypeError("key type not supported: {}".format(type(key)))
+            raise TypeError(f"key type not supported: {type(key)}")
         if not isinstance(value, (torch.Tensor, int, float)):
-            raise TypeError("value type not supported: {}".format(type(value)))
+            raise TypeError(f"value type not supported: {type(value)}")
         # todo: is it okay for cross-split setting? this can be problematic,
         #   but it is fine if the data shapes match up
         if self.__DNDarray.comm.rank not in self.tile_locations[key]:
             return None
         # this will set the tile values using the torch setitem function
         arr = self.__getitem__(key)
         arr.__setitem__(slice(0, None), value)
@@ -371,21 +371,21 @@
     -----------
     This tiling scheme is intended for use with the :func:`~heat.core.linalg.qr.qr` function.
     """
 
     def __init__(self, arr: DNDarray, tiles_per_proc: int = 2) -> None:  # noqa: D107
         # lshape_map -> rank (int), lshape (tuple of the local lshape, self.lshape)
         if not isinstance(arr, DNDarray):
-            raise TypeError("arr must be a DNDarray, is currently a {}".format(type(self)))
+            raise TypeError(f"arr must be a DNDarray, is currently a {type(self)}")
         if not isinstance(tiles_per_proc, int):
-            raise TypeError("tiles_per_proc must be an int, is currently a {}".format(type(self)))
+            raise TypeError(f"tiles_per_proc must be an int, is currently a {type(self)}")
         if tiles_per_proc < 1:
-            raise ValueError("Tiles per process must be >= 1, currently: {}".format(tiles_per_proc))
+            raise ValueError(f"Tiles per process must be >= 1, currently: {tiles_per_proc}")
         if len(arr.shape) != 2:
-            raise ValueError("Arr must be 2 dimensional, current shape {}".format(arr.shape))
+            raise ValueError(f"Arr must be 2 dimensional, current shape {arr.shape}")
 
         lshape_map = arr.create_lshape_map(force_check=True)
 
         # if there is only one element of the diagonal on the next process
         d = 1 if tiles_per_proc <= 2 else tiles_per_proc - 1
         redist = torch.where(
             torch.cumsum(lshape_map[..., arr.split], dim=0) >= arr.gshape[arr.split - 1] - d
@@ -416,19 +416,17 @@
             # re-test for empty processes and remove empty rows
             empties = torch.where(lshape_map[..., 0] == 0)[0]
             if empties.numel() > 0:
                 # need to remove the entry in the rows per process
                 for e in empties:
                     row_per_proc_list[e] = 0
 
-        row_inds = []
-        for c in col_inds:
-            # set the row indices to be the same for all of the column indices
-            #   (however many there are)
-            row_inds.append(c)
+        row_inds = list(col_inds)
+        # set the row indices to be the same for all of the column indices
+        #   (however many there are)
 
         if arr.split == 0 and arr.gshape[0] < arr.gshape[1]:
             # need to adjust the very last tile to be the remaining
             col_inds[-1] = arr.gshape[1] - sum(col_inds[:-1])
 
         # if there is too little data on the last tile then combine them
         if arr.split == 0 and last_diag_pr < arr.comm.size - 1:
@@ -526,15 +524,15 @@
     ) -> None:
         """
         Add more columns after the diagonal ends if ``m<n`` and ``arr.split==1``
         """
         # need to add to col inds with the rest of the columns
         tile_columns = sum(col_per_proc_list)
         r = last_diag_pr + 1
-        for i in range(len(col_inds), tile_columns):
+        for _ in range(len(col_inds), tile_columns):
             col_inds.append(lshape_map[r, 1])
             r += 1
         # if the 1st dim is > 0th dim then in split=1 the cols need to be extended
         col_proc_ind = torch.cumsum(
             torch.tensor(col_per_proc_list, device=arr.larray.device), dim=0
         )
         for pr in range(arr.comm.size):
@@ -687,24 +685,24 @@
         Adjust the rows on the processes which are greater than the last diagonal processs to have
         rows which are chunked evenly into ``tiles_per_proc`` rows.
         """
         nz = torch.nonzero(
             input=torch.tensor(row_inds, device=arr.larray.device) == 0, as_tuple=False
         )
         lp_map = lshape_map.tolist()
-        for i in range(last_diag_pr.item() + 1, arr.comm.size):
-            # loop over all of the rest of the processes
-            for t in range(tiles_per_proc):
-                _, lshape, _ = arr.comm.chunk(lp_map[i], 0, rank=t, w_size=tiles_per_proc)
-                # row_inds[nz[0].item()] = lshape[0]
-                if row_inds[-1] == 0:
-                    row_inds[-1] = lshape[0]
-                else:
-                    row_inds.append(lshape[0])
-                nz = nz[1:]
+        for i, t in itertools.product(
+            range(last_diag_pr.item() + 1, arr.comm.size), range(tiles_per_proc)
+        ):
+            _, lshape, _ = arr.comm.chunk(lp_map[i], 0, rank=t, w_size=tiles_per_proc)
+            # row_inds[nz[0].item()] = lshape[0]
+            if row_inds[-1] == 0:
+                row_inds[-1] = lshape[0]
+            else:
+                row_inds.append(lshape[0])
+            nz = nz[1:]
 
     @staticmethod
     def __last_tile_row_adjust_sp1(arr: DNDarray, row_inds: List[int, ...]) -> None:
         """
         Add extra row/s if there is space below the diagonal (``split=1``)
         """
         if arr.gshape[0] - arr.gshape[1] > 10:  # todo: determine best value for this
@@ -850,15 +848,15 @@
         >>> print(a_tiles.get_start_stop(key=(3, 3)))
         [0/1] (tensor(2), tensor(6), tensor(8), tensor(10))
         [1/1] (tensor(2), tensor(6), tensor(8), tensor(10))
         """
         split = self.__DNDarray.split
         pr = self.tile_map[key][..., 2].unique()
         if pr.numel() > 1:
-            raise ValueError("Tile/s must be located on one process. currently on: {}".format(pr))
+            raise ValueError(f"Tile/s must be located on one process. currently on: {pr}")
         row_inds = self.row_indices + [self.__DNDarray.gshape[0]]
         col_inds = self.col_indices + [self.__DNDarray.gshape[1]]
 
         row_start = row_inds[sum(self.tile_rows_per_process[:pr]) if split == 0 else 0]
         col_start = col_inds[sum(self.tile_columns_per_process[:pr]) if split == 1 else 0]
 
         if isinstance(key, int):
@@ -920,17 +918,15 @@
         [0/1]         [0., 0., 0.]])
         [1/1] None
         """
         arr = self.__DNDarray
         tile_map = self.__tile_map
         local_arr = arr.larray
         if not isinstance(key, (int, tuple, slice)):
-            raise TypeError(
-                "key must be an int, tuple, or slice, is currently {}".format(type(key))
-            )
+            raise TypeError(f"key must be an int, tuple, or slice, is currently {type(key)}")
         involved_procs = tile_map[key][..., 2].unique()
         if involved_procs.nelement() == 1 and involved_procs == arr.comm.rank:
             st0, sp0, st1, sp1 = self.get_start_stop(key=key)
             return local_arr[st0:sp0, st1:sp1]
         elif involved_procs.nelement() > 1:
             raise ValueError("Slicing across splits is not allowed")
         else:
@@ -1093,17 +1089,15 @@
         Notes
         -----
         This function overwrites most, if not all, of the elements of this class. Intended for use with the Q matrix,
         to match the tiling of a/R. For this to work properly it is required that the 0th dim of both matrices is equal
         """
         if not isinstance(tiles_to_match, SquareDiagTiles):
             raise TypeError(
-                "tiles_to_match must be a SquareDiagTiles object, currently: {}".format(
-                    type(tiles_to_match)
-                )
+                f"tiles_to_match must be a SquareDiagTiles object, currently: {type(tiles_to_match)}"
             )
         base_dnd = self.__DNDarray
         match_dnd = tiles_to_match.__DNDarray
         # this map will take the same tile row and column sizes up to the last diagonal row/column
         # the last row/column is determined by the number of rows/columns on the non-split dimension
         if base_dnd.split == match_dnd.split == 0:
             # this implies that the gshape[0]'s are equal
```

### Comparing `heat-1.2.2/heat/core/trigonometrics.py` & `heat-1.3.0/heat/core/trigonometrics.py`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/core/types.py` & `heat-1.3.0/heat/core/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,26 +99,25 @@
         device: devices.Device
             The device on which to place the created DNDarray
         comm: communication.Communication
             The MPI communication object to use in distribution and further operations
         """
         torch_type = cls.torch_type()
         if torch_type is NotImplemented:
-            raise TypeError("cannot create '{}' instances".format(cls))
+            raise TypeError(f"cannot create '{cls}' instances")
 
         value_count = len(value)
 
         # sanitize the distributed processing flags
         comm = communication.sanitize_comm(comm)
         device = devices.sanitize_device(device)
 
         # check whether there are too many arguments
         if value_count >= 2:
-            raise TypeError("function takes at most 1 argument ({} given)".format(value_count))
-        # if no value is given, we will initialize the value to be zero
+            raise TypeError(f"function takes at most 1 argument ({value_count} given)")
         elif value_count == 0:
             value = ((0,),)
 
         # otherwise, attempt to create a torch tensor of given type
         try:
             array = value[0]._DNDarray__array.type(torch_type)
             return dndarray.DNDarray(
@@ -510,19 +509,22 @@
     # already a heat type
     try:
         if issubclass(a_type, datatype):
             return a_type
     except TypeError:
         pass
 
+    # extract type of numpy.dtype
+    a_type = getattr(a_type, "type", a_type)
+
     # try to look the corresponding type up
     try:
         return __type_mappings[a_type]
     except KeyError:
-        raise TypeError("data type {} is not understood".format(a_type))
+        raise TypeError(f"data type {a_type} is not understood")
 
 
 def heat_type_is_exact(ht_dtype: Type[datatype]) -> bool:
     """
     Check if HeAT type is an exact type, i.e an integer type. True if ht_dtype is an integer, False otherwise
 
     Parameters
@@ -594,15 +596,15 @@
     except TypeError:
         pass
 
     # last resort, type of the object at first position
     try:
         return canonical_heat_type(type(obj[0]))
     except (KeyError, IndexError, TypeError):
-        raise TypeError("data type of {} is not understood".format(obj))
+        raise TypeError(f"data type of {obj} is not understood")
 
 
 # type code assignment
 __type_codes = collections.OrderedDict(
     [
         (bool, 0),
         (uint8, 1),
@@ -718,17 +720,17 @@
     False
     >>> ht.can_cast("i8", "i4", "same_kind")
     True
     >>> ht.can_cast("i8", "i4", "unsafe")
     True
     """
     if not isinstance(casting, str):
-        raise TypeError("expected string, found {}".format(type(casting)))
+        raise TypeError(f"expected string, found {type(casting)}")
     if casting not in __cast_kinds:
-        raise ValueError("casting must be one of {}".format(str(__cast_kinds)[1:-1]))
+        raise ValueError(f"casting must be one of {str(__cast_kinds)[1:-1]}")
 
     # obtain the types codes of the canonical HeAT types
     try:
         typecode_from = __type_codes[canonical_heat_type(from_)]
     except TypeError:
         typecode_from = __type_codes[heat_type_of(from_)]
     typecode_to = __type_codes[canonical_heat_type(to)]
@@ -986,15 +988,15 @@
         try:
             dtype = heat_type_of(dtype)
         except (KeyError, IndexError, TypeError):
             # If given type is not heat type
             pass
 
         if dtype not in _inexact:
-            raise TypeError("Data type {} not inexact, not supported".format(dtype))
+            raise TypeError(f"Data type {dtype} not inexact, not supported")
 
         return super(finfo, cls).__new__(cls)._init(dtype)
 
     def _init(self, dtype: Type[datatype]):
         _torch_finfo = torch.finfo(dtype.torch_type())
         for word in ["bits", "eps", "max", "min", "tiny"]:
             setattr(self, word, getattr(_torch_finfo, word))
@@ -1032,15 +1034,15 @@
         try:
             dtype = heat_type_of(dtype)
         except (KeyError, IndexError, TypeError):
             # If given type is not heat type
             pass
 
         if dtype not in _exact:
-            raise TypeError("Data type {} not exact, not supported".format(dtype))
+            raise TypeError(f"Data type {dtype} not exact, not supported")
 
         return super(iinfo, cls).__new__(cls)._init(dtype)
 
     def _init(self, dtype: Type[datatype]):
         _torch_iinfo = torch.iinfo(dtype.torch_type())
         for word in ["bits", "min", "max"]:
             setattr(self, word, getattr(_torch_iinfo, word))
```

### Comparing `heat-1.2.2/heat/core/version.py` & `heat-1.3.0/heat/core/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """This module contains Heat's version information."""
 
+
 major: int = 1
 """Indicates Heat's main version."""
-minor: int = 2
+minor: int = 3
 """Indicates feature extension."""
-micro: int = 2
+micro: int = 0
 """Indicates revisions for bugfixes."""
 extension: str = None
 """Indicates special builds, e.g. for specific hardware."""
 
 if not extension:
-    __version__: str = "{}.{}.{}".format(major, minor, micro)
+    __version__: str = f"{major}.{minor}.{micro}"
     """The combined version string, consisting out of major, minor, micro and possibly extension."""
 else:
-    __version__: str = "{}.{}.{}-{}".format(major, minor, micro, extension)
+    __version__: str = f"{major}.{minor}.{micro}-{extension}"
```

### Comparing `heat-1.2.2/heat/datasets/diabetes.h5` & `heat-1.3.0/heat/datasets/diabetes.h5`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/datasets/iris.csv` & `heat-1.3.0/heat/datasets/iris.csv`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/datasets/iris.h5` & `heat-1.3.0/heat/datasets/iris.h5`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/datasets/iris.nc` & `heat-1.3.0/heat/datasets/iris.nc`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/datasets/iris_X_test.csv` & `heat-1.3.0/heat/datasets/iris_X_test.csv`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/datasets/iris_X_train.csv` & `heat-1.3.0/heat/datasets/iris_X_train.csv`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/datasets/iris_y_pred_proba.csv` & `heat-1.3.0/heat/datasets/iris_y_pred_proba.csv`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/graph/laplacian.py` & `heat-1.3.0/heat/graph/laplacian.py`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/naive_bayes/gaussianNB.py` & `heat-1.3.0/heat/naive_bayes/gaussianNB.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,26 +79,23 @@
         y : DNDarray
             Labels for training set. Shape = (n_samples, )
         sample_weight : DNDarray, optional
             Weights applied to individual samples (1. for unweighted). Shape = (n_samples, )
         """
         # sanitize input - to be moved to sanitation module, cf. #468
         if not isinstance(x, ht.DNDarray):
-            raise ValueError("input needs to be a ht.DNDarray, but was {}".format(type(x)))
+            raise ValueError(f"input needs to be a ht.DNDarray, but was {type(x)}")
         if not isinstance(y, ht.DNDarray):
-            raise ValueError("input needs to be a ht.DNDarray, but was {}".format(type(y)))
+            raise ValueError(f"input needs to be a ht.DNDarray, but was {type(y)}")
         if y.ndim != 1:
-            raise ValueError("expected y to be a 1-D tensor, is {}-D".format(y.ndim))
-        if sample_weight is not None:
-            if not isinstance(sample_weight, ht.DNDarray):
-                raise ValueError(
-                    "sample_weight needs to be a ht.DNDarray, but was {}".format(
-                        type(sample_weight)
-                    )
-                )
+            raise ValueError(f"expected y to be a 1-D tensor, is {y.ndim}-D")
+        if sample_weight is not None and not isinstance(sample_weight, ht.DNDarray):
+            raise ValueError(
+                f"sample_weight needs to be a ht.DNDarray, but was {type(sample_weight)}"
+            )
         classes = ht.unique(y, sorted=True)
         if classes.split is not None:
             classes = ht.resplit(classes, axis=None)
 
         return self.__partial_fit(x, y, classes, _refit=True, sample_weight=sample_weight)
 
     def __check_partial_fit_first_call(self, classes: Optional[DNDarray] = None) -> bool:
@@ -116,16 +113,15 @@
             unique_labels = classes
             if getattr(self, "classes_", None) is None:
                 self.classes_ = unique_labels
                 # This is the first call to partial_fit
                 return True
             if not ht.equal(self.classes_, unique_labels):
                 raise ValueError(
-                    "`classes={}` is not the same as on last call "
-                    "to partial_fit, was: {}".format(classes, self.classes_)
+                    f"`classes={classes}` is not the same as on last call to partial_fit, was: {self.classes_}"
                 )
         # classes is None and self.classes_ has already previously been set:
         # nothing to do
         return False
 
     @staticmethod
     def __update_mean_variance(
@@ -260,29 +256,27 @@
             (ie, throw away any past fitting and start over).
         sample_weight : DNDarray, optional
             Weights applied to individual samples (1. for unweighted). Shape = (n_samples,)
         """
         # TODO: sanitize x and y shape: sanitation/validation module, cf. #468
         n_samples = x.shape[0]
         if x.ndim != 2:
-            raise ValueError("expected x to be a 2-D tensor, is {}-D".format(x.ndim))
+            raise ValueError(f"expected x to be a 2-D tensor, is {x.ndim}-D")
         if y.shape[0] != n_samples:
             raise ValueError(
-                "y.shape[0] must match number of samples {}, is {}".format(n_samples, y.shape[0])
+                f"y.shape[0] must match number of samples {n_samples}, is {y.shape[0]}"
             )
 
         # TODO: sanitize sample_weight: sanitation/validation module, cf. #468
         if sample_weight is not None:
             if sample_weight.ndim != 1:
                 raise ValueError("Sample weights must be 1D tensor")
             if sample_weight.shape != (n_samples,):
                 raise ValueError(
-                    "sample_weight.shape == {}, expected {}!".format(
-                        sample_weight.shape, (n_samples,)
-                    )
+                    f"sample_weight.shape == {sample_weight.shape}, expected {(n_samples, )}!"
                 )
 
         # If the ratio of data variance between dimensions is too small, it
         # will cause numerical errors. To address this, we artificially
         # boost the variance by epsilon, a small fraction of the standard
         # deviation of the largest dimension.
         self.epsilon_ = self.var_smoothing * ht.var(x, axis=0).max()
@@ -322,30 +316,27 @@
                 # Initialize the priors to zeros for each class
                 self.class_prior_ = ht.zeros(
                     len(self.classes_), dtype=ht.float64, split=None, device=x.device
                 )
         else:
             if x.shape[1] != self.theta_.shape[1]:
                 raise ValueError(
-                    "Number of features {} does not match previous data {}.".format(
-                        x.shape[1], self.theta_.shape[1]
-                    )
+                    f"Number of features {x.shape[1]} does not match previous data {self.theta_.shape[1]}."
                 )
             # Put epsilon back in each time
             self.sigma_[:, :] -= self.epsilon_
 
         classes = self.classes_
 
         unique_y = ht.unique(y, sorted=True).resplit_(None)
         unique_y_in_classes = ht.eq(unique_y, classes)
 
         if not ht.all(unique_y_in_classes):
             raise ValueError(
-                "The target label(s) {} in y do not exist in the "
-                "initial classes {}".format(unique_y[~unique_y_in_classes], classes)
+                f"The target label(s) {unique_y[~unique_y_in_classes]} in y do not exist in the initial classes {classes}"
             )
         # from now on: extract torch tensors for local operations
         # DNDarrays for distributed operations only
         for y_i in unique_y.larray:
             # assuming classes.split is None
             if y_i in classes.larray:
                 i = torch.where(classes.larray == y_i)[0].item()
@@ -378,15 +369,15 @@
             self.class_count_.larray[:, i] += N_i
 
         self.sigma_[:, :] += self.epsilon_
 
         # Update only if no priors are provided
         if self.priors is None:
             # distributed class_count_: sum along distribution axis
-            self.class_count_ = self.class_count_.sum(axis=0, keepdim=True)
+            self.class_count_ = self.class_count_.sum(axis=0, keepdims=True)
             # Empirical prior, with sample_weight taken into account
             self.class_prior_ = (self.class_count_ / self.class_count_.sum()).squeeze(0)
 
         return self
 
     def __joint_log_likelihood(self, x: DNDarray) -> DNDarray:
         """
@@ -405,15 +396,15 @@
         return joint_log_likelihood
 
     def logsumexp(
         self,
         a: DNDarray,
         axis: Optional[Union[int, Tuple[int, ...]]] = None,
         b: Optional[DNDarray] = None,
-        keepdim: bool = False,
+        keepdims: bool = False,
         return_sign: bool = False,
     ) -> DNDarray:
         """
         Adapted to HeAT from scikit-learn.
         Compute the log of the sum of exponentials of input elements. The result, ``np.log(np.sum(np.exp(a)))``
         calculated in a numerically more stable way. If `b` is given then ``np.log(np.sum(b*np.exp(a)))``
         is returned.
@@ -421,15 +412,15 @@
         Parameters
         ----------
         a : DNDarray
             Input array.
         axis : None or int or Tuple [int,...], optional
             Axis or axes over which the sum is taken. By default ``axis`` is ``None``,
             and all elements are summed.
-        keepdim : bool, optional
+        keepdims : bool, optional
             If this is set to ``True``, the axes which are reduced are left in the
             result as dimensions with size one. With this option, the result
             will broadcast correctly against the original array.
         b : DNDarray, optional
             Scaling factor for ``exp(a)`` must be of the same shape as ``a`` or
             broadcastable to ``a``. These values may be negative in order to
             implement subtraction.
@@ -442,37 +433,37 @@
             #TODO If return_sign is True, this will be an array of floating-point
             numbers matching res and +1, 0, or -1 depending on the sign
             of the result. If ``False``, only one result is returned.
         """
         if b is not None:
             raise NotImplementedError("Not implemented for weighted logsumexp")
 
-        a_max = ht.max(a, axis=axis, keepdim=True)
+        a_max = ht.max(a, axis=axis, keepdims=True)
 
         # TODO: sanitize a_max / implement isfinite(): sanitation module, cf. #468
         # if a_max.ndim > 0:
         #     a_max[~np.isfinite(a_max)] = 0
         # elif not np.isfinite(a_max):
         #     a_max = 0
 
         # TODO: reinstate after allowing b not None
         # if b is not None:
         #     b = np.asarray(b)
         #     tmp = b * np.exp(a - a_max)
         # else:
         tmp = ht.exp(a - a_max)
 
-        s = ht.sum(tmp, axis=axis, keepdim=keepdim)
+        s = ht.sum(tmp, axis=axis, keepdims=keepdims)
         if return_sign:
             raise NotImplementedError("Not implemented for return_sign")
             # sgn = np.sign(s)  # TODO: np.sign
             # s *= sgn  # /= makes more sense but we need zero -> zero
         out = ht.log(s)
 
-        if not keepdim:
+        if not keepdims:
             a_max = ht.squeeze(a_max, axis=axis)
         out += a_max
 
         # if return_sign: #TODO: np.sign
         #    return out, sgn
         # else:
         return out
@@ -486,15 +477,15 @@
         ----------
         x : DNDarray
             Input data with shape (n_samples, n_features)
         """
         # sanitize input
         # TODO: sanitation/validation module, cf. #468
         if not isinstance(x, ht.DNDarray):
-            raise ValueError("input needs to be a ht.DNDarray, but was {}".format(type(x)))
+            raise ValueError(f"input needs to be a ht.DNDarray, but was {type(x)}")
         jll = self.__joint_log_likelihood(x)
         return self.classes_[ht.argmax(jll, axis=1)]
 
     def predict_log_proba(self, x: DNDarray) -> DNDarray:
         """
         Adapted to HeAT from scikit-learn.
         Return log-probability estimates of the samples for each class in
```

### Comparing `heat-1.2.2/heat/nn/__init__.py` & `heat-1.3.0/heat/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/nn/data_parallel.py` & `heat-1.3.0/heat/nn/data_parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,47 +61,43 @@
                 "For use with DASO please use DataParallelMultiGPU instead of DataParallel"
             )
         super(DataParallel, self).__init__()
         self.module = module
         self.comm = comm
         self.blocking_parameter_updates = blocking_parameter_updates
 
-        self._dp_optimizers = list()
+        self._dp_optimizers = []
         self._layer_wait_handles = OrderedDict()
-        self._fwd_hook_handles = list()
+        self._fwd_hook_handles = []
         # set of layers' names with active wait handles (only relevant for non-blocking)
         self._active_layers = set()
         # slices of parameters belonging to one and the same layer
-        self._param_slices = dict()
+        self._param_slices = {}
         # pytorch internal parameter indexing
-        self._param_indices = dict()
+        self._param_indices = {}
 
         # raise error if no DP optimizer is given
         if not isinstance(optimizer, (list, tuple)):
             optimizer = [optimizer]
         for i in optimizer:
             if not isinstance(i, optim.DataParallelOptimizer):
                 raise TypeError("optimizers must be optim.DataParallelOptimizer")
 
         # current implementation of non-blocking communication during parameter updates has some limitations that cause
         # fallback onto blocking in case of overstepping them
-        if not self.blocking_parameter_updates:
-            # usage of multiple optimizers isn't supported nor is the
-            # usage of optimizer with parameters being unequal to model's parameters
-            if (
-                len(optimizer) > 1
-                or list(module.parameters())
-                != optimizer[0].torch_optimizer.param_groups[0]["params"]
-            ):
-                self.blocking_parameter_updates = True
-                warnings.warn(
-                    "Usage of more than one DataParallelOptimizer causes fallback on blocking MPI "
-                    "communication during parameter updates.",
-                    stacklevel=2,
-                )
+        if not self.blocking_parameter_updates and (
+            len(optimizer) > 1
+            or list(module.parameters()) != optimizer[0].torch_optimizer.param_groups[0]["params"]
+        ):
+            self.blocking_parameter_updates = True
+            warnings.warn(
+                "Usage of more than one DataParallelOptimizer causes fallback on blocking MPI "
+                "communication during parameter updates.",
+                stacklevel=2,
+            )
 
         # assign given optimizers to this model
         for dp_optimizer in optimizer:
             self._dp_optimizers.append(dp_optimizer)
             dp_optimizer.blocking_parameter_updates = self.blocking_parameter_updates
 
         # unify parameters across nodes by unifying the random seed and resetting parameters
@@ -248,24 +244,25 @@
         ----------
         layer_name : str
             Name of the layer
         param_name : str
             Name of the parameter
         """
         # hook function for blocking gradient data exchange
+
         def _hook(grad_loc: torch.Tensor) -> torch.Tensor:
             with torch.no_grad():
                 wrk = grad_loc.to(torch.float)  # bfloat16)
             # counterbalance local gradient averaging
             wrk *= 1 / float(self.comm.size)
             # perform MPI IAllreduce to compute global gradient, returns wait handle
             wait_handle = self.comm.Iallreduce(MPI.IN_PLACE, wrk, MPI.SUM)  # mpi_sum_bf16)
             # if layer wait handle dict does not contain the layer, add it -> automatically tracks reversed layer order
             if layer_name not in self._layer_wait_handles:
-                self._layer_wait_handles[layer_name] = list()
+                self._layer_wait_handles[layer_name] = []
             # add layer to set of active layers
             self._active_layers.add(layer_name)
             # assign wait handle to its layer, layer-internal sorting by size
             # bisect.insort(
             #     self._layer_wait_handles[layer_name], (wrk.numel(), param_name, wait_handle)
             # )
             # TODO: is sorting faster? or is there any difference?
@@ -284,14 +281,15 @@
 
         Parameters
         ----------
         layer_name : str
             Name of the layer
         """
         # hook function for non-blocking parameter update
+
         def _hook(_, input_):
             # update parameters of given layer
             param_slice = self._param_slices[layer_name]
             self._iparam_update(param_slice, [layer_name])
             return input_
 
         return _hook
@@ -336,15 +334,15 @@
         self, module: torch.nn.Module, optimizer: optim.DASO, comm: MPICommunication = MPI_WORLD
     ):  # noqa: D107
         super(DataParallelMultiGPU, self).__init__()
         rank = comm.rank
         if torch.cuda.device_count() > 1:
             self.loc_gpus = torch.cuda.device_count()
             local_rank = rank % self.loc_gpus
-            device = "cuda:" + str(local_rank)
+            device = f"cuda:{str(local_rank)}"
             torch.cuda.set_device(device=device)
             module = tnn.parallel.DistributedDataParallel(module, device_ids=[local_rank])
         else:
             warnings.warn(
                 "DataParallelMultiGPU should be used with multiple GPUs per node", UserWarning
             )
         self.module = module
```

### Comparing `heat-1.2.2/heat/optim/__init__.py` & `heat-1.3.0/heat/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/optim/dp_optimizer.py` & `heat-1.3.0/heat/optim/dp_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
                 else:
                     color = 111 + i if rank in lp_ranks else 222 + i
                     key = 0 + i if rank in lp_ranks else 444 + i
                     reduced_comms.append(MPICommunication(self.comm.Split(color, key)))
                 reduced_ranks.append(tuple(lp_ranks))
             self.reduced_comms, self.reduced_ranks = reduced_comms, reduced_ranks
             self.base_loc_ranks = base_loc_ranks
-            self.device = "cuda:" + str(local_rank)
+            self.device = f"cuda:{str(local_rank)}"
             torch.cuda.set_device(device=self.device)
 
         self.current_batch, self.last_batch = 0, None
 
         self._prev_params = []
         self.epoch = 0
         self._send_mod, self._send_mod_m1 = 0, None
@@ -650,20 +650,19 @@
         self._prev_params.append([waits, params_list, shapes, batches_to_wait])
 
     @torch.no_grad()
     def _local_update(self, sending_process: Tuple) -> None:
         # use torch to send the network parameters of a single process to the other processes
         if not torch.distributed.is_initialized() or sending_process is None:
             return
-        snds = {}
-        for name, param in self.module.named_parameters():
-            if param.requires_grad:
-                snds[name] = torch.distributed.broadcast(
-                    param, sending_process, async_op=True
-                )  # default is SUM
+        snds = {
+            name: torch.distributed.broadcast(param, sending_process, async_op=True)
+            for name, param in self.module.named_parameters()
+            if param.requires_grad
+        }
         for name, param in self.module.named_parameters():
             if param.requires_grad:
                 snds[name].wait()
 
     @staticmethod
     @torch.no_grad()
     @torch.jit.script
@@ -671,15 +670,15 @@
         jtparams: torch.Tensor, iter_dict: Dict[str, torch.Tensor], cast: int
     ) -> torch.Tensor:
         """
         Jitted loop to pack the data into a flattened buffer to be sent
         """
         st = 0
         cast_type = torch.float if cast == 2 else torch.bfloat16 if cast == 0 else torch.half
-        for name, par in iter_dict.items():
+        for par in iter_dict.values():
             if par.requires_grad:
                 # flatten and prep the data for sending
                 p = torch.flatten(par)
                 p = p.to(cast_type)
                 jtparams[st : st + par.numel()] = p
                 st += par.numel()
         return jtparams
@@ -824,15 +823,15 @@
 
     def zero_grad(self) -> None:
         """
         Reset gradients of local optimizer's parameters.
         """
         # reset view onto params in order to reset all gradients
         self.local_optimizer.param_groups[0]["params"] = self.params_ref[:]
-        self.local_optimizer.zero_grad()
+        self.local_optimizer.zero_grad(set_to_none=False)
 
 
 class DataParallelOptimizer:
     """
     Uses a torch.optim.Optimizer for data parallelism. It should be used in combination with DataParallel (DP) class.
     To optimize a DP module, DP optimizer has to be passed to DP module during its initialization.
     See :func:`nn.DataParallel <heat.nn.data_parallel.DataParallel>` for a basic example of usage.
@@ -870,8 +869,8 @@
 
     def zero_grad(self) -> None:
         """
         Reset gradients of optimizer's params.
         """
         # reset view onto params in order to reset all gradients
         self.torch_optimizer.param_groups[0]["params"] = self.params_ref[:]
-        self.torch_optimizer.zero_grad()
+        self.torch_optimizer.zero_grad(set_to_none=False)
```

### Comparing `heat-1.2.2/heat/optim/utils.py` & `heat-1.3.0/heat/optim/utils.py`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/regression/lasso.py` & `heat-1.3.0/heat/regression/lasso.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,51 +129,48 @@
         y : DNDarray
             Labels, Shape = (n_samples,)
         """
         # Get number of model parameters
         _, n = x.shape
 
         if y.ndim > 2:
-            raise ValueError("y.ndim must <= 2, currently: {}".format(y.ndim))
+            raise ValueError(f"y.ndim must <= 2, currently: {y.ndim}")
         if x.ndim != 2:
-            raise ValueError("X.ndim must == 2, currently: {}".format(x.ndim))
+            raise ValueError(f"X.ndim must == 2, currently: {x.ndim}")
 
         if len(y.shape) == 1:
             y = ht.expand_dims(y, axis=1)
 
         # Initialize model parameters
         theta = ht.zeros((n, 1), dtype=float, device=x.device)
 
         # Looping until max number of iterations or convergence
         for i in range(self.max_iter):
-
             theta_old = theta.copy()
 
             # Looping through each coordinate
             for j in range(n):
-
                 X_j = ht.array(x.larray[:, j : j + 1], is_split=0)
 
                 y_est = x @ theta
                 theta_j = theta.larray[j].item()
 
                 rho = (X_j * (y - y_est + theta_j * X_j)).mean()
 
                 # Intercept parameter theta[0] not be regularized
                 if j == 0:
                     theta[j] = rho
                 else:
                     theta[j] = self.soft_threshold(rho)
 
             diff = self.rmse(theta, theta_old)
-            if self.tol is not None:
-                if diff < self.tol:
-                    self.n_iter = i + 1
-                    self.__theta = theta
-                    break
+            if self.tol is not None and diff < self.tol:
+                self.n_iter = i + 1
+                self.__theta = theta
+                break
 
         self.n_iter = i + 1
         self.__theta = theta
 
     def predict(self, x: DNDarray) -> DNDarray:
         """
         Apply lasso model to input data. First row data corresponds to interception
```

### Comparing `heat-1.2.2/heat/spatial/distance.py` & `heat-1.3.0/heat/spatial/distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,16 +125,15 @@
     Parameters
     ----------
     x : torch.Tensor
         2D tensor of size :math:`m x f`
     y : torch.Tensor
         2D tensor of size :math:`n x f`
     """
-    d = torch.sum(torch.abs(x.unsqueeze(1) - y.unsqueeze(0)), dim=2)
-    return d
+    return torch.sum(torch.abs(x.unsqueeze(1) - y.unsqueeze(0)), dim=2)
 
 
 def cdist(X: DNDarray, Y: DNDarray = None, quadratic_expansion: bool = False) -> DNDarray:
     """
     Calculate Euclidian distance between two DNDarrays:
 
     .. math:: d(x,y) = \\sqrt{(|x-y|^2)}
@@ -247,17 +246,15 @@
             if promoted_type == types.float32:
                 torch_type = torch.float32
                 mpi_type = MPI.FLOAT
             elif promoted_type == types.float64:
                 torch_type = torch.float64
                 mpi_type = MPI.DOUBLE
             else:
-                raise NotImplementedError(
-                    "Datatype {} currently not supported as input".format(X.dtype)
-                )
+                raise NotImplementedError(f"Datatype {X.dtype} currently not supported as input")
 
         d = factories.zeros(
             (X.shape[0], X.shape[0]), dtype=X.dtype, split=X.split, device=X.device, comm=X.comm
         )
 
         if X.split is None:
             d.larray = metric(X.larray, X.larray)
@@ -359,65 +356,54 @@
                         device=X.device.torch_device,
                     )
                     comm.Recv(symmetric, source=receiver, tag=num_iter)
                     d.larray[:, scolumns[0] : scolumns[1]] = symmetric.transpose(0, 1)
 
         else:
             raise NotImplementedError(
-                "Input split was X.split = {}. Splittings other than 0 or None currently not supported.".format(
-                    X.split
-                )
+                f"Input split was X.split = {X.split}. Splittings other than 0 or None currently not supported."
             )
-    # Y is not None
     else:
         if len(Y.shape) > 2:
             raise NotImplementedError(
-                "Only 2D data matrices are supported, but input shapes were X: {}, Y: {}".format(
-                    X.shape, Y.shape
-                )
+                f"Only 2D data matrices are supported, but input shapes were X: {X.shape}, Y: {Y.shape}"
             )
 
         if X.comm != Y.comm:
             raise NotImplementedError("Differing communicators not supported")
 
         if X.split is None:
             if Y.split is None:
                 split = None
             elif Y.split == 0:
                 split = 1
             else:
                 raise NotImplementedError(
-                    "Input splits were X.split = {}, Y.split = {}. Splittings other than 0 or None currently not supported.".format(
-                        X.split, Y.split
-                    )
+                    f"Input splits were X.split = {X.split}, Y.split = {Y.split}. Splittings other than 0 or None currently not supported."
                 )
         elif X.split == 0:
             split = X.split
         else:
             # ToDo: Find out if even possible
             raise NotImplementedError(
-                "Input splits were X.split = {}, Y.split = {}. Splittings other than 0 or None currently not supported.".format(
-                    X.split, Y.split
-                )
+                f"Input splits were X.split = {X.split}, Y.split = {Y.split}. Splittings other than 0 or None currently not supported."
             )
 
         promoted_type = types.promote_types(X.dtype, Y.dtype)
         promoted_type = types.promote_types(promoted_type, types.float32)
         X = X.astype(promoted_type)
         Y = Y.astype(promoted_type)
         if promoted_type == types.float32:
             torch_type = torch.float32
             mpi_type = MPI.FLOAT
         elif promoted_type == types.float64:
             torch_type = torch.float64
             mpi_type = MPI.DOUBLE
         else:
-            raise NotImplementedError(
-                "Datatype {} currently not supported as input".format(X.dtype)
-            )
+            raise NotImplementedError(f"Datatype {X.dtype} currently not supported as input")
 
         d = factories.zeros(
             (X.shape[0], Y.shape[0]), dtype=promoted_type, split=split, device=X.device, comm=X.comm
         )
 
         if X.split is None:
             d.larray = metric(X.larray, Y.larray)
@@ -481,14 +467,12 @@
                             (count, f), dtype=torch_type, device=X.device.torch_device
                         )
                         Y.comm.Recv(moving, source=sender, tag=iter)
 
                     d_ij = metric(x_, moving)
                     d.larray[:, columns[0] : columns[1]] = d_ij
 
-            else:
-                raise NotImplementedError(
-                    "Input splits were X.split = {}, Y.split = {}. Splittings other than 0 or None currently not supported.".format(
-                        X.split, Y.split
-                    )
-                )
+        elif X.split == 0:
+            raise NotImplementedError(
+                f"Input splits were X.split = {X.split}, Y.split = {Y.split}. Splittings other than 0 or None currently not supported."
+            )
     return d
```

### Comparing `heat-1.2.2/heat/utils/data/_utils.py` & `heat-1.3.0/heat/utils/data/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         stop = num_names + 1
         output_name_lcl = output_folder
         output_name_lcl += "imagenet_merged.h5"
         return start, stop, output_name_lcl
 
     train_start, train_stop, output_name_lcl_train = _find_output_name_and_stsp(num_train)
     val_start, val_stop, output_name_lcl_val = _find_output_name_and_stsp(num_val)
-    output_name_lcl_val = output_name_lcl_val[:-3] + "_validation.h5"
+    output_name_lcl_val = f"{output_name_lcl_val[:-3]}_validation.h5"
 
     # create the output files
     train_lcl_file = h5py.File(output_name_lcl_train, "w")
     dt = h5py.string_dtype(encoding="ascii")
     train_lcl_file.create_dataset("images", (2502,), chunks=(1251,), maxshape=(None,), dtype=dt)
     train_lcl_file.create_dataset("metadata", (2502, 9), chunks=(1251, 9), maxshape=(None, 9))
     train_lcl_file.create_dataset(
```

### Comparing `heat-1.2.2/heat/utils/data/datatools.py` & `heat-1.3.0/heat/utils/data/datatools.py`

 * *Files identical despite different names*

### Comparing `heat-1.2.2/heat/utils/data/mnist.py` & `heat-1.3.0/heat/utils/data/mnist.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             train=train,
             transform=transform,
             target_transform=target_transform,
             download=download,
         )
         if split != 0 and split is not None:
             raise ValueError("split must be 0 or None")
-        split = split if not test_set else None
+        split = None if test_set else split
         array = factories.array(self.data, split=split)
         targets = factories.array(self.targets, split=split)
         self.test_set = test_set
         self.partial_dataset = False
         self.comm = array.comm
         self.htdata = array
         self.httargets = targets
```

### Comparing `heat-1.2.2/heat/utils/data/partial_dataset.py` & `heat-1.3.0/heat/utils/data/partial_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         self.file = file
         self.comm = comm
         self.transforms = transforms if isinstance(transforms, (list, tuple)) else [transforms]
         self.gpu = True if torch.cuda.device_count() > 0 and use_gpu else False
         self.torch_device = "cpu"
         if torch.cuda.is_available() and use_gpu:
             dev_id = MPI_WORLD.rank % torch.cuda.device_count()
-            self.torch_device = torch.device("cuda:" + str(dev_id))
+            self.torch_device = torch.device(f"cuda:{str(dev_id)}")
             torch.cuda.set_device(dev_id)
 
         f = h5py.File(file, "r")
         # too much data for the process
         fkeys = list(f.keys())
 
         sz = f[fkeys[0]].len()
```

### Comparing `heat-1.2.2/heat.egg-info/SOURCES.txt` & `heat-1.3.0/heat.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 heat/core/types.py
 heat/core/version.py
 heat/core/linalg/__init__.py
 heat/core/linalg/basics.py
 heat/core/linalg/qr.py
 heat/core/linalg/solver.py
 heat/core/linalg/svd.py
+heat/core/linalg/svdtools.py
 heat/datasets/__init__.py
 heat/datasets/diabetes.h5
 heat/datasets/iris.csv
 heat/datasets/iris.h5
 heat/datasets/iris.nc
 heat/datasets/iris_X_test.csv
 heat/datasets/iris_X_train.csv
@@ -70,17 +71,24 @@
 heat/nn/functional.py
 heat/optim/__init__.py
 heat/optim/dp_optimizer.py
 heat/optim/lr_scheduler.py
 heat/optim/utils.py
 heat/regression/__init__.py
 heat/regression/lasso.py
+heat/sparse/__init__.py
+heat/sparse/_operations.py
+heat/sparse/arithmetics.py
+heat/sparse/dcsr_matrix.py
+heat/sparse/factories.py
+heat/sparse/manipulations.py
 heat/spatial/__init__.py
 heat/spatial/distance.py
 heat/utils/__init__.py
 heat/utils/vision_transforms.py
 heat/utils/data/__init__.py
 heat/utils/data/_utils.py
 heat/utils/data/datatools.py
 heat/utils/data/matrixgallery.py
 heat/utils/data/mnist.py
-heat/utils/data/partial_dataset.py
+heat/utils/data/partial_dataset.py
+heat/utils/data/spherical.py
```

### Comparing `heat-1.2.2/setup.py` & `heat-1.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,32 +17,34 @@
     description="A framework for high-performance data analytics and machine learning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Helmholtz Association",
     author_email="martin.siggel@dlr.de",
     url="https://github.com/helmholtz-analytics/heat",
     keywords=["data", "analytics", "tensors", "distributed", "gpu"],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 4 - Beta",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
     ],
     install_requires=[
         "mpi4py>=3.0.0",
-        "numpy>=1.13.0",
-        "torch>=1.7.0, <1.13.2",
+        "numpy>=1.20.0",
+        "torch>=1.8.0, <2.0.2",
         "scipy>=0.14.0",
         "pillow>=6.0.0",
         "torchvision>=0.8.0",
     ],
     extras_require={
         "docutils": ["docutils>=0.16"],
         "hdf5": ["h5py>=2.8.0"],
         "netcdf": ["netCDF4>=1.5.6"],
         "dev": ["pre-commit>=1.18.3"],
         "examples": ["scikit-learn>=0.24.0", "matplotlib>=3.1.0"],
+        "cb": ["perun>=0.2.0"],
     },
 )
```

