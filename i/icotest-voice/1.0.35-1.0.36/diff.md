# Comparing `tmp/icotest-voice-1.0.35.tar.gz` & `tmp/icotest-voice-1.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icotest-voice-1.0.35.tar", last modified: Fri Jun 16 16:22:10 2023, max compression
+gzip compressed data, was "icotest-voice-1.0.36.tar", last modified: Tue Jun 20 10:09:04 2023, max compression
```

## Comparing `icotest-voice-1.0.35.tar` & `icotest-voice-1.0.36.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.966893 icotest-voice-1.0.35/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2022-09-26 08:19:31.000000 icotest-voice-1.0.35/LICENSE
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       19 2022-09-26 09:44:42.000000 icotest-voice-1.0.35/MANIFEST.in
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8432 2023-06-16 16:22:10.966893 icotest-voice-1.0.35/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     6844 2023-06-16 16:17:58.000000 icotest-voice-1.0.35/README.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.958893 icotest-voice-1.0.35/docs/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      858 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/Controller.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8597 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/ControllersApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1148 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/Device.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    37042 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/DevicesApi.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      497 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/HostConfig.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      376 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/InlineObject.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      326 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/InlineObject1.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      386 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/InlineResponse200.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      423 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/InlineResponse200Files.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      457 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/Message.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      894 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/Request.md
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26941 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/docs/RequestsApi.md
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.958893 icotest-voice-1.0.35/icotest_voice/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1438 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/__init__.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.962893 icotest-voice-1.0.35/icotest_voice/api/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      256 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/api/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    23734 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/api/controllers_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   102070 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/api/devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    82601 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/api/requests_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26193 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/api_client.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9729 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/configuration.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3742 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/exceptions.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.962893 icotest-voice-1.0.35/icotest_voice/models/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      839 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/__init__.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    10518 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/controller.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    14635 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8379 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/host_config.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3617 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/inline_object.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3566 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/inline_object1.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3347 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/inline_response200.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4826 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/inline_response200_files.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5555 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/message.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    13806 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/models/request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12273 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/icotest_voice/rest.py
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.962893 icotest-voice-1.0.35/icotest_voice.egg-info/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8432 2023-06-16 16:22:10.000000 icotest-voice-1.0.35/icotest_voice.egg-info/PKG-INFO
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1428 2023-06-16 16:22:10.000000 icotest-voice-1.0.35/icotest_voice.egg-info/SOURCES.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2023-06-16 16:22:10.000000 icotest-voice-1.0.35/icotest_voice.egg-info/dependency_links.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      125 2023-06-16 16:22:10.000000 icotest-voice-1.0.35/icotest_voice.egg-info/requires.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       14 2023-06-16 16:22:10.000000 icotest-voice-1.0.35/icotest_voice.egg-info/top_level.txt
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      826 2023-06-16 16:14:14.000000 icotest-voice-1.0.35/pyproject.toml
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2023-06-16 16:22:10.966893 icotest-voice-1.0.35/setup.cfg
-drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-16 16:22:10.966893 icotest-voice-1.0.35/test/
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1661 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_controller.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1299 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_controllers_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1830 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_device.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3039 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_devices_api.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1752 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_host_config.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1352 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_inline_object.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1415 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_inline_object1.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1632 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_inline_response200.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1520 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_inline_response200_files.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1452 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_message.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1906 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_request.py
--rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2628 2023-06-16 16:00:27.000000 icotest-voice-1.0.35/test/test_requests_api.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.260591 icotest-voice-1.0.36/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1067 2022-09-26 08:19:31.000000 icotest-voice-1.0.36/LICENSE
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       19 2022-09-26 09:44:42.000000 icotest-voice-1.0.36/MANIFEST.in
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8431 2023-06-20 10:09:04.260591 icotest-voice-1.0.36/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     6843 2023-06-20 10:07:36.000000 icotest-voice-1.0.36/README.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.256591 icotest-voice-1.0.36/docs/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      858 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/Controller.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8597 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/ControllersApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1148 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/Device.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    36998 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/DevicesApi.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      497 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/HostConfig.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      376 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/InlineObject.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      326 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/InlineObject1.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      386 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/InlineResponse200.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      423 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/InlineResponse200Files.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      457 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/Message.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      894 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/Request.md
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26941 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/docs/RequestsApi.md
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.256591 icotest-voice-1.0.36/icotest_voice/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1438 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/__init__.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.256591 icotest-voice-1.0.36/icotest_voice/api/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      256 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/api/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    23734 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/api/controllers_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)   101320 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/api/devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    82601 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/api/requests_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    26193 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/api_client.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     9729 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/configuration.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3742 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/exceptions.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.260591 icotest-voice-1.0.36/icotest_voice/models/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      839 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/__init__.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    10518 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/controller.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    14635 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8379 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3617 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/inline_object.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3566 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/inline_object1.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3347 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/inline_response200.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     4826 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/inline_response200_files.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     5555 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/message.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    13806 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/models/request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)    12273 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/icotest_voice/rest.py
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.256591 icotest-voice-1.0.36/icotest_voice.egg-info/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     8431 2023-06-20 10:09:04.000000 icotest-voice-1.0.36/icotest_voice.egg-info/PKG-INFO
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1428 2023-06-20 10:09:04.000000 icotest-voice-1.0.36/icotest_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)        1 2023-06-20 10:09:04.000000 icotest-voice-1.0.36/icotest_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      125 2023-06-20 10:09:04.000000 icotest-voice-1.0.36/icotest_voice.egg-info/requires.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       14 2023-06-20 10:09:04.000000 icotest-voice-1.0.36/icotest_voice.egg-info/top_level.txt
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)      826 2023-06-20 10:04:27.000000 icotest-voice-1.0.36/pyproject.toml
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)       38 2023-06-20 10:09:04.260591 icotest-voice-1.0.36/setup.cfg
+drwxr-xr-x   0 shipkaliev  (1000) shipkaliev  (1000)        0 2023-06-20 10:09:04.260591 icotest-voice-1.0.36/test/
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1661 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_controller.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1299 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_controllers_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1830 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_device.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     3039 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_devices_api.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1752 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_host_config.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1352 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_inline_object.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1415 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_inline_object1.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1632 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_inline_response200.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1520 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_inline_response200_files.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1452 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_message.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     1906 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_request.py
+-rw-r--r--   0 shipkaliev  (1000) shipkaliev  (1000)     2628 2023-06-20 09:59:48.000000 icotest-voice-1.0.36/test/test_requests_api.py
```

### Comparing `icotest-voice-1.0.35/LICENSE` & `icotest-voice-1.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.35/PKG-INFO` & `icotest-voice-1.0.36/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icotest-voice
-Version: 1.0.35
+Version: 1.0.36
 Summary: Icotest Voice API
 Author-email: Shaun Hirst <shaun.hirst@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
 License: Copyright © 2022 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,16 +20,16 @@
 License-File: LICENSE
 
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.35
-- Package version: 1.0.35
+- API version: 1.0.36
+- Package version: 1.0.36
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -64,15 +64,15 @@
     host = "https://localhost/icotest_voice"
 )
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique id of the controller
+    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c" # str: the unique id of the controller
 
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
```

### Comparing `icotest-voice-1.0.35/README.md` & `icotest-voice-1.0.36/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.35
-- Package version: 1.0.35
+- API version: 1.0.36
+- Package version: 1.0.36
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -43,15 +43,15 @@
     host = "https://localhost/icotest_voice"
 )
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique id of the controller
+    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c" # str: the unique id of the controller
 
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
```

### Comparing `icotest-voice-1.0.35/docs/Controller.md` & `icotest-voice-1.0.36/docs/Controller.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.35/docs/ControllersApi.md` & `icotest-voice-1.0.36/docs/ControllersApi.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.35/docs/Device.md` & `icotest-voice-1.0.36/docs/Device.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.35/docs/DevicesApi.md` & `icotest-voice-1.0.36/docs/DevicesApi.md`

 * *Files 1% similar despite different names*

```diff
@@ -555,19 +555,19 @@
 **403** | Forbidden |  -  |
 **404** | Not Found |  -  |
 **500** | Internal Server Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **post_device_make_call**
