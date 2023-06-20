# Comparing `tmp/datacrunch-1.4.0.tar.gz` & `tmp/datacrunch-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacrunch-1.4.0.tar", last modified: Wed Jun 14 14:08:27 2023, max compression
+gzip compressed data, was "datacrunch-1.4.1.tar", last modified: Tue Jun 20 13:53:07 2023, max compression
```

## Comparing `datacrunch-1.4.0.tar` & `datacrunch-1.4.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.131384 datacrunch-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 14:08:17.000000 datacrunch-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-14 14:08:27.131384 datacrunch-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-14 14:08:17.000000 datacrunch-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/authentication/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch/balance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/balance/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch/http_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/http_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/http_client/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/images/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch/instance_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/instance_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/instance_types/instance_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/datacrunch/instances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/instances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/instances/instances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/datacrunch/ssh_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/ssh_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/ssh_keys/ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/datacrunch/startup_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/startup_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/startup_scripts/startup_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/datacrunch/volume_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/volume_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/volume_types/volume_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/datacrunch/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-06-14 14:08:17.000000 datacrunch-1.4.0/datacrunch/volumes/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.123384 datacrunch-1.4.0/datacrunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-14 14:08:27.000000 datacrunch-1.4.0/datacrunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-14 14:08:27.000000 datacrunch-1.4.0/datacrunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:08:27.000000 datacrunch-1.4.0/datacrunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-14 14:08:27.000000 datacrunch-1.4.0/datacrunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 14:08:27.000000 datacrunch-1.4.0/datacrunch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 14:08:27.131384 datacrunch-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-14 14:08:17.000000 datacrunch-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/integration_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/integration_tests/test_volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/authentication/test_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/balance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/balance/test_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/http_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/http_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/http_client/test_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/images/test_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/instance_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/instance_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/instance_types/test_instance_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/instances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/instances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/instances/test_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/ssh_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/ssh_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/ssh_keys/test_ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.127385 datacrunch-1.4.0/tests/unit_tests/startup_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/startup_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/startup_scripts/test_startup_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/test_datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/test_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.131384 datacrunch-1.4.0/tests/unit_tests/volume_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/volume_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/volume_types/test_volume_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:27.131384 datacrunch-1.4.0/tests/unit_tests/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-06-14 14:08:17.000000 datacrunch-1.4.0/tests/unit_tests/volumes/test_volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 13:52:42.000000 datacrunch-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-20 13:53:07.079662 datacrunch-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-20 13:52:42.000000 datacrunch-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.075662 datacrunch-1.4.1/datacrunch/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.075662 datacrunch-1.4.1/datacrunch/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/authentication/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.075662 datacrunch-1.4.1/datacrunch/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/balance/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.075662 datacrunch-1.4.1/datacrunch/http_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/http_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/http_client/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.075662 datacrunch-1.4.1/datacrunch/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/images/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.075662 datacrunch-1.4.1/datacrunch/instance_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/instance_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/instance_types/instance_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.075662 datacrunch-1.4.1/datacrunch/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/instances/instances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.075662 datacrunch-1.4.1/datacrunch/ssh_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/ssh_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/ssh_keys/ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/datacrunch/startup_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/startup_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/startup_scripts/startup_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/datacrunch/volume_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/volume_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/volume_types/volume_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/datacrunch/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-06-20 13:52:42.000000 datacrunch-1.4.1/datacrunch/volumes/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.075662 datacrunch-1.4.1/datacrunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-20 13:53:07.000000 datacrunch-1.4.1/datacrunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-20 13:53:07.000000 datacrunch-1.4.1/datacrunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:53:07.000000 datacrunch-1.4.1/datacrunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-20 13:53:07.000000 datacrunch-1.4.1/datacrunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 13:53:07.000000 datacrunch-1.4.1/datacrunch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:53:07.079662 datacrunch-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-20 13:52:42.000000 datacrunch-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/integration_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/integration_tests/test_volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/unit_tests/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/authentication/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/unit_tests/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/balance/test_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/unit_tests/http_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/http_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/http_client/test_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/unit_tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/images/test_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/unit_tests/instance_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/instance_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/instance_types/test_instance_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/unit_tests/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/instances/test_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/unit_tests/ssh_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/ssh_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/ssh_keys/test_ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/unit_tests/startup_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/startup_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/startup_scripts/test_startup_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/test_datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/test_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/unit_tests/volume_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/volume_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/volume_types/test_volume_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:53:07.079662 datacrunch-1.4.1/tests/unit_tests/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-06-20 13:52:42.000000 datacrunch-1.4.1/tests/unit_tests/volumes/test_volumes.py
```

### Comparing `datacrunch-1.4.0/LICENSE` & `datacrunch-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/PKG-INFO` & `datacrunch-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacrunch
-Version: 1.4.0
+Version: 1.4.1
 Summary: Official Python SDK for DataCrunch Public API
 Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy
 Author-email: info@datacrunch.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datacrunch Version: 1.4.0 Summary: Official Python
