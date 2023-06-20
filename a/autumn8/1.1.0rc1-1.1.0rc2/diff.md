# Comparing `tmp/autumn8-1.1.0rc1.tar.gz` & `tmp/autumn8-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.1.0rc1.tar", last modified: Mon Jun 19 13:20:56 2023, max compression
+gzip compressed data, was "autumn8-1.1.0rc2.tar", last modified: Tue Jun 20 13:13:25 2023, max compression
```

## Comparing `autumn8-1.1.0rc1.tar` & `autumn8-1.1.0rc2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     8030 2023-06-19 12:42:47.000000 autumn8-1.1.0rc1/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12773 2023-06-19 12:49:40.000000 autumn8-1.1.0rc1/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17485 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5170 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-06-19 13:20:04.000000 autumn8-1.1.0rc1/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7161 2023-06-13 13:38:00.000000 autumn8-1.1.0rc1/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-24 15:09:02.000000 autumn8-1.1.0rc1/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.1.0rc1/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.1.0rc1/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.1.0rc1/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.1.0rc1/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.1.0rc1/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.1.0rc1/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/examples/tensorflow_custom_layers.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      108 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/exceptions.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       71 2023-06-19 12:42:33.000000 autumn8-1.1.0rc1/autumn8/i18n.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4067 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12004 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/lib/api/user.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1595 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/lib/asyncio.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.1.0rc1/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3606 2023-06-12 13:36:42.000000 autumn8-1.1.0rc1/autumn8/lib/service.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       69 2023-06-13 13:38:00.000000 autumn8-1.1.0rc1/autumn8/libenv.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/autumn8/types/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1924 2023-06-13 13:38:00.000000 autumn8-1.1.0rc1/autumn8/types/deployment.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      464 2023-06-13 13:38:00.000000 autumn8-1.1.0rc1/autumn8/types/router.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.466950 autumn8-1.1.0rc1/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-06-19 13:20:56.000000 autumn8-1.1.0rc1/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1544 2023-06-19 13:20:56.000000 autumn8-1.1.0rc1/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-06-19 13:20:56.000000 autumn8-1.1.0rc1/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-06-19 13:20:56.000000 autumn8-1.1.0rc1/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-06-19 13:20:56.000000 autumn8-1.1.0rc1/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-06-19 13:20:56.000000 autumn8-1.1.0rc1/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-19 13:20:56.476952 autumn8-1.1.0rc1/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-06-06 16:39:42.000000 autumn8-1.1.0rc1/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.1.0rc1/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.641544 autumn8-1.1.0rc2/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-06-20 13:13:25.641544 autumn8-1.1.0rc2/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-06-06 16:39:42.000000 autumn8-1.1.0rc2/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.621544 autumn8-1.1.0rc2/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.1.0rc2/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.631544 autumn8-1.1.0rc2/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.1.0rc2/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.1.0rc2/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     8030 2023-06-20 13:09:32.000000 autumn8-1.1.0rc2/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-06-06 16:39:42.000000 autumn8-1.1.0rc2/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.631544 autumn8-1.1.0rc2/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12773 2023-06-20 13:09:32.000000 autumn8-1.1.0rc2/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17489 2023-06-20 13:08:56.000000 autumn8-1.1.0rc2/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.1.0rc2/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5170 2023-06-12 13:36:42.000000 autumn8-1.1.0rc2/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-06-06 16:39:42.000000 autumn8-1.1.0rc2/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.1.0rc2/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-06-06 16:39:42.000000 autumn8-1.1.0rc2/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-06-06 16:39:42.000000 autumn8-1.1.0rc2/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.631544 autumn8-1.1.0rc2/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.1.0rc2/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-06-20 13:12:08.000000 autumn8-1.1.0rc2/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.631544 autumn8-1.1.0rc2/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.1.0rc2/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7161 2023-06-13 13:38:00.000000 autumn8-1.1.0rc2/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.1.0rc2/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.1.0rc2/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-24 15:09:02.000000 autumn8-1.1.0rc2/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.631544 autumn8-1.1.0rc2/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.1.0rc2/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.1.0rc2/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.1.0rc2/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.1.0rc2/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.1.0rc2/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.631544 autumn8-1.1.0rc2/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.1.0rc2/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.1.0rc2/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.1.0rc2/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.1.0rc2/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.1.0rc2/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.1.0rc2/autumn8/examples/tensorflow_custom_layers.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      108 2023-06-12 13:36:42.000000 autumn8-1.1.0rc2/autumn8/exceptions.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       71 2023-06-20 13:09:32.000000 autumn8-1.1.0rc2/autumn8/i18n.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.641544 autumn8-1.1.0rc2/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.1.0rc2/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.641544 autumn8-1.1.0rc2/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-06-06 16:39:42.000000 autumn8-1.1.0rc2/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4067 2023-06-12 13:36:42.000000 autumn8-1.1.0rc2/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12004 2023-06-12 13:36:42.000000 autumn8-1.1.0rc2/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-06-06 16:39:42.000000 autumn8-1.1.0rc2/autumn8/lib/api/user.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1595 2023-06-12 13:36:42.000000 autumn8-1.1.0rc2/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-06-06 16:39:42.000000 autumn8-1.1.0rc2/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-06-06 16:39:42.000000 autumn8-1.1.0rc2/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-06-06 16:39:42.000000 autumn8-1.1.0rc2/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.1.0rc2/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.1.0rc2/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3606 2023-06-12 13:36:42.000000 autumn8-1.1.0rc2/autumn8/lib/service.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       69 2023-06-13 13:38:00.000000 autumn8-1.1.0rc2/autumn8/libenv.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.641544 autumn8-1.1.0rc2/autumn8/types/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1957 2023-06-20 12:21:32.000000 autumn8-1.1.0rc2/autumn8/types/deployment.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      502 2023-06-20 13:08:10.000000 autumn8-1.1.0rc2/autumn8/types/router.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.621544 autumn8-1.1.0rc2/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-06-20 13:13:25.000000 autumn8-1.1.0rc2/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1544 2023-06-20 13:13:25.000000 autumn8-1.1.0rc2/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-06-20 13:13:25.000000 autumn8-1.1.0rc2/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-06-20 13:13:25.000000 autumn8-1.1.0rc2/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-06-20 13:13:25.000000 autumn8-1.1.0rc2/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-06-20 13:13:25.000000 autumn8-1.1.0rc2/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-06-06 16:39:42.000000 autumn8-1.1.0rc2/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-06-20 13:13:25.641544 autumn8-1.1.0rc2/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.1.0rc2/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-06-20 13:13:25.641544 autumn8-1.1.0rc2/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-06-06 16:39:42.000000 autumn8-1.1.0rc2/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.1.0rc2/tests/test_settings.py
```

### Comparing `autumn8-1.1.0rc1/PKG-INFO` & `autumn8-1.1.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.1.0rc1/README.md` & `autumn8-1.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/cli/analyze.py` & `autumn8-1.1.0rc2/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/cli/cli_environment.py` & `autumn8-1.1.0rc2/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/cli/commands/cloud.py` & `autumn8-1.1.0rc2/autumn8/cli/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/cli/commands/models.py` & `autumn8-1.1.0rc2/autumn8/cli/commands/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,26 +290,26 @@
         input_file=input_file,
         inferred_model_name=inferred_model_name,
         inferred_quantization=inferred_quantization,
         inferred_input_dims=inferred_input_dims,
         should_skip_inputs=should_skip_inputs,
         is_source_annotated_model=is_source_annotated_model,
     )
