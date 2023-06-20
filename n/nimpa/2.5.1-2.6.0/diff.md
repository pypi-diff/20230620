# Comparing `tmp/nimpa-2.5.1.tar.gz` & `tmp/nimpa-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimpa-2.5.1.tar", last modified: Thu Sep 15 11:54:47 2022, max compression
+gzip compressed data, was "nimpa-2.6.0.tar", last modified: Tue Jun 20 21:27:05 2023, max compression
```

## Comparing `nimpa-2.5.1.tar` & `nimpa-2.6.0.tar`

### file list

```diff
@@ -1,60 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 11:54:47.687235 nimpa-2.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 11:54:47.679235 nimpa-2.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 11:54:47.683235 nimpa-2.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-09-15 11:53:54.000000 nimpa-2.5.1/.github/workflows/comment-bot.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-09-15 11:53:54.000000 nimpa-2.5.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-09-15 11:53:54.000000 nimpa-2.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-09-15 11:53:54.000000 nimpa-2.5.1/.mailmap
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-09-15 11:53:54.000000 nimpa-2.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-09-15 11:53:54.000000 nimpa-2.5.1/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (121)    10786 2022-09-15 11:53:54.000000 nimpa-2.5.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)     6461 2022-09-15 11:54:47.687235 nimpa-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4137 2022-09-15 11:53:54.000000 nimpa-2.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 11:54:47.683235 nimpa-2.5.1/niftypet/
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 11:54:47.683235 nimpa-2.5.1/niftypet/nimpa/
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2936 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-15 11:54:47.000000 nimpa-2.5.1/niftypet/nimpa/_dist_ver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 11:54:47.683235 nimpa-2.5.1/niftypet/nimpa/auxdata/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/auxdata/PSF-17_scl-1.npy
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/auxdata/PSF-17_scl-2.npy
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 11:54:47.683235 nimpa-2.5.1/niftypet/nimpa/img/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/img/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6662 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/img/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 11:54:47.683235 nimpa-2.5.1/niftypet/nimpa/include/
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/include/conv.h
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/include/cuhelpers.h
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/include/isub.h
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/include/nlm.h
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/include/rsmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 11:54:47.683235 nimpa-2.5.1/niftypet/nimpa/prc/
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/prc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/prc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    39467 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/prc/imio.py
--rw-r--r--   0 runner    (1001) docker     (121)     4137 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/prc/num.py
--rw-r--r--   0 runner    (1001) docker     (121)    54414 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/prc/prc.py
--rw-r--r--   0 runner    (1001) docker     (121)    39529 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/prc/regseg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 11:54:47.687235 nimpa-2.5.1/niftypet/nimpa/prc/src/
--rw-r--r--   0 runner    (1001) docker     (121)    10084 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/prc/src/conv.cu
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/prc/src/cuhelpers.cu
--rw-r--r--   0 runner    (1001) docker     (121)    11539 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/prc/src/img_module.cu
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/prc/src/isub.cu
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/prc/src/nlm.cu
--rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-09-15 11:53:54.000000 nimpa-2.5.1/niftypet/nimpa/prc/src/rsmpl.cu
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 11:54:47.687235 nimpa-2.5.1/nimpa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6461 2022-09-15 11:54:47.000000 nimpa-2.5.1/nimpa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-09-15 11:54:47.000000 nimpa-2.5.1/nimpa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 11:54:47.000000 nimpa-2.5.1/nimpa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 11:54:47.000000 nimpa-2.5.1/nimpa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-09-15 11:54:47.000000 nimpa-2.5.1/nimpa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-15 11:54:47.000000 nimpa-2.5.1/nimpa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-09-15 11:53:54.000000 nimpa-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-09-15 11:54:47.687235 nimpa-2.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2491 2022-09-15 11:53:54.000000 nimpa-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 11:54:47.687235 nimpa-2.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-15 11:53:54.000000 nimpa-2.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-15 11:53:54.000000 nimpa-2.5.1/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     5233 2022-09-15 11:53:54.000000 nimpa-2.5.1/tests/test_improc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.408407 nimpa-2.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.376407 nimpa-2.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.388407 nimpa-2.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-20 21:26:36.000000 nimpa-2.6.0/.github/workflows/comment-bot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-20 21:26:36.000000 nimpa-2.6.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-20 21:26:36.000000 nimpa-2.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-20 21:26:36.000000 nimpa-2.6.0/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-20 21:26:36.000000 nimpa-2.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-20 21:26:36.000000 nimpa-2.6.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-06-20 21:26:36.000000 nimpa-2.6.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-20 21:27:05.408407 nimpa-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-20 21:26:36.000000 nimpa-2.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.388407 nimpa-2.6.0/niftypet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.388407 nimpa-2.6.0/niftypet/nimpa/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 21:27:05.000000 nimpa-2.6.0/niftypet/nimpa/_dist_ver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.388407 nimpa-2.6.0/niftypet/nimpa/acr/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23066 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr/ioaux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.380407 nimpa-2.6.0/niftypet/nimpa/acr_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.392407 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29032 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-bone-screw.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43475 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-bottom.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    64947 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-inserts-bottoms.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    74141 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-inserts.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51732 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-lid0.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49716 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-lid1.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29661 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-0.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31700 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-1.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32804 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-main-cap-2.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54619 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-main-compartment.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36432 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_mumap/acr-screws.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.396407 nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30028 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/acr-cap.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52702 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/acr-inserts.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42033 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/acr-main.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49854 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/core_nac/acr-rng.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.396407 nimpa-2.6.0/niftypet/nimpa/acr_design/rods/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    90448 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/rods/acr-rods-ends-water.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    85997 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/rods/acr-rods-ends.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)   104781 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/rods/acr-rods-water.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    87513 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/rods/acr-rods.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.400407 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50067 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-air-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)   144632 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-bckg-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50022 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-bone-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50154 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-h2o-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43625 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-hot1-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43546 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-hot2-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43417 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-hot3-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43385 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-hot4-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)   157319 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-insrt-bckg-sampling.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)   443005 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/acr_design/sampling/acr-rods-sampling.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.400407 nimpa-2.6.0/niftypet/nimpa/auxdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/auxdata/PSF-17_scl-1.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/auxdata/PSF-17_scl-2.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.400407 nimpa-2.6.0/niftypet/nimpa/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/img/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/img/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/img/signa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.400407 nimpa-2.6.0/niftypet/nimpa/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/include/conv.h
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/include/cuhelpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/include/isub.h
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/include/nlm.h
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/include/rsmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.404407 nimpa-2.6.0/niftypet/nimpa/prc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39801 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/imio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/num.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55780 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/prc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40726 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/regseg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.404407 nimpa-2.6.0/niftypet/nimpa/prc/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/src/conv.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/src/cuhelpers.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    11539 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/src/img_module.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/src/isub.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/src/nlm.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-20 21:26:36.000000 nimpa-2.6.0/niftypet/nimpa/prc/src/rsmpl.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.404407 nimpa-2.6.0/nimpa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-20 21:27:05.000000 nimpa-2.6.0/nimpa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-20 21:27:05.000000 nimpa-2.6.0/nimpa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:27:05.000000 nimpa-2.6.0/nimpa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-20 21:27:05.000000 nimpa-2.6.0/nimpa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 21:27:05.000000 nimpa-2.6.0/nimpa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-20 21:26:36.000000 nimpa-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:27:05.408407 nimpa-2.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2664 2023-06-20 21:26:36.000000 nimpa-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:05.408407 nimpa-2.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:36.000000 nimpa-2.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-20 21:26:36.000000 nimpa-2.6.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-20 21:26:36.000000 nimpa-2.6.0/tests/test_improc.py
```

### Comparing `nimpa-2.5.1/.github/workflows/comment-bot.yml` & `nimpa-2.6.0/.github/workflows/comment-bot.yml`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/.github/workflows/test.yml` & `nimpa-2.6.0/.github/workflows/test.yml`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,16 @@
   check:
     if: github.event_name != 'pull_request' || !contains('OWNER,MEMBER,COLLABORATOR', github.event.pull_request.author_association)
     runs-on: ubuntu-latest
     name: Check
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v4
+      with:
+        python-version: '3.x'
     - name: set PYSHA
       run: echo "PYSHA=$(python -VV | sha256sum | cut -d' ' -f1)" >> $GITHUB_ENV
     - uses: actions/cache@v3
       with:
         path: ~/.cache/pre-commit
         key: pre-commit|${{ env.PYSHA }}|${{ hashFiles('.pre-commit-config.yaml') }}
     - name: dependencies
@@ -34,54 +36,51 @@
         EVENT: ${{ github.event_name }}
     - run: pre-commit run -a --show-diff-on-failure
   test:
     if: github.event_name != 'pull_request' || !contains('OWNER,MEMBER,COLLABORATOR', github.event.pull_request.author_association)
     runs-on: [self-hosted, cuda, python]
     strategy:
       matrix:
-        python: [3.7, '3.10']
+        python: [3.7, 3.11]
     name: Test py${{ matrix.python }}
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Run setup-python
-      run: setup-python -p${{ matrix.python }}
+      # `dipy` lacks PEP518 support, so requries `packaging, numpy`
+      run: setup-python -p${{ matrix.python }} packaging numpy
     - run: pip install -U -e .[dev]
+      env:
+        # https://github.com/scikit-build/scikit-build/issues/740
+        SETUPTOOLS_ENABLE_FEATURES: legacy-editable
     - run: pytest
-    - uses: codecov/codecov-action@v1
+    - uses: codecov/codecov-action@v3
     - name: Post Run setup-python
       run: setup-python -p${{ matrix.python }} -Dr
       if: ${{ always() }}
   deploy:
     needs: [check, test]
     name: PyPI Deploy
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - uses: actions/setup-python@v4
+      with:
+        python-version: '3.x'
     - id: dist
       uses: casperdcl/deploy-pypi@v2
       with:
-        requirements: twine setuptools wheel setuptools_scm[toml] ninst scikit-build
-        build: sdist
+        build: -s
         gpg_key: ${{ secrets.GPG_KEY }}
         password: ${{ secrets.PYPI_TOKEN }}
         upload: ${{ github.event_name == 'push' && startsWith(github.ref, 'refs/tags') }}
