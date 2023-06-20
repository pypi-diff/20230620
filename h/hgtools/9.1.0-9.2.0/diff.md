# Comparing `tmp/hgtools-9.1.0.tar.gz` & `tmp/hgtools-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgtools-9.1.0.tar", last modified: Mon Jan 10 03:23:08 2022, max compression
+gzip compressed data, was "hgtools-9.2.0.tar", last modified: Tue Jun 20 10:14:07 2023, max compression
```

## Comparing `hgtools-9.1.0.tar` & `hgtools-9.2.0.tar`

### file list

```diff
@@ -1,48 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:23:08.881492 hgtools-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-01-10 03:22:50.000000 hgtools-9.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-01-10 03:22:50.000000 hgtools-9.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-01-10 03:22:50.000000 hgtools-9.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:23:08.877492 hgtools-9.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-01-10 03:22:50.000000 hgtools-9.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:23:08.877492 hgtools-9.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-01-10 03:22:50.000000 hgtools-9.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-01-10 03:22:50.000000 hgtools-9.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-01-10 03:22:50.000000 hgtools-9.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     9612 2022-01-10 03:22:50.000000 hgtools-9.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-01-10 03:22:50.000000 hgtools-9.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3202 2022-01-10 03:23:08.881492 hgtools-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2511 2022-01-10 03:22:50.000000 hgtools-9.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:23:08.877492 hgtools-9.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-01-10 03:22:50.000000 hgtools-9.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-01-10 03:22:50.000000 hgtools-9.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-01-10 03:22:50.000000 hgtools-9.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:23:08.877492 hgtools-9.1.0/hgtools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:23:08.881492 hgtools-9.1.0/hgtools/managers/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/managers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3512 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6044 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/managers/cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/managers/library.py
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/managers/reentry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/managers/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:23:08.881492 hgtools-9.1.0/hgtools/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/tests/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5396 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/tests/test_mercurial.py
--rw-r--r--   0 runner    (1001) docker     (121)     2403 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/tests/test_reentry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/tests/test_versioning.py
--rw-r--r--   0 runner    (1001) docker     (121)     6020 2022-01-10 03:22:50.000000 hgtools-9.1.0/hgtools/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-10 03:23:08.877492 hgtools-9.1.0/hgtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3202 2022-01-10 03:23:08.000000 hgtools-9.1.0/hgtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-01-10 03:23:08.000000 hgtools-9.1.0/hgtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-10 03:23:08.000000 hgtools-9.1.0/hgtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-01-10 03:23:08.000000 hgtools-9.1.0/hgtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-10 03:23:08.000000 hgtools-9.1.0/hgtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-01-10 03:22:50.000000 hgtools-9.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-01-10 03:22:50.000000 hgtools-9.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-01-10 03:22:50.000000 hgtools-9.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-01-10 03:23:08.881492 hgtools-9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-01-10 03:22:50.000000 hgtools-9.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-01-10 03:22:50.000000 hgtools-9.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:14:07.656766 hgtools-9.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 10:13:43.000000 hgtools-9.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 10:13:43.000000 hgtools-9.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:14:07.644765 hgtools-9.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 10:13:43.000000 hgtools-9.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:14:07.644765 hgtools-9.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-20 10:13:43.000000 hgtools-9.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-20 10:13:43.000000 hgtools-9.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 10:13:43.000000 hgtools-9.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-06-20 10:13:43.000000 hgtools-9.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-20 10:13:43.000000 hgtools-9.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-20 10:14:07.656766 hgtools-9.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-20 10:13:43.000000 hgtools-9.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:14:07.644765 hgtools-9.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-20 10:13:43.000000 hgtools-9.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-20 10:13:43.000000 hgtools-9.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-20 10:13:43.000000 hgtools-9.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:14:07.644765 hgtools-9.2.0/hgtools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:14:07.652765 hgtools-9.2.0/hgtools/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/managers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3512 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/managers/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/managers/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/managers/reentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/managers/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:14:07.656766 hgtools-9.2.0/hgtools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/tests/test_mercurial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/tests/test_reentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/tests/test_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-20 10:13:43.000000 hgtools-9.2.0/hgtools/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:14:07.648765 hgtools-9.2.0/hgtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-20 10:14:07.000000 hgtools-9.2.0/hgtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-20 10:14:07.000000 hgtools-9.2.0/hgtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:14:07.000000 hgtools-9.2.0/hgtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 10:14:07.000000 hgtools-9.2.0/hgtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 10:14:07.000000 hgtools-9.2.0/hgtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-20 10:13:43.000000 hgtools-9.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-20 10:13:43.000000 hgtools-9.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-20 10:13:43.000000 hgtools-9.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-20 10:14:07.656766 hgtools-9.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-20 10:13:43.000000 hgtools-9.2.0/tox.ini
```

### Comparing `hgtools-9.1.0/CHANGES.rst` & `hgtools-9.2.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v9.2.0
+======
+
+* #34: Fixed test failures when running tests and
+  ``ui.relative-paths=yes``.
+
 v9.1.0
 ======
 
 * Require Python 3.7 or later.
 
 v9.0.0
 ======
