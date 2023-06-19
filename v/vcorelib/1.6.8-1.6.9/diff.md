# Comparing `tmp/vcorelib-1.6.8.tar.gz` & `tmp/vcorelib-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-1.6.8.tar", last modified: Wed Jun 14 04:14:26 2023, max compression
+gzip compressed data, was "vcorelib-1.6.9.tar", last modified: Mon Jun 19 22:11:18 2023, max compression
```

## Comparing `vcorelib-1.6.8.tar` & `vcorelib-1.6.9.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.234040 vcorelib-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 04:12:50.000000 vcorelib-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-14 04:14:26.234040 vcorelib-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-14 04:12:50.000000 vcorelib-1.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 04:12:50.000000 vcorelib-1.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:14:26.234040 vcorelib-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-14 04:12:50.000000 vcorelib-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.226039 vcorelib-1.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-14 04:12:50.000000 vcorelib-1.6.8/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-14 04:12:50.000000 vcorelib-1.6.8/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-14 04:12:50.000000 vcorelib-1.6.8/tests/test_namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.226039 vcorelib-1.6.8/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.226039 vcorelib-1.6.8/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.230039 vcorelib-1.6.8/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.230039 vcorelib-1.6.8/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.230039 vcorelib-1.6.8/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.230039 vcorelib-1.6.8/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.230039 vcorelib-1.6.8/vcorelib/io/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/io/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/io/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/io/arbiter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/io/arbiter/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.230039 vcorelib-1.6.8/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/io/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/io/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.230039 vcorelib-1.6.8/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.230039 vcorelib-1.6.8/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/math/analysis/average.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.230039 vcorelib-1.6.8/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.230039 vcorelib-1.6.8/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.234040 vcorelib-1.6.8/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.234040 vcorelib-1.6.8/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.234040 vcorelib-1.6.8/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.234040 vcorelib-1.6.8/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.234040 vcorelib-1.6.8/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.234040 vcorelib-1.6.8/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.234040 vcorelib-1.6.8/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.234040 vcorelib-1.6.8/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-14 04:12:50.000000 vcorelib-1.6.8/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:14:26.226039 vcorelib-1.6.8/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-14 04:14:26.000000 vcorelib-1.6.8/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-14 04:14:26.000000 vcorelib-1.6.8/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:14:26.000000 vcorelib-1.6.8/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-14 04:14:26.000000 vcorelib-1.6.8/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 04:14:26.000000 vcorelib-1.6.8/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.990047 vcorelib-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-19 22:09:56.000000 vcorelib-1.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-19 22:11:18.990047 vcorelib-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-19 22:09:56.000000 vcorelib-1.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-19 22:09:56.000000 vcorelib-1.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 22:11:18.990047 vcorelib-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-19 22:09:56.000000 vcorelib-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.982047 vcorelib-1.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-19 22:09:56.000000 vcorelib-1.6.9/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-19 22:09:56.000000 vcorelib-1.6.9/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-19 22:09:56.000000 vcorelib-1.6.9/tests/test_namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.982047 vcorelib-1.6.9/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.986047 vcorelib-1.6.9/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.986047 vcorelib-1.6.9/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.986047 vcorelib-1.6.9/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.986047 vcorelib-1.6.9/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.986047 vcorelib-1.6.9/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.986047 vcorelib-1.6.9/vcorelib/io/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/io/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/io/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/io/arbiter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/io/arbiter/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.986047 vcorelib-1.6.9/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/io/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.986047 vcorelib-1.6.9/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.990047 vcorelib-1.6.9/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/math/analysis/average.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.990047 vcorelib-1.6.9/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.990047 vcorelib-1.6.9/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.990047 vcorelib-1.6.9/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.990047 vcorelib-1.6.9/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.990047 vcorelib-1.6.9/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.990047 vcorelib-1.6.9/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.990047 vcorelib-1.6.9/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.990047 vcorelib-1.6.9/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.990047 vcorelib-1.6.9/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.990047 vcorelib-1.6.9/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-19 22:09:56.000000 vcorelib-1.6.9/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:11:18.986047 vcorelib-1.6.9/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-19 22:11:18.000000 vcorelib-1.6.9/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-19 22:11:18.000000 vcorelib-1.6.9/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 22:11:18.000000 vcorelib-1.6.9/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-19 22:11:18.000000 vcorelib-1.6.9/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 22:11:18.000000 vcorelib-1.6.9/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-1.6.8/LICENSE` & `vcorelib-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/PKG-INFO` & `vcorelib-1.6.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.6.8
+Version: 1.6.9
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=cbecbdee1a9d85055f8d94cf088f2e53
+    hash=665bc6acc8632e143d0a9513eb1dac2d
     =====================================
 -->
 
