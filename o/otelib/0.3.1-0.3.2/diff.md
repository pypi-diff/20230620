# Comparing `tmp/otelib-0.3.1.tar.gz` & `tmp/otelib-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otelib-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "otelib-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `otelib-0.3.1.tar` & `otelib-0.3.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0      184 2023-05-24 13:56:13.254460 otelib-0.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0      637 2023-05-24 13:56:13.254460 otelib-0.3.1/.github/pull_request_template.md
--rwxr-xr-x   0        0        0     3658 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/utils/wait_for_it.sh
--rw-r--r--   0        0        0      675 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/workflows/cd_release.yml
--rw-r--r--   0        0        0      437 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/workflows/ci_automerge_dependabot.yml
--rw-r--r--   0        0        0      479 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/workflows/ci_cd_updated_master.yml
--rw-r--r--   0        0        0      544 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/workflows/ci_check_dependencies.yml
--rw-r--r--   0        0        0      920 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/workflows/ci_dependabot.yml
--rw-r--r--   0        0        0     3537 2023-05-24 13:56:13.258460 otelib-0.3.1/.github/workflows/ci_tests.yml
--rw-r--r--   0        0        0     3152 2023-05-24 13:56:13.258460 otelib-0.3.1/.gitignore
--rw-r--r--   0        0        0     1731 2023-05-24 13:56:13.258460 otelib-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     9185 2023-05-24 13:57:09.989290 otelib-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1050 2023-05-24 13:56:13.258460 otelib-0.3.1/LICENSE
--rw-r--r--   0        0        0     8173 2023-05-24 13:56:13.258460 otelib-0.3.1/README.md
--rw-r--r--   0        0        0     2438 2023-05-24 13:56:13.258460 otelib-0.3.1/docs/demo-notebooks/execute.ipynb
--rw-r--r--   0        0        0    11095 2023-05-24 13:56:13.258460 otelib-0.3.1/docs/img/classes.svg
--rw-r--r--   0        0        0     5473 2023-05-24 13:56:13.258460 otelib-0.3.1/docs/img/filters.drawio
--rw-r--r--   0        0        0     6814 2023-05-24 13:56:13.258460 otelib-0.3.1/docs/img/generic-pipeline.svg
--rw-r--r--   0        0        0    43501 2023-05-24 13:56:13.258460 otelib-0.3.1/docs/img/otelib-overview.png
--rw-r--r--   0        0        0    22053 2023-05-24 13:56:13.258460 otelib-0.3.1/docs/img/pipeline.jpg
--rw-r--r--   0        0        0      226 2023-05-24 13:57:10.553318 otelib-0.3.1/otelib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/__init__.py
--rw-r--r--   0        0        0     2638 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/client.py
--rw-r--r--   0        0        0     1960 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/factories.py
--rw-r--r--   0        0        0      354 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/__init__.py
--rw-r--r--   0        0        0     4911 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/base.py
--rw-r--r--   0        0        0     1876 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/client.py
--rw-r--r--   0        0        0     2678 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/dataresource.py
--rw-r--r--   0        0        0      438 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/filter.py
--rw-r--r--   0        0        0      461 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/function.py
--rw-r--r--   0        0        0      445 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/mapping.py
--rw-r--r--   0        0        0      487 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/python/transformation.py
--rw-r--r--   0        0        0      354 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/__init__.py
--rw-r--r--   0        0        0     4755 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/base.py
--rw-r--r--   0        0        0     1719 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/client.py
--rw-r--r--   0        0        0      388 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/dataresource.py
--rw-r--r--   0        0        0      288 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/filter.py
--rw-r--r--   0        0        0      300 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/function.py
--rw-r--r--   0        0        0      294 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/mapping.py
--rw-r--r--   0        0        0      328 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/services/transformation.py
--rw-r--r--   0        0        0     3827 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/strategies.py
--rw-r--r--   0        0        0      582 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/backends/utils.py
--rw-r--r--   0        0        0     3012 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/client.py
--rw-r--r--   0        0        0     1260 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/exceptions.py
--rw-r--r--   0        0        0      562 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/pipe.py
--rw-r--r--   0        0        0      484 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/settings.py
--rw-r--r--   0        0        0      218 2023-05-24 13:56:13.258460 otelib-0.3.1/otelib/warnings.py
--rw-r--r--   0        0        0     1865 2023-05-24 13:56:13.258460 otelib-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    11856 2023-05-24 13:56:13.258460 otelib-0.3.1/test_pythonbackend.ipynb
--rw-r--r--   0        0        0     8762 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     1504 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/strategies/conftest.py
--rw-r--r--   0        0        0     7010 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/strategies/test_abc.py
--rw-r--r--   0        0        0     9783 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/strategies/test_all_strategies.py
--rw-r--r--   0        0        0     1061 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/test_config.py
--rw-r--r--   0        0        0     5021 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/test_oteclient.py
--rw-r--r--   0        0        0    10937 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/test_pipe.py
--rw-r--r--   0        0        0     3904 2023-05-24 13:56:13.258460 otelib-0.3.1/tests/utils.py
--rw-r--r--   0        0        0     9440 1970-01-01 00:00:00.000000 otelib-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      184 2023-06-20 13:33:46.086920 otelib-0.3.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      637 2023-06-20 13:33:46.086920 otelib-0.3.2/.github/pull_request_template.md
+-rwxr-xr-x   0        0        0     3658 2023-06-20 13:33:46.086920 otelib-0.3.2/.github/utils/wait_for_it.sh
+-rw-r--r--   0        0        0      675 2023-06-20 13:33:46.086920 otelib-0.3.2/.github/workflows/cd_release.yml
+-rw-r--r--   0        0        0      437 2023-06-20 13:33:46.086920 otelib-0.3.2/.github/workflows/ci_automerge_dependabot.yml
+-rw-r--r--   0        0        0      479 2023-06-20 13:33:46.086920 otelib-0.3.2/.github/workflows/ci_cd_updated_master.yml
+-rw-r--r--   0        0        0      544 2023-06-20 13:33:46.086920 otelib-0.3.2/.github/workflows/ci_check_dependencies.yml
+-rw-r--r--   0        0        0      920 2023-06-20 13:33:46.086920 otelib-0.3.2/.github/workflows/ci_dependabot.yml
+-rw-r--r--   0        0        0     3537 2023-06-20 13:33:46.086920 otelib-0.3.2/.github/workflows/ci_tests.yml
+-rw-r--r--   0        0        0     3152 2023-06-20 13:33:46.086920 otelib-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1731 2023-06-20 13:33:46.086920 otelib-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9924 2023-06-20 13:34:58.531974 otelib-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1050 2023-06-20 13:33:46.086920 otelib-0.3.2/LICENSE
+-rw-r--r--   0        0        0     8270 2023-06-20 13:33:46.086920 otelib-0.3.2/README.md
+-rw-r--r--   0        0        0     2438 2023-06-20 13:33:46.086920 otelib-0.3.2/docs/demo-notebooks/execute.ipynb
+-rw-r--r--   0        0        0    11095 2023-06-20 13:33:46.086920 otelib-0.3.2/docs/img/classes.svg
+-rw-r--r--   0        0        0     5473 2023-06-20 13:33:46.086920 otelib-0.3.2/docs/img/filters.drawio
+-rw-r--r--   0        0        0     6814 2023-06-20 13:33:46.086920 otelib-0.3.2/docs/img/generic-pipeline.svg
+-rw-r--r--   0        0        0    43501 2023-06-20 13:33:46.086920 otelib-0.3.2/docs/img/otelib-overview.png
+-rw-r--r--   0        0        0    22053 2023-06-20 13:33:46.086920 otelib-0.3.2/docs/img/pipeline.jpg
+-rw-r--r--   0        0        0      226 2023-06-20 13:34:59.227985 otelib-0.3.2/otelib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 13:33:46.086920 otelib-0.3.2/otelib/backends/__init__.py
+-rw-r--r--   0        0        0     2638 2023-06-20 13:33:46.086920 otelib-0.3.2/otelib/backends/client.py
+-rw-r--r--   0        0        0     1960 2023-06-20 13:33:46.086920 otelib-0.3.2/otelib/backends/factories.py
+-rw-r--r--   0        0        0      354 2023-06-20 13:33:46.086920 otelib-0.3.2/otelib/backends/python/__init__.py
+-rw-r--r--   0        0        0     4911 2023-06-20 13:33:46.086920 otelib-0.3.2/otelib/backends/python/base.py
+-rw-r--r--   0        0        0     1876 2023-06-20 13:33:46.086920 otelib-0.3.2/otelib/backends/python/client.py
+-rw-r--r--   0        0        0     2678 2023-06-20 13:33:46.086920 otelib-0.3.2/otelib/backends/python/dataresource.py
+-rw-r--r--   0        0        0      438 2023-06-20 13:33:46.086920 otelib-0.3.2/otelib/backends/python/filter.py
+-rw-r--r--   0        0        0      461 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/python/function.py
+-rw-r--r--   0        0        0      445 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/python/mapping.py
+-rw-r--r--   0        0        0      487 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/python/transformation.py
+-rw-r--r--   0        0        0      354 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/services/__init__.py
+-rw-r--r--   0        0        0     4755 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/services/base.py
+-rw-r--r--   0        0        0     1719 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/services/client.py
+-rw-r--r--   0        0        0      388 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/services/dataresource.py
+-rw-r--r--   0        0        0      288 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/services/filter.py
+-rw-r--r--   0        0        0      300 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/services/function.py
+-rw-r--r--   0        0        0      294 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/services/mapping.py
+-rw-r--r--   0        0        0      328 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/services/transformation.py
+-rw-r--r--   0        0        0     4204 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/strategies.py
+-rw-r--r--   0        0        0      582 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/backends/utils.py
+-rw-r--r--   0        0        0     3012 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/client.py
+-rw-r--r--   0        0        0     1260 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/exceptions.py
+-rw-r--r--   0        0        0      562 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/pipe.py
+-rw-r--r--   0        0        0      484 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/settings.py
+-rw-r--r--   0        0        0      218 2023-06-20 13:33:46.090920 otelib-0.3.2/otelib/warnings.py
+-rw-r--r--   0        0        0     1865 2023-06-20 13:33:46.090920 otelib-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    11856 2023-06-20 13:33:46.090920 otelib-0.3.2/test_pythonbackend.ipynb
+-rw-r--r--   0        0        0     8762 2023-06-20 13:33:46.090920 otelib-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0     1504 2023-06-20 13:33:46.090920 otelib-0.3.2/tests/strategies/conftest.py
+-rw-r--r--   0        0        0     7010 2023-06-20 13:33:46.090920 otelib-0.3.2/tests/strategies/test_abc.py
+-rw-r--r--   0        0        0     9783 2023-06-20 13:33:46.090920 otelib-0.3.2/tests/strategies/test_all_strategies.py
+-rw-r--r--   0        0        0     1061 2023-06-20 13:33:46.090920 otelib-0.3.2/tests/test_config.py
+-rw-r--r--   0        0        0     5021 2023-06-20 13:33:46.090920 otelib-0.3.2/tests/test_oteclient.py
+-rw-r--r--   0        0        0    12651 2023-06-20 13:33:46.090920 otelib-0.3.2/tests/test_pipe.py
+-rw-r--r--   0        0        0     3904 2023-06-20 13:33:46.090920 otelib-0.3.2/tests/utils.py
+-rw-r--r--   0        0        0     9537 1970-01-01 00:00:00.000000 otelib-0.3.2/PKG-INFO
```

### Comparing `otelib-0.3.1/.github/pull_request_template.md` & `otelib-0.3.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/.github/utils/wait_for_it.sh` & `otelib-0.3.2/.github/utils/wait_for_it.sh`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/.github/workflows/cd_release.yml` & `otelib-0.3.2/.github/workflows/cd_release.yml`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/.github/workflows/ci_check_dependencies.yml` & `otelib-0.3.2/.github/workflows/ci_check_dependencies.yml`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/.github/workflows/ci_dependabot.yml` & `otelib-0.3.2/.github/workflows/ci_dependabot.yml`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/.github/workflows/ci_tests.yml` & `otelib-0.3.2/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/.gitignore` & `otelib-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/.pre-commit-config.yaml` & `otelib-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/CHANGELOG.md` & `otelib-0.3.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 # Changelog
 
