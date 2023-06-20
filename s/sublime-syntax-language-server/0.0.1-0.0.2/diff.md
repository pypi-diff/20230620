# Comparing `tmp/sublime-syntax-language-server-0.0.1.tar.gz` & `tmp/sublime-syntax-language-server-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sublime-syntax-language-server-0.0.1.tar", last modified: Mon Jun 19 08:56:11 2023, max compression
+gzip compressed data, was "sublime-syntax-language-server-0.0.2.tar", last modified: Tue Jun 20 15:11:35 2023, max compression
```

## Comparing `sublime-syntax-language-server-0.0.1.tar` & `sublime-syntax-language-server-0.0.2.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.603760 sublime-syntax-language-server-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.599760 sublime-syntax-language-server-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.599760 sublime-syntax-language-server-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-06-19 08:56:11.603760 sublime-syntax-language-server-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.599760 sublime-syntax-language-server-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.599760 sublime-syntax-language-server-0.0.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/docs/api/sublime-syntax-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.599760 sublime-syntax-language-server-0.0.1/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.599760 sublime-syntax-language-server-0.0.1/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       49 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/requirements/web.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.599760 sublime-syntax-language-server-0.0.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/scripts/generate-api.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 08:56:11.603760 sublime-syntax-language-server-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.595760 sublime-syntax-language-server-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.599760 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 08:56:11.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.595760 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.603760 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/assets/json/sublime-syntax.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.599760 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-06-19 08:56:11.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-19 08:56:11.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:56:11.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-19 08:56:11.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 08:56:11.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-19 08:56:11.000000 sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.603760 sublime-syntax-language-server-0.0.1/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:11.603760 sublime-syntax-language-server-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/tests/Requirementstxt.sublime-syntax
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/tests/server_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-19 08:55:45.000000 sublime-syntax-language-server-0.0.1/tests/syntax_test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/api/sublime-syntax-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/requirements/web.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/scripts/generate-requirements.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.728149 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/assets/json/sublime-syntax.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 15:11:35.000000 sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:35.732149 sublime-syntax-language-server-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/tests/Requirementstxt.sublime-syntax
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/tests/server_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-20 15:11:23.000000 sublime-syntax-language-server-0.0.2/tests/syntax_test_requirements.txt
```

### Comparing `sublime-syntax-language-server-0.0.1/.github/workflows/main.yml` & `sublime-syntax-language-server-0.0.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.1/.gitignore` & `sublime-syntax-language-server-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.1/.pre-commit-config.yaml` & `sublime-syntax-language-server-0.0.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -64,21 +64,21 @@
           - mdformat-myst
           - mdformat-toc
           - mdformat-deflist
           - mdformat-beautysh
           - mdformat-black
           - mdformat-config
   - repo: https://github.com/DavidAnson/markdownlint-cli2
-    rev: v0.7.1
+    rev: v0.8.1
     hooks:
       - id: markdownlint-cli2
         additional_dependencies:
           - markdown-it-texmath@0.9.1
   - repo: https://github.com/perltidy/perltidy
-    rev: "20230309.02"
+    rev: "20230309.03"
     hooks:
       - id: perltidy
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/PyCQA/isort
@@ -88,15 +88,15 @@
   - repo: https://github.com/pycqa/pydocstyle
     rev: 6.3.0
     hooks:
       - id: pydocstyle
         additional_dependencies:
           - tomli
   - repo: https://github.com/kumaraditya303/mirrors-pyright
-    rev: v1.1.310
+    rev: v1.1.313
     hooks:
       - id: pyright
   - repo: https://github.com/PyCQA/bandit
     rev: 1.7.5
     hooks:
       - id: bandit
         args:
```

### Comparing `sublime-syntax-language-server-0.0.1/LICENSE` & `sublime-syntax-language-server-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.1/PKG-INFO` & `sublime-syntax-language-server-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sublime-syntax-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: sublime-syntax language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://sublime-syntax-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/sublime-syntax-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/sublime-syntax-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/sublime-syntax-language-server
```

### Comparing `sublime-syntax-language-server-0.0.1/README.md` & `sublime-syntax-language-server-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.1/docs/conf.py` & `sublime-syntax-language-server-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.1/docs/resources/configure.md` & `sublime-syntax-language-server-0.0.2/docs/resources/configure.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # Configure
 
-See customization in
-<https://sublime-syntax-language-server.readthedocs.io/en/latest/api/sublime-syntax-language-server.html#sublime_syntax_language_server.server.get_document>.
-
 ## (Neo)[Vim](https://www.vim.org)
 
 ### [coc.nvim](https://github.com/neoclide/coc.nvim)
 
 ```json
 {
   "languageserver": {
```

### Comparing `sublime-syntax-language-server-0.0.1/docs/resources/install.md` & `sublime-syntax-language-server-0.0.2/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.1/flake.nix` & `sublime-syntax-language-server-0.0.2/flake.nix`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.1/pyproject.toml` & `sublime-syntax-language-server-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/__main__.py` & `sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/api.py` & `sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/api.py`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/assets/json/sublime-syntax.json` & `sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/assets/json/sublime-syntax.json`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server/server.py` & `sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     TEXT_DOCUMENT_DID_OPEN,
     TEXT_DOCUMENT_HOVER,
     CompletionItem,
     CompletionItemKind,
     CompletionList,
     CompletionParams,
     Diagnostic,
+    DiagnosticSeverity,
     DidChangeTextDocumentParams,
     Hover,
     InitializeParams,
     MarkupContent,
     MarkupKind,
     Position,
     Range,
