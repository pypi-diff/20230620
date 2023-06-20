# Comparing `tmp/pkgbuild-language-server-0.0.3.tar.gz` & `tmp/pkgbuild-language-server-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgbuild-language-server-0.0.3.tar", last modified: Tue Jun 20 10:47:28 2023, max compression
+gzip compressed data, was "pkgbuild-language-server-0.0.4.tar", last modified: Tue Jun 20 12:25:20 2023, max compression
```

## Comparing `pkgbuild-language-server-0.0.3.tar` & `pkgbuild-language-server-0.0.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.017107 pkgbuild-language-server-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-20 10:47:28.017107 pkgbuild-language-server-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/docs/api/pkgbuild-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/requirements/cache.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/requirements/package.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/scripts/generate-api.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:47:28.017107 pkgbuild-language-server-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.009107 pkgbuild-language-server-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 10:47:27.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.009107 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/jinja2/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/jinja2/template.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.017107 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/json/pkgbuild.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/package.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.013107 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-20 10:47:27.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-20 10:47:28.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:47:27.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:47:27.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 10:47:27.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 10:47:27.000000 pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.017107 pkgbuild-language-server-0.0.3/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:47:28.017107 pkgbuild-language-server-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 10:47:17.000000 pkgbuild-language-server-0.0.3/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.420702 pkgbuild-language-server-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.416702 pkgbuild-language-server-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.416702 pkgbuild-language-server-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-20 12:25:20.420702 pkgbuild-language-server-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.416702 pkgbuild-language-server-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.416702 pkgbuild-language-server-0.0.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/docs/api/pkgbuild-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.416702 pkgbuild-language-server-0.0.4/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.416702 pkgbuild-language-server-0.0.4/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/requirements/cache.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/requirements/package.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.416702 pkgbuild-language-server-0.0.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/scripts/generate-api.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 12:25:20.420702 pkgbuild-language-server-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.412702 pkgbuild-language-server-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.420702 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 12:25:20.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.412702 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.420702 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/assets/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/assets/jinja2/template.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.420702 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/assets/json/pkgbuild.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.420702 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-20 12:25:20.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-20 12:25:20.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:25:20.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 12:25:20.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 12:25:20.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 12:25:20.000000 pkgbuild-language-server-0.0.4/src/pkgbuild_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.420702 pkgbuild-language-server-0.0.4/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:25:20.420702 pkgbuild-language-server-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 12:25:06.000000 pkgbuild-language-server-0.0.4/tests/server_test.py
```

### Comparing `pkgbuild-language-server-0.0.3/.github/workflows/main.yml` & `pkgbuild-language-server-0.0.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/.gitignore` & `pkgbuild-language-server-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/.pre-commit-config.yaml` & `pkgbuild-language-server-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/LICENSE` & `pkgbuild-language-server-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/PKG-INFO` & `pkgbuild-language-server-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgbuild-language-server
-Version: 0.0.3
+Version: 0.0.4
 Summary: pkgbuild language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://pkgbuild-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/pkgbuild-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/pkgbuild-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/pkgbuild-language-server
```

### Comparing `pkgbuild-language-server-0.0.3/README.md` & `pkgbuild-language-server-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/docs/conf.py` & `pkgbuild-language-server-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/docs/resources/configure.md` & `pkgbuild-language-server-0.0.4/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/docs/resources/install.md` & `pkgbuild-language-server-0.0.4/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/flake.nix` & `pkgbuild-language-server-0.0.4/flake.nix`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/pyproject.toml` & `pkgbuild-language-server-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/__init__.py` & `pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/__init__.py`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/__main__.py` & `pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/api.py` & `pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/api.py`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/jinja2/template.md.j2` & `pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/assets/jinja2/template.md.j2`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/assets/json/pkgbuild.json` & `pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/assets/json/pkgbuild.json`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/package.py` & `pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/package.py`

 * *Files identical despite different names*

### Comparing `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server/server.py` & `pkgbuild-language-server-0.0.4/src/pkgbuild_language_server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,16 @@
         def completions(params: CompletionParams) -> CompletionList:
             r"""Completions.
 
             :param params:
             :type params: CompletionParams
             :rtype: CompletionList
             """
+            if not check_extension(params.text_document.uri):
+                return CompletionList(is_incomplete=False, items=[])
             word = self._cursor_word(
                 params.text_document.uri, params.position, False, True
             )
             token = "" if word is None else word[0]
             items = [
                 CompletionItem(
                     label=x,
```

### Comparing `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/PKG-INFO` & `pkgbuild-language-server-0.0.4/src/pkgbuild_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkgbuild-language-server
-Version: 0.0.3
+Version: 0.0.4
 Summary: pkgbuild language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://pkgbuild-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/pkgbuild-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/pkgbuild-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/pkgbuild-language-server
```

### Comparing `pkgbuild-language-server-0.0.3/src/pkgbuild_language_server.egg-info/SOURCES.txt` & `pkgbuild-language-server-0.0.4/src/pkgbuild_language_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

