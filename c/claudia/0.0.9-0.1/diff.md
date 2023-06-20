# Comparing `tmp/claudia-0.0.9.tar.gz` & `tmp/claudia-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claudia-0.0.9.tar", last modified: Mon May 22 22:47:31 2023, max compression
+gzip compressed data, was "claudia-0.1.tar", last modified: Tue Jun 20 17:54:42 2023, max compression
```

## Comparing `claudia-0.0.9.tar` & `claudia-0.1.tar`

### file list

```diff
@@ -1,87 +1,105 @@
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.041493 claudia-0.0.9/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1073 2023-05-11 10:47:00.000000 claudia-0.0.9/LICENSE
--rw-r--r--   0 ksaxena    (502) staff       (20)     3533 2023-05-22 22:47:31.041286 claudia-0.0.9/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     4935 2023-05-20 01:17:00.000000 claudia-0.0.9/README.md
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.016780 claudia-0.0.9/claudia.egg-info/
--rw-r--r--   0 ksaxena    (502) staff       (20)     3533 2023-05-22 22:47:30.000000 claudia-0.0.9/claudia.egg-info/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     2610 2023-05-22 22:47:30.000000 claudia-0.0.9/claudia.egg-info/SOURCES.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-05-22 22:47:30.000000 claudia-0.0.9/claudia.egg-info/dependency_links.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-22 22:47:30.000000 claudia-0.0.9/claudia.egg-info/entry_points.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       88 2023-05-22 22:47:30.000000 claudia-0.0.9/claudia.egg-info/requires.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-05-22 22:47:30.000000 claudia-0.0.9/claudia.egg-info/top_level.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-05-22 22:47:31.041576 claudia-0.0.9/setup.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)     1477 2023-05-22 19:16:03.000000 claudia-0.0.9/setup.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.009898 claudia-0.0.9/src/
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.018624 claudia-0.0.9/src/claudia/
--rw-r--r--   0 ksaxena    (502) staff       (20)     3184 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/README.md
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    13074 2023-05-22 22:45:51.000000 claudia-0.0.9/src/claudia/claudia.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.019898 claudia-0.0.9/src/claudia/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/features/nft_burn_mint.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/features/payments.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/features/trustline.feature
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.022337 claudia-0.0.9/src/claudia/javascript/
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/cleanup
--rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/cucumber.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.022698 claudia-0.0.9/src/claudia/javascript/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1226 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/context.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.023935 claudia-0.0.9/src/claudia/javascript/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)     2106 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/lib/ObjFactory.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.026052 claudia-0.0.9/src/claudia/javascript/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    38728 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/steps/common.js
--rw-r--r--   0 ksaxena    (502) staff       (20)      300 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/steps/constants.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/steps/nft_mint_burn.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/steps/payments.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/steps/trustline.js
--rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/package-lock.json
--rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/package.json
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      869 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     4674 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/runTest
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.027301 claudia-0.0.9/src/claudia/network_setup/
--rw-rw-r--   0 ksaxena    (502) staff       (20)      251 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/Dockerfile
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.028414 claudia-0.0.9/src/claudia/network_setup/configs/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     1520 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled.cfg
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.029182 claudia-0.0.9/src/claudia/network_setup/configs/rippled_1/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2150 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_1/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_1/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.029997 claudia-0.0.9/src/claudia/network_setup/configs/rippled_2/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_2/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_2/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.030851 claudia-0.0.9/src/claudia/network_setup/configs/rippled_3/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_3/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_3/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.031551 claudia-0.0.9/src/claudia/network_setup/configs/rippled_4/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2190 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_4/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_4/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.032268 claudia-0.0.9/src/claudia/network_setup/configs/rippled_5/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2226 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_5/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_5/validators.txt
--rw-rw-r--   0 ksaxena    (502) staff       (20)      279 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.033877 claudia-0.0.9/src/claudia/network_setup/lib/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     1619 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/lib/build_rippled.sh
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2161 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/lib/rippled_network.yml
--rw-rw-r--   0 ksaxena    (502) staff       (20)     9944 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/lib/setup_helper.sh
--rw-rw-r--   0 ksaxena    (502) staff       (20)     5094 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/lib/validate_network.py
--rw-rw-r--   0 ksaxena    (502) staff       (20)     3800 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/setup.sh
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.036032 claudia-0.0.9/src/claudia/python/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/behave.ini
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/cleanup
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.037077 claudia-0.0.9/src/claudia/python/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     2977 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/environment.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.037804 claudia-0.0.9/src/claudia/python/features/exceptions/
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/exceptions/InvalidInputException.py
--rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/exceptions/UnconfiguredEnvironmentException.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.038633 claudia-0.0.9/src/claudia/python/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)      301 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/lib/Helpers.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     7674 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/lib/ObjFactory.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.040792 claudia-0.0.9/src/claudia/python/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    24750 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/steps/common.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/steps/constants.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    66340 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/steps/nft_mint_burn.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    21822 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/steps/payments.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    54620 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/steps/trustline.py
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     1381 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     5634 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/runTest
--rw-r--r--   0 ksaxena    (502) staff       (20)       88 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/requirements.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.850494 claudia-0.1/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1074 2023-05-25 22:01:40.000000 claudia-0.1/LICENSE
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11118 2023-06-20 17:54:42.850088 claudia-0.1/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)      402 2023-06-20 16:42:24.000000 claudia-0.1/README.md
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.821787 claudia-0.1/claudia.egg-info/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11118 2023-06-20 17:54:42.000000 claudia-0.1/claudia.egg-info/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3558 2023-06-20 17:54:42.000000 claudia-0.1/claudia.egg-info/SOURCES.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-06-20 17:54:42.000000 claudia-0.1/claudia.egg-info/dependency_links.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-06-20 17:54:42.000000 claudia-0.1/claudia.egg-info/entry_points.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)      109 2023-06-20 17:54:42.000000 claudia-0.1/claudia.egg-info/requires.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-06-20 17:54:42.000000 claudia-0.1/claudia.egg-info/top_level.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-06-20 17:54:42.850607 claudia-0.1/setup.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1475 2023-06-20 17:53:03.000000 claudia-0.1/setup.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.812449 claudia-0.1/src/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.823321 claudia-0.1/src/claudia/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    10771 2023-06-20 17:53:03.000000 claudia-0.1/src/claudia/README.md
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    37453 2023-06-20 17:53:03.000000 claudia-0.1/src/claudia/claudia.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.824366 claudia-0.1/src/claudia/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/features/nft_burn_mint.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-06-16 17:41:43.000000 claudia-0.1/src/claudia/features/payments.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/features/trustline.feature
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.826888 claudia-0.1/src/claudia/javascript/
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/javascript/cleanup
+-rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/javascript/cucumber.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.827180 claudia-0.1/src/claudia/javascript/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1227 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/javascript/features/context.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.827620 claudia-0.1/src/claudia/javascript/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2107 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/javascript/features/lib/ObjFactory.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.829265 claudia-0.1/src/claudia/javascript/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    38910 2023-06-20 16:42:24.000000 claudia-0.1/src/claudia/javascript/features/steps/common.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)      303 2023-06-05 20:21:20.000000 claudia-0.1/src/claudia/javascript/features/steps/constants.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/javascript/features/steps/nft_mint_burn.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/javascript/features/steps/payments.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/javascript/features/steps/trustline.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-06-14 21:08:34.000000 claudia-0.1/src/claudia/javascript/package-lock.json
+-rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/javascript/package.json
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      870 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/javascript/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     5028 2023-06-20 16:42:24.000000 claudia-0.1/src/claudia/javascript/runTest
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.830175 claudia-0.1/src/claudia/network_setup/
+-rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/Dockerfile.rippled_build
+-rw-r--r--   0 ksaxena    (502) staff       (20)      714 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/Dockerfile.rippled_install
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.815733 claudia-0.1/src/claudia/network_setup/configs/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.815416 claudia-0.1/src/claudia/network_setup/configs/rippled/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.830834 claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_1/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1796 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_1/rippled.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_1/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.831389 claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_2/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1838 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_2/rippled.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_2/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.832081 claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_3/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1838 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_3/rippled.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_3/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.832691 claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_4/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1837 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_4/rippled.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)      119 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_4/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.833034 claudia-0.1/src/claudia/network_setup/configs/sidechain/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2150 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/sidechain/bridge_bootstrap.json
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.834550 claudia-0.1/src/claudia/network_setup/configs/sidechain/witness/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1212 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/sidechain/witness/witness01.json
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1211 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/sidechain/witness/witness02.json
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1211 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/sidechain/witness/witness03.json
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1211 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/sidechain/witness/witness04.json
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1211 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/configs/sidechain/witness/witness05.json
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.836489 claudia-0.1/src/claudia/network_setup/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1775 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/lib/build.sh
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1268 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/lib/rippled_network.yml
+-rw-r--r--   0 ksaxena    (502) staff       (20)    28048 2023-06-20 17:53:03.000000 claudia-0.1/src/claudia/network_setup/lib/setup_helper.sh
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1268 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/lib/sidechain_network.yml
+-rw-r--r--   0 ksaxena    (502) staff       (20)     5442 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/lib/validate_network.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3999 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/network_setup/lib/witness_action.sh
+-rw-r--r--   0 ksaxena    (502) staff       (20)     7323 2023-06-20 17:53:03.000000 claudia-0.1/src/claudia/network_setup/setup.sh
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.837964 claudia-0.1/src/claudia/python/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/python/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/python/behave.ini
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/python/cleanup
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.838556 claudia-0.1/src/claudia/python/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/python/features/__init__.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.838785 claudia-0.1/src/claudia/python/features/__pycache__/
+-rw-r--r--   0 ksaxena    (502) staff       (20)      191 2023-06-01 16:46:55.000000 claudia-0.1/src/claudia/python/features/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3210 2023-06-20 16:42:24.000000 claudia-0.1/src/claudia/python/features/environment.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.839596 claudia-0.1/src/claudia/python/features/exceptions/
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/python/features/exceptions/InvalidInputException.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/python/features/exceptions/UnconfiguredEnvironmentException.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.840217 claudia-0.1/src/claudia/python/features/exceptions/__pycache__/
+-rw-r--r--   0 ksaxena    (502) staff       (20)      461 2023-06-01 16:46:55.000000 claudia-0.1/src/claudia/python/features/exceptions/__pycache__/InvalidInputException.cpython-311.pyc
+-rw-r--r--   0 ksaxena    (502) staff       (20)      483 2023-06-01 16:46:55.000000 claudia-0.1/src/claudia/python/features/exceptions/__pycache__/UnconfiguredEnvironmentException.cpython-311.pyc
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.842716 claudia-0.1/src/claudia/python/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)      301 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/python/features/lib/Helpers.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     7674 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/python/features/lib/ObjFactory.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.844860 claudia-0.1/src/claudia/python/features/lib/__pycache__/
+-rw-r--r--   0 ksaxena    (502) staff       (20)      747 2023-06-01 16:46:55.000000 claudia-0.1/src/claudia/python/features/lib/__pycache__/Helpers.cpython-311.pyc
+-rw-r--r--   0 ksaxena    (502) staff       (20)     7136 2023-06-01 16:46:55.000000 claudia-0.1/src/claudia/python/features/lib/__pycache__/ObjFactory.cpython-311.pyc
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.847877 claudia-0.1/src/claudia/python/features/steps/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-06-20 17:54:42.848932 claudia-0.1/src/claudia/python/features/steps/__pycache__/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    28136 2023-06-16 17:13:32.000000 claudia-0.1/src/claudia/python/features/steps/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0 ksaxena    (502) staff       (20)      489 2023-06-16 17:07:49.000000 claudia-0.1/src/claudia/python/features/steps/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 ksaxena    (502) staff       (20)    24750 2023-06-16 17:41:43.000000 claudia-0.1/src/claudia/python/features/steps/common.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      252 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/python/features/steps/constants.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    66340 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/python/features/steps/nft_mint_burn.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    21822 2023-06-16 17:41:43.000000 claudia-0.1/src/claudia/python/features/steps/payments.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    54620 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/python/features/steps/trustline.py
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     1382 2023-05-30 20:36:34.000000 claudia-0.1/src/claudia/python/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     6158 2023-06-20 16:42:24.000000 claudia-0.1/src/claudia/python/runTest
+-rw-r--r--   0 ksaxena    (502) staff       (20)      109 2023-06-15 20:50:01.000000 claudia-0.1/src/claudia/requirements.txt
```

### Comparing `claudia-0.0.9/LICENSE` & `claudia-0.1/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `claudia-0.0.9/setup.py` & `claudia-0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         requirements = content.split('\n')
 
     return requirements
 
 
 setup(
     name='claudia',
-    version='0.0.9',
+    version='0.1',
     description='Run XRPL Automated Tests',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     author="Kausty Saxena",
     author_email="ksaxena@ripple.com",
     keywords="ripple xrpl python javascript",
     url='https://xrpl.org/',
```

