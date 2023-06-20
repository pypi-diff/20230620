# Comparing `tmp/pyds-cli-0.1.8.tar.gz` & `tmp/pyds-cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyds-cli-0.1.8.tar", last modified: Mon Apr 17 18:15:50 2023, max compression
+gzip compressed data, was "pyds-cli-0.1.9.tar", last modified: Tue Jun 20 04:16:20 2023, max compression
```

## Comparing `pyds-cli-0.1.8.tar` & `pyds-cli-0.1.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.529710 pyds-cli-0.1.8/
--rw-r--r--   0 ericmjl    (501) staff       (20)       28 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/MANIFEST.in
--rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-17 18:15:50.529556 pyds-cli-0.1.8/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)     2814 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/README.md
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.519844 pyds-cli-0.1.8/pyds/
--rw-r--r--   0 ericmjl    (501) staff       (20)       93 2023-04-05 22:39:01.000000 pyds-cli-0.1.8/pyds/__init__.py
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.521219 pyds-cli-0.1.8/pyds/cli/
--rw-r--r--   0 ericmjl    (501) staff       (20)     1910 2023-04-05 22:38:40.000000 pyds-cli-0.1.8/pyds/cli/__init__.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      933 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/conda.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      398 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/docs.py
--rw-r--r--   0 ericmjl    (501) staff       (20)     2858 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/environment.py
--rw-r--r--   0 ericmjl    (501) staff       (20)     2516 2023-04-03 18:58:17.000000 pyds-cli-0.1.8/pyds/cli/package.py
--rw-r--r--   0 ericmjl    (501) staff       (20)     4996 2023-04-17 18:10:42.000000 pyds-cli-0.1.8/pyds/cli/project.py
--rw-r--r--   0 ericmjl    (501) staff       (20)     2693 2023-04-03 18:58:17.000000 pyds-cli-0.1.8/pyds/cli/system.py
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.523739 pyds-cli-0.1.8/pyds/cli/templates/
--rw-r--r--   0 ericmjl    (501) staff       (20)       98 2023-04-03 18:56:44.000000 pyds-cli-0.1.8/pyds/cli/templates/.bumpversion.cfg.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       34 2021-11-05 23:29:52.000000 pyds-cli-0.1.8/pyds/cli/templates/.darglint.j2
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.524221 pyds-cli-0.1.8/pyds/cli/templates/.devcontainer/
--rw-r--r--   0 ericmjl    (501) staff       (20)     2587 2021-11-15 12:34:35.000000 pyds-cli-0.1.8/pyds/cli/templates/.devcontainer/Dockerfile.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      645 2021-11-15 12:35:38.000000 pyds-cli-0.1.8/pyds/cli/templates/.devcontainer/devcontainer.json.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      229 2023-04-03 18:58:17.000000 pyds-cli-0.1.8/pyds/cli/templates/.env.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       29 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/.flake8.j2
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.518414 pyds-cli-0.1.8/pyds/cli/templates/.github/
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.524824 pyds-cli-0.1.8/pyds/cli/templates/.github/workflows/
--rw-r--r--   0 ericmjl    (501) staff       (20)      257 2021-11-15 12:34:35.000000 pyds-cli-0.1.8/pyds/cli/templates/.github/workflows/code-style.yaml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)     1546 2023-04-03 18:58:17.000000 pyds-cli-0.1.8/pyds/cli/templates/.github/workflows/docs.yaml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)     1113 2023-04-03 18:58:17.000000 pyds-cli-0.1.8/pyds/cli/templates/.github/workflows/pr-tests.yaml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)     2312 2023-04-03 18:58:17.000000 pyds-cli-0.1.8/pyds/cli/templates/.gitignore.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      923 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/.pre-commit-config.yaml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      124 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/MANIFEST.in.j2
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.525468 pyds-cli-0.1.8/pyds/cli/templates/docs/
--rw-r--r--   0 ericmjl    (501) staff       (20)       63 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/docs/api.md.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      607 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/docs/apidocs.css.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       21 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/docs/config.js.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      488 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/docs/index.md.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      664 2023-04-03 18:58:17.000000 pyds-cli-0.1.8/pyds/cli/templates/environment.yml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)     1833 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/mkdocs.yaml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)     1594 2023-04-05 17:48:28.000000 pyds-cli-0.1.8/pyds/cli/templates/pyproject.toml.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      212 2023-04-03 18:58:17.000000 pyds-cli-0.1.8/pyds/cli/templates/setup.cfg.j2
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.526406 pyds-cli-0.1.8/pyds/cli/templates/src/
--rw-r--r--   0 ericmjl    (501) staff       (20)      221 2023-04-03 18:58:17.000000 pyds-cli-0.1.8/pyds/cli/templates/src/__init__.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      659 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/src/cli.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       48 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/src/models.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       35 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/src/preprocessing.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)      192 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/src/schemas.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       40 2021-11-05 23:30:25.000000 pyds-cli-0.1.8/pyds/cli/templates/src/utils.py.j2
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.527059 pyds-cli-0.1.8/pyds/cli/templates/tests/
--rw-r--r--   0 ericmjl    (501) staff       (20)       36 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/tests/test___init__.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       40 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/tests/test_cli.py.j2
--rw-r--r--   0 ericmjl    (501) staff       (20)       62 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/pyds/cli/templates/tests/test_models.py.j2
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.527591 pyds-cli-0.1.8/pyds/utils/
--rw-r--r--   0 ericmjl    (501) staff       (20)     6913 2023-04-17 18:15:11.000000 pyds-cli-0.1.8/pyds/utils/__init__.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      123 2023-04-03 18:58:17.000000 pyds-cli-0.1.8/pyds/utils/paths.py
--rw-r--r--   0 ericmjl    (501) staff       (20)     8487 2023-04-17 17:58:46.000000 pyds-cli-0.1.8/pyds/utils/project.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       75 2023-04-17 18:15:44.000000 pyds-cli-0.1.8/pyds/version.py
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.528347 pyds-cli-0.1.8/pyds_cli.egg-info/
--rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-17 18:15:50.000000 pyds-cli-0.1.8/pyds_cli.egg-info/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)     1809 2023-04-17 18:15:50.000000 pyds-cli-0.1.8/pyds_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-04-17 18:15:50.000000 pyds-cli-0.1.8/pyds_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-17 18:15:50.000000 pyds-cli-0.1.8/pyds_cli.egg-info/entry_points.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)      172 2023-04-17 18:15:50.000000 pyds-cli-0.1.8/pyds_cli.egg-info/requires.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)       21 2023-04-17 18:15:50.000000 pyds-cli-0.1.8/pyds_cli.egg-info/top_level.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)     1611 2023-04-17 18:15:44.000000 pyds-cli-0.1.8/pyproject.toml
--rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-17 18:15:50.529751 pyds-cli-0.1.8/setup.cfg
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.518875 pyds-cli-0.1.8/tests/
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-17 18:15:50.529372 pyds-cli-0.1.8/tests/cli/
--rw-r--r--   0 ericmjl    (501) staff       (20)     1233 2023-04-03 18:58:17.000000 pyds-cli-0.1.8/tests/cli/conftest.py
--rw-r--r--   0 ericmjl    (501) staff       (20)     1042 2023-04-03 18:58:17.000000 pyds-cli-0.1.8/tests/cli/test___init__.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      981 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/tests/cli/test_conda.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      504 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/tests/cli/test_docs.py
--rw-r--r--   0 ericmjl    (501) staff       (20)     1446 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/tests/cli/test_environment.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      390 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/tests/cli/test_package.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      833 2023-04-05 17:42:03.000000 pyds-cli-0.1.8/tests/cli/test_project.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      274 2021-12-12 03:24:31.000000 pyds-cli-0.1.8/tests/cli/test_system.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.923068 pyds-cli-0.1.9/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       28 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/MANIFEST.in
+-rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-06-20 04:16:20.922909 pyds-cli-0.1.9/PKG-INFO
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2814 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/README.md
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.913253 pyds-cli-0.1.9/pyds/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       93 2023-04-05 22:39:01.000000 pyds-cli-0.1.9/pyds/__init__.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.914336 pyds-cli-0.1.9/pyds/cli/
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1910 2023-04-05 22:38:40.000000 pyds-cli-0.1.9/pyds/cli/__init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      933 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/conda.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      398 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/docs.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2858 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/environment.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2578 2023-06-20 04:13:06.000000 pyds-cli-0.1.9/pyds/cli/package.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     4996 2023-04-17 18:10:42.000000 pyds-cli-0.1.9/pyds/cli/project.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2693 2023-04-03 18:58:17.000000 pyds-cli-0.1.9/pyds/cli/system.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.916957 pyds-cli-0.1.9/pyds/cli/templates/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       98 2023-04-03 18:56:44.000000 pyds-cli-0.1.9/pyds/cli/templates/.bumpversion.cfg.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       34 2021-11-05 23:29:52.000000 pyds-cli-0.1.9/pyds/cli/templates/.darglint.j2
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.917369 pyds-cli-0.1.9/pyds/cli/templates/.devcontainer/
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2587 2021-11-15 12:34:35.000000 pyds-cli-0.1.9/pyds/cli/templates/.devcontainer/Dockerfile.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      645 2021-11-15 12:35:38.000000 pyds-cli-0.1.9/pyds/cli/templates/.devcontainer/devcontainer.json.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      229 2023-04-03 18:58:17.000000 pyds-cli-0.1.9/pyds/cli/templates/.env.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       29 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/.flake8.j2
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.912003 pyds-cli-0.1.9/pyds/cli/templates/.github/
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.918045 pyds-cli-0.1.9/pyds/cli/templates/.github/workflows/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      257 2021-11-15 12:34:35.000000 pyds-cli-0.1.9/pyds/cli/templates/.github/workflows/code-style.yaml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1546 2023-04-03 18:58:17.000000 pyds-cli-0.1.9/pyds/cli/templates/.github/workflows/docs.yaml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1113 2023-04-03 18:58:17.000000 pyds-cli-0.1.9/pyds/cli/templates/.github/workflows/pr-tests.yaml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)     2312 2023-04-03 18:58:17.000000 pyds-cli-0.1.9/pyds/cli/templates/.gitignore.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      923 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/.pre-commit-config.yaml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      124 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/MANIFEST.in.j2
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.918684 pyds-cli-0.1.9/pyds/cli/templates/docs/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       63 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/docs/api.md.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      607 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/docs/apidocs.css.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       21 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/docs/config.js.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      488 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/docs/index.md.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      664 2023-04-17 18:43:57.000000 pyds-cli-0.1.9/pyds/cli/templates/environment.yml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1833 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/mkdocs.yaml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1594 2023-04-05 17:48:28.000000 pyds-cli-0.1.9/pyds/cli/templates/pyproject.toml.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      212 2023-04-03 18:58:17.000000 pyds-cli-0.1.9/pyds/cli/templates/setup.cfg.j2
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.919627 pyds-cli-0.1.9/pyds/cli/templates/src/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      221 2023-04-03 18:58:17.000000 pyds-cli-0.1.9/pyds/cli/templates/src/__init__.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      659 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/src/cli.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       48 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/src/models.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       35 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/src/preprocessing.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)      192 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/src/schemas.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       40 2021-11-05 23:30:25.000000 pyds-cli-0.1.9/pyds/cli/templates/src/utils.py.j2
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.920298 pyds-cli-0.1.9/pyds/cli/templates/tests/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       36 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/tests/test___init__.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       40 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/tests/test_cli.py.j2
+-rw-r--r--   0 ericmjl    (501) staff       (20)       62 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/pyds/cli/templates/tests/test_models.py.j2
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.920739 pyds-cli-0.1.9/pyds/utils/
+-rw-r--r--   0 ericmjl    (501) staff       (20)     6913 2023-04-17 18:15:11.000000 pyds-cli-0.1.9/pyds/utils/__init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      123 2023-04-03 18:58:17.000000 pyds-cli-0.1.9/pyds/utils/paths.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     8487 2023-04-17 17:58:46.000000 pyds-cli-0.1.9/pyds/utils/project.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       75 2023-06-20 04:16:17.000000 pyds-cli-0.1.9/pyds/version.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.921538 pyds-cli-0.1.9/pyds_cli.egg-info/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-06-20 04:16:20.000000 pyds-cli-0.1.9/pyds_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1809 2023-06-20 04:16:20.000000 pyds-cli-0.1.9/pyds_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-06-20 04:16:20.000000 pyds-cli-0.1.9/pyds_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-06-20 04:16:20.000000 pyds-cli-0.1.9/pyds_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)      172 2023-06-20 04:16:20.000000 pyds-cli-0.1.9/pyds_cli.egg-info/requires.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)       21 2023-06-20 04:16:20.000000 pyds-cli-0.1.9/pyds_cli.egg-info/top_level.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1611 2023-06-20 04:16:17.000000 pyds-cli-0.1.9/pyproject.toml
+-rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-06-20 04:16:20.923108 pyds-cli-0.1.9/setup.cfg
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.912459 pyds-cli-0.1.9/tests/
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-06-20 04:16:20.922682 pyds-cli-0.1.9/tests/cli/
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1233 2023-04-03 18:58:17.000000 pyds-cli-0.1.9/tests/cli/conftest.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1042 2023-04-03 18:58:17.000000 pyds-cli-0.1.9/tests/cli/test___init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      981 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/tests/cli/test_conda.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      504 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/tests/cli/test_docs.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1446 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/tests/cli/test_environment.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      390 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/tests/cli/test_package.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      833 2023-04-05 17:42:03.000000 pyds-cli-0.1.9/tests/cli/test_project.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      274 2021-12-12 03:24:31.000000 pyds-cli-0.1.9/tests/cli/test_system.py
```

### Comparing `pyds-cli-0.1.8/README.md` & `pyds-cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/__init__.py` & `pyds-cli-0.1.9/pyds/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/conda.py` & `pyds-cli-0.1.9/pyds/cli/conda.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/environment.py` & `pyds-cli-0.1.9/pyds/cli/environment.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/package.py` & `pyds-cli-0.1.9/pyds/cli/package.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         response = typer.confirm("Please double-check: is the version bump done right?")
         if response:
             run(f"bumpversion {bump} --verbose", show_out=True, activate_env=True)
             run("git add . && git commit")
             run("rm dist/*")
             run(f"python -m build {here()}", show_out=True, activate_env=True)
             run(f"twine upload -r {to} dist/*", show_out=True, activate_env=True)