-> str post_device_make_call(device_id, call_type, phone_number, call_duration=call_duration, outgoing_recording_file=outgoing_recording_file, playback_file=playback_file, playback_loop=playback_loop, wait_time=wait_time)
+> str post_device_make_call(device_id, phone_number, call_duration=call_duration, outgoing_recording_file=outgoing_recording_file, playback_file=playback_file, playback_loop=playback_loop, wait_time=wait_time)
 
 POST make call
 
-Post request to make an internal or external call
+Post request to make a call
 
 ### Example
 
 ```python
 from __future__ import print_function
 import time
 import icotest_voice
@@ -581,37 +581,35 @@
 
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient() as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.DevicesApi(api_client)
     device_id = 'device_id_example' # str | the unique id of the device
-call_type = 'call_type_example' # str | internal or external call
-phone_number = '1' # str | the number to call
+phone_number = 'i3' # str | the number to call (add \"i\" before the number for a DECT internal call)
 call_duration = 56 # int | the duration of the call in seconds (0 is unlimited) (optional)
 outgoing_recording_file = 'outgoing_call.wav' # str | the filename of the recorded call (optional)
 playback_file = 'audio_playback.wav' # str | the filename of the playback file (optional)
 playback_loop = true # bool | whether to play the playback file in a loop (optional)
 wait_time = 30 # int | the duration of the wait time in seconds for the callee to respond (optional)
 
     try:
         # POST make call
-        api_response = api_instance.post_device_make_call(device_id, call_type, phone_number, call_duration=call_duration, outgoing_recording_file=outgoing_recording_file, playback_file=playback_file, playback_loop=playback_loop, wait_time=wait_time)
+        api_response = api_instance.post_device_make_call(device_id, phone_number, call_duration=call_duration, outgoing_recording_file=outgoing_recording_file, playback_file=playback_file, playback_loop=playback_loop, wait_time=wait_time)
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling DevicesApi->post_device_make_call: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **device_id** | **str**| the unique id of the device | 
- **call_type** | **str**| internal or external call | 
- **phone_number** | **str**| the number to call | 
+ **phone_number** | **str**| the number to call (add \&quot;i\&quot; before the number for a DECT internal call) | 
  **call_duration** | **int**| the duration of the call in seconds (0 is unlimited) | [optional] 
  **outgoing_recording_file** | **str**| the filename of the recorded call | [optional] 
  **playback_file** | **str**| the filename of the playback file | [optional] 
  **playback_loop** | **bool**| whether to play the playback file in a loop | [optional] 
  **wait_time** | **int**| the duration of the wait time in seconds for the callee to respond | [optional] 
 
 ### Return type
```

