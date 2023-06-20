# Comparing `tmp/nobuco-0.5.3.tar.gz` & `tmp/nobuco-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.5.3.tar", last modified: Mon Jun 19 21:45:24 2023, max compression
+gzip compressed data, was "nobuco-0.5.4.tar", last modified: Tue Jun 20 17:25:59 2023, max compression
```

## Comparing `nobuco-0.5.3.tar` & `nobuco-0.5.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.893394 nobuco-0.5.3/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.3/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    22244 2023-06-19 21:45:24.893394 nobuco-0.5.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    20410 2023-06-19 11:19:36.000000 nobuco-0.5.3/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.885394 nobuco-0.5.3/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13970 2023-06-19 19:46:46.000000 nobuco-0.5.3/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.885394 nobuco-0.5.3/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.5.3/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.5.3/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4095 2023-06-19 20:43:10.000000 nobuco-0.5.3/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.885394 nobuco-0.5.3/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.5.3/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.885394 nobuco-0.5.3/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.3/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.3/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.889394 nobuco-0.5.3/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.893394 nobuco-0.5.3/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-15 13:23:44.000000 nobuco-0.5.3/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-06-19 11:09:59.000000 nobuco-0.5.3/nobuco/node_converters/attention.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-06-19 13:20:31.000000 nobuco-0.5.3/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-16 16:26:28.000000 nobuco-0.5.3/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.5.3/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.5.3/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1533 2023-06-06 20:30:38.000000 nobuco-0.5.3/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-06-19 13:27:23.000000 nobuco-0.5.3/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13838 2023-06-06 20:13:59.000000 nobuco-0.5.3/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.5.3/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1662 2023-06-19 20:57:04.000000 nobuco-0.5.3/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-07 02:32:02.000000 nobuco-0.5.3/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-06-19 21:15:29.000000 nobuco-0.5.3/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-06-19 13:43:03.000000 nobuco-0.5.3/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.5.3/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6244 2023-06-19 13:24:40.000000 nobuco-0.5.3/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11297 2023-06-19 20:07:28.000000 nobuco-0.5.3/nobuco/node_converters/tensor_manipulation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-06 21:33:32.000000 nobuco-0.5.3/nobuco/node_converters/tensor_shape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-06-19 20:13:01.000000 nobuco-0.5.3/nobuco/node_converters/torchvision.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.893394 nobuco-0.5.3/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-06 19:21:15.000000 nobuco-0.5.3/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-09 15:11:00.000000 nobuco-0.5.3/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.893394 nobuco-0.5.3/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.3/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 21:45:24.885394 nobuco-0.5.3/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    22244 2023-06-19 21:45:24.000000 nobuco-0.5.3/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-06-19 21:45:24.000000 nobuco-0.5.3/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-19 21:45:24.000000 nobuco-0.5.3/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-19 21:45:24.000000 nobuco-0.5.3/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-19 21:45:24.000000 nobuco-0.5.3/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-19 21:44:16.000000 nobuco-0.5.3/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-19 21:45:24.893394 nobuco-0.5.3/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.123032 nobuco-0.5.4/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.5.4/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24637 2023-06-20 17:25:59.123032 nobuco-0.5.4/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22803 2023-06-20 17:23:27.000000 nobuco-0.5.4/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.115032 nobuco-0.5.4/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13970 2023-06-19 19:46:46.000000 nobuco-0.5.4/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.115032 nobuco-0.5.4/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.5.4/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-19 20:03:57.000000 nobuco-0.5.4/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4095 2023-06-19 20:43:10.000000 nobuco-0.5.4/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.115032 nobuco-0.5.4/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.5.4/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.115032 nobuco-0.5.4/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4419 2023-06-17 09:52:53.000000 nobuco-0.5.4/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.5.4/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.115032 nobuco-0.5.4/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.119032 nobuco-0.5.4/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6967 2023-06-15 13:23:44.000000 nobuco-0.5.4/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2225 2023-06-19 11:09:59.000000 nobuco-0.5.4/nobuco/node_converters/attention.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-06-19 13:20:31.000000 nobuco-0.5.4/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1165 2023-06-16 16:26:28.000000 nobuco-0.5.4/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.5.4/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.5.4/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1790 2023-06-20 11:58:19.000000 nobuco-0.5.4/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5152 2023-06-19 13:27:23.000000 nobuco-0.5.4/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14354 2023-06-20 11:35:42.000000 nobuco-0.5.4/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.5.4/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2213 2023-06-20 12:20:54.000000 nobuco-0.5.4/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-07 02:32:02.000000 nobuco-0.5.4/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2934 2023-06-19 21:15:29.000000 nobuco-0.5.4/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9538 2023-06-19 13:43:03.000000 nobuco-0.5.4/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.5.4/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6449 2023-06-20 11:32:28.000000 nobuco-0.5.4/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11315 2023-06-20 11:52:34.000000 nobuco-0.5.4/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-06 21:33:32.000000 nobuco-0.5.4/nobuco/node_converters/tensor_shape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      452 2023-06-19 20:13:01.000000 nobuco-0.5.4/nobuco/node_converters/torchvision.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.123032 nobuco-0.5.4/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-06 19:21:15.000000 nobuco-0.5.4/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-09 15:11:00.000000 nobuco-0.5.4/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.123032 nobuco-0.5.4/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.5.4/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-20 17:25:59.115032 nobuco-0.5.4/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    24637 2023-06-20 17:25:59.000000 nobuco-0.5.4/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1702 2023-06-20 17:25:59.000000 nobuco-0.5.4/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-20 17:25:59.000000 nobuco-0.5.4/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-20 17:25:59.000000 nobuco-0.5.4/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-20 17:25:59.000000 nobuco-0.5.4/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-20 17:20:57.000000 nobuco-0.5.4/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-20 17:25:59.123032 nobuco-0.5.4/setup.cfg
```

### Comparing `nobuco-0.5.3/LICENSE` & `nobuco-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/PKG-INFO` & `nobuco-0.5.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1
-Name: nobuco
-Version: 0.5.3
-Summary: Pytorch to Tensorflow conversion made somewhat easy
-Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Alexander Lutsenko
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
-Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
-Keywords: pytorch,tensorflow,keras,converter
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
 <img src="docs/nobuco.png">
 <sup><a href="https://www.behance.net/diliajl">diliajl</a></sup>
 </p>
 
 **No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
