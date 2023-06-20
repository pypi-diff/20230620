# Comparing `tmp/hyfi-0.8.1.tar.gz` & `tmp/hyfi-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.8.1.tar", max compression
+gzip compressed data, was "hyfi-0.8.2.tar", max compression
```

## Comparing `hyfi-0.8.1.tar` & `hyfi-0.8.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     1071 2023-06-19 08:19:13.066612 hyfi-0.8.1/LICENSE
--rw-r--r--   0        0        0     1828 2023-06-19 08:19:13.066612 hyfi-0.8.1/README.md
--rw-r--r--   0        0        0     4608 2023-06-19 08:19:36.907040 hyfi-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3804 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2544 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/__click__.py
--rw-r--r--   0        0        0      647 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9823 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      735 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-06-19 08:19:36.835039 hyfi-0.8.1/src/hyfi/_version.py
--rw-r--r--   0        0        0      777 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     3339 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     6832 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-06-19 08:19:13.070612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/util.py
--rw-r--r--   0        0        0      464 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/cached_path/_cached_path/version.py
--rw-r--r--   0        0        0        0 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-06-19 08:19:36.835039 hyfi-0.8.1/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      435 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       49 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      141 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0      320 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      559 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      725 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      948 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0       61 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       96 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0     1719 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      396 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      806 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      153 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      195 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0     6369 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     3045 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8363 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4535 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     6610 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0    20944 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/hydra/__init__.py
--rw-r--r--   0        0        0     7618 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/hydra/main.py
--rw-r--r--   0        0        0     3512 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     2099 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    16589 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0     2636 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/joblib/pipe.py
--rw-r--r--   0        0        0    30789 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      219 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     2365 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0      949 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/path/batch.py
--rw-r--r--   0        0        0     3758 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5335 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/py.typed
--rw-r--r--   0        0        0     4013 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     5089 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     6948 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/dataframe.py
--rw-r--r--   0        0        0     5667 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/env.py
--rw-r--r--   0        0        0     6215 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/file.py
--rw-r--r--   0        0        0    10015 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1114 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3767 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     4162 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     2002 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0     9981 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     5584 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0      232 2023-06-19 08:19:13.074612 hyfi-0.8.1/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 hyfi-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-19 09:58:52.696677 hyfi-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1828 2023-06-19 09:58:52.696677 hyfi-0.8.2/README.md
+-rw-r--r--   0        0        0     4608 2023-06-19 09:59:17.932727 hyfi-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     3804 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2544 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      647 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9824 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      735 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-19 09:59:17.864727 hyfi-0.8.2/src/hyfi/_version.py
+-rw-r--r--   0        0        0      777 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     3339 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     6832 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/cached_path/_cached_path/version.py
+-rw-r--r--   0        0        0        0 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-19 09:59:17.864727 hyfi-0.8.2/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      435 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      141 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0      320 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      559 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      725 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      948 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       96 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      396 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      806 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      153 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      195 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0     6369 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     3045 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8363 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4535 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     6610 2023-06-19 09:58:52.700677 hyfi-0.8.2/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0    20946 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/hydra/__init__.py
+-rw-r--r--   0        0        0     7618 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/hydra/main.py
+-rw-r--r--   0        0        0     3512 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     2099 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    16589 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0     2636 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/joblib/pipe.py
+-rw-r--r--   0        0        0    30789 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     2365 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0      949 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0     3758 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5335 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4013 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     5089 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     6948 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/utils/dataframe.py
+-rw-r--r--   0        0        0     5667 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0     6215 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/utils/file.py
+-rw-r--r--   0        0        0    10015 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1114 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3767 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     4162 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     2002 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0     9981 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     5584 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      232 2023-06-19 09:58:52.704677 hyfi-0.8.2/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     3190 1970-01-01 00:00:00.000000 hyfi-0.8.2/PKG-INFO
```

### Comparing `hyfi-0.8.1/LICENSE` & `hyfi-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/README.md` & `hyfi-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/pyproject.toml` & `hyfi-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.8.1"
+version = "0.8.2"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-0.8.1/src/hyfi/__cli__.py` & `hyfi-0.8.2/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/__click__.py` & `hyfi-0.8.2/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/__global__/__init__.py` & `hyfi-0.8.2/src/hyfi/__global__/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/__global__/config.py` & `hyfi-0.8.2/src/hyfi/__global__/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
             config = Composer(
                 overrides=["+project=__init__"],
                 config_module=__about__.config_module,
             ).config_as_dict
 
         # Skip project config initialization.
         if "project" not in config:
-            logger.info("No project config found, skip project config initialization.")
+            logger.debug("No project config found, skip project config initialization.")
             return
         self.project = ProjectConfig(**config["project"])
         # self.project.init_project()
         # Initialize joblib backend if joblib is not set.
         if self.project.joblib:
             self.project.joblib.init_backend()
```

### Comparing `hyfi-0.8.1/src/hyfi/__init__.py` & `hyfi-0.8.2/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/about/__init__.py` & `hyfi-0.8.2/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/batch/__init__.py` & `hyfi-0.8.2/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/__init__.py` & `hyfi-0.8.2/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/__init__.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/_cached_path.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/cache_file.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/common.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/file_lock.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/meta.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/progress.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/__init__.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/beaker.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/hf.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/http.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/testing.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/cached_path/_cached_path/util.py` & `hyfi-0.8.2/src/hyfi/cached_path/_cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.8.2/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.8.2/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.8.2/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.8.2/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.8.2/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/conf/project/__init__.yaml` & `hyfi-0.8.2/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/copier/__init__.py` & `hyfi-0.8.2/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/dotenv/__init__.py` & `hyfi-0.8.2/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/graphics/collage.py` & `hyfi-0.8.2/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/graphics/motion.py` & `hyfi-0.8.2/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/graphics/utils.py` & `hyfi-0.8.2/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/hydra/__init__.py` & `hyfi-0.8.2/src/hyfi/hydra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,18 +610,18 @@
             getattr(self, method)(val)
 
     def initialize_configs(
         self,
         **data,
     ):
         if not self.config_group:
-            logger.info("There is no config group specified.")
+            logger.debug("There is no config group specified.")
             return
         # Initialize the config with the given config_name.
-        logger.info(
+        logger.debug(
             "Initializing `%s` class with `%s` config in `%s` group.",
             self.__class__.__name__,
             self.config_name,
             self.config_group,
         )
         data = Composer(
             config_group=f"{self.config_group}={self.config_name}",
```

### Comparing `hyfi-0.8.1/src/hyfi/hydra/main.py` & `hyfi-0.8.2/src/hyfi/hydra/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/joblib/__init__.py` & `hyfi-0.8.2/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/joblib/batch/apply.py` & `hyfi-0.8.2/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-0.8.2/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/joblib/batch/batcher.py` & `hyfi-0.8.2/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/joblib/pipe.py` & `hyfi-0.8.2/src/hyfi/joblib/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/main/__init__.py` & `hyfi-0.8.2/src/hyfi/main/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/path/__init__.py` & `hyfi-0.8.2/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/path/batch.py` & `hyfi-0.8.2/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/path/task.py` & `hyfi-0.8.2/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/project/__init__.py` & `hyfi-0.8.2/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/task/__init__.py` & `hyfi-0.8.2/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/task/batch.py` & `hyfi-0.8.2/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/utils/dataframe.py` & `hyfi-0.8.2/src/hyfi/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/utils/env.py` & `hyfi-0.8.2/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/utils/file.py` & `hyfi-0.8.2/src/hyfi/utils/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/utils/func.py` & `hyfi-0.8.2/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/utils/google.py` & `hyfi-0.8.2/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/utils/gpu.py` & `hyfi-0.8.2/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/utils/lib.py` & `hyfi-0.8.2/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/utils/logging.py` & `hyfi-0.8.2/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/utils/notebook.py` & `hyfi-0.8.2/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/src/hyfi/utils/tools.py` & `hyfi-0.8.2/src/hyfi/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.8.1/PKG-INFO` & `hyfi-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.8.1
+Version: 0.8.2
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