### Comparing `icotest-voice-1.0.35/docs/Request.md` & `icotest-voice-1.0.36/docs/Request.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.35/docs/RequestsApi.md` & `icotest-voice-1.0.36/docs/RequestsApi.md`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.35/icotest_voice/__init__.py` & `icotest-voice-1.0.36/icotest_voice/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.0.35"
+__version__ = "1.0.36"
 
 # import apis into sdk package
 from icotest_voice.api.controllers_api import ControllersApi
 from icotest_voice.api.devices_api import DevicesApi
 from icotest_voice.api.requests_api import RequestsApi
 
 # import ApiClient
```

### Comparing `icotest-voice-1.0.35/icotest_voice/api/controllers_api.py` & `icotest-voice-1.0.36/icotest_voice/api/controllers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/icotest_voice/api/devices_api.py` & `icotest-voice-1.0.36/icotest_voice/api/devices_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -999,27 +999,26 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def post_device_make_call(self, device_id, call_type, phone_number, **kwargs):  # noqa: E501
+    def post_device_make_call(self, device_id, phone_number, **kwargs):  # noqa: E501
         """POST make call  # noqa: E501
 
-        Post request to make an internal or external call  # noqa: E501
+        Post request to make a call  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.post_device_make_call(device_id, call_type, phone_number, async_req=True)
+        >>> thread = api.post_device_make_call(device_id, phone_number, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str device_id: the unique id of the device (required)
-        :param str call_type: internal or external call (required)
-        :param str phone_number: the number to call (required)
+        :param str phone_number: the number to call (add \"i\" before the number for a DECT internal call) (required)
         :param int call_duration: the duration of the call in seconds (0 is unlimited)
         :param str outgoing_recording_file: the filename of the recorded call
         :param str playback_file: the filename of the playback file
         :param bool playback_loop: whether to play the playback file in a loop
         :param int wait_time: the duration of the wait time in seconds for the callee to respond
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1029,29 +1028,28 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.post_device_make_call_with_http_info(device_id, call_type, phone_number, **kwargs)  # noqa: E501
+        return self.post_device_make_call_with_http_info(device_id, phone_number, **kwargs)  # noqa: E501
 
-    def post_device_make_call_with_http_info(self, device_id, call_type, phone_number, **kwargs):  # noqa: E501
+    def post_device_make_call_with_http_info(self, device_id, phone_number, **kwargs):  # noqa: E501
         """POST make call  # noqa: E501
 