-# vcorelib ([1.6.8](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.9](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.8/README.md` & `vcorelib-1.6.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=cbecbdee1a9d85055f8d94cf088f2e53
+    hash=665bc6acc8632e143d0a9513eb1dac2d
     =====================================
 -->
 
-# vcorelib ([1.6.8](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.9](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.8/pyproject.toml` & `vcorelib-1.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "1.6.8"
+version = "1.6.9"
 description = "A collection of core Python utilities."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `vcorelib-1.6.8/setup.py` & `vcorelib-1.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/tests/test_logging.py` & `vcorelib-1.6.9/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/tests/test_names.py` & `vcorelib-1.6.9/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/tests/test_namespace.py` & `vcorelib-1.6.9/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/args/__init__.py` & `vcorelib-1.6.9/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/args/newline.py` & `vcorelib-1.6.9/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/asyncio/__init__.py` & `vcorelib-1.6.9/vcorelib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/asyncio/cli.py` & `vcorelib-1.6.9/vcorelib/asyncio/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
     # Default to a valid interrupt signal.
     if signal is None:
         signal = getattr(_signal, "CTRL_C_EVENT", _signal.SIGINT)
     assert signal is not None
 
     try:
-        await proc.communicate(input=stdin)
+        with log_time(logger, "Process '%s' (%d)", name, proc.pid):
+            await proc.communicate(input=stdin)
 
     except _CancelledError:
         # Send the process a signal and wait for it to terminate.
         proc.send_signal(signal)
         logger.warning(
             "Sending signal %d to process '%s' (%d).", signal, name, proc.pid
         )
```

### Comparing `vcorelib-1.6.8/vcorelib/asyncio/subprocess.py` & `vcorelib-1.6.9/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/dict/__init__.py` & `vcorelib-1.6.9/vcorelib/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/dict/cache.py` & `vcorelib-1.6.9/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/dict/codec.py` & `vcorelib-1.6.9/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/dict/config.py` & `vcorelib-1.6.9/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/dict/env.py` & `vcorelib-1.6.9/vcorelib/dict/env.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/graph/__init__.py` & `vcorelib-1.6.9/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/graph/abc.py` & `vcorelib-1.6.9/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/graph/edge.py` & `vcorelib-1.6.9/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/graph/node.py` & `vcorelib-1.6.9/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/graph/port.py` & `vcorelib-1.6.9/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/io/__init__.py` & `vcorelib-1.6.9/vcorelib/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/io/abc.py` & `vcorelib-1.6.9/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/io/arbiter/base.py` & `vcorelib-1.6.9/vcorelib/io/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/io/arbiter/context.py` & `vcorelib-1.6.9/vcorelib/io/arbiter/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/io/arbiter/directory.py` & `vcorelib-1.6.9/vcorelib/io/arbiter/directory.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/io/archive/__init__.py` & `vcorelib-1.6.9/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/io/cache.py` & `vcorelib-1.6.9/vcorelib/io/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,17 @@
                     if logger is not None:
                         logger.log(
                             level,
                             "Extracted archive '%s' in %ss.",
                             archive,
                             nano_str(time_ns, True),
                         )