### Comparing `claudia-0.0.9/src/claudia/features/nft_burn_mint.feature` & `claudia-0.1/src/claudia/features/nft_burn_mint.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.9/src/claudia/features/payments.feature` & `claudia-0.1/src/claudia/features/payments.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.9/src/claudia/features/trustline.feature` & `claudia-0.1/src/claudia/features/trustline.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.9/src/claudia/javascript/features/context.js` & `claudia-0.1/src/claudia/javascript/features/context.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -70,8 +70,8 @@
 00000450: 6674 5f6d 696e 745f 7265 7370 6f6e 7365  ft_mint_response
 00000460: 5f32 3a20 2727 2c0a 2020 2020 6e66 745f  _2: '',.    nft_
 00000470: 6275 726e 5f72 6573 706f 6e73 655f 313a  burn_response_1:
 00000480: 2027 272c 0a20 2020 206e 6674 5f62 7572   '',.    nft_bur
 00000490: 6e5f 7265 7370 6f6e 7365 5f32 3a20 2727  n_response_2: ''
 000004a0: 2c0a 2020 2020 6578 6365 7074 696f 6e3a  ,.    exception:
 000004b0: 2027 272c 0a20 2020 2074 6573 7453 7461   '',.    testSta
-000004c0: 7475 733a 2027 270a 7d3b                 tus: ''.};
+000004c0: 7475 733a 2027 270a 7d3b 0a              tus: ''.};.
```

### Comparing `claudia-0.0.9/src/claudia/javascript/features/lib/ObjFactory.js` & `claudia-0.1/src/claudia/javascript/features/lib/ObjFactory.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -125,8 +125,8 @@
 000007c0: 6565 3a20 2266 6565 5f72 6571 7565 7374  ee: "fee_request
 000007d0: 222c 0a20 2020 2020 2020 2054 783a 2022  ",.        Tx: "
 000007e0: 7478 222c 0a20 2020 2020 2020 2041 6363  tx",.        Acc
 000007f0: 6f75 6e74 4e46 5473 3a20 2261 6363 6f75  ountNFTs: "accou
 00000800: 6e74 5f6e 6674 7322 2c0a 2020 2020 2020  nt_nfts",.      
 00000810: 2020 4c65 6467 6572 4375 7272 656e 743a    LedgerCurrent:
 00000820: 2022 6c65 6467 6572 5f63 7572 7265 6e74   "ledger_current