-        Post request to make an internal or external call  # noqa: E501
+        Post request to make a call  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.post_device_make_call_with_http_info(device_id, call_type, phone_number, async_req=True)
+        >>> thread = api.post_device_make_call_with_http_info(device_id, phone_number, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str device_id: the unique id of the device (required)
-        :param str call_type: internal or external call (required)
-        :param str phone_number: the number to call (required)
+        :param str phone_number: the number to call (add \"i\" before the number for a DECT internal call) (required)
         :param int call_duration: the duration of the call in seconds (0 is unlimited)
         :param str outgoing_recording_file: the filename of the recorded call
         :param str playback_file: the filename of the playback file
         :param bool playback_loop: whether to play the playback file in a loop
         :param int wait_time: the duration of the wait time in seconds for the callee to respond
         :param _return_http_data_only: response data without head status code
                                        and headers
@@ -1067,15 +1065,14 @@
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
             'device_id',
-            'call_type',
             'phone_number',
             'call_duration',
             'outgoing_recording_file',
             'playback_file',
             'playback_loop',
             'wait_time'
         ]
@@ -1096,18 +1093,14 @@
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'device_id' is set
         if self.api_client.client_side_validation and ('device_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['device_id'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `device_id` when calling `post_device_make_call`")  # noqa: E501
-        # verify the required parameter 'call_type' is set
-        if self.api_client.client_side_validation and ('call_type' not in local_var_params or  # noqa: E501
-                                                        local_var_params['call_type'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `call_type` when calling `post_device_make_call`")  # noqa: E501
         # verify the required parameter 'phone_number' is set
         if self.api_client.client_side_validation and ('phone_number' not in local_var_params or  # noqa: E501
                                                         local_var_params['phone_number'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `phone_number` when calling `post_device_make_call`")  # noqa: E501
 
         if self.api_client.client_side_validation and ('phone_number' in local_var_params and  # noqa: E501
                                                         len(local_var_params['phone_number']) > 40):  # noqa: E501
@@ -1121,16 +1114,14 @@
         collection_formats = {}
 
         path_params = {}
         if 'device_id' in local_var_params:
             path_params['device_id'] = local_var_params['device_id']  # noqa: E501
 
         query_params = []
-        if 'call_type' in local_var_params and local_var_params['call_type'] is not None:  # noqa: E501
-            query_params.append(('call_type', local_var_params['call_type']))  # noqa: E501
         if 'phone_number' in local_var_params and local_var_params['phone_number'] is not None:  # noqa: E501
             query_params.append(('phone_number', local_var_params['phone_number']))  # noqa: E501
         if 'call_duration' in local_var_params and local_var_params['call_duration'] is not None:  # noqa: E501
             query_params.append(('call_duration', local_var_params['call_duration']))  # noqa: E501
         if 'outgoing_recording_file' in local_var_params and local_var_params['outgoing_recording_file'] is not None:  # noqa: E501
             query_params.append(('outgoing_recording_file', local_var_params['outgoing_recording_file']))  # noqa: E501
         if 'playback_file' in local_var_params and local_var_params['playback_file'] is not None:  # noqa: E501
```

### Comparing `icotest-voice-1.0.35/icotest_voice/api/requests_api.py` & `icotest-voice-1.0.36/icotest_voice/api/requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/icotest_voice/api_client.py` & `icotest-voice-1.0.36/icotest_voice/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.35/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.36/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `icotest-voice-1.0.35/icotest_voice/configuration.py` & `icotest-voice-1.0.36/icotest_voice/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -251,16 +251,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.35\n"\
-               "SDK Package Version: 1.0.35".\
+               "Version of the API: 1.0.36\n"\
+               "SDK Package Version: 1.0.36".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `icotest-voice-1.0.35/icotest_voice/exceptions.py` & `icotest-voice-1.0.36/icotest_voice/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `icotest-voice-1.0.35/icotest_voice/models/__init__.py` & `icotest-voice-1.0.36/icotest_voice/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/icotest_voice/models/controller.py` & `icotest-voice-1.0.36/icotest_voice/models/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.35/icotest_voice/models/device.py` & `icotest-voice-1.0.36/icotest_voice/models/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.35/icotest_voice/models/host_config.py` & `icotest-voice-1.0.36/icotest_voice/models/host_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.35/icotest_voice/models/inline_object.py` & `icotest-voice-1.0.36/icotest_voice/models/inline_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.35/icotest_voice/models/inline_object1.py` & `icotest-voice-1.0.36/icotest_voice/models/inline_object1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.35/icotest_voice/models/inline_response200.py` & `icotest-voice-1.0.36/icotest_voice/models/inline_response200.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.35/icotest_voice/models/inline_response200_files.py` & `icotest-voice-1.0.36/icotest_voice/models/inline_response200_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.35/icotest_voice/models/message.py` & `icotest-voice-1.0.36/icotest_voice/models/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.35/icotest_voice/models/request.py` & `icotest-voice-1.0.36/icotest_voice/models/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `icotest-voice-1.0.35/icotest_voice/rest.py` & `icotest-voice-1.0.36/icotest_voice/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/icotest_voice.egg-info/PKG-INFO` & `icotest-voice-1.0.36/icotest_voice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icotest-voice
-Version: 1.0.35
+Version: 1.0.36
 Summary: Icotest Voice API
 Author-email: Shaun Hirst <shaun.hirst@3adesign.co.uk>, Ivo Shipkaliev <ivo@3adesign.co.uk>
 License: Copyright © 2022 3ADesign Limited
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -20,16 +20,16 @@
 License-File: LICENSE
 
 # icotest-voice
 IcoTest Voice API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.35
-- Package version: 1.0.35
+- API version: 1.0.36
+- Package version: 1.0.36
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -64,15 +64,15 @@
     host = "https://localhost/icotest_voice"
 )
 
 # Enter a context with an instance of the API client
 with icotest_voice.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = icotest_voice.ControllersApi(api_client)
-    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c"  # str: the unique id of the controller
+    controller_id = "ac331ccb-5841-44ec-9d32-4f4fe0c3c16c" # str: the unique id of the controller
 
     try:
         # DELETE Controller
         api_instance.delete_controller(controller_id)
     except ApiException as e:
         print("Exception when calling ControllersApi->delete_controller: %s\n" % e)
```

### Comparing `icotest-voice-1.0.35/icotest_voice.egg-info/SOURCES.txt` & `icotest-voice-1.0.36/icotest_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icotest-voice-1.0.35/pyproject.toml` & `icotest-voice-1.0.36/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icotest-voice"
-version = "1.0.35"
+version = "1.0.36"
 description = "Icotest Voice API"
 readme = "README.md"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Icotest Voice"]
 authors = [
     { name = "Shaun Hirst", email =  "shaun.hirst@3adesign.co.uk" },
     { name = "Ivo Shipkaliev", email = "ivo@3adesign.co.uk" }
 ]
```

### Comparing `icotest-voice-1.0.35/test/test_controller.py` & `icotest-voice-1.0.36/test/test_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/test/test_controllers_api.py` & `icotest-voice-1.0.36/test/test_controllers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/test/test_device.py` & `icotest-voice-1.0.36/test/test_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/test/test_devices_api.py` & `icotest-voice-1.0.36/test/test_devices_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/test/test_host_config.py` & `icotest-voice-1.0.36/test/test_host_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/test/test_inline_object.py` & `icotest-voice-1.0.36/test/test_inline_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/test/test_inline_object1.py` & `icotest-voice-1.0.36/test/test_inline_object1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/test/test_inline_response200.py` & `icotest-voice-1.0.36/test/test_inline_response200.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/test/test_inline_response200_files.py` & `icotest-voice-1.0.36/test/test_inline_response200_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/test/test_message.py` & `icotest-voice-1.0.36/test/test_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/test/test_request.py` & `icotest-voice-1.0.36/test/test_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `icotest-voice-1.0.35/test/test_requests_api.py` & `icotest-voice-1.0.36/test/test_requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     IcoTest Voice
 
     IcoTest Voice API  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.35
+    The version of the OpenAPI document: 1.0.36
     Contact: shaun.hirst@3adesign.co.uk
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

