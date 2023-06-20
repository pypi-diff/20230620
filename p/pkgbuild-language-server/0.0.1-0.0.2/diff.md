# Comparing `tmp/pkgbuild-language-server-0.0.1.tar.gz` & `tmp/pkgbuild-language-server-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgbuild-language-server-0.0.1.tar", last modified: Mon Jun 19 15:12:44 2023, max compression
+gzip compressed data, was "pkgbuild-language-server-0.0.2.tar", last modified: Tue Jun 20 08:14:37 2023, max compression
```

## Comparing `pkgbuild-language-server-0.0.1.tar` & `pkgbuild-language-server-0.0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/docs/api/pkgbuild-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/requirements/cache.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/scripts/generate-api.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.374855 pkgbuild-language-server-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 15:12:44.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.374855 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)    15502 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/assets/json/pkgbuild.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-19 15:12:44.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-19 15:12:44.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:12:44.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-19 15:12:44.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 15:12:44.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 15:12:44.000000 pkgbuild-language-server-0.0.1/src/pkgbuild_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:12:44.378855 pkgbuild-language-server-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-19 15:12:29.000000 pkgbuild-language-server-0.0.1/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.675552 pkgbuild-language-server-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.663552 pkgbuild-language-server-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.667552 pkgbuild-language-server-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-20 08:14:37.675552 pkgbuild-language-server-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.667552 pkgbuild-language-server-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.667552 pkgbuild-language-server-0.0.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/docs/api/pkgbuild-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.667552 pkgbuild-language-server-0.0.2/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.667552 pkgbuild-language-server-0.0.2/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/requirements/cache.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.667552 pkgbuild-language-server-0.0.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/scripts/generate-api.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:14:37.675552 pkgbuild-language-server-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.659551 pkgbuild-language-server-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.671552 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.659551 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.671552 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/assets/json/pkgbuild.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.671552 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.675552 pkgbuild-language-server-0.0.2/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.675552 pkgbuild-language-server-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/tests/server_test.py
```

### Comparing `pkgbuild-language-server-0.0.1/.github/workflows/main.yml` & `pkgbuild-language-server-0.0.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.1/.gitignore` & `pkgbuild-language-server-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.1/.pre-commit-config.yaml` & `pkgbuild-language-server-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.1/LICENSE` & `pkgbuild-language-server-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.1/PKG-INFO` & `pkgbuild-language-server-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgbuild-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: pkgbuild language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://pkgbuild-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/pkgbuild-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/pkgbuild-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/pkgbuild-language-server
@@ -66,15 +66,17 @@
 [![pypi/status](https://shields.io/pypi/status/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#description)
 [![pypi/v](https://shields.io/pypi/v/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#history)
 [![pypi/downloads](https://shields.io/pypi/dd/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/format](https://shields.io/pypi/format/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 
-Language server for [PKGBUILD](https://wiki.archlinux.org/title/PKGBUILD).
+Language server for [ArchLinux](https://archlinux.org)/[Windows Msys2](https://msys2.org)'s
+[PKGBUILD](https://wiki.archlinux.org/title/PKGBUILD) and
+[`*.install`](https://wiki.archlinux.org/title/PKGBUILD#install)
 
 PKGBUILD is a subtype of bash. See
 [bash-language-server](https://github.com/bash-lsp/bash-language-server) to get
 support of bash language server.
 
 - [x] document hover
 - [x] completion
```

### Comparing `pkgbuild-language-server-0.0.1/README.md` & `pkgbuild-language-server-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 [![pypi/status](https://shields.io/pypi/status/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#description)
 [![pypi/v](https://shields.io/pypi/v/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#history)
 [![pypi/downloads](https://shields.io/pypi/dd/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/format](https://shields.io/pypi/format/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 
-Language server for [PKGBUILD](https://wiki.archlinux.org/title/PKGBUILD).
+Language server for [ArchLinux](https://archlinux.org)/[Windows Msys2](https://msys2.org)'s
+[PKGBUILD](https://wiki.archlinux.org/title/PKGBUILD) and
+[`*.install`](https://wiki.archlinux.org/title/PKGBUILD#install)
 
 PKGBUILD is a subtype of bash. See
 [bash-language-server](https://github.com/bash-lsp/bash-language-server) to get
 support of bash language server.
 
 - [x] document hover
 - [x] completion
```

### Comparing `pkgbuild-language-server-0.0.1/docs/conf.py` & `pkgbuild-language-server-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.1/docs/resources/configure.md` & `pkgbuild-language-server-0.0.2/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.1/docs/resources/install.md` & `pkgbuild-language-server-0.0.2/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.1/flake.nix` & `pkgbuild-language-server-0.0.2/flake.nix`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.1/pyproject.toml` & `pkgbuild-language-server-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/__main__.py` & `pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/api.py` & `pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     :rtype: str
     """
     return "\n".join(
         [token.content.replace("\n", " ") for token in tokens if token.content]
     )
 
 
-def init_document() -> dict[str, tuple[str, str]]:
+def init_document() -> dict[str, tuple[str, str, str]]:
     r"""Init document.
 
-    :rtype: dict[str, tuple[str, str]]
+    :rtype: dict[str, tuple[str, str, str]]
     """
     md = MarkdownIt("commonmark", {})
     with open(
         os.path.join(
             os.path.join(site_data_dir("man"), "man5"), "PKGBUILD.5.gz"
         ),
         "rb",
@@ -69,12 +69,17 @@
     for index, close_index in zip(indices, close_indices):
         children = tokens[index].children
         if children is None:
             continue
         vars = children[2].content.split()
         kind = vars[1].lstrip("(").rstrip(")") if len(vars) > 1 else ""
         kind = {"": "Variable", "array": "Field"}.get(kind, kind)
-        items[vars[0]] = (
-            kind,
+        belongs_to_install = vars[0].startswith("pre_") or vars[0].startswith(
+            "post_"
+        )
+        # Don't need to append `()` to PKGBUILD's functions due to `package_XXX()`
+        items[vars[0] + ("()" if belongs_to_install else "")] = (
+            "Function" if belongs_to_install else kind,
             get_content(tokens[index + 1 : close_index]),
+            "install" if belongs_to_install else "PKGBUILD",
         )
     return items
```

### Comparing `pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/assets/json/pkgbuild.json` & `pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/assets/json/pkgbuild.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6249999999999997%*

 * *Differences: {"'arch'": "{insert: [(2, 'PKGBUILD')]}",*

 * * "'backup'": "{insert: [(2, 'PKGBUILD')]}",*

 * * "'build()'": "{insert: [(2, 'PKGBUILD')]}",*

 * * "'changelog'": "{insert: [(2, 'PKGBUILD')]}",*

 * * "'check()'": "{insert: [(2, 'PKGBUILD')]}",*

 * * "'checkdepends'": "{insert: [(2, 'PKGBUILD')]}",*

 * * "'cksums'": "{insert: [(2, 'PKGBUILD')]}",*

 * * "'conflicts'": "{insert: [(2, 'PKGBUILD')]}",*

 * * "'depends'": "{insert: [(2, 'PKGBUILD')]}",*

 * * "'directory'": "{insert: [(2, 'PKGBUILD')]}",*

 * * "'epoch'": "{insert: [(2, 'PKGBUILD')]}",*

 * * "'fragment'" […]*

```diff
@@ -1,170 +1,212 @@
 {
     "arch": [
         "Field",
-        "Defines on which architectures the given package is available (e.g., arch=(i686 x86_64)). Packages that contain no architecture specific files should use arch=(any). Valid characters for members of this array are alphanumerics and \"\\_\"."
+        "Defines on which architectures the given package is available (e.g., arch=(i686 x86_64)). Packages that contain no architecture specific files should use arch=(any). Valid characters for members of this array are alphanumerics and \"\\_\".",
+        "PKGBUILD"
     ],
     "backup": [
         "Field",
-        "An array of file names, without preceding slashes, that should be backed up if the package is removed or upgraded. This is commonly used for packages placing configuration files in */etc*. See \\\"Handling Config Files\\\" in **pacman**(8) for more information."
+        "An array of file names, without preceding slashes, that should be backed up if the package is removed or upgraded. This is commonly used for packages placing configuration files in */etc*. See \\\"Handling Config Files\\\" in **pacman**(8) for more information.",
+        "PKGBUILD"
     ],
     "build()": [
         "Function",
-        "The optional build() function is used to compile and/or adjust the source files in preparation to be installed by the package() function."
+        "The optional build() function is used to compile and/or adjust the source files in preparation to be installed by the package() function.",
+        "PKGBUILD"
     ],
     "changelog": [
         "Variable",
-        "Specifies a changelog file that is to be included in the package. The changelog file should end in a single newline. This file should reside in the same directory as the PKGBUILD and will be copied into the package by makepkg. It does not need to be included in the source array (e.g., changelog=\\$pkgname.changelog)."
+        "Specifies a changelog file that is to be included in the package. The changelog file should end in a single newline. This file should reside in the same directory as the PKGBUILD and will be copied into the package by makepkg. It does not need to be included in the source array (e.g., changelog=\\$pkgname.changelog).",
+        "PKGBUILD"
     ],
     "check()": [
         "Function",
-        "An optional check() function can be specified in which a package's test-suite may be run. This function is run between the build() and package() functions. Be sure any exotic commands used are covered by the checkdepends array."
+        "An optional check() function can be specified in which a package's test-suite may be run. This function is run between the build() and package() functions. Be sure any exotic commands used are covered by the checkdepends array.",
+        "PKGBUILD"
     ],
     "checkdepends": [
         "Field",
-        "An array of packages this package depends on to run its test suite but are not needed at runtime. Packages in this list follow the same format as depends. These dependencies are only considered when the check() function is present and is to be run by makepkg.\nAdditional architecture-specific checkdepends can be added by appending an underscore and the architecture name e.g., *checkdepends_x86_64=()*."
+        "An array of packages this package depends on to run its test suite but are not needed at runtime. Packages in this list follow the same format as depends. These dependencies are only considered when the check() function is present and is to be run by makepkg.\nAdditional architecture-specific checkdepends can be added by appending an underscore and the architecture name e.g., *checkdepends_x86_64=()*.",
+        "PKGBUILD"
     ],
     "cksums": [
         "Field",
-        "This array contains CRC checksums for every source file specified in the source array (in the same order). makepkg will use this to verify source file integrity during subsequent builds. If *SKIP* is put in the array in place of a normal hash, the integrity check for that source file will be skipped. To easily generate cksums, run \"makepkg -g \\>\\> PKGBUILD\". If desired, move the cksums line to an appropriate location. Note that checksums generated by \\\"makepkg -g\\\" should be verified using checksum values provided by the software developer."
+        "This array contains CRC checksums for every source file specified in the source array (in the same order). makepkg will use this to verify source file integrity during subsequent builds. If *SKIP* is put in the array in place of a normal hash, the integrity check for that source file will be skipped. To easily generate cksums, run \"makepkg -g \\>\\> PKGBUILD\". If desired, move the cksums line to an appropriate location. Note that checksums generated by \\\"makepkg -g\\\" should be verified using checksum values provided by the software developer.",
+        "PKGBUILD"
     ],
     "conflicts": [
         "Field",
-        "An array of packages that will conflict with this package (i.e. they cannot both be installed at the same time). This directive follows the same format as depends. Versioned conflicts are supported using the operators as described in depends.\nAdditional architecture-specific conflicts can be added by appending an underscore and the architecture name e.g., *conflicts_x86_64=()*."
+        "An array of packages that will conflict with this package (i.e. they cannot both be installed at the same time). This directive follows the same format as depends. Versioned conflicts are supported using the operators as described in depends.\nAdditional architecture-specific conflicts can be added by appending an underscore and the architecture name e.g., *conflicts_x86_64=()*.",
+        "PKGBUILD"
     ],
     "depends": [
         "Field",
-        "An array of packages this package depends on to run. Entries in this list should be surrounded with single quotes and contain at least the package name. Entries can also include a version requirement of the form *name\\<\\>version*, where \\<\\> is one of five comparisons: \\>= (greater than or equal to), \\<= (less than or equal to), = (equal to), \\> (greater than), or \\< (less than).\nIf the dependency name appears to be a library (ends with .so), makepkg will try to find a binary that depends on the library in the built package and append the version needed by the binary. Appending the version yourself disables automatic detection.\nAdditional architecture-specific depends can be added by appending an underscore and the architecture name e.g., *depends_x86_64=()*."
+        "An array of packages this package depends on to run. Entries in this list should be surrounded with single quotes and contain at least the package name. Entries can also include a version requirement of the form *name\\<\\>version*, where \\<\\> is one of five comparisons: \\>= (greater than or equal to), \\<= (less than or equal to), = (equal to), \\> (greater than), or \\< (less than).\nIf the dependency name appears to be a library (ends with .so), makepkg will try to find a binary that depends on the library in the built package and append the version needed by the binary. Appending the version yourself disables automatic detection.\nAdditional architecture-specific depends can be added by appending an underscore and the architecture name e.g., *depends_x86_64=()*.",
+        "PKGBUILD"
     ],
     "directory": [
         "Variable",
-        "(optional) Specifies an alternate directory name for makepkg to download the VCS source into."
+        "(optional) Specifies an alternate directory name for makepkg to download the VCS source into.",
+        "PKGBUILD"
     ],
     "epoch": [
         "Variable",
-        "Used to force the package to be seen as newer than any previous versions with a lower epoch, even if the version number would normally not trigger such an upgrade. This value is required to be a positive integer; the default value if left unspecified is *0*. This is useful when the version numbering scheme of a package changes (or is alphanumeric), breaking normal version comparison logic. See **pacman**(8) for more information on version comparisons."
+        "Used to force the package to be seen as newer than any previous versions with a lower epoch, even if the version number would normally not trigger such an upgrade. This value is required to be a positive integer; the default value if left unspecified is *0*. This is useful when the version numbering scheme of a package changes (or is alphanumeric), breaking normal version comparison logic. See **pacman**(8) for more information on version comparisons.",
+        "PKGBUILD"
     ],
     "fragment": [
         "Variable",
-        "(optional) Allows specifying a revision number or branch for makepkg to checkout from the VCS. A fragment has the form type=value, for example to checkout a given revision the source line would be source=(url#revision=123). The available types depends on the VCS being used:\n**bzr**\nrevision (see bzr help revisionspec for details)"
+        "(optional) Allows specifying a revision number or branch for makepkg to checkout from the VCS. A fragment has the form type=value, for example to checkout a given revision the source line would be source=(url#revision=123). The available types depends on the VCS being used:\n**bzr**\nrevision (see bzr help revisionspec for details)",
+        "PKGBUILD"
     ],
     "groups": [
         "Field",
-        "An array of symbolic names that represent groups of packages, allowing you to install multiple packages by requesting a single target. For example, one could install all KDE packages by installing the *kde* group."
+        "An array of symbolic names that represent groups of packages, allowing you to install multiple packages by requesting a single target. For example, one could install all KDE packages by installing the *kde* group.",
+        "PKGBUILD"
     ],
     "install": [
         "Variable",
-        "Specifies a special install script that is to be included in the package. This file should reside in the same directory as the PKGBUILD and will be copied into the package by makepkg. It does not need to be included in the source array (e.g., install=\\$pkgname.install)."
+        "Specifies a special install script that is to be included in the package. This file should reside in the same directory as the PKGBUILD and will be copied into the package by makepkg. It does not need to be included in the source array (e.g., install=\\$pkgname.install).",
+        "PKGBUILD"
     ],
     "license": [
         "Field",
-        "This field specifies the license(s) that apply to the package. Commonly used licenses can be found in */usr/share/licenses/common*. If you see the package's license there, simply reference it in the license field (e.g., license=(GPL)). If the package provides a license not available in */usr/share/licenses/common*, then you should include it in the package itself and set license=(custom) or license=(custom:LicenseName). The license should be placed in *\\$pkgdir/usr/share/licenses/\\$pkgname/* when building the package. If multiple licenses are applicable, list all of them: license=(GPL FDL)."
+        "This field specifies the license(s) that apply to the package. Commonly used licenses can be found in */usr/share/licenses/common*. If you see the package's license there, simply reference it in the license field (e.g., license=(GPL)). If the package provides a license not available in */usr/share/licenses/common*, then you should include it in the package itself and set license=(custom) or license=(custom:LicenseName). The license should be placed in *\\$pkgdir/usr/share/licenses/\\$pkgname/* when building the package. If multiple licenses are applicable, list all of them: license=(GPL FDL).",
+        "PKGBUILD"
     ],
     "makedepends": [
         "Field",
-        "An array of packages this package depends on to build but are not needed at runtime. Packages in this list follow the same format as depends.\nAdditional architecture-specific makedepends can be added by appending an underscore and the architecture name e.g., *makedepends_x86_64=()*."
+        "An array of packages this package depends on to build but are not needed at runtime. Packages in this list follow the same format as depends.\nAdditional architecture-specific makedepends can be added by appending an underscore and the architecture name e.g., *makedepends_x86_64=()*.",
+        "PKGBUILD"
     ],
     "md5sums,": [
         "sha1sums,",
-        "Alternative integrity checks that makepkg supports; these all behave similar to the cksums option described above. To enable use and generation of these checksums, be sure to set up the INTEGRITY_CHECK option in **makepkg.conf**(5)."
+        "Alternative integrity checks that makepkg supports; these all behave similar to the cksums option described above. To enable use and generation of these checksums, be sure to set up the INTEGRITY_CHECK option in **makepkg.conf**(5).",
+        "PKGBUILD"
     ],
     "noextract": [
         "Field",
-        "An array of file names corresponding to those from the source array. Files listed here will not be extracted with the rest of the source files. This is useful for packages that use compressed data directly."
+        "An array of file names corresponding to those from the source array. Files listed here will not be extracted with the rest of the source files. This is useful for packages that use compressed data directly.",
+        "PKGBUILD"
     ],
     "optdepends": [
         "Field",
-        "An array of packages (and accompanying reasons) that are not essential for base functionality, but may be necessary to make full use of the contents of this package. optdepends are currently for informational purposes only and are not utilized by pacman during dependency resolution. Packages in this list follow the same format as depends, with an optional description appended. The format for specifying optdepends descriptions is:\noptdepends=(python: for library bindings) "
+        "An array of packages (and accompanying reasons) that are not essential for base functionality, but may be necessary to make full use of the contents of this package. optdepends are currently for informational purposes only and are not utilized by pacman during dependency resolution. Packages in this list follow the same format as depends, with an optional description appended. The format for specifying optdepends descriptions is:\noptdepends=(python: for library bindings) ",
+        "PKGBUILD"
     ],
     "options": [
         "Field",
-        "This array allows you to override some of makepkg's default behavior when building packages. To set an option, just include the option name in the options array. To reverse the default behavior, place an \"!\" at the front of the option. Only specify the options you specifically want to override, the rest will be taken from **makepkg.conf**(5). **NOTE:** *force* is a now-removed option in favor of the top level *epoch* variable.\n**strip**\nStrip symbols from binaries and libraries. If you frequently use a debugger on programs or libraries, it may be helpful to disable this option."
+        "This array allows you to override some of makepkg's default behavior when building packages. To set an option, just include the option name in the options array. To reverse the default behavior, place an \"!\" at the front of the option. Only specify the options you specifically want to override, the rest will be taken from **makepkg.conf**(5). **NOTE:** *force* is a now-removed option in favor of the top level *epoch* variable.\n**strip**\nStrip symbols from binaries and libraries. If you frequently use a debugger on programs or libraries, it may be helpful to disable this option.",
+        "PKGBUILD"
     ],
     "package()": [
         "Function",
-        "The package() function is used to install files into the directory that will become the root directory of the built package and is run after all the optional functions listed below. The packaging stage is run using fakeroot to ensure correct file permissions in the resulting package. All other functions will be run as the user calling makepkg."
+        "The package() function is used to install files into the directory that will become the root directory of the built package and is run after all the optional functions listed below. The packaging stage is run using fakeroot to ensure correct file permissions in the resulting package. All other functions will be run as the user calling makepkg.",
+        "PKGBUILD"
     ],
     "pkgbase": [
         "Variable",
-        "The name used to refer to the group of packages in the output of makepkg and in the naming of source-only tarballs. If not specified, the first element in the pkgname array is used. Valid characters for this variable are alphanumerics, and any of the following characters: \"@ . \\_ + -\". Additionally, the variable is not allowed to start with hyphens or dots."
+        "The name used to refer to the group of packages in the output of makepkg and in the naming of source-only tarballs. If not specified, the first element in the pkgname array is used. Valid characters for this variable are alphanumerics, and any of the following characters: \"@ . \\_ + -\". Additionally, the variable is not allowed to start with hyphens or dots.",
+        "PKGBUILD"
     ],
     "pkgdesc": [
         "Variable",
-        "This should be a brief description of the package and its functionality. Try to keep the description to one line of text and to not use the package's name."
+        "This should be a brief description of the package and its functionality. Try to keep the description to one line of text and to not use the package's name.",
+        "PKGBUILD"
     ],
     "pkgdir": [
         "Variable",
-        "This contains the directory where makepkg bundles the installed package. This directory will become the root directory of your built package. This variable should only be used in the package() function."
+        "This contains the directory where makepkg bundles the installed package. This directory will become the root directory of your built package. This variable should only be used in the package() function.",
+        "PKGBUILD"
     ],
     "pkgname": [
         "Field",
-        "Either the name of the package or an array of names for split packages. Valid characters for members of this array are alphanumerics, and any of the following characters: \"@ . \\_ + -\". Additionally, names are not allowed to start with hyphens or dots."
+        "Either the name of the package or an array of names for split packages. Valid characters for members of this array are alphanumerics, and any of the following characters: \"@ . \\_ + -\". Additionally, names are not allowed to start with hyphens or dots.",
+        "PKGBUILD"
     ],
     "pkgrel": [
         "Variable",
-        "This is the release number specific to the distribution. This allows package maintainers to make updates to the package's configure flags, for example. This is typically set to *1* for each new upstream software release and incremented for intermediate PKGBUILD updates. The variable is a positive integer, with an optional subrelease level specified by adding another positive integer separated by a period (i.e. in the form x.y)."
+        "This is the release number specific to the distribution. This allows package maintainers to make updates to the package's configure flags, for example. This is typically set to *1* for each new upstream software release and incremented for intermediate PKGBUILD updates. The variable is a positive integer, with an optional subrelease level specified by adding another positive integer separated by a period (i.e. in the form x.y).",
+        "PKGBUILD"
     ],
     "pkgver": [
         "Variable",
-        "The version of the software as released from the author (e.g., *2.7.1*). The variable is not allowed to contain colons, forward slashes, hyphens or whitespace.\nThe pkgver variable can be automatically updated by providing a pkgver() function in the PKGBUILD that outputs the new package version. This is run after downloading and extracting the sources and running the prepare() function (if present), so it can use those files in determining the new pkgver. This is most useful when used with sources from version control systems (see below)."
+        "The version of the software as released from the author (e.g., *2.7.1*). The variable is not allowed to contain colons, forward slashes, hyphens or whitespace.\nThe pkgver variable can be automatically updated by providing a pkgver() function in the PKGBUILD that outputs the new package version. This is run after downloading and extracting the sources and running the prepare() function (if present), so it can use those files in determining the new pkgver. This is most useful when used with sources from version control systems (see below).",
+        "PKGBUILD"
     ],
-    "post_install": [
-        "Variable",
-        "Run right after files are extracted. One argument is passed: new package full version string."
+    "post_install()": [
+        "Function",
+        "Run right after files are extracted. One argument is passed: new package full version string.",
+        "install"
     ],
-    "post_remove": [
-        "Variable",
-        "Run right after files are removed. One argument is passed: old package full version string."
+    "post_remove()": [
+        "Function",
+        "Run right after files are removed. One argument is passed: old package full version string.",
+        "install"
     ],
-    "post_upgrade": [
-        "Variable",
-        "Run after files are extracted. Two arguments are passed in this order: new package full version string, old package full version string."
+    "post_upgrade()": [
+        "Function",
+        "Run after files are extracted. Two arguments are passed in this order: new package full version string, old package full version string.",
+        "install"
     ],
-    "pre_install": [
-        "Variable",
-        "Run right before files are extracted. One argument is passed: new package full version string."
+    "pre_install()": [
+        "Function",
+        "Run right before files are extracted. One argument is passed: new package full version string.",
+        "install"
     ],
-    "pre_remove": [
-        "Variable",
-        "Run right before files are removed. One argument is passed: old package full version string."
+    "pre_remove()": [
+        "Function",
+        "Run right before files are removed. One argument is passed: old package full version string.",
+        "install"
     ],
-    "pre_upgrade": [
-        "Variable",
-        "Run right before files are extracted. Two arguments are passed in this order: new package full version string, old package full version string."
+    "pre_upgrade()": [
+        "Function",
+        "Run right before files are extracted. Two arguments are passed in this order: new package full version string, old package full version string.",
+        "install"
     ],
     "prepare()": [
         "Function",
-        "An optional prepare() function can be specified in which operations to prepare the sources for building, such as patching, are performed. This function is run after the source extraction and before the build() function. The prepare() function is skipped when source extraction is skipped."
+        "An optional prepare() function can be specified in which operations to prepare the sources for building, such as patching, are performed. This function is run after the source extraction and before the build() function. The prepare() function is skipped when source extraction is skipped.",
+        "PKGBUILD"
     ],
     "provides": [
         "Field",
-        "An array of \"virtual provisions\" this package provides. This allows a package to provide dependencies other than its own package name. For example, the dcron package can provide *cron*, which allows packages to depend on *cron* rather than *dcron OR fcron*.\nVersioned provisions are also possible, in the *name=version* format. For example, dcron can provide *cron=2.0* to satisfy the *cron\\>=2.0* dependency of other packages. Provisions involving the \\> and \\< operators are invalid as only specific versions of a package may be provided.\nIf the provision name appears to be a library (ends with .so), makepkg will try to find the library in the built package and append the correct version. Appending the version yourself disables automatic detection.\nAdditional architecture-specific provides can be added by appending an underscore and the architecture name e.g., *provides_x86_64=()*."
+        "An array of \"virtual provisions\" this package provides. This allows a package to provide dependencies other than its own package name. For example, the dcron package can provide *cron*, which allows packages to depend on *cron* rather than *dcron OR fcron*.\nVersioned provisions are also possible, in the *name=version* format. For example, dcron can provide *cron=2.0* to satisfy the *cron\\>=2.0* dependency of other packages. Provisions involving the \\> and \\< operators are invalid as only specific versions of a package may be provided.\nIf the provision name appears to be a library (ends with .so), makepkg will try to find the library in the built package and append the correct version. Appending the version yourself disables automatic detection.\nAdditional architecture-specific provides can be added by appending an underscore and the architecture name e.g., *provides_x86_64=()*.",
+        "PKGBUILD"
     ],
     "query": [
         "Variable",
-        "(optional) Allows specifying whether a VCS checkout should be checked for PGP-signed revisions. The source line should have the format source=(url#fragment?signed) or source=(url?signed#fragment). Currently only supported by Git."
+        "(optional) Allows specifying whether a VCS checkout should be checked for PGP-signed revisions. The source line should have the format source=(url#fragment?signed) or source=(url?signed#fragment). Currently only supported by Git.",
+        "PKGBUILD"
     ],
     "replaces": [
         "Field",
-        "An array of packages this package should replace. This can be used to handle renamed/combined packages. For example, if the *j2re* package is renamed to *jre*, this directive allows future upgrades to continue as expected even though the package has moved. Versioned replaces are supported using the operators as described in depends.\nSysupgrade is currently the only pacman operation that utilizes this field. A normal sync or upgrade will not use its value.\nAdditional architecture-specific replaces can be added by appending an underscore and the architecture name e.g., *replaces_x86_64=()*."
+        "An array of packages this package should replace. This can be used to handle renamed/combined packages. For example, if the *j2re* package is renamed to *jre*, this directive allows future upgrades to continue as expected even though the package has moved. Versioned replaces are supported using the operators as described in depends.\nSysupgrade is currently the only pacman operation that utilizes this field. A normal sync or upgrade will not use its value.\nAdditional architecture-specific replaces can be added by appending an underscore and the architecture name e.g., *replaces_x86_64=()*.",
+        "PKGBUILD"
     ],
     "source": [
         "Field",
-        "An array of source files required to build the package. Source files must either reside in the same directory as the PKGBUILD, or be a fully-qualified URL that makepkg can use to download the file. To simplify the maintenance of PKGBUILDs, use the \\$pkgname and \\$pkgver variables when specifying the download location, if possible. Compressed files will be extracted automatically unless found in the noextract array described below.\nAdditional architecture-specific sources can be added by appending an underscore and the architecture name e.g., *source_x86_64=()*. There must be a corresponding integrity array with checksums, e.g. *cksums_x86_64=()*.\nIt is also possible to change the name of the downloaded file, which is helpful with weird URLs and for handling multiple source files with the same name. The syntax is: source=(filename::url).\nmakepkg also supports building developmental versions of packages using sources downloaded from version control systems (VCS). For more information, see Using VCS Sources below.\nFiles in the source array with extensions .sig, .sign or, .asc are recognized by makepkg as PGP signatures and will be automatically used to verify the integrity of the corresponding source file."
+        "An array of source files required to build the package. Source files must either reside in the same directory as the PKGBUILD, or be a fully-qualified URL that makepkg can use to download the file. To simplify the maintenance of PKGBUILDs, use the \\$pkgname and \\$pkgver variables when specifying the download location, if possible. Compressed files will be extracted automatically unless found in the noextract array described below.\nAdditional architecture-specific sources can be added by appending an underscore and the architecture name e.g., *source_x86_64=()*. There must be a corresponding integrity array with checksums, e.g. *cksums_x86_64=()*.\nIt is also possible to change the name of the downloaded file, which is helpful with weird URLs and for handling multiple source files with the same name. The syntax is: source=(filename::url).\nmakepkg also supports building developmental versions of packages using sources downloaded from version control systems (VCS). For more information, see Using VCS Sources below.\nFiles in the source array with extensions .sig, .sign or, .asc are recognized by makepkg as PGP signatures and will be automatically used to verify the integrity of the corresponding source file.",
+        "PKGBUILD"
     ],
     "srcdir": [
         "Variable",
-        "This contains the directory where makepkg extracts, or copies, all source files.\nAll of the packaging functions defined above are run starting inside \\$srcdir"
+        "This contains the directory where makepkg extracts, or copies, all source files.\nAll of the packaging functions defined above are run starting inside \\$srcdir",
+        "PKGBUILD"
     ],
     "startdir": [
         "Variable",
-        "This contains the absolute path to the directory where the PKGBUILD is located, which is usually the output of \\$(pwd) when makepkg is started. Use of this variable is deprecated and strongly discouraged."
+        "This contains the absolute path to the directory where the PKGBUILD is located, which is usually the output of \\$(pwd) when makepkg is started. Use of this variable is deprecated and strongly discouraged.",
+        "PKGBUILD"
     ],
     "url": [
         "Variable",
-        "The URL to the VCS repository. This must include the VCS in the URL protocol for makepkg to recognize this as a VCS source. If the protocol does not include the VCS name, it can be added by prefixing the URL with vcs+. For example, using a Git repository over HTTPS would have a source URL in the form: git+https://\\...."
+        "The URL to the VCS repository. This must include the VCS in the URL protocol for makepkg to recognize this as a VCS source. If the protocol does not include the VCS name, it can be added by prefixing the URL with vcs+. For example, using a Git repository over HTTPS would have a source URL in the form: git+https://\\....",
+        "PKGBUILD"
     ],
     "validpgpkeys": [
         "Field",
-        "An array of PGP fingerprints. If this array is non-empty, makepkg will only accept signatures from the keys listed here and will ignore the trust values from the keyring. If the source file was signed with a subkey, makepkg will still use the primary key for comparison.\nOnly full fingerprints are accepted. They must be uppercase and must not contain whitespace characters."
+        "An array of PGP fingerprints. If this array is non-empty, makepkg will only accept signatures from the keys listed here and will ignore the trust values from the keyring. If the source file was signed with a subkey, makepkg will still use the primary key for comparison.\nOnly full fingerprints are accepted. They must be uppercase and must not contain whitespace characters.",
+        "PKGBUILD"
     ]
 }
```

### Comparing `pkgbuild-language-server-0.0.1/src/pkgbuild_language_server/server.py` & `pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,39 +22,40 @@
     Range,
     TextDocumentPositionParams,
 )
 from platformdirs import user_cache_dir
 from pygls.server import LanguageServer
 
 
-def check_extension(uri: str) -> bool:
+def check_extension(uri: str) -> Literal["install", "PKGBUILD", ""]:
     r"""Check extension.
 
     :param uri:
     :type uri: str
-    :rtype: bool
+    :rtype: Literal["install", "PKGBUILD", ""]
     """
-    return (
-        uri.split(os.path.extsep)[-1] == "install"
-        or os.path.basename(uri) == "PKGBUILD"
-    )
+    if uri.split(os.path.extsep)[-1] == "install":
+        return "install"
+    if os.path.basename(uri) == "PKGBUILD":
+        return "PKGBUILD"
+    return ""
 
 
 def get_document(
     method: Literal["builtin", "cache", "system"] = "builtin"
-) -> dict[str, tuple[str, str]]:
+) -> dict[str, tuple[str, str, str]]:
     r"""Get document. ``builtin`` will use builtin pkgbuild.json. ``cache``
     will generate a cache from ``${XDG_CACHE_DIRS:-/usr/share}
     /info/pkgbuild.info.gz``. ``system`` is same as ``cache`` except it doesn't
     generate cache. Some distribution's pkgbuild doesn't contain textinfo. So
     we use ``builtin`` as default.
 
     :param method:
     :type method: Literal["builtin", "cache", "system"]
-    :rtype: dict[str, tuple[str, str]]
+    :rtype: dict[str, tuple[str, str, str]]
     """
     if method == "builtin":
         file = os.path.join(
             os.path.join(
                 os.path.join(os.path.dirname(__file__), "assets"), "json"
             ),
             "pkgbuild.json",
@@ -131,29 +132,29 @@
         def completions(params: CompletionParams) -> CompletionList:
             r"""Completions.
 
             :param params:
             :type params: CompletionParams
             :rtype: CompletionList
             """
-            if not check_extension(params.text_document.uri):
-                return CompletionList(is_incomplete=False, items=[])
             word = self._cursor_word(
                 params.text_document.uri, params.position, False
             )
             token = "" if word is None else word[0]
             items = [
                 CompletionItem(
                     label=x,
                     kind=getattr(CompletionItemKind, self.document[x][0]),
                     documentation=self.document[x][1],
                     insert_text=x,
                 )
                 for x in self.document
                 if x.startswith(token)
+                and self.document[x][2]
+                == check_extension(params.text_document.uri)
             ]
             return CompletionList(is_incomplete=False, items=items)
 
     def _cursor_line(self, uri: str, position: Position) -> str:
         r"""Cursor line.
 
         :param uri:
@@ -176,23 +177,27 @@
         :type uri: str
         :param position:
         :type position: Position
         :param include_all:
         :type include_all: bool
         :rtype: Tuple[str, Range] | None
         """
+        if check_extension(uri) == "PKGBUILD":
+            # PKGBUILD contains package_XXX
+            pat = r"[a-z]+"
+        else:
+            # *.install contains pre_install()
+            pat = r"[a-z_]+"
         line = self._cursor_line(uri, position)
         cursor = position.character
-        for m in re.finditer(r"[a-z]+", line):
+        for m in re.finditer(pat, line):
             end = m.end() if include_all else cursor
             if m.start() <= cursor <= m.end():
                 word = (
                     line[m.start() : end],
                     Range(
-                        start=Position(
-                            line=position.line, character=m.start()
-                        ),
-                        end=Position(line=position.line, character=end),
+                        Position(position.line, m.start()),
+                        Position(position.line, end),
                     ),
                 )
                 return word
         return None
```

### Comparing `pkgbuild-language-server-0.0.1/src/pkgbuild_language_server.egg-info/PKG-INFO` & `pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgbuild-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: pkgbuild language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://pkgbuild-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/pkgbuild-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/pkgbuild-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/pkgbuild-language-server
@@ -66,15 +66,17 @@
 [![pypi/status](https://shields.io/pypi/status/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#description)
 [![pypi/v](https://shields.io/pypi/v/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#history)
 [![pypi/downloads](https://shields.io/pypi/dd/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/format](https://shields.io/pypi/format/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 
-Language server for [PKGBUILD](https://wiki.archlinux.org/title/PKGBUILD).
+Language server for [ArchLinux](https://archlinux.org)/[Windows Msys2](https://msys2.org)'s
+[PKGBUILD](https://wiki.archlinux.org/title/PKGBUILD) and
+[`*.install`](https://wiki.archlinux.org/title/PKGBUILD#install)
 
 PKGBUILD is a subtype of bash. See
 [bash-language-server](https://github.com/bash-lsp/bash-language-server) to get
 support of bash language server.
 
 - [x] document hover
 - [x] completion
```

### Comparing `pkgbuild-language-server-0.0.1/src/pkgbuild_language_server.egg-info/SOURCES.txt` & `pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