+Metadata-Version: 2.1 Name: datacrunch Version: 1.4.1 Summary: Official Python
 SDK for DataCrunch Public API Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy Author-email: info@datacrunch.io Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Development Status :: 5 - Production/
```

### Comparing `datacrunch-1.4.0/README.md` & `datacrunch-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch/authentication/authentication.py` & `datacrunch-1.4.1/datacrunch/authentication/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,20 @@
         payload = {
             "grant_type": REFRESH_TOKEN,
             "refresh_token": self._refresh_token
         }
 
         response = requests.post(
             url, json=payload, headers=self._generate_headers())
-        handle_error(response)
+
+        # if refresh token is also expired, authenticate again:
+        if response.status_code == 401 or response.status_code == 400:
+            return self.authenticate()
+        else:
+            handle_error(response)
 
         auth_data = response.json()
 
         self._access_token = auth_data['access_token']
         self._refresh_token = auth_data['refresh_token']
         self._scope = auth_data['scope']
         self._token_type = auth_data['token_type']
@@ -100,8 +105,8 @@
 
     def is_expired(self) -> bool:
         """Returns true if the access token is expired.
 
         :return: True if the access token is expired, otherwise False.
         :rtype: bool
         """
-        return time.time() > self._expires_at
+        return time.time() >= self._expires_at
```

### Comparing `datacrunch-1.4.0/datacrunch/balance/balance.py` & `datacrunch-1.4.1/datacrunch/balance/balance.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch/constants.py` & `datacrunch-1.4.1/datacrunch/constants.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch/datacrunch.py` & `datacrunch-1.4.1/datacrunch/datacrunch.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch/exceptions.py` & `datacrunch-1.4.1/datacrunch/exceptions.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch/helpers.py` & `datacrunch-1.4.1/datacrunch/helpers.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch/http_client/http_client.py` & `datacrunch-1.4.1/datacrunch/http_client/http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,19 +45,19 @@
         :type json: dict, optional
 
         :raises APIException: an api exception with message and error type code
 
         :return: Response object
         :rtype: requests.Response
         """
+        self._refresh_token_if_expired()
+
         url = self._add_base_url(url)
         headers = self._generate_headers()
 
-        self._refresh_token_if_expired()
-
         response = requests.post(url, json=json, headers=headers, **kwargs)
         handle_error(response)
 
         return response
 
     def put(self, url: str, json: dict = None, **kwargs) -> requests.Response:
         """Sends a PUT request.
@@ -72,19 +72,19 @@
         :type json: dict, optional
 
         :raises APIException: an api exception with message and error type code
 
         :return: Response object
         :rtype: requests.Response
         """
+        self._refresh_token_if_expired()
+
         url = self._add_base_url(url)
         headers = self._generate_headers()
 
-        self._refresh_token_if_expired()
-
         response = requests.put(url, json=json, headers=headers, **kwargs)
         handle_error(response)
 
         return response
 
     def get(self, url: str, params: dict = None, **kwargs) -> requests.Response:
         """Sends a GET request.
@@ -99,19 +99,19 @@
         :type params: dict, optional
 
         :raises APIException: an api exception with message and error type code
 
         :return: Response object
         :rtype: requests.Response
         """
+        self._refresh_token_if_expired()
+
         url = self._add_base_url(url)
         headers = self._generate_headers()
 
-        self._refresh_token_if_expired()
-
         response = requests.get(url, params=params, headers=headers, **kwargs)
         handle_error(response)
 
         return response
 
     def delete(self, url: str, json: dict = None, **kwargs) -> requests.Response:
         """Sends a DELETE request.