-00000830: 220a 2020 2020 7d0a 7d3b                 ".    }.};
+00000830: 220a 2020 2020 7d0a 7d3b 0a              ".    }.};.
```

### Comparing `claudia-0.0.9/src/claudia/javascript/features/steps/common.js` & `claudia-0.1/src/claudia/javascript/features/steps/common.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -172,18 +172,22 @@
     return response
 }
 
 async function getClient() {
     let client = null
     context.url = `${context.connectionScheme}://${context.connectionUrl}`;
     if (context.connectionType == "websocket") {
-        client = new xrpl.Client(context.url, {
-            feeCushion: 1
-        });
-        await client.connect()
+        try {
+            client = new xrpl.Client(context.url, {
+                feeCushion: 1
+            });
+            await client.connect()
+        } catch (error) {
+            throw new Error("\nERROR: Cannot connect to " + context.url + ". Make sure the network is accessible.")
+        }
     } else {
         throw "Unsupported CONNECTION_TYPE = '" + context.connectionType + "'";
     }
     return client;
 }
 
 async function get_account_info_response(context, account_id) {
```

### Comparing `claudia-0.0.9/src/claudia/javascript/features/steps/nft_mint_burn.js` & `claudia-0.1/src/claudia/javascript/features/steps/nft_mint_burn.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.9/src/claudia/javascript/features/steps/payments.js` & `claudia-0.1/src/claudia/javascript/features/steps/payments.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.9/src/claudia/javascript/features/steps/trustline.js` & `claudia-0.1/src/claudia/javascript/features/steps/trustline.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.9/src/claudia/javascript/package-lock.json` & `claudia-0.1/src/claudia/javascript/package-lock.json`

 * *Files identical despite different names*

### Comparing `claudia-0.0.9/src/claudia/javascript/runSetup` & `claudia-0.1/src/claudia/javascript/runSetup`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 }
 
 # cd javascript/
 validate_launch_dir
 # detect_OS
 validate_node
 regenearate_node_modules
-script_teardown 0
+script_teardown 0
```

### Comparing `claudia-0.0.9/src/claudia/javascript/runTest` & `claudia-0.1/src/claudia/javascript/runTest`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # !/bin/bash
 set +e
 
 final_exit_status=1
 clientType="websocket"
-network="local"
+network="local-mainnet"
 tag="smoke"
 feature="payments"
 
 trap 'script_teardown 1' INT
 
 function usage() {
   echo "Usage: $0 [Optional parameters]"
-  echo "\n  --network: The network to be used to run the tests on. Allowed values are 'local', 'devnet' and 'testnet' and is defaulted to $network. \n  More information: https://xrpl.org/parallel-networks.html"
+  echo "\n  --network: The network to be used to run the tests on. Allowed values are 'local-mainnet', 'local-sidechain', 'devnet' and 'testnet' and is defaulted to $network. \n  More information: https://xrpl.org/parallel-networks.html"
   echo "\n  --tag: Tag name of the all the tests to be included in the test run. Allowed values are 'smoke', 'regression' and 'time_intensive' and is defaulted to $tag. \n  More information: https://cucumber.io/docs/cucumber/api/?lang=javascript#tags"
   echo "\n  --feature <Feature file to be used for the test run. Allowed values are 'payments', 'trustline', 'nft_mint_burn', and 'all' and is defaulted to $feature. \n  More information: https://cucumber.io/docs/gherkin/reference/"
   echo "\n"
   exit 1
 }
 
 function load_feature_files() {  
@@ -32,17 +32,17 @@
   exit_status=${1:-1}
   cleanup_feature_files
   cd ..
   exit ${exit_status}
 }
 
 function validate_input_flags() {
-  if [[ "${network}" != "local" ]] && [[ "${network}" != "devnet" ]] && [[ "${network}" != "testnet" ]];
+  if [[ "${network}" != "local-mainnet" ]] && [[ "${network}" != "devnet" ]] && [[ "${network}" != "testnet" ]] && [[ "${network}" != "local-sidechain" ]];
   then
-    echo "ERROR: Invalid network. Flag is set to '$network'. Allowed values are 'local', 'devnet' and 'testnet'."
+    echo "ERROR: Invalid network. Flag is set to '$network'. Allowed values are 'local-mainnet', 'local-sidechain', 'devnet' and 'testnet'."
     usage
     script_teardown 1
   fi
 
   if [[ "${tag}" != "smoke" ]] && [[ "${tag}" != "regression" ]] && [[ "${tag}" != "time_intensive" ]];
   then
     echo "ERROR: Invalid tag. Flag is set to '$tag'. Allowed values are 'smoke', 'regression' and 'time_intensive'."
@@ -55,24 +55,34 @@
     echo "ERROR: Invalid feature. Flag is set to '$feature'. Allowed values are 'payments', 'trustline', 'nft_mint_burn', and 'all'."
     usage
     script_teardown 1
   fi
 }
 
 function set_launch_vars() {
-  if [[ $network == "local" ]];
+  if [[ $network == "local-mainnet" ]];
   then
     if [[ $clientType = "websocket" ]];
     then
       export CONNECTION_SCHEME="ws"
-      export CONNECTION_URL="127.0.0.5:6006"
+      export CONNECTION_URL="127.0.0.1:6001"
       export CONNECTION_TYPE="websocket"
     fi
   fi
   
+  if [[ $network == "local-sidechain" ]];
+  then
+    if [[ $clientType = "websocket" ]];
+    then
+      export CONNECTION_SCHEME="ws"
+      export CONNECTION_URL="127.0.0.1:6003"
+      export CONNECTION_TYPE="websocket"
+    fi
+  fi
+
   if [[ $network == "devnet" ]];
   then
     if [[ $clientType = "websocket" ]];
     then
       export CONNECTION_SCHEME="wss"
       export CONNECTION_URL="s.devnet.rippletest.net:51233"
       export CONNECTION_TYPE="websocket"
```

### Comparing `claudia-0.0.9/src/claudia/network_setup/configs/rippled.cfg` & `claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_1/rippled.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,79 @@
 [network_id]
 12
 
 [server]
-port_rpc
+port_rpc_admin_local
 port_peer
-port_ws
+port_ws_admin_local
 
-
-[port_rpc]
+[port_rpc_admin_local]
 port = 51234
 ip = 0.0.0.0
-admin = 127.0.0.1
-protocol =  https, http
+admin = 0.0.0.0
+protocol = http
 
 [port_peer]
-# port = 2459
-port = 3000
+port = 2459
 ip = 0.0.0.0
+# alternatively, to accept connections on IPv4 + IPv6, use:
+#ip = ::
 protocol = peer
 
-[port_ws]
-port = 51233
+[port_ws_admin_local]
+port = 6006
 ip = 0.0.0.0
-admin = 127.0.0.1
-protocol = wss2,ws
+admin = 0.0.0.0
+protocol = ws
 
 [port_grpc]
 port = 50051
-ip = 0.0.0.0
-
-[compression]
-true
-
-[node_size]
-huge
-
-[ssl_verify]
-0
-
-[ledger_history]
-full
+ip = 127.0.0.1
+secure_gateway = 127.0.0.1
 
 [node_db]
-type=nudb
-path=/var/lib/rippled/private_nw/db/nudb
-earliest_seq=3
+type=NuDB
+path=/var/lib/rippled/db/nudb
+earliest_seq=1
 
 [database_path]
-/var/lib/rippled/private_nw/db
+/var/lib/rippled/db
 
 [debug_logfile]
-/var/log/rippled/private_nw/debug.log
+/var/log/rippled/debug.log
+
+[sntp_servers]
+time.windows.com
+time.apple.com
+time.nist.gov
+pool.ntp.org
 
 [validators_file]
 validators.txt
 
-[ips_fixed]
-localhost 2459
-localhost 2469
-localhost 2479
-localhost 2489
-localhost 2499
+# Turn down default logging to save disk space in the long run.
+# Valid values here are trace, debug, info, warning, error, and fatal
+[rpc_startup]
+{ "command": "log_level", "severity": "warning" }
 
+# If ssl_verify is 1, certificates will be validated.
+# To allow the use of self-signed certificates for development or internal use,
+# set to ssl_verify to 0.
+[ssl_verify]
+1
 
-[rpc_startup]
-{ "command": "log_level", "severity": "debug" }
+[ips_fixed]
+rippled_1 2459
+rippled_2 2459
 
-[signing_support]
-true
+[validation_seed]
+shAnFpK99yUm8zAcAgrf3JyB6Gpts
 
-[voting]
-reference_fee = 8
-account_reserve = 10000000
-owner_reserve = 2000000
+[amendment_majority_time]
+30 minutes
 
 [features]
 PayChan  
 Flow
 FlowCross
 TickSize
 fix1368
@@ -112,12 +109,7 @@
 TicketBatch
 FlowSortStrands
 fixSTAmountCanonicalize
 fixRmSmallIncreasedQOffers
 CheckCashMakesTrustLine
 NonFungibleTokensV1
 NonFungibleTokensV1_1
-fixNonFungibleTokensV1_2
-XRPFees
-DisallowIncoming
-
-
```

### Comparing `claudia-0.0.9/src/claudia/network_setup/configs/rippled_1/rippled.cfg` & `claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_4/rippled.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+[network_id]
+22
+
 [server]
 port_rpc_admin_local
 port_peer
 port_ws_admin_local
-#port_ws_public
-#ssl_key = /etc/ssl/private/server.key
-#ssl_cert = /etc/ssl/certs/server.crt
 
 [port_rpc_admin_local]
 port = 51234
 ip = 0.0.0.0
 admin = 0.0.0.0
 protocol = http
 
@@ -26,37 +26,33 @@
 protocol = ws
 
 [port_grpc]
 port = 50051
 ip = 127.0.0.1
 secure_gateway = 127.0.0.1
 
-#[port_ws_public]
-#port = 6005
-#ip = 127.0.0.1
-#protocol = wss
-
 [node_db]
 type=NuDB
 path=/var/lib/rippled/db/nudb
-online_delete=512
-advisory_delete=0
+earliest_seq=1
 
 [database_path]
 /var/lib/rippled/db
 
 [debug_logfile]
 /var/log/rippled/debug.log
 
 [sntp_servers]
 time.windows.com
 time.apple.com
 time.nist.gov
 pool.ntp.org
 
+# [ips]
+# r.altnet.rippletest.net 51235
 [validators_file]
 validators.txt
 
 # Turn down default logging to save disk space in the long run.
 # Valid values here are trace, debug, info, warning, error, and fatal
 [rpc_startup]
 { "command": "log_level", "severity": "warning" }
@@ -65,30 +61,19 @@
 # To allow the use of self-signed certificates for development or internal use,
 # set to ssl_verify to 0.
 [ssl_verify]
 1
 
 
 [ips_fixed]
-rippled_1 2459
-rippled_2 2459
 rippled_3 2459
 rippled_4 2459
-rippled_5 2459
-
-[network_id]
-12
 
 [validation_seed]
-shAnFpK99yUm8zAcAgrf3JyB6Gpts
-
-[voting]
-reference_fee = 8
-account_reserve = 10000000
-owner_reserve = 2000000
+snjm2cyL7iLfHkJJZvKKBBGNdaq6e
 
 [amendment_majority_time]
 30 minutes
 
 [features]
 PayChan  
 Flow
@@ -127,11 +112,7 @@
 TicketBatch
 FlowSortStrands
 fixSTAmountCanonicalize
 fixRmSmallIncreasedQOffers
 CheckCashMakesTrustLine
 NonFungibleTokensV1
 NonFungibleTokensV1_1
-fixNonFungibleTokensV1_2
-XRPFees
-DisallowIncoming
-
```

### Comparing `claudia-0.0.9/src/claudia/network_setup/configs/rippled_2/rippled.cfg` & `claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_3/rippled.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+[network_id]
+22
+
 [server]
 port_rpc_admin_local
 port_peer
 port_ws_admin_local
-#port_ws_public
-#ssl_key = /etc/ssl/private/server.key
-#ssl_cert = /etc/ssl/certs/server.crt
 
 [port_rpc_admin_local]
 port = 51234
 ip = 0.0.0.0
 admin = 0.0.0.0
 protocol = http
 
@@ -26,24 +26,18 @@
 protocol = ws
 
 [port_grpc]
 port = 50051
 ip = 127.0.0.1
 secure_gateway = 127.0.0.1
 
-#[port_ws_public]
-#port = 6005
-#ip = 127.0.0.1
-#protocol = wss
-
 [node_db]
 type=NuDB
 path=/var/lib/rippled/db/nudb
-online_delete=512
-advisory_delete=0
+earliest_seq=1
 
 [database_path]
 /var/lib/rippled/db
 
 [debug_logfile]
 /var/log/rippled/debug.log
 
@@ -68,30 +62,19 @@
 # To allow the use of self-signed certificates for development or internal use,
 # set to ssl_verify to 0.
 [ssl_verify]
 1
 
 
 [ips_fixed]
-rippled_1 2459
-rippled_2 2459
 rippled_3 2459
 rippled_4 2459
-rippled_5 2459
-
-[network_id]
-12
 
 [validation_seed]
-ssEnojtkdgpVer28b2jVD98DYygrY
-
-[voting]
-reference_fee = 8
-account_reserve = 10000000
-owner_reserve = 2000000
+snaAU7bmrkMNwYm1pHFApyTDz6nA1
 
 [amendment_majority_time]
 30 minutes
 
 [features]
 PayChan  
 Flow
@@ -130,11 +113,7 @@
 TicketBatch
 FlowSortStrands
 fixSTAmountCanonicalize
 fixRmSmallIncreasedQOffers
 CheckCashMakesTrustLine
 NonFungibleTokensV1
 NonFungibleTokensV1_1
-fixNonFungibleTokensV1_2
-XRPFees
-DisallowIncoming
-
```

### Comparing `claudia-0.0.9/src/claudia/network_setup/configs/rippled_3/rippled.cfg` & `claudia-0.1/src/claudia/network_setup/configs/rippled/rippled_2/rippled.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+[network_id]
+12
+
 [server]
 port_rpc_admin_local
 port_peer
 port_ws_admin_local
-#port_ws_public
-#ssl_key = /etc/ssl/private/server.key
-#ssl_cert = /etc/ssl/certs/server.crt
 
 [port_rpc_admin_local]
 port = 51234
 ip = 0.0.0.0
 admin = 0.0.0.0
 protocol = http
 
@@ -26,24 +26,18 @@
 protocol = ws
 
 [port_grpc]
 port = 50051
 ip = 127.0.0.1
 secure_gateway = 127.0.0.1
 
-#[port_ws_public]
-#port = 6005
-#ip = 127.0.0.1
-#protocol = wss
-
 [node_db]
 type=NuDB
 path=/var/lib/rippled/db/nudb
-online_delete=512
-advisory_delete=0
+earliest_seq=1
 
 [database_path]
 /var/lib/rippled/db
 
 [debug_logfile]
 /var/log/rippled/debug.log
 
@@ -70,28 +64,17 @@
 [ssl_verify]
 1
 
 
 [ips_fixed]
 rippled_1 2459
 rippled_2 2459
-rippled_3 2459
-rippled_4 2459
-rippled_5 2459
-
-[network_id]
-12
 
 [validation_seed]
-snaAU7bmrkMNwYm1pHFApyTDz6nA1
-
-[voting]
-reference_fee = 8
-account_reserve = 10000000
-owner_reserve = 2000000
+ssEnojtkdgpVer28b2jVD98DYygrY
 
 [amendment_majority_time]
 30 minutes
 
 [features]
 PayChan  
 Flow
@@ -130,11 +113,7 @@
 TicketBatch
 FlowSortStrands
 fixSTAmountCanonicalize
 fixRmSmallIncreasedQOffers
 CheckCashMakesTrustLine
 NonFungibleTokensV1
 NonFungibleTokensV1_1
-fixNonFungibleTokensV1_2
-XRPFees
-DisallowIncoming
-
```

### Comparing `claudia-0.0.9/src/claudia/network_setup/lib/validate_network.py` & `claudia-0.1/src/claudia/network_setup/lib/validate_network.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,26 +6,24 @@
 # Usage:
 #   python3 scripts/validate_network.py [optional parameter]
 #       [--rippledServer <rippled host:port (default: localhost:5001)>
 ################################################################################
 
 import argparse
 import json
-import logging
 import sys
-
 import requests
 import time
 
 GENESIS_ACCOUNT_ID = "rHb9CJAWyB4rj91VRWn96DkukG4bwdtyTh"
 GENESIS_ACCOUNT_SEED = "snoPBrXtMeMyMHUVTgbuqAfg1SUTb"
 DEFAULT_RIPPLED_SERVER = "localhost:5001"
 TRANSFER_AMOUNT = "10000000000"
 DESTINATION_ACCOUNT_ID = "rh1HPuRVsYYvThxG2Bs1MfjmrVC73S16Fb"
-VALIDATION_CHECK_TIMEOUT = 180  # seconds
+VALIDATION_CHECK_TIMEOUT = 300  # seconds
 
 
 class RippledServer(object):
     def __init__(self, rippled_server=DEFAULT_RIPPLED_SERVER):
         self.rippled_server = "http://{}".format(rippled_server)
 
     def execute_transaction(self, payload, method):
@@ -92,38 +90,32 @@
                 else:
                     if tx_response["meta"]["TransactionResult"] == engine_result:
                         return True
             time.sleep(1)
         raise Exception("  Transaction not validated: {}".format(tx_id))
 
 
-def parse_arguments():
-    parser = argparse.ArgumentParser()
-    parser.add_argument('--rippledServer', default=DEFAULT_RIPPLED_SERVER,
-                        help="rippled server (default: {})".format(DEFAULT_RIPPLED_SERVER))
-    return parser.parse_args()
-
-
-def main(rippled_server):
-    rippled = RippledServer(rippled_server)
-    print("  Server State")
-
+def verify_network(rippled):
+    print("  Server State: ", end="")
     start_time = time.time()
     while True:
         time.sleep(5)
         server_info = rippled.execute_transaction(payload={}, method="server_info")
         server_state = server_info["info"]["server_state"]
         proposers = server_info["info"]["last_close"]["proposers"]
         if server_state in ("full", "proposing") and proposers != 0:
+            print("{}".format(server_state))
             break
 
         if time.time() > (start_time + VALIDATION_CHECK_TIMEOUT):
-            print("  {}".format(server_state))
+            print("{}".format(server_state))
             sys.exit(1)
 
+
+def verify_payment_txn(rippled):
     print("  Verify Payment Transaction")
     initial_balance = int(rippled.get_account_balance(DESTINATION_ACCOUNT_ID))
 
     payload = {
         "tx_json": {
             "TransactionType": "Payment",
             "Account": GENESIS_ACCOUNT_ID,
@@ -136,10 +128,26 @@
     new_balance = int(rippled.get_account_balance(DESTINATION_ACCOUNT_ID))
 
     if new_balance != (initial_balance + int(TRANSFER_AMOUNT)):
         print("  Account balance mismatch")
         sys.exit(1)
 
 
+def parse_arguments():
+    parser = argparse.ArgumentParser()
+    parser.add_argument('--rippledServer', default=DEFAULT_RIPPLED_SERVER,
+                        help="rippled server (default: {})".format(DEFAULT_RIPPLED_SERVER))
+    parser.add_argument("--paymentTransaction", help="Submit a Payment Transaction", action='store_true')
+
+    return parser.parse_args()
+
+
+def main(rippled_server, submit_payment_txn):
+    rippled = RippledServer(rippled_server)
+    verify_network(rippled)
+    if submit_payment_txn:
+        verify_payment_txn(rippled)
+
+
 if __name__ == '__main__':
     cmd_args = parse_arguments()
-    main(cmd_args.rippledServer)
+    main(cmd_args.rippledServer, cmd_args.paymentTransaction)
```

### Comparing `claudia-0.0.9/src/claudia/python/features/environment.py` & `claudia-0.1/src/claudia/python/features/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 
 
 def before_all(context):
     context.connectionType = read_env_var('CONNECTION_TYPE')
     connectionScheme = read_env_var('CONNECTION_SCHEME')
     connectionURL = read_env_var('CONNECTION_URL')
     context.url = "{}://{}".format(connectionScheme, connectionURL)
-    context.client = get_client(context)
+    try:
+        context.client = get_client(context)
+    except ConnectionRefusedError:
+        raise Exception("\nERROR: Cannot connect to {}. Make sure the network is accessible.".format(context.url))
     context.crypto_algorithm = CryptoAlgorithm.SECP256K1
     context.test_genesis_wallet = get_test_genesis_wallet(context)
     context.default_fee = int(get_fee(context.client))
 
 
 def get_test_genesis_wallet(context):
     test_genesis_account_id = "rh1HPuRVsYYvThxG2Bs1MfjmrVC73S16Fb"
@@ -56,15 +59,18 @@
     context.destinationWallet = None
     context.destinationAddress = ""
     context.destinationBalance = 0
 
 
 def after_all(context):
     if context.connectionType == "websocket":
-        context.client.close()
+        try:
+            context.client.close()
+        except AttributeError as e:
+            pass
 
 
 def get_client(context):
     if context.connectionType == "jsonrpc":
         client = JsonRpcClient(context.url)
     elif context.connectionType == "websocket":
         client = WebsocketClient(context.url)
```

### Comparing `claudia-0.0.9/src/claudia/python/features/lib/ObjFactory.py` & `claudia-0.1/src/claudia/python/features/lib/ObjFactory.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.9/src/claudia/python/features/steps/common.py` & `claudia-0.1/src/claudia/python/features/steps/common.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.9/src/claudia/python/features/steps/nft_mint_burn.py` & `claudia-0.1/src/claudia/python/features/steps/nft_mint_burn.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.9/src/claudia/python/features/steps/payments.py` & `claudia-0.1/src/claudia/python/features/steps/payments.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.9/src/claudia/python/features/steps/trustline.py` & `claudia-0.1/src/claudia/python/features/steps/trustline.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.9/src/claudia/python/runSetup` & `claudia-0.1/src/claudia/python/runSetup`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,8 @@
 
 # validate_launch_dir
 # detect_OS
 install_pip3
 install_xrpl_py
 install_behave
 install_py_hamcrest
-script_teardown 0
+script_teardown 0
```

### Comparing `claudia-0.0.9/src/claudia/python/runTest` & `claudia-0.1/src/claudia/python/runTest`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # !/bin/bash
 set +e
 
 clientType="websocket"
-network="local"
+network="local-mainnet"
 tag="smoke"
 feature="payments"
 
 trap 'script_teardown 1' INT
 
 function usage() {
   echo "Usage: $0 [Optional parameters]"
   echo "\n  --clientType: The type of client to be used. Allowed values are 'websocket' and 'jsonrpc' and is defaulted to $clientType. \n  More information: https://xrpl.org/get-started-using-http-websocket-apis.html#differences-between-json-rpc-and-websocket>"
-  echo "\n  --network: The network to be used to run the tests on. Allowed values are 'local', 'devnet' and 'testnet' and is defaulted to $network. \n  More information: https://xrpl.org/parallel-networks.html"
+  echo "\n  --network: The network to be used to run the tests on. Allowed values are 'local-mainnet', 'local-sidechain', 'devnet' and 'testnet' and is defaulted to $network. \n  More information: https://xrpl.org/parallel-networks.html"
   echo "\n  --tag: Tag name of the all the tests to be included in the test run. Allowed values are 'smoke', 'regression' and 'time_intensive' and is defaulted to $tag. \n  More information: https://behave.readthedocs.io/en/latest/tag_expressions.html"
   echo "\n  --feature <Feature file to be used for the test run. Allowed values are 'payments', 'trustline', 'nft_mint_burn', and 'all' and is defaulted to $feature. \n  More information: https://behave.readthedocs.io/en/latest/tutorial.html?highlight=feature#feature-files"
   echo "\n"
   exit 1
 }
 
 function load_feature_files() {
@@ -37,17 +37,17 @@
   then
     echo ${clientType}
     echo "ERROR: Invalid clientType. Flag is set to '$clientType'. Allowed values are 'websocket' and 'jsonrpc'."
     usage
     script_teardown 1
   fi
 
-  if [[ "${network}" != "local" ]] && [[ "${network}" != "devnet" ]] && [[ "${network}" != "testnet" ]];
+  if [[ "${network}" != "local-mainnet" ]] && [[ "${network}" != "devnet" ]] && [[ "${network}" != "testnet" ]] && [[ "${network}" != "local-sidechain" ]];
   then
-    echo "ERROR: Invalid network. Flag is set to '$network'. Allowed values are 'local', 'devnet' and 'testnet'."
+    echo "ERROR: Invalid network. Flag is set to '$network'. Allowed values are 'local-mainnet', 'local-sidechain', 'devnet' and 'testnet'."
     usage
     script_teardown 1
   fi
 
   if [[ "${tag}" != "smoke" ]] && [[ "${tag}" != "regression" ]] && [[ "${tag}" != "time_intensive" ]];
   then
     echo "ERROR: Invalid tag. Flag is set to '$tag'. Allowed values are 'smoke', 'regression' and 'time_intensive'."
@@ -60,29 +60,44 @@
     echo "ERROR: Invalid feature. Flag is set to '$feature'. Allowed values are 'payments', 'trustline', 'nft_mint_burn', and 'all'."
     usage
     script_teardown 1
   fi
 }
 
 function set_launch_vars() {
-  if [[ $network == "local" ]];
+  if [[ $network == "local-mainnet" ]];
   then
     if [[ $clientType = "websocket" ]];
     then
       export CONNECTION_SCHEME="ws"
-      export CONNECTION_URL="127.0.0.5:6006"
+      export CONNECTION_URL="127.0.0.1:6001"
       export CONNECTION_TYPE="websocket"
     elif [[ $clientType = "jsonrpc" ]];
     then
       export CONNECTION_SCHEME="http"
-      export CONNECTION_URL="127.0.0.5:51234"
+      export CONNECTION_URL="127.0.0.1:5001"
       export CONNECTION_TYPE="jsonrpc"
     fi
   fi
   
+  if [[ $network == "local-sidechain" ]];
+  then
+    if [[ $clientType = "websocket" ]];
+    then
+      export CONNECTION_SCHEME="ws"
+      export CONNECTION_URL="127.0.0.1:6003"
+      export CONNECTION_TYPE="websocket"
+    elif [[ $clientType = "jsonrpc" ]];
+    then
+      export CONNECTION_SCHEME="http"
+      export CONNECTION_URL="127.0.0.1:5003"
+      export CONNECTION_TYPE="jsonrpc"
+    fi
+  fi
+
   if [[ $network == "devnet" ]];
   then
     if [[ $clientType = "websocket" ]];
     then
       export CONNECTION_SCHEME="wss"
       export CONNECTION_URL="s.devnet.rippletest.net:51233"
       export CONNECTION_TYPE="websocket"
```