+
+                    assert path.is_dir(), path
+
                     return self.load(path, logger, level, **kwargs)
 
         if loaded and logger is not None:
             logger.log(
                 level,
                 "Cache loaded in %ss.",
                 nano_str(self.load_time_ns, True),
```

### Comparing `vcorelib-1.6.8/vcorelib/io/decode.py` & `vcorelib-1.6.9/vcorelib/io/decode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/io/encode.py` & `vcorelib-1.6.9/vcorelib/io/encode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/io/mapping.py` & `vcorelib-1.6.9/vcorelib/io/mapping.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/io/types.py` & `vcorelib-1.6.9/vcorelib/io/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,17 +71,19 @@
         """Determine if this extension is a kind of archive file."""
         return self in {FileExtension.ZIP, FileExtension.TAR}
 
     @staticmethod
     def has_archive(path: _Pathlike) -> _Optional[Path]:
         """Determine if a path has an associated archive file."""
 
+        path = normalize(path)
+
         for ext in [FileExtension.ZIP, FileExtension.TAR]:
             for ext_str in ext.value:  # pylint: disable=not-an-iterable
-                check_path = Path(f"{normalize(path)}.{ext_str}")
+                check_path = path.with_suffix(f".{ext_str}")
                 if check_path.is_file():
                     return check_path
 
         return None
 
     def is_data(self) -> bool:
         """Determine if this etension is a kind of data file."""
@@ -116,16 +118,17 @@
     def candidates(
         self, path: _Pathlike, exists_only: bool = False
     ) -> _Iterator[Path]:
         """
         For a given path, iterate over candidate paths that have the suffixes
         for this kind of file extension.
         """
+        orig = normalize(path)
         for ext in self.value:
-            path = normalize(path).with_suffix(f".{ext}")
+            path = orig.with_suffix(f".{ext}")
             if not exists_only or path.exists():
                 yield path
 
     @staticmethod
     def archive_candidates(
         path: _Pathlike, exists_only: bool = False
     ) -> _Iterator[Path]:
```

### Comparing `vcorelib-1.6.8/vcorelib/logging.py` & `vcorelib-1.6.9/vcorelib/logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/math/__init__.py` & `vcorelib-1.6.9/vcorelib/math/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/math/analysis/average.py` & `vcorelib-1.6.9/vcorelib/math/analysis/average.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-1.6.9/vcorelib/math/analysis/rate/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-1.6.9/vcorelib/math/analysis/rate/limiter.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/math/time.py` & `vcorelib-1.6.9/vcorelib/math/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/names.py` & `vcorelib-1.6.9/vcorelib/names.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/namespace.py` & `vcorelib-1.6.9/vcorelib/namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/paths/__init__.py` & `vcorelib-1.6.9/vcorelib/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/paths/context.py` & `vcorelib-1.6.9/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/paths/info.py` & `vcorelib-1.6.9/vcorelib/paths/info.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/paths/info_cache.py` & `vcorelib-1.6.9/vcorelib/paths/info_cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/platform/__init__.py` & `vcorelib-1.6.9/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/schemas/__init__.py` & `vcorelib-1.6.9/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/schemas/base.py` & `vcorelib-1.6.9/vcorelib/schemas/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/schemas/json.py` & `vcorelib-1.6.9/vcorelib/schemas/json.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/schemas/mixins.py` & `vcorelib-1.6.9/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/script/__init__.py` & `vcorelib-1.6.9/vcorelib/script/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/target/__init__.py` & `vcorelib-1.6.9/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/target/evaluation.py` & `vcorelib-1.6.9/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/target/expression.py` & `vcorelib-1.6.9/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/target/resolver.py` & `vcorelib-1.6.9/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/task/__init__.py` & `vcorelib-1.6.9/vcorelib/task/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,29 @@
 from typing import List as _List
 from typing import Optional as _Optional
 from typing import Set as _Set
 from typing import Tuple as _Tuple
 
 # internal
 from vcorelib.dict import merge_dicts
+from vcorelib.logging import LoggerMixin
 from vcorelib.math.time import Timer, nano_str
 from vcorelib.target import Substitutions, Target
 
 Outbox = _Dict[str, _Any]
 Inbox = _Dict[str, Outbox]
 TaskExecute = _Callable[[Inbox, Outbox], _Coroutine[_Any, _Any, bool]]
 TaskGenerator = _Callable[..., _asyncio.Task]
 
 
 class TaskFailed(Exception):
     """A custom exception to indicate that a task failed."""
 
 
-class Task:  # pylint: disable=too-many-instance-attributes
+class Task(LoggerMixin):  # pylint: disable=too-many-instance-attributes
     """A basic task interface definition."""
 
     stages = ["run_enter", "run", "run_exit"]
     default_requirements: _Set[str] = set()
 
     def __init__(
         self,
@@ -73,18 +74,17 @@
         self.times_invoked: int = 0
         self.dependency_time: int = 0
         self.execute_time: int = 0
         if timer is None:
             timer = Timer()
         self.timer = timer
 
-        # Get a logger if needed.
-        if log is None:
-            log = getLogger(name)
-        self.log = log
+        # Initialize logging.
+        super().__init__(logger=log if log is not None else getLogger(name))
+        self.log = self.logger
 
         # Create an execute function if none was provided.
         if execute is None:
             execute = self.create_execute(*args, **kwargs)
         self.execute = execute
 
         # Create a target if one wasn't provided.
```

### Comparing `vcorelib-1.6.8/vcorelib/task/dict/melder.py` & `vcorelib-1.6.9/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/task/manager.py` & `vcorelib-1.6.9/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/task/subprocess/run.py` & `vcorelib-1.6.9/vcorelib/task/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib/task/time/sleep.py` & `vcorelib-1.6.9/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.8/vcorelib.egg-info/PKG-INFO` & `vcorelib-1.6.9/vcorelib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.6.8
+Version: 1.6.9
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=cbecbdee1a9d85055f8d94cf088f2e53
+    hash=665bc6acc8632e143d0a9513eb1dac2d
     =====================================
 -->
 
-# vcorelib ([1.6.8](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.9](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.8/vcorelib.egg-info/SOURCES.txt` & `vcorelib-1.6.9/vcorelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