```

### Comparing `hgtools-9.1.0/LICENSE` & `hgtools-9.2.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hgtools-9.1.0/PKG-INFO` & `hgtools-9.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: hgtools
-Version: 9.1.0
+Version: 9.2.0
 Summary: Classes for Mercurial and Git repositories
 Home-page: https://github.com/jaraco/hgtools
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Framework :: Setuptools Plugin
 Requires-Python: >=3.7
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/hgtools.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/hgtools
 
 .. image:: https://img.shields.io/pypi/pyversions/hgtools.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/hgtools
 
 .. image:: https://github.com/jaraco/hgtools/workflows/tests/badge.svg
    :target: https://github.com/jaraco/hgtools/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 Usage
 =====
 
 hgtools
 provides classes for inspecting and working with repositories in the
@@ -83,9 +82,7 @@
 
 Example::
 
     >>> from hgtools.managers import RepoManager
     >>> RepoManager().get_first_valid_manager().get_current_version()
     '9.0.1.dev0'
 
-
-
```

### Comparing `hgtools-9.1.0/README.rst` & `hgtools-9.2.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 .. image:: https://img.shields.io/pypi/v/hgtools.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/hgtools
 
 .. image:: https://img.shields.io/pypi/pyversions/hgtools.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/hgtools
 
 .. image:: https://github.com/jaraco/hgtools/workflows/tests/badge.svg
    :target: https://github.com/jaraco/hgtools/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 Usage
 =====
 
 hgtools
 provides classes for inspecting and working with repositories in the
```

### Comparing `hgtools-9.1.0/docs/conf.py` & `hgtools-9.2.0/docs/conf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,42 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
     '../CHANGES.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
                 pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
                 with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
-                url='https://www.python.org/dev/peps/pep-{pep_number:0>4}/',
+                url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
 
-# Be strict about any broken references:
+# Be strict about any broken references
 nitpicky = True
 
 # Include Python intersphinx mapping to prevent failures
 # jaraco/skeleton#51
 extensions += ['sphinx.ext.intersphinx']
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
 }
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
```

### Comparing `hgtools-9.1.0/hgtools/managers/base.py` & `hgtools-9.2.0/hgtools/managers/base.py`

 * *Files identical despite different names*

### Comparing `hgtools-9.1.0/hgtools/managers/cmd.py` & `hgtools-9.2.0/hgtools/managers/cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import re
 import operator
 import itertools
 import collections
 
 import packaging
 
@@ -42,21 +41,16 @@
         except Exception:
             pass
 
     def find_files(self):
         """
         Find versioned files in self.location
         """