-    - id: meta
-      name: Changelog
-      run: |
-        echo ::set-output name=tag::${GITHUB_REF#refs/tags/}
-        git log --pretty='format:%d%n- %s%n%b---' $(git tag --sort=v:refname | tail -n2 | head -n1)..HEAD > _CHANGES.md
     - if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-      uses: softprops/action-gh-release@v1
+      name: Release
+      run: |
+        changelog=$(git log --pretty='format:%d%n- %s%n%b---' $(git tag --sort=v:refname | tail -n2 | head -n1)..HEAD)
+        tag="${GITHUB_REF#refs/tags/}"
+        gh release create --title "nimpa $tag beta" --draft --notes "$changelog" "$tag" dist/${{ steps.dist.outputs.targz }} dist/${{ steps.dist.outputs.targz_asc }}
       env:
-        GITHUB_TOKEN: ${{ secrets.GH_TOKEN }}
-      with:
-        name: nimpa ${{ steps.meta.outputs.tag }} stable
-        body_path: _CHANGES.md
-        draft: true
-        files: |
-          dist/${{ steps.dist.outputs.targz }}
-          dist/${{ steps.dist.outputs.targz_asc }}
+        GH_TOKEN: ${{ github.token }}
```

### Comparing `nimpa-2.5.1/.pre-commit-config.yaml` & `nimpa-2.6.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 default_language_version:
   python: python3
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.3.0
+  rev: v4.4.0
   hooks:
   - id: check-added-large-files
   - id: check-case-conflict
   - id: check-docstring-first
   - id: check-executables-have-shebangs
   - id: check-toml
   - id: check-merge-conflict
@@ -21,34 +21,35 @@
   - id: todo
     name: Check TODO
     language: pygrep
     args: [-i]
     entry: TODO
     types: [text]
     exclude: ^(.pre-commit-config.yaml|.github/workflows/test.yml)$
-- repo: https://gitlab.com/pycqa/flake8
-  rev: 3.9.2
+- repo: https://github.com/PyCQA/flake8
+  rev: 5.0.4
   hooks:
   - id: flake8
     args: [-j8]
     additional_dependencies:
     - flake8-broken-line
     - flake8-bugbear
     - flake8-comprehensions
     - flake8-debugger
     - flake8-isort
+    - flake8-pyproject
     - flake8-string-format
 - repo: https://github.com/google/yapf
-  rev: v0.32.0
+  rev: v0.40.0
   hooks:
   - id: yapf
     args: [-i]
     additional_dependencies: [toml]
 - repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
 - repo: https://github.com/doublify/pre-commit-clang-format
   rev: '6230247'
   hooks:
   - id: clang-format
     files: \.(cc?|cuh?|cxx|cpp|h|hpp|hxx|java|js)$
```

### Comparing `nimpa-2.5.1/.zenodo.json` & `nimpa-2.6.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/LICENCE` & `nimpa-2.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/PKG-INFO` & `nimpa-2.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,124 +1,122 @@
 Metadata-Version: 2.1
 Name: nimpa
-Version: 2.5.1
+Version: 2.6.0
 Summary: CUDA-accelerated Python utilities for high-throughput neuroimage processing and analysis
-Home-page: https://github.com/NiftyPET/NIMPA
-Author: Pawel Markiewicz
-Author-email: p.markiewicz@ucl.ac.uk
-Maintainer: Casper da Costa-Luis
-Maintainer-email: casper.dcl@physics.org
-License: Apache 2.0
-Project-URL: Changelog, https://github.com/NiftyPET/NIMPA/releases
-Project-URL: Documentation, https://niftypet.readthedocs.io
-Description: =======================================================
-        NIMPA: Neuro and NiftyPET Image Processing and Analysis
-        =======================================================
-        
-        |Docs| |Version| |Downloads| |Py-Versions| |DOI| |Licence| |Tests|
-        
-        NIMPA is a stand-alone Python sub-package of NiftyPET_, dedicated to high-throughput processing and analysis of brain images, particularly those, which are acquired using positron emission tomography (PET) and magnetic resonance (MR).  Although, it is an essential part of the NiftyPET_ package for seamless PET image reconstruction, NIMPA is equally well suited for independent image processing, including image trimming, upsampling and partial volume correction (PVC).
-        
-        .. _NiftyPET: https://github.com/NiftyPET/NiftyPET
-        
-        Trimming is performed in order to reduce the unused image voxels in brain imaging, when using whole body PET scanners, for which only some part of the field of view (FOV) is used.
-        
-        The upsampling is needed for more accurate extraction (sampling) of PET data using regions of interest (ROI), obtained using parcellation of the corresponding T1w MR image, usually of higher image resolution.
-        
-        PVC is needed to correct for the spill-in and spill-out of PET signal from defined ROIs (specific for any given application).
-        
-        **Documentation with installation manual and tutorials**: https://niftypet.readthedocs.io/
-        
-        Quick Install
-        ~~~~~~~~~~~~~
-        
-        Note that it's recommended (but not required) to use `conda`.
-        
-        .. code:: sh
-        
-            # cross-platform install
-            conda install -c conda-forge python=3 \
-              ipykernel numpy scipy scikit-image matplotlib ipywidgets dcm2niix
-            pip install "nimpa>=2"
-        
-        For optional `dcm2niix <https://github.com/rordenlab/dcm2niix>`_ (image conversion from DICOM to NIfTI) and/or `niftyreg <https://github.com/KCL-BMEIS/niftyreg>`_ (image registration) support, simply install them separately (``pip install dcm2niix niftyreg``).
-        
-        External CMake Projects
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        The raw C/CUDA libraries may be included in external projects using ``cmake``.
-        Simply build the project and use ``find_package(NiftyPETnimpa)``.
-        
-        .. code:: sh
-        
-            # print installation directory (after `pip install nimpa`)...
-            python -c "from niftypet.nimpa import cmake_prefix; print(cmake_prefix)"
-        
-            # ... or build & install directly with cmake
-            mkdir build && cd build
-            cmake ../niftypet && cmake --build . && cmake --install . --prefix /my/install/dir
-        
-        At this point any external project may include NIMPA as follows
-        (Once setting ``-DCMAKE_PREFIX_DIR=<installation prefix from above>``):
-        
-        .. code:: cmake
-        
-            cmake_minimum_required(VERSION 3.3 FATAL_ERROR)
-            project(myproj)
-            find_package(NiftyPETnimpa COMPONENTS improc REQUIRED)
-            add_executable(myexe ...)
-            target_link_libraries(myexe PRIVATE NiftyPET::improc)
-        
-        Licence
-        ~~~~~~~
-        
-        |Licence| |DOI|
-        
-        Copyright 2018-21
-        
-        - `Pawel J. Markiewicz <https://github.com/pjmark>`__ @ University College London
-        - `Casper O. da Costa-Luis <https://github.com/casperdcl>`__ @ University College London/King's College London
-        - `Contributors <https://github.com/NiftyPET/NIMPA/graphs/contributors>`__
-        
-        .. |Docs| image:: https://readthedocs.org/projects/niftypet/badge/?version=latest
-           :target: https://niftypet.readthedocs.io/en/latest/?badge=latest
-        .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4417633.svg
-           :target: https://doi.org/10.5281/zenodo.4417633
-        .. |Licence| image:: https://img.shields.io/pypi/l/nimpa.svg?label=licence
-           :target: https://github.com/NiftyPET/NIMPA/blob/master/LICENCE
-        .. |Tests| image:: https://img.shields.io/github/workflow/status/NiftyPET/NIMPA/Test?logo=GitHub
-           :target: https://github.com/NiftyPET/NIMPA/actions
-        .. |Downloads| image:: https://img.shields.io/pypi/dm/nimpa.svg?logo=pypi&logoColor=white&label=PyPI%20downloads
-           :target: https://pypi.org/project/nimpa
-        .. |Version| image:: https://img.shields.io/pypi/v/nimpa.svg?logo=python&logoColor=white
-           :target: https://github.com/NiftyPET/NIMPA/releases
-        .. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/nimpa.svg?logo=python&logoColor=white
-           :target: https://pypi.org/project/nimpa
-        
+Author-email: Pawel Markiewicz <p.markiewicz@ucl.ac.uk>
+Maintainer-email: Casper da Costa-Luis <casper.dcl@physics.org>
+License: Apache-2.0
+Project-URL: documentation, https://niftypet.readthedocs.io
+Project-URL: repository, https://github.com/NiftyPET/NIMPA
+Project-URL: changelog, https://github.com/NiftyPET/NIMPA/releases
 Keywords: PET,MR,processing,analysis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: dev
+Provides-Extra: plot
 Provides-Extra: cuda
 Provides-Extra: dcm2niix
-Provides-Extra: dev
 Provides-Extra: niftyreg
-Provides-Extra: plot
+License-File: LICENCE
+
+=======================================================
+NIMPA: Neuro and NiftyPET Image Processing and Analysis
+=======================================================
+
+|Docs| |Version| |Downloads| |Py-Versions| |DOI| |Licence| |Tests|
+
+NIMPA is a stand-alone Python sub-package of NiftyPET_, dedicated to high-throughput processing and analysis of brain images, particularly those, which are acquired using positron emission tomography (PET) and magnetic resonance (MR).  Although, it is an essential part of the NiftyPET_ package for seamless PET image reconstruction, NIMPA is equally well suited for independent image processing, including image trimming, upsampling and partial volume correction (PVC).
+
+.. _NiftyPET: https://github.com/NiftyPET/NiftyPET
+
+Trimming is performed in order to reduce the unused image voxels in brain imaging, when using whole body PET scanners, for which only some part of the field of view (FOV) is used.
+
+The upsampling is needed for more accurate extraction (sampling) of PET data using regions of interest (ROI), obtained using parcellation of the corresponding T1w MR image, usually of higher image resolution.
+
+PVC is needed to correct for the spill-in and spill-out of PET signal from defined ROIs (specific for any given application).
+
+**Documentation with installation manual and tutorials**: https://niftypet.readthedocs.io/
+
+Quick Install
+~~~~~~~~~~~~~
+
+Note that it's recommended (but not required) to use `conda`.
+
+.. code:: sh
+
+    # cross-platform install
+    conda install -c conda-forge python=3 \
+      ipykernel numpy scipy scikit-image matplotlib ipywidgets dipy nibabel pydicom
+    pip install "nimpa>=2"
+
+For optional `dcm2niix <https://github.com/rordenlab/dcm2niix>`_ (image conversion from DICOM to NIfTI) and/or `niftyreg <https://github.com/KCL-BMEIS/niftyreg>`_ (image registration) support, simply install them separately (``pip install dcm2niix niftyreg``).
+
+External CMake Projects
+~~~~~~~~~~~~~~~~~~~~~~~
+
+The raw C/CUDA libraries may be included in external projects using ``cmake``.
+Simply build the project and use ``find_package(NiftyPETnimpa)``.
+
+.. code:: sh
+
+    # print installation directory (after `pip install nimpa`)...
+    python -c "from niftypet.nimpa import cmake_prefix; print(cmake_prefix)"
+
+    # ... or build & install directly with cmake
+    mkdir build && cd build
+    cmake ../niftypet && cmake --build . && cmake --install . --prefix /my/install/dir
+
+At this point any external project may include NIMPA as follows
+(Once setting ``-DCMAKE_PREFIX_DIR=<installation prefix from above>``):
+
+.. code:: cmake
+
+    cmake_minimum_required(VERSION 3.3 FATAL_ERROR)
+    project(myproj)
+    find_package(NiftyPETnimpa COMPONENTS improc REQUIRED)
+    add_executable(myexe ...)
+    target_link_libraries(myexe PRIVATE NiftyPET::improc)
+
+Licence
+~~~~~~~
+
+|Licence| |DOI|
+
+Copyright 2018-21
+
+- `Pawel J. Markiewicz <https://github.com/pjmark>`__ @ University College London
+- `Casper O. da Costa-Luis <https://github.com/casperdcl>`__ @ University College London/King's College London
+- `Contributors <https://github.com/NiftyPET/NIMPA/graphs/contributors>`__
+
+.. |Docs| image:: https://readthedocs.org/projects/niftypet/badge/?version=latest
+   :target: https://niftypet.readthedocs.io/en/latest/?badge=latest
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4417633.svg
+   :target: https://doi.org/10.5281/zenodo.4417633
+.. |Licence| image:: https://img.shields.io/pypi/l/nimpa.svg?label=licence
+   :target: https://github.com/NiftyPET/NIMPA/blob/master/LICENCE
+.. |Tests| image:: https://img.shields.io/github/workflow/status/NiftyPET/NIMPA/Test?logo=GitHub
+   :target: https://github.com/NiftyPET/NIMPA/actions
+.. |Downloads| image:: https://img.shields.io/pypi/dm/nimpa.svg?logo=pypi&logoColor=white&label=PyPI%20downloads
+   :target: https://pypi.org/project/nimpa
+.. |Version| image:: https://img.shields.io/pypi/v/nimpa.svg?logo=python&logoColor=white
+   :target: https://github.com/NiftyPET/NIMPA/releases
+.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/nimpa.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/nimpa
```

### Comparing `nimpa-2.5.1/README.rst` & `nimpa-2.6.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 Note that it's recommended (but not required) to use `conda`.
 
 .. code:: sh
 
     # cross-platform install
     conda install -c conda-forge python=3 \
-      ipykernel numpy scipy scikit-image matplotlib ipywidgets dcm2niix
+      ipykernel numpy scipy scikit-image matplotlib ipywidgets dipy nibabel pydicom
     pip install "nimpa>=2"
 
 For optional `dcm2niix <https://github.com/rordenlab/dcm2niix>`_ (image conversion from DICOM to NIfTI) and/or `niftyreg <https://github.com/KCL-BMEIS/niftyreg>`_ (image registration) support, simply install them separately (``pip install dcm2niix niftyreg``).
 
 External CMake Projects
 ~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `nimpa-2.5.1/niftypet/CMakeLists.txt` & `nimpa-2.6.0/niftypet/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/niftypet/nimpa/__init__.py` & `nimpa-2.6.0/niftypet/nimpa/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,69 +18,88 @@
     # utils
     'LOG_FORMAT', 'LogHandler',
     # config
     'path_resources', 'resources', 'cmake_prefix',
     # numcu
     'add', 'div', 'mul',
     # improc
-    'conv_separable', 'isub', 'nlm',
+    'conv_separable', 'isub', 'nlm', 'aff_dist', 'centre_mass_rel',
     # core
-    'create_disk', 'imdiff', 'imscroll', 'profile_points', 'imtrimup',
+    'create_disk', 'get_cylinder', 'imdiff', 'imscroll', 'profile_points', 'imtrimup',
     'affine_fsl', 'affine_dipy', 'affine_niftyreg',
     'array2nii', 'bias_field_correction',
     'centre_mass_img', 'centre_mass_corr', 'coreg_spm', 'coreg_vinci',
     'create_dir', 'create_mask', 'ct2mu',
-    'dcm2im', 'dcm2nii', 'dcmanonym', 'dcminfo', 'dcmsort',
+    'dcm2im', 'dcm2nii', 'dcmanonym', 'dcminfo', 'dcmsort', 'isdcm', 'dcmdir',
     'dice_coeff', 'dice_coeff_multiclass', 'fwhm2sig', 'getmgh', 'getnii', 'mgh2nii',
     'getnii_descr', 'im_cut', 'imfill', 'imsmooth', 'iyang', 'motion_reg', 'nii_gzip',
     'nii_modify', 'nii_ugzip', 'niisort', 'orientnii', 'pet2pet_rigid', 'pick_t1w',
     'psf_gaussian', 'psf_measured', 'pvc_iyang', 'realign_mltp_spm', 'resample_fsl',
     'resample_mltp_spm', 'resample_niftyreg', 'resample_spm', 'resample_vinci', 'resample_dipy',
-    'time_stamp', 'rem_chars'] # yapf: disable
+    'time_stamp', 'rem_chars',
+    # Signa
+    'pifa2nii', 'nii2pifa',
+    # ACR
+    'acr'
+    # 'get_params', 'get_paths', 'extract_reso_part', 'sampling_masks'
+    # 'create_mumap_core', 'create_nac_core', 'create_reso', 'create_sampl_reso', 'create_sampl',
+    # 'standard_analysis', 'estimate_fwhm'
+    ] # yapf: disable
+
+from os import fspath
+
+try:          # py<3.9
+    import importlib_resources as iresources
+except ImportError:
+    from importlib import resources as iresources
 
 try:
     from numcu import add, div, mul
 except ImportError:
     pass
-from pkg_resources import resource_filename
 
 from niftypet.ninst import cudasetup as cs
 from niftypet.ninst.dinf import dev_info, gpuinfo
 from niftypet.ninst.tools import LOG_FORMAT, LogHandler, path_resources, resources
 
-from .img import create_disk, imdiff, imscroll, profile_points
+from . import acr
+from .img import create_disk, get_cylinder, imdiff, imscroll, nii2pifa, pifa2nii, profile_points
 from .prc import imtrimup  # for backward compatibility
 from .prc import (
+    aff_dist,
     affine_dipy,
     affine_fsl,
     affine_niftyreg,
     array2nii,
     bias_field_correction,
     centre_mass_corr,
     centre_mass_img,
+    centre_mass_rel,
     conv_separable,
     coreg_spm,
     coreg_vinci,
     create_dir,
     create_mask,
     ct2mu,
     dcm2im,
     dcm2nii,
     dcmanonym,
+    dcmdir,
     dcminfo,
     dcmsort,
     dice_coeff,
     dice_coeff_multiclass,
     fwhm2sig,
     getmgh,
     getnii,
     getnii_descr,
     im_cut,
     imfill,
     imsmooth,
+    isdcm,
     isub,
     iyang,
     mgh2nii,
     motion_reg,
     nii_gzip,
     nii_modify,
     nii_ugzip,
@@ -100,8 +119,8 @@
     resample_niftyreg,
     resample_spm,
     resample_vinci,
     time_stamp,
 )
 
 # for use in `cmake -DCMAKE_PREFIX_PATH=...`
-cmake_prefix = resource_filename(__name__, "cmake")
+cmake_prefix = fspath(iresources.files("niftypet.nimpa").resolve() / "cmake")
```

### Comparing `nimpa-2.5.1/niftypet/nimpa/img/gen.py` & `nimpa-2.6.0/niftypet/nimpa/img/gen.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     amin = a.min()
     return np.where(-amin > amax, amin, amax)
 
 
 def create_disk(shape_in, r=1, a=0, b=0, gen_scale=1, threshold=None):
     if len(shape_in) == 2:
         shape = (1,) + shape_in
-    if len(shape_in) == 3:
+    elif len(shape_in) == 3:
         shape = shape_in
 
     imsk = np.zeros((gen_scale * shape[1], gen_scale * shape[2]), dtype=np.float32)
     for t in np.arange(0, math.pi, math.pi / (gen_scale*400)):
         x = gen_scale * r * np.cos(t) + gen_scale*a
         y = gen_scale * r * np.sin(t) + gen_scale*b
 
@@ -48,18 +48,51 @@
     if gen_scale > 1:
         imsk = ndi.interpolation.zoom(imsk, gen_scale**-1, order=1)
 
     if threshold:
         imsk = imsk > threshold
 
     if len(shape_in) == 3:
-        msk = np.repeat(imsk.reshape((1, shape[1], shape[1])), shape[0], axis=0)
+        return np.repeat(imsk.reshape((1, shape[1], shape[1])), shape[0], axis=0)
     elif len(shape_in) == 2:
-        msk = imsk
-    return msk
+        return imsk
+
+
+def get_cylinder(Cnt, rad=25, xo=0, yo=0, unival=1, gpu_dim=False, mask=True, two_d=False):
+    ''' Output image with a uniform cylinder of intensity = `unival`.
+        A better version of generating disk/cylinder in a given image space.
+        Arguments:
+        Cnt:    dictionary containing constants for the image space
+        rad:    radius
+        xo, yo: transaxial centre
+    '''
+
+    if mask: unival = 1
+
+    imdsk = np.zeros((1, Cnt['SZ_IMY'], Cnt['SZ_IMX']), dtype=np.float32)
+
+    for t in np.arange(0, math.pi, math.pi / (2*360)):
+        x = xo + rad * math.cos(t)
+        y = yo + rad * math.sin(t)
+        yf = np.arange(-y + 2*yo, y, Cnt['SZ_VOXY'] / 2)
+        v = np.int32(.5 * Cnt['SZ_IMX'] - np.ceil(yf / Cnt['SZ_VOXY']))
+        u = np.int32(.5 * Cnt['SZ_IMY'] + np.floor(x / Cnt['SZ_VOXY']))
+        imdsk[0, v, u] = unival
+
+    if two_d:
+        imdsk = np.squeeze(imdsk)
+    else:
+        imdsk = np.repeat(imdsk, Cnt['SZ_IMZ'], axis=0)
+
+    if mask: imdsk = imdsk.astype(dtype=bool)
+
+    if gpu_dim and not two_d:
+        return np.transpose(imdsk, (1, 2, 0))
+    else:
+        return imdsk
 
 
 def profile_points(im, p0, p1, steps=100):
     p = np.array([p1[0] - p0[0], p1[1] - p0[1]])
     nrm = np.sum(p**2)**.5
     p = p / nrm
```

### Comparing `nimpa-2.5.1/niftypet/nimpa/include/conv.h` & `nimpa-2.6.0/niftypet/nimpa/include/conv.h`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/niftypet/nimpa/include/rsmpl.h` & `nimpa-2.6.0/niftypet/nimpa/include/rsmpl.h`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/niftypet/nimpa/prc/CMakeLists.txt` & `nimpa-2.6.0/niftypet/nimpa/prc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/niftypet/nimpa/prc/__init__.py` & `nimpa-2.6.0/niftypet/nimpa/prc/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 # initialise the module folder
 __all__ = [
     # imio
     'array2nii', 'create_dir', 'dcm2im', 'dcm2nii', 'dcmanonym', 'dcminfo', 'dcmsort', 'fwhm2sig',
     'mgh2nii', 'getmgh', 'getnii', 'getnii_descr', 'nii_gzip', 'nii_ugzip', 'niisort', 'orientnii',
-    'pick_t1w', 'time_stamp', 'rem_chars',
+    'pick_t1w', 'time_stamp', 'rem_chars', 'isdcm', 'dcmdir',
     # prc
-    'bias_field_correction', 'centre_mass_img', 'centre_mass_corr', 'ct2mu', 'im_cut',
-    'imsmooth', 'imtrimup',
+    'bias_field_correction', 'centre_mass_img', 'centre_mass_rel', 'centre_mass_corr', 'ct2mu',
+    'im_cut', 'imsmooth', 'imtrimup',
     'iyang', 'nii_modify', 'pet2pet_rigid', 'psf_gaussian', 'psf_measured', 'pvc_iyang',
     # num
     'conv_separable', 'isub', 'nlm',
     # regseg
-    'affine_dipy', 'affine_fsl', 'affine_niftyreg',
+    'aff_dist', 'affine_dipy', 'affine_fsl', 'affine_niftyreg',
     'coreg_spm', 'coreg_vinci', 'create_mask', 'dice_coeff', 'dice_coeff_multiclass',
     'imfill', 'motion_reg', 'realign_mltp_spm', 'resample_fsl', 'resample_dipy',
     'resample_mltp_spm', 'resample_niftyreg', 'resample_spm',
     'resample_vinci'] # yapf: disable
 
 from .imio import (
     array2nii,
     create_dir,
     dcm2im,
     dcm2nii,
     dcmanonym,
+    dcmdir,
     dcminfo,
     dcmsort,
     fwhm2sig,
     getmgh,
     getnii,
     getnii_descr,
+    isdcm,
     mgh2nii,
     nii_gzip,
     nii_ugzip,
     niisort,
     orientnii,
     pick_t1w,
     rem_chars,
@@ -41,26 +43,28 @@
 from .num import conv_separable, isub, nlm
 
 # will be deprecated
 from .prc import (
     bias_field_correction,
     centre_mass_corr,
     centre_mass_img,
+    centre_mass_rel,
     ct2mu,
     im_cut,
     imsmooth,
     imtrimup,
     iyang,
     nii_modify,
     pet2pet_rigid,
     psf_gaussian,
     psf_measured,
     pvc_iyang,
 )
 from .regseg import (
+    aff_dist,
     affine_dipy,
     affine_fsl,
     affine_niftyreg,
     coreg_spm,
     coreg_vinci,
     create_mask,
     dice_coeff,
```

### Comparing `nimpa-2.5.1/niftypet/nimpa/prc/imio.py` & `nimpa-2.6.0/niftypet/nimpa/prc/imio.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,41 +9,37 @@
 from pathlib import Path
 from subprocess import run
 from textwrap import dedent
 
 import nibabel as nib
 import numpy as np
 import pydicom as dcm
-from miutil.imio.nii import array2nii  # NOQA: F401 # yapf: disable
+from miutil.fdio import create_dir, hasext
 from miutil.imio.nii import getnii  # NOQA: F401 # yapf: disable
 from miutil.imio.nii import nii_gzip  # NOQA: F401 # yapf: disable
 from miutil.imio.nii import nii_ugzip  # NOQA: F401 # yapf: disable
 from miutil.imio.nii import niisort  # NOQA: F401 # yapf: disable
+from miutil.imio.nii import array2nii
 
 # > NiftyPET resources
 from .. import resources as rs
 
 log = logging.getLogger(__name__)
 
 # > possible extensions for DICOM files
-dcmext = ('dcm', 'DCM', 'ima', 'IMA', 'img', 'IMG')
+dcmext = 'dcm', 'ima', 'img'
 
 # > remove characters unwanted in file/folder names
-avoid_chars = '{}[]!@#$%^&*.()+=:;~ '
+avoid_chars = '/{}[]!@#$%^&*.()+=:;~ '
 
 # > DICOM coding of PET isotopes
 istp_code = {
     'C-111A1': 'F18', 'C-105A1': 'C11', 'C-B1038': 'O15', 'C-128A2': 'Ge68', 'C-131A3': 'Ga68'}
 
 
-def create_dir(pth):
-    if not os.path.exists(pth):
-        os.makedirs(pth)
-
-
 def time_stamp(simple_ascii=False):
     now = datetime.datetime.now()
     if simple_ascii:
         nowstr = str(now.year) + '-' + str(now.month) + '-' + str(now.day) + '_' + str(
             now.hour) + 'h' + str(now.minute)
     else:
         nowstr = str(now.year) + '-' + str(now.month) + '-' + str(now.day) + ' ' + str(
@@ -57,23 +53,42 @@
 
 def rem_chars(txt, replacement_char='_'):
     ''' remove disallowed or inconvenient characters
         (as def. in `avoid_chars`) from file/folder names.
     '''
     for c in avoid_chars:
         txt = txt.replace(c, '_')
+    txt = txt.lstrip(replacement_char)
+    return txt or 'undefined'
+
+
+def isdcm(f):
+    try:
+        dcm.dcmread(f)
+    except Exception:
+        return False
+    else:
+        return True
 
-    while txt[0] == replacement_char:
-        txt = txt[1:]
 
-    return txt
+def dcmdir(inpth):
+    '''
+    Check if the folder has DICOM files and
+    specify them
+    '''
+    if not inpth.is_dir():
+        raise IOError('unrecognised folder')
+    dcmlst = [f for f in inpth.iterdir() if isdcm(f)]
+    Ndcm = len(dcmlst) # number of DICOM files
+    return {'fdcm': dcmlst, 'N': Ndcm} if Ndcm > 0 else None
 
 
 def mgh2nii(fim, fout=None, output=None):
-    ''' Convert `*.mgh` or `*.mgz` FreeSurfer image to NIfTI.
+    '''
+    Convert `*.mgh` or `*.mgz` FreeSurfer image to NIfTI.
         Arguments:
             fim: path to the input MGH file
             fout: path to the output NIfTI file, if None then
                   creates based on `fim`
             output: if not None and an applicable string it will
             output a dictionary or an array (see below)
         Return:
@@ -806,39 +821,39 @@
         raise ValueError('The input is not a dictionary!')
 
     dcmlst = []
     # list of mu-map DICOM files
     if 'mumapDCM' in datain:
         dcmump = os.listdir(datain['mumapDCM'])
         # accept only *.dcm extensions
-        dcmump = [os.path.join(datain['mumapDCM'], d) for d in dcmump if d.endswith(dcmext)]
+        dcmump = [os.path.join(datain['mumapDCM'], d) for d in dcmump if hasext(d, dcmext)]
         dcmlst += dcmump
 
     if 'T1DCM' in datain:
         dcmt1 = os.listdir(datain['T1DCM'])
         # accept only *.dcm extensions
-        dcmt1 = [os.path.join(datain['T1DCM'], d) for d in dcmt1 if d.endswith(dcmext)]
+        dcmt1 = [os.path.join(datain['T1DCM'], d) for d in dcmt1 if hasext(d, dcmext)]
         dcmlst += dcmt1
 
     if 'T2DCM' in datain:
         dcmt2 = os.listdir(datain['T2DCM'])
         # accept only *.dcm extensions
-        dcmt2 = [os.path.join(datain['T2DCM'], d) for d in dcmt2 if d.endswith(dcmext)]
+        dcmt2 = [os.path.join(datain['T2DCM'], d) for d in dcmt2 if hasext(d, dcmext)]
         dcmlst += dcmt2
 
     if 'UTE1' in datain:
         dcmute1 = os.listdir(datain['UTE1'])
         # accept only *.dcm extensions
-        dcmute1 = [os.path.join(datain['UTE1'], d) for d in dcmute1 if d.endswith(dcmext)]
+        dcmute1 = [os.path.join(datain['UTE1'], d) for d in dcmute1 if hasext(d, dcmext)]
         dcmlst += dcmute1
 
     if 'UTE2' in datain:
         dcmute2 = os.listdir(datain['UTE2'])
         # accept only *.dcm extensions
-        dcmute2 = [os.path.join(datain['UTE2'], d) for d in dcmute2 if d.endswith(dcmext)]
+        dcmute2 = [os.path.join(datain['UTE2'], d) for d in dcmute2 if hasext(d, dcmext)]
         dcmlst += dcmute2
 
     # list-mode data dcm
     if 'lm_dcm' in datain:
         dcmlst += [datain['lm_dcm']]
 
     if 'lm_ima' in datain:
@@ -877,20 +892,20 @@
 
     # > check if a folder containing DICOM files
     elif isinstance(dcmpth, str) and os.path.isdir(dcmpth):
         dircontent = os.listdir(dcmpth)
         # > create a list of DICOM files inside the folder
         dcmlst = [
             os.path.join(dcmpth, d) for d in dircontent
-            if os.path.isfile(os.path.join(dcmpth, d)) and d.endswith(dcmext)]
+            if os.path.isfile(os.path.join(dcmpth, d)) and hasext(d, dcmext)]
         log.debug('recognised the input argument as the folder containing DICOM files.')
 
     # > check if a folder containing DICOM files
     elif isinstance(dcmpth, list):
-        if not all(os.path.isfile(d) and d.endswith(dcmext) for d in dcmpth):
+        if not all(os.path.isfile(d) and hasext(d, dcmext) for d in dcmpth):
             raise IOError('Not all files in the list are DICOM files.')
         dcmlst = dcmpth
         log.debug('recognised the input argument as the list of DICOM file paths.')
 
     # > check if dictionary of data input <datain>
     elif isinstance(dcmpth, dict) and 'corepath' in dcmpth:
         dcmlst = list_dcm_datain(dcmpth)
@@ -1049,29 +1064,29 @@
 
 def dcm2im(fpth):
     '''
     Get the DICOM files from 'fpth' into an image with the affine transformation.
     fpth can be a list of DICOM files or a path (string) to the folder with DICOM files.
     '''
     # possible DICOM file extensions
-    ext = ('dcm', 'DCM', 'ima', 'IMA')
+    ext = 'dcm', 'ima'
 
     # case when given a folder path
     if isinstance(fpth, str) and os.path.isdir(fpth):
-        SZ0 = len([d for d in os.listdir(fpth) if d.endswith(ext)])
+        SZ0 = len([d for d in os.listdir(fpth) if hasext(d, ext)])
         # list of DICOM files
         fdcms = os.listdir(fpth)
-        fdcms = [os.path.join(fpth, f) for f in fdcms if f.endswith(ext)]
+        fdcms = [os.path.join(fpth, f) for f in fdcms if hasext(f, ext)]
 
     # case when list of DICOM files is given
     elif isinstance(fpth, list) and os.path.isfile(os.path.join(fpth[0])):
         SZ0 = len(fpth)
         # list of DICOM files
         fdcms = fpth
-        fdcms = [f for f in fdcms if f.endswith(ext)]
+        fdcms = [f for f in fdcms if hasext(f, ext)]
     else:
         raise NameError('Unrecognised input for DICOM files.')
 
     if SZ0 < 1:
         log.error('No DICOM images in the specified path.')
         raise IOError('Input DICOM images not recognised')
```

### Comparing `nimpa-2.5.1/niftypet/nimpa/prc/num.py` & `nimpa-2.6.0/niftypet/nimpa/prc/num.py`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/niftypet/nimpa/prc/prc.py` & `nimpa-2.6.0/niftypet/nimpa/prc/prc.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,50 +4,54 @@
 """
 import logging
 import multiprocessing
 import os
 import pathlib
 import re
 import sys
+from pathlib import Path, PurePath
 from subprocess import run
 from textwrap import dedent
 from warnings import warn
 
 import nibabel as nib
 import numpy as np
 import scipy.ndimage as ndi
-from pkg_resources import resource_filename
+from miutil.fdio import hasext
 from tqdm.auto import trange
 
 from . import imio, regseg
 from .num import conv_separable
 
+try:          # py<3.9
+    import importlib_resources as resources
+except ImportError:
+    from importlib import resources
+
 try:
     import SimpleITK as sitk
     sitk_flag = True
 except ImportError:
     sitk_flag = False
 
 log = logging.getLogger(__name__)
 
-# possible extentions for DICOM files
-dcmext = ('dcm', 'DCM', 'ima', 'IMA', 'img', 'IMG')
-niiext = ('nii.gz', 'nii', 'img', 'hdr')
+# filename extentions
+dcmext = 'dcm', 'ima', 'img'
+niiext = 'nii.gz', 'nii', 'img', 'hdr'
 
 
-# ----------------------------------------------------------------------
 def num(s):
     '''Converts the string to a float or integer number.'''
     try:
         return int(s)
     except ValueError:
         return float(s)
 
 
-# ----------------------------------------------------------------------
 def psf_gaussian(vx_size=(1, 1, 1), fwhm=(6, 5, 5), hradius=8):
     '''
     Separable kernels for Gaussian convolution executed on the GPU device
     The output kernels are in this order: z, y, x
     '''
 
     # if voxel size is given as scalar, interpret it as an isotropic
@@ -86,15 +90,16 @@
     return krnl
 
 
 # ----------------------------------------------------------------------
 def psf_measured(scanner='mmr', scale=1):
     if scanner == 'mmr':
         # file name for the mMR's PSF and chosen scale
-        fdat = resource_filename("niftypet.nimpa", f"auxdata/PSF-17_scl-{scale:d}.npy")
+        fdat = os.fspath(
+            resources.files("niftypet.nimpa").resolve() / "auxdata" / f"PSF-17_scl-{scale:d}.npy")
         # transaxial and axial PSF
         Hxy, Hz = np.load(fdat)
         return np.array([Hz, Hxy, Hxy], dtype=np.float32)
     raise NameError(f'Unsupported scanner ({scanner}):'
                     ' only Siemens mMR (mmr) is currently supported')
 
 
@@ -123,15 +128,16 @@
     '''
     if gpu is not None:
         warn("gpu is automatic", DeprecationWarning, stacklevel=2)
     if Cnt is not None and 'DEVID' in Cnt:
         dev_id = Cnt['DEVID']
 
     isfile = False
-    if isinstance(fim, str) and os.path.isfile(fim):
+    if isinstance(fim, (str, Path, PurePath)) and os.path.isfile(fim):
+        fim = Path(fim)
         isfile = True
         imd = imio.getnii(fim, output='all')
         im = imd['im']
         voxsize = imd['voxsize']
         affine = imd['affine']
     elif isinstance(fim, dict) and 'voxsize' in fim:
         im = fim['im']
@@ -144,24 +150,31 @@
             "incorrect image input.\nNIfTI file path, dictionary or Numpy array are accepted.")
 
     if psf is None:
         if voxsize is None and Cnt is not None and 'SO_VXZ' in Cnt:
             voxsize = [Cnt['SO_VXZ'], Cnt['SO_VXY'], Cnt['SO_VXX']]
         elif voxsize is None and Cnt is None:
             raise ValueError('the correct voxel size has to be provided')
-        psf = psf_gaussian(vx_size=voxsize, fwhm=fwhm)
+
+        # > check if the GPU kernel size (17, radius=8) will be sufficient to fit the PSF
+        if np.any(2 * (fwhm / np.min(voxsize)) > (17 - 1)):
+            hradius = (2 * (fwhm / np.min(voxsize)) + 1) // 2
+            psf = psf_gaussian(vx_size=voxsize, fwhm=fwhm, hradius=hradius)
+        else:
+            psf = psf_gaussian(vx_size=voxsize, fwhm=fwhm)
+
     imsmo = conv_separable(im, psf, output=output_array, dev_id=dev_id, sync=sync)
 
     # output dictionary
     dctout = {}
     dctout['im'] = imsmo
     dctout['fwhm'] = fwhm
 
     if isfile and fout == '':
-        if fim.endswith('.nii.gz'):
+        if hasext(fim, 'nii.gz'):
             fout = fim.split('.nii.gz')[0] + '_smo' + str(fwhm).replace('.', '-') + '.nii.gz'
         else:
             fout = os.path.splitext(fim)[0] + '_smo' + str(fwhm).replace(
                 '.', '-') + os.path.splitext(fim)[1]
 
     if isfile:
         dctout['affine'] = affine
@@ -204,16 +217,16 @@
 # <><><><><><><><><><><><><><><><><><><><><><><><><><><><>
 # FUNCTIONS: TRIM &  PARTIAL VOLUME EFFECTS AND CORRECTION
 # <><><><><><><><><><><><><><><><><><><><><><><><><><><><>
 
 
 def imtrimup(fims, refim='', affine=None, scale=2, divdim=8**2, fmax=0.05, int_order=0,
              outpath=None, fname='', fcomment='', fcomment_pfx='', store_avg=False,
-             store_img_intrmd=False, store_img=False, imdtype=np.float32, memlim=False,
-             verbose=False, Cnt=None):
+             store_img_intrmd=False, store_img=False, imdtype=np.float32, grid_mode=True,
+             memlim=False, verbose=False, Cnt=None):
     '''
     Trim and upsample PET image(s), e.g., for GPU execution,
     PVC correction, ROI sampling, etc.
     The input images 'fims' can be passed in multiple ways:
     1. as a string of the folder containing NIfTI files
     2. as a string of a NIfTI file path (this way a 4D image can be loaded).
     3. as a list of NIfTI file paths.
@@ -232,38 +245,40 @@
     outpath: output folder path
     fname: file name when image given as a numpy matrix
     fcomment: part of the name of the output file, left for the user as a comment
     fcomment_pfx: part of the name of the output file at the start (prefix)
     store_img_intrmd: stores intermediate images with suffix '_i'
     store_avg: stores the average image (if multiple images are given)
     imdtype: data type for output images
+    grid_mode: mode for scipy zooming.  Default is True, where the distance including
+               the full pixel extent is used.
     memlim: Ture for cases when memory is limited and takes more processing time instead.
     verbose: verbose mode [True/False]
     '''
     if Cnt is None:
         Cnt = {}
 
     # case when input folder is given
     if isinstance(fims, (str, pathlib.PurePath)) and os.path.isdir(fims):
         # list of input images (e.g., PET)
-        fimlist = [os.path.join(fims, f) for f in os.listdir(fims) if f.endswith(niiext)]
+        fimlist = [os.path.join(fims, f) for f in os.listdir(fims) if hasext(f, niiext)]
         imdic = imio.niisort(fimlist, memlim=memlim)
         if not (imdic['N'] > 50 and memlim):
             imin = imdic['im']
         imshape = imdic['shape']
         affine = imdic['affine']
         fldrin = fims
         fnms = [os.path.basename(f).split('.nii')[0] for f in imdic['files'] if f is not None]
         # number of images/frames
         Nim = imdic['N']
         using_multiple_files = True
 
     # case when input file is a 3D or 4D NIfTI image
-    elif isinstance(
-            fims, (str, pathlib.PurePath)) and os.path.isfile(fims) and str(fims).endswith(niiext):
+    elif isinstance(fims,
+                    (str, pathlib.PurePath)) and os.path.isfile(fims) and hasext(fims, niiext):
         imdic = imio.getnii(fims, output='all')
         imin = imdic['im']
         if imin.ndim == 3:
             imin.shape = (1, imin.shape[0], imin.shape[1], imin.shape[2])
         imdtype = imdic['dtype']
         imshape = imdic['shape'][-3:]
         affine = imdic['affine']
@@ -357,35 +372,38 @@
     # ------------------------------------------------------
 
     # ------------------------------------------------------
     # scaled input image and get a sum image as the base for trimming
     if any(scale > 1):
         newshape = (scale[0] * imshape[0], scale[1] * imshape[1], scale[2] * imshape[2])
         imsum = np.zeros(newshape, dtype=imdtype)
+        mode = 'constant'
+        if grid_mode:
+            mode = 'grid-' + mode
         if not memlim:
             imscl = np.zeros((Nim,) + newshape, dtype=imdtype)
-            with trange(Nim, desc="loading-scaling",
-                        disable=log.getEffectiveLevel() > logging.INFO,
-                        leave=log.getEffectiveLevel() <= logging.INFO) as pbar:
+            with trange(Nim, desc="loading-scaling", disable=log.getEffectiveLevel()
+                        > logging.INFO, leave=log.getEffectiveLevel() <= logging.INFO) as pbar:
                 for i in pbar:
                     imscl[i, :, :, :] = ndi.interpolation.zoom(imin[i, :, :, :], tuple(scale),
-                                                               order=int_order)
+                                                               order=int_order, mode=mode,
+                                                               grid_mode=grid_mode)
                     imsum += imscl[i, :, :, :]
         else:
-            with trange(Nim, desc="loading-scaling",
-                        disable=log.getEffectiveLevel() > logging.INFO,
-                        leave=log.getEffectiveLevel() <= logging.INFO) as pbar:
+            with trange(Nim, desc="loading-scaling", disable=log.getEffectiveLevel()
+                        > logging.INFO, leave=log.getEffectiveLevel() <= logging.INFO) as pbar:
                 for i in pbar:
                     if Nim > 50 and using_multiple_files:
                         imin_temp = imio.getnii(imdic['files'][i])
-                        imsum += ndi.interpolation.zoom(imin_temp, tuple(scale), order=int_order)
+                        imsum += ndi.interpolation.zoom(imin_temp, tuple(scale), order=int_order,
+                                                        mode=mode, grid_mode=grid_mode)
                         log.debug(' image sum: read {}'.format(imdic['files'][i]))
                     else:
-                        imsum += ndi.interpolation.zoom(imin[i, :, :, :], tuple(scale),
-                                                        order=int_order)
+                        imsum += ndi.interpolation.zoom(imin[i, :, :, :], tuple(scale), mode=mode,
+                                                        order=int_order, grid_mode=grid_mode)
     else:
         imscl = imin
         imsum = np.sum(imin, axis=0)
 
     # import pdb; pdb.set_trace()
     # ------------------------------------------------------
 
@@ -475,17 +493,18 @@
     imsumt[iz0t:, iy0t:iy1t, ix0t:ix1t] = imsum[iz0s:, iy0s:iy1 + 1, ix0s:ix1 + 1]
 
     # > new affine matrix for the upscaled and trimmed image
     # > use the scale factor reversely for consistency
     A = np.diag(np.append(sf[::-1], 1.) * np.diag(affine))
 
     # > note half of new voxel offset is used for the new centre of voxels
-    A[0, 3] = affine[0, 3] + A[0, 0] * (ix0-0.5)
-    A[1, 3] = affine[1, 3] + (affine[1, 1] * (imshape[1] - 1) - A[1, 1] * (iy1-0.5))
-    A[2, 3] = affine[2, 3] - A[1, 1] * 0.5
+    A[0, 3] = affine[0, 3] + A[0, 0] * (ix0 - 0.5 * (scale[2] - 1))
+    A[1, 3] = affine[1, 3] + (affine[1, 1] * (imshape[1] - 1) - A[1, 1] * (iy1 - 0.5 *
+                                                                           (scale[1] - 1)))
+    A[2, 3] = affine[2, 3] - A[2, 2] * 0.5 * (scale[0] - 1)
     A[3, 3] = 1
 
     # output dictionary
     dctout = {'affine': A, 'trimpar': trimpar, 'imsum': imsumt}
 
     # NIfTI image description (to be stored in the header)
     niidescr = 'trim(x,y,z):' + str(trimpar['x']) + ',' + str(trimpar['y']) + ',' + str(
@@ -502,17 +521,16 @@
         imio.array2nii(imsumt[::-1, ::-1, :], A, fsum, descrip=niidescr)
         log.debug('saved averaged image to: {}'.format(fsum))
         dctout['fsum'] = fsum
 
     # list of file names for the upsampled and trimmed images
     fpetu = []
     # > perform the trimming and save the intermediate images if requested
-    with trange(Nim, desc="finalising trimming/scaling",
-                disable=log.getEffectiveLevel() > logging.INFO,
-                leave=log.getEffectiveLevel() <= logging.INFO) as pbar:
+    with trange(Nim, desc="finalising trimming/scaling", disable=log.getEffectiveLevel()
+                > logging.INFO, leave=log.getEffectiveLevel() <= logging.INFO) as pbar:
 
         for i in pbar:
 
             # memory saving option, second time doing interpolation
             if memlim:
                 if Nim > 50 and using_multiple_files:
                     imin_temp = imio.getnii(imdic['files'][i])
@@ -898,14 +916,58 @@
     else:
         raise ValueError('unrecognised output option')
 
 
 # ==============================================================================
 
 
+def centre_mass_rel(im, com=None):
+    '''
+    get the relative centre of mass and the corrected affine matrix
+    '''
+
+    if isinstance(im, (str, PurePath)):
+        imdct = imio.getnii(im, output='all')
+    elif isinstance(im, dict) and 'shape' in im:
+        imdct = im
+    else:
+        raise ValueError('unrecognised input image')
+
+    if com is None:
+        com = centre_mass_img(imdct)
+
+    # > initialise the list of relative NIfTI image CoMs
+    com_nii = []
+
+    # > modified affine for the centre of mass
+    mA = imdct['affine'].copy()
+
+    # > go through x, y and z
+    for i in range(3):
+        vox_size = max(imdct['affine'][i, :-1], key=abs)
+
+        # > get the relative centre of mass for each axis (relative to the translation
+        # > values in the affine matrix)
+        if vox_size > 0:
+            com_rel = com[2 - i] + imdct['affine'][i, -1]
+        else:
+            com_rel = com[2 - i] - abs(vox_size) * imdct['shape'][-i - 1] + imdct['affine'][i, -1]
+
+        mA[i, -1] -= com_rel
+
+        com_nii.append(com_rel)
+
+    log.info('''
+        \r relative CoM values are:
+        \r {}
+        '''.format(com_nii))
+
+    return mA, com_nii
+
+
 # ==============================================================================
 def centre_mass_corr(img, Cnt=None, com=None, flip=None, outpath=None, fcomment='_com-modified',
                      fout=None):
     """
     Image centre of mass correction. The O point is in the middle of the
     image centre of voxel value mass (e.g, radio-activity).
     Arguments:
@@ -943,39 +1005,15 @@
         com = centre_mass_img(imdct, output='mm')
 
     com = np.array(com)
 
     if not isinstance(com, np.ndarray):
         raise ValueError('The Centre of Mass is not a Numpy array!')
 
-    # > initialise the list of relative NIfTI image CoMs
-    com_nii = []
-
-    # > modified affine for the centre of mass
-    mA = imdct['affine'].copy()
-
-    # > go through x, y and z
-    for i in range(3):
-        vox_size = max(imdct['affine'][i, :-1], key=abs)
-
-        # > get the relative centre of mass for each axis (relative to the translation
-        # > values in the affine matrix)
-        if vox_size > 0:
-            com_rel = com[2 - i] + imdct['affine'][i, -1]
-        else:
-            com_rel = com[2 - i] - abs(vox_size) * imdct['shape'][-i - 1] + imdct['affine'][i, -1]
-
-        mA[i, -1] -= com_rel
-
-        com_nii.append(com_rel)
-
-    log.info('''
-        \r relative CoM values are:
-        \r {}
-        '''.format(com_nii))
+    mA, com_nii = centre_mass_rel(imdct, com)
 
     # >------------------------------------------------------
     # > get the file name and path separated
     fsplt = os.path.split(imdct['fim'])
 
     # > get the output path
     if outpath is not None:
@@ -988,39 +1026,41 @@
 
     # > get the output file name
     if fout is not None:
         fimc = fout
 
         if isinstance(fimc, pathlib.Path) and (fimc.suffix != '.gz' or fimc.suffix != '.nii'):
             fimc.with_suffix('.nii.gz')
-
-        elif isinstance(fimc, str) and not fimc.endswith(('.nii', 'nii.gz')):
+        elif isinstance(fimc, str) and not hasext(fimc, ('nii', 'nii.gz')):
             fimc = fimc + '.nii.gz'
 
         fimc = pathlib.Path(fimc)
 
-        if not fimc.parent == '.':
+        if fimc.parent != '.':
             opth = fimc.parent
             fnm = fimc.name
         else:
             fnm = fimc
     else:
         fnm = fsplt[1].split('.nii')[0] + fcomment + '.nii.gz'
 
-    # save to NIfTI
+    # > save to NIfTI, first load
     innii = nib.load(imdct['fim'])
-    # get a new NIfTI image for the perturbed MR
+
+    # > get the data and flip if needed
     imdata = innii.get_fdata()
     if flip is not None:
         imdata = imdata[::flip[2], ::flip[1], ::flip[0], ...]
-    newnii = nib.Nifti1Image(imdata, mA, innii.header)
 
+    # > generate a new NIfTI image
     fnew = os.path.join(opth, fnm)
-    # save into a new file name for the T1w
+    innii.header['descrip'] = 'NiftyPET: CoM-modified'
+    newnii = nib.Nifti1Image(imdata, mA, innii.header)
     nib.save(newnii, fnew)
+
     return {'fim': fnew, 'com_rel': com_nii, 'com_abs': com}
 
 
 # ==============================================================================
 
 
 def nii_modify(nii, fimout='', outpath='', fcomment='', voxel_range=None):
@@ -1183,15 +1223,15 @@
     elif isinstance(fmr, list) and all(map(os.path.isfile, fmr)):
         fins = fmr
         log.info('multiple input files => ignoring the single output file name.')
         fimout = ''
 
     # > path to a folder
     elif isinstance(fmr, (str, pathlib.PurePath)) and os.path.isdir(fmr):
-        fins = [os.path.join(fmr, f) for f in os.listdir(fmr) if f.endswith(('.nii', '.nii.gz'))]
+        fins = [os.path.join(fmr, f) for f in os.listdir(fmr) if hasext(f, ('nii', 'nii.gz'))]
         log.info('multiple input files from input folder.')
         fimout = ''
 
     else:
         raise ValueError('could not decode the input of floating images.')
     # --------------------------------------------------------------------------
```

### Comparing `nimpa-2.5.1/niftypet/nimpa/prc/regseg.py` & `nimpa-2.6.0/niftypet/nimpa/prc/regseg.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import glob
 import logging
 import os
 import shutil
 import sys
 from os import fspath
+from pathlib import PurePath
 from subprocess import call
 from textwrap import dedent
 
 import nibabel as nib
 import numpy as np
 import scipy.ndimage as ndi
 from dipy.align import _public as align
@@ -33,19 +34,24 @@
             ix0 = np.argmax(immsk[iz, iy, :] > 0)
             ix1 = immsk.shape[2] - np.argmax(immsk[iz, iy, ::-1] > 0)
             if (ix1 - ix0) > immsk.shape[2] - 10: continue
             immsk[iz, iy, ix0:ix1] = 1
     return immsk
 
 
+# SPM options
+# 'mi'  - Mutual Information (default)
+# 'nmi' - Normalised Mutual Information
+# 'ecc' - Entropy Correlation Coefficient
+# 'ncc' - Normalised Cross Correlation
+
+
 # ------------------------------------------------------------------------------
 # Create object mask for the input image
 # ------------------------------------------------------------------------------
-
-
 def create_mask(
     fnii,
     fimout='',
     outpath='',
     fill=1,
     dtype_fill=np.uint8,
     thrsh=0.,
@@ -100,28 +106,56 @@
 
 
 # <><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><>
 # I M A G E   R E G I S T R A T I O N
 # <><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><>
 
 
+# ------------------------------------------------------------------------------
+def aff_dist(A, pnt, offset=40):
+    ''' find average point distance after applying
+        the affine transformation `A` to a point `pnt`
+        and its `offset` in all directions.
+    '''
+
+    # > get the sampling point(s) for evaluation of motion
+    p = np.array(pnt + [1])
+    pp = np.matmul(A, p)
+
+    # > measure of distance after applying the transformation
+    dist = np.sum((pp - p)**2)**.5
+
+    # > get it in a list for all the offsets
+    dist = [dist]
+    for x in [p[0] - offset, p[0] + offset]:
+        for y in [p[1] - offset, p[1] + offset]:
+            for z in [p[2] - offset, p[2] + offset]:
+
+                p = np.array([x, y, z, 1])
+                pp = np.matmul(A, p)
+                dist.append(np.sum((pp - p)**2)**.5)
+
+    return max(dist)
+
+
+# ------------------------------------------------------------------------------
 def affine_dipy(
     fref,
     fflo,
     nbins=32,
     metric='MI',
     level_iters=None,
     sigmas=None,
     factors=None,
     outpath=None,
     faffine=None,
     pickname='ref',
     fcomment='',
-    rfwhm=15.,
-    ffwhm=15.,
+    rfwhm=8.,
+    ffwhm=8.,
     verbose=True,
 ):
     """
     Perform affine 3-stage image registration using DIPY.
 
     Arguments:
       fref: file path to the reference image to which the floating image
@@ -214,31 +248,31 @@
         opth = os.path.dirname(fflo)
     else:
         opth = outpath
 
     imio.create_dir(opth)
 
     # > the output naming
-    if os.path.dirname(fimout) != '':
+    if fimout is not None and os.path.dirname(fimout) != '':
         fout = fimout
-    elif fimout is not None and not os.path.isfile(fimout):
-        fout = os.path.join(opth, fimout)
+    # elif fimout is not None and not os.path.isfile(fimout):
+    #     fout = os.path.join(opth, fimout)
     elif pickname == 'ref':
         fout = os.path.join(
             opth, 'resampled-dipy_to_ref-' + os.path.basename(fref).split('.nii')[0] + fcomment +
             '.nii.gz')
     elif pickname == 'flo':
         fout = os.path.join(
             opth, 'resampled-dipy_to_flo-' + os.path.basename(fflo).split('.nii')[0] + fcomment +
             '.nii.gz')
     # ------------------------------------------------------------------
 
     # ------------------------------------------------------------------
     if faff is not None:
-        if faff.endswith('.npy'):
+        if isinstance(faff, (str, PurePath)) and hasext(faff, 'npy'):
             affine = np.load(faff)
         elif isinstance(faff, np.ndarray):
             affine = faff
         else:
             raise ValueError('e> unrecognised affine matrix input')
     else:
         affine = None
@@ -253,15 +287,15 @@
         raise ValueError('e> unrecognised interpolation input')
     # ------------------------------------------------------------------
 
     # ------------------------------------------------------------------
     # > DIPY RESAMPLING
     # ------------------------------------------------------------------
     static, static_affine, moving, moving_affine, between_affine = align._handle_pipeline_inputs(
-        fflo, fref, moving_affine=None, static_affine=None, starting_affine=affine)
+        str(fflo), str(fref), moving_affine=None, static_affine=None, starting_affine=affine)
     affine_map = align.AffineMap(between_affine, static.shape, static_affine, moving.shape,
                                  moving_affine)
     rsmpl = affine_map.transform(moving, interpolation=interpolation)
 
     del moving, static
 
     # > save to NIfTI
@@ -277,15 +311,15 @@
     fname_aff='',
     pickname='ref',
     fcomment='',
     executable=None,
     omp=1,
     rigOnly=False,
     affDirect=False,
-    maxit=5,
+    maxit=10,
     speed=True,
     pi=50,
     pv=50,
     smof=0,
     smor=0,
     rmsk=True,
     fmsk=True,
@@ -343,15 +377,16 @@
 
     # call the registration routine
     cmd = [
         executable, '-ref', fref, '-flo', fflo, '-aff', faff, '-pi',
         str(pi), '-pv',
         str(pv), '-smooF',
         str(smof), '-smooR',
-        str(smor), '-maxit', '10', '-omp',
+        str(smor), '-maxit',
+        str(maxit), '-omp',
         str(omp), '-res', fout]
     if speed:
         cmd.append('-speeeeed')
     if rigOnly:
         cmd.append('-rigOnly')
     if affDirect:
         cmd.append('affDirect')
@@ -469,15 +504,15 @@
     imio.create_dir(tmpth)
 
     # > uncompress for SPM
     fungz = []
     for f in fims:
         if f[-3:] == '.gz':
             fun = imio.nii_ugzip(f, outpath=tmpth)
-        elif os.path.isfile(f) and f.endswith('nii'):
+        elif os.path.isfile(f) and hasext(f, 'nii'):
             if niicopy:
                 fun = os.path.join(tmpth, os.path.basename(f).split('.nii')[0] + '_copy.nii')
                 shutil.copyfile(f, fun)
             else:
                 fun = f
         else:
             log.warning('omitting file/folder: {}'.format(f))
@@ -487,15 +522,15 @@
         niisrt = imio.niisort([
             os.path.join(tmpth, f) for f in os.listdir(tmpth)
             if os.path.isfile(os.path.join(tmpth, f))])
         fsrt = niisrt['files']
     else:
         fsrt = fungz
 
-    P_input = [f + ',1' for f in fsrt if f.endswith('nii') and f[0] != 'r' and 'mean' not in f]
+    P_input = [f + ',1' for f in fsrt if hasext(f, 'nii') and f[0] != 'r' and 'mean' not in f]
 
     # > maximal number of characters per line (for Matlab array)
     Pinmx = max(map(len, P_input))
 
     # > equalise the input char array
     Pineq = [f.ljust(Pinmx) for f in P_input]
 
@@ -588,21 +623,21 @@
     imio.create_dir(opth)
 
     # > working file names (not touching the original ones)
     _fims = []
 
     # > decompress if necessary
     for f in fims:
-        if not os.path.isfile(f) and not (f.endswith('nii') or f.endswith('nii.gz')):
-            raise IOError('e> could not open file:', f)
+        if not os.path.isfile(f) and not hasext(f, ('nii', 'nii.gz')):
+            raise IOError('could not open file:', f)
 
-        if f[-3:] == '.gz':
+        if hasext(f, 'gz'):
             fugz = imio.nii_ugzip(f, outpath=os.path.join(opth, 'copy'))
         elif copy_input:
-            fnm = os.path.basename(f).split('.nii')[0] + '_copy.nii'
+            fnm = os.path.basename(f).rsplit('.nii', 1)[0] + '_copy.nii'
             fugz = os.path.join(opth, 'copy', fnm)
             shutil.copyfile(f, fugz)
         else:
             fugz = f
 
         _fims.append(fugz)
 
@@ -735,15 +770,15 @@
             fout = os.path.join(
                 opth, 'affine-vinci',
                 'affine-flo-' + os.path.basename(fflo).split('.nii')[0] + fcomment + '.nii.gz')
 
     else:
 
         # > add '.xml' extension if not in the affine output file name
-        if not fname_aff.endswith('.xml'):
+        if not hasext(fname_aff, 'xml'):
             fname_aff += '.xml'
 
         faff = os.path.join(opth, 'affine-vinci', fname_aff)
 
         fout = os.path.join(opth, fname_aff.split('.')[0] + '.nii.gz')
     # --------------------------------------------------------------------------
 
@@ -976,40 +1011,35 @@
     # --------------------------------------------------------------------------
     # > output path
     if outpath == '' and fname_aff != '' and os.path.isfile(fname_aff):
         opth = os.path.dirname(fname_aff)
         if opth == '':
             opth = os.path.dirname(fflo)
         fname_aff = os.path.basename(fname_aff)
-
     elif outpath == '':
         opth = os.path.dirname(fflo)
     else:
         opth = outpath
     imio.create_dir(opth)
 
     imio.create_dir(os.path.join(opth, 'affine-fsl'))
 
     # > output floating and affine file names
     if fname_aff == '':
-
         if pickname == 'ref':
             faff = os.path.join(
                 opth, 'affine-fsl',
                 'affine-ref-' + os.path.basename(fref).split('.nii')[0] + fcomment + '.txt')
-
         else:
             faff = os.path.join(
                 opth, 'affine-fsl',
                 'affine-flo-' + os.path.basename(fflo).split('.nii')[0] + fcomment + '.txt')
-
     else:
-
-        # > add '.xml' extension if not in the affine output file name
-        if not fname_aff.endswith('.txt'):
+        # > add '.txt' extension if not in the affine output file name
+        if not hasext(fname_aff, 'txt'):
             fname_aff += '.txt'
 
         faff = os.path.join(opth, 'affine-vinci', fname_aff)
     # --------------------------------------------------------------------------
 
     # > command with options for FSL-FLIRT registration
     cmd = [
```

### Comparing `nimpa-2.5.1/niftypet/nimpa/prc/src/conv.cu` & `nimpa-2.6.0/niftypet/nimpa/prc/src/conv.cu`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/niftypet/nimpa/prc/src/cuhelpers.cu` & `nimpa-2.6.0/niftypet/nimpa/prc/src/cuhelpers.cu`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/niftypet/nimpa/prc/src/img_module.cu` & `nimpa-2.6.0/niftypet/nimpa/prc/src/img_module.cu`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/niftypet/nimpa/prc/src/isub.cu` & `nimpa-2.6.0/niftypet/nimpa/prc/src/isub.cu`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/niftypet/nimpa/prc/src/nlm.cu` & `nimpa-2.6.0/niftypet/nimpa/prc/src/nlm.cu`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/niftypet/nimpa/prc/src/rsmpl.cu` & `nimpa-2.6.0/niftypet/nimpa/prc/src/rsmpl.cu`

 * *Files identical despite different names*

### Comparing `nimpa-2.5.1/nimpa.egg-info/PKG-INFO` & `nimpa-2.6.0/nimpa.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,124 +1,122 @@
 Metadata-Version: 2.1
 Name: nimpa
-Version: 2.5.1
+Version: 2.6.0
 Summary: CUDA-accelerated Python utilities for high-throughput neuroimage processing and analysis
-Home-page: https://github.com/NiftyPET/NIMPA
-Author: Pawel Markiewicz
-Author-email: p.markiewicz@ucl.ac.uk
-Maintainer: Casper da Costa-Luis
-Maintainer-email: casper.dcl@physics.org
-License: Apache 2.0
-Project-URL: Changelog, https://github.com/NiftyPET/NIMPA/releases
-Project-URL: Documentation, https://niftypet.readthedocs.io
-Description: =======================================================
-        NIMPA: Neuro and NiftyPET Image Processing and Analysis
-        =======================================================
-        
-        |Docs| |Version| |Downloads| |Py-Versions| |DOI| |Licence| |Tests|
-        
-        NIMPA is a stand-alone Python sub-package of NiftyPET_, dedicated to high-throughput processing and analysis of brain images, particularly those, which are acquired using positron emission tomography (PET) and magnetic resonance (MR).  Although, it is an essential part of the NiftyPET_ package for seamless PET image reconstruction, NIMPA is equally well suited for independent image processing, including image trimming, upsampling and partial volume correction (PVC).
-        
-        .. _NiftyPET: https://github.com/NiftyPET/NiftyPET
-        
-        Trimming is performed in order to reduce the unused image voxels in brain imaging, when using whole body PET scanners, for which only some part of the field of view (FOV) is used.
-        
-        The upsampling is needed for more accurate extraction (sampling) of PET data using regions of interest (ROI), obtained using parcellation of the corresponding T1w MR image, usually of higher image resolution.
-        
-        PVC is needed to correct for the spill-in and spill-out of PET signal from defined ROIs (specific for any given application).
-        
-        **Documentation with installation manual and tutorials**: https://niftypet.readthedocs.io/
-        
-        Quick Install
-        ~~~~~~~~~~~~~
-        
-        Note that it's recommended (but not required) to use `conda`.
-        
-        .. code:: sh
-        
-            # cross-platform install
-            conda install -c conda-forge python=3 \
-              ipykernel numpy scipy scikit-image matplotlib ipywidgets dcm2niix
-            pip install "nimpa>=2"
-        
-        For optional `dcm2niix <https://github.com/rordenlab/dcm2niix>`_ (image conversion from DICOM to NIfTI) and/or `niftyreg <https://github.com/KCL-BMEIS/niftyreg>`_ (image registration) support, simply install them separately (``pip install dcm2niix niftyreg``).
-        
-        External CMake Projects
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        The raw C/CUDA libraries may be included in external projects using ``cmake``.
-        Simply build the project and use ``find_package(NiftyPETnimpa)``.
-        
-        .. code:: sh
-        
-            # print installation directory (after `pip install nimpa`)...
-            python -c "from niftypet.nimpa import cmake_prefix; print(cmake_prefix)"
-        
-            # ... or build & install directly with cmake
-            mkdir build && cd build
-            cmake ../niftypet && cmake --build . && cmake --install . --prefix /my/install/dir
-        
-        At this point any external project may include NIMPA as follows
-        (Once setting ``-DCMAKE_PREFIX_DIR=<installation prefix from above>``):
-        
-        .. code:: cmake
-        
-            cmake_minimum_required(VERSION 3.3 FATAL_ERROR)
-            project(myproj)
-            find_package(NiftyPETnimpa COMPONENTS improc REQUIRED)
-            add_executable(myexe ...)
-            target_link_libraries(myexe PRIVATE NiftyPET::improc)
-        
-        Licence
-        ~~~~~~~
-        
-        |Licence| |DOI|
-        
-        Copyright 2018-21
-        
-        - `Pawel J. Markiewicz <https://github.com/pjmark>`__ @ University College London
-        - `Casper O. da Costa-Luis <https://github.com/casperdcl>`__ @ University College London/King's College London
-        - `Contributors <https://github.com/NiftyPET/NIMPA/graphs/contributors>`__
-        
-        .. |Docs| image:: https://readthedocs.org/projects/niftypet/badge/?version=latest
-           :target: https://niftypet.readthedocs.io/en/latest/?badge=latest
-        .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4417633.svg
-           :target: https://doi.org/10.5281/zenodo.4417633
-        .. |Licence| image:: https://img.shields.io/pypi/l/nimpa.svg?label=licence
-           :target: https://github.com/NiftyPET/NIMPA/blob/master/LICENCE
-        .. |Tests| image:: https://img.shields.io/github/workflow/status/NiftyPET/NIMPA/Test?logo=GitHub
-           :target: https://github.com/NiftyPET/NIMPA/actions
-        .. |Downloads| image:: https://img.shields.io/pypi/dm/nimpa.svg?logo=pypi&logoColor=white&label=PyPI%20downloads
-           :target: https://pypi.org/project/nimpa
-        .. |Version| image:: https://img.shields.io/pypi/v/nimpa.svg?logo=python&logoColor=white
-           :target: https://github.com/NiftyPET/NIMPA/releases
-        .. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/nimpa.svg?logo=python&logoColor=white
-           :target: https://pypi.org/project/nimpa
-        
+Author-email: Pawel Markiewicz <p.markiewicz@ucl.ac.uk>
+Maintainer-email: Casper da Costa-Luis <casper.dcl@physics.org>
+License: Apache-2.0
+Project-URL: documentation, https://niftypet.readthedocs.io
+Project-URL: repository, https://github.com/NiftyPET/NIMPA
+Project-URL: changelog, https://github.com/NiftyPET/NIMPA/releases
 Keywords: PET,MR,processing,analysis
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: dev
+Provides-Extra: plot
 Provides-Extra: cuda
 Provides-Extra: dcm2niix
-Provides-Extra: dev
 Provides-Extra: niftyreg
-Provides-Extra: plot
+License-File: LICENCE
+
+=======================================================
+NIMPA: Neuro and NiftyPET Image Processing and Analysis
+=======================================================
+
+|Docs| |Version| |Downloads| |Py-Versions| |DOI| |Licence| |Tests|
+
+NIMPA is a stand-alone Python sub-package of NiftyPET_, dedicated to high-throughput processing and analysis of brain images, particularly those, which are acquired using positron emission tomography (PET) and magnetic resonance (MR).  Although, it is an essential part of the NiftyPET_ package for seamless PET image reconstruction, NIMPA is equally well suited for independent image processing, including image trimming, upsampling and partial volume correction (PVC).
+
+.. _NiftyPET: https://github.com/NiftyPET/NiftyPET
+
+Trimming is performed in order to reduce the unused image voxels in brain imaging, when using whole body PET scanners, for which only some part of the field of view (FOV) is used.
+
+The upsampling is needed for more accurate extraction (sampling) of PET data using regions of interest (ROI), obtained using parcellation of the corresponding T1w MR image, usually of higher image resolution.
+
+PVC is needed to correct for the spill-in and spill-out of PET signal from defined ROIs (specific for any given application).
+
+**Documentation with installation manual and tutorials**: https://niftypet.readthedocs.io/
+
+Quick Install
+~~~~~~~~~~~~~
+
+Note that it's recommended (but not required) to use `conda`.
+
+.. code:: sh
+
+    # cross-platform install
+    conda install -c conda-forge python=3 \
+      ipykernel numpy scipy scikit-image matplotlib ipywidgets dipy nibabel pydicom
+    pip install "nimpa>=2"
+
+For optional `dcm2niix <https://github.com/rordenlab/dcm2niix>`_ (image conversion from DICOM to NIfTI) and/or `niftyreg <https://github.com/KCL-BMEIS/niftyreg>`_ (image registration) support, simply install them separately (``pip install dcm2niix niftyreg``).
+
+External CMake Projects
+~~~~~~~~~~~~~~~~~~~~~~~
+
+The raw C/CUDA libraries may be included in external projects using ``cmake``.
+Simply build the project and use ``find_package(NiftyPETnimpa)``.
+
+.. code:: sh
+
+    # print installation directory (after `pip install nimpa`)...
+    python -c "from niftypet.nimpa import cmake_prefix; print(cmake_prefix)"
+
+    # ... or build & install directly with cmake
+    mkdir build && cd build
+    cmake ../niftypet && cmake --build . && cmake --install . --prefix /my/install/dir
+
+At this point any external project may include NIMPA as follows
+(Once setting ``-DCMAKE_PREFIX_DIR=<installation prefix from above>``):
+
+.. code:: cmake
+
+    cmake_minimum_required(VERSION 3.3 FATAL_ERROR)
+    project(myproj)
+    find_package(NiftyPETnimpa COMPONENTS improc REQUIRED)
+    add_executable(myexe ...)
+    target_link_libraries(myexe PRIVATE NiftyPET::improc)
+
+Licence
+~~~~~~~
+
+|Licence| |DOI|
+
+Copyright 2018-21
+
+- `Pawel J. Markiewicz <https://github.com/pjmark>`__ @ University College London
+- `Casper O. da Costa-Luis <https://github.com/casperdcl>`__ @ University College London/King's College London
+- `Contributors <https://github.com/NiftyPET/NIMPA/graphs/contributors>`__
+
+.. |Docs| image:: https://readthedocs.org/projects/niftypet/badge/?version=latest
+   :target: https://niftypet.readthedocs.io/en/latest/?badge=latest
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4417633.svg
+   :target: https://doi.org/10.5281/zenodo.4417633
+.. |Licence| image:: https://img.shields.io/pypi/l/nimpa.svg?label=licence
+   :target: https://github.com/NiftyPET/NIMPA/blob/master/LICENCE
+.. |Tests| image:: https://img.shields.io/github/workflow/status/NiftyPET/NIMPA/Test?logo=GitHub
+   :target: https://github.com/NiftyPET/NIMPA/actions
+.. |Downloads| image:: https://img.shields.io/pypi/dm/nimpa.svg?logo=pypi&logoColor=white&label=PyPI%20downloads
+   :target: https://pypi.org/project/nimpa
+.. |Version| image:: https://img.shields.io/pypi/v/nimpa.svg?logo=python&logoColor=white
+   :target: https://github.com/NiftyPET/NIMPA/releases
+.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/nimpa.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/nimpa
```

### Comparing `nimpa-2.5.1/setup.py` & `nimpa-2.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 """
 Compile CUDA source code and setup Python 3 package 'nimpa'
 for namespace 'niftypet'.
 """
 import logging
 import re
-import sys
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools_scm import get_version
 
 from niftypet.ninst import cudasetup as cs
 from niftypet.ninst import dinf
@@ -34,21 +33,24 @@
 # if exists, import the resources and get the constants
 resources = cs.get_resources()
 # get the current setup, if any
 Cnt = resources.get_setup()
 
 build_ver = ".".join(__version__.split('.')[:3]).split(".dev")[0]
 setup_kwargs = {
-    "use_scm_version": True, "packages": find_packages(exclude=["tests"]),
-    "package_data": {"niftypet": ["nimpa/auxdata/*"]}, "install_requires": [
-        'dipy>=1.3.0', 'miutil[nii]>=0.10.0', 'nibabel>=2.4.0', 'ninst>=0.12.0', 'numpy>=1.14',
-        'pydicom>=1.0.2', 'scipy', 'setuptools', 'spm12']}
+    "use_scm_version": True, "packages": find_packages(exclude=["tests"]), "package_data": {
+        "niftypet": [
+            "nimpa/auxdata/*", "nimpa/acr_design/core_mumap/*", "nimpa/acr_design/core_nac/*",
+            "nimpa/acr_design/rods/*", "nimpa/acr_design/sampling/*"]}, "install_requires": [
+                'dcm2niix', 'dipy>=1.3.0', 'imageio', 'miutil[nii]>=0.10.0', 'nibabel>=2.4.0',
+                'ninst>=0.12.0', 'numpy>=1.14', 'pydicom>=1.0.2', 'scipy', 'setuptools', 'spm12',
+                'SimpleITK']}
 # 'SimpleITK>=1.2.0'
 cmake_args = [
-    f"-DNIMPA_BUILD_VERSION={build_ver}", f"-DPython3_ROOT_DIR={sys.prefix}",
+    f"-DNIMPA_BUILD_VERSION={build_ver}",
     f"-DNIMPA_KERNEL_RADIUS={getattr(resources, 'RSZ_PSF_KRNL', 8)}"]
 
 try:
     import cuvec as cu
     from skbuild import setup as sksetup
     assert cu.include_path.is_dir()
     nvcc_arches = {"{2:d}{3:d}".format(*i) for i in dinf.gpuinfo() if i[2:4] >= (3, 5)}
```

### Comparing `nimpa-2.5.1/tests/test_improc.py` & `nimpa-2.6.0/tests/test_improc.py`

 * *Files identical despite different names*