@@ -63,14 +27,15 @@
 - [Essentials](#essentials)
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
   - [Control flows](#control-flows)
   - [Dynamic shapes](#dynamic-shapes)
 - [So we put a converter inside your converter](#so-we-put-a-converter-inside-your-converter)
+- [But was it worth it?](#but-was-it-worth-it)
 - [More nice things](#more-nice-things)
   - [Nobuco knowledge base](#nobuco-knowledge-base)
 
 <!-- tocstop -->
 
 ## Essentials
 
@@ -534,14 +499,93 @@
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x: model(input=x))
 ```
 
 <img src="docs/converter_inside_converter2.svg" width="100%">
 
+## But was it worth it?
+
+Let's cut to the chase, here's the numbers.
+
+**mobilenet_v3_large** (26.8 Mb)
+
+|                   | nobuco  | onnx_tf  | speedup |
+|-------------------|---------|----------|---------|
+| x86 (XNNPACK)     | 11.1 ms | 14.7 ms  | 1.3x    |
+| Arm CPU (XNNPACK) | 24.3 ms | 40.3 ms  | 1.6x    |
+| Arm GPU (OpenCL)  | 21.3 ms | 192.6 ms | 9x      |
+
+**deeplabv3_resnet50** (158.5 Mb)
+
+|                   | nobuco | onnx_tf | speedup |
+|-------------------|--------|---------|---------|
+| x86 (XNNPACK)     | 1.25 s | 1.34 s  | 1.07x   |
+| Arm CPU (XNNPACK) | 2.0 s  | 2.7 s   | 1.35x   |
+| Arm GPU (OpenCL)  | 1.6 s  | 2.6 s   | 1.62x   |
+
+As we can see, redundant transpositions may completely ruin the performance, especially on a GPU.
+But that's not the only issue.
+Let's test this:
+
+```python
+class SliceReLU(nn.Module):
+    def forward(self, x):
+        x[:, 1:2, 16:25, 8::2] = torch.relu_(x[:, 1:2, 16:25, 8::2])
+        return x
+```
+
+|                   | nobuco     | onnx_tf    | speedup |
+|-------------------|------------|------------|---------|
+| x86 (XNNPACK)     | 0.40 ms    | 1.57 ms    | 3.9x    |
+| Arm CPU           | 4.6 ms     | **2.9** ms | 0.6x    |
+| Arm CPU (XNNPACK) | **2.1** ms | FAIL       | —       |
+| Arm GPU (OpenCL)  | 21.8 ms    | FAIL       | —       |
+
+Again, the graph obtained with `onnx_tf` is much slower on x86 CPU.
+Worse yet, on mobile processor, optimized TFLite delegates for both GPU and CPU failed.
+No transpose ops were added this time, so who's to blame?
+It suffices to see what `torch.trace` gives us:
+
+<table>
+<tr>
+<th>slice_relu.onnx</th>
+</tr>
+<tr>
+<td>
+<img src="docs/slice_relu_onnx.png" width="100%">
+</td>
+</tr>
+</table>
+
+`onnx_tf` does a fair job optimizing the graph it's given,
+but combining consecutive `slice` ops seems to be too much to ask.
+It also leaves out garbage nodes sometimes (see free-floating `While` in this example).
+
+Nobuco evades these types of problems by simply not dealing with `onnx`.
+
+<table>
+  <tr>
+    <th>slice_relu_nobuco.tflite</th>
+    <th>slice_relu_onnxtf.tflite</th>
+  </tr>
+  <tr>
+    <td>
+      <p align="center">
+        <img src="docs/slice_relu_nobuco.png" width="60%">
+      </p>
+    </td>
+    <td>
+      <p align="center">
+        <img src="docs/slice_relu_onnxtf.png" width="60%">
+      </p>
+    </td>
+  </tr>
+</table>
+
 ## More nice things
 
 ### Nobuco knowledge base
 
 Don't want to convert anything but looking for a tensorflow equivalent of a certain pytorch node (operation or module)?
 Nobuco already implements quite a few node converters, most written in concise and (hopefully) understandable way.
 These are located in [nobuco/node_converters](https://github.com/AlexanderLutsenko/nobuco/tree/master/nobuco/node_converters),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nobuco-0.5.3/README.md` & `nobuco-0.5.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+Metadata-Version: 2.1
+Name: nobuco
+Version: 0.5.4
+Summary: Pytorch to Tensorflow conversion made somewhat easy
+Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Alexander Lutsenko
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
+Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
+Keywords: pytorch,tensorflow,keras,converter
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
 <img src="docs/nobuco.png">
 <sup><a href="https://www.behance.net/diliajl">diliajl</a></sup>
 </p>
 
 **No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
@@ -27,14 +63,15 @@
 - [Essentials](#essentials)
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
   - [Control flows](#control-flows)
   - [Dynamic shapes](#dynamic-shapes)
 - [So we put a converter inside your converter](#so-we-put-a-converter-inside-your-converter)
+- [But was it worth it?](#but-was-it-worth-it)
 - [More nice things](#more-nice-things)
   - [Nobuco knowledge base](#nobuco-knowledge-base)
 
 <!-- tocstop -->
 
 ## Essentials
 
@@ -498,14 +535,93 @@
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x: model(input=x))
 ```
 
 <img src="docs/converter_inside_converter2.svg" width="100%">
 
+## But was it worth it?
+
+Let's cut to the chase, here's the numbers.
+
+**mobilenet_v3_large** (26.8 Mb)
+
+|                   | nobuco  | onnx_tf  | speedup |
+|-------------------|---------|----------|---------|
+| x86 (XNNPACK)     | 11.1 ms | 14.7 ms  | 1.3x    |
+| Arm CPU (XNNPACK) | 24.3 ms | 40.3 ms  | 1.6x    |
+| Arm GPU (OpenCL)  | 21.3 ms | 192.6 ms | 9x      |
+
+**deeplabv3_resnet50** (158.5 Mb)
+
+|                   | nobuco | onnx_tf | speedup |
+|-------------------|--------|---------|---------|
+| x86 (XNNPACK)     | 1.25 s | 1.34 s  | 1.07x   |
+| Arm CPU (XNNPACK) | 2.0 s  | 2.7 s   | 1.35x   |
+| Arm GPU (OpenCL)  | 1.6 s  | 2.6 s   | 1.62x   |
+
+As we can see, redundant transpositions may completely ruin the performance, especially on a GPU.
+But that's not the only issue.
+Let's test this:
+
+```python
+class SliceReLU(nn.Module):
+    def forward(self, x):
+        x[:, 1:2, 16:25, 8::2] = torch.relu_(x[:, 1:2, 16:25, 8::2])
+        return x
+```
+
+|                   | nobuco     | onnx_tf    | speedup |
+|-------------------|------------|------------|---------|
+| x86 (XNNPACK)     | 0.40 ms    | 1.57 ms    | 3.9x    |
+| Arm CPU           | 4.6 ms     | **2.9** ms | 0.6x    |
+| Arm CPU (XNNPACK) | **2.1** ms | FAIL       | —       |
+| Arm GPU (OpenCL)  | 21.8 ms    | FAIL       | —       |
+
+Again, the graph obtained with `onnx_tf` is much slower on x86 CPU.
+Worse yet, on mobile processor, optimized TFLite delegates for both GPU and CPU failed.
+No transpose ops were added this time, so who's to blame?
+It suffices to see what `torch.trace` gives us:
+
+<table>
+<tr>
+<th>slice_relu.onnx</th>
+</tr>
+<tr>
+<td>
+<img src="docs/slice_relu_onnx.png" width="100%">
+</td>
+</tr>
+</table>
+
+`onnx_tf` does a fair job optimizing the graph it's given,
+but combining consecutive `slice` ops seems to be too much to ask.
+It also leaves out garbage nodes sometimes (see free-floating `While` in this example).
+
+Nobuco evades these types of problems by simply not dealing with `onnx`.
+
+<table>
+  <tr>
+    <th>slice_relu_nobuco.tflite</th>
+    <th>slice_relu_onnxtf.tflite</th>
+  </tr>
+  <tr>
+    <td>
+      <p align="center">
+        <img src="docs/slice_relu_nobuco.png" width="60%">
+      </p>
+    </td>
+    <td>
+      <p align="center">
+        <img src="docs/slice_relu_onnxtf.png" width="60%">
+      </p>
+    </td>
+  </tr>
+</table>
+
 ## More nice things
 
 ### Nobuco knowledge base
 
 Don't want to convert anything but looking for a tensorflow equivalent of a certain pytorch node (operation or module)?
 Nobuco already implements quite a few node converters, most written in concise and (hopefully) understandable way.
 These are located in [nobuco/node_converters](https://github.com/AlexanderLutsenko/nobuco/tree/master/nobuco/node_converters),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nobuco-0.5.3/nobuco/__init__.py` & `nobuco-0.5.4/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/commons.py` & `nobuco-0.5.4/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/convert.py` & `nobuco-0.5.4/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/converters/channel_ordering.py` & `nobuco-0.5.4/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/converters/node_converter.py` & `nobuco-0.5.4/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/converters/tensor.py` & `nobuco-0.5.4/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/converters/type_cast.py` & `nobuco-0.5.4/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/converters/validation.py` & `nobuco-0.5.4/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/entity/keras.py` & `nobuco-0.5.4/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/entity/pytorch.py` & `nobuco-0.5.4/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/funcs.py` & `nobuco-0.5.4/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/layers/channel_order.py` & `nobuco-0.5.4/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/layers/container.py` & `nobuco-0.5.4/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/layers/weight.py` & `nobuco-0.5.4/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/locate/link.py` & `nobuco-0.5.4/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/locate/locate.py` & `nobuco-0.5.4/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/activation.py` & `nobuco-0.5.4/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/attention.py` & `nobuco-0.5.4/nobuco/node_converters/attention.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/boolean.py` & `nobuco-0.5.4/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/boolean_mask.py` & `nobuco-0.5.4/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/comparison.py` & `nobuco-0.5.4/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/convolution.py` & `nobuco-0.5.4/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/dropout.py` & `nobuco-0.5.4/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/interpolation.py` & `nobuco-0.5.4/nobuco/node_converters/interpolation.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,27 +11,33 @@
 from nobuco.commons import TF_TENSOR_CLASSES
 from nobuco.converters.node_converter import converter
 
 
 @converter(F.interpolate)
 def converter_interpolate(input: Tensor, size: Optional[int] = None, scale_factor: Optional[List[float]] = None, mode: str = 'nearest',
                 align_corners: Optional[bool] = None, recompute_scale_factor: Optional[bool] = None, antialias: bool = False):
+
     if mode == 'bilinear':
         method = ResizeMethod.BILINEAR
     elif mode == 'nearest':
         method = ResizeMethod.NEAREST_NEIGHBOR
     else:
         raise Exception('Unsupported mode: ', mode)
 
     def func(input, size=None, scale_factor=None, mode='nearest', align_corners=None, recompute_scale_factor=None, antialias=False):
+        assert not (align_corners and antialias), "'align_corners' and 'antialias' cannot both be True"
+
         if isinstance(scale_factor, numbers.Number) or (isinstance(scale_factor, TF_TENSOR_CLASSES) and tf.size(scale_factor) == 1):
             scale_factor = (scale_factor, scale_factor)
 
         if isinstance(size, numbers.Number) or (isinstance(size, TF_TENSOR_CLASSES) and tf.size(size) == 1):
             size = (size, size)
 
         if size is None:
             _, h, w, _ = input.shape
             size = (int(h * scale_factor[0]), int(w * scale_factor[1]))
 
-        return tf.image.resize(input, size=size, method=method, antialias=antialias)
+        if align_corners:
+            return tf.compat.v1.image.resize(input, size=size, method=method, align_corners=align_corners)
+        else:
+            return tf.image.resize(input, size=size, method=method, antialias=antialias)
     return func
```

### Comparing `nobuco-0.5.3/nobuco/node_converters/linear.py` & `nobuco-0.5.4/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/math.py` & `nobuco-0.5.4/nobuco/node_converters/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,28 @@
 @converter(torch.clamp, torch.Tensor.clamp, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_clamp(input: Tensor, min: Optional[Number]=None, max: Optional[Number]=None, *, out: Optional[Tensor]=None):
     def func(input, min=None, max=None, *, out=None):
         return tf.keras.backend.clip(input, min_value=min, max_value=max)
     return func
 
 
+@converter(torch.Tensor.clamp_min, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_clamp(self, min):
+    def func(self, min):
+        return tf.keras.backend.clip(self, min_value=min, max_value=None)
+    return func
+
+
+@converter(torch.Tensor.clamp_max, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_clamp(self, max):
+    def func(self, max):
+        return tf.keras.backend.clip(self, min_value=None, max_value=max)
+    return func
+
+
 @converter(torch.minimum, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_minimum(input: Tensor, other: Tensor, *, out: Optional[Tensor]=None):
     def func(input, other, *, out=None):
         return tf.minimum(input, other)
     return func
```

### Comparing `nobuco-0.5.3/nobuco/node_converters/misc.py` & `nobuco-0.5.4/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/normalization.py` & `nobuco-0.5.4/nobuco/node_converters/normalization.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,35 @@
     return layer
 
     # def func(input, *args, **kwargs):
     #     return (input - running_mean) / (tf.sqrt(running_var + epsilon)) * weight + bias
     # return func
 
 
+@converter(nn.InstanceNorm1d, nn.InstanceNorm2d)
+def converter_InstanceNorm(self, input: Tensor):
+    params = []
+
+    scale = False
+    if self.weight is not None:
+        scale = True
+        params.append(self.weight.detach.numpy())
+
+    center = False
+    if self.bias is not None:
+        center = True
+        params.append(self.bias.detach.numpy())
+
+    epsilon = self.eps
+
+    import tensorflow_addons as tfa
+    layer = tfa.layers.InstanceNormalization(axis=-1, epsilon=epsilon, scale=scale, center=center, weights=params)
+    return layer
+
+
 @converter(F.layer_norm, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_layer_norm(input: Tensor,
                normalized_shape: List[int],
                weight: Optional[Tensor] = None,
                bias: Optional[Tensor] = None,
                eps: float = 1e-5
                ):
```

### Comparing `nobuco-0.5.3/nobuco/node_converters/padding.py` & `nobuco-0.5.4/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/pooling.py` & `nobuco-0.5.4/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/recurrent.py` & `nobuco-0.5.4/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/slice.py` & `nobuco-0.5.4/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/tensor_cast.py` & `nobuco-0.5.4/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/node_converters/tensor_creation.py` & `nobuco-0.5.4/nobuco/node_converters/tensor_creation.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,21 @@
         if dtype is None:
             return tf.zeros(shape=size)
         else:
             return tf.zeros(shape=size, dtype=tf_type)
     return func
 
 
+@converter(torch.Tensor.zero_, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_zero_(self):
+    def func(self):
+        return tf.zeros_like(self)
+    return func
+
+
 @converter(torch.zeros_like, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_zeros_like(input: Tensor, *, memory_format=None, dtype=None, layout=None, device=None, pin_memory=False, requires_grad=False):
     def func(input: Tensor, *, memory_format=None, dtype=None, layout=None, device=None, pin_memory=False, requires_grad=False):
         tf_type = dtype_pytorch2keras(dtype)
         return tf.zeros_like(input, dtype=tf_type)
     return func
```

### Comparing `nobuco-0.5.3/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.5.4/nobuco/node_converters/tensor_manipulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,22 +134,22 @@
     def func(self, split_size, dim=0):
         if get_channel_order(self) == ChannelOrder.TENSORFLOW:
             dim = dim_pytorch2keras(dim, num_dims)
         return tf.split(self, num_or_size_splits=split_size, axis=dim)
     return func
 
 
-@converter(torch.Tensor.chunk, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
-def converter_chunk(self, chunks, dim=0):
-    num_dims = self.dim()
+@converter(torch.chunk, torch.Tensor.chunk, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+def converter_chunk(input, chunks, dim=0):
+    num_dims = input.dim()
 
-    def func(self, chunks, dim=0):
-        if get_channel_order(self) == ChannelOrder.TENSORFLOW:
+    def func(input, chunks, dim=0):
+        if get_channel_order(input) == ChannelOrder.TENSORFLOW:
             dim = dim_pytorch2keras(dim, num_dims)
-        return tf.split(self, num_or_size_splits=chunks, axis=dim)
+        return tf.split(input, num_or_size_splits=chunks, axis=dim)
     return func
 
 
 @converter(torch.Tensor.repeat, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_repeat(self, *sizes):
     def func(self, *sizes):
         if get_channel_order(self) == ChannelOrder.TENSORFLOW:
```

### Comparing `nobuco-0.5.3/nobuco/trace/tensor_storage.py` & `nobuco-0.5.4/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/trace/trace.py` & `nobuco-0.5.4/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/util.py` & `nobuco-0.5.4/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/vis/console_stylizer.py` & `nobuco-0.5.4/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco/vis/html_stylizer.py` & `nobuco-0.5.4/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/nobuco.egg-info/PKG-INFO` & `nobuco-0.5.4/nobuco.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.5.3
+Version: 0.5.4
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,14 +63,15 @@
 - [Essentials](#essentials)
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
   - [Control flows](#control-flows)
   - [Dynamic shapes](#dynamic-shapes)
 - [So we put a converter inside your converter](#so-we-put-a-converter-inside-your-converter)
+- [But was it worth it?](#but-was-it-worth-it)
 - [More nice things](#more-nice-things)
   - [Nobuco knowledge base](#nobuco-knowledge-base)
 
 <!-- tocstop -->
 
 ## Essentials
 
@@ -534,14 +535,93 @@
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x: model(input=x))
 ```
 
 <img src="docs/converter_inside_converter2.svg" width="100%">
 
+## But was it worth it?
+
+Let's cut to the chase, here's the numbers.
+
+**mobilenet_v3_large** (26.8 Mb)
+
+|                   | nobuco  | onnx_tf  | speedup |
+|-------------------|---------|----------|---------|
+| x86 (XNNPACK)     | 11.1 ms | 14.7 ms  | 1.3x    |
+| Arm CPU (XNNPACK) | 24.3 ms | 40.3 ms  | 1.6x    |
+| Arm GPU (OpenCL)  | 21.3 ms | 192.6 ms | 9x      |
+
+**deeplabv3_resnet50** (158.5 Mb)
+
+|                   | nobuco | onnx_tf | speedup |
+|-------------------|--------|---------|---------|
+| x86 (XNNPACK)     | 1.25 s | 1.34 s  | 1.07x   |
+| Arm CPU (XNNPACK) | 2.0 s  | 2.7 s   | 1.35x   |
+| Arm GPU (OpenCL)  | 1.6 s  | 2.6 s   | 1.62x   |
+
+As we can see, redundant transpositions may completely ruin the performance, especially on a GPU.
+But that's not the only issue.
+Let's test this:
+
+```python
+class SliceReLU(nn.Module):
+    def forward(self, x):
+        x[:, 1:2, 16:25, 8::2] = torch.relu_(x[:, 1:2, 16:25, 8::2])
+        return x
+```
+
+|                   | nobuco     | onnx_tf    | speedup |
+|-------------------|------------|------------|---------|
+| x86 (XNNPACK)     | 0.40 ms    | 1.57 ms    | 3.9x    |
+| Arm CPU           | 4.6 ms     | **2.9** ms | 0.6x    |
+| Arm CPU (XNNPACK) | **2.1** ms | FAIL       | —       |
+| Arm GPU (OpenCL)  | 21.8 ms    | FAIL       | —       |
+
+Again, the graph obtained with `onnx_tf` is much slower on x86 CPU.
+Worse yet, on mobile processor, optimized TFLite delegates for both GPU and CPU failed.
+No transpose ops were added this time, so who's to blame?
+It suffices to see what `torch.trace` gives us:
+
+<table>
+<tr>
+<th>slice_relu.onnx</th>
+</tr>
+<tr>
+<td>
+<img src="docs/slice_relu_onnx.png" width="100%">
+</td>
+</tr>
+</table>
+
+`onnx_tf` does a fair job optimizing the graph it's given,
+but combining consecutive `slice` ops seems to be too much to ask.
+It also leaves out garbage nodes sometimes (see free-floating `While` in this example).
+
+Nobuco evades these types of problems by simply not dealing with `onnx`.
+
+<table>
+  <tr>
+    <th>slice_relu_nobuco.tflite</th>
+    <th>slice_relu_onnxtf.tflite</th>
+  </tr>
+  <tr>
+    <td>
+      <p align="center">
+        <img src="docs/slice_relu_nobuco.png" width="60%">
+      </p>
+    </td>
+    <td>
+      <p align="center">
+        <img src="docs/slice_relu_onnxtf.png" width="60%">
+      </p>
+    </td>
+  </tr>
+</table>
+
 ## More nice things
 
 ### Nobuco knowledge base
 
 Don't want to convert anything but looking for a tensorflow equivalent of a certain pytorch node (operation or module)?
 Nobuco already implements quite a few node converters, most written in concise and (hopefully) understandable way.
 These are located in [nobuco/node_converters](https://github.com/AlexanderLutsenko/nobuco/tree/master/nobuco/node_converters),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nobuco-0.5.3/nobuco.egg-info/SOURCES.txt` & `nobuco-0.5.4/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.5.3/pyproject.toml` & `nobuco-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.5.3"
+version = "0.5.4"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