-        all_files = self._invoke('locate', '-I', '.').splitlines()
-        # now we have a list of all files in self.location relative to
-        #  self.find_root()
-        # Remove the parent dirs from them.
-        from_root = os.path.relpath(self.location, self.find_root())
-        loc_rel_paths = [os.path.relpath(path, from_root) for path in all_files]
-        return loc_rel_paths
+        cmd = 'locate', '-I', '.', '--config', 'ui.relative-paths=yes'
+        return self._invoke(*cmd).splitlines()
 
     def get_parent_revs(self, rev=None):
         cmd = ['parents', '--style', 'default', '--config', 'defaults.parents=']
         if rev:
             cmd.extend(['--rev', str(rev)])
         out = self._invoke(*cmd)
         cs_pat = r'^changeset:\s+(?P<local>\d+):(?P<hash>[0-9a-zA-Z]+)'
```

### Comparing `hgtools-9.1.0/hgtools/managers/library.py` & `hgtools-9.2.0/hgtools/managers/library.py`

 * *Files identical despite different names*

### Comparing `hgtools-9.1.0/hgtools/managers/reentry.py` & `hgtools-9.2.0/hgtools/managers/reentry.py`

 * *Files identical despite different names*

### Comparing `hgtools-9.1.0/hgtools/managers/subprocess.py` & `hgtools-9.2.0/hgtools/managers/subprocess.py`

 * *Files identical despite different names*

### Comparing `hgtools-9.1.0/hgtools/tests/conftest.py` & `hgtools-9.2.0/hgtools/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     mgr = managers.MercurialManager()
     _ensure_present(mgr)
     mgr._invoke('init', '.')
     os.makedirs('bar')
     touch('bar/baz')
     mgr._invoke('addremove')
     mgr._invoke('ci', '-m', 'committed')
-    with open('bar/baz', 'w') as baz:
+    with open('bar/baz', 'w', encoding='utf-8') as baz:
         baz.write('content')
     mgr._invoke('ci', '-m', 'added content')
     return tmpdir_as_cwd
 
 
 @pytest.fixture
 def git_repo(tmpdir_as_cwd):
@@ -40,16 +40,16 @@
     mgr._invoke('init')
     mgr._invoke('config', 'user.email', 'hgtools@example.com')
     mgr._invoke('config', 'user.name', 'HGTools')
     os.makedirs('bar')
     touch('bar/baz')
     mgr._invoke('add', '.')
     mgr._invoke('commit', '-m', 'committed')
-    with open('bar/baz', 'w') as baz:
+    with open('bar/baz', 'w', encoding='utf-8') as baz:
         baz.write('content')
     mgr._invoke('commit', '-am', 'added content')
     return tmpdir_as_cwd
 
 
 def touch(filename):
-    with open(filename, 'a'):
+    with open(filename, 'a', encoding='utf-8'):
         pass
```

### Comparing `hgtools-9.1.0/hgtools/tests/test_git.py` & `hgtools-9.2.0/hgtools/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `hgtools-9.1.0/hgtools/tests/test_managers.py` & `hgtools-9.2.0/hgtools/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `hgtools-9.1.0/hgtools/tests/test_mercurial.py` & `hgtools-9.2.0/hgtools/tests/test_mercurial.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     def test_no_tags(self):
         "No tag should return empty set"
         assert self.mgr.get_tags('0') == set([])
 
     def test_local_modifications(self):
         "Local modifications should return empty set"
-        with open('bar/baz', 'w') as f:
+        with open('bar/baz', 'w', encoding='utf-8') as f:
             f.write('changed')
         assert self.mgr.get_tags() == set([])
 
     def test_parent_tag(self):
         self.mgr._invoke('tag', '1.0')
         assert self.mgr.get_tags() == set(['tip'])
         assert self.mgr.get_parent_tags() == set(['tip'])
@@ -116,22 +116,22 @@
 
     def _setup_branchy_tags(self):
         """
         Create two heads, one which has a 1.0 tag and a different one which
         has a 1.1 tag.
         """
         # create a commit with a tag
-        with open('bar/baz', 'a') as f:
+        with open('bar/baz', 'a', encoding='utf-8') as f:
             f.write('\nmore to say\n')
         self.mgr._invoke('commit', '-m', 'Had more to say')
         self.mgr._invoke('tag', '1.0')
         # update to the pre-tagged revision
         self.mgr._invoke('update', '1')
         # Make a different commit