@@ -126,32 +126,32 @@
         :type json: dict, optional
 
         :raises APIException: an api exception with message and error type code
 
         :return: Response object
         :rtype: requests.Response
         """
+        self._refresh_token_if_expired()
+
         url = self._add_base_url(url)
         headers = self._generate_headers()
 
-        self._refresh_token_if_expired()
-
         response = requests.delete(url, headers=headers, json=json, **kwargs)
         handle_error(response)
 
         return response
 
     def _refresh_token_if_expired(self) -> None:
         """refreshes the access token if it expired.
 
         Uses the refresh token to refresh, and if the refresh token is also expired, uses the client credentials.
 
         :raises APIException: an api exception with message and error type code
         """
-        if(self._auth_service.is_expired()):
+        if (self._auth_service.is_expired()):
             # try to refresh. if refresh token has expired, reauthenticate
             try:
                 self._auth_service.refresh()
             except Exception:
                 self._auth_service.authenticate()
 
     def _generate_headers(self) -> dict:
@@ -178,15 +178,15 @@
     def _generate_user_agent(self) -> str:
         """generate the user agent string.
 
         :return: user agent string
         :rtype: str
         """
         # get the first 10 chars of the client id
-        client_id_truncated = self._auth_service._client_id[:10]  
+        client_id_truncated = self._auth_service._client_id[:10]
 
         return f'datacrunch-python-v{self._version}-{client_id_truncated}'
 
     def _add_base_url(self, url: str) -> str:
         """Adds the base url to the relative url
 
         example:
```

### Comparing `datacrunch-1.4.0/datacrunch/images/images.py` & `datacrunch-1.4.1/datacrunch/images/images.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch/instance_types/instance_types.py` & `datacrunch-1.4.1/datacrunch/instance_types/instance_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch/instances/instances.py` & `datacrunch-1.4.1/datacrunch/instances/instances.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch/ssh_keys/ssh_keys.py` & `datacrunch-1.4.1/datacrunch/ssh_keys/ssh_keys.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch/startup_scripts/startup_scripts.py` & `datacrunch-1.4.1/datacrunch/startup_scripts/startup_scripts.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch/volume_types/volume_types.py` & `datacrunch-1.4.1/datacrunch/volume_types/volume_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch/volumes/volumes.py` & `datacrunch-1.4.1/datacrunch/volumes/volumes.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/datacrunch.egg-info/PKG-INFO` & `datacrunch-1.4.1/datacrunch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacrunch
-Version: 1.4.0
+Version: 1.4.1
 Summary: Official Python SDK for DataCrunch Public API
 Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy
 Author-email: info@datacrunch.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datacrunch Version: 1.4.0 Summary: Official Python
+Metadata-Version: 2.1 Name: datacrunch Version: 1.4.1 Summary: Official Python
 SDK for DataCrunch Public API Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy Author-email: info@datacrunch.io Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Development Status :: 5 - Production/
```

### Comparing `datacrunch-1.4.0/datacrunch.egg-info/SOURCES.txt` & `datacrunch-1.4.1/datacrunch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/setup.py` & `datacrunch-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/integration_tests/conftest.py` & `datacrunch-1.4.1/tests/integration_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/integration_tests/test_volumes.py` & `datacrunch-1.4.1/tests/integration_tests/test_volumes.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/unit_tests/authentication/test_authentication.py` & `datacrunch-1.4.1/tests/unit_tests/authentication/test_authentication.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-import responses # https://github.com/getsentry/responses
+import responses  # https://github.com/getsentry/responses
 from responses import matchers
 import time
 
 from datacrunch.exceptions import APIException
 from datacrunch.authentication.authentication import AuthenticationService
 
 INVALID_REQUEST = 'invalid_request'
@@ -18,14 +18,15 @@
 SCOPE = 'fullAccess'
 TOKEN_TYPE = 'Bearer'
 EXPIRES_IN = 3600
 
 ACCESS_TOKEN2 = 'access2'
 REFRESH_TOKEN2 = 'refresh2'
 
+
 class TestAuthenticationService:
 
     @pytest.fixture
     def authentication_service(self):
         return AuthenticationService(CLIENT_ID, CLIENT_SECRET, BASE_URL)
 
     @pytest.fixture