+            run("git push", show_out=True, activate_env=True)
 
 
 @app.command()
 def reinstall(
     env_file: str = typer.Option("environment.yml", help="Environment file name.")
 ):
     """Reinstall the custom package into the conda environment.
```

### Comparing `pyds-cli-0.1.8/pyds/cli/project.py` & `pyds-cli-0.1.9/pyds/cli/project.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/system.py` & `pyds-cli-0.1.9/pyds/cli/system.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/templates/.devcontainer/Dockerfile.j2` & `pyds-cli-0.1.9/pyds/cli/templates/.devcontainer/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/templates/.devcontainer/devcontainer.json.j2` & `pyds-cli-0.1.9/pyds/cli/templates/.devcontainer/devcontainer.json.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/templates/.github/workflows/docs.yaml.j2` & `pyds-cli-0.1.9/pyds/cli/templates/.github/workflows/docs.yaml.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/templates/.github/workflows/pr-tests.yaml.j2` & `pyds-cli-0.1.9/pyds/cli/templates/.github/workflows/pr-tests.yaml.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/templates/.gitignore.j2` & `pyds-cli-0.1.9/pyds/cli/templates/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/templates/.pre-commit-config.yaml.j2` & `pyds-cli-0.1.9/pyds/cli/templates/.pre-commit-config.yaml.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/templates/docs/apidocs.css.j2` & `pyds-cli-0.1.9/pyds/cli/templates/docs/apidocs.css.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/templates/environment.yml.j2` & `pyds-cli-0.1.9/pyds/cli/templates/environment.yml.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/templates/mkdocs.yaml.j2` & `pyds-cli-0.1.9/pyds/cli/templates/mkdocs.yaml.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/templates/pyproject.toml.j2` & `pyds-cli-0.1.9/pyds/cli/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/cli/templates/src/cli.py.j2` & `pyds-cli-0.1.9/pyds/cli/templates/src/cli.py.j2`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/utils/__init__.py` & `pyds-cli-0.1.9/pyds/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds/utils/project.py` & `pyds-cli-0.1.9/pyds/utils/project.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyds_cli.egg-info/SOURCES.txt` & `pyds-cli-0.1.9/pyds_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/pyproject.toml` & `pyds-cli-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 include-package-data = true
 
 [tool.setuptools.packages]
 find = {}  # Scanning implicit namespaces is active by default
 
 [project]
 name = "pyds-cli"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
     "typer >=0.3.2",
     "pyyaml >=6.0",
     "jinja2 >=3.0.2",
     "loguru >=0.5.3",
     "pyprojroot >=0.2.0",
     "python-dotenv >=0.19.1",
```

### Comparing `pyds-cli-0.1.8/tests/cli/conftest.py` & `pyds-cli-0.1.9/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/tests/cli/test___init__.py` & `pyds-cli-0.1.9/tests/cli/test___init__.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/tests/cli/test_conda.py` & `pyds-cli-0.1.9/tests/cli/test_conda.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/tests/cli/test_environment.py` & `pyds-cli-0.1.9/tests/cli/test_environment.py`

 * *Files identical despite different names*

### Comparing `pyds-cli-0.1.8/tests/cli/test_project.py` & `pyds-cli-0.1.9/tests/cli/test_project.py`

 * *Files identical despite different names*

