# Comparing `tmp/weconnect-mqtt-0.9.0.dev5.tar.gz` & `tmp/weconnect-mqtt-0.9.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weconnect-mqtt-0.9.0.dev5.tar", last modified: Thu Jun 24 20:38:42 2021, max compression
+gzip compressed data, was "weconnect-mqtt-0.9.0.dev6.tar", last modified: Fri Jun 25 09:48:46 2021, max compression
```

## Comparing `weconnect-mqtt-0.9.0.dev5.tar` & `weconnect-mqtt-0.9.0.dev6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 20:38:42.898617 weconnect-mqtt-0.9.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-06-24 20:38:23.000000 weconnect-mqtt-0.9.0.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5660 2021-06-24 20:38:42.902617 weconnect-mqtt-0.9.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4150 2021-06-24 20:38:23.000000 weconnect-mqtt-0.9.0.dev5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2938 2021-06-24 20:38:42.902617 weconnect-mqtt-0.9.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2021-06-24 20:38:23.000000 weconnect-mqtt-0.9.0.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 20:38:42.898617 weconnect-mqtt-0.9.0.dev5/weconnect_mqtt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-24 20:38:23.000000 weconnect-mqtt-0.9.0.dev5/weconnect_mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-06-24 20:38:23.000000 weconnect-mqtt-0.9.0.dev5/weconnect_mqtt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-06-24 20:38:23.000000 weconnect-mqtt-0.9.0.dev5/weconnect_mqtt/__version.py
--rw-r--r--   0 runner    (1001) docker     (121)    20880 2021-06-24 20:38:23.000000 weconnect-mqtt-0.9.0.dev5/weconnect_mqtt/weconnect_mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 20:38:42.898617 weconnect-mqtt-0.9.0.dev5/weconnect_mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5660 2021-06-24 20:38:42.000000 weconnect-mqtt-0.9.0.dev5/weconnect_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      381 2021-06-24 20:38:42.000000 weconnect-mqtt-0.9.0.dev5/weconnect_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 20:38:42.000000 weconnect-mqtt-0.9.0.dev5/weconnect_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-06-24 20:38:42.000000 weconnect-mqtt-0.9.0.dev5/weconnect_mqtt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-06-24 20:38:42.000000 weconnect-mqtt-0.9.0.dev5/weconnect_mqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-06-24 20:38:42.000000 weconnect-mqtt-0.9.0.dev5/weconnect_mqtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 09:48:46.663283 weconnect-mqtt-0.9.0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-06-25 09:48:26.000000 weconnect-mqtt-0.9.0.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     5660 2021-06-25 09:48:46.663283 weconnect-mqtt-0.9.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4150 2021-06-25 09:48:26.000000 weconnect-mqtt-0.9.0.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2938 2021-06-25 09:48:46.663283 weconnect-mqtt-0.9.0.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2021-06-25 09:48:26.000000 weconnect-mqtt-0.9.0.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 09:48:46.659283 weconnect-mqtt-0.9.0.dev6/weconnect_mqtt/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-25 09:48:26.000000 weconnect-mqtt-0.9.0.dev6/weconnect_mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-06-25 09:48:26.000000 weconnect-mqtt-0.9.0.dev6/weconnect_mqtt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-06-25 09:48:26.000000 weconnect-mqtt-0.9.0.dev6/weconnect_mqtt/__version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20880 2021-06-25 09:48:26.000000 weconnect-mqtt-0.9.0.dev6/weconnect_mqtt/weconnect_mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-25 09:48:46.663283 weconnect-mqtt-0.9.0.dev6/weconnect_mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5660 2021-06-25 09:48:46.000000 weconnect-mqtt-0.9.0.dev6/weconnect_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2021-06-25 09:48:46.000000 weconnect-mqtt-0.9.0.dev6/weconnect_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-25 09:48:46.000000 weconnect-mqtt-0.9.0.dev6/weconnect_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2021-06-25 09:48:46.000000 weconnect-mqtt-0.9.0.dev6/weconnect_mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2021-06-25 09:48:46.000000 weconnect-mqtt-0.9.0.dev6/weconnect_mqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-06-25 09:48:46.000000 weconnect-mqtt-0.9.0.dev6/weconnect_mqtt.egg-info/top_level.txt
```

### Comparing `weconnect-mqtt-0.9.0.dev5/LICENSE` & `weconnect-mqtt-0.9.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `weconnect-mqtt-0.9.0.dev5/PKG-INFO` & `weconnect-mqtt-0.9.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weconnect-mqtt
-Version: 0.9.0.dev5
+Version: 0.9.0.dev6
 Summary: CMQTT Client that publishes data from Volkswagen WeConnect
 Home-page: https://github.com/tillsteinbach/WeConnect-mqtt
 Author: Till Steinbach
 License: MIT
 Description: # WeConnect-MQTT
         [![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/tillsteinbach/WeConnect-mqtt/)
         [![GitHub release (latest by date)](https://img.shields.io/github/v/release/tillsteinbach/WeConnect-mqtt)](https://github.com/tillsteinbach/WeConnect-mqtt/releases/latest)
```

### Comparing `weconnect-mqtt-0.9.0.dev5/README.md` & `weconnect-mqtt-0.9.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `weconnect-mqtt-0.9.0.dev5/setup.cfg` & `weconnect-mqtt-0.9.0.dev6/setup.cfg`

 * *Files identical despite different names*

### Comparing `weconnect-mqtt-0.9.0.dev5/setup.py` & `weconnect-mqtt-0.9.0.dev6/setup.py`

 * *Files identical despite different names*

### Comparing `weconnect-mqtt-0.9.0.dev5/weconnect_mqtt/weconnect_mqtt.py` & `weconnect-mqtt-0.9.0.dev6/weconnect_mqtt/weconnect_mqtt.py`

 * *Files identical despite different names*

### Comparing `weconnect-mqtt-0.9.0.dev5/weconnect_mqtt.egg-info/PKG-INFO` & `weconnect-mqtt-0.9.0.dev6/weconnect_mqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weconnect-mqtt
-Version: 0.9.0.dev5
+Version: 0.9.0.dev6
 Summary: CMQTT Client that publishes data from Volkswagen WeConnect
 Home-page: https://github.com/tillsteinbach/WeConnect-mqtt
 Author: Till Steinbach
 License: MIT
 Description: # WeConnect-MQTT
         [![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/tillsteinbach/WeConnect-mqtt/)
         [![GitHub release (latest by date)](https://img.shields.io/github/v/release/tillsteinbach/WeConnect-mqtt)](https://github.com/tillsteinbach/WeConnect-mqtt/releases/latest)
```