@@ -30,45 +31,42 @@
 from platformdirs import user_cache_dir
 from pygls.server import LanguageServer
 
 # https://github.com/iamcco/coc-diagnostic/pull/136/files
 PAT = 'Assertion selector "[^"]+" from line (\\d+) failed against line \\d+, column range (\\d+)-(\\d+) \\(with text "[^"]+"\\) has scope \\[([^\\]]+)\\]'
 
 
-def check_extension(uri: str) -> str:
+def check_extension(uri: str) -> Literal["sublime-syntax", "syntax_test", ""]:
     r"""Check extension.
 
     :param uri:
     :type uri: str
-    :rtype: str
+    :rtype: Literal["sublime-syntax", "syntax_test", ""]
     """
     if uri.split(os.path.extsep)[-1] == "sublime-syntax":
         return "sublime-syntax"
     if os.path.basename(uri).startswith("syntax_test_"):
         return "syntax_test"
     return ""
 
 
 def diagnostic(
-    uri: str, syntax_path: str = "."
+    path: str, syntax_path: str = "."
 ) -> dict[tuple[int, int, int], str]:
     r"""Diagnostic.
 
-    :param uri:
-    :type uri: str
+    :param path:
+    :type path: str
     :param syntax_path:
     :type syntax_path: str
     :rtype: dict[tuple[int, int, int], str]
     """
-    filename = uri.strip("file://")
-    if filename == uri:
-        return {}
     try:
         check_output(  # nosec: B603 B607
-            ["syntest", filename, syntax_path], universal_newlines=True
+            ["syntest", path, syntax_path], universal_newlines=True
         )
         return {}
     except CalledProcessError as e:
         lines = e.output.splitlines()
     results = {}
     for line in lines:
         m = re.match(PAT, line.strip())
@@ -199,29 +197,30 @@
         def did_change(params: DidChangeTextDocumentParams) -> None:
             r"""Did change.
 
             :param params:
             :type params: DidChangeTextDocumentParams
             :rtype: None
             """
-            text_doc = self.workspace.get_document(params.text_document.uri)
+            doc = self.workspace.get_document(params.text_document.uri)
+            if doc.path is None:
+                return None
             diagnostics = [
                 Diagnostic(
                     range=Range(
                         Position(line, col),
                         Position(line, endcol),
                     ),
                     message=msg,
+                    severity=DiagnosticSeverity.Error,
                     source="pip-compile",
                 )
-                for (line, col, endcol), msg in diagnostic(
-                    params.text_document.uri
-                ).items()
+                for (line, col, endcol), msg in diagnostic(doc.path).items()
             ]
-            self.publish_diagnostics(text_doc.uri, diagnostics)
+            self.publish_diagnostics(doc.uri, diagnostics)
 
     def _cursor_line(self, uri: str, position: Position) -> str:
         r"""Cursor line.
 
         :param uri:
         :type uri: str
         :param position:
```

### Comparing `sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server.egg-info/PKG-INFO` & `sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sublime-syntax-language-server
-Version: 0.0.1
+Version: 0.0.2
 Summary: sublime-syntax language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://sublime-syntax-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/sublime-syntax-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/sublime-syntax-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/sublime-syntax-language-server
```

### Comparing `sublime-syntax-language-server-0.0.1/src/sublime_syntax_language_server.egg-info/SOURCES.txt` & `sublime-syntax-language-server-0.0.2/src/sublime_syntax_language_server.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 .github/workflows/main.yml
 docs/conf.py
 docs/index.md
 docs/requirements.txt
 docs/api/sublime-syntax-language-server.md
 docs/resources/configure.md
 docs/resources/install.md
+docs/resources/requirements.md
 requirements/dev.txt
 requirements/web.txt
 scripts/generate-api.md.pl
+scripts/generate-requirements.md.pl
 src/sublime_syntax_language_server/__init__.py
 src/sublime_syntax_language_server/__main__.py
 src/sublime_syntax_language_server/_version.py
 src/sublime_syntax_language_server/api.py
 src/sublime_syntax_language_server/py.typed
 src/sublime_syntax_language_server/server.py
 src/sublime_syntax_language_server.egg-info/PKG-INFO
```

### Comparing `sublime-syntax-language-server-0.0.1/tests/Requirementstxt.sublime-syntax` & `sublime-syntax-language-server-0.0.2/tests/Requirementstxt.sublime-syntax`

 * *Files identical despite different names*

### Comparing `sublime-syntax-language-server-0.0.1/tests/server_test.py` & `sublime-syntax-language-server-0.0.2/tests/server_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from shutil import which
 
 import pytest
 
 from sublime_syntax_language_server.server import diagnostic, get_document
 
-URI = "file://" + "syntax_test_requirements.txt"
+PATH = "syntax_test_requirements.txt"
 
 
 class Test:
     r"""Test."""
 
     @staticmethod
     def test_get_document() -> None:
@@ -26,15 +26,15 @@
     )
     def test_diagnostic() -> None:
         r"""Test diagnostic.
 
         :rtype: None
         """
         os.chdir(os.path.dirname(__file__))
-        result = diagnostic(URI)
+        result = diagnostic(PATH)
         expected = {
             (
                 "82",
                 "48",
                 "58",
             ): "<source.requirements-txt>, <markup.underline.link.url.requirements-txt>"
         }
```

### Comparing `sublime-syntax-language-server-0.0.1/tests/syntax_test_requirements.txt` & `sublime-syntax-language-server-0.0.2/tests/syntax_test_requirements.txt`

 * *Files identical despite different names*