@@ -74,68 +75,73 @@
 
         x = responses.calls[0].request
 
         # assert
         assert excinfo.value.code == INVALID_REQUEST
         assert excinfo.value.message == INVALID_REQUEST_MESSAGE
         assert responses.assert_call_count(endpoint, 1) is True
-        assert responses.calls[0].request.body == f'{{"grant_type": "client_credentials", "client_id": "{CLIENT_ID}", "client_secret": "{CLIENT_SECRET}"}}'.encode()
+        assert responses.calls[0].request.body == f'{{"grant_type": "client_credentials", "client_id": "{CLIENT_ID}", "client_secret": "{CLIENT_SECRET}"}}'.encode(
+        )
 
     def test_refresh_successful(self, authentication_service, endpoint):
         # add a response for the client credentials grant
         responses.add(
             responses.POST,
             endpoint,
             json={
                 'access_token': ACCESS_TOKEN,
                 'refresh_token': REFRESH_TOKEN,
                 'scope': SCOPE,
                 'token_type': TOKEN_TYPE,
                 'expires_in': EXPIRES_IN
             },
-            match=[matchers.json_params_matcher({"grant_type":"client_credentials", "client_id": CLIENT_ID, "client_secret": CLIENT_SECRET})],
+            match=[matchers.json_params_matcher(
+                {"grant_type": "client_credentials", "client_id": CLIENT_ID, "client_secret": CLIENT_SECRET})],
             status=200
         )
 
         # add another response for the refresh token grant
         responses.add(
             responses.POST,
             endpoint,
             json={
                 'access_token': ACCESS_TOKEN2,
                 'refresh_token': REFRESH_TOKEN2,
                 'scope': SCOPE,
                 'token_type': TOKEN_TYPE,
                 'expires_in': EXPIRES_IN
             },
-            match=[matchers.json_params_matcher({"grant_type":"refresh_token", "refresh_token": REFRESH_TOKEN})],
+            match=[matchers.json_params_matcher(
+                {"grant_type": "refresh_token", "refresh_token": REFRESH_TOKEN})],
             status=200
         )
 
         # act
-        auth_data = authentication_service.authenticate() # authenticate first
+        auth_data = authentication_service.authenticate()  # authenticate first
 
         # assert
         assert type(auth_data) == dict
         assert authentication_service._access_token == ACCESS_TOKEN
         assert authentication_service._refresh_token == REFRESH_TOKEN
         assert authentication_service._scope == SCOPE
         assert authentication_service._token_type == TOKEN_TYPE
         assert authentication_service._expires_at != None
-        assert responses.calls[0].request.body == f'{{"grant_type": "client_credentials", "client_id": "{CLIENT_ID}", "client_secret": "{CLIENT_SECRET}"}}'.encode()
+        assert responses.calls[0].request.body == f'{{"grant_type": "client_credentials", "client_id": "{CLIENT_ID}", "client_secret": "{CLIENT_SECRET}"}}'.encode(
+        )
 
-        auth_data2 = authentication_service.refresh() # refresh
+        auth_data2 = authentication_service.refresh()  # refresh
 
         assert type(auth_data2) == dict
         assert authentication_service._access_token == ACCESS_TOKEN2
         assert authentication_service._refresh_token == REFRESH_TOKEN2
         assert authentication_service._scope == SCOPE
         assert authentication_service._token_type == TOKEN_TYPE
         assert authentication_service._expires_at != None