-    model_config = {
-        "name": model_name,
-        "framework": framework,
-        "quantization": quantization,
-        "inputs": input_dims,
-        "group_id": group_id,
-    }
+    model_config = NewModelInfo(
+        name=model_name,
+        framework=framework,
+        quantization=quantization,
+        inputs=input_dims,
+        group_id=group_id,
+    )
 
     if not auto_confirm:
         logger.info("")
         logger.info("The details for your model are as follows:")
-        click.echo(f"{json.dumps(model_config, indent=4)}")
+        click.echo(f"{json.dumps(model_config.dict(), indent=4)}")
         click.confirm(
             text="\n" + "Do you want to upload it to AutoDL?",
             abort=True,
             default=True,
         )
 
     model_upload_response = autodl_service.upload_model(
```

### Comparing `autumn8-1.1.0rc1/autumn8/cli/examples.py` & `autumn8-1.1.0rc2/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/cli/interactive.py` & `autumn8-1.1.0rc2/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/cli/main.py` & `autumn8-1.1.0rc2/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/cli/options.py` & `autumn8-1.1.0rc2/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/cli/pending_uploads.py` & `autumn8-1.1.0rc2/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/cli/validation.py` & `autumn8-1.1.0rc2/autumn8/cli/validation.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/common/config/cloud_info.py` & `autumn8-1.1.0rc2/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/common/config/settings.py` & `autumn8-1.1.0rc2/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/common/config/supported_instances.py` & `autumn8-1.1.0rc2/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/common/types.py` & `autumn8-1.1.0rc2/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/env/__init__.py` & `autumn8-1.1.0rc2/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/examples/mnist.py` & `autumn8-1.1.0rc2/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/examples/model.py` & `autumn8-1.1.0rc2/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/examples/sbert-alpha.py` & `autumn8-1.1.0rc2/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.1.0rc2/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/lib/__init__.py` & `autumn8-1.1.0rc2/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/lib/api/cloud.py` & `autumn8-1.1.0rc2/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/lib/api/lab.py` & `autumn8-1.1.0rc2/autumn8/lib/api/lab.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/lib/api/user.py` & `autumn8-1.1.0rc2/autumn8/lib/api/user.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/lib/api_creds.py` & `autumn8-1.1.0rc2/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/lib/asyncio.py` & `autumn8-1.1.0rc2/autumn8/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/lib/http.py` & `autumn8-1.1.0rc2/autumn8/lib/http.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/lib/logging.py` & `autumn8-1.1.0rc2/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/lib/logging.yaml` & `autumn8-1.1.0rc2/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/lib/package_resolver.py` & `autumn8-1.1.0rc2/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/lib/service.py` & `autumn8-1.1.0rc2/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/autumn8/types/deployment.py` & `autumn8-1.1.0rc2/autumn8/types/deployment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import dataclasses
 import enum
 import json
-from typing import Optional, Union
 from dataclasses import dataclass
+from typing import Optional, Union
+
 from pydantic import BaseModel
 
 
 class DeploymentStatus(str, enum.Enum):
     STARTING = "STARTING"
     READY = "READY"
     INVALID = "INVALID"
     CRASHED = "CRASHED"
     SLEEPING = "SLEEPING"
+    TERMINATING = "TERMINATING"
     TERMINATED = "TERMINATED"
 
 
 class ServerType(str, enum.Enum):
     MULTIMODEL_SERVER = "MULTIMODEL_SERVER"
     CUSTOM_PYTORCH_INFERER = "PYTORCH"  # for CLI imported models
     TORCHSERVE = "TORCHSERVE"
```

### Comparing `autumn8-1.1.0rc1/autumn8.egg-info/PKG-INFO` & `autumn8-1.1.0rc2/autumn8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.1.0rc1/autumn8.egg-info/SOURCES.txt` & `autumn8-1.1.0rc2/autumn8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/pyproject.toml` & `autumn8-1.1.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/tests/test_io_bottleneck_detection.py` & `autumn8-1.1.0rc2/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.1.0rc1/tests/test_settings.py` & `autumn8-1.1.0rc2/tests/test_settings.py`

 * *Files identical despite different names*

