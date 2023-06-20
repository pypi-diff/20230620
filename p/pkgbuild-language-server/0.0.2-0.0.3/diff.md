# Comparing `tmp/pkgbuild-language-server-0.0.2.tar.gz` & `tmp/pkgbuild-language-server-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgbuild-language-server-0.0.2.tar", last modified: Tue Jun 20 08:14:37 2023, max compression
+gzip compressed data, was "pkgbuild-language-server-0.0.3.tar", last modified: Tue Jun 20 10:47:28 2023, max compression
```

## Comparing `pkgbuild-language-server-0.0.2.tar` & `pkgbuild-language-server-0.0.3.tar`

### file list

```diff
@@ -1,55 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.675552 pkgbuild-language-server-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.663552 pkgbuild-language-server-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.667552 pkgbuild-language-server-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-20 08:14:37.675552 pkgbuild-language-server-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.667552 pkgbuild-language-server-0.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.667552 pkgbuild-language-server-0.0.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/docs/api/pkgbuild-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.667552 pkgbuild-language-server-0.0.2/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.667552 pkgbuild-language-server-0.0.2/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/requirements/cache.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.667552 pkgbuild-language-server-0.0.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/scripts/generate-api.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:14:37.675552 pkgbuild-language-server-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.659551 pkgbuild-language-server-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.671552 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.659551 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.671552 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/assets/json/pkgbuild.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.671552 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 08:14:37.000000 pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.675552 pkgbuild-language-server-0.0.2/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:14:37.675552 pkgbuild-language-server-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 08:14:27.000000 pkgbuild-language-server-0.0.2/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.017107 pkgbuild-language-server-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-20 10:47:28.017107 pkgbuild-language-server-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/docs/api/pkgbuild-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/requirements/cache.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/requirements/package.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/scripts/generate-api.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:47:28.017107 pkgbuild-language-server-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.009107 pkgbuild-language-server-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 10:47:27.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.009107 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/jinja2/template.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.017107 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/json/pkgbuild.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-20 10:47:27.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-20 10:47:28.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:47:27.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:47:27.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 10:47:27.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 10:47:27.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.017107 pkgbuild-language-server-0.0.3/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.017107 pkgbuild-language-server-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/tests/server_test.py
```

### Comparing `pkgbuild-language-server-0.0.2/.github/workflows/main.yml` & `pkgbuild-language-server-0.0.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.2/.gitignore` & `pkgbuild-language-server-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.2/.pre-commit-config.yaml` & `pkgbuild-language-server-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.2/LICENSE` & `pkgbuild-language-server-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.2/PKG-INFO` & `pkgbuild-language-server-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgbuild-language-server
-Version: 0.0.2
+Version: 0.0.3
 Summary: pkgbuild language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://pkgbuild-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/pkgbuild-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/pkgbuild-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/pkgbuild-language-server
