# Comparing `tmp/requirements-language-server-0.0.2.tar.gz` & `tmp/requirements-language-server-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirements-language-server-0.0.2.tar", last modified: Sun Jun 18 17:24:24 2023, max compression
+gzip compressed data, was "requirements-language-server-0.0.3.tar", last modified: Tue Jun 20 15:11:55 2023, max compression
```

## Comparing `requirements-language-server-0.0.2.tar` & `requirements-language-server-0.0.3.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/docs/api/requirements-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/scripts/generate-api.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/src/requirements_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/src/requirements_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/src/requirements_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/src/requirements_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.678070 requirements-language-server-0.0.2/src/requirements_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/src/requirements_language_server/assets/jinja2/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/src/requirements_language_server/assets/jinja2/template.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/src/requirements_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/src/requirements_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-18 17:24:24.000000 requirements-language-server-0.0.2/src/requirements_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:24:24.682070 requirements-language-server-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/tests/api_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/tests/requirements.txt.in
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 17:24:11.000000 requirements-language-server-0.0.2/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/api/requirements-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/scripts/generate-api.md.pl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/scripts/generate-requirements.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.830108 requirements-language-server-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.834108 requirements-language-server-0.0.3/src/requirements_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/src/requirements_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/src/requirements_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/src/requirements_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.830108 requirements-language-server-0.0.3/src/requirements_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/src/requirements_language_server/assets/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/src/requirements_language_server/assets/jinja2/template.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/src/requirements_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/src/requirements_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 15:11:55.000000 requirements-language-server-0.0.3/src/requirements_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:11:55.838108 requirements-language-server-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/tests/api_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/tests/requirements.txt.in
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-20 15:11:43.000000 requirements-language-server-0.0.3/tests/server_test.py
```

### Comparing `requirements-language-server-0.0.2/.github/workflows/main.yml` & `requirements-language-server-0.0.3/.github/workflows/main.yml`

 * *Files 0% similar despite different names*

```diff
@@ -85,13 +85,13 @@
         with:
           # body_path: build/CHANGELOG.md
           files: |
             dist/*
   deploy:
     needs: build
     runs-on: ubuntu-latest
+    if: startsWith(github.ref, 'refs/tags/')
     steps:
       - uses: Freed-Wu/update-aur-package@v1.0.11
-        if: startsWith(github.ref, 'refs/tags/')
         with:
           package_name: python-requirements-language-server
           ssh_private_key: ${{secrets.AUR_SSH_PRIVATE_KEY}}
```

### Comparing `requirements-language-server-0.0.2/.gitignore` & `requirements-language-server-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.2/.pre-commit-config.yaml` & `requirements-language-server-0.0.3/.pre-commit-config.yaml`

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

### Comparing `requirements-language-server-0.0.2/LICENSE` & `requirements-language-server-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.2/PKG-INFO` & `requirements-language-server-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirements-language-server
-Version: 0.0.2
+Version: 0.0.3
 Summary: requirements language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://requirements-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/requirements-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/requirements-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/requirements-language-server
@@ -94,108 +94,17 @@
 
 ![file](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/da7e162d-fa82-461a-a8b4-09db684e766c)
 
 ### Diagnostic
 
 ![module](https://user-images.githubusercontent.com/32936898/194537147-bf4b4528-2594-46df-b05c-56c38c419920.png)
 
-## Usage
-
-### Vim/Neovim
-
-#### [coc.nvim](https://github.com/neoclide/coc.nvim)
-
-```json
-{
-  "languageserver": {
-    "requirements": {
-      "command": "requirements-language-server",
-      "filetypes": [
-        "requirements"
-      ]
-    }
-  }
-}
-```
-
-#### [vim-lsp](https://github.com/prabirshrestha/vim-lsp)
-
-```vim
-if executable('requirements-language-server')
-  augroup lsp
-    autocmd!
-    autocmd User lsp_setup call lsp#register_server({
-          \ 'name': 'requirements',
-          \ 'cmd': {server_info->['requirements-language-server']},
-          \ 'whitelist': ['requirements'],
-          \ })
-  augroup END
-endif
-```
-
-### Neovim
-
-```lua
-vim.api.nvim_create_autocmd({ "BufEnter" }, {
-  pattern = { "requirements*.txt*" },
-  callback = function()
-    vim.lsp.start({
-      name = "requirements",
-      cmd = { "requirements-language-server" }
-    })
-  end,
-})
-```
-
-### Emacs
-
-```elisp
-(make-lsp-client :new-connection
-(lsp-stdio-connection
-  `(,(executable-find "requirements-language-server")))
-  :activation-fn (lsp-activate-on "requirements*.txt*")
-  :server-id "requirements")))
-```
-
-### Sublime
-
-```json
-{
-  "clients": {
-    "requirements": {
-      "command": [
-        "requirements-language-server"
-      ],
-      "enabled": true,
-      "selector": "source.requirements"
-    }
-  }
-}
-```
-
-## Customization
-
-You can customize the document hover template. A default template is
-[here](https://github.com/Freed-Wu/requirements-language-server/tree/main/src/requirements_language_server/assets/jinja2/template.md.j2).
-The syntax rule is [jinja](https://docs.jinkan.org/docs/jinja2/templates.html).
-The template path is decided by your OS:
-
-```shell
-$ requirements-language-server --print-config template
-/home/wzy/.config/pip/template.md.j2
-```
-
-You can generate cache by `requirements-language-server --generate-cache` to
-fasten document hover and completion. Every time you change template, the cache
-must be regenerated.
-
-```shell
-$ requirements-language-server --print-config cache
-/home/wzy/.cache/pip/pip.json
-```
+Read
+[![readthedocs](https://shields.io/readthedocs/requirements-language-server)](https://requirements-language-server.readthedocs.io)
+to know more.
 
 ## Related Projects
 
 - [requirements.txt.vim](https://github.com/raimon49/requirements.txt.vim):
   syntax highlight for vim
 - [vim-polyglot](https://github.com/sheerun/vim-polyglot): contains above
 - [bat](https://github.com/sharkdp/bat): syntax highlight for less
```

### Comparing `requirements-language-server-0.0.2/README.md` & `requirements-language-server-0.0.3/src/requirements_language_server.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: requirements-language-server
+Version: 0.0.3
+Summary: requirements language server
+Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
+License: GPL v3
+Project-URL: Homepage, https://requirements-language-server.readthedocs.io
+Project-URL: Download, https://github.com/Freed-Wu/requirements-language-server/releases
+Project-URL: Bug Report, https://github.com/Freed-Wu/requirements-language-server/issues
+Project-URL: Source, https://github.com/Freed-Wu/requirements-language-server
+Keywords: requirements,language server
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # requirements-language-server
 
 [![readthedocs](https://shields.io/readthedocs/requirements-language-server)](https://requirements-language-server.readthedocs.io)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Freed-Wu/requirements-language-server/main.svg)](https://results.pre-commit.ci/latest/github/Freed-Wu/requirements-language-server/main)
 [![github/workflow](https://github.com/Freed-Wu/requirements-language-server/actions/workflows/main.yml/badge.svg)](https://github.com/Freed-Wu/requirements-language-server/actions)
 [![codecov](https://codecov.io/gh/Freed-Wu/requirements-language-server/branch/main/graph/badge.svg)](https://codecov.io/gh/Freed-Wu/requirements-language-server)
 [![DeepSource](https://deepsource.io/gh/Freed-Wu/requirements-language-server.svg/?show_trend=true)](https://deepsource.io/gh/Freed-Wu/requirements-language-server)
@@ -61,108 +94,17 @@
 
 ![file](https://github.com/Freed-Wu/requirements-language-server/assets/32936898/da7e162d-fa82-461a-a8b4-09db684e766c)
 
 ### Diagnostic
 
 ![module](https://user-images.githubusercontent.com/32936898/194537147-bf4b4528-2594-46df-b05c-56c38c419920.png)
 
-## Usage
-
-### Vim/Neovim
-
-#### [coc.nvim](https://github.com/neoclide/coc.nvim)
-
-```json
-{
-  "languageserver": {
-    "requirements": {
-      "command": "requirements-language-server",
-      "filetypes": [
-        "requirements"
-      ]
-    }
-  }
-}
-```
-
-#### [vim-lsp](https://github.com/prabirshrestha/vim-lsp)
-
-```vim
-if executable('requirements-language-server')
-  augroup lsp
-    autocmd!
-    autocmd User lsp_setup call lsp#register_server({
-          \ 'name': 'requirements',
-          \ 'cmd': {server_info->['requirements-language-server']},
-          \ 'whitelist': ['requirements'],
-          \ })
-  augroup END
-endif
-```
-
-### Neovim
-
-```lua
-vim.api.nvim_create_autocmd({ "BufEnter" }, {
-  pattern = { "requirements*.txt*" },
-  callback = function()
-    vim.lsp.start({
-      name = "requirements",
-      cmd = { "requirements-language-server" }
-    })
-  end,
-})
-```
-
-### Emacs
-
-```elisp
-(make-lsp-client :new-connection
-(lsp-stdio-connection
-  `(,(executable-find "requirements-language-server")))
-  :activation-fn (lsp-activate-on "requirements*.txt*")
-  :server-id "requirements")))
-```
-
-### Sublime
-
-```json
-{
-  "clients": {
-    "requirements": {
-      "command": [
-        "requirements-language-server"
-      ],
-      "enabled": true,
-      "selector": "source.requirements"
-    }
-  }
-}
-```
-
-## Customization
-
-You can customize the document hover template. A default template is
-[here](https://github.com/Freed-Wu/requirements-language-server/tree/main/src/requirements_language_server/assets/jinja2/template.md.j2).
-The syntax rule is [jinja](https://docs.jinkan.org/docs/jinja2/templates.html).
-The template path is decided by your OS:
-
-```shell
-$ requirements-language-server --print-config template
-/home/wzy/.config/pip/template.md.j2
-```
-
-You can generate cache by `requirements-language-server --generate-cache` to
-fasten document hover and completion. Every time you change template, the cache
-must be regenerated.
-
-```shell
-$ requirements-language-server --print-config cache
-/home/wzy/.cache/pip/pip.json
-```
+Read
+[![readthedocs](https://shields.io/readthedocs/requirements-language-server)](https://requirements-language-server.readthedocs.io)
+to know more.
 
 ## Related Projects
 
 - [requirements.txt.vim](https://github.com/raimon49/requirements.txt.vim):
   syntax highlight for vim
 - [vim-polyglot](https://github.com/sheerun/vim-polyglot): contains above
 - [bat](https://github.com/sharkdp/bat): syntax highlight for less
```

### Comparing `requirements-language-server-0.0.2/docs/conf.py` & `requirements-language-server-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.2/docs/resources/install.md` & `requirements-language-server-0.0.3/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.2/flake.nix` & `requirements-language-server-0.0.3/flake.nix`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.2/pyproject.toml` & `requirements-language-server-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.2/src/requirements_language_server/__init__.py` & `requirements-language-server-0.0.3/src/requirements_language_server/__init__.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.2/src/requirements_language_server/__main__.py` & `requirements-language-server-0.0.3/src/requirements_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.2/src/requirements_language_server/api.py` & `requirements-language-server-0.0.3/src/requirements_language_server/api.py`

 * *Files identical despite different names*

### Comparing `requirements-language-server-0.0.2/src/requirements_language_server/server.py` & `requirements-language-server-0.0.3/src/requirements_language_server/server.py`

 * *Files 0% similar despite different names*

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
@@ -241,14 +242,15 @@
             diagnostics = [
                 Diagnostic(
                     range=Range(
                         Position(line, 0),
                         Position(line, len(source.splitlines()[line])),
                     ),
                     message=msg,
+                    severity=DiagnosticSeverity.Error,
                     source="pip-compile",
                 )
                 for line, msg in diagnostic(params.text_document.uri).items()
             ]
             self.publish_diagnostics(text_doc.uri, diagnostics)
 
     def _cursor_line(self, uri: str, position: Position) -> str:
```

### Comparing `requirements-language-server-0.0.2/src/requirements_language_server.egg-info/SOURCES.txt` & `requirements-language-server-0.0.3/src/requirements_language_server.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 requirements.txt
 .github/FUNDING.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/index.md
 docs/requirements.txt
 docs/api/requirements-language-server.md
+docs/resources/configure.md
 docs/resources/install.md
+docs/resources/requirements.md
 requirements/dev.txt
 scripts/generate-api.md.pl
+scripts/generate-requirements.md.pl
 src/requirements_language_server/__init__.py
 src/requirements_language_server/__main__.py
 src/requirements_language_server/_version.py
 src/requirements_language_server/api.py
 src/requirements_language_server/py.typed
 src/requirements_language_server/server.py
 src/requirements_language_server.egg-info/PKG-INFO
```