-        with open('bar/baz', 'a') as f:
+        with open('bar/baz', 'a', encoding='utf-8') as f:
             f.write('\na different concept\n')
         self.mgr._invoke('commit', '-m', 'A different approach')
         self.mgr._invoke('tag', '1.1')
 
     def test_ancestral_tags_local(self):
         """
         get_ancestral_tags should only return tagged revisions ancestral
```

### Comparing `hgtools-9.1.0/hgtools/tests/test_reentry.py` & `hgtools-9.2.0/hgtools/tests/test_reentry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-import py.test
+import pytest
 
 from hgtools.managers import reentry
 
 
 def hello_world():
     print("hello world")
 
@@ -70,19 +70,19 @@
         assert proc.returncode == 0
         out = "args are ['echo', 'foo', 'bar']\n"
         assert proc.stdio.stdout.getvalue() == out
 
 
 class TestErrors:
     def test_name_error(self):
-        with py.test.raises(NameError) as exc_info:
+        with pytest.raises(NameError) as exc_info:
             with reentry.in_process_context([]) as proc:
                 not_present  # noqa
         assert proc.returncode == 1
         msg = "name 'not_present' is not defined"
         assert str(exc_info.value).endswith(msg)
 
     def test_keyboard_interrupt(self):
-        with py.test.raises(KeyboardInterrupt):
+        with pytest.raises(KeyboardInterrupt):
             with reentry.in_process_context([]) as proc:
                 raise KeyboardInterrupt()
         assert proc.returncode == 1
```

### Comparing `hgtools-9.1.0/hgtools/tests/test_versioning.py` & `hgtools-9.2.0/hgtools/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `hgtools-9.1.0/hgtools/versioning.py` & `hgtools-9.2.0/hgtools/versioning.py`

 * *Files identical despite different names*

### Comparing `hgtools-9.1.0/hgtools.egg-info/PKG-INFO` & `hgtools-9.2.0/hgtools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: hgtools
-Version: 9.1.0
+Version: 9.2.0
 Summary: Classes for Mercurial and Git repositories
 Home-page: https://github.com/jaraco/hgtools
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Framework :: Setuptools Plugin
 Requires-Python: >=3.7
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/hgtools.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/hgtools
 
 .. image:: https://img.shields.io/pypi/pyversions/hgtools.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/hgtools
 
 .. image:: https://github.com/jaraco/hgtools/workflows/tests/badge.svg
    :target: https://github.com/jaraco/hgtools/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2021-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
 Usage
 =====
 
 hgtools
 provides classes for inspecting and working with repositories in the
@@ -83,9 +82,7 @@
 
 Example::
 
     >>> from hgtools.managers import RepoManager
     >>> RepoManager().get_first_valid_manager().get_current_version()
     '9.0.1.dev0'
 
-
-
```

### Comparing `hgtools-9.1.0/hgtools.egg-info/SOURCES.txt` & `hgtools-9.2.0/hgtools.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
-.readthedocs.yml
+.readthedocs.yaml
 CHANGES.rst
 LICENSE
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
-setup.py
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 hgtools/__init__.py
```

### Comparing `hgtools-9.1.0/setup.cfg` & `hgtools-9.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -30,25 +30,27 @@
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy; \
+	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.0.1
+	pytest-enabler >= 1.3
+	pytest-ruff
 	
 	pygments
 docs = 
-	sphinx
-	jaraco.packaging >= 8.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `hgtools-9.1.0/tox.ini` & `hgtools-9.2.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -4,26 +4,30 @@
 # https://github.com/jaraco/skeleton/issues/6
 tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
+setenv =
+	PYTHONWARNDEFAULTENCODING = 1
 commands =
 	pytest {posargs}
 usedevelop = True
-extras = testing
+extras =
+	testing
 
 [testenv:docs]
 extras =
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
+	python -m sphinxlint
 
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
```