-        assert responses.calls[1].request.body == f'{{"grant_type": "refresh_token", "refresh_token": "{REFRESH_TOKEN}"}}'.encode()
+        assert responses.calls[1].request.body == f'{{"grant_type": "refresh_token", "refresh_token": "{REFRESH_TOKEN}"}}'.encode(
+        )
         assert responses.assert_call_count(endpoint, 2) is True
 
     def test_refresh_failed(self, authentication_service, endpoint):
         # arrange - add responses mock
         # first response for authentication - ok
         responses.add(
             responses.POST,
@@ -143,48 +149,54 @@
             json={
                 'access_token': ACCESS_TOKEN,
                 'refresh_token': REFRESH_TOKEN,
                 'scope': SCOPE,
                 'token_type': TOKEN_TYPE,
                 'expires_in': EXPIRES_IN
             },
-            match=[matchers.json_params_matcher({"grant_type":"client_credentials", "client_id": CLIENT_ID, "client_secret": CLIENT_SECRET})],
+            match=[matchers.json_params_matcher(
+                {"grant_type": "client_credentials", "client_id": CLIENT_ID, "client_secret": CLIENT_SECRET})],
             status=200
         )
 
         # second response for the refresh - failed
         responses.add(
             responses.POST,
             endpoint,
             json={"code": INVALID_REQUEST, "message": INVALID_REQUEST_MESSAGE},
-            match=[matchers.json_params_matcher({"grant_type":"refresh_token", "refresh_token": REFRESH_TOKEN})],
-            status=400
+            match=[matchers.json_params_matcher(
+                {"grant_type": "refresh_token", "refresh_token": REFRESH_TOKEN})],
+            status=500
         )
 
         # act
-        authentication_service.authenticate() # authenticate first
+        authentication_service.authenticate()  # authenticate first
 
         with pytest.raises(APIException) as excinfo:
             authentication_service.refresh()
 
         # assert
         assert excinfo.value.code == INVALID_REQUEST
         assert excinfo.value.message == INVALID_REQUEST_MESSAGE
         assert responses.assert_call_count(endpoint, 2) is True
-        assert responses.calls[0].request.body == f'{{"grant_type": "client_credentials", "client_id": "{CLIENT_ID}", "client_secret": "{CLIENT_SECRET}"}}'.encode()
-        assert responses.calls[1].request.body == f'{{"grant_type": "refresh_token", "refresh_token": "{REFRESH_TOKEN}"}}'.encode()
+        assert responses.calls[0].request.body == f'{{"grant_type": "client_credentials", "client_id": "{CLIENT_ID}", "client_secret": "{CLIENT_SECRET}"}}'.encode(
+        )
+        assert responses.calls[1].request.body == f'{{"grant_type": "refresh_token", "refresh_token": "{REFRESH_TOKEN}"}}'.encode(
+        )
 
     def test_is_expired(self, authentication_service, endpoint):
         # arrange
         current_time = time.time()
         future_time = current_time + 3600
 
         # act
-        authentication_service._expires_at = current_time # set the expired_at as current time
+        # set the expired_at as current time
+        authentication_service._expires_at = current_time
         is_expired_current = authentication_service.is_expired()
 
-        authentication_service._expires_at = future_time # set the expired_at as future time
+        # set the expired_at as future time
+        authentication_service._expires_at = future_time
         is_expired_future = authentication_service.is_expired()
 
         # assert
         assert is_expired_current == True
-        assert is_expired_future == False
+        assert is_expired_future == False
```

### Comparing `datacrunch-1.4.0/tests/unit_tests/balance/test_balance.py` & `datacrunch-1.4.1/tests/unit_tests/balance/test_balance.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/unit_tests/conftest.py` & `datacrunch-1.4.1/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/unit_tests/http_client/test_http_client.py` & `datacrunch-1.4.1/tests/unit_tests/http_client/test_http_client.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/unit_tests/images/test_images.py` & `datacrunch-1.4.1/tests/unit_tests/images/test_images.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/unit_tests/instance_types/test_instance_types.py` & `datacrunch-1.4.1/tests/unit_tests/instance_types/test_instance_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/unit_tests/instances/test_instances.py` & `datacrunch-1.4.1/tests/unit_tests/instances/test_instances.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/unit_tests/ssh_keys/test_ssh_keys.py` & `datacrunch-1.4.1/tests/unit_tests/ssh_keys/test_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/unit_tests/startup_scripts/test_startup_scripts.py` & `datacrunch-1.4.1/tests/unit_tests/startup_scripts/test_startup_scripts.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/unit_tests/test_datacrunch.py` & `datacrunch-1.4.1/tests/unit_tests/test_datacrunch.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/unit_tests/test_exceptions.py` & `datacrunch-1.4.1/tests/unit_tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/unit_tests/volume_types/test_volume_types.py` & `datacrunch-1.4.1/tests/unit_tests/volume_types/test_volume_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.4.0/tests/unit_tests/volumes/test_volumes.py` & `datacrunch-1.4.1/tests/unit_tests/volumes/test_volumes.py`

 * *Files identical despite different names*