-## [v0.3.1](https://github.com/EMMC-ASBL/otelib/tree/v0.3.1) (2023-05-23)
+## [v0.3.2](https://github.com/EMMC-ASBL/otelib/tree/v0.3.2) (2023-06-08)
+
+[Full Changelog](https://github.com/EMMC-ASBL/otelib/compare/v0.3.1...v0.3.2)
+
+**Closed issues:**
+
+- Fix: input\_pipe  not set correctly when two pipelines are merged [\#110](https://github.com/EMMC-ASBL/otelib/issues/110)
+
+**Merged pull requests:**
+
+- \[Auto-generated\] Update dependencies [\#117](https://github.com/EMMC-ASBL/otelib/pull/117) ([TEAM4-0](https://github.com/TEAM4-0))
+- Doi badge [\#115](https://github.com/EMMC-ASBL/otelib/pull/115) ([jesper-friis](https://github.com/jesper-friis))
+- Add checks to make sure input\_pipe is set to the first filter [\#111](https://github.com/EMMC-ASBL/otelib/pull/111) ([Treesarj](https://github.com/Treesarj))
+
+## [v0.3.1](https://github.com/EMMC-ASBL/otelib/tree/v0.3.1) (2023-05-24)
 
 [Full Changelog](https://github.com/EMMC-ASBL/otelib/compare/v0.3.0...v0.3.1)
 
 **Merged pull requests:**
 
 - \[Auto-generated\] Update dependencies [\#113](https://github.com/EMMC-ASBL/otelib/pull/113) ([TEAM4-0](https://github.com/TEAM4-0))
 - Enh/add auth [\#96](https://github.com/EMMC-ASBL/otelib/pull/96) ([MBueschelberger](https://github.com/MBueschelberger))
```

### Comparing `otelib-0.3.1/LICENSE` & `otelib-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/README.md` & `otelib-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/otelib?logo=pypi)](https://pypi.org/project/otelib)
 [![PyPI](https://img.shields.io/pypi/v/otelib?logo=pypi)](https://pypi.org/project/otelib)
 [![Codecov master](https://img.shields.io/codecov/c/github/EMMC-ASBL/otelib/master?logo=codecov)](https://app.codecov.io/gh/EMMC-ASBL/otelib)
 [![CI - Tests](https://github.com/EMMC-ASBL/otelib/actions/workflows/ci_tests.yml/badge.svg?branch=master)](https://github.com/EMMC-ASBL/otelib/actions/workflows/ci_tests.yml?query=branch%3Amaster)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/m/EMMC-ASBL/otelib?logo=github)](https://github.com/EMMC-ASBL/otelib/pulse)
 [![GitHub last commit](https://img.shields.io/github/last-commit/EMMC-ASBL/otelib?logo=github)](https://github.com/EMMC-ASBL/otelib/pulse)
+[![DOI](https://zenodo.org/badge/447285057.svg)](https://zenodo.org/badge/latestdoi/447285057)
+
+
 
 OTELib is a small Python library on top of the OTEAPI, that provides a simple and pythonic interface to the REST services.
 
 It makes it very simple to configure, set up and run a pipeline based on the pipes and filter design pattern.
 
 ## Content
```

### Comparing `otelib-0.3.1/docs/demo-notebooks/execute.ipynb` & `otelib-0.3.2/docs/demo-notebooks/execute.ipynb`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/docs/img/classes.svg` & `otelib-0.3.2/docs/img/classes.svg`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/docs/img/filters.drawio` & `otelib-0.3.2/docs/img/filters.drawio`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/docs/img/generic-pipeline.svg` & `otelib-0.3.2/docs/img/generic-pipeline.svg`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/docs/img/otelib-overview.png` & `otelib-0.3.2/docs/img/otelib-overview.png`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/docs/img/pipeline.jpg` & `otelib-0.3.2/docs/img/pipeline.jpg`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/otelib/backends/client.py` & `otelib-0.3.2/otelib/backends/client.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/otelib/backends/factories.py` & `otelib-0.3.2/otelib/backends/factories.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/otelib/backends/python/base.py` & `otelib-0.3.2/otelib/backends/python/base.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/otelib/backends/python/client.py` & `otelib-0.3.2/otelib/backends/python/client.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/otelib/backends/python/dataresource.py` & `otelib-0.3.2/otelib/backends/python/dataresource.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/otelib/backends/services/base.py` & `otelib-0.3.2/otelib/backends/services/base.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/otelib/backends/services/client.py` & `otelib-0.3.2/otelib/backends/services/client.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/otelib/backends/strategies.py` & `otelib-0.3.2/otelib/backends/strategies.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,22 +111,36 @@
         """Used by `__rshift__` to set the input pipe.
 
         Parameters:
             input_pipe: A pipe representing the strategy that is "piped" into this
                 strategy.
 
         """
-        self.input_pipe = input_pipe
+        start_filter = _find_start_filter(self)
+        start_filter.input_pipe = input_pipe
 
     def __rshift__(self, other: "AbstractBaseStrategy") -> "AbstractBaseStrategy":
         """Implements strategy concatenation using the `>>` symbol.
 
         Parameters:
             other: The next strategy this one is "piping" into.
 
         Returns:
             The next strategy this one is "piped" into.
 
         """
         pipe = Pipe(self)
         other._set_input(pipe)
         return other
+
+
+def _find_start_filter(other):
+    """Used by _set_input to find the input filter,
+    incase of pipeline concatenation."""
+
+    while hasattr(other, "input_pipe"):
+        pipe = other.input_pipe
+        if hasattr(pipe, "input"):
+            other = pipe.input
+        else:
+            return other
+    return other
```

### Comparing `otelib-0.3.1/otelib/backends/utils.py` & `otelib-0.3.2/otelib/backends/utils.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/otelib/client.py` & `otelib-0.3.2/otelib/client.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/otelib/exceptions.py` & `otelib-0.3.2/otelib/exceptions.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/otelib/pipe.py` & `otelib-0.3.2/otelib/pipe.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/pyproject.toml` & `otelib-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     "Operating System :: OS Independent",
 ]
 keywords = ["OTE", "OTE-API"]
 requires-python = "~=3.9"
 dynamic = ["version"]
 
 dependencies = [
-    "oteapi-core >=0.4.2,<1",
+    "oteapi-core >=0.4.4,<1",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pre-commit ~=3.3",
     "pylint ~=2.17",
     "pytest ~=7.3",
-    "pytest-cov ~=4.0",
+    "pytest-cov ~=4.1",
     "requests-mock ~=1.10",
 ]
 
 [project.urls]
 Home = "https://github.com/EMMC-ASBL/otelib"
 Documentation = "https://EMMC-ASBL.github.io/otelib"
 Source = "https://github.com/EMMC-ASBL/otelib"
```

### Comparing `otelib-0.3.1/test_pythonbackend.ipynb` & `otelib-0.3.2/test_pythonbackend.ipynb`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/tests/conftest.py` & `otelib-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/tests/strategies/conftest.py` & `otelib-0.3.2/tests/strategies/conftest.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/tests/strategies/test_abc.py` & `otelib-0.3.2/tests/strategies/test_abc.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/tests/strategies/test_all_strategies.py` & `otelib-0.3.2/tests/strategies/test_all_strategies.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/tests/test_config.py` & `otelib-0.3.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/tests/test_oteclient.py` & `otelib-0.3.2/tests/test_oteclient.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/tests/test_pipe.py` & `otelib-0.3.2/tests/test_pipe.py`

 * *Files 14% similar despite different names*

```diff
@@ -321,7 +321,55 @@
         session_ids = [x for x in pipeline.cache if "session" in x]
         assert len(session_ids) == 1
         session_id = session_ids[0]
         session = pipeline.cache[session_id]
     for key, value in session_test_content.items():
         assert key in session
         assert value == session[key]
+
+
+def test_pipeing_concatenate(  # pylint: disable=too-many-statements
+    backend: str,
+    server_url: str,
+) -> None:
+    """Tests for the correct chaining of resources and filters in a pipeline.
+    This function tests for issue 110: https://github.com/EMMC-ASBL/otelib/issues/110
+    """
+
+    import importlib
+
+    strategies = importlib.import_module(f"otelib.backends.{backend}")
+    server_url = server_url if backend != "python" else backend
+
+    strategy_kwargs = {}
+    if backend == "python":
+        # Setup custom cache
+        cache = {}
+        strategy_kwargs["cache"] = cache
+
+    data_resource1: "DataResource" = strategies.DataResource(
+        server_url, **strategy_kwargs
+    )
+    dataid1 = data_resource1.strategy_id
+    filter1: "Filter" = strategies.Filter(server_url, **strategy_kwargs)
+    filterid1 = filter1.strategy_id
+    pipeline1 = data_resource1 >> filter1
+
+    data_resource2: "DataResource" = strategies.DataResource(
+        server_url, **strategy_kwargs
+    )
+    dataid2 = data_resource2.strategy_id
+    filter2: "Filter" = strategies.Filter(server_url, **strategy_kwargs)
+    filterid2 = filter2.strategy_id
+    pipeline2 = data_resource2 >> filter2
+
+    pipeline_combined = pipeline1 >> pipeline2
+
+    # confirm that we can retrieve the strategy ids
+    pipeline_tail = pipeline_combined  # or should it be pipeline head?
+    assert pipeline_tail.strategy_id == dataid1
+    pipeline_tail = pipeline_tail.input_pipe.input
+    assert pipeline_tail.strategy_id == filterid1
+    pipeline_tail = pipeline_tail.input_pipe.input
+    assert pipeline_tail.strategy_id == dataid2
+    pipeline_tail = pipeline_tail.input_pipe.input
+    assert pipeline_tail.strategy_id == filterid2
```

### Comparing `otelib-0.3.1/tests/utils.py` & `otelib-0.3.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `otelib-0.3.1/PKG-INFO` & `otelib-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: otelib
-Version: 0.3.1
+Version: 0.3.2
 Summary: Open Translation Environment (OTE) REST API client library.
 Keywords: OTE,OTE-API
 Author-email: SINTEF <TEAM4.0@SINTEF.no>
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Requires-Dist: oteapi-core >=0.4.2,<1
+Requires-Dist: oteapi-core >=0.4.4,<1
 Requires-Dist: pre-commit ~=3.3 ; extra == "dev"
 Requires-Dist: pylint ~=2.17 ; extra == "dev"
 Requires-Dist: pytest ~=7.3 ; extra == "dev"
-Requires-Dist: pytest-cov ~=4.0 ; extra == "dev"
+Requires-Dist: pytest-cov ~=4.1 ; extra == "dev"
 Requires-Dist: requests-mock ~=1.10 ; extra == "dev"
 Project-URL: Changelog, https://github.com/EMMC-ASBL/otelib/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://EMMC-ASBL.github.io/otelib
 Project-URL: Home, https://github.com/EMMC-ASBL/otelib
 Project-URL: Issue Tracker, https://github.com/EMMC-ASBL/otelib/issues
 Project-URL: Package, https://pypi.org/project/otelib
 Project-URL: Source, https://github.com/EMMC-ASBL/otelib
@@ -31,14 +31,17 @@
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/otelib?logo=pypi)](https://pypi.org/project/otelib)
 [![PyPI](https://img.shields.io/pypi/v/otelib?logo=pypi)](https://pypi.org/project/otelib)
 [![Codecov master](https://img.shields.io/codecov/c/github/EMMC-ASBL/otelib/master?logo=codecov)](https://app.codecov.io/gh/EMMC-ASBL/otelib)
 [![CI - Tests](https://github.com/EMMC-ASBL/otelib/actions/workflows/ci_tests.yml/badge.svg?branch=master)](https://github.com/EMMC-ASBL/otelib/actions/workflows/ci_tests.yml?query=branch%3Amaster)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/m/EMMC-ASBL/otelib?logo=github)](https://github.com/EMMC-ASBL/otelib/pulse)
 [![GitHub last commit](https://img.shields.io/github/last-commit/EMMC-ASBL/otelib?logo=github)](https://github.com/EMMC-ASBL/otelib/pulse)
+[![DOI](https://zenodo.org/badge/447285057.svg)](https://zenodo.org/badge/latestdoi/447285057)
+
+
 
 OTELib is a small Python library on top of the OTEAPI, that provides a simple and pythonic interface to the REST services.
 
 It makes it very simple to configure, set up and run a pipeline based on the pipes and filter design pattern.
 
 ## Content
```