@@ -68,23 +68,31 @@
 [![pypi/downloads](https://shields.io/pypi/dd/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/format](https://shields.io/pypi/format/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 
 Language server for [ArchLinux](https://archlinux.org)/[Windows Msys2](https://msys2.org)'s
 [PKGBUILD](https://wiki.archlinux.org/title/PKGBUILD) and
-[`*.install`](https://wiki.archlinux.org/title/PKGBUILD#install)
+[`*.install`](https://wiki.archlinux.org/title/PKGBUILD#install).
 
 PKGBUILD is a subtype of bash. See
 [bash-language-server](https://github.com/bash-lsp/bash-language-server) to get
 support of bash language server.
 
 - [x] document hover
 - [x] completion
 
-![document hover](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/91bfde00-28f7-4376-8b7a-10a0bd56ba51)
+## Document hover
 
-![completion](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/b4444ba5-44ab-473c-9691-b3d61ed09acd)
+![keyword](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/91bfde00-28f7-4376-8b7a-10a0bd56ba51)
+
+![package](https://github.com/Freed-Wu/pkgbuild-language-server/assets/32936898/3d9fa906-35ea-4063-a9eb-06282d3e8596)
+
+## Completion
+
+![keyword](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/b4444ba5-44ab-473c-9691-b3d61ed09acd)
+
+![package](https://github.com/Freed-Wu/pkgbuild-language-server/assets/32936898/090dae36-52fe-47f9-ae2d-cd3256cb55e8)
 
 Read
 [![readthedocs](https://shields.io/readthedocs/pkgbuild-language-server)](https://pkgbuild-language-server.readthedocs.io)
 to know more.
```

### Comparing `pkgbuild-language-server-0.0.2/README.md` & `pkgbuild-language-server-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -35,23 +35,31 @@
 [![pypi/downloads](https://shields.io/pypi/dd/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/format](https://shields.io/pypi/format/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 
 Language server for [ArchLinux](https://archlinux.org)/[Windows Msys2](https://msys2.org)'s
 [PKGBUILD](https://wiki.archlinux.org/title/PKGBUILD) and
-[`*.install`](https://wiki.archlinux.org/title/PKGBUILD#install)
+[`*.install`](https://wiki.archlinux.org/title/PKGBUILD#install).
 
 PKGBUILD is a subtype of bash. See
 [bash-language-server](https://github.com/bash-lsp/bash-language-server) to get
 support of bash language server.
 
 - [x] document hover
 - [x] completion
 
-![document hover](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/91bfde00-28f7-4376-8b7a-10a0bd56ba51)
+## Document hover
 
-![completion](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/b4444ba5-44ab-473c-9691-b3d61ed09acd)
+![keyword](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/91bfde00-28f7-4376-8b7a-10a0bd56ba51)
+
+![package](https://github.com/Freed-Wu/pkgbuild-language-server/assets/32936898/3d9fa906-35ea-4063-a9eb-06282d3e8596)
+
+## Completion
+
+![keyword](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/b4444ba5-44ab-473c-9691-b3d61ed09acd)
+
+![package](https://github.com/Freed-Wu/pkgbuild-language-server/assets/32936898/090dae36-52fe-47f9-ae2d-cd3256cb55e8)
 
 Read
 [![readthedocs](https://shields.io/readthedocs/pkgbuild-language-server)](https://pkgbuild-language-server.readthedocs.io)
 to know more.
```

### Comparing `pkgbuild-language-server-0.0.2/docs/conf.py` & `pkgbuild-language-server-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.2/docs/resources/configure.md` & `pkgbuild-language-server-0.0.3/docs/resources/configure.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,33 @@
 # Configure
 
 See customization in
 <https://pkgbuild-language-server.readthedocs.io/en/latest/api/pkgbuild-language-server.html#pkgbuild_language_server.server.get_document>.
 
+You can customize the document hover template. A default template is
+[here](https://github.com/Freed-Wu/pkgbuild-language-server/tree/main/src/pkgbuild_language_server/assets/jinja2/template.md.j2).
+The syntax rule is [jinja](https://docs.jinkan.org/docs/jinja2/templates.html).
+The template path is decided by your OS:
+
+```shell
+$ pkgbuild-language-server --print-config template
+/home/wzy/.config/pacman/template.md.j2
+```
+
+To complete package names, a cache is needed.
+Install [pyalpm](https://archlinux.org/packages/extra/x86_64/pyalpm)
+by `pip install 'pkgbuild-language-server[package]'` and then
+`pkgbuild-language-server --generate-cache`. Every time you change template,
+the cache must be regenerated.
+
+```shell
+$ pkgbuild-language-server --print-config cache
+/home/wzy/.cache/pacman.json
+```
+
 ## (Neo)[Vim](https://www.vim.org)
 
 ### [coc.nvim](https://github.com/neoclide/coc.nvim)
 
 ```json
 {
   "languageserver": {
```

### Comparing `pkgbuild-language-server-0.0.2/docs/resources/install.md` & `pkgbuild-language-server-0.0.3/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.2/flake.nix` & `pkgbuild-language-server-0.0.3/flake.nix`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.2/pyproject.toml` & `pkgbuild-language-server-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [build-system]
 # FIXME: setuptools-generate stop setuptools_scm working
 requires = [
   "setuptools_scm[toml] >= 6.2",
-  # "setuptools-generate >= 0.0.6"
+  # "setuptools-generate >= 0.0.6",
+  # "platformdirs",
 ]
 build-backend = "setuptools.build_meta"
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [project]
 name = "pkgbuild-language-server"
 description = "pkgbuild language server"
```

### Comparing `pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/__main__.py` & `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 r"""This module can be called by
 `python -m <https://docs.python.org/3/library/__main__.html>`_.
 """
+import logging
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from contextlib import suppress
 from datetime import datetime
 
+from . import CONFIG
 from . import __name__ as NAME
 from . import __version__
 
+logger = logging.getLogger(__name__)
 NAME = NAME.replace("_", "-")
 VERSION = rf"""{NAME} {__version__}
 Copyright (C) {datetime.now().year}
 Written by Wu Zhenyu
 """
 EPILOG = """
 Report bugs to <wuzhenyu@ustc.edu>.
@@ -21,25 +24,51 @@
 def get_parser():
     r"""Get a parser for unit test."""
     parser = ArgumentParser(
         epilog=EPILOG,
         formatter_class=RawDescriptionHelpFormatter,
     )
     parser.add_argument("--version", version=VERSION, action="version")
+    parser.add_argument(
+        "--print-config",
+        choices=["template", "cache", "all"],
+        help="print config value",
+    )
+    parser.add_argument(
+        "--generate-cache",
+        action="store_true",
+        help="generate cache for archlinux packages",
+    )
     with suppress(ImportError):
         import shtab
 
         shtab.add_argument_to(parser)
     return parser
 
 
 def main():
     r"""Parse arguments and provide shell completions."""
     parser = get_parser()
-    parser.parse_args()
+    args = parser.parse_args()
+    if args.print_config:
+        print(
+            CONFIG.get(
+                args.print_config,
+                "\n".join([k + ": " + v for k, v in CONFIG.items()]),
+            )
+        )
+        return None
+    if args.generate_cache:
+        from .package import generate_cache
+
+        try:
+            generate_cache()
+        except ImportError as e:
+            logger.error(f"Please install {e.name}!")
+        return None
 
     from .server import PKGBUILDLanguageServer
 
     PKGBUILDLanguageServer(NAME, __version__).start_io()
 
 
 if __name__ == "__main__":
```

### Comparing `pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/api.py` & `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/api.py`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/assets/json/pkgbuild.json` & `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/json/pkgbuild.json`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.2/src/pkgbuild_language_server/server.py` & `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     Position,
     Range,
     TextDocumentPositionParams,
 )
 from platformdirs import user_cache_dir
 from pygls.server import LanguageServer
 
+from . import CACHE
+
 
 def check_extension(uri: str) -> Literal["install", "PKGBUILD", ""]:
     r"""Check extension.
 
     :param uri:
     :type uri: str
     :rtype: Literal["install", "PKGBUILD", ""]
@@ -75,38 +77,53 @@
     else:
         from .api import init_document
 
         document = init_document()
     return document
 
 
+def get_packages() -> dict[str, str]:
+    r"""Get packages.
+
+    :rtype: dict[str, str]
+    """
+    try:
+        with open(CACHE, "r") as f:
+            packages = json.load(f)
+    except FileNotFoundError:
+        packages = {}
+    return packages
+
+
 class PKGBUILDLanguageServer(LanguageServer):
     r"""PKGBUILD language server."""
 
     def __init__(self, *args: Any) -> None:
         r"""Init.
 
         :param args:
         :type args: Any
         :rtype: None
         """
         super().__init__(*args)
         self.document = {}
+        self.packages = {}
 
         @self.feature(INITIALIZE)
         def initialize(params: InitializeParams) -> None:
             r"""Initialize.
 
             :param params:
             :type params: InitializeParams
             :rtype: None
             """
             opts = params.initialization_options
             method = getattr(opts, "method", "builtin")
             self.document = get_document(method)  # type: ignore
+            self.packages = get_packages()
 
         @self.feature(TEXT_DOCUMENT_HOVER)
         def hover(params: TextDocumentPositionParams) -> Hover | None:
             r"""Hover.
 
             :param params:
             :type params: TextDocumentPositionParams
@@ -114,18 +131,18 @@
             """
             if not check_extension(params.text_document.uri):
                 return None
             word = self._cursor_word(
                 params.text_document.uri, params.position, True
             )
             if not word:
-                return None
+                return self.hover(params)
             result = self.document.get(word[0])
             if not result:
-                return None
+                return self.hover(params)
             doc = f"**{result[0]}**\n{result[1]}"
             return Hover(
                 contents=MarkupContent(kind=MarkupKind.Markdown, value=doc),
                 range=word[1],
             )
 
         @self.feature(TEXT_DOCUMENT_COMPLETION)
@@ -133,29 +150,41 @@
             r"""Completions.
 
             :param params:
             :type params: CompletionParams
             :rtype: CompletionList
             """
             word = self._cursor_word(
-                params.text_document.uri, params.position, False
+                params.text_document.uri, params.position, False, True
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
                 and self.document[x][2]
                 == check_extension(params.text_document.uri)
             ]
+            items += [
+                CompletionItem(
+                    label=x,
+                    kind=CompletionItemKind.Module,
+                    documentation=MarkupContent(
+                        kind=MarkupKind.Markdown, value=self.packages[x]
+                    ),
+                    insert_text=x,
+                )
+                for x in self.packages
+                if x.startswith(token)
+            ]
             return CompletionList(is_incomplete=False, items=items)
 
     def _cursor_line(self, uri: str, position: Position) -> str:
         r"""Cursor line.
 
         :param uri:
         :type uri: str
@@ -165,39 +194,68 @@
         """
         doc = self.workspace.get_document(uri)
         content = doc.source
         line = content.split("\n")[position.line]
         return str(line)
 
     def _cursor_word(
-        self, uri: str, position: Position, include_all: bool = True
+        self,
+        uri: str,
+        position: Position,
+        include_all: bool = True,
+        package_name: bool = False,
     ) -> Tuple[str, Range] | None:
         r"""Cursor word.
 
         :param uri:
         :type uri: str
         :param position:
         :type position: Position
         :param include_all:
         :type include_all: bool
+        :param package_name:
+        :type package_name: bool
         :rtype: Tuple[str, Range] | None
         """
-        if check_extension(uri) == "PKGBUILD":
-            # PKGBUILD contains package_XXX
-            pat = r"[a-z]+"
+        if package_name:
+            pat = r"[-0-9_a-z]+"
         else:
-            # *.install contains pre_install()
-            pat = r"[a-z_]+"
+            if check_extension(uri) == "PKGBUILD":
+                # PKGBUILD contains package_XXX
+                pat = r"[a-z]+"
+            else:
+                # *.install contains pre_install()
+                pat = r"[a-z_]+"
         line = self._cursor_line(uri, position)
         cursor = position.character
         for m in re.finditer(pat, line):
             end = m.end() if include_all else cursor
             if m.start() <= cursor <= m.end():
                 word = (
                     line[m.start() : end],
                     Range(
                         Position(position.line, m.start()),
                         Position(position.line, end),
                     ),
                 )
                 return word
         return None
+
+    def hover(self, params: TextDocumentPositionParams) -> Hover | None:
+        r"""Hover.
+
+        :param params:
+        :type params: TextDocumentPositionParams
+        :rtype: Hover | None
+        """
+        word = self._cursor_word(
+            params.text_document.uri, params.position, True, True
+        )
+        if not word:
+            return None
+        doc = self.packages.get(word[0])
+        if not doc:
+            return None
+        return Hover(
+            contents=MarkupContent(kind=MarkupKind.Markdown, value=doc),
+            range=word[1],
+        )
```

### Comparing `pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/PKG-INFO` & `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgbuild-language-server
-Version: 0.0.2
+Version: 0.0.3
 Summary: pkgbuild language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://pkgbuild-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/pkgbuild-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/pkgbuild-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/pkgbuild-language-server
@@ -68,23 +68,31 @@
 [![pypi/downloads](https://shields.io/pypi/dd/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/format](https://shields.io/pypi/format/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/pkgbuild-language-server)](https://pypi.org/project/pkgbuild-language-server/#files)
 
 Language server for [ArchLinux](https://archlinux.org)/[Windows Msys2](https://msys2.org)'s
 [PKGBUILD](https://wiki.archlinux.org/title/PKGBUILD) and
-[`*.install`](https://wiki.archlinux.org/title/PKGBUILD#install)
+[`*.install`](https://wiki.archlinux.org/title/PKGBUILD#install).
 
 PKGBUILD is a subtype of bash. See
 [bash-language-server](https://github.com/bash-lsp/bash-language-server) to get
 support of bash language server.
 
 - [x] document hover
 - [x] completion
 
-![document hover](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/91bfde00-28f7-4376-8b7a-10a0bd56ba51)
+## Document hover
 
-![completion](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/b4444ba5-44ab-473c-9691-b3d61ed09acd)
+![keyword](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/91bfde00-28f7-4376-8b7a-10a0bd56ba51)
+
+![package](https://github.com/Freed-Wu/pkgbuild-language-server/assets/32936898/3d9fa906-35ea-4063-a9eb-06282d3e8596)
+
+## Completion
+
+![keyword](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/b4444ba5-44ab-473c-9691-b3d61ed09acd)
+
+![package](https://github.com/Freed-Wu/pkgbuild-language-server/assets/32936898/090dae36-52fe-47f9-ae2d-cd3256cb55e8)
 
 Read
 [![readthedocs](https://shields.io/readthedocs/pkgbuild-language-server)](https://pkgbuild-language-server.readthedocs.io)
 to know more.
```

### Comparing `pkgbuild-language-server-0.0.2/src/pkgbuild_language_server.egg-info/SOURCES.txt` & `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -14,25 +14,28 @@
 docs/index.md
 docs/requirements.txt
 docs/api/pkgbuild-language-server.md
 docs/resources/configure.md
 docs/resources/install.md
 requirements/cache.txt
 requirements/dev.txt
+requirements/package.txt
 scripts/generate-api.md.pl
 src/pkgbuild_language_server/__init__.py
 src/pkgbuild_language_server/__main__.py
 src/pkgbuild_language_server/_version.py
 src/pkgbuild_language_server/api.py
+src/pkgbuild_language_server/package.py
 src/pkgbuild_language_server/py.typed
 src/pkgbuild_language_server/server.py
 src/pkgbuild_language_server.egg-info/PKG-INFO
 src/pkgbuild_language_server.egg-info/SOURCES.txt
 src/pkgbuild_language_server.egg-info/dependency_links.txt
 src/pkgbuild_language_server.egg-info/entry_points.txt
 src/pkgbuild_language_server.egg-info/requires.txt
 src/pkgbuild_language_server.egg-info/top_level.txt
+src/pkgbuild_language_server/assets/jinja2/template.md.j2
 src/pkgbuild_language_server/assets/json/pkgbuild.json
 templates/class.txt
 templates/def.txt
 templates/noarg.txt
 tests/server_test.py
```

