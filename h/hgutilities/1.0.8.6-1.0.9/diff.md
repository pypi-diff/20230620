# Comparing `tmp/hgutilities-1.0.8.6.tar.gz` & `tmp/hgutilities-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgutilities-1.0.8.6.tar", last modified: Mon Jun 19 17:20:30 2023, max compression
+gzip compressed data, was "hgutilities-1.0.9.tar", last modified: Tue Jun 20 08:48:30 2023, max compression
```

## Comparing `hgutilities-1.0.8.6.tar` & `hgutilities-1.0.9.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.758204 hgutilities-1.0.8.6/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.608407 hgutilities-1.0.8.6/.eggs/
--rw-r-----   0 henry     (1000) henry     (1000)      211 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/README.txt
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.598235 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.615489 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/
--rw-r-----   0 henry     (1000) henry     (1000)     1023 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE
--rw-r-----   0 henry     (1000) henry     (1000)    24836 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     2575 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD
--rw-r-----   0 henry     (1000) henry     (1000)       92 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/WHEEL
--rw-r-----   0 henry     (1000) henry     (1000)     1734 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt
--rw-r-----   0 henry     (1000) henry     (1000)      102 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/requires.txt
--rw-r-----   0 henry     (1000) henry     (1000)       15 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/top_level.txt
--rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/zip-safe
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.634556 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/
--rw-r-----   0 henry     (1000) henry     (1000)     5891 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)       98 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__main__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.645651 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)     7516 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4963 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1634 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2634 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    10366 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3086 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5165 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     6554 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5593 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    10226 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)    24841 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2845 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_cli.py
--rw-r-----   0 henry     (1000) henry     (1000)     2696 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_entrypoints.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.648637 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.651453 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      252 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/__init__.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4755 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1190 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2838 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py
--rw-r-----   0 henry     (1000) henry     (1000)      530 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/setuptools.py
--rw-r-----   0 henry     (1000) henry     (1000)     1067 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py
--rw-r-----   0 henry     (1000) henry     (1000)      845 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py
--rw-r-----   0 henry     (1000) henry     (1000)     1575 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_version_cls.py
--rw-r-----   0 henry     (1000) henry     (1000)     7237 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/config.py
--rw-r-----   0 henry     (1000) henry     (1000)     1867 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/discover.py
--rw-r-----   0 henry     (1000) henry     (1000)     3100 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py
--rw-r-----   0 henry     (1000) henry     (1000)     4287 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py
--rw-r-----   0 henry     (1000) henry     (1000)     2293 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py
--rw-r-----   0 henry     (1000) henry     (1000)     9599 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py
--rw-r-----   0 henry     (1000) henry     (1000)     1776 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hacks.py
--rw-r-----   0 henry     (1000) henry     (1000)     6128 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg.py
--rw-r-----   0 henry     (1000) henry     (1000)     4166 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py
--rw-r-----   0 henry     (1000) henry     (1000)     3620 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/integration.py
--rw-r-----   0 henry     (1000) henry     (1000)      585 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py
--rw-r-----   0 henry     (1000) henry     (1000)     5117 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py
--rw-r-----   0 henry     (1000) henry     (1000)    17034 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/version.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.599576 hgutilities-1.0.8.6/.github/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.652040 hgutilities-1.0.8.6/.github/workflows/
--rw-r-----   0 henry     (1000) henry     (1000)     1084 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/.github/workflows/python-publish.yml
--rw-r-----   0 henry     (1000) henry     (1000)    35149 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/LICENSE.md
--rw-r-----   0 henry     (1000) henry     (1000)     7813 2023-06-19 17:20:30.757745 hgutilities-1.0.8.6/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     7148 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/README.md
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.652530 hgutilities-1.0.8.6/hgutilities/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.655966 hgutilities-1.0.8.6/hgutilities/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)     2483 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/Documentation/hgutilities.txt
--rw-r-----   0 henry     (1000) henry     (1000)      154 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.656488 hgutilities-1.0.8.6/hgutilities/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      368 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/__pycache__/__init__.cpython-310.pyc
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.659893 hgutilities-1.0.8.6/hgutilities/defaults/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.665316 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      614 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/defaults.txt
--rw-r-----   0 henry     (1000) henry     (1000)      701 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/docs.txt
--rw-r-----   0 henry     (1000) henry     (1000)      353 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/inherit.txt
--rw-r-----   0 henry     (1000) henry     (1000)      608 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/loaddefaults.txt
--rw-r-----   0 henry     (1000) henry     (1000)      524 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/Documentation/processkwargs.txt
--rw-r-----   0 henry     (1000) henry     (1000)      239 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.669866 hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      448 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3821 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/docs.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      765 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2281 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3202 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2962 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/docs.py
--rw-r-----   0 henry     (1000) henry     (1000)      671 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/inherit.py
--rw-r-----   0 henry     (1000) henry     (1000)     1562 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/loaddefaults.py
--rw-r-----   0 henry     (1000) henry     (1000)     2571 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/defaults/processkwargs.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.676108 hgutilities-1.0.8.6/hgutilities/plotting/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.680549 hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/
--rw-r-----   0 henry     (1000) henry     (1000)      195 2023-06-18 19:27:52.000000 hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/Animate.txt
--rw-r-----   0 henry     (1000) henry     (1000)      842 2023-06-19 13:58:26.000000 hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/Figure.txt
--rw-r-----   0 henry     (1000) henry     (1000)      366 2023-06-19 13:52:51.000000 hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/Figures.txt
--rw-r-----   0 henry     (1000) henry     (1000)       73 2023-06-19 17:09:56.000000 hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/Quick.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.686577 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)      581 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/Animate.txt
--rw-r-----   0 henry     (1000) henry     (1000)      414 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/Figure.txt
--rw-r-----   0 henry     (1000) henry     (1000)      564 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/Figures.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)      791 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/create_animations.txt
--rw-r-----   0 henry     (1000) henry     (1000)      612 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/create_figures.txt
--rw-r-----   0 henry     (1000) henry     (1000)     1155 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/Documentation/plotting.txt
--rw-r-----   0 henry     (1000) henry     (1000)    12516 2023-06-19 16:24:29.000000 hgutilities-1.0.8.6/hgutilities/plotting/README.md
--rw-r-----   0 henry     (1000) henry     (1000)     1220 2023-06-19 15:37:00.000000 hgutilities-1.0.8.6/hgutilities/plotting/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.692022 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)     1193 2023-06-19 15:39:42.000000 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4083 2023-06-18 19:35:30.000000 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/animate.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     7823 2023-06-19 14:01:32.000000 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/figure.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3985 2023-06-19 17:06:30.000000 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/figures.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      770 2023-06-19 17:02:15.000000 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5885 2023-06-19 17:16:52.000000 hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/quick.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2936 2023-06-18 19:35:17.000000 hgutilities-1.0.8.6/hgutilities/plotting/animate.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.700248 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.708011 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/
--rw-r-----   0 henry     (1000) henry     (1000)      283 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Bar.txt
--rw-r-----   0 henry     (1000) henry     (1000)      183 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Bars.txt
--rw-r-----   0 henry     (1000) henry     (1000)      738 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
--rw-r-----   0 henry     (1000) henry     (1000)      762 2023-06-19 12:08:59.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Data.txt
--rw-r-----   0 henry     (1000) henry     (1000)     1135 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Line.txt
--rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Lines.txt
--rw-r-----   0 henry     (1000) henry     (1000)      355 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Pie.txt
--rw-r-----   0 henry     (1000) henry     (1000)      582 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Surface.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.715365 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)      664 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Bar.txt
--rw-r-----   0 henry     (1000) henry     (1000)      869 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Bars.txt
--rw-r-----   0 henry     (1000) henry     (1000)      365 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Colormap.txt
--rw-r-----   0 henry     (1000) henry     (1000)      762 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Data.txt
--rw-r-----   0 henry     (1000) henry     (1000)      659 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Line.txt
--rw-r-----   0 henry     (1000) henry     (1000)     1210 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Lines.txt
--rw-r-----   0 henry     (1000) henry     (1000)      656 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Pie.txt
--rw-r-----   0 henry     (1000) henry     (1000)      859 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Surface.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.722747 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      581 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1564 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1304 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      731 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      590 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2260 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      813 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1657 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      229 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/bar.py
--rw-r-----   0 henry     (1000) henry     (1000)     1025 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/bars.py
--rw-r-----   0 henry     (1000) henry     (1000)      872 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/colorplot.py
--rw-r-----   0 henry     (1000) henry     (1000)      255 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/data.py
--rw-r-----   0 henry     (1000) henry     (1000)      232 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/line.py
--rw-r-----   0 henry     (1000) henry     (1000)     1677 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/lines.py
--rw-r-----   0 henry     (1000) henry     (1000)      387 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/pie.py
--rw-r-----   0 henry     (1000) henry     (1000)     1014 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/datatypes/surface.py
--rw-r-----   0 henry     (1000) henry     (1000)     6162 2023-06-19 13:54:04.000000 hgutilities-1.0.8.6/hgutilities/plotting/figure.py
--rw-r-----   0 henry     (1000) henry     (1000)     2944 2023-06-19 17:04:36.000000 hgutilities-1.0.8.6/hgutilities/plotting/figures.py
--rw-r-----   0 henry     (1000) henry     (1000)      545 2023-06-19 17:02:12.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotfunctions.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.729345 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.731277 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/Documentation/
--rw-r-----   0 henry     (1000) henry     (1000)      508 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/Documentation/Plot.txt
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/Documentation/__init__.py
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.738251 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5316 2023-06-19 14:01:33.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3938 2023-06-18 20:06:55.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2030 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4790 2023-06-19 14:01:33.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1377 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     3246 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     4997 2023-06-19 13:15:58.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plot.py
--rw-r-----   0 henry     (1000) henry     (1000)     3530 2023-06-18 20:06:50.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotbars.py
--rw-r-----   0 henry     (1000) henry     (1000)     2671 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotcolorplot.py
--rw-r-----   0 henry     (1000) henry     (1000)     6981 2023-06-19 12:15:57.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotlines.py
--rw-r-----   0 henry     (1000) henry     (1000)     1284 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotpie.py
--rw-r-----   0 henry     (1000) henry     (1000)     3786 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotsurface.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.742595 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.746633 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      197 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1177 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     5394 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1770 2023-06-19 14:04:15.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      719 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/figuresize.py
--rw-r-----   0 henry     (1000) henry     (1000)     4561 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/griddimensions.py
--rw-r-----   0 henry     (1000) henry     (1000)     4541 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/plotshape.py
--rw-r-----   0 henry     (1000) henry     (1000)     1789 2023-06-19 14:04:01.000000 hgutilities-1.0.8.6/hgutilities/plotting/plotutils/savefigure.py
--rw-r-----   0 henry     (1000) henry     (1000)     4591 2023-06-19 17:16:47.000000 hgutilities-1.0.8.6/hgutilities/plotting/quick.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.752362 hgutilities-1.0.8.6/hgutilities/utils/
--rw-r-----   0 henry     (1000) henry     (1000)        0 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/utils/__init__.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.756875 hgutilities-1.0.8.6/hgutilities/utils/__pycache__/
--rw-r-----   0 henry     (1000) henry     (1000)      184 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/utils/__pycache__/__init__.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      511 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/utils/__pycache__/dicts.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2048 2023-06-18 19:09:39.000000 hgutilities-1.0.8.6/hgutilities/utils/__pycache__/groups.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     1422 2023-06-18 19:09:38.000000 hgutilities-1.0.8.6/hgutilities/utils/__pycache__/paths.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)     2242 2023-06-19 16:46:20.000000 hgutilities-1.0.8.6/hgutilities/utils/__pycache__/readwrite.cpython-310.pyc
--rw-r-----   0 henry     (1000) henry     (1000)      191 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/utils/dicts.py
--rw-r-----   0 henry     (1000) henry     (1000)     2373 2023-06-14 13:20:48.000000 hgutilities-1.0.8.6/hgutilities/utils/filenames.py
--rw-r-----   0 henry     (1000) henry     (1000)     1830 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/utils/groups.py
--rw-r-----   0 henry     (1000) henry     (1000)      927 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/utils/paths.py
--rw-r-----   0 henry     (1000) henry     (1000)      668 2023-06-18 19:06:03.000000 hgutilities-1.0.8.6/hgutilities/utils/plots.py
--rw-r-----   0 henry     (1000) henry     (1000)     1154 2023-06-14 13:31:22.000000 hgutilities-1.0.8.6/hgutilities/utils/readwrite.py
-drwxr-x---   0 henry     (1000) henry     (1000)        0 2023-06-19 17:20:30.654995 hgutilities-1.0.8.6/hgutilities.egg-info/
--rw-r-----   0 henry     (1000) henry     (1000)     7813 2023-06-19 17:20:30.000000 hgutilities-1.0.8.6/hgutilities.egg-info/PKG-INFO
--rw-r-----   0 henry     (1000) henry     (1000)     9505 2023-06-19 17:20:30.000000 hgutilities-1.0.8.6/hgutilities.egg-info/SOURCES.txt
--rw-r-----   0 henry     (1000) henry     (1000)        1 2023-06-19 17:20:30.000000 hgutilities-1.0.8.6/hgutilities.egg-info/dependency_links.txt
--rw-r-----   0 henry     (1000) henry     (1000)       35 2023-06-19 17:20:30.000000 hgutilities-1.0.8.6/hgutilities.egg-info/requires.txt
--rw-r-----   0 henry     (1000) henry     (1000)       12 2023-06-19 17:20:30.000000 hgutilities-1.0.8.6/hgutilities.egg-info/top_level.txt
--rw-r-----   0 henry     (1000) henry     (1000)       38 2023-06-19 17:20:30.758332 hgutilities-1.0.8.6/setup.cfg
--rw-r-----   0 henry     (1000) henry     (1000)     1455 2023-06-19 13:29:22.000000 hgutilities-1.0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.418915 hgutilities-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.184246 hgutilities-1.0.9/.eggs/
+-rw-rw-rw-   0        0        0      217 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.171455 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.194980 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/
+-rw-rw-rw-   0        0        0     1040 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE
+-rw-rw-rw-   0        0        0    25546 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO
+-rw-rw-rw-   0        0        0     2605 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD
+-rw-rw-rw-   0        0        0       97 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/WHEEL
+-rw-rw-rw-   0        0        0     1776 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt
+-rw-rw-rw-   0        0        0      112 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.237185 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/
+-rw-rw-rw-   0        0        0     6082 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__init__.py
+-rw-rw-rw-   0        0        0      104 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.253467 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/
+-rw-rw-rw-   0        0        0     7504 2023-06-20 08:48:29.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4951 2023-06-20 08:48:29.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1622 2023-06-20 08:48:29.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2622 2023-06-20 08:48:29.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10354 2023-06-20 08:48:29.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3074 2023-06-20 08:48:29.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5153 2023-06-20 08:48:30.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6542 2023-06-20 08:48:30.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5581 2023-06-20 08:48:29.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10214 2023-06-20 08:48:29.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0    24829 2023-06-20 08:48:29.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2931 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_cli.py
+-rw-rw-rw-   0        0        0     2795 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_entrypoints.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.254464 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/
+-rw-rw-rw-   0        0        0        0 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.256458 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/
+-rw-rw-rw-   0        0        0      240 2023-06-20 08:48:29.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4743 2023-06-20 08:48:29.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1178 2023-06-20 08:48:29.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2933 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py
+-rw-rw-rw-   0        0        0      552 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/setuptools.py
+-rw-rw-rw-   0        0        0     1105 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py
+-rw-rw-rw-   0        0        0      887 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py
+-rw-rw-rw-   0        0        0     1623 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_version_cls.py
+-rw-rw-rw-   0        0        0     7453 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/config.py
+-rw-rw-rw-   0        0        0     1936 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/discover.py
+-rw-rw-rw-   0        0        0     3186 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py
+-rw-rw-rw-   0        0        0     4408 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py
+-rw-rw-rw-   0        0        0     2367 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py
+-rw-rw-rw-   0        0        0     9922 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py
+-rw-rw-rw-   0        0        0     1833 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hacks.py
+-rw-rw-rw-   0        0        0     6323 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg.py
+-rw-rw-rw-   0        0        0     4312 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py
+-rw-rw-rw-   0        0        0     3747 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/integration.py
+-rw-rw-rw-   0        0        0      611 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py
+-rw-rw-rw-   0        0        0     5297 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py
+-rw-rw-rw-   0        0        0    17597 2023-06-20 08:46:11.000000 hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/version.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.172447 hgutilities-1.0.9/.github/
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.260443 hgutilities-1.0.9/.github/workflows/
+-rw-rw-rw-   0        0        0     1123 2023-06-16 10:32:25.000000 hgutilities-1.0.9/.github/workflows/python-publish.yml
+-rw-rw-rw-   0        0        0    35823 2023-06-16 10:32:25.000000 hgutilities-1.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0     7982 2023-06-20 08:48:30.418915 hgutilities-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7224 2023-06-16 10:32:25.000000 hgutilities-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.260443 hgutilities-1.0.9/hgutilities/
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.278744 hgutilities-1.0.9/hgutilities/Documentation/
+-rw-rw-rw-   0        0        0        0 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/Documentation/__init__.py
+-rw-rw-rw-   0        0        0     2505 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/Documentation/hgutilities.txt
+-rw-rw-rw-   0        0        0      163 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.279741 hgutilities-1.0.9/hgutilities/__pycache__/
+-rw-rw-rw-   0        0        0      368 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/__pycache__/__init__.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.281733 hgutilities-1.0.9/hgutilities/defaults/
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.298430 hgutilities-1.0.9/hgutilities/defaults/Documentation/
+-rw-rw-rw-   0        0        0        0 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/defaults/Documentation/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/defaults/Documentation/defaults.txt
+-rw-rw-rw-   0        0        0      715 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/defaults/Documentation/docs.txt
+-rw-rw-rw-   0        0        0      361 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/defaults/Documentation/inherit.txt
+-rw-rw-rw-   0        0        0      625 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/defaults/Documentation/loaddefaults.txt
+-rw-rw-rw-   0        0        0      537 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/defaults/Documentation/processkwargs.txt
+-rw-rw-rw-   0        0        0      239 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.301395 hgutilities-1.0.9/hgutilities/defaults/__pycache__/
+-rw-rw-rw-   0        0        0      448 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/defaults/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3821 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/defaults/__pycache__/docs.cpython-310.pyc
+-rw-rw-rw-   0        0        0      765 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2281 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3202 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2962 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/defaults/docs.py
+-rw-rw-rw-   0        0        0      671 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/defaults/inherit.py
+-rw-rw-rw-   0        0        0     1562 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/defaults/loaddefaults.py
+-rw-rw-rw-   0        0        0     2571 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/defaults/processkwargs.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.308184 hgutilities-1.0.9/hgutilities/plotting/
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.319150 hgutilities-1.0.9/hgutilities/plotting/Default Settings/
+-rw-rw-rw-   0        0        0      195 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/Default Settings/Animate.txt
+-rw-rw-rw-   0        0        0      842 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/Default Settings/Figure.txt
+-rw-rw-rw-   0        0        0      366 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/Default Settings/Figures.txt
+-rw-rw-rw-   0        0        0       79 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/Default Settings/Quick.txt
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/Default Settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.338597 hgutilities-1.0.9/hgutilities/plotting/Documentation/
+-rw-rw-rw-   0        0        0      598 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/Documentation/Animate.txt
+-rw-rw-rw-   0        0        0      424 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/Documentation/Figure.txt
+-rw-rw-rw-   0        0        0      579 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/Documentation/Figures.txt
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/Documentation/__init__.py
+-rw-rw-rw-   0        0        0      811 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/Documentation/create_animations.txt
+-rw-rw-rw-   0        0        0      628 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/Documentation/create_figures.txt
+-rw-rw-rw-   0        0        0     1180 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/Documentation/plotting.txt
+-rw-rw-rw-   0        0        0    12516 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/README.md
+-rw-rw-rw-   0        0        0     1220 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.342229 hgutilities-1.0.9/hgutilities/plotting/__pycache__/
+-rw-rw-rw-   0        0        0     1193 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4083 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/__pycache__/animate.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7823 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/__pycache__/figure.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3985 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/__pycache__/figures.cpython-310.pyc
+-rw-rw-rw-   0        0        0      770 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5885 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/__pycache__/quick.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2936 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/animate.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.346215 hgutilities-1.0.9/hgutilities/plotting/datatypes/
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.368544 hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/
+-rw-rw-rw-   0        0        0      283 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/Bar.txt
+-rw-rw-rw-   0        0        0      183 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/Bars.txt
+-rw-rw-rw-   0        0        0      738 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
+-rw-rw-rw-   0        0        0      762 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/Data.txt
+-rw-rw-rw-   0        0        0     1135 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/Line.txt
+-rw-rw-rw-   0        0        0      191 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/Lines.txt
+-rw-rw-rw-   0        0        0      355 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/Pie.txt
+-rw-rw-rw-   0        0        0      582 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/Surface.txt
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.392061 hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/
+-rw-rw-rw-   0        0        0      677 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Bar.txt
+-rw-rw-rw-   0        0        0      887 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Bars.txt
+-rw-rw-rw-   0        0        0      374 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Colormap.txt
+-rw-rw-rw-   0        0        0      782 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Data.txt
+-rw-rw-rw-   0        0        0      674 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Line.txt
+-rw-rw-rw-   0        0        0     1232 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Lines.txt
+-rw-rw-rw-   0        0        0      670 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Pie.txt
+-rw-rw-rw-   0        0        0      872 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Surface.txt
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.397041 hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/
+-rw-rw-rw-   0        0        0      197 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      581 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1564 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1304 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc
+-rw-rw-rw-   0        0        0      731 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc
+-rw-rw-rw-   0        0        0      590 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2260 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc
+-rw-rw-rw-   0        0        0      813 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1657 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc
+-rw-rw-rw-   0        0        0      229 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/bar.py
+-rw-rw-rw-   0        0        0     1025 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/bars.py
+-rw-rw-rw-   0        0        0      872 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/colorplot.py
+-rw-rw-rw-   0        0        0      255 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/data.py
+-rw-rw-rw-   0        0        0      232 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/line.py
+-rw-rw-rw-   0        0        0     1677 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/lines.py
+-rw-rw-rw-   0        0        0      387 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/pie.py
+-rw-rw-rw-   0        0        0     1014 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/datatypes/surface.py
+-rw-rw-rw-   0        0        0     6162 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/figure.py
+-rw-rw-rw-   0        0        0     2944 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/figures.py
+-rw-rw-rw-   0        0        0      545 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plotfunctions.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.400030 hgutilities-1.0.9/hgutilities/plotting/plottypes/
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.404018 hgutilities-1.0.9/hgutilities/plotting/plottypes/Documentation/
+-rw-rw-rw-   0        0        0      508 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/Documentation/Plot.txt
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/Documentation/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.408003 hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/
+-rw-rw-rw-   0        0        0      197 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5316 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3938 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2030 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4790 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1377 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3246 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4997 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/plot.py
+-rw-rw-rw-   0        0        0     3530 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/plotbars.py
+-rw-rw-rw-   0        0        0     2671 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/plotcolorplot.py
+-rw-rw-rw-   0        0        0     6981 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/plotlines.py
+-rw-rw-rw-   0        0        0     1284 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/plotpie.py
+-rw-rw-rw-   0        0        0     3786 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plottypes/plotsurface.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.409997 hgutilities-1.0.9/hgutilities/plotting/plotutils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:14:15.000000 hgutilities-1.0.9/hgutilities/plotting/plotutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.412935 hgutilities-1.0.9/hgutilities/plotting/plotutils/__pycache__/
+-rw-rw-rw-   0        0        0      197 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plotutils/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1177 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5394 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1770 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc
+-rw-rw-rw-   0        0        0      719 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plotutils/figuresize.py
+-rw-rw-rw-   0        0        0     4561 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plotutils/griddimensions.py
+-rw-rw-rw-   0        0        0     4541 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plotutils/plotshape.py
+-rw-rw-rw-   0        0        0     1789 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/plotutils/savefigure.py
+-rw-rw-rw-   0        0        0     4719 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/plotting/quick.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.415925 hgutilities-1.0.9/hgutilities/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.417918 hgutilities-1.0.9/hgutilities/utils/__pycache__/
+-rw-rw-rw-   0        0        0      184 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/utils/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      511 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/utils/__pycache__/dicts.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2048 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/utils/__pycache__/groups.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1422 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/utils/__pycache__/paths.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2242 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/utils/__pycache__/readwrite.cpython-310.pyc
+-rw-rw-rw-   0        0        0      195 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/utils/dicts.py
+-rw-rw-rw-   0        0        0     2373 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/utils/filenames.py
+-rw-rw-rw-   0        0        0     1877 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/utils/groups.py
+-rw-rw-rw-   0        0        0      961 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/utils/paths.py
+-rw-rw-rw-   0        0        0      697 2023-06-16 10:32:25.000000 hgutilities-1.0.9/hgutilities/utils/plots.py
+-rw-rw-rw-   0        0        0     1154 2023-06-20 08:46:17.000000 hgutilities-1.0.9/hgutilities/utils/readwrite.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:48:30.273761 hgutilities-1.0.9/hgutilities.egg-info/
+-rw-rw-rw-   0        0        0     7982 2023-06-20 08:48:30.000000 hgutilities-1.0.9/hgutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9505 2023-06-20 08:48:30.000000 hgutilities-1.0.9/hgutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:48:30.000000 hgutilities-1.0.9/hgutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-20 08:48:30.000000 hgutilities-1.0.9/hgutilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 08:48:30.000000 hgutilities-1.0.9/hgutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:48:30.418915 hgutilities-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1491 2023-06-20 08:46:33.000000 hgutilities-1.0.9/setup.py
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/PKG-INFO`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,710 +1,710 @@
-Metadata-Version: 2.1
-Name: setuptools-scm
-Version: 7.1.0
-Summary: the blessed package to manage your versions by scm tags
-Home-page: https://github.com/pypa/setuptools_scm/
-Author: Ronny Pfannschmidt
-Author-email: opensource@ronnypfannschmidt.de
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Version Control
-Classifier: Topic :: System :: Software Distribution
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: packaging (>=20.0)
-Requires-Dist: setuptools
-Requires-Dist: typing-extensions
-Requires-Dist: tomli (>=1.0.0) ; python_version < "3.11"
-Requires-Dist: importlib-metadata ; python_version < "3.8"
-Provides-Extra: test
-Requires-Dist: pytest (>=6.2) ; extra == 'test'
-Requires-Dist: virtualenv (>20) ; extra == 'test'
-Provides-Extra: toml
-Requires-Dist: setuptools (>=42) ; extra == 'toml'
-
-setuptools_scm
-==============
-
-``setuptools_scm`` extracts Python package versions from ``git`` or
-``hg`` metadata instead of declaring them as the version argument
-or in a SCM managed file.
-
-Additionally ``setuptools_scm`` provides setuptools with a list of
-files that are managed by the SCM (i.e. it automatically adds all of
-the SCM-managed files to the sdist). Unwanted files must be excluded
-by discarding them via ``MANIFEST.in``.
-
-``setuptools_scm`` supports the following scm out of the box:
-
-* git
-* mercurial
-
-.. image:: https://github.com/pypa/setuptools_scm/workflows/python%20tests+artifacts+release/badge.svg
-    :target: https://github.com/pypa/setuptools_scm/actions
-
-.. image:: https://tidelift.com/badges/package/pypi/setuptools-scm
-   :target: https://tidelift.com/subscription/pkg/pypi-setuptools-scm?utm_source=pypi-setuptools-scm&utm_medium=readme
-
-
-``pyproject.toml`` usage
-------------------------
-
-The preferred way to configure ``setuptools_scm`` is to author
-settings in a ``tool.setuptools_scm`` section of ``pyproject.toml``.
-
-This feature requires Setuptools 42 or later, released in Nov, 2019.
-If your project needs to support build from sdist on older versions
-of Setuptools, you will need to also implement the ``setup.py usage``
-for those legacy environments.
-
-First, ensure that ``setuptools_scm`` is present during the project's
-built step by specifying it as one of the build requirements.
-
-.. code:: toml
-
-    # pyproject.toml
-    [build-system]
-    requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
-
-That will be sufficient to require ``setuptools_scm`` for projects
-that support PEP 518 (`pip <https://pypi.org/project/pip>`_ and
-`pep517 <https://pypi.org/project/pep517/>`_). Many tools,
-especially those that invoke ``setup.py`` for any reason, may
-continue to rely on ``setup_requires``. For maximum compatibility
-with those uses, consider also including a ``setup_requires`` directive
-(described below in ``setup.py usage`` and ``setup.cfg``).
-
-To enable version inference, you need to set the version
-dynamically in the ``project`` section of ``pyproject.toml``:
-
-.. code:: toml
-
-    # pyproject.toml
-    [project]
-    # version = "0.0.1"  # Remove any existing version parameter.
-    dynamic = ["version"]
-
-Then add this section to your ``pyproject.toml``:
-
-.. code:: toml
-
-    # pyproject.toml
-    [tool.setuptools_scm]
-
-Including this section is comparable to supplying
-``use_scm_version=True`` in ``setup.py``. Additionally,
-include arbitrary keyword arguments in that section
-to be supplied to ``get_version()``. For example:
-
-.. code:: toml
-
-    # pyproject.toml
-    [tool.setuptools_scm]
-    write_to = "pkg/_version.py"
-
-Where ``pkg`` is the name of your package.
-
-If you need to confirm which version string is being generated
-or debug the configuration, you can install
-`setuptools-scm <https://github.com/pypa/setuptools_scm>`_
-directly in your working environment and run:
-
-.. code-block:: shell
-
-    $ python -m setuptools_scm
-
-    # To explore other options, try:
-    $ python -m setuptools_scm --help
-
-
-``setup.py`` usage (deprecated)
--------------------------------
-
-.. warning::
-
-   ``setup_requires`` has been deprecated in favor of ``pyproject.toml``
-
-The following settings are considered legacy behavior and
-superseded by the ``pyproject.toml`` usage, but for maximal
-compatibility, projects may also supply the configuration in
-this older form.
-
-To use ``setuptools_scm`` just modify your project's ``setup.py`` file
-like this:
-
-* Add ``setuptools_scm`` to the ``setup_requires`` parameter.
-* Add the ``use_scm_version`` parameter and set it to ``True``.
-
-For example:
-
-.. code:: python
-
-    from setuptools import setup
-    setup(
-        ...,
-        use_scm_version=True,
-        setup_requires=['setuptools_scm'],
-        ...,
-    )
-
-Arguments to ``get_version()`` (see below) may be passed as a dictionary to
-``use_scm_version``. For example:
-
-.. code:: python
-
-    from setuptools import setup
-    setup(
-        ...,
-        use_scm_version = {
-            "root": "..",
-            "relative_to": __file__,
-            "local_scheme": "node-and-timestamp"
-        },
-        setup_requires=['setuptools_scm'],
-        ...,
-    )
-
-You can confirm the version number locally via ``setup.py``:
-
-.. code-block:: shell
-
-    $ python setup.py --version
-
-.. note::
-
-   If you see unusual version numbers for packages but ``python setup.py
-   --version`` reports the expected version number, ensure ``[egg_info]`` is
-   not defined in ``setup.cfg``.
-
-
-``setup.cfg`` usage (deprecated)
-------------------------------------
-
-as ``setup_requires`` is deprecated in favour of ``pyproject.toml``
-usage in ``setup.cfg`` is considered deprecated,
-please use ``pyproject.toml`` whenever possible.
-
-
-Programmatic usage
-------------------
-
-In order to use ``setuptools_scm`` from code that is one directory deeper
-than the project's root, you can use:
-
-.. code:: python
-
-    from setuptools_scm import get_version
-    version = get_version(root='..', relative_to=__file__)
-
-See `setup.py Usage (deprecated)`_ above for how to use this within ``setup.py``.
-
-
-Retrieving package version at runtime
--------------------------------------
-
-If you have opted not to hardcode the version number inside the package,
-you can retrieve it at runtime from PEP-0566_ metadata using
-``importlib.metadata`` from the standard library (added in Python 3.8)
-or the `importlib_metadata`_ backport:
-
-.. code:: python
-
-    from importlib.metadata import version, PackageNotFoundError
-
-    try:
-        __version__ = version("package-name")
-    except PackageNotFoundError:
-        # package is not installed
-        pass
-
-Alternatively, you can use ``pkg_resources`` which is included in
-``setuptools`` (but has a significant runtime cost):
-
-.. code:: python
-
-   from pkg_resources import get_distribution, DistributionNotFound
-
-   try:
-       __version__ = get_distribution("package-name").version
-   except DistributionNotFound:
-        # package is not installed
-       pass
-
-However, this does place a runtime dependency on ``setuptools`` and can add up to
-a few 100ms overhead for the package import time.
-
-.. _PEP-0566: https://www.python.org/dev/peps/pep-0566/
-.. _importlib_metadata: https://pypi.org/project/importlib-metadata/
-
-
-Usage from Sphinx
------------------
-
-It is discouraged to use ``setuptools_scm`` from Sphinx itself,
-instead use ``importlib.metadata`` after editable/real installation:
-
-.. code:: python
-
-    # contents of docs/conf.py
-    from importlib.metadata import version
-    release = version('myproject')
-    # for example take major/minor
-    version = '.'.join(release.split('.')[:2])
-
-The underlying reason is, that services like *Read the Docs* sometimes change
-the working directory for good reasons and using the installed metadata
-prevents using needless volatile data there.
-
-
-Usage from Docker
------------------
-
-By default, docker will not copy the ``.git``  folder into your container.
-Therefore, builds with version inference might fail.
-Consequently, you can use the following snipped to infer the version from
-the host os without copying the entire ``.git`` folder to your Dockerfile.
-
-.. code:: dockerfile
-
-    RUN --mount=source=.git,target=.git,type=bind \
-        pip install --no-cache-dir -e .
-
-However, this build step introduces a dependency to the state of your local
-.git folder the build cache and triggers the long-running pip install process on every build.
-To optimize build caching, one can use an environment variable to pretend a pseudo
-version that is used to cache the results of the pip install process:
-
-.. code:: dockerfile
-
-    FROM python
-    COPY pyproject.toml
-    ARG PSEUDO_VERSION=1
-    RUN SETUPTOOLS_SCM_PRETEND_VERSION=${PSEUDO_VERSION} pip install -e .[test]
-    RUN --mount=source=.git,target=.git,type=bind pip install -e .
-
-Note that running this Dockerfile requires docker with BuildKit enabled
-`[docs] <https://github.com/moby/buildkit/blob/v0.8.3/frontend/dockerfile/docs/syntax.md>`_.
-
-To avoid BuildKit and mounting of the .git folder altogether, one can also pass the desired
-version as a build argument. Note that ``SETUPTOOLS_SCM_PRETEND_VERSION_FOR_${UPPERCASED_DIST_NAME}``
-is preferred over ``SETUPTOOLS_SCM_PRETEND_VERSION``.
-
-
-Default versioning scheme
--------------------------
-
-In the standard configuration ``setuptools_scm`` takes a look at three things:
-
-1. latest tag (with a version number)
-2. the distance to this tag (e.g. number of revisions since latest tag)
-3. workdir state (e.g. uncommitted changes since latest tag)
-
-and uses roughly the following logic to render the version:
-
-no distance and clean:
-    ``{tag}``
-distance and clean:
-    ``{next_version}.dev{distance}+{scm letter}{revision hash}``
-no distance and not clean:
-    ``{tag}+dYYYYMMDD``
-distance and not clean:
-    ``{next_version}.dev{distance}+{scm letter}{revision hash}.dYYYYMMDD``
-
-The next version is calculated by adding ``1`` to the last numeric component of
-the tag.
-
-For Git projects, the version relies on `git describe <https://git-scm.com/docs/git-describe>`_,
-so you will see an additional ``g`` prepended to the ``{revision hash}``.
-
-
-Semantic Versioning (SemVer)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Due to the default behavior it's necessary to always include a
-patch version (the ``3`` in ``1.2.3``), or else the automatic guessing
-will increment the wrong part of the SemVer (e.g. tag ``2.0`` results in
-``2.1.devX`` instead of ``2.0.1.devX``). So please make sure to tag
-accordingly.
-
-.. note::
-
-    Future versions of ``setuptools_scm`` will switch to `SemVer
-    <http://semver.org/>`_ by default hiding the the old behavior as an
-    configurable option.
-
-
-Builtin mechanisms for obtaining version numbers
-------------------------------------------------
-
-1. the SCM itself (git/hg)
-2. ``.hg_archival`` files (mercurial archives)
-3. ``.git_archival.txt`` files (git archives, see subsection below)
-4. ``PKG-INFO``
-
-
-Git archives
-~~~~~~~~~~~~
-
-Git archives are supported, but a few changes to your repository are required.
-
-Create a ``.git_archival.txt`` file in the root directory of your repository,
-and copy-paste this into it::
-
-    node: $Format:%H$
-    node-date: $Format:%cI$
-    describe-name: $Format:%(describe:tags=true,match=*[0-9]*)$
-    ref-names: $Format:%D$
-
-Create the ``.gitattributes`` file in the root directory of your repository
-if it doesn't already exist, and copy-paste this into it::
-
-    .git_archival.txt  export-subst
-
-Finally, don't forget to commit those two files::
-
-    git add .git_archival.txt .gitattributes && git commit
-
-Note that if you are creating a ``_version.py`` file, note that it should not
-be kept in version control.
-
-
-File finders hook makes most of MANIFEST.in unnecessary
--------------------------------------------------------
-
-``setuptools_scm`` implements a `file_finders
-<https://setuptools.pypa.io/en/latest/userguide/extension.html#adding-support-for-revision-control-systems>`_
-entry point which returns all files tracked by your SCM. This eliminates
-the need for a manually constructed ``MANIFEST.in`` in most cases where this
-would be required when not using ``setuptools_scm``, namely:
-
-* To ensure all relevant files are packaged when running the ``sdist`` command.
-
-* When using `include_package_data <https://setuptools.readthedocs.io/en/latest/setuptools.html#including-data-files>`_
-  to include package data as part of the ``build`` or ``bdist_wheel``.
-
-``MANIFEST.in`` may still be used: anything defined there overrides the hook.
-This is mostly useful to exclude files tracked in your SCM from packages,
-although in principle it can be used to explicitly include non-tracked files
-too.
-
-
-Configuration parameters
-------------------------
-
-In order to configure the way ``use_scm_version`` works you can provide
-a mapping with options instead of a boolean value.
-
-The currently supported configuration keys are:
-
-:root:
-    Relative path to cwd, used for finding the SCM root; defaults to ``.``
-
-:version_scheme:
-    Configures how the local version number is constructed; either an
-    entrypoint name or a callable.
-
-:local_scheme:
-    Configures how the local component of the version is constructed; either an
-    entrypoint name or a callable.
-
-:write_to:
-    A path to a file that gets replaced with a file containing the current
-    version. It is ideal for creating a ``_version.py`` file within the
-    package, typically used to avoid using `pkg_resources.get_distribution`
-    (which adds some overhead).
-
-    .. warning::
-
-      Only files with :code:`.py` and :code:`.txt` extensions have builtin
-      templates, for other file types it is necessary to provide
-      :code:`write_to_template`.
-
-:write_to_template:
-    A newstyle format string that is given the current version as
-    the ``version`` keyword argument for formatting.
-
-:relative_to:
-    A file from which the root can be resolved.
-    Typically called by a script or module that is not in the root of the
-    repository to point ``setuptools_scm`` at the root of the repository by
-    supplying ``__file__``.
-
-:tag_regex:
-   A Python regex string to extract the version part from any SCM tag.
-    The regex needs to contain either a single match group, or a group
-    named ``version``, that captures the actual version information.
-
-    Defaults to the value of ``setuptools_scm.config.DEFAULT_TAG_REGEX``
-    (see `config.py <src/setuptools_scm/config.py>`_).
-
-:parentdir_prefix_version:
-    If the normal methods for detecting the version (SCM version,
-    sdist metadata) fail, and the parent directory name starts with
-    ``parentdir_prefix_version``, then this prefix is stripped and the rest of
-    the parent directory name is matched with ``tag_regex`` to get a version
-    string.  If this parameter is unset (the default), then this fallback is
-    not used.
-
-    This is intended to cover GitHub's "release tarballs", which extract into
-    directories named ``projectname-tag/`` (in which case
-    ``parentdir_prefix_version`` can be set e.g. to ``projectname-``).
-
-:fallback_version:
-    A version string that will be used if no other method for detecting the
-    version worked (e.g., when using a tarball with no metadata). If this is
-    unset (the default), setuptools_scm will error if it fails to detect the
-    version.
-
-:parse:
-    A function that will be used instead of the discovered SCM for parsing the
-    version.
-    Use with caution, this is a function for advanced use, and you should be
-    familiar with the ``setuptools_scm`` internals to use it.
-
-:git_describe_command:
-    This command will be used instead the default ``git describe`` command.
-    Use with caution, this is a function for advanced use, and you should be
-    familiar with the ``setuptools_scm`` internals to use it.
-
-    Defaults to the value set by ``setuptools_scm.git.DEFAULT_DESCRIBE``
-    (see `git.py <src/setuptools_scm/git.py>`_).
-
-:normalize:
-    A boolean flag indicating if the version string should be normalized.
-    Defaults to ``True``. Setting this to ``False`` is equivalent to setting
-    ``version_cls`` to ``setuptools_scm.version.NonNormalizedVersion``
-
-:version_cls:
-    An optional class used to parse, verify and possibly normalize the version
-    string. Its constructor should receive a single string argument, and its
-    ``str`` should return the normalized version string to use.
-    This option can also receive a class qualified name as a string.
-
-    This defaults to ``packaging.version.Version`` if available. If
-    ``packaging`` is not installed, ``pkg_resources.packaging.version.Version``
-    is used. Note that it is known to modify git release candidate schemes.
-
-    The ``setuptools_scm.NonNormalizedVersion`` convenience class is
-    provided to disable the normalization step done by
-    ``packaging.version.Version``. If this is used while ``setuptools_scm``
-    is integrated in a setuptools packaging process, the non-normalized
-    version number will appear in all files (see ``write_to``) BUT note
-    that setuptools will still normalize it to create the final distribution,
-    so as to stay compliant with the python packaging standards.
-
-To use ``setuptools_scm`` in other Python code you can use the ``get_version``
-function:
-
-.. code:: python
-
-    from setuptools_scm import get_version
-    my_version = get_version()
-
-It optionally accepts the keys of the ``use_scm_version`` parameter as
-keyword arguments.
-
-Example configuration in ``setup.py`` format:
-
-.. code:: python
-
-    from setuptools import setup
-
-    setup(
-        use_scm_version={
-            'write_to': '_version.py',
-            'write_to_template': '__version__ = "{version}"',
-            'tag_regex': r'^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$',
-        }
-    )
-
-
-Environment variables
----------------------
-
-:SETUPTOOLS_SCM_PRETEND_VERSION:
-    when defined and not empty,
-    its used as the primary source for the version number
-    in which case it will be a unparsed string
-
-:SETUPTOOLS_SCM_PRETEND_VERSION_FOR_${UPPERCASED_DIST_NAME}:
-    when defined and not empty,
-    its used as the primary source for the version number
-    in which case it will be a unparsed string
-
-    it takes precedence over ``SETUPTOOLS_SCM_PRETEND_VERSION``
-
-:SETUPTOOLS_SCM_DEBUG:
-    when defined and not empty,
-    a lot of debug information will be printed as part of ``setuptools_scm``
-    operating
-
-:SOURCE_DATE_EPOCH:
-    when defined, used as the timestamp from which the
-    ``node-and-date`` and ``node-and-timestamp`` local parts are
-    derived, otherwise the current time is used
-    (https://reproducible-builds.org/docs/source-date-epoch/)
-
-:SETUPTOOLS_SCM_IGNORE_VCS_ROOTS:
-    when defined, a ``os.pathsep`` separated list
-    of directory names to ignore for root finding
-
-
-Extending setuptools_scm
-------------------------
-
-``setuptools_scm`` ships with a few ``setuptools`` entrypoints based hooks to
-extend its default capabilities.
-
-
-Adding a new SCM
-~~~~~~~~~~~~~~~~
-
-``setuptools_scm`` provides two entrypoints for adding new SCMs:
-
-``setuptools_scm.parse_scm``
-    A function used to parse the metadata of the current workdir
-    using the name of the control directory/file of your SCM as the
-    entrypoint's name. E.g. for the built-in entrypoint for git the
-    entrypoint is named ``.git`` and references ``setuptools_scm.git:parse``
-
-  The return value MUST be a ``setuptools_scm.version.ScmVersion`` instance
-  created by the function ``setuptools_scm.version:meta``.
-
-``setuptools_scm.files_command``
-  Either a string containing a shell command that prints all SCM managed
-  files in its current working directory or a callable, that given a
-  pathname will return that list.
-
-  Also use then name of your SCM control directory as name of the entrypoint.
-
-
-Version number construction
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-``setuptools_scm.version_scheme``
-    Configures how the version number is constructed given a
-    ``setuptools_scm.version.ScmVersion`` instance and should return a string
-    representing the version.
-
-    Available implementations:
-
-    :guess-next-dev: Automatically guesses the next development version (default).
-        Guesses the upcoming release by incrementing the pre-release segment if present,
-        otherwise by incrementing the micro segment. Then appends :code:`.devN`.
-        In case the tag ends with ``.dev0`` the version is not bumped
-        and custom ``.devN`` versions will trigger a error.
-    :post-release: generates post release versions (adds :code:`.postN`)
-    :python-simplified-semver: Basic semantic versioning. Guesses the upcoming release
-        by incrementing the minor segment and setting the micro segment to zero if the
-        current branch contains the string ``'feature'``, otherwise by incrementing the
-        micro version. Then appends :code:`.devN`. Not compatible with pre-releases.
-    :release-branch-semver: Semantic versioning for projects with release branches. The
-        same as ``guess-next-dev`` (incrementing the pre-release or micro segment) if on
-        a release branch: a branch whose name (ignoring namespace) parses as a version
-        that matches the most recent tag up to the minor segment. Otherwise if on a
-        non-release branch, increments the minor segment and sets the micro segment to
-        zero, then appends :code:`.devN`.
-    :no-guess-dev: Does no next version guessing, just adds :code:`.post1.devN`
-
-``setuptools_scm.local_scheme``
-    Configures how the local part of a version is rendered given a
-    ``setuptools_scm.version.ScmVersion`` instance and should return a string
-    representing the local version.
-    Dates and times are in Coordinated Universal Time (UTC), because as part
-    of the version, they should be location independent.
-
-    Available implementations:
-
-    :node-and-date: adds the node on dev versions and the date on dirty
-                    workdir (default)
-    :node-and-timestamp: like ``node-and-date`` but with a timestamp of
-                         the form ``{:%Y%m%d%H%M%S}`` instead
-    :dirty-tag: adds ``+dirty`` if the current workdir has changes
-    :no-local-version: omits local version, useful e.g. because pypi does
-                       not support it
-
-
-Importing in ``setup.py``
-~~~~~~~~~~~~~~~~~~~~~~~~~
-
-To support usage in ``setup.py`` passing a callable into ``use_scm_version``
-is supported.
-
-Within that callable, ``setuptools_scm`` is available for import.
-The callable must return the configuration.
-
-.. code:: python
-
-    # content of setup.py
-    import setuptools
-
-    def myversion():
-        from setuptools_scm.version import get_local_dirty_tag
-        def clean_scheme(version):
-            return get_local_dirty_tag(version) if version.dirty else '+clean'
-
-        return {'local_scheme': clean_scheme}
-
-    setup(
-        ...,
-        use_scm_version=myversion,
-        ...
-    )
-
-
-Note on testing non-installed versions
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-While the general advice is to test against a installed version,
-some environments require a test prior to install,
-
-.. code::
-
-  $ python setup.py egg_info
-  $ PYTHONPATH=$PWD:$PWD/src pytest
-
-
-Interaction with Enterprise Distributions
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Some enterprise distributions like RHEL7 and others
-ship rather old setuptools versions due to various release management details.
-
-In those case its typically possible to build by using a sdist against ``setuptools_scm<2.0``.
-As those old setuptools versions lack sensible types for versions,
-modern setuptools_scm is unable to support them sensibly.
-
-In case the project you need to build can not be patched to either use old setuptools_scm,
-its still possible to install a more recent version of setuptools in order to handle the build
-and/or install the package by using wheels or eggs.
-
-
-Code of Conduct
----------------
-
-Everyone interacting in the ``setuptools_scm`` project's codebases, issue
-trackers, chat rooms, and mailing lists is expected to follow the
-`PSF Code of Conduct`_.
-
-.. _PSF Code of Conduct: https://github.com/pypa/.github/blob/main/CODE_OF_CONDUCT.md
-
-
-Security Contact
-================
-
-To report a security vulnerability, please use the
-`Tidelift security contact <https://tidelift.com/security>`_.
-Tidelift will coordinate the fix and disclosure.
+Metadata-Version: 2.1
+Name: setuptools-scm
+Version: 7.1.0
+Summary: the blessed package to manage your versions by scm tags
+Home-page: https://github.com/pypa/setuptools_scm/
+Author: Ronny Pfannschmidt
+Author-email: opensource@ronnypfannschmidt.de
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Version Control
+Classifier: Topic :: System :: Software Distribution
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: packaging (>=20.0)
+Requires-Dist: setuptools
+Requires-Dist: typing-extensions
+Requires-Dist: tomli (>=1.0.0) ; python_version < "3.11"
+Requires-Dist: importlib-metadata ; python_version < "3.8"
+Provides-Extra: test
+Requires-Dist: pytest (>=6.2) ; extra == 'test'
+Requires-Dist: virtualenv (>20) ; extra == 'test'
+Provides-Extra: toml
+Requires-Dist: setuptools (>=42) ; extra == 'toml'
+
+setuptools_scm
+==============
+
+``setuptools_scm`` extracts Python package versions from ``git`` or
+``hg`` metadata instead of declaring them as the version argument
+or in a SCM managed file.
+
+Additionally ``setuptools_scm`` provides setuptools with a list of
+files that are managed by the SCM (i.e. it automatically adds all of
+the SCM-managed files to the sdist). Unwanted files must be excluded
+by discarding them via ``MANIFEST.in``.
+
+``setuptools_scm`` supports the following scm out of the box:
+
+* git
+* mercurial
+
+.. image:: https://github.com/pypa/setuptools_scm/workflows/python%20tests+artifacts+release/badge.svg
+    :target: https://github.com/pypa/setuptools_scm/actions
+
+.. image:: https://tidelift.com/badges/package/pypi/setuptools-scm
+   :target: https://tidelift.com/subscription/pkg/pypi-setuptools-scm?utm_source=pypi-setuptools-scm&utm_medium=readme
+
+
+``pyproject.toml`` usage
+------------------------
+
+The preferred way to configure ``setuptools_scm`` is to author
+settings in a ``tool.setuptools_scm`` section of ``pyproject.toml``.
+
+This feature requires Setuptools 42 or later, released in Nov, 2019.
+If your project needs to support build from sdist on older versions
+of Setuptools, you will need to also implement the ``setup.py usage``
+for those legacy environments.
+
+First, ensure that ``setuptools_scm`` is present during the project's
+built step by specifying it as one of the build requirements.
+
+.. code:: toml
+
+    # pyproject.toml
+    [build-system]
+    requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
+
+That will be sufficient to require ``setuptools_scm`` for projects
+that support PEP 518 (`pip <https://pypi.org/project/pip>`_ and
+`pep517 <https://pypi.org/project/pep517/>`_). Many tools,
+especially those that invoke ``setup.py`` for any reason, may
+continue to rely on ``setup_requires``. For maximum compatibility
+with those uses, consider also including a ``setup_requires`` directive
+(described below in ``setup.py usage`` and ``setup.cfg``).
+
+To enable version inference, you need to set the version
+dynamically in the ``project`` section of ``pyproject.toml``:
+
+.. code:: toml
+
+    # pyproject.toml
+    [project]
+    # version = "0.0.1"  # Remove any existing version parameter.
+    dynamic = ["version"]
+
+Then add this section to your ``pyproject.toml``:
+
+.. code:: toml
+
+    # pyproject.toml
+    [tool.setuptools_scm]
+
+Including this section is comparable to supplying
+``use_scm_version=True`` in ``setup.py``. Additionally,
+include arbitrary keyword arguments in that section
+to be supplied to ``get_version()``. For example:
+
+.. code:: toml
+
+    # pyproject.toml
+    [tool.setuptools_scm]
+    write_to = "pkg/_version.py"
+
+Where ``pkg`` is the name of your package.
+
+If you need to confirm which version string is being generated
+or debug the configuration, you can install
+`setuptools-scm <https://github.com/pypa/setuptools_scm>`_
+directly in your working environment and run:
+
+.. code-block:: shell
+
+    $ python -m setuptools_scm
+
+    # To explore other options, try:
+    $ python -m setuptools_scm --help
+
+
+``setup.py`` usage (deprecated)
+-------------------------------
+
+.. warning::
+
+   ``setup_requires`` has been deprecated in favor of ``pyproject.toml``
+
+The following settings are considered legacy behavior and
+superseded by the ``pyproject.toml`` usage, but for maximal
+compatibility, projects may also supply the configuration in
+this older form.
+
+To use ``setuptools_scm`` just modify your project's ``setup.py`` file
+like this:
+
+* Add ``setuptools_scm`` to the ``setup_requires`` parameter.
+* Add the ``use_scm_version`` parameter and set it to ``True``.
+
+For example:
+
+.. code:: python
+
+    from setuptools import setup
+    setup(
+        ...,
+        use_scm_version=True,
+        setup_requires=['setuptools_scm'],
+        ...,
+    )
+
+Arguments to ``get_version()`` (see below) may be passed as a dictionary to
+``use_scm_version``. For example:
+
+.. code:: python
+
+    from setuptools import setup
+    setup(
+        ...,
+        use_scm_version = {
+            "root": "..",
+            "relative_to": __file__,
+            "local_scheme": "node-and-timestamp"
+        },
+        setup_requires=['setuptools_scm'],
+        ...,
+    )
+
+You can confirm the version number locally via ``setup.py``:
+
+.. code-block:: shell
+
+    $ python setup.py --version
+
+.. note::
+
+   If you see unusual version numbers for packages but ``python setup.py
+   --version`` reports the expected version number, ensure ``[egg_info]`` is
+   not defined in ``setup.cfg``.
+
+
+``setup.cfg`` usage (deprecated)
+------------------------------------
+
+as ``setup_requires`` is deprecated in favour of ``pyproject.toml``
+usage in ``setup.cfg`` is considered deprecated,
+please use ``pyproject.toml`` whenever possible.
+
+
+Programmatic usage
+------------------
+
+In order to use ``setuptools_scm`` from code that is one directory deeper
+than the project's root, you can use:
+
+.. code:: python
+
+    from setuptools_scm import get_version
+    version = get_version(root='..', relative_to=__file__)
+
+See `setup.py Usage (deprecated)`_ above for how to use this within ``setup.py``.
+
+
+Retrieving package version at runtime
+-------------------------------------
+
+If you have opted not to hardcode the version number inside the package,
+you can retrieve it at runtime from PEP-0566_ metadata using
+``importlib.metadata`` from the standard library (added in Python 3.8)
+or the `importlib_metadata`_ backport:
+
+.. code:: python
+
+    from importlib.metadata import version, PackageNotFoundError
+
+    try:
+        __version__ = version("package-name")
+    except PackageNotFoundError:
+        # package is not installed
+        pass
+
+Alternatively, you can use ``pkg_resources`` which is included in
+``setuptools`` (but has a significant runtime cost):
+
+.. code:: python
+
+   from pkg_resources import get_distribution, DistributionNotFound
+
+   try:
+       __version__ = get_distribution("package-name").version
+   except DistributionNotFound:
+        # package is not installed
+       pass
+
+However, this does place a runtime dependency on ``setuptools`` and can add up to
+a few 100ms overhead for the package import time.
+
+.. _PEP-0566: https://www.python.org/dev/peps/pep-0566/
+.. _importlib_metadata: https://pypi.org/project/importlib-metadata/
+
+
+Usage from Sphinx
+-----------------
+
+It is discouraged to use ``setuptools_scm`` from Sphinx itself,
+instead use ``importlib.metadata`` after editable/real installation:
+
+.. code:: python
+
+    # contents of docs/conf.py
+    from importlib.metadata import version
+    release = version('myproject')
+    # for example take major/minor
+    version = '.'.join(release.split('.')[:2])
+
+The underlying reason is, that services like *Read the Docs* sometimes change
+the working directory for good reasons and using the installed metadata
+prevents using needless volatile data there.
+
+
+Usage from Docker
+-----------------
+
+By default, docker will not copy the ``.git``  folder into your container.
+Therefore, builds with version inference might fail.
+Consequently, you can use the following snipped to infer the version from
+the host os without copying the entire ``.git`` folder to your Dockerfile.
+
+.. code:: dockerfile
+
+    RUN --mount=source=.git,target=.git,type=bind \
+        pip install --no-cache-dir -e .
+
+However, this build step introduces a dependency to the state of your local
+.git folder the build cache and triggers the long-running pip install process on every build.
+To optimize build caching, one can use an environment variable to pretend a pseudo
+version that is used to cache the results of the pip install process:
+
+.. code:: dockerfile
+
+    FROM python
+    COPY pyproject.toml
+    ARG PSEUDO_VERSION=1
+    RUN SETUPTOOLS_SCM_PRETEND_VERSION=${PSEUDO_VERSION} pip install -e .[test]
+    RUN --mount=source=.git,target=.git,type=bind pip install -e .
+
+Note that running this Dockerfile requires docker with BuildKit enabled
+`[docs] <https://github.com/moby/buildkit/blob/v0.8.3/frontend/dockerfile/docs/syntax.md>`_.
+
+To avoid BuildKit and mounting of the .git folder altogether, one can also pass the desired
+version as a build argument. Note that ``SETUPTOOLS_SCM_PRETEND_VERSION_FOR_${UPPERCASED_DIST_NAME}``
+is preferred over ``SETUPTOOLS_SCM_PRETEND_VERSION``.
+
+
+Default versioning scheme
+-------------------------
+
+In the standard configuration ``setuptools_scm`` takes a look at three things:
+
+1. latest tag (with a version number)
+2. the distance to this tag (e.g. number of revisions since latest tag)
+3. workdir state (e.g. uncommitted changes since latest tag)
+
+and uses roughly the following logic to render the version:
+
+no distance and clean:
+    ``{tag}``
+distance and clean:
+    ``{next_version}.dev{distance}+{scm letter}{revision hash}``
+no distance and not clean:
+    ``{tag}+dYYYYMMDD``
+distance and not clean:
+    ``{next_version}.dev{distance}+{scm letter}{revision hash}.dYYYYMMDD``
+
+The next version is calculated by adding ``1`` to the last numeric component of
+the tag.
+
+For Git projects, the version relies on `git describe <https://git-scm.com/docs/git-describe>`_,
+so you will see an additional ``g`` prepended to the ``{revision hash}``.
+
+
+Semantic Versioning (SemVer)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Due to the default behavior it's necessary to always include a
+patch version (the ``3`` in ``1.2.3``), or else the automatic guessing
+will increment the wrong part of the SemVer (e.g. tag ``2.0`` results in
+``2.1.devX`` instead of ``2.0.1.devX``). So please make sure to tag
+accordingly.
+
+.. note::
+
+    Future versions of ``setuptools_scm`` will switch to `SemVer
+    <http://semver.org/>`_ by default hiding the the old behavior as an
+    configurable option.
+
+
+Builtin mechanisms for obtaining version numbers
+------------------------------------------------
+
+1. the SCM itself (git/hg)
+2. ``.hg_archival`` files (mercurial archives)
+3. ``.git_archival.txt`` files (git archives, see subsection below)
+4. ``PKG-INFO``
+
+
+Git archives
+~~~~~~~~~~~~
+
+Git archives are supported, but a few changes to your repository are required.
+
+Create a ``.git_archival.txt`` file in the root directory of your repository,
+and copy-paste this into it::
+
+    node: $Format:%H$
+    node-date: $Format:%cI$
+    describe-name: $Format:%(describe:tags=true,match=*[0-9]*)$
+    ref-names: $Format:%D$
+
+Create the ``.gitattributes`` file in the root directory of your repository
+if it doesn't already exist, and copy-paste this into it::
+
+    .git_archival.txt  export-subst
+
+Finally, don't forget to commit those two files::
+
+    git add .git_archival.txt .gitattributes && git commit
+
+Note that if you are creating a ``_version.py`` file, note that it should not
+be kept in version control.
+
+
+File finders hook makes most of MANIFEST.in unnecessary
+-------------------------------------------------------
+
+``setuptools_scm`` implements a `file_finders
+<https://setuptools.pypa.io/en/latest/userguide/extension.html#adding-support-for-revision-control-systems>`_
+entry point which returns all files tracked by your SCM. This eliminates
+the need for a manually constructed ``MANIFEST.in`` in most cases where this
+would be required when not using ``setuptools_scm``, namely:
+
+* To ensure all relevant files are packaged when running the ``sdist`` command.
+
+* When using `include_package_data <https://setuptools.readthedocs.io/en/latest/setuptools.html#including-data-files>`_
+  to include package data as part of the ``build`` or ``bdist_wheel``.
+
+``MANIFEST.in`` may still be used: anything defined there overrides the hook.
+This is mostly useful to exclude files tracked in your SCM from packages,
+although in principle it can be used to explicitly include non-tracked files
+too.
+
+
+Configuration parameters
+------------------------
+
+In order to configure the way ``use_scm_version`` works you can provide
+a mapping with options instead of a boolean value.
+
+The currently supported configuration keys are:
+
+:root:
+    Relative path to cwd, used for finding the SCM root; defaults to ``.``
+
+:version_scheme:
+    Configures how the local version number is constructed; either an
+    entrypoint name or a callable.
+
+:local_scheme:
+    Configures how the local component of the version is constructed; either an
+    entrypoint name or a callable.
+
+:write_to:
+    A path to a file that gets replaced with a file containing the current
+    version. It is ideal for creating a ``_version.py`` file within the
+    package, typically used to avoid using `pkg_resources.get_distribution`
+    (which adds some overhead).
+
+    .. warning::
+
+      Only files with :code:`.py` and :code:`.txt` extensions have builtin
+      templates, for other file types it is necessary to provide
+      :code:`write_to_template`.
+
+:write_to_template:
+    A newstyle format string that is given the current version as
+    the ``version`` keyword argument for formatting.
+
+:relative_to:
+    A file from which the root can be resolved.
+    Typically called by a script or module that is not in the root of the
+    repository to point ``setuptools_scm`` at the root of the repository by
+    supplying ``__file__``.
+
+:tag_regex:
+   A Python regex string to extract the version part from any SCM tag.
+    The regex needs to contain either a single match group, or a group
+    named ``version``, that captures the actual version information.
+
+    Defaults to the value of ``setuptools_scm.config.DEFAULT_TAG_REGEX``
+    (see `config.py <src/setuptools_scm/config.py>`_).
+
+:parentdir_prefix_version:
+    If the normal methods for detecting the version (SCM version,
+    sdist metadata) fail, and the parent directory name starts with
+    ``parentdir_prefix_version``, then this prefix is stripped and the rest of
+    the parent directory name is matched with ``tag_regex`` to get a version
+    string.  If this parameter is unset (the default), then this fallback is
+    not used.
+
+    This is intended to cover GitHub's "release tarballs", which extract into
+    directories named ``projectname-tag/`` (in which case
+    ``parentdir_prefix_version`` can be set e.g. to ``projectname-``).
+
+:fallback_version:
+    A version string that will be used if no other method for detecting the
+    version worked (e.g., when using a tarball with no metadata). If this is
+    unset (the default), setuptools_scm will error if it fails to detect the
+    version.
+
+:parse:
+    A function that will be used instead of the discovered SCM for parsing the
+    version.
+    Use with caution, this is a function for advanced use, and you should be
+    familiar with the ``setuptools_scm`` internals to use it.
+
+:git_describe_command:
+    This command will be used instead the default ``git describe`` command.
+    Use with caution, this is a function for advanced use, and you should be
+    familiar with the ``setuptools_scm`` internals to use it.
+
+    Defaults to the value set by ``setuptools_scm.git.DEFAULT_DESCRIBE``
+    (see `git.py <src/setuptools_scm/git.py>`_).
+
+:normalize:
+    A boolean flag indicating if the version string should be normalized.
+    Defaults to ``True``. Setting this to ``False`` is equivalent to setting
+    ``version_cls`` to ``setuptools_scm.version.NonNormalizedVersion``
+
+:version_cls:
+    An optional class used to parse, verify and possibly normalize the version
+    string. Its constructor should receive a single string argument, and its
+    ``str`` should return the normalized version string to use.
+    This option can also receive a class qualified name as a string.
+
+    This defaults to ``packaging.version.Version`` if available. If
+    ``packaging`` is not installed, ``pkg_resources.packaging.version.Version``
+    is used. Note that it is known to modify git release candidate schemes.
+
+    The ``setuptools_scm.NonNormalizedVersion`` convenience class is
+    provided to disable the normalization step done by
+    ``packaging.version.Version``. If this is used while ``setuptools_scm``
+    is integrated in a setuptools packaging process, the non-normalized
+    version number will appear in all files (see ``write_to``) BUT note
+    that setuptools will still normalize it to create the final distribution,
+    so as to stay compliant with the python packaging standards.
+
+To use ``setuptools_scm`` in other Python code you can use the ``get_version``
+function:
+
+.. code:: python
+
+    from setuptools_scm import get_version
+    my_version = get_version()
+
+It optionally accepts the keys of the ``use_scm_version`` parameter as
+keyword arguments.
+
+Example configuration in ``setup.py`` format:
+
+.. code:: python
+
+    from setuptools import setup
+
+    setup(
+        use_scm_version={
+            'write_to': '_version.py',
+            'write_to_template': '__version__ = "{version}"',
+            'tag_regex': r'^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$',
+        }
+    )
+
+
+Environment variables
+---------------------
+
+:SETUPTOOLS_SCM_PRETEND_VERSION:
+    when defined and not empty,
+    its used as the primary source for the version number
+    in which case it will be a unparsed string
+
+:SETUPTOOLS_SCM_PRETEND_VERSION_FOR_${UPPERCASED_DIST_NAME}:
+    when defined and not empty,
+    its used as the primary source for the version number
+    in which case it will be a unparsed string
+
+    it takes precedence over ``SETUPTOOLS_SCM_PRETEND_VERSION``
+
+:SETUPTOOLS_SCM_DEBUG:
+    when defined and not empty,
+    a lot of debug information will be printed as part of ``setuptools_scm``
+    operating
+
+:SOURCE_DATE_EPOCH:
+    when defined, used as the timestamp from which the
+    ``node-and-date`` and ``node-and-timestamp`` local parts are
+    derived, otherwise the current time is used
+    (https://reproducible-builds.org/docs/source-date-epoch/)
+
+:SETUPTOOLS_SCM_IGNORE_VCS_ROOTS:
+    when defined, a ``os.pathsep`` separated list
+    of directory names to ignore for root finding
+
+
+Extending setuptools_scm
+------------------------
+
+``setuptools_scm`` ships with a few ``setuptools`` entrypoints based hooks to
+extend its default capabilities.
+
+
+Adding a new SCM
+~~~~~~~~~~~~~~~~
+
+``setuptools_scm`` provides two entrypoints for adding new SCMs:
+
+``setuptools_scm.parse_scm``
+    A function used to parse the metadata of the current workdir
+    using the name of the control directory/file of your SCM as the
+    entrypoint's name. E.g. for the built-in entrypoint for git the
+    entrypoint is named ``.git`` and references ``setuptools_scm.git:parse``
+
+  The return value MUST be a ``setuptools_scm.version.ScmVersion`` instance
+  created by the function ``setuptools_scm.version:meta``.
+
+``setuptools_scm.files_command``
+  Either a string containing a shell command that prints all SCM managed
+  files in its current working directory or a callable, that given a
+  pathname will return that list.
+
+  Also use then name of your SCM control directory as name of the entrypoint.
+
+
+Version number construction
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+``setuptools_scm.version_scheme``
+    Configures how the version number is constructed given a
+    ``setuptools_scm.version.ScmVersion`` instance and should return a string
+    representing the version.
+
+    Available implementations:
+
+    :guess-next-dev: Automatically guesses the next development version (default).
+        Guesses the upcoming release by incrementing the pre-release segment if present,
+        otherwise by incrementing the micro segment. Then appends :code:`.devN`.
+        In case the tag ends with ``.dev0`` the version is not bumped
+        and custom ``.devN`` versions will trigger a error.
+    :post-release: generates post release versions (adds :code:`.postN`)
+    :python-simplified-semver: Basic semantic versioning. Guesses the upcoming release
+        by incrementing the minor segment and setting the micro segment to zero if the
+        current branch contains the string ``'feature'``, otherwise by incrementing the
+        micro version. Then appends :code:`.devN`. Not compatible with pre-releases.
+    :release-branch-semver: Semantic versioning for projects with release branches. The
+        same as ``guess-next-dev`` (incrementing the pre-release or micro segment) if on
+        a release branch: a branch whose name (ignoring namespace) parses as a version
+        that matches the most recent tag up to the minor segment. Otherwise if on a
+        non-release branch, increments the minor segment and sets the micro segment to
+        zero, then appends :code:`.devN`.
+    :no-guess-dev: Does no next version guessing, just adds :code:`.post1.devN`
+
+``setuptools_scm.local_scheme``
+    Configures how the local part of a version is rendered given a
+    ``setuptools_scm.version.ScmVersion`` instance and should return a string
+    representing the local version.
+    Dates and times are in Coordinated Universal Time (UTC), because as part
+    of the version, they should be location independent.
+
+    Available implementations:
+
+    :node-and-date: adds the node on dev versions and the date on dirty
+                    workdir (default)
+    :node-and-timestamp: like ``node-and-date`` but with a timestamp of
+                         the form ``{:%Y%m%d%H%M%S}`` instead
+    :dirty-tag: adds ``+dirty`` if the current workdir has changes
+    :no-local-version: omits local version, useful e.g. because pypi does
+                       not support it
+
+
+Importing in ``setup.py``
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To support usage in ``setup.py`` passing a callable into ``use_scm_version``
+is supported.
+
+Within that callable, ``setuptools_scm`` is available for import.
+The callable must return the configuration.
+
+.. code:: python
+
+    # content of setup.py
+    import setuptools
+
+    def myversion():
+        from setuptools_scm.version import get_local_dirty_tag
+        def clean_scheme(version):
+            return get_local_dirty_tag(version) if version.dirty else '+clean'
+
+        return {'local_scheme': clean_scheme}
+
+    setup(
+        ...,
+        use_scm_version=myversion,
+        ...
+    )
+
+
+Note on testing non-installed versions
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+While the general advice is to test against a installed version,
+some environments require a test prior to install,
+
+.. code::
+
+  $ python setup.py egg_info
+  $ PYTHONPATH=$PWD:$PWD/src pytest
+
+
+Interaction with Enterprise Distributions
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Some enterprise distributions like RHEL7 and others
+ship rather old setuptools versions due to various release management details.
+
+In those case its typically possible to build by using a sdist against ``setuptools_scm<2.0``.
+As those old setuptools versions lack sensible types for versions,
+modern setuptools_scm is unable to support them sensibly.
+
+In case the project you need to build can not be patched to either use old setuptools_scm,
+its still possible to install a more recent version of setuptools in order to handle the build
+and/or install the package by using wheels or eggs.
+
+
+Code of Conduct
+---------------
+
+Everyone interacting in the ``setuptools_scm`` project's codebases, issue
+trackers, chat rooms, and mailing lists is expected to follow the
+`PSF Code of Conduct`_.
+
+.. _PSF Code of Conduct: https://github.com/pypa/.github/blob/main/CODE_OF_CONDUCT.md
+
+
+Security Contact
+================
+
+To report a security vulnerability, please use the
+`Tidelift security contact <https://tidelift.com/security>`_.
+Tidelift will coordinate the fix and disclosure.
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/RECORD`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-setuptools_scm/__init__.py,sha256=uiEukCjK_iXePWmkIMzSvLL1ScZCzdFITfD5wvaAdAM,5891
-setuptools_scm/__main__.py,sha256=PUkvI9W-hylvxv5sd1sosqWXEliN3d30x7BIKVEAQaQ,98
-setuptools_scm/_cli.py,sha256=axI6F_QF66Vg0Pfp_7nvktH2gdeTiG_xG4D7XXXUk38,2845
-setuptools_scm/_entrypoints.py,sha256=lLf40uD0nWi4njK3Hs3JYWZbhw9wzGIJzlPpbc3wTiE,2696
-setuptools_scm/_overrides.py,sha256=y75kOjwBGdOqojz0we5NAf_-iMMJB-Tt6pPktwU1pd8,1067
-setuptools_scm/_types.py,sha256=sho6RgWu2eU1uURtJymR_9PZi_wvGaD95Y4SN_1lnOo,845
-setuptools_scm/_version_cls.py,sha256=bmNimKGN_rPTO_HoLbr2KOZh-Zpqa0YD_Cr9KyD7-QU,1575
-setuptools_scm/config.py,sha256=eRxBrtDbfhhiBA7bET5VZDf0qPDGVgrAAEURFtWDCEo,7237
-setuptools_scm/discover.py,sha256=Wl0m0oD54gc_0ObnEPKSuNsV85KF9ZlNKu-LMsrIT8M,1867
-setuptools_scm/file_finder.py,sha256=0ExSEMFWJ9W9IApc97mj3msCWvuRcKP0rhX0UJfFUic,3100
-setuptools_scm/file_finder_git.py,sha256=t-W-69MmLl2dwCLyOekZyCsAr46L6m9BgPqU6FRpgtY,4287
-setuptools_scm/file_finder_hg.py,sha256=B52r5e_VhovbUS5VExzQz-hiKFgPe-wAKTBf0-m0WUQ,2293
-setuptools_scm/git.py,sha256=_mBrHxJUpfwAg6u94RSF8Q-R2D3EjB4rXpOearljd7w,9599
-setuptools_scm/hacks.py,sha256=wM5s2YBuTj1UmREt0yBa9Pxni66d91qugBMid4kTpDM,1776
-setuptools_scm/hg.py,sha256=2L6CAofHm-cNFFlb5V9VFhKmfVvRwAZnof-f-GLayWk,6128
-setuptools_scm/hg_git.py,sha256=s_mbg6v-jgA9KfkoZjqUiDayAPeQzk8TVoQT9jZ7D6Q,4166
-setuptools_scm/integration.py,sha256=-aYNnFC2zk6i3FZfKgEQs8mcKfbQXvZtPtKc_14nKqs,3620
-setuptools_scm/scm_workdir.py,sha256=Njay5Ob7d1lvAV3MjJN4vfz7VQaT0kEUPj7-nlf4QRY,585
-setuptools_scm/utils.py,sha256=2fvBSG1IZThe12cJsJFOsDTIJGxoy3-8vYJt67GziIw,5117
-setuptools_scm/version.py,sha256=xuvazAc3YpOkjnWyENhecN8hs6y-sNVoI-35KARsWog,17034
-setuptools_scm/_integration/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-setuptools_scm/_integration/pyproject_reading.py,sha256=_Qb2JzWLM7Wz01Ti6c7uHsRbsoR1PP8GLTR6v7ATdMw,2838
-setuptools_scm/_integration/setuptools.py,sha256=wTI3QF2HPcxtKRp6pjDwavd2mb2K2qtYX9GzpxQh2cc,530
-setuptools_scm-7.1.0.dist-info/LICENSE,sha256=iYB6zyMJvShfAzQE7nhYFgLzzZuBmhasLw5fYP9KRz4,1023
-setuptools_scm-7.1.0.dist-info/METADATA,sha256=s_LpfHpFmr--B93gVH4k5arDPUr8_Qhs2ln9-FXEjY0,24836
-setuptools_scm-7.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-setuptools_scm-7.1.0.dist-info/entry_points.txt,sha256=30rP8QH6CS8nDIZH6prkd4AsSh7EFL-PI0HOb6q76aQ,1734
-setuptools_scm-7.1.0.dist-info/top_level.txt,sha256=kiu-91q3_rJLUoc2wl8_lC4cIlpgtgdD_4NaChF4hOA,15
-setuptools_scm-7.1.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-setuptools_scm-7.1.0.dist-info/RECORD,,
+setuptools_scm/__init__.py,sha256=uiEukCjK_iXePWmkIMzSvLL1ScZCzdFITfD5wvaAdAM,5891
+setuptools_scm/__main__.py,sha256=PUkvI9W-hylvxv5sd1sosqWXEliN3d30x7BIKVEAQaQ,98
+setuptools_scm/_cli.py,sha256=axI6F_QF66Vg0Pfp_7nvktH2gdeTiG_xG4D7XXXUk38,2845
+setuptools_scm/_entrypoints.py,sha256=lLf40uD0nWi4njK3Hs3JYWZbhw9wzGIJzlPpbc3wTiE,2696
+setuptools_scm/_overrides.py,sha256=y75kOjwBGdOqojz0we5NAf_-iMMJB-Tt6pPktwU1pd8,1067
+setuptools_scm/_types.py,sha256=sho6RgWu2eU1uURtJymR_9PZi_wvGaD95Y4SN_1lnOo,845
+setuptools_scm/_version_cls.py,sha256=bmNimKGN_rPTO_HoLbr2KOZh-Zpqa0YD_Cr9KyD7-QU,1575
+setuptools_scm/config.py,sha256=eRxBrtDbfhhiBA7bET5VZDf0qPDGVgrAAEURFtWDCEo,7237
+setuptools_scm/discover.py,sha256=Wl0m0oD54gc_0ObnEPKSuNsV85KF9ZlNKu-LMsrIT8M,1867
+setuptools_scm/file_finder.py,sha256=0ExSEMFWJ9W9IApc97mj3msCWvuRcKP0rhX0UJfFUic,3100
+setuptools_scm/file_finder_git.py,sha256=t-W-69MmLl2dwCLyOekZyCsAr46L6m9BgPqU6FRpgtY,4287
+setuptools_scm/file_finder_hg.py,sha256=B52r5e_VhovbUS5VExzQz-hiKFgPe-wAKTBf0-m0WUQ,2293
+setuptools_scm/git.py,sha256=_mBrHxJUpfwAg6u94RSF8Q-R2D3EjB4rXpOearljd7w,9599
+setuptools_scm/hacks.py,sha256=wM5s2YBuTj1UmREt0yBa9Pxni66d91qugBMid4kTpDM,1776
+setuptools_scm/hg.py,sha256=2L6CAofHm-cNFFlb5V9VFhKmfVvRwAZnof-f-GLayWk,6128
+setuptools_scm/hg_git.py,sha256=s_mbg6v-jgA9KfkoZjqUiDayAPeQzk8TVoQT9jZ7D6Q,4166
+setuptools_scm/integration.py,sha256=-aYNnFC2zk6i3FZfKgEQs8mcKfbQXvZtPtKc_14nKqs,3620
+setuptools_scm/scm_workdir.py,sha256=Njay5Ob7d1lvAV3MjJN4vfz7VQaT0kEUPj7-nlf4QRY,585
+setuptools_scm/utils.py,sha256=2fvBSG1IZThe12cJsJFOsDTIJGxoy3-8vYJt67GziIw,5117
+setuptools_scm/version.py,sha256=xuvazAc3YpOkjnWyENhecN8hs6y-sNVoI-35KARsWog,17034
+setuptools_scm/_integration/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+setuptools_scm/_integration/pyproject_reading.py,sha256=_Qb2JzWLM7Wz01Ti6c7uHsRbsoR1PP8GLTR6v7ATdMw,2838
+setuptools_scm/_integration/setuptools.py,sha256=wTI3QF2HPcxtKRp6pjDwavd2mb2K2qtYX9GzpxQh2cc,530
+setuptools_scm-7.1.0.dist-info/LICENSE,sha256=iYB6zyMJvShfAzQE7nhYFgLzzZuBmhasLw5fYP9KRz4,1023
+setuptools_scm-7.1.0.dist-info/METADATA,sha256=s_LpfHpFmr--B93gVH4k5arDPUr8_Qhs2ln9-FXEjY0,24836
+setuptools_scm-7.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+setuptools_scm-7.1.0.dist-info/entry_points.txt,sha256=30rP8QH6CS8nDIZH6prkd4AsSh7EFL-PI0HOb6q76aQ,1734
+setuptools_scm-7.1.0.dist-info/top_level.txt,sha256=kiu-91q3_rJLUoc2wl8_lC4cIlpgtgdD_4NaChF4hOA,15
+setuptools_scm-7.1.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+setuptools_scm-7.1.0.dist-info/RECORD,,
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/EGG-INFO/entry_points.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-[distutils.setup_keywords]
-use_scm_version = setuptools_scm.integration:version_keyword
-
-[setuptools.file_finders]
-setuptools_scm = setuptools_scm.integration:find_files
-
-[setuptools.finalize_distribution_options]
-setuptools_scm = setuptools_scm.integration:infer_version
-
-[setuptools_scm.files_command]
-.git = setuptools_scm.file_finder_git:git_find_files
-.hg = setuptools_scm.file_finder_hg:hg_find_files
-
-[setuptools_scm.files_command_fallback]
-.git_archival.txt = setuptools_scm.file_finder_git:git_archive_find_files
-.hg_archival.txt = setuptools_scm.file_finder_hg:hg_archive_find_files
-
-[setuptools_scm.local_scheme]
-dirty-tag = setuptools_scm.version:get_local_dirty_tag
-no-local-version = setuptools_scm.version:get_no_local_node
-node-and-date = setuptools_scm.version:get_local_node_and_date
-node-and-timestamp = setuptools_scm.version:get_local_node_and_timestamp
-
-[setuptools_scm.parse_scm]
-.git = setuptools_scm.git:parse
-.hg = setuptools_scm.hg:parse
-
-[setuptools_scm.parse_scm_fallback]
-.git_archival.txt = setuptools_scm.git:parse_archival
-.hg_archival.txt = setuptools_scm.hg:parse_archival
-PKG-INFO = setuptools_scm.hacks:parse_pkginfo
-pip-egg-info = setuptools_scm.hacks:parse_pip_egg_info
-pyproject.toml = setuptools_scm.hacks:fallback_version
-setup.py = setuptools_scm.hacks:fallback_version
-
-[setuptools_scm.version_scheme]
-calver-by-date = setuptools_scm.version:calver_by_date
-guess-next-dev = setuptools_scm.version:guess_next_dev_version
-no-guess-dev = setuptools_scm.version:no_guess_dev_version
-post-release = setuptools_scm.version:postrelease_version
-python-simplified-semver = setuptools_scm.version:simplified_semver_version
-release-branch-semver = setuptools_scm.version:release_branch_semver_version
+[distutils.setup_keywords]
+use_scm_version = setuptools_scm.integration:version_keyword
+
+[setuptools.file_finders]
+setuptools_scm = setuptools_scm.integration:find_files
+
+[setuptools.finalize_distribution_options]
+setuptools_scm = setuptools_scm.integration:infer_version
+
+[setuptools_scm.files_command]
+.git = setuptools_scm.file_finder_git:git_find_files
+.hg = setuptools_scm.file_finder_hg:hg_find_files
+
+[setuptools_scm.files_command_fallback]
+.git_archival.txt = setuptools_scm.file_finder_git:git_archive_find_files
+.hg_archival.txt = setuptools_scm.file_finder_hg:hg_archive_find_files
+
+[setuptools_scm.local_scheme]
+dirty-tag = setuptools_scm.version:get_local_dirty_tag
+no-local-version = setuptools_scm.version:get_no_local_node
+node-and-date = setuptools_scm.version:get_local_node_and_date
+node-and-timestamp = setuptools_scm.version:get_local_node_and_timestamp
+
+[setuptools_scm.parse_scm]
+.git = setuptools_scm.git:parse
+.hg = setuptools_scm.hg:parse
+
+[setuptools_scm.parse_scm_fallback]
+.git_archival.txt = setuptools_scm.git:parse_archival
+.hg_archival.txt = setuptools_scm.hg:parse_archival
+PKG-INFO = setuptools_scm.hacks:parse_pkginfo
+pip-egg-info = setuptools_scm.hacks:parse_pip_egg_info
+pyproject.toml = setuptools_scm.hacks:fallback_version
+setup.py = setuptools_scm.hacks:fallback_version
+
+[setuptools_scm.version_scheme]
+calver-by-date = setuptools_scm.version:calver_by_date
+guess-next-dev = setuptools_scm.version:guess_next_dev_version
+no-guess-dev = setuptools_scm.version:no_guess_dev_version
+post-release = setuptools_scm.version:postrelease_version
+python-simplified-semver = setuptools_scm.version:simplified_semver_version
+release-branch-semver = setuptools_scm.version:release_branch_semver_version
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/__init__.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 5891
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 6082
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 16
    flags     : 16777216
    code
       0x970064005a00640164026c016d025a020100640164036c035a03640164
@@ -213,33 +213,33 @@
     44         316 LOAD_CONST              29 ('{version}')
    
     37         318 LOAD_CONST              30 (('.py', '.txt'))
                320 BUILD_CONST_KEY_MAP      2
                322 STORE_NAME              38 (TEMPLATES)
    
     48         324 LOAD_CONST              72 (('root', '_t.PathT', 'return', 'ScmVersion | None'))
-               326 LOAD_CONST              35 (<code object version_from_scm, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\__init__.py", line 48>)
+               326 LOAD_CONST              35 (<code object version_from_scm, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\__init__.py", line 48>)
                328 MAKE_FUNCTION            4 (annotations)
                330 STORE_NAME              39 (version_from_scm)
    
     62         332 NOP
    
     58         334 LOAD_CONST              73 ((None,))
                336 LOAD_CONST              74 (('root', '_t.PathT', 'version', 'str', 'write_to', '_t.PathT', 'template', 'str | None', 'return', 'None'))
-               338 LOAD_CONST              42 (<code object dump_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\__init__.py", line 58>)
+               338 LOAD_CONST              42 (<code object dump_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\__init__.py", line 58>)
                340 MAKE_FUNCTION            5 (defaults, annotations)
                342 STORE_NAME              40 (dump_version)
    
     81         344 LOAD_CONST              75 (('config', 'Configuration', 'return', 'ScmVersion | None'))
-               346 LOAD_CONST              45 (<code object _do_parse, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\__init__.py", line 81>)
+               346 LOAD_CONST              45 (<code object _do_parse, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\__init__.py", line 81>)
                348 MAKE_FUNCTION            4 (annotations)
                350 STORE_NAME              41 (_do_parse)
    
    107         352 LOAD_CONST              76 (('config', 'Configuration', 'return', 'NoReturn'))
-               354 LOAD_CONST              47 (<code object _version_missing, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\__init__.py", line 107>)
+               354 LOAD_CONST              47 (<code object _version_missing, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\__init__.py", line 107>)
                356 MAKE_FUNCTION            4 (annotations)
                358 STORE_NAME              42 (_version_missing)
    
    121         360 LOAD_CONST              48 ('.')
    
    122         362 LOAD_NAME               24 (DEFAULT_VERSION_SCHEME)
    
@@ -269,20 +269,20 @@
    
    135         388 LOAD_CONST              49 (True)
    
    136         390 LOAD_CONST              50 (False)
    
    120         392 BUILD_TUPLE             16
                394 LOAD_CONST              77 (('root', 'str', 'version_scheme', 'Callable[[ScmVersion], str] | str', 'local_scheme', 'Callable[[ScmVersion], str] | str', 'write_to', '_t.PathT | None', 'write_to_template', 'str | None', 'relative_to', 'str | None', 'tag_regex', 'str', 'parentdir_prefix_version', 'str | None', 'fallback_version', 'str | None', 'fallback_root', '_t.PathT', 'parse', 'Any | None', 'git_describe_command', 'Any | None', 'dist_name', 'str | None', 'version_cls', 'Any | None', 'normalize', 'bool', 'search_parent_directories', 'bool', 'return', 'str'))
-               396 LOAD_CONST              69 (<code object get_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\__init__.py", line 120>)
+               396 LOAD_CONST              69 (<code object get_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\__init__.py", line 120>)
                398 MAKE_FUNCTION            5 (defaults, annotations)
                400 STORE_NAME              43 (get_version)
    
    152         402 LOAD_CONST              78 (('config', 'Configuration', 'return', 'str | None'))
-               404 LOAD_CONST              70 (<code object _get_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\__init__.py", line 152>)
+               404 LOAD_CONST              70 (<code object _get_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\__init__.py", line 152>)
                406 MAKE_FUNCTION            4 (annotations)
                408 STORE_NAME              44 (_get_version)
    
    173         410 BUILD_LIST               0
                412 LOAD_CONST              71 (('get_version', 'dump_version', 'version_from_scm', 'Configuration', 'DEFAULT_VERSION_SCHEME', 'DEFAULT_LOCAL_SCHEME', 'DEFAULT_TAG_REGEX', 'PRETEND_KEY', 'PRETEND_KEY_NAMED', 'Version', 'NonNormalizedVersion', 'function_has_arg', 'trace', 'format_version', 'meta', 'iter_matching_entrypoints'))
                414 LIST_EXTEND              1
                416 STORE_NAME              45 (__all__)
@@ -369,15 +369,15 @@
             2
             ('category', 'stacklevel')
             ('root',)
          names      ('warnings', 'warn', 'DeprecationWarning', 'Configuration', '_version_from_entrypoints')
          varnames   ('root', 'config')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
          name       'version_from_scm'
          firstlineno 48
          lnotab 0x0201160102010c0102fd12052001
       'version'
       'str'
       'write_to'
       'template'
@@ -538,15 +538,15 @@
             "bad file format: '{}' (of {}) \nonly *.txt and *.py are supported"
             'w'
             ('version', 'version_tuple')
          names      ('isinstance', 'str', 'os', 'path', 'normpath', 'join', 'splitext', 'TEMPLATES', 'get', 'ValueError', 'format', '_version_as_tuple', 'open', 'write')
          varnames   ('root', 'version', 'write_to', 'template', 'target', 'ext', 'version_tuple', 'fp')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
          name       'dump_version'
          firstlineno 58
          lnotab 0x02062e017a014a01380204010c0118014aff0eff10051e02220154ff
       'config'
       'Configuration'
       code
          argcount  : 1
@@ -661,15 +661,15 @@
             '\nplease return a parsed version'
             True
             ('fallback',)
          names      ('_read_pretended_version_for', 'parse', '_call_entrypoint_fn', 'absolute_root', 'isinstance', 'str', 'TypeError', 'ScmVersion', '_version_from_entrypoints')
          varnames   ('config', 'pretended', 'parse_result', 'version')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
          name       '_do_parse'
          firstlineno 81
          lnotab
             0x02011e01040104020e0136012a010c0114ff100404012e01060224032a
             0104ff1204
       'NoReturn'
       code
@@ -698,15 +698,15 @@
             None
             'setuptools-scm was unable to detect version for '
             ".\n\nMake sure you're either building from a fully intact git repository or PyPI tarballs. Most other sources (such as GitHub's tarballs, a git checkout without the .git folder) don't contain the necessary metadata and will not work.\n\nFor example, if you're using pip, instead of https://github.com/user/proj/archive/master.zip use git+https://github.com/user/proj.git#egg=proj"
          names      ('LookupError', 'absolute_root')
          varnames   ('config',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
          name       '_version_missing'
          firstlineno 107
          lnotab 0x02010c0114ff
       '.'
       True
       False
       'version_scheme'
@@ -770,15 +770,15 @@
             '\n    If supplied, relative_to should be a file from which root may\n    be resolved. Typically called by a script or module that is not\n    in the root of the repository to direct setuptools_scm to the\n    root of the repository by supplying ``__file__``.\n    '
             None
             ()
          names      ('Configuration', 'locals', '_get_version', '_version_missing')
          varnames   ('root', 'version_scheme', 'local_scheme', 'write_to', 'write_to_template', 'relative_to', 'tag_regex', 'parentdir_prefix_version', 'fallback_version', 'fallback_root', 'parse', 'git_describe_command', 'dist_name', 'version_cls', 'normalize', 'search_parent_directories', 'config', 'maybe_version')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
          name       'get_version'
          firstlineno 120
          lnotab 0x021930011e0104011e01
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
@@ -848,15 +848,15 @@
             None
             ('version_scheme', 'local_scheme')
             ('root', 'version', 'write_to', 'template')
          names      ('_do_parse', 'format_version', 'version_scheme', 'local_scheme', 'write_to', 'dump_version', 'root', 'write_to_template')
          varnames   ('config', 'parsed_version', 'version_string')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
          name       '_get_version'
          firstlineno 152
          lnotab
             0x02011e01040104010c0102010c010cfd12050e010c010c0102010c010c
             fc1207
       ('get_version', 'dump_version', 'version_from_scm', 'Configuration', 'DEFAULT_VERSION_SCHEME', 'DEFAULT_LOCAL_SCHEME', 'DEFAULT_TAG_REGEX', 'PRETEND_KEY', 'PRETEND_KEY_NAMED', 'Version', 'NonNormalizedVersion', 'function_has_arg', 'trace', 'format_version', 'meta', 'iter_matching_entrypoints')
       ('root', '_t.PathT', 'return', 'ScmVersion | None')
@@ -866,15 +866,15 @@
       ('config', 'Configuration', 'return', 'NoReturn')
       ('root', 'str', 'version_scheme', 'Callable[[ScmVersion], str] | str', 'local_scheme', 'Callable[[ScmVersion], str] | str', 'write_to', '_t.PathT | None', 'write_to_template', 'str | None', 'relative_to', 'str | None', 'tag_regex', 'str', 'parentdir_prefix_version', 'str | None', 'fallback_version', 'str | None', 'fallback_root', '_t.PathT', 'parse', 'Any | None', 'git_describe_command', 'Any | None', 'dist_name', 'str | None', 'version_cls', 'Any | None', 'normalize', 'bool', 'search_parent_directories', 'bool', 'return', 'str')
       ('config', 'Configuration', 'return', 'str | None')
    names      ('__doc__', '__future__', 'annotations', 'os', 'warnings', 'typing', 'Any', 'Callable', 'TYPE_CHECKING', '_entrypoints', '_call_entrypoint_fn', '_version_from_entrypoints', '_overrides', '_read_pretended_version_for', 'PRETEND_KEY', 'PRETEND_KEY_NAMED', '_version_cls', '_version_as_tuple', 'NonNormalizedVersion', 'Version', 'config', 'Configuration', 'DEFAULT_LOCAL_SCHEME', 'DEFAULT_TAG_REGEX', 'DEFAULT_VERSION_SCHEME', 'discover', 'iter_matching_entrypoints', 'utils', 'function_has_arg', 'trace', 'version', 'format_version', 'meta', 'ScmVersion', 'NoReturn', '', '_types', '_t', 'TEMPLATES', 'version_from_scm', 'dump_version', '_do_parse', '_version_missing', 'get_version', '_get_version', '__all__')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020104040c02080108010c010c010c020c010c010c010c010c010c
       010c010c010c010c010c010c010c010c010c010c010c010c0204010c020c
       03020602f9060b080e02fc0a17081a080e02010201020102010201020102
       010201020102010201020102010201020102f00a200815
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_entrypoints.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 2696
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 2795
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 16777216
    code
       0x9700640064016c006d015a010100640064026c025a02640064036c036d
@@ -108,41 +108,41 @@
                146 JUMP_FORWARD            15 (to 178)
    
     18     >>  148 LOAD_NAME                4 (Any)
                150 STORE_NAME              14 (Configuration)
    
     20         152 PUSH_NULL
                154 LOAD_BUILD_CLASS
-               156 LOAD_CONST              14 (<code object Protocol, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 20>)
+               156 LOAD_CONST              14 (<code object Protocol, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 20>)
                158 MAKE_FUNCTION            0
                160 LOAD_CONST              15 ('Protocol')
                162 PRECALL                  2
                166 CALL                     2
                176 STORE_NAME              16 (Protocol)
    
     24     >>  178 PUSH_NULL
                180 LOAD_BUILD_CLASS
-               182 LOAD_CONST              16 (<code object MaybeConfigFunction, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 24>)
+               182 LOAD_CONST              16 (<code object MaybeConfigFunction, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 24>)
                184 MAKE_FUNCTION            0
                186 LOAD_CONST              17 ('MaybeConfigFunction')
                188 LOAD_NAME               16 (Protocol)
                190 PRECALL                  3
                194 CALL                     3
                204 STORE_NAME              20 (MaybeConfigFunction)
    
     36         206 LOAD_CONST              40 (('root', '_t.PathT', 'config', 'Configuration', 'fn', 'MaybeConfigFunction', 'return', 'ScmVersion | None'))
-               208 LOAD_CONST              25 (<code object _call_entrypoint_fn, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 36>)
+               208 LOAD_CONST              25 (<code object _call_entrypoint_fn, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 36>)
                210 MAKE_FUNCTION            4 (annotations)
                212 STORE_NAME              21 (_call_entrypoint_fn)
    
     53         214 NOP
    
     52         216 LOAD_CONST              41 ((False,))
                218 LOAD_CONST              42 (('config', 'Configuration', 'fallback', 'bool', 'return', 'ScmVersion | None'))
-               220 LOAD_CONST              29 (<code object _version_from_entrypoints, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 52>)
+               220 LOAD_CONST              29 (<code object _version_from_entrypoints, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 52>)
                222 MAKE_FUNCTION            5 (defaults, annotations)
                224 STORE_NAME              22 (_version_from_entrypoints)
    
     73         226 NOP
    
     74         228 LOAD_CONST               0 (0)
                230 LOAD_CONST              30 (('entry_points',))
@@ -178,15 +178,15 @@
                280 LOAD_CONST              31 (('defaultdict',))
                282 IMPORT_NAME             27 (collections)
                284 IMPORT_FROM             28 (defaultdict)
                286 STORE_NAME              28 (defaultdict)
                288 POP_TOP
    
     81         290 LOAD_CONST              43 (('return', 'dict[str, list[_t.EntrypointProtocol]]'))
-               292 LOAD_CONST              33 (<code object entry_points, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 81>)
+               292 LOAD_CONST              33 (<code object entry_points, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 81>)
                294 MAKE_FUNCTION            4 (annotations)
                296 STORE_NAME              24 (entry_points)
                298 POP_EXCEPT
                300 JUMP_FORWARD             4 (to 310)
    
     78     >>  302 RERAISE                  0
            >>  304 COPY                     3
@@ -200,15 +200,15 @@
                318 POP_EXCEPT
                320 RERAISE                  1
    
     90     >>  322 NOP
    
     89         324 LOAD_CONST              44 ((None,))
                326 LOAD_CONST              45 (('group', 'str', 'name', 'str | None', 'return', 'Iterator[_t.EntrypointProtocol]'))
-               328 LOAD_CONST              39 (<code object iter_entry_points, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 89>)
+               328 LOAD_CONST              39 (<code object iter_entry_points, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 89>)
                330 MAKE_FUNCTION            5 (defaults, annotations)
                332 STORE_NAME              29 (iter_entry_points)
                334 LOAD_CONST               2 (None)
                336 RETURN_VALUE
    ExceptionTable:
      228 to 238 -> 242 [0]
      242 to 250 -> 316 [1] lasti
@@ -251,15 +251,15 @@
          consts
             'Protocol'
             None
          names      ('__name__', '__module__', '__qualname__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
          name       'Protocol'
          firstlineno 20
          lnotab 0x0a01
       'Protocol'
       code
          argcount  : 0
          nlocals   : 0
@@ -280,26 +280,26 @@
                       14 LOAD_NAME                3 (__annotations__)
                       16 LOAD_CONST               2 ('__name__')
                       18 STORE_SUBSCR
          
           27          22 LOAD_NAME                4 (overload)
          
           28          24 LOAD_CONST              12 (('root', '_t.PathT', 'config', 'Configuration', 'return', 'ScmVersion | None'))
-                      26 LOAD_CONST               9 (<code object __call__, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 27>)
+                      26 LOAD_CONST               9 (<code object __call__, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 27>)
                       28 MAKE_FUNCTION            4 (annotations)
          
           27          30 PRECALL                  0
                       34 CALL                     0
          
           28          44 STORE_NAME               5 (__call__)
          
           31          46 LOAD_NAME                4 (overload)
          
           32          48 LOAD_CONST              13 (('root', '_t.PathT', 'return', 'ScmVersion | None'))
-                      50 LOAD_CONST              10 (<code object __call__, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 31>)
+                      50 LOAD_CONST              10 (<code object __call__, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 31>)
                       52 MAKE_FUNCTION            4 (annotations)
          
           31          54 PRECALL                  0
                       58 CALL                     0
          
           32          68 STORE_NAME               5 (__call__)
                       70 LOAD_CONST              11 (None)
@@ -326,15 +326,15 @@
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'root', 'config')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
                name       '__call__'
                firstlineno 27
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
@@ -346,26 +346,26 @@
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'root')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
                name       '__call__'
                firstlineno 31
                lnotab 0x0202
             None
             ('root', '_t.PathT', 'config', 'Configuration', 'return', 'ScmVersion | None')
             ('root', '_t.PathT', 'return', 'ScmVersion | None')
          names      ('__name__', '__module__', '__qualname__', '__annotations__', 'overload', '__call__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
          name       'MaybeConfigFunction'
          firstlineno 24
          lnotab 0x0c010a02020106ff0e010203020106ff0e01
       'MaybeConfigFunction'
       'root'
       '_t.PathT'
       'config'
@@ -441,15 +441,15 @@
             " are required to provide a named argument 'config', setuptools_scm>=8.0 will remove support."
             2
             ('category', 'stacklevel')
          names      ('function_has_arg', 'warnings', 'warn', '__module__', '__name__', 'DeprecationWarning')
          varnames   ('root', 'config', 'fn')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
          name       '_call_entrypoint_fn'
          firstlineno 36
          lnotab 0x020320011a02160124030c0102fb1207
       False
       'fallback'
       'bool'
       code
@@ -550,15 +550,15 @@
             1
             ('iter_matching_entrypoints',)
             'version_from_ep'
          names      ('fallback_root', 'absolute_root', 'discover', 'iter_matching_entrypoints', 'trace', '_call_entrypoint_fn', 'load')
          varnames   ('config', 'fallback', 'entrypoint', 'root', 'iter_matching_entrypoints', 'ep', 'version')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
          name       '_version_from_entrypoints'
          firstlineno 52
          lnotab 0x020304010401100204010e020c0222011e0146012001040108ff0202
       ('entry_points',)
       ('defaultdict',)
       'dict[str, list[_t.EntrypointProtocol]]'
       code
@@ -589,15 +589,15 @@
          consts
             None
             'importlib metadata missing, this may happen at build time for python3.7'
          names      ('warnings', 'warn', 'defaultdict', 'list')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
          name       'entry_points'
          firstlineno 81
          lnotab 0x0201160102ff1004
       'group'
       'str'
       'name'
       'str | None'
@@ -652,15 +652,15 @@
                      142 LOAD_FAST                3 (eps)
                      144 PRECALL                  1
                      148 CALL                     1
                      158 RETURN_VALUE
          
           99     >>  160 LOAD_CLOSURE             1 (name)
                      162 BUILD_TUPLE              1
-                     164 LOAD_CONST               3 (<code object <genexpr>, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 99>)
+                     164 LOAD_CONST               3 (<code object <genexpr>, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_entrypoints.py", line 99>)
                      166 MAKE_FUNCTION            8 (closure)
                      168 LOAD_FAST                3 (eps)
                      170 GET_ITER
                      172 PRECALL                  0
                      176 CALL                     0
                      186 RETURN_VALUE
          consts
@@ -697,36 +697,36 @@
                             48 RETURN_VALUE
                consts
                   None
                names      ('name',)
                varnames   ('.0', 'ep')
                freevars   ('name',)
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
                name       '<genexpr>'
                firstlineno 99
                lnotab 0x
          names      ('entry_points', 'hasattr', 'select', 'iter')
          varnames   ('group', 'name', 'all_eps', 'eps')
          freevars   ()
          cellvars   ('name',)
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
          name       'iter_entry_points'
          firstlineno 89
          lnotab 0x04031c0120012e02100104011e01
       ('root', '_t.PathT', 'config', 'Configuration', 'fn', 'MaybeConfigFunction', 'return', 'ScmVersion | None')
       (False,)
       ('config', 'Configuration', 'fallback', 'bool', 'return', 'ScmVersion | None')
       ('return', 'dict[str, list[_t.EntrypointProtocol]]')
       (None,)
       ('group', 'str', 'name', 'str | None', 'return', 'Iterator[_t.EntrypointProtocol]')
    names      ('__future__', 'annotations', 'warnings', 'typing', 'Any', 'Iterator', 'overload', 'TYPE_CHECKING', 'utils', 'function_has_arg', 'trace', 'version', 'ScmVersion', 'config', 'Configuration', 'typing_extensions', 'Protocol', '', '_types', '_t', 'MaybeConfigFunction', '_call_entrypoint_fn', '_version_from_entrypoints', 'importlib.metadata', 'entry_points', 'ImportError', 'importlib_metadata', 'collections', 'defaultdict', 'iter_entry_points')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_entrypoints.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c0208010c010c010c010c020c010c010c0204010c010c010e
       0204021a041c0c081102ff0a150201100108010201100108010c020cfd0c
       fd080f02ff
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_overrides.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 1067
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 1105
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 16777216
    code
       0x9700640064016c006d015a010100640064026c025a02640364046c036d
@@ -58,15 +58,15 @@
    
     12          74 LOAD_NAME               10 (PRETEND_KEY)
                 76 LOAD_CONST               9 ('_FOR_{name}')
                 78 BINARY_OP                0 (+)
                 82 STORE_NAME              11 (PRETEND_KEY_NAMED)
    
     15          84 LOAD_CONST              15 (('config', 'Configuration', 'return', 'ScmVersion | None'))
-                86 LOAD_CONST              14 (<code object _read_pretended_version_for, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_overrides.py", line 15>)
+                86 LOAD_CONST              14 (<code object _read_pretended_version_for, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_overrides.py", line 15>)
                 88 MAKE_FUNCTION            4 (annotations)
                 90 STORE_NAME              12 (_read_pretended_version_for)
                 92 LOAD_CONST               2 (None)
                 94 RETURN_VALUE
    consts
       0
       ('annotations',)
@@ -169,20 +169,20 @@
             ('name',)
             True
             ('tag', 'preformatted', 'config')
          names      ('trace', 'dist_name', 'os', 'environ', 'get', 'PRETEND_KEY_NAMED', 'format', 'upper', 'PRETEND_KEY', 'meta')
          varnames   ('config', 'pretended')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_overrides.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_overrides.py'
          name       '_read_pretended_version_for'
          firstlineno 15
          lnotab 0x02062a020e012c0162ff120404020401480204032402
       ('config', 'Configuration', 'return', 'ScmVersion | None')
    names      ('__future__', 'annotations', 'os', 'config', 'Configuration', 'utils', 'trace', 'version', 'meta', 'ScmVersion', 'PRETEND_KEY', 'PRETEND_KEY_NAMED', '_read_pretended_version_for')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_overrides.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_overrides.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0208020c010c010c010c0304010a03
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/_version_cls.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 1575
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 1623
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 16777216
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -39,24 +39,24 @@
                 42 IMPORT_NAME              4 (packaging.version)
                 44 IMPORT_FROM              6 (Version)
                 46 STORE_NAME               6 (Version)
                 48 POP_TOP
    
      9          50 PUSH_NULL
                 52 LOAD_BUILD_CLASS
-                54 LOAD_CONST               5 (<code object NonNormalizedVersion, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_version_cls.py", line 9>)
+                54 LOAD_CONST               5 (<code object NonNormalizedVersion, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_version_cls.py", line 9>)
                 56 MAKE_FUNCTION            0
                 58 LOAD_CONST               6 ('NonNormalizedVersion')
                 60 LOAD_NAME                6 (Version)
                 62 PRECALL                  3
                 66 CALL                     3
                 76 STORE_NAME               7 (NonNormalizedVersion)
    
     34          78 LOAD_CONST              13 (('version_str', 'str', 'return', 'tuple[int | str, ...]'))
-                80 LOAD_CONST              11 (<code object _version_as_tuple, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_version_cls.py", line 34>)
+                80 LOAD_CONST              11 (<code object _version_as_tuple, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_version_cls.py", line 34>)
                 82 MAKE_FUNCTION            4 (annotations)
                 84 STORE_NAME               8 (_version_as_tuple)
                 86 LOAD_CONST              12 (None)
                 88 RETURN_VALUE
    consts
       0
       ('annotations',)
@@ -81,25 +81,25 @@
          
           10          12 LOAD_CONST               1 ('A non-normalizing version handler.\n\n    You can use this class to preserve version verification but skip normalization.\n    For example you can use this to avoid git release candidate version tags\n    ("1.0.0-rc1") to be normalized to "1.0.0rc1". Only use this if you fully\n    trust the version tags.\n    ')
                       14 STORE_NAME               3 (__doc__)
          
           18          16 LOAD_CONST               9 (('version', 'str', 'return', 'None'))
                       18 LOAD_CLOSURE             0 (__class__)
                       20 BUILD_TUPLE              1
-                      22 LOAD_CONST               6 (<code object __init__, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_version_cls.py", line 18>)
+                      22 LOAD_CONST               6 (<code object __init__, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_version_cls.py", line 18>)
                       24 MAKE_FUNCTION           12 (annotations, closure)
                       26 STORE_NAME               4 (__init__)
          
           25          28 LOAD_CONST              10 (('return', 'str'))
-                      30 LOAD_CONST               7 (<code object __str__, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_version_cls.py", line 25>)
+                      30 LOAD_CONST               7 (<code object __str__, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_version_cls.py", line 25>)
                       32 MAKE_FUNCTION            4 (annotations)
                       34 STORE_NAME               5 (__str__)
          
           29          36 LOAD_CONST              10 (('return', 'str'))
-                      38 LOAD_CONST               8 (<code object __repr__, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_version_cls.py", line 29>)
+                      38 LOAD_CONST               8 (<code object __repr__, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_version_cls.py", line 29>)
                       40 MAKE_FUNCTION            4 (annotations)
                       42 STORE_NAME               6 (__repr__)
                       44 LOAD_CLOSURE             0 (__class__)
                       46 COPY                     1
                       48 STORE_NAME               7 (__classcell__)
                       50 RETURN_VALUE
          consts
@@ -138,15 +138,15 @@
                             86 RETURN_VALUE
                consts
                   None
                names      ('super', '__init__', '_raw_version')
                varnames   ('self', 'version')
                freevars   ('__class__',)
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_version_cls.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_version_cls.py'
                name       '__init__'
                firstlineno 18
                lnotab 0x04024203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -159,15 +159,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_raw_version',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_version_cls.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_version_cls.py'
                name       '__str__'
                firstlineno 25
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -186,25 +186,25 @@
                   None
                   '<NonNormalizedVersion('
                   ')>'
                names      ('_raw_version',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_version_cls.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_version_cls.py'
                name       '__repr__'
                firstlineno 29
                lnotab 0x0202
             ('version', 'str', 'return', 'None')
             ('return', 'str')
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', '__str__', '__repr__', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_version_cls.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_version_cls.py'
          name       'NonNormalizedVersion'
          firstlineno 9
          lnotab 0x0c0104080c070804
       'NonNormalizedVersion'
       'version_str'
       'str'
       'return'
@@ -305,21 +305,21 @@
             'dev'
             'setuptools_scm'
             'failed to parse version %s'
          names      ('Version', 'release', 'dev', 'local', 'InvalidVersion', 'getLogger', 'exception')
          varnames   ('version_str', 'parsed_version', 'version_fields', 'log')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_version_cls.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_version_cls.py'
          name       '_version_as_tuple'
          firstlineno 34
          lnotab 0x020102011e070e010e011c010e01160106f512021e012c010afc
       None
       ('version_str', 'str', 'return', 'tuple[int | str, ...]')
    names      ('__future__', 'annotations', 'logging', 'getLogger', 'packaging.version', 'InvalidVersion', 'Version', 'NonNormalizedVersion', '_version_as_tuple')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_version_cls.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_version_cls.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c020c020c010c031c19
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/config.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 7237
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 7453
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 16777216
    code
       0x970064005a00640164026c016d025a020100640164036c035a03640164
@@ -152,38 +152,38 @@
     29         218 LOAD_CONST              20 ('guess-next-dev')
                220 STORE_NAME              30 (DEFAULT_VERSION_SCHEME)
    
     30         222 LOAD_CONST              21 ('node-and-date')
                224 STORE_NAME              31 (DEFAULT_LOCAL_SCHEME)
    
     33         226 LOAD_CONST              41 (('value', 'str | Pattern[str] | None', 'return', 'Pattern[str]'))
-               228 LOAD_CONST              26 (<code object _check_tag_regex, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 33>)
+               228 LOAD_CONST              26 (<code object _check_tag_regex, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 33>)
                230 MAKE_FUNCTION            4 (annotations)
                232 STORE_NAME              32 (_check_tag_regex)
    
     48         234 LOAD_CONST              42 (('root', '_t.PathT', 'relative_to', '_t.PathT | None', 'return', 'str'))
-               236 LOAD_CONST              32 (<code object _check_absolute_root, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 48>)
+               236 LOAD_CONST              32 (<code object _check_absolute_root, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 48>)
                238 MAKE_FUNCTION            4 (annotations)
                240 STORE_NAME              33 (_check_absolute_root)
    
     74         242 LOAD_NAME               13 (Union)
                244 LOAD_NAME               21 (Version)
                246 LOAD_NAME               20 (NonNormalizedVersion)
                248 BUILD_TUPLE              2
                250 BINARY_SUBSCR
                260 STORE_NAME              34 (_VersionT)
    
     77         262 LOAD_CONST              43 (('version_cls', 'type[_VersionT] | str | None', 'normalize', 'bool', 'return', 'type[_VersionT]'))
-               264 LOAD_CONST              38 (<code object _validate_version_cls, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 77>)
+               264 LOAD_CONST              38 (<code object _validate_version_cls, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 77>)
                266 MAKE_FUNCTION            4 (annotations)
                268 STORE_NAME              35 (_validate_version_cls)
    
    106         270 PUSH_NULL
                272 LOAD_BUILD_CLASS
-               274 LOAD_CONST              39 (<code object Configuration, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 106>)
+               274 LOAD_CONST              39 (<code object Configuration, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 106>)
                276 MAKE_FUNCTION            0
                278 LOAD_CONST              40 ('Configuration')
                280 PRECALL                  2
                284 CALL                     2
                294 STORE_NAME              36 (Configuration)
                296 LOAD_CONST               3 (None)
                298 RETURN_VALUE
@@ -281,15 +281,15 @@
             1
             'version'
             "Expected tag_regex to contain a single match group or a group named 'version' to identify the version part of any tag."
          names      ('DEFAULT_TAG_REGEX', 're', 'compile', 'groupindex', 'keys', 'groups', 'warnings', 'warn')
          varnames   ('value', 'regex', 'group_names')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
          name       '_check_tag_regex'
          firstlineno 33
          lnotab 0x020104010e01280232013401160102ff1005
       'root'
       '_t.PathT'
       'relative_to'
       '_t.PathT | None'
@@ -468,15 +468,15 @@
             '\nassuming the parent directory was passed'
             'dir'
             'file'
          names      ('trace', 'repr', 'locals', 'os', 'path', 'isabs', 'commonpath', 'warnings', 'warn', 'isdir', 'join', 'dirname', 'abspath')
          varnames   ('root', 'relative_to')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
          name       '_check_absolute_root'
          firstlineno 48
          lnotab
             0x0201520106023cff02023cfe02034a0218020cff02ff10043e01180306
             fe02ff10052001420220017a01
       'version_cls'
       'type[_VersionT] | str | None'
@@ -600,15 +600,15 @@
             1
             "Unable to import version_cls='"
             "'"
          names      ('ValueError', 'NonNormalizedVersion', 'Version', 'isinstance', 'str', 'importlib', 'rsplit', 'import_module', 'cast', 'Type', '_VersionT', 'getattr')
          varnames   ('version_cls', 'normalize', 'importlib', 'pkg', 'cls_name', 'version_cls_host')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
          name       '_validate_version_cls'
          firstlineno 77
          lnotab
             0x0203040204010c0102ff10040e0304010e012a010202080232012a015e
             0102012c02
       code
          argcount  : 0
@@ -690,114 +690,114 @@
          
          132          84 LOAD_CONST              12 (True)
          
          133          86 LOAD_CONST              13 (False)
          
          114          88 BUILD_TUPLE             16
                       90 LOAD_CONST              57 (('relative_to', '_t.PathT | None', 'root', '_t.PathT', 'version_scheme', 'str | Callable[[ScmVersion], str | None]', 'local_scheme', 'str | Callable[[ScmVersion], str | None]', 'write_to', '_t.PathT | None', 'write_to_template', 'str | None', 'tag_regex', 'str | Pattern[str]', 'parentdir_prefix_version', 'str | None', 'fallback_version', 'str | None', 'fallback_root', '_t.PathT', 'parse', 'Any | None', 'git_describe_command', '_t.CMD_TYPE | None', 'dist_name', 'str | None', 'version_cls', 'type[_VersionT] | type | str | None', 'normalize', 'bool', 'search_parent_directories', 'bool'))
-                      92 LOAD_CONST              36 (<code object __init__, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 114>)
+                      92 LOAD_CONST              36 (<code object __init__, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 114>)
                       94 MAKE_FUNCTION            5 (defaults, annotations)
                       96 STORE_NAME               8 (__init__)
          
          156          98 LOAD_NAME                9 (property)
          
          157         100 LOAD_CONST              58 (('return', 'str'))
-                     102 LOAD_CONST              38 (<code object fallback_root, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 156>)
+                     102 LOAD_CONST              38 (<code object fallback_root, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 156>)
                      104 MAKE_FUNCTION            4 (annotations)
          
          156         106 PRECALL                  0
                      110 CALL                     0
          
          157         120 STORE_NAME              10 (fallback_root)
          
          160         122 LOAD_NAME               10 (fallback_root)
                      124 LOAD_ATTR               11 (setter)
          
          161         134 LOAD_CONST              59 (('value', '_t.PathT', 'return', 'None'))
-                     136 LOAD_CONST              41 (<code object fallback_root, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 160>)
+                     136 LOAD_CONST              41 (<code object fallback_root, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 160>)
                      138 MAKE_FUNCTION            4 (annotations)
          
          160         140 PRECALL                  0
                      144 CALL                     0
          
          161         154 STORE_NAME              10 (fallback_root)
          
          164         156 LOAD_NAME                9 (property)
          
          165         158 LOAD_CONST              58 (('return', 'str'))
-                     160 LOAD_CONST              42 (<code object absolute_root, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 164>)
+                     160 LOAD_CONST              42 (<code object absolute_root, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 164>)
                      162 MAKE_FUNCTION            4 (annotations)
          
          164         164 PRECALL                  0
                      168 CALL                     0
          
          165         178 STORE_NAME              12 (absolute_root)
          
          168         180 LOAD_NAME                9 (property)
          
          169         182 LOAD_CONST              60 (('return', 'str | None'))
-                     184 LOAD_CONST              43 (<code object relative_to, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 168>)
+                     184 LOAD_CONST              43 (<code object relative_to, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 168>)
                      186 MAKE_FUNCTION            4 (annotations)
          
          168         188 PRECALL                  0
                      192 CALL                     0
          
          169         202 STORE_NAME              13 (relative_to)
          
          172         204 LOAD_NAME               13 (relative_to)
                      206 LOAD_ATTR               11 (setter)
          
          173         216 LOAD_CONST              59 (('value', '_t.PathT', 'return', 'None'))
-                     218 LOAD_CONST              44 (<code object relative_to, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 172>)
+                     218 LOAD_CONST              44 (<code object relative_to, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 172>)
                      220 MAKE_FUNCTION            4 (annotations)
          
          172         222 PRECALL                  0
                      226 CALL                     0
          
          173         236 STORE_NAME              13 (relative_to)
          
          179         238 LOAD_NAME                9 (property)
          
          180         240 LOAD_CONST              58 (('return', 'str'))
-                     242 LOAD_CONST              45 (<code object root, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 179>)
+                     242 LOAD_CONST              45 (<code object root, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 179>)
                      244 MAKE_FUNCTION            4 (annotations)
          
          179         246 PRECALL                  0
                      250 CALL                     0
          
          180         260 STORE_NAME              14 (root)
          
          183         262 LOAD_NAME               14 (root)
                      264 LOAD_ATTR               11 (setter)
          
          184         274 LOAD_CONST              59 (('value', '_t.PathT', 'return', 'None'))
-                     276 LOAD_CONST              46 (<code object root, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 183>)
+                     276 LOAD_CONST              46 (<code object root, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 183>)
                      278 MAKE_FUNCTION            4 (annotations)
          
          183         280 PRECALL                  0
                      284 CALL                     0
          
          184         294 STORE_NAME              14 (root)
          
          190         296 LOAD_NAME                9 (property)
          
          191         298 LOAD_CONST              61 (('return', 'Pattern[str]'))
-                     300 LOAD_CONST              48 (<code object tag_regex, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 190>)
+                     300 LOAD_CONST              48 (<code object tag_regex, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 190>)
                      302 MAKE_FUNCTION            4 (annotations)
          
          190         304 PRECALL                  0
                      308 CALL                     0
          
          191         318 STORE_NAME              15 (tag_regex)
          
          194         320 LOAD_NAME               15 (tag_regex)
                      322 LOAD_ATTR               11 (setter)
          
          195         332 LOAD_CONST              62 (('value', 'str | Pattern[str]', 'return', 'None'))
-                     334 LOAD_CONST              49 (<code object tag_regex, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 194>)
+                     334 LOAD_CONST              49 (<code object tag_regex, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 194>)
                      336 MAKE_FUNCTION            4 (annotations)
          
          194         338 PRECALL                  0
                      342 CALL                     0
          
          195         352 STORE_NAME              15 (tag_regex)
          
@@ -807,15 +807,15 @@
          
          202         358 NOP
          
          203         360 NOP
          
          199         362 LOAD_CONST              63 (('pyproject.toml', None, None))
                      364 LOAD_CONST              64 (('name', 'str', 'dist_name', 'str | None', '_load_toml', 'Callable[[str], dict[str, Any]] | None', 'kwargs', 'Any', 'return', 'Configuration'))
-                     366 LOAD_CONST              56 (<code object from_file, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 198>)
+                     366 LOAD_CONST              56 (<code object from_file, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\config.py", line 198>)
                      368 MAKE_FUNCTION            5 (defaults, annotations)
          
          198         370 PRECALL                  0
                      374 CALL                     0
          
          199         384 STORE_NAME              17 (from_file)
                      386 LOAD_CONST              10 (None)
@@ -965,15 +965,15 @@
                consts
                   None
                   '.'
                names      ('os', 'fspath', '_relative_to', '_root', 'root', 'version_scheme', 'local_scheme', 'write_to', 'write_to_template', 'parentdir_prefix_version', 'fallback_version', 'fallback_root', 'parse', 'tag_regex', 'git_describe_command', 'dist_name', 'search_parent_directories', 'parent', '_validate_version_cls', 'version_cls')
                varnames   ('self', 'relative_to', 'root', 'version_scheme', 'local_scheme', 'write_to', 'write_to_template', 'tag_regex', 'parentdir_prefix_version', 'fallback_version', 'fallback_root', 'parse', 'git_describe_command', 'dist_name', 'version_cls', 'normalize', 'search_parent_directories')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
                name       '__init__'
                firstlineno 114
                lnotab
                   0x02163a010e0232010e010e010e010e010e010e010e010e010e010e010e
                   010e010e02
             'return'
             code
@@ -989,15 +989,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_fallback_root',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
                name       'fallback_root'
                firstlineno 156
                lnotab 0x0202
             'value'
             'None'
             code
                argcount  : 2
@@ -1022,15 +1022,15 @@
                             76 RETURN_VALUE
                consts
                   None
                names      ('os', 'path', 'abspath', '_fallback_root')
                varnames   ('self', 'value')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
                name       'fallback_root'
                firstlineno 160
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1043,15 +1043,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_absolute_root',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
                name       'absolute_root'
                firstlineno 164
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1064,15 +1064,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_relative_to',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
                name       'relative_to'
                firstlineno 168
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
@@ -1131,15 +1131,15 @@
                   None
                   'root'
                   'relative_to'
                names      ('_check_absolute_root', '_root', '_absolute_root', 'os', 'fspath', '_relative_to', 'trace', 'repr')
                varnames   ('self', 'value')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
                name       'relative_to'
                firstlineno 172
                lnotab 0x0202340132014401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -1152,15 +1152,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_root',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
                name       'root'
                firstlineno 179
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
@@ -1221,15 +1221,15 @@
                   None
                   'root'
                   'relative_to'
                names      ('_check_absolute_root', '_relative_to', '_absolute_root', 'os', 'fspath', '_root', 'trace', 'repr')
                varnames   ('self', 'value')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
                name       'root'
                firstlineno 183
                lnotab 0x0202340132014401
             'Pattern[str]'
             code
                argcount  : 1
                nlocals   : 1
@@ -1243,15 +1243,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('_tag_regex',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
                name       'tag_regex'
                firstlineno 190
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -1271,15 +1271,15 @@
                             44 RETURN_VALUE
                consts
                   None
                names      ('_check_tag_regex', '_tag_regex')
                varnames   ('self', 'value')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
                name       'tag_regex'
                firstlineno 194
                lnotab 0x0202
             'pyproject.toml'
             'name'
             '_load_toml'
             'Callable[[str], dict[str, Any]] | None'
@@ -1328,15 +1328,15 @@
                   ('_load_toml',)
                   'relative_to'
                   ()
                names      ('_read_pyproject', '_get_args_for_pyproject')
                varnames   ('cls', 'name', 'dist_name', '_load_toml', 'kwargs', 'pyproject_data', 'args')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
                name       'from_file'
                firstlineno 198
                lnotab 0x020f22012202
             ('relative_to', '_t.PathT | None', 'root', '_t.PathT', 'version_scheme', 'str | Callable[[ScmVersion], str | None]', 'local_scheme', 'str | Callable[[ScmVersion], str | None]', 'write_to', '_t.PathT | None', 'write_to_template', 'str | None', 'tag_regex', 'str | Pattern[str]', 'parentdir_prefix_version', 'str | None', 'fallback_version', 'str | None', 'fallback_root', '_t.PathT', 'parse', 'Any | None', 'git_describe_command', '_t.CMD_TYPE | None', 'dist_name', 'str | None', 'version_cls', 'type[_VersionT] | type | str | None', 'normalize', 'bool', 'search_parent_directories', 'bool')
             ('return', 'str')
             ('value', '_t.PathT', 'return', 'None')
             ('return', 'str | None')
@@ -1344,15 +1344,15 @@
             ('value', 'str | Pattern[str]', 'return', 'None')
             ('pyproject.toml', None, None)
             ('name', 'str', 'dist_name', 'str | None', '_load_toml', 'Callable[[str], dict[str, Any]] | None', 'kwargs', 'Any', 'return', 'Configuration')
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__annotations__', 'DEFAULT_VERSION_SCHEME', 'DEFAULT_LOCAL_SCHEME', 'DEFAULT_TAG_REGEX', '__init__', 'property', 'fallback_root', 'setter', 'absolute_root', 'relative_to', 'root', 'tag_regex', 'classmethod', 'from_file')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
          name       'Configuration'
          firstlineno 106
          lnotab
             0x0c0104020a010a010a010a040201020302010201020102010201020102
             0102010201020102010201020102ed0a2a020106ff0e0102030c0106ff0e
             010203020106ff0e010203020106ff0e0102030c0106ff0e010206020106
             ff0e0102030c0106ff0e010206020106ff0e0102030c0106ff0e01020302
@@ -1361,13 +1361,13 @@
       ('value', 'str | Pattern[str] | None', 'return', 'Pattern[str]')
       ('root', '_t.PathT', 'relative_to', '_t.PathT | None', 'return', 'str')
       ('version_cls', 'type[_VersionT] | str | None', 'normalize', 'bool', 'return', 'type[_VersionT]')
    names      ('__doc__', '__future__', 'annotations', 'os', 're', 'warnings', 'typing', 'Any', 'Callable', 'cast', 'Pattern', 'Type', 'TYPE_CHECKING', 'Union', '_integration.pyproject_reading', 'get_args_for_pyproject', '_get_args_for_pyproject', 'read_pyproject', '_read_pyproject', '_version_cls', 'NonNormalizedVersion', 'Version', 'utils', 'trace', '', '_types', '_t', 'setuptools_scm.version', 'ScmVersion', 'DEFAULT_TAG_REGEX', 'DEFAULT_VERSION_SCHEME', 'DEFAULT_LOCAL_SCHEME', '_check_tag_regex', '_check_absolute_root', '_VersionT', '_validate_version_cls', 'Configuration')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\config.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020104010c020801080108010c010c010c010c010c010c010c020c
       030c010c010c010c0304010c010c02040104010403080f081a1403081d
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/discover.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 1867
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 1936
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 16777216
    code
       0x9700640064016c006d015a010100640064026c025a02640064036c036d
@@ -71,25 +71,25 @@
                 94 STORE_NAME              13 (trace)
                 96 POP_TOP
    
     15          98 NOP
    
     14         100 LOAD_CONST              26 ((True,))
                102 LOAD_CONST              27 (('root', '_t.PathT', 'search_parents', 'bool', 'return', 'Iterator[_t.PathT]'))
-               104 LOAD_CONST              17 (<code object walk_potential_roots, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\discover.py", line 14>)
+               104 LOAD_CONST              17 (<code object walk_potential_roots, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\discover.py", line 14>)
                106 MAKE_FUNCTION            5 (defaults, annotations)
                108 STORE_NAME              14 (walk_potential_roots)
    
     34         110 LOAD_CONST              28 (('root', '_t.PathT', 'name', 'str', 'return', 'bool'))
-               112 LOAD_CONST              20 (<code object match_entrypoint, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\discover.py", line 34>)
+               112 LOAD_CONST              20 (<code object match_entrypoint, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\discover.py", line 34>)
                114 MAKE_FUNCTION            4 (annotations)
                116 STORE_NAME              15 (match_entrypoint)
    
     50         118 LOAD_CONST              29 (('root', '_t.PathT', 'entrypoint', 'str', 'config', 'Configuration', 'return', 'Iterable[_t.EntrypointProtocol]'))
-               120 LOAD_CONST              25 (<code object iter_matching_entrypoints, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\discover.py", line 50>)
+               120 LOAD_CONST              25 (<code object iter_matching_entrypoints, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\discover.py", line 50>)
                122 MAKE_FUNCTION            4 (annotations)
                124 STORE_NAME              16 (iter_matching_entrypoints)
                126 LOAD_CONST               2 (None)
                128 RETURN_VALUE
    consts
       0
       ('annotations',)
@@ -163,15 +163,15 @@
          consts
             '\n    Iterate though a path and each of its parents.\n    :param root: File path.\n    :param search_parents: If ``False`` the parents are not considered.\n    '
             None
          names      ('os', 'path', 'split')
          varnames   ('root', 'search_parents', 'tail')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\discover.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\discover.py'
          name       'walk_potential_roots'
          firstlineno 14
          lnotab 0x060904010801040204020401080144fe
       'name'
       'str'
       code
          argcount  : 2
@@ -228,15 +228,15 @@
             True
             'ignoring bad ep'
             False
          names      ('os', 'path', 'exists', 'join', 'isabs', 'trace')
          varnames   ('root', 'name')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\discover.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\discover.py'
          name       'match_entrypoint'
          firstlineno 34
          lnotab 0x02087a013e0104012002
       'entrypoint'
       'config'
       'Configuration'
       'Iterable[_t.EntrypointProtocol]'
@@ -331,23 +331,23 @@
             'found ep'
             'in'
             None
          names      ('trace', '_entrypoints', 'iter_entry_points', 'walk_potential_roots', 'search_parent_directories', 'match_entrypoint', 'name', 'parent')
          varnames   ('root', 'entrypoint', 'config', 'iter_entry_points', 'wd', 'ep')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\discover.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\discover.py'
          name       'iter_matching_entrypoints'
          firstlineno 50
          lnotab 0x060b22010c022e011a012a0124010e010afc02ff
       (True,)
       ('root', '_t.PathT', 'search_parents', 'bool', 'return', 'Iterator[_t.PathT]')
       ('root', '_t.PathT', 'name', 'str', 'return', 'bool')
       ('root', '_t.PathT', 'entrypoint', 'str', 'config', 'Configuration', 'return', 'Iterable[_t.EntrypointProtocol]')
    names      ('__future__', 'annotations', 'os', 'typing', 'Iterable', 'Iterator', 'TYPE_CHECKING', '', '_types', '_t', 'config', 'Configuration', 'utils', 'trace', 'walk_potential_roots', 'match_entrypoint', 'iter_matching_entrypoints')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\discover.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\discover.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0208010c010c010c0204010c010c010c0402ff0a140810
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 3100
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 3186
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 16777216
    code
       0x9700640064016c006d015a010100640064026c025a02640064036c036d
@@ -56,20 +56,20 @@
                 70 STORE_NAME              11 (trace)
                 72 POP_TOP
    
     17          74 NOP
    
     13          76 LOAD_CONST              23 ((False,))
                 78 LOAD_CONST              24 (('path', '_t.PathT', 'scm_files', 'set[str]', 'scm_dirs', 'set[str]', 'force_all_files', 'bool', 'return', 'list[str]'))
-                80 LOAD_CONST              18 (<code object scm_find_files, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder.py", line 13>)
+                80 LOAD_CONST              18 (<code object scm_find_files, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder.py", line 13>)
                 82 MAKE_FUNCTION            5 (defaults, annotations)
                 84 STORE_NAME              12 (scm_find_files)
    
     76          86 LOAD_CONST              25 (('toplevel', 'str | None', 'return', 'TypeGuard[str]'))
-                88 LOAD_CONST              22 (<code object is_toplevel_acceptable, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder.py", line 76>)
+                88 LOAD_CONST              22 (<code object is_toplevel_acceptable, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder.py", line 76>)
                 90 MAKE_FUNCTION            4 (annotations)
                 92 STORE_NAME              13 (is_toplevel_acceptable)
                 94 LOAD_CONST               2 (None)
                 96 RETURN_VALUE
    consts
       0
       ('annotations',)
@@ -193,15 +193,15 @@
                      328 CALL                     1
                      338 STORE_DEREF             14 (realdirpath)
          
           41         340 LOAD_CONST              10 (('n', 'str', 'return', 'bool'))
                      342 LOAD_CLOSURE            14 (realdirpath)
                      344 LOAD_CLOSURE             1 (scm_files)
                      346 BUILD_TUPLE              2
-                     348 LOAD_CONST               7 (<code object _link_not_in_scm, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder.py", line 41>)
+                     348 LOAD_CONST               7 (<code object _link_not_in_scm, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder.py", line 41>)
                      350 MAKE_FUNCTION           12 (annotations, closure)
                      352 STORE_DEREF             13 (_link_not_in_scm)
          
           45         354 LOAD_DEREF               3 (force_all_files)
                      356 POP_JUMP_FORWARD_IF_TRUE    12 (to 382)
                      358 LOAD_DEREF              14 (realdirpath)
                      360 LOAD_FAST                2 (scm_dirs)
@@ -285,15 +285,15 @@
          
           60         768 EXTENDED_ARG             1
                      770 JUMP_BACKWARD          283 (to 206)
          
           61     >>  772 LOAD_CLOSURE            13 (_link_not_in_scm)
                      774 LOAD_CLOSURE             3 (force_all_files)
                      776 BUILD_TUPLE              2
-                     778 LOAD_CONST               9 (<code object <listcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder.py", line 61>)
+                     778 LOAD_CONST               9 (<code object <listcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder.py", line 61>)
                      780 MAKE_FUNCTION            8 (closure)
          
           62         782 LOAD_FAST                8 (dirnames)
          
           61         784 GET_ITER
                      786 PRECALL                  0
                      790 CALL                     0
@@ -431,15 +431,15 @@
                        >>  194 RETURN_VALUE
                consts
                   None
                names      ('os', 'path', 'join', 'normcase', 'islink')
                varnames   ('n', 'fn')
                freevars   ('realdirpath', 'scm_files')
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder.py'
                name       '_link_not_in_scm'
                firstlineno 41
                lnotab 0x04017a01
             None
             code
                argcount  : 1
                nlocals   : 2
@@ -474,24 +474,24 @@
                             42 JUMP_BACKWARD           18 (to 8)
                        >>   44 RETURN_VALUE
                consts
                names      ()
                varnames   ('.0', 'dn')
                freevars   ('_link_not_in_scm', 'force_all_files')
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder.py'
                name       '<listcomp>'
                firstlineno 61
                lnotab 0x0a0104ff020114ff020102ff
             ('n', 'str', 'return', 'bool')
          names      ('os', 'path', 'normcase', 'realpath', 'set', 'walk', 'islink', 'relpath', 'startswith', 'pardir', 'append', 'join', 'add')
          varnames   ('path', 'scm_files', 'scm_dirs', 'force_all_files', 'realpath', 'seen', 'res', 'dirpath', 'dirnames', 'filenames', 'filename', 'fullfilename', 'is_tracked')
          freevars   ()
          cellvars   ('scm_files', 'force_all_files', '_link_not_in_scm', 'realdirpath')
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder.py'
          name       'scm_find_files'
          firstlineno 13
          lnotab
             0x0a1578011c0104013a0278020e040c020e0102016a0104ff0e023afe02
             05a2010e01040108020e0104010a0102ff1c0308011a01020240017c0108
             01a4012e01
       'toplevel'
@@ -528,15 +528,15 @@
                       72 LOAD_METHOD              3 (split)
                       94 LOAD_GLOBAL              0 (os)
                      106 LOAD_ATTR                4 (pathsep)
                      116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (ignored)
          
-          82         132 LOAD_CONST               5 (<code object <listcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder.py", line 82>)
+          82         132 LOAD_CONST               5 (<code object <listcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder.py", line 82>)
                      134 MAKE_FUNCTION            0
                      136 LOAD_FAST                1 (ignored)
                      138 GET_ITER
                      140 PRECALL                  0
                      144 CALL                     0
                      154 STORE_FAST               1 (ignored)
          
@@ -581,30 +581,30 @@
                             72 JUMP_BACKWARD           34 (to 6)
                        >>   74 RETURN_VALUE
                consts
                names      ('os', 'path', 'normcase')
                varnames   ('.0', 'p')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder.py'
                name       '<listcomp>'
                firstlineno 82
                lnotab 0x
          names      ('os', 'environ', 'get', 'split', 'pathsep', 'trace')
          varnames   ('toplevel', 'ignored')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder.py'
          name       'is_toplevel_acceptable'
          firstlineno 76
          lnotab 0x0202040104027a0118022002
       (False,)
       ('path', '_t.PathT', 'scm_files', 'set[str]', 'scm_dirs', 'set[str]', 'force_all_files', 'bool', 'return', 'list[str]')
       ('toplevel', 'str | None', 'return', 'TypeGuard[str]')
    names      ('__future__', 'annotations', 'os', 'typing', 'TYPE_CHECKING', 'typing_extensions', 'TypeGuard', '', '_types', '_t', 'utils', 'trace', 'scm_find_files', 'is_toplevel_acceptable')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0208010c0204010c010c020c0702fc0a3f
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/file_finder_git.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 4287
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 4408
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 16777216
    code
       0x9700640064016c006d015a010100640064026c025a02640064026c035a
@@ -108,37 +108,37 @@
                150 LOAD_ATTR               19 (getLogger)
                160 LOAD_NAME               20 (__name__)
                162 PRECALL                  1
                166 CALL                     1
                176 STORE_NAME              21 (log)
    
     23         178 LOAD_CONST              28 (('path', 'str', 'return', 'str | None'))
-               180 LOAD_CONST              16 (<code object _git_toplevel, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder_git.py", line 23>)
+               180 LOAD_CONST              16 (<code object _git_toplevel, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder_git.py", line 23>)
                182 MAKE_FUNCTION            4 (annotations)
                184 STORE_NAME              22 (_git_toplevel)
    
     60         186 LOAD_CONST              29 (('fd', 'IO[bytes]', 'toplevel', 'str', 'return', 'tuple[set[str], set[str]]'))
-               188 LOAD_CONST              21 (<code object _git_interpret_archive, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder_git.py", line 60>)
+               188 LOAD_CONST              21 (<code object _git_interpret_archive, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder_git.py", line 60>)
                190 MAKE_FUNCTION            4 (annotations)
                192 STORE_NAME              23 (_git_interpret_archive)
    
     73         194 LOAD_CONST              30 (('toplevel', 'str', 'return', 'tuple[set[str], set[str]]'))
-               196 LOAD_CONST              22 (<code object _git_ls_files_and_dirs, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder_git.py", line 73>)
+               196 LOAD_CONST              22 (<code object _git_ls_files_and_dirs, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder_git.py", line 73>)
                198 MAKE_FUNCTION            4 (annotations)
                200 STORE_NAME              24 (_git_ls_files_and_dirs)
    
     95         202 LOAD_CONST              31 (('',))
                204 LOAD_CONST              32 (('path', '_t.PathT', 'return', 'list[str]'))
-               206 LOAD_CONST              26 (<code object git_find_files, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder_git.py", line 95>)
+               206 LOAD_CONST              26 (<code object git_find_files, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder_git.py", line 95>)
                208 MAKE_FUNCTION            5 (defaults, annotations)
                210 STORE_NAME              25 (git_find_files)
    
    107         212 LOAD_CONST              31 (('',))
                214 LOAD_CONST              32 (('path', '_t.PathT', 'return', 'list[str]'))
-               216 LOAD_CONST              27 (<code object git_archive_find_files, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder_git.py", line 107>)
+               216 LOAD_CONST              27 (<code object git_archive_find_files, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\file_finder_git.py", line 107>)
                218 MAKE_FUNCTION            5 (defaults, annotations)
                220 STORE_NAME              26 (git_archive_find_files)
                222 LOAD_CONST               2 (None)
                224 RETURN_VALUE
    consts
       0
       ('annotations',)
@@ -372,15 +372,15 @@
             'cwd='
             '\nout='
             'find files toplevel'
          names      ('os', 'path', 'abspath', 'do_ex', 'log', 'error', 'strip', 'replace', 'endswith', 'len', 'trace', 'normcase', 'realpath', 'subprocess', 'CalledProcessError', 'OSError')
          varnames   ('path', 'cwd', 'out', 'err', 'ret')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder_git.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder_git.py'
          name       '_git_toplevel'
          firstlineno 23
          lnotab
             0x0201020142012e010c02340104010c01060102fe1a040c010401380104
             0106067204300120019e011c020601120206fe
       'fd'
       'IO[bytes]'
@@ -510,15 +510,15 @@
             'r|*'
             ('fileobj', 'mode')
             '/'
          names      ('tarfile', 'open', 'set', 'getmembers', 'os', 'path', 'normcase', 'name', 'replace', 'sep', 'type', 'DIRTYPE', 'add')
          varnames   ('fd', 'toplevel', 'tf', 'git_files', 'git_dirs', 'member', 'name')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder_git.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder_git.py'
          name       '_git_interpret_archive'
          firstlineno 60
          lnotab 0x02012e011c0106012c018e012a012c022c0106f7
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
@@ -674,15 +674,15 @@
             ('stdout', 'cwd', 'stderr')
             0
             "listing git files failed - pretending there aren't any"
          names      ('os', 'path', 'sep', 'subprocess', 'Popen', 'PIPE', 'DEVNULL', 'stdout', '_git_interpret_archive', 'close', 'terminate', 'Exception', 'wait', 'log', 'error', 'set')
          varnames   ('toplevel', 'cmd', 'proc')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder_git.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder_git.py'
          name       '_git_ls_files_and_dirs'
          firstlineno 73
          lnotab
             0x02043201160130ff1203120102010201280332012cff32013201120130
             0134013cfd
       ''
       '_t.PathT'
@@ -778,15 +778,15 @@
          consts
             None
             'toplevel mismatch'
          names      ('_git_toplevel', 'os', 'fspath', 'is_toplevel_acceptable', 'path', 'abspath', 'normpath', 'startswith', 'trace', '_git_ls_files_and_dirs', 'scm_find_files')
          varnames   ('path', 'toplevel', 'fullpath', 'git_files', 'git_dirs')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder_git.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder_git.py'
          name       'git_find_files'
          firstlineno 95
          lnotab 0x020142011e010401080178012a0122012401
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
@@ -873,26 +873,26 @@
             'git archive detected - fallback to listing all files'
             True
             ('force_all_files',)
          names      ('os', 'path', 'join', 'exists', 'data_from_mime', 'get', 'trace', 'scm_find_files', 'set')
          varnames   ('path', 'archival', 'data')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder_git.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder_git.py'
          name       'git_archive_find_files'
          firstlineno 107
          lnotab 0x020340013e0104021e02300204021e01
       ('path', 'str', 'return', 'str | None')
       ('fd', 'IO[bytes]', 'toplevel', 'str', 'return', 'tuple[set[str], set[str]]')
       ('toplevel', 'str', 'return', 'tuple[set[str], set[str]]')
       ('',)
       ('path', '_t.PathT', 'return', 'list[str]')
    names      ('__future__', 'annotations', 'logging', 'os', 'subprocess', 'tarfile', 'typing', 'IO', 'TYPE_CHECKING', 'file_finder', 'is_toplevel_acceptable', 'scm_find_files', 'utils', 'data_from_mime', 'do_ex', 'trace', '', '_types', '_t', 'getLogger', '__name__', 'log', '_git_toplevel', '_git_interpret_archive', '_git_ls_files_and_dirs', 'git_find_files', 'git_archive_find_files')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder_git.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\file_finder_git.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c0208010801080108010c010c020c010c010c010c010c0204
       010c0320030825080d08160a0c
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/integration.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 3620
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 3747
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 16777216
    code
       0x9700640064016c006d015a010100640064026c025a02640064026c035a
@@ -125,42 +125,42 @@
                178 STORE_NAME              24 (_t)
                180 POP_TOP
    
     26     >>  182 LOAD_NAME                9 (setuptools)
                184 LOAD_ATTR               25 (__version__)
                194 BUILD_TUPLE              1
                196 LOAD_CONST              35 (('_version', 'str', 'return', 'None'))
-               198 LOAD_CONST              19 (<code object _warn_on_old_setuptools, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\integration.py", line 26>)
+               198 LOAD_CONST              19 (<code object _warn_on_old_setuptools, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\integration.py", line 26>)
                200 MAKE_FUNCTION            5 (defaults, annotations)
                202 STORE_NAME              26 (_warn_on_old_setuptools)
    
     56         204 PUSH_NULL
                206 LOAD_NAME               26 (_warn_on_old_setuptools)
                208 PRECALL                  0
                212 CALL                     0
                222 POP_TOP
    
     59         224 LOAD_CONST              36 (('dist', 'setuptools.Distribution', 'config', 'Configuration', 'return', 'None'))
-               226 LOAD_CONST              24 (<code object _assign_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\integration.py", line 59>)
+               226 LOAD_CONST              24 (<code object _assign_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\integration.py", line 59>)
                228 MAKE_FUNCTION            4 (annotations)
                230 STORE_NAME              27 (_assign_version)
    
     68         232 LOAD_CONST              37 (('dist', 'setuptools.Distribution', 'keyword', 'str', 'value', 'bool | dict[str, Any] | Callable[[], dict[str, Any]]', 'return', 'None'))
-               234 LOAD_CONST              28 (<code object version_keyword, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\integration.py", line 68>)
+               234 LOAD_CONST              28 (<code object version_keyword, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\integration.py", line 68>)
                236 MAKE_FUNCTION            4 (annotations)
                238 STORE_NAME              28 (version_keyword)
    
     94         240 LOAD_CONST              38 (('',))
                242 LOAD_CONST              39 (('path', '_t.PathT', 'return', 'list[str]'))
-               244 LOAD_CONST              33 (<code object find_files, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\integration.py", line 94>)
+               244 LOAD_CONST              33 (<code object find_files, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\integration.py", line 94>)
                246 MAKE_FUNCTION            5 (defaults, annotations)
                248 STORE_NAME              29 (find_files)
    
    110         250 LOAD_CONST              40 (('dist', 'setuptools.Distribution', 'return', 'None'))
-               252 LOAD_CONST              34 (<code object infer_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\integration.py", line 110>)
+               252 LOAD_CONST              34 (<code object infer_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\integration.py", line 110>)
                254 MAKE_FUNCTION            4 (annotations)
                256 STORE_NAME              30 (infer_version)
                258 LOAD_CONST               2 (None)
                260 RETURN_VALUE
    consts
       0
       ('annotations',)
@@ -240,15 +240,15 @@
             45
             '\nERROR: setuptools=='
             ' is used in combination with setuptools_scm>=6.x\n\nYour build configuration is incomplete and previously worked by accident!\nsetuptools_scm requires setuptools>=45\n\n\nThis happens as setuptools is unable to replace itself when a activated build dependency\nrequires a more recent setuptools version\n(it does not respect "setuptools>X" in setup_requires).\n\n\nsetuptools>=31 is required for setup.cfg metadata support\nsetuptools>=42 is required for pyproject.toml configuration support\n\nSuggested workarounds if applicable:\n - preinstalling build dependencies like setuptools_scm before running setup.py\n - installing setuptools_scm using the system package manager to ensure consistency\n - migrating from the deprecated setup_requires mechanism to pep517/518\n   and using a pyproject.toml to declare build dependencies\n   which are reliably pre-installed before running the build tools\n'
          names      ('int', 'split', 'warnings', 'warn', 'RuntimeWarning')
          varnames   ('_version',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\integration.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\integration.py'
          name       '_warn_on_old_setuptools'
          firstlineno 26
          lnotab 0x0201580116010c01020102ff06ff0eff14ff
       'dist'
       'setuptools.Distribution'
       'config'
       'Configuration'
@@ -289,15 +289,15 @@
                       96 RETURN_VALUE
          consts
             None
          names      ('_get_version', '_version_missing', 'metadata', 'version')
          varnames   ('dist', 'config', 'maybe_version')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\integration.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\integration.py'
          name       '_assign_version'
          firstlineno 59
          lnotab 0x02011e0204012202
       'keyword'
       'value'
       'bool | dict[str, Any] | Callable[[], dict[str, Any]]'
       code
@@ -409,15 +409,15 @@
             'dist_name may not be specified in the setup keyword '
             'version keyword'
             ()
          names      ('callable', 'trace', 'vars', 'metadata', 'name', '_read_dist_name_from_setup_cfg', 'Configuration', '_assign_version')
          varnames   ('dist', 'keyword', 'value', 'dist_name', 'config')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\integration.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\integration.py'
          name       'version_keyword'
          firstlineno 68
          lnotab
             0x020504010401080106011e0114020a0102ff10030c01020126fe100418
             0104011c011c01
       ''
       'path'
@@ -515,15 +515,15 @@
             'setuptools_scm.files_command'
             'setuptools_scm.files_command_fallback'
             '.'
          names      ('itertools', 'chain', 'iter_entry_points', 'load', 'isinstance', 'str', 'do', 'splitlines')
          varnames   ('path', 'ep', 'command', 'res')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\integration.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\integration.py'
          name       'find_files'
          firstlineno 94
          lnotab 0x020116011c011cfe140428012a026e021601040108ff0202
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
@@ -646,15 +646,15 @@
             'pyproject.toml'
             'setuptools_scm'
             ('dist_name',)
          names      ('trace', 'vars', 'metadata', 'name', '_read_dist_name_from_setup_cfg', 'os', 'path', 'isfile', 'Configuration', 'from_file', '_assign_version', 'LookupError')
          varnames   ('dist', 'dist_name', 'config', 'e')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\integration.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\integration.py'
          name       'infer_version'
          firstlineno 110
          lnotab
             0x02010c01020126fe1004180104011c013e0104010c01040102012a0426
             fd120132ff
       ('_version', 'str', 'return', 'None')
       ('dist', 'setuptools.Distribution', 'config', 'Configuration', 'return', 'None')
@@ -662,13 +662,13 @@
       ('',)
       ('path', '_t.PathT', 'return', 'list[str]')
       ('dist', 'setuptools.Distribution', 'return', 'None')
    names      ('__future__', 'annotations', 'itertools', 'os', 'warnings', 'typing', 'Any', 'Callable', 'TYPE_CHECKING', 'setuptools', '', '_get_version', '_version_missing', '_entrypoints', 'iter_entry_points', '_integration.setuptools', 'read_dist_name_from_setup_cfg', '_read_dist_name_from_setup_cfg', 'config', 'Configuration', 'utils', 'do', 'trace', '_types', '_t', '__version__', '_warn_on_old_setuptools', '_assign_version', 'version_keyword', 'find_files', 'infer_version')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\integration.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\integration.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c020801080108010c010c010c0208020c010c010c010c030c
       010c010c0204010c03161e14030809081a0a10
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/utils.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 5117
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 5297
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 16777216
    code
       0x970064005a00640164026c016d025a020100640164036c035a03640164
@@ -139,88 +139,88 @@
                250 CALL                     0
                260 LOAD_CONST              13 ('Windows')
                262 COMPARE_OP               2 (==)
                268 STORE_NAME              26 (IS_WINDOWS)
    
     28         270 PUSH_NULL
                272 LOAD_BUILD_CLASS
-               274 LOAD_CONST              14 (<code object _CmdResult, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 28>)
+               274 LOAD_CONST              14 (<code object _CmdResult, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 28>)
                276 MAKE_FUNCTION            0
                278 LOAD_CONST              15 ('_CmdResult')
                280 LOAD_NAME               16 (NamedTuple)
                282 PRECALL                  3
                286 CALL                     3
                296 STORE_NAME              27 (_CmdResult)
    
     34         298 LOAD_CONST              62 (('env', 'Mapping[str, str]', 'return', 'dict[str, str]'))
-               300 LOAD_CONST              20 (<code object no_git_env, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 34>)
+               300 LOAD_CONST              20 (<code object no_git_env, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 34>)
                302 MAKE_FUNCTION            4 (annotations)
                304 STORE_NAME              28 (no_git_env)
    
     55         306 LOAD_CONST              62 (('env', 'Mapping[str, str]', 'return', 'dict[str, str]'))
-               308 LOAD_CONST              21 (<code object avoid_pip_isolation, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 55>)
+               308 LOAD_CONST              21 (<code object avoid_pip_isolation, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 55>)
                310 MAKE_FUNCTION            4 (annotations)
                312 STORE_NAME              29 (avoid_pip_isolation)
    
     76         314 LOAD_CONST              22 (False)
                316 LOAD_CONST              23 (('indent',))
                318 BUILD_CONST_KEY_MAP      1
                320 LOAD_CONST              63 (('k', 'object', 'indent', 'bool', 'return', 'None'))
-               322 LOAD_CONST              29 (<code object trace, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 76>)
+               322 LOAD_CONST              29 (<code object trace, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 76>)
                324 MAKE_FUNCTION            6 (kwdefaults, annotations)
                326 STORE_NAME              30 (trace)
    
     83         328 LOAD_CONST              64 (('str_or_bytes', 'str | bytes', 'return', 'str'))
-               330 LOAD_CONST              33 (<code object ensure_stripped_str, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 83>)
+               330 LOAD_CONST              33 (<code object ensure_stripped_str, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 83>)
                332 MAKE_FUNCTION            4 (annotations)
                334 STORE_NAME              31 (ensure_stripped_str)
    
     90         336 LOAD_CONST              65 (('cmd', '_t.CMD_TYPE', 'cwd', '_t.PathT', 'return', 'subprocess.CompletedProcess[str]'))
-               338 LOAD_CONST              39 (<code object _run, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 90>)
+               338 LOAD_CONST              39 (<code object _run, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 90>)
                340 MAKE_FUNCTION            4 (annotations)
                342 STORE_NAME              32 (_run)
    
    107         344 LOAD_CONST              66 (('.',))
                346 LOAD_CONST              67 (('cmd', '_t.CMD_TYPE', 'cwd', '_t.PathT', 'return', '_CmdResult'))
-               348 LOAD_CONST              41 (<code object do_ex, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 107>)
+               348 LOAD_CONST              41 (<code object do_ex, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 107>)
                350 MAKE_FUNCTION            5 (defaults, annotations)
                352 STORE_NAME              33 (do_ex)
    
    132         354 LOAD_CONST              66 (('.',))
                356 LOAD_CONST              68 (('cmd', 'list[str] | str', 'cwd', 'str | _t.PathT', 'return', 'str'))
-               358 LOAD_CONST              44 (<code object do, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 132>)
+               358 LOAD_CONST              44 (<code object do, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 132>)
                360 MAKE_FUNCTION            5 (defaults, annotations)
                362 STORE_NAME              34 (do)
    
    139         364 LOAD_CONST              69 (('path', '_t.PathT', 'return', 'dict[str, str]'))
-               366 LOAD_CONST              46 (<code object data_from_mime, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 139>)
+               366 LOAD_CONST              46 (<code object data_from_mime, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 139>)
                368 MAKE_FUNCTION            4 (annotations)
                370 STORE_NAME              35 (data_from_mime)
    
    149         372 LOAD_CONST              70 (('fn', 'object | FunctionType', 'argname', 'str', 'return', 'bool'))
-               374 LOAD_CONST              50 (<code object function_has_arg, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 149>)
+               374 LOAD_CONST              50 (<code object function_has_arg, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 149>)
                376 MAKE_FUNCTION            4 (annotations)
                378 STORE_NAME              36 (function_has_arg)
    
    155         380 LOAD_CONST              71 ((None, True))
                382 LOAD_CONST              72 (('name', 'str', 'args', 'list[str] | None', 'warn', 'bool', 'return', 'bool'))
-               384 LOAD_CONST              56 (<code object has_command, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 155>)
+               384 LOAD_CONST              56 (<code object has_command, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 155>)
                386 MAKE_FUNCTION            5 (defaults, annotations)
                388 STORE_NAME              37 (has_command)
    
    169         390 LOAD_CONST              73 (('name', 'str', 'return', 'None'))
-               392 LOAD_CONST              57 (<code object require_command, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 169>)
+               392 LOAD_CONST              57 (<code object require_command, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 169>)
                394 MAKE_FUNCTION            4 (annotations)
                396 STORE_NAME              38 (require_command)
    
    175         398 NOP
    
    174         400 LOAD_CONST              74 ((None,))
                402 LOAD_CONST              75 (('group', 'str', 'name', 'str | None', 'return', 'Iterator[_t.EntrypointProtocol]'))
-               404 LOAD_CONST              61 (<code object iter_entry_points, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 174>)
+               404 LOAD_CONST              61 (<code object iter_entry_points, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 174>)
                406 MAKE_FUNCTION            5 (defaults, annotations)
                408 STORE_NAME              39 (iter_entry_points)
                410 LOAD_CONST               3 (None)
                412 RETURN_VALUE
    consts
       '\nutils\n'
       0
@@ -275,15 +275,15 @@
             'int'
             'returncode'
             None
          names      ('__name__', '__module__', '__qualname__', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       '_CmdResult'
          firstlineno 28
          lnotab 0x0c010a010a01
       '_CmdResult'
       'env'
       'Mapping[str, str]'
       'return'
@@ -324,15 +324,15 @@
                      106 LOAD_FAST                1 (k)
                      108 LOAD_FAST                2 (v)
                      110 PRECALL                  2
                      114 CALL                     2
                      124 POP_TOP
                  >>  126 JUMP_BACKWARD           43 (to 42)
          
-          47     >>  128 LOAD_CONST               2 (<code object <dictcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 47>)
+          47     >>  128 LOAD_CONST               2 (<code object <dictcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 47>)
                      130 MAKE_FUNCTION            0
          
           49         132 LOAD_FAST                0 (env)
                      134 LOAD_METHOD              0 (items)
                      156 PRECALL                  0
                      160 CALL                     0
          
@@ -383,23 +383,23 @@
                consts
                   'GIT_'
                   ('GIT_EXEC_PATH', 'GIT_SSH', 'GIT_SSH_COMMAND')
                names      ('startswith',)
                varnames   ('.0', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
                name       '<dictcomp>'
                firstlineno 47
                lnotab 0x0802080128fd020408fd0403
          names      ('items', 'startswith', 'trace')
          varnames   ('env', 'k', 'v')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       'no_git_env'
          firstlineno 34
          lnotab 0x020a32012a012201040226fe
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
@@ -411,15 +411,15 @@
             00000000000000a003000000000000000000000000000000000000000064
             0384007c01640219000000000000000000a0040000000000000000000000
             0000000000000000007402000000000000000000006a0200000000000000
             00a6010000ab0100000000000000004400a6000000ab0000000000000000
             00a6010000ab0100000000000000007c0164023c0000007c015300
           55           0 RESUME                   0
          
-          62           2 LOAD_CONST               1 (<code object <dictcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 62>)
+          62           2 LOAD_CONST               1 (<code object <dictcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 62>)
                        4 MAKE_FUNCTION            0
                        6 LOAD_FAST                0 (env)
                        8 LOAD_METHOD              0 (items)
                       30 PRECALL                  0
                       34 CALL                     0
                       44 GET_ITER
                       46 PRECALL                  0
@@ -434,15 +434,15 @@
           64          70 LOAD_FAST                1 (new_env)
                       72 RETURN_VALUE
          
           66     >>   74 LOAD_GLOBAL              2 (os)
                       86 LOAD_ATTR                2 (pathsep)
                       96 LOAD_METHOD              3 (join)
          
-          67         118 LOAD_CONST               3 (<code object <listcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 67>)
+          67         118 LOAD_CONST               3 (<code object <listcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 67>)
                      120 MAKE_FUNCTION            0
          
           69         122 LOAD_FAST                1 (new_env)
                      124 LOAD_CONST               2 ('PYTHONPATH')
                      126 BINARY_SUBSCR
                      136 LOAD_METHOD              4 (split)
                      158 LOAD_GLOBAL              2 (os)
@@ -490,15 +490,15 @@
                        >>   36 RETURN_VALUE
                consts
                   'PYTHONNOUSERSITE'
                names      ()
                varnames   ('.0', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
                name       '<dictcomp>'
                firstlineno 62
                lnotab 0x
             'PYTHONPATH'
             code
                argcount  : 1
                nlocals   : 2
@@ -524,23 +524,23 @@
                        >>   24 RETURN_VALUE
                consts
                   'pip-build-env-'
                names      ()
                varnames   ('.0', 'path')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
                name       '<listcomp>'
                firstlineno 67
                lnotab 0x0802020108fe0202
          names      ('items', 'os', 'pathsep', 'join', 'split')
          varnames   ('env', 'new_env')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       'avoid_pip_isolation'
          firstlineno 55
          lnotab 0x02073c01080104022c01040248fe10ff1607
       False
       ('indent',)
       'k'
       'object'
@@ -576,15 +576,15 @@
                       56 POP_JUMP_FORWARD_IF_FALSE    43 (to 144)
          
           79          58 LOAD_FAST                1 (k)
                       60 LOAD_CONST               2 (0)
                       62 BINARY_SUBSCR
                       72 BUILD_TUPLE              1
                       74 LOAD_GLOBAL              5 (NULL + tuple)
-                      86 LOAD_CONST               3 (<code object <genexpr>, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 79>)
+                      86 LOAD_CONST               3 (<code object <genexpr>, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 79>)
                       88 MAKE_FUNCTION            0
                       90 LOAD_FAST                1 (k)
                       92 LOAD_CONST               1 (1)
                       94 LOAD_CONST               0 (None)
                       96 BUILD_SLICE              2
                       98 BINARY_SUBSCR
                      108 GET_ITER
@@ -647,25 +647,25 @@
                consts
                   '    '
                   None
                names      ('textwrap', 'indent', 'str')
                varnames   ('.0', 's')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
                name       '<genexpr>'
                firstlineno 79
                lnotab 0x
             True
             ('file', 'flush')
          names      ('DEBUG', 'len', 'tuple', 'print', 'sys', 'stderr')
          varnames   ('indent', 'k')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       'trace'
          firstlineno 76
          lnotab 0x02010e012a01560132fd
       'str_or_bytes'
       'str | bytes'
       'str'
       code
@@ -709,15 +709,15 @@
             None
             'utf-8'
             'surrogateescape'
          names      ('isinstance', 'str', 'strip', 'decode')
          varnames   ('str_or_bytes',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       'ensure_stripped_str'
          firstlineno 83
          lnotab 0x02012a012802
       'cmd'
       '_t.CMD_TYPE'
       'cwd'
       '_t.PathT'
@@ -784,15 +784,15 @@
             '1'
             ('LC_ALL', 'LANGUAGE', 'HGPLAIN')
             ('capture_output', 'cwd', 'env', 'text')
          names      ('subprocess', 'run', 'str', 'dict', 'avoid_pip_isolation', 'no_git_env', 'os', 'environ')
          varnames   ('cmd', 'cwd')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       '_run'
          firstlineno 90
          lnotab 0x02011601020102011c010c014a030201020102fa100802f4
       '.'
       code
          argcount  : 2
          nlocals   : 4
@@ -835,15 +835,15 @@
          109     >>   58 LOAD_FAST                0 (cmd)
                       60 STORE_FAST               2 (cmd_4_trace)
                       62 JUMP_FORWARD            31 (to 126)
          
          112     >>   64 LOAD_CONST               1 (' ')
                       66 LOAD_METHOD              3 (join)
          
-         113          88 LOAD_CONST               2 (<code object <listcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 113>)
+         113          88 LOAD_CONST               2 (<code object <listcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 113>)
                       90 MAKE_FUNCTION            0
                       92 LOAD_FAST                0 (cmd)
                       94 GET_ITER
                       96 PRECALL                  0
                      100 CALL                     0
          
          112         110 PRECALL                  1
@@ -970,15 +970,15 @@
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                37 (to 84)
                             10 STORE_DEREF              1 (s)
                             12 LOAD_GLOBAL              1 (NULL + all)
                             24 LOAD_CLOSURE             1 (s)
                             26 BUILD_TUPLE              1
-                            28 LOAD_CONST               0 (<code object <genexpr>, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 113>)
+                            28 LOAD_CONST               0 (<code object <genexpr>, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 113>)
                             30 MAKE_FUNCTION            8 (closure)
                             32 LOAD_CONST               1 (' {[:')
                             34 GET_ITER
                             36 PRECALL                  0
                             40 CALL                     0
                             50 PRECALL                  1
                             54 CALL                     1
@@ -1021,25 +1021,25 @@
                                   30 RETURN_VALUE
                      consts
                         None
                      names      ()
                      varnames   ('.0', 'c')
                      freevars   ('s',)
                      cellvars   ()
-                     filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+                     filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
                      name       '<genexpr>'
                      firstlineno 113
                      lnotab 0x
                   ' {[:'
                   '"'
                names      ('all',)
                varnames   ('.0',)
                freevars   ()
                cellvars   ('s',)
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
                name       '<listcomp>'
                firstlineno 113
                lnotab 0x
             '----\ncmd:\n'
             True
             ('indent',)
             ' in:'
@@ -1047,15 +1047,15 @@
             'out:\n'
             'err:\n'
             'ret:'
          names      ('DEBUG', 'isinstance', 'list', 'join', 'trace', 'os', 'name', 'tuple', 'shlex', 'split', '_run', 'stdout', 'stderr', 'returncode', '_CmdResult', 'ensure_stripped_str')
          varnames   ('cmd', 'cwd', 'cmd_4_trace', 'res')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       'do_ex'
          firstlineno 107
          lnotab
             0x020138010603180116ff1003240120015801280220010e012e010e012e
             010e012a010c0158ff
       'list[str] | str'
       'str | _t.PathT'
@@ -1096,15 +1096,15 @@
                       92 RETURN_VALUE
          consts
             None
          names      ('do_ex', 'DEBUG', 'print')
          varnames   ('cmd', 'cwd', 'out', 'err', 'ret')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       'do'
          firstlineno 132
          lnotab 0x0201280112011e01
       'path'
       code
          argcount  : 1
          nlocals   : 4
@@ -1165,15 +1165,15 @@
                      152 PRECALL                  1
                      156 CALL                     1
                      166 PRECALL                  2
                      170 CALL                     2
                      180 POP_TOP
          
          144         182 LOAD_GLOBAL              9 (NULL + dict)
-                     194 LOAD_CONST               4 (<code object <genexpr>, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 144>)
+                     194 LOAD_CONST               4 (<code object <genexpr>, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\utils.py", line 144>)
                      196 MAKE_FUNCTION            0
                      198 LOAD_FAST                2 (content)
                      200 LOAD_METHOD              5 (splitlines)
                      222 PRECALL                  0
                      226 CALL                     0
                      236 GET_ITER
                      238 PRECALL                  0
@@ -1235,24 +1235,24 @@
                   ': '
                   1
                   None
                names      ('split',)
                varnames   ('.0', 'x')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
                name       '<genexpr>'
                firstlineno 144
                lnotab 0x
             'data'
          names      ('open', 'read', 'trace', 'repr', 'dict', 'splitlines')
          varnames   ('path', 'fp', 'content', 'data')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       'data_from_mime'
          firstlineno 139
          lnotab 0x0201240128ff2e023a0256012001
       'fn'
       'object | FunctionType'
       'argname'
       code
@@ -1286,15 +1286,15 @@
                       78 RETURN_VALUE
          consts
             None
          names      ('isinstance', 'FunctionType', '__code__', 'co_varnames')
          varnames   ('fn', 'argname', 'code')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       'function_has_arg'
          firstlineno 149
          lnotab 0x02012e010e01
       True
       'name'
       'args'
       'list[str] | None'
@@ -1395,15 +1395,15 @@
             False
             '%r was not found'
             ('category',)
          names      ('_run', 'returncode', 'OSError', 'trace', 'sys', 'exc_info', 'warnings', 'warn', 'RuntimeWarning')
          varnames   ('name', 'args', 'warn', 'cmd', 'p', 'res')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       'has_command'
          firstlineno 155
          lnotab 0x020102011601200514fc1201340108fe080508013c01
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -1437,15 +1437,15 @@
             False
             ('warn',)
             '%r was not found'
          names      ('has_command', 'OSError')
          varnames   ('name',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       'require_command'
          firstlineno 169
          lnotab 0x0201220124ff
       'group'
       'str | None'
       'Iterator[_t.EntrypointProtocol]'
       code
@@ -1476,15 +1476,15 @@
             None
             1
             ('iter_entry_points',)
          names      ('_entrypoints', 'iter_entry_points')
          varnames   ('group', 'name', 'iter_entry_points')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
          name       'iter_entry_points'
          firstlineno 174
          lnotab 0x02040c02
       ('env', 'Mapping[str, str]', 'return', 'dict[str, str]')
       ('k', 'object', 'indent', 'bool', 'return', 'None')
       ('str_or_bytes', 'str | bytes', 'return', 'str')
       ('cmd', '_t.CMD_TYPE', 'cwd', '_t.PathT', 'return', 'subprocess.CompletedProcess[str]')
@@ -1498,14 +1498,14 @@
       ('name', 'str', 'return', 'None')
       (None,)
       ('group', 'str', 'name', 'str | None', 'return', 'Iterator[_t.EntrypointProtocol]')
    names      ('__doc__', '__future__', 'annotations', 'os', 'platform', 'shlex', 'subprocess', 'sys', 'textwrap', 'warnings', 'types', 'CodeType', 'FunctionType', 'typing', 'Iterator', 'Mapping', 'NamedTuple', 'TYPE_CHECKING', '', '_types', '_t', 'bool', 'environ', 'get', 'DEBUG', 'system', 'IS_WINDOWS', '_CmdResult', 'no_git_env', 'avoid_pip_isolation', 'trace', 'ensure_stripped_str', '_run', 'do_ex', 'do', 'data_from_mime', 'function_has_arg', 'has_command', 'require_command', 'iter_entry_points')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\utils.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020104030c0208010801080108010801080108010c010c010c010c
       010c010c0204020c02460126031c06081508150e07080708110a190a0708
       0a08060a0e080602ff
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/__pycache__/version.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 17034
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 17597
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 16777216
    code
       0x9700640064016c006d015a010100640064026c025a02640064026c035a
@@ -188,50 +188,50 @@
     30         262 LOAD_CONST              23 (3)
                264 STORE_NAME              32 (SEMVER_PATCH)
    
     31         266 LOAD_CONST              23 (3)
                268 STORE_NAME              33 (SEMVER_LEN)
    
     34         270 LOAD_CONST             117 (('tag', 'str | object', 'config', 'Configuration', 'return', 'dict[str, str] | None'))
-               272 LOAD_CONST              30 (<code object _parse_version_tag, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 34>)
+               272 LOAD_CONST              30 (<code object _parse_version_tag, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 34>)
                274 MAKE_FUNCTION            4 (annotations)
                276 STORE_NAME              34 (_parse_version_tag)
    
     58         278 LOAD_CONST             118 (('group', 'str', 'callable_or_name', 'str | Any', 'return', 'Any'))
-               280 LOAD_CONST              36 (<code object callable_or_entrypoint, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 58>)
+               280 LOAD_CONST              36 (<code object callable_or_entrypoint, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 58>)
                282 MAKE_FUNCTION            4 (annotations)
                284 STORE_NAME              35 (callable_or_entrypoint)
    
     71         286 NOP
    
     70         288 LOAD_CONST             119 ((None,))
                290 LOAD_CONST             120 (('tag', '_VersionT | str', 'config', 'Configuration | None', 'return', '_VersionT | None'))
-               292 LOAD_CONST              40 (<code object tag_to_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 70>)
+               292 LOAD_CONST              40 (<code object tag_to_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 70>)
                294 MAKE_FUNCTION            5 (defaults, annotations)
                296 STORE_NAME              36 (tag_to_version)
    
    104         298 NOP
    
    103         300 LOAD_CONST             119 ((None,))
                302 LOAD_CONST             121 (('tags', 'list[str]', 'config', 'Configuration | None', 'return', 'list[_VersionT]'))
-               304 LOAD_CONST              44 (<code object tags_to_versions, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 103>)
+               304 LOAD_CONST              44 (<code object tags_to_versions, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 103>)
                306 MAKE_FUNCTION            5 (defaults, annotations)
                308 STORE_NAME              37 (tags_to_versions)
    
    119         310 PUSH_NULL
                312 LOAD_BUILD_CLASS
-               314 LOAD_CONST              45 (<code object ScmVersion, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 119>)
+               314 LOAD_CONST              45 (<code object ScmVersion, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 119>)
                316 MAKE_FUNCTION            0
                318 LOAD_CONST              46 ('ScmVersion')
                320 PRECALL                  2
                324 CALL                     2
                334 STORE_NAME              38 (ScmVersion)
    
    196         336 LOAD_CONST             122 (('tag', '_VersionT | str', 'preformatted', 'bool', 'config', 'Configuration | None', 'return', '_VersionT | str'))
-               338 LOAD_CONST              49 (<code object _parse_tag, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 196>)
+               338 LOAD_CONST              49 (<code object _parse_tag, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 196>)
                340 MAKE_FUNCTION            4 (annotations)
                342 STORE_NAME              39 (_parse_tag)
    
    211         344 NOP
    
    212         346 NOP
    
@@ -243,176 +243,176 @@
    
    216         354 NOP
    
    217         356 NOP
    
    209         358 LOAD_CONST             123 ((None, False, None, False, None, None, None))
                360 LOAD_CONST             124 (('tag', 'str | _VersionT', 'distance', 'int | None', 'dirty', 'bool', 'node', 'str | None', 'preformatted', 'bool', 'branch', 'str | None', 'config', 'Configuration | None', 'node_date', 'date | None', 'kw', 'Any', 'return', 'ScmVersion'))
-               362 LOAD_CONST              61 (<code object meta, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 209>)
+               362 LOAD_CONST              61 (<code object meta, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 209>)
                364 MAKE_FUNCTION            5 (defaults, annotations)
                366 STORE_NAME              40 (meta)
    
    242         368 LOAD_CONST             125 (('tag_version', 'ScmVersion', 'return', 'str'))
-               370 LOAD_CONST              63 (<code object guess_next_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 242>)
+               370 LOAD_CONST              63 (<code object guess_next_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 242>)
                372 MAKE_FUNCTION            4 (annotations)
                374 STORE_NAME              41 (guess_next_version)
    
    247         376 LOAD_CONST             125 (('tag_version', 'ScmVersion', 'return', 'str'))
-               378 LOAD_CONST              64 (<code object _dont_guess_next_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 247>)
+               378 LOAD_CONST              64 (<code object _dont_guess_next_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 247>)
                380 MAKE_FUNCTION            4 (annotations)
                382 STORE_NAME              42 (_dont_guess_next_version)
    
    252         384 LOAD_CONST             126 (('version_string', 'str', 'return', 'str'))
-               386 LOAD_CONST              66 (<code object _strip_local, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 252>)
+               386 LOAD_CONST              66 (<code object _strip_local, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 252>)
                388 MAKE_FUNCTION            4 (annotations)
                390 STORE_NAME              43 (_strip_local)
    
    257         392 LOAD_CONST             127 (('version', 'str', 'return', 'str'))
-               394 LOAD_CONST              68 (<code object _add_post, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 257>)
+               394 LOAD_CONST              68 (<code object _add_post, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 257>)
                396 MAKE_FUNCTION            4 (annotations)
                398 STORE_NAME              44 (_add_post)
    
    265         400 LOAD_CONST             128 (('version', 'str', 'return', 'str | None'))
-               402 LOAD_CONST              69 (<code object _bump_dev, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 265>)
+               402 LOAD_CONST              69 (<code object _bump_dev, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 265>)
                404 MAKE_FUNCTION            4 (annotations)
                406 STORE_NAME              45 (_bump_dev)
    
    280         408 LOAD_CONST             127 (('version', 'str', 'return', 'str'))
-               410 LOAD_CONST              70 (<code object _bump_regex, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 280>)
+               410 LOAD_CONST              70 (<code object _bump_regex, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 280>)
                412 MAKE_FUNCTION            4 (annotations)
                414 STORE_NAME              46 (_bump_regex)
    
    292         416 LOAD_CONST             129 (('version', 'ScmVersion', 'return', 'str'))
-               418 LOAD_CONST              71 (<code object guess_next_dev_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 292>)
+               418 LOAD_CONST              71 (<code object guess_next_dev_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 292>)
                420 MAKE_FUNCTION            4 (annotations)
                422 STORE_NAME              47 (guess_next_dev_version)
    
    300         424 NOP
    
    299         426 LOAD_CONST             130 ((True,))
                428 LOAD_CONST             131 (('version', 'ScmVersion', 'retain', 'int', 'increment', 'bool', 'return', 'str'))
-               430 LOAD_CONST              76 (<code object guess_next_simple_semver, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 299>)
+               430 LOAD_CONST              76 (<code object guess_next_simple_semver, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 299>)
                432 MAKE_FUNCTION            5 (defaults, annotations)
                434 STORE_NAME              48 (guess_next_simple_semver)
    
    315         436 LOAD_CONST             129 (('version', 'ScmVersion', 'return', 'str'))
-               438 LOAD_CONST              77 (<code object simplified_semver_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 315>)
+               438 LOAD_CONST              77 (<code object simplified_semver_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 315>)
                440 MAKE_FUNCTION            4 (annotations)
                442 STORE_NAME              49 (simplified_semver_version)
    
    329         444 LOAD_CONST             129 (('version', 'ScmVersion', 'return', 'str'))
-               446 LOAD_CONST              78 (<code object release_branch_semver_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 329>)
+               446 LOAD_CONST              78 (<code object release_branch_semver_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 329>)
                448 MAKE_FUNCTION            4 (annotations)
                450 STORE_NAME              50 (release_branch_semver_version)
    
    354         452 LOAD_CONST             129 (('version', 'ScmVersion', 'return', 'str'))
-               454 LOAD_CONST              79 (<code object release_branch_semver, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 354>)
+               454 LOAD_CONST              79 (<code object release_branch_semver, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 354>)
                456 MAKE_FUNCTION            4 (annotations)
                458 STORE_NAME              51 (release_branch_semver)
    
    364         460 LOAD_CONST             129 (('version', 'ScmVersion', 'return', 'str'))
-               462 LOAD_CONST              80 (<code object no_guess_dev_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 364>)
+               462 LOAD_CONST              80 (<code object no_guess_dev_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 364>)
                464 MAKE_FUNCTION            4 (annotations)
                466 STORE_NAME              52 (no_guess_dev_version)
    
    371         468 LOAD_CONST             132 (('ver', 'str', 'return', 'Match[str] | None'))
-               470 LOAD_CONST              83 (<code object date_ver_match, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 371>)
+               470 LOAD_CONST              83 (<code object date_ver_match, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 371>)
                472 MAKE_FUNCTION            4 (annotations)
                474 STORE_NAME              53 (date_ver_match)
    
    384         476 NOP
    
    385         478 NOP
    
    386         480 NOP
    
    382         482 LOAD_CONST             133 ((None, None, None))
                484 LOAD_CONST             134 (('version', 'ScmVersion', 'node_date', 'date | None', 'date_fmt', 'str | None', 'version_cls', 'type | None', 'return', 'str'))
-               486 LOAD_CONST              87 (<code object guess_next_date_ver, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 382>)
+               486 LOAD_CONST              87 (<code object guess_next_date_ver, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 382>)
                488 MAKE_FUNCTION            5 (defaults, annotations)
                490 STORE_NAME              54 (guess_next_date_ver)
    
    435         492 LOAD_CONST             129 (('version', 'ScmVersion', 'return', 'str'))
-               494 LOAD_CONST              88 (<code object calver_by_date, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 435>)
+               494 LOAD_CONST              88 (<code object calver_by_date, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 435>)
                496 MAKE_FUNCTION            4 (annotations)
                498 STORE_NAME              55 (calver_by_date)
    
    453         500 LOAD_CONST             135 (('version', 'ScmVersion', 'time_format', 'str', 'return', 'str'))
-               502 LOAD_CONST              90 (<code object _format_local_with_time, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 453>)
+               502 LOAD_CONST              90 (<code object _format_local_with_time, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 453>)
                504 MAKE_FUNCTION            4 (annotations)
                506 STORE_NAME              56 (_format_local_with_time)
    
    465         508 LOAD_CONST             129 (('version', 'ScmVersion', 'return', 'str'))
-               510 LOAD_CONST              91 (<code object get_local_node_and_date, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 465>)
+               510 LOAD_CONST              91 (<code object get_local_node_and_date, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 465>)
                512 MAKE_FUNCTION            4 (annotations)
                514 STORE_NAME              57 (get_local_node_and_date)
    
    469         516 LOAD_CONST             136 (('%Y%m%d%H%M%S',))
                518 LOAD_CONST             137 (('version', 'ScmVersion', 'fmt', 'str', 'return', 'str'))
-               520 LOAD_CONST              94 (<code object get_local_node_and_timestamp, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 469>)
+               520 LOAD_CONST              94 (<code object get_local_node_and_timestamp, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 469>)
                522 MAKE_FUNCTION            5 (defaults, annotations)
                524 STORE_NAME              58 (get_local_node_and_timestamp)
    
    473         526 LOAD_CONST             129 (('version', 'ScmVersion', 'return', 'str'))
-               528 LOAD_CONST              95 (<code object get_local_dirty_tag, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 473>)
+               528 LOAD_CONST              95 (<code object get_local_dirty_tag, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 473>)
                530 MAKE_FUNCTION            4 (annotations)
                532 STORE_NAME              59 (get_local_dirty_tag)
    
    477         534 LOAD_CONST             138 (('_', 'Any', 'return', 'str'))
-               536 LOAD_CONST              97 (<code object get_no_local_node, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 477>)
+               536 LOAD_CONST              97 (<code object get_no_local_node, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 477>)
                538 MAKE_FUNCTION            4 (annotations)
                540 STORE_NAME              60 (get_no_local_node)
    
    481         542 LOAD_CONST             129 (('version', 'ScmVersion', 'return', 'str'))
-               544 LOAD_CONST              98 (<code object postrelease_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 481>)
+               544 LOAD_CONST              98 (<code object postrelease_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 481>)
                546 MAKE_FUNCTION            4 (annotations)
                548 STORE_NAME              61 (postrelease_version)
    
    488         550 LOAD_CONST             139 (('group', 'str', 'name', 'str', 'return', 'Any | None'))
-               552 LOAD_CONST             101 (<code object _get_ep, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 488>)
+               552 LOAD_CONST             101 (<code object _get_ep, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 488>)
                554 MAKE_FUNCTION            4 (annotations)
                556 STORE_NAME              62 (_get_ep)
    
    505         558 NOP
    
    498         560 LOAD_CONST             119 ((None,))
                562 LOAD_CONST             140 (('entrypoint', 'str', 'scheme_value', 'str | list[str] | tuple[str, ...] | Callable[[ScmVersion], str] | None', '_memo', 'set[object] | None', 'return', 'Iterator[Callable[[ScmVersion], str]]'))
-               564 LOAD_CONST             108 (<code object _iter_version_schemes, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 498>)
+               564 LOAD_CONST             108 (<code object _iter_version_schemes, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 498>)
                566 MAKE_FUNCTION            5 (defaults, annotations)
                568 STORE_NAME              63 (_iter_version_schemes)
    
    524         570 LOAD_NAME               15 (overload)
    
    525         572 LOAD_CONST             141 (('version', 'ScmVersion', 'entypoint', 'str', 'given_value', 'str', 'default', 'str', 'return', 'str'))
-               574 LOAD_CONST             112 (<code object _call_version_scheme, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 524>)
+               574 LOAD_CONST             112 (<code object _call_version_scheme, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 524>)
                576 MAKE_FUNCTION            4 (annotations)
    
    524         578 PRECALL                  0
                582 CALL                     0
    
    525         592 STORE_NAME              64 (_call_version_scheme)
    
    531         594 LOAD_NAME               15 (overload)
    
    532         596 LOAD_CONST             142 (('version', 'ScmVersion', 'entypoint', 'str', 'given_value', 'str', 'default', 'None', 'return', 'str | None'))
-               598 LOAD_CONST             114 (<code object _call_version_scheme, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 531>)
+               598 LOAD_CONST             114 (<code object _call_version_scheme, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 531>)
                600 MAKE_FUNCTION            4 (annotations)
    
    531         602 PRECALL                  0
                606 CALL                     0
    
    532         616 STORE_NAME              64 (_call_version_scheme)
    
    538         618 LOAD_CONST             143 (('version', 'ScmVersion', 'entypoint', 'str', 'given_value', 'str', 'default', 'str | None', 'return', 'str | None'))
-               620 LOAD_CONST             115 (<code object _call_version_scheme, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 538>)
+               620 LOAD_CONST             115 (<code object _call_version_scheme, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 538>)
                622 MAKE_FUNCTION            4 (annotations)
                624 STORE_NAME              64 (_call_version_scheme)
    
    548         626 LOAD_CONST             144 (('version', 'ScmVersion', 'config', 'Any', 'return', 'str'))
-               628 LOAD_CONST             116 (<code object format_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 548>)
+               628 LOAD_CONST             116 (<code object format_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 548>)
                630 MAKE_FUNCTION            4 (annotations)
                632 STORE_NAME              65 (format_version)
                634 LOAD_CONST               2 (None)
                636 RETURN_VALUE
    consts
       0
       ('annotations',)
@@ -575,15 +575,15 @@
             ('version', 'prefix', 'suffix')
             "tag '"
             "' parsed to "
          names      ('isinstance', 'str', 'tag_regex', 'match', 'len', 'groups', 'group', 'start', 'end', 'trace')
          varnames   ('tag', 'config', 'tagstring', 'match', 'result', 'key')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_parse_version_tag'
          firstlineno 34
          lnotab 0x02034c013402040104024a010602040328015e015efd06062a01
       'group'
       'str'
       'callable_or_name'
       'str | Any'
@@ -662,15 +662,15 @@
             1
             ('iter_entry_points',)
             'ep found:'
          names      ('trace', 'callable', '_entrypoints', 'iter_entry_points', 'name', 'load')
          varnames   ('group', 'callable_or_name', 'iter_entry_points', 'ep')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'callable_or_entrypoint'
          firstlineno 58
          lnotab 0x020124021e0104010c021c012a012cfe
       '_VersionT | str'
       'Configuration | None'
       '_VersionT | None'
       code
@@ -817,15 +817,15 @@
             'suffix'
             ''
             "tag {!r} will be stripped of its suffix '{}'"
          names      ('trace', 'Configuration', '_parse_version_tag', 'isinstance', 'dict', 'get', 'warnings', 'warn', 'format', 'version_cls', 'repr')
          varnames   ('tag', 'config', 'tagdict', 'version_str', 'version')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'tag_to_version'
          firstlineno 70
          lnotab
             0x0207200204011c022001560130010402100120022c011601180110ff0e
             ff10062a013a02
       'tags'
       'list[str]'
@@ -874,15 +874,15 @@
          consts
             '\n    take tags that might be prefixed with a keyword and return only the version part\n    :param tags: an iterable of tags\n    :param config: optional configuration object\n    '
             ('config',)
          names      ('tag_to_version', 'append')
          varnames   ('tags', 'config', 'result', 'tag', 'parsed')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'tags_to_versions'
          firstlineno 103
          lnotab 0x020804010801220104012c01
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
@@ -909,60 +909,60 @@
          
          128          18 NOP
          
          129          20 NOP
          
          120          22 LOAD_CONST              38 ((None, None, False, False, None, None))
                       24 LOAD_CONST              39 (('tag_version', 'Any', 'config', 'Configuration', 'distance', 'int | None', 'node', 'str | None', 'dirty', 'bool', 'preformatted', 'bool', 'branch', 'str | None', 'node_date', 'date | None', 'kw', 'object'))
-                      26 LOAD_CONST              19 (<code object __init__, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 120>)
+                      26 LOAD_CONST              19 (<code object __init__, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 120>)
                       28 MAKE_FUNCTION            5 (defaults, annotations)
                       30 STORE_NAME               3 (__init__)
          
          151          32 LOAD_NAME                4 (property)
          
          152          34 LOAD_CONST              40 (('return', 'dict[str, Any]'))
-                      36 LOAD_CONST              22 (<code object extra, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 151>)
+                      36 LOAD_CONST              22 (<code object extra, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 151>)
                       38 MAKE_FUNCTION            4 (annotations)
          
          151          40 PRECALL                  0
                       44 CALL                     0
          
          152          54 STORE_NAME               5 (extra)
          
          160          56 LOAD_NAME                4 (property)
          
          161          58 LOAD_CONST              41 (('return', 'bool'))
-                      60 LOAD_CONST              23 (<code object exact, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 160>)
+                      60 LOAD_CONST              23 (<code object exact, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 160>)
                       62 MAKE_FUNCTION            4 (annotations)
          
          160          64 PRECALL                  0
                       68 CALL                     0
          
          161          78 STORE_NAME               6 (exact)
          
          164          80 LOAD_CONST              42 (('return', 'str'))
-                      82 LOAD_CONST              25 (<code object __repr__, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 164>)
+                      82 LOAD_CONST              25 (<code object __repr__, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 164>)
                       84 MAKE_FUNCTION            4 (annotations)
                       86 STORE_NAME               7 (__repr__)
          
          170          88 LOAD_CONST              43 (('fmt', 'str', 'kw', 'object', 'return', 'str'))
-                      90 LOAD_CONST              27 (<code object format_with, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 170>)
+                      90 LOAD_CONST              27 (<code object format_with, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 170>)
                       92 MAKE_FUNCTION            4 (annotations)
                       94 STORE_NAME               8 (format_with)
          
          182          96 LOAD_CONST              44 (('clean_format', 'str', 'dirty_format', 'str', 'kw', 'object', 'return', 'str'))
-                      98 LOAD_CONST              30 (<code object format_choice, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 182>)
+                      98 LOAD_CONST              30 (<code object format_choice, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 182>)
                      100 MAKE_FUNCTION            4 (annotations)
                      102 STORE_NAME               9 (format_choice)
          
          188         104 NOP
          
          185         106 LOAD_CONST              45 (('{guessed}.dev{distance}',))
                      108 LOAD_CONST              46 (('guess_next', 'Callable[Concatenate[ScmVersion, _t.P], str]', 'fmt', 'str', 'k', '_t.P.args', 'kw', '_t.P.kwargs', 'return', 'str'))
-                     110 LOAD_CONST              37 (<code object format_next_version, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 185>)
+                     110 LOAD_CONST              37 (<code object format_next_version, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 185>)
                      112 MAKE_FUNCTION            5 (defaults, annotations)
                      114 STORE_NAME              10 (format_next_version)
                      116 LOAD_CONST               1 (None)
                      118 RETURN_VALUE
          consts
             'ScmVersion'
             None
@@ -1100,15 +1100,15 @@
                   'unknown args'
                   0
                   'SOURCE_DATE_EPOCH'
                names      ('trace', 'tag', 'distance', 'node', 'node_date', 'os', 'environ', 'int', 'datetime', 'fromtimestamp', 'timezone', 'utc', 'time', 'now', '_extra', 'dirty', 'preformatted', 'branch', 'config')
                varnames   ('self', 'tag_version', 'config', 'distance', 'node', 'dirty', 'preformatted', 'branch', 'node_date', 'kw', 'date_epoch')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
                name       '__init__'
                firstlineno 120
                lnotab
                   0x020c040120010e01080104010e010e010e011c013e014a0246010e010e
                   010e010e01
             'return'
             'dict[str, Any]'
@@ -1145,15 +1145,15 @@
                   'ScmVersion.extra is deprecated and will be removed in future'
                   2
                   ('category', 'stacklevel')
                names      ('warnings', 'warn', 'DeprecationWarning', '_extra')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
                name       'extra'
                firstlineno 151
                lnotab 0x0202160102010c0102fd1205
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
@@ -1168,15 +1168,15 @@
                             18 RETURN_VALUE
                consts
                   None
                names      ('distance',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
                name       'exact'
                firstlineno 160
                lnotab 0x0202
             'str'
             code
                argcount  : 1
                nlocals   : 1
@@ -1198,15 +1198,15 @@
                consts
                   None
                   '<ScmVersion {tag} dist={distance} node={node} dirty={dirty} branch={branch}>'
                names      ('format_with',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
                name       '__repr__'
                firstlineno 164
                lnotab 0x0201180102ff
             'fmt'
             code
                argcount  : 2
                nlocals   : 3
@@ -1257,15 +1257,15 @@
                   None
                   ('time', 'tag', 'distance', 'node', 'dirty', 'branch', 'node_date')
                   ()
                names      ('format', 'time', 'tag', 'distance', 'node', 'dirty', 'branch', 'node_date')
                varnames   ('self', 'fmt', 'kw')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
                name       'format_with'
                firstlineno 170
                lnotab 0x020110010c010c010c010c010c010c010cf9040802f8
             'clean_format'
             'dirty_format'
             code
                argcount  : 3
@@ -1294,15 +1294,15 @@
                             46 RETURN_VALUE
                consts
                   None
                names      ('format_with', 'dirty')
                varnames   ('self', 'clean_format', 'dirty_format', 'kw')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
                name       'format_choice'
                firstlineno 182
                lnotab 0x0201
             '{guessed}.dev{distance}'
             'guess_next'
             'Callable[Concatenate[ScmVersion, _t.P], str]'
             'k'
@@ -1343,15 +1343,15 @@
                consts
                   None
                   ('guessed',)
                names      ('format_with',)
                varnames   ('self', 'guess_next', 'fmt', 'k', 'kw', 'guessed')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
                name       'format_next_version'
                firstlineno 185
                lnotab 0x02071801
             (None, None, False, False, None, None)
             ('tag_version', 'Any', 'config', 'Configuration', 'distance', 'int | None', 'node', 'str | None', 'dirty', 'bool', 'preformatted', 'bool', 'branch', 'str | None', 'node_date', 'date | None', 'kw', 'object')
             ('return', 'dict[str, Any]')
             ('return', 'bool')
@@ -1360,15 +1360,15 @@
             ('clean_format', 'str', 'dirty_format', 'str', 'kw', 'object', 'return', 'str')
             ('{guessed}.dev{distance}',)
             ('guess_next', 'Callable[Concatenate[ScmVersion, _t.P], str]', 'fmt', 'str', 'k', '_t.P.args', 'kw', '_t.P.kwargs', 'return', 'str')
          names      ('__name__', '__module__', '__qualname__', '__init__', 'property', 'extra', 'exact', '__repr__', 'format_with', 'format_choice', 'format_next_version')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'ScmVersion'
          firstlineno 119
          lnotab
             0x0a050201020102010201020102f70a1f020106ff0e010208020106ff0e
             0102030806080c080602fd
       'ScmVersion'
       'preformatted'
@@ -1420,15 +1420,15 @@
                      102 RETURN_VALUE
          consts
             None
          names      ('isinstance', 'version_cls', 'tag_to_version')
          varnames   ('tag', 'preformatted', 'config', 'version')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_parse_tag'
          firstlineno 196
          lnotab 0x0203040104012e01200108010402
       False
       'str | _VersionT'
       'distance'
       'int | None'
@@ -1534,15 +1534,15 @@
             '->'
             "Can't parse version %s"
             ('distance', 'node', 'dirty', 'preformatted', 'branch', 'config', 'node_date')
          names      ('warnings', 'warn', 'Configuration', '_parse_tag', 'trace', 'ScmVersion')
          varnames   ('tag', 'distance', 'dirty', 'node', 'preformatted', 'branch', 'config', 'node_date', 'kw', 'parsed_version')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'meta'
          firstlineno 209
          lnotab
             0x020b0401160102ff10041c01220124011e010c0102ff02020201020102
             0102010201020102f8040902f7
       'tag_version'
       code
@@ -1580,15 +1580,15 @@
                  >>  126 RETURN_VALUE
          consts
             None
          names      ('_strip_local', 'str', 'tag', '_bump_dev', '_bump_regex')
          varnames   ('tag_version', 'version')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'guess_next_version'
          firstlineno 242
          lnotab 0x02014201
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 5
@@ -1623,15 +1623,15 @@
                  >>  126 RETURN_VALUE
          consts
             None
          names      ('_strip_local', 'str', 'tag', '_bump_dev', '_add_post')
          varnames   ('tag_version', 'version')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_dont_guess_next_version'
          firstlineno 247
          lnotab 0x02014201
       'version_string'
       code
          argcount  : 1
          nlocals   : 4
@@ -1657,15 +1657,15 @@
          consts
             None
             '+'
          names      ('partition',)
          varnames   ('version_string', 'public', 'sep', 'local')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_strip_local'
          firstlineno 252
          lnotab 0x02013201
       'version'
       code
          argcount  : 1
          nlocals   : 1
@@ -1702,15 +1702,15 @@
             'post'
             ' already is a post release, refusing to guess the update'
             '.post1'
          names      ('ValueError',)
          varnames   ('version',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_add_post'
          firstlineno 257
          lnotab 0x020108010c0108ff1003
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
@@ -1768,15 +1768,15 @@
             '0'
             'choosing custom numbers for the `.devX` distance is not supported.\n The '
             " can't be bumped\nPlease drop the tag or create a new supported one ending in .dev0"
          names      ('rsplit', 'ValueError')
          varnames   ('version', 'prefix', 'tail')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_bump_dev'
          firstlineno 265
          lnotab 0x02010801040232010c010c01020202fe06ff1006
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 5
@@ -1843,15 +1843,15 @@
             ('version',)
             '%s%d'
             1
          names      ('re', 'match', 'ValueError', 'format', 'groups', 'int')
          varnames   ('version', 'match', 'prefix', 'tail')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_bump_regex'
          firstlineno 280
          lnotab 0x02012a0104010c01020128fe10052e01
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
@@ -1883,15 +1883,15 @@
          consts
             None
             '{tag}'
          names      ('exact', 'format_with', 'format_next_version', 'guess_next_version')
          varnames   ('version',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'guess_next_dev_version'
          firstlineno 292
          lnotab 0x02010e012a02
       True
       'retain'
       'int'
       'increment'
@@ -1919,15 +1919,15 @@
             00000000000000740c000000000000000000006b0000000000b02d6402a0
             070000000000000000000000000000000000000000640784007c034400a6
             000000ab000000000000000000a6010000ab0100000000000000005300
          299           0 RESUME                   0
          
          302           2 NOP
          
-         303           4 LOAD_CONST               1 (<code object <listcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 303>)
+         303           4 LOAD_CONST               1 (<code object <listcomp>, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 303>)
                        6 MAKE_FUNCTION            0
                        8 LOAD_GLOBAL              1 (NULL + str)
                       20 LOAD_FAST                0 (version)
                       22 LOAD_ATTR                1 (tag)
                       32 PRECALL                  1
                       36 CALL                     1
                       46 LOAD_METHOD              2 (split)
@@ -2022,15 +2022,15 @@
                      446 CALL                     1
                      456 LOAD_GLOBAL             12 (SEMVER_LEN)
                      468 COMPARE_OP               0 (<)
                      474 POP_JUMP_BACKWARD_IF_TRUE    45 (to 386)
          
          312     >>  476 LOAD_CONST               2 ('.')
                      478 LOAD_METHOD              7 (join)
-                     500 LOAD_CONST               7 (<code object <genexpr>, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 312>)
+                     500 LOAD_CONST               7 (<code object <genexpr>, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\version.py", line 312>)
                      502 MAKE_FUNCTION            0
                      504 LOAD_FAST                3 (parts)
                      506 GET_ITER
                      508 PRECALL                  0
                      512 CALL                     0
                      522 PRECALL                  1
                      526 CALL                     1
@@ -2061,15 +2061,15 @@
                             40 JUMP_BACKWARD           18 (to 6)
                        >>   42 RETURN_VALUE
                consts
                names      ('int',)
                varnames   ('.0', 'i')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
                name       '<listcomp>'
                firstlineno 303
                lnotab 0x
             '.'
             " can't be parsed as numeric version"
             0
             -1
@@ -2100,23 +2100,23 @@
                             50 RETURN_VALUE
                consts
                   None
                names      ('str',)
                varnames   ('.0', 'i')
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
                name       '<genexpr>'
                firstlineno 312
                lnotab 0x
          names      ('str', 'tag', 'split', 'ValueError', 'len', 'append', 'SEMVER_LEN', 'join')
          varnames   ('version', 'retain', 'increment', 'parts')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'guess_next_simple_semver'
          firstlineno 299
          lnotab 0x020302017601120124ff080226012aff26020401200130012aff3002
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 5
@@ -2181,15 +2181,15 @@
             ('retain', 'increment')
             'feature'
             ('retain',)
          names      ('exact', 'guess_next_simple_semver', 'SEMVER_LEN', 'branch', 'format_next_version', 'SEMVER_MINOR', 'SEMVER_PATCH')
          varnames   ('version',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'simplified_semver_version'
          firstlineno 315
          lnotab 0x02010e012e022001180118ff1204180118ff
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 5
@@ -2327,15 +2327,15 @@
             1
             '.'
             ('retain',)
          names      ('exact', 'format_with', 'branch', '_parse_version_tag', 'split', 'config', 'str', 'tag', 'SEMVER_MINOR', 'format_next_version', 'guess_next_version', 'guess_next_simple_semver')
          varnames   ('version', 'branch_ver_data', 'branch_ver', 'tag_ver_up_to_minor', 'branch_ver_up_to_minor')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'release_branch_semver_version'
          firstlineno 329
          lnotab
             0x02010e012a010e020c014aff10030401100118021404680144010c0234
             02
       code
          argcount  : 1
@@ -2372,15 +2372,15 @@
             'release_branch_semver is deprecated and will be removed in future. Use release_branch_semver_version instead'
             2
             ('category', 'stacklevel')
          names      ('warnings', 'warn', 'DeprecationWarning', 'release_branch_semver_version')
          varnames   ('version',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'release_branch_semver'
          firstlineno 354
          lnotab 0x0201160102020c0102fc1206
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
@@ -2412,15 +2412,15 @@
          consts
             None
             '{tag}'
          names      ('exact', 'format_with', 'format_next_version', '_dont_guess_next_version')
          varnames   ('version',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'no_guess_dev_version'
          firstlineno 364
          lnotab 0x02010e012a02
       'ver'
       'Match[str] | None'
       code
          argcount  : 1
@@ -2448,15 +2448,15 @@
          consts
             None
             '^(?P<date>(?P<year>\\d{2}|\\d{4})(?:\\.\\d{1,2}){2})(?:\\.(?P<patch>\\d*)){0,1}?$'
          names      ('re', 'match')
          varnames   ('ver', 'match')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'date_ver_match'
          firstlineno 371
          lnotab 0x02011602020302fb1007
       'date_fmt'
       'version_cls'
       'type | None'
       code
@@ -2681,15 +2681,15 @@
             0
             '{node_date:{date_fmt}}.{patch}'
             ('node_date', 'date_fmt', 'patch')
          names      ('date_ver_match', 'str', 'tag', 'warnings', 'warn', 'len', 'group', 'datetime', 'now', 'timezone', 'utc', 'date', 'strptime', 'int', 'format', 'PkgVersion')
          varnames   ('version', 'node_date', 'date_fmt', 'version_cls', 'match', 'today', 'head_date', 'tag_date', 'patch', 'next_version')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'guess_next_date_ver'
          firstlineno 382
          lnotab
             0x020c42010401160108ff10040401060304015401600108020401060274
             010c013601260210021601180104ff0eff10050401180106ff120404010e
             013001
       code
@@ -2797,15 +2797,15 @@
             -1
             'version'
             ('node_date', 'version_cls')
          names      ('exact', 'dirty', 'format_with', 'branch', 'startswith', '_parse_version_tag', 'split', 'config', 'date_ver_match', 'format_next_version', 'guess_next_date_ver', 'node_date', 'version_cls')
          varnames   ('version', 'branch_ver', 'ver', 'match')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'calver_by_date'
          firstlineno 435
          lnotab 0x02011c012a0242016601040110011e010401040118010c010c0116fd
       'time_format'
       code
          argcount  : 2
          nlocals   : 2
@@ -2856,15 +2856,15 @@
             ('time_format',)
             '+{node}'
             '+{node}.d{time:{time_format}}'
          names      ('exact', 'node', 'format_choice')
          varnames   ('version', 'time_format')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_format_local_with_time'
          firstlineno 453
          lnotab 0x02021c01180106ff1204180106ff
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -2885,15 +2885,15 @@
             None
             '%Y%m%d'
             ('time_format',)
          names      ('_format_local_with_time',)
          varnames   ('version',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'get_local_node_and_date'
          firstlineno 465
          lnotab 0x0201
       '%Y%m%d%H%M%S'
       'fmt'
       code
          argcount  : 2
@@ -2915,15 +2915,15 @@
          consts
             None
             ('time_format',)
          names      ('_format_local_with_time',)
          varnames   ('version', 'fmt')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'get_local_node_and_timestamp'
          firstlineno 469
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -2944,15 +2944,15 @@
             None
             ''
             '+dirty'
          names      ('format_choice',)
          varnames   ('version',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'get_local_dirty_tag'
          firstlineno 473
          lnotab 0x0201
       '_'
       code
          argcount  : 1
          nlocals   : 1
@@ -2966,15 +2966,15 @@
          consts
             None
             ''
          names      ()
          varnames   ('_',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'get_no_local_node'
          firstlineno 477
          lnotab 0x0201
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
@@ -3007,15 +3007,15 @@
             None
             '{tag}'
             '{tag}.post{distance}'
          names      ('exact', 'format_with')
          varnames   ('version',)
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'postrelease_version'
          firstlineno 481
          lnotab 0x02010e012a02
       'name'
       'Any | None'
       code
          argcount  : 2
@@ -3070,15 +3070,15 @@
             1
             ('iter_entry_points',)
             'ep found:'
          names      ('_entrypoints', 'iter_entry_points', 'trace', 'name', 'load')
          varnames   ('group', 'name', 'iter_entry_points', 'ep')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_get_ep'
          firstlineno 488
          lnotab 0x02010c021c012a012c02
       'entrypoint'
       'scheme_value'
       'str | list[str] | tuple[str, ...] | Callable[[ScmVersion], str] | None'
       '_memo'
@@ -3199,15 +3199,15 @@
             None
             'str|List[str]|Tuple[str, ...]|Callable[["ScmVersion"], str]|None'
             ('_memo',)
          names      ('set', 'isinstance', 'str', 'cast', '_get_ep', 'list', 'tuple', 'add', '_iter_version_schemes', 'callable')
          varnames   ('entrypoint', 'scheme_value', '_memo', 'variant')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_iter_version_schemes'
          firstlineno 498
          lnotab
             0x060904011c012a010c0102011efe10053801080108012a0132fd04041e
             010cff
       'entypoint'
       'given_value'
@@ -3224,15 +3224,15 @@
                        4 RETURN_VALUE
          consts
             None
          names      ()
          varnames   ('version', 'entypoint', 'given_value', 'default')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_call_version_scheme'
          firstlineno 524
          lnotab 0x0204
       'None'
       code
          argcount  : 4
          nlocals   : 4
@@ -3245,15 +3245,15 @@
                        4 RETURN_VALUE
          consts
             None
          names      ()
          varnames   ('version', 'entypoint', 'given_value', 'default')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_call_version_scheme'
          firstlineno 531
          lnotab 0x0204
       code
          argcount  : 4
          nlocals   : 6
          stacksize : 4
@@ -3294,15 +3294,15 @@
                       76 RETURN_VALUE
          consts
             None
          names      ('_iter_version_schemes',)
          varnames   ('version', 'entypoint', 'given_value', 'default', 'scheme', 'result')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       '_call_version_scheme'
          firstlineno 538
          lnotab 0x020324011601040108ff0202
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
@@ -3413,15 +3413,15 @@
             'local_scheme'
             '+unknown'
             'local_version'
          names      ('trace', 'preformatted', 'isinstance', 'tag', 'str', '_call_version_scheme')
          varnames   ('version', 'config', 'main_version', 'local_version')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
          name       'format_version'
          firstlineno 548
          lnotab
             0x0201200120010e0138010e010c0114ff1003200108010c0114ff100320
             01
       ('tag', 'str | object', 'config', 'Configuration', 'return', 'dict[str, str] | None')
       ('group', 'str', 'callable_or_name', 'str | Any', 'return', 'Any')
@@ -3451,15 +3451,15 @@
       ('version', 'ScmVersion', 'entypoint', 'str', 'given_value', 'str', 'default', 'None', 'return', 'str | None')
       ('version', 'ScmVersion', 'entypoint', 'str', 'given_value', 'str', 'default', 'str | None', 'return', 'str | None')
       ('version', 'ScmVersion', 'config', 'Any', 'return', 'str')
    names      ('__future__', 'annotations', 'os', 're', 'warnings', 'datetime', 'date', 'timezone', 'typing', 'Any', 'Callable', 'cast', 'Iterator', 'List', 'Match', 'overload', 'Tuple', 'TYPE_CHECKING', 'typing_extensions', 'Concatenate', '', '_types', '_t', '_version_cls', 'Version', 'PkgVersion', 'config', 'Configuration', '_VersionT', 'utils', 'trace', 'SEMVER_MINOR', 'SEMVER_PATCH', 'SEMVER_LEN', '_parse_version_tag', 'callable_or_entrypoint', 'tag_to_version', 'tags_to_versions', 'ScmVersion', '_parse_tag', 'meta', 'guess_next_version', '_dont_guess_next_version', '_strip_local', '_add_post', '_bump_dev', '_bump_regex', 'guess_next_dev_version', 'guess_next_simple_semver', 'simplified_semver_version', 'release_branch_semver_version', 'release_branch_semver', 'no_guess_dev_version', 'date_ver_match', 'guess_next_date_ver', 'calver_by_date', '_format_local_with_time', 'get_local_node_and_date', 'get_local_node_and_timestamp', 'get_local_dirty_tag', 'get_no_local_node', 'postrelease_version', '_get_ep', '_iter_version_schemes', '_call_version_scheme', 'format_version')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\version.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c020801080108010c010c010c010c010c010c010c010c010c
       010c010c010c0204010c020c020c010c010c010c02040104010403081808
       0d02ff0a2202ff0a101a4d080f02010201020102010201020102f80a2108
       05080508050808080f080c080802ff0a10080e0819080a0807080d020102
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/pyproject_reading.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 2838
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 2933
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 16777216
    code
       0x97005500640064016c006d015a010100640064026c025a02640064026c
@@ -112,41 +112,41 @@
                176 LOAD_CONST              12 ('TypeAlias')
                178 LOAD_NAME               17 (__annotations__)
                180 LOAD_CONST              14 ('TOML_LOADER')
                182 STORE_SUBSCR
    
     21         186 PUSH_NULL
                188 LOAD_BUILD_CLASS
-               190 LOAD_CONST              15 (<code object PyProjectData, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_integration\pyproject_reading.py", line 21>)
+               190 LOAD_CONST              15 (<code object PyProjectData, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_integration\pyproject_reading.py", line 21>)
                192 MAKE_FUNCTION            0
                194 LOAD_CONST              16 ('PyProjectData')
                196 LOAD_NAME                8 (NamedTuple)
                198 PRECALL                  3
                202 CALL                     3
                212 STORE_NAME              19 (PyProjectData)
    
     32         214 LOAD_CONST              33 (('data', 'str', 'return', 'TOML_RESULT'))
-               216 LOAD_CONST              20 (<code object lazy_toml_load, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_integration\pyproject_reading.py", line 32>)
+               216 LOAD_CONST              20 (<code object lazy_toml_load, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_integration\pyproject_reading.py", line 32>)
                218 MAKE_FUNCTION            4 (annotations)
                220 STORE_NAME              20 (lazy_toml_load)
    
     42         222 NOP
    
     43         224 NOP
    
     44         226 NOP
    
     41         228 LOAD_CONST              34 (('pyproject.toml', 'setuptools_scm', None))
                230 LOAD_CONST              35 (('name', 'str', 'tool_name', 'str', '_load_toml', 'TOML_LOADER | None', 'return', 'PyProjectData'))
-               232 LOAD_CONST              27 (<code object read_pyproject, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_integration\pyproject_reading.py", line 41>)
+               232 LOAD_CONST              27 (<code object read_pyproject, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_integration\pyproject_reading.py", line 41>)
                234 MAKE_FUNCTION            5 (defaults, annotations)
                236 STORE_NAME              21 (read_pyproject)
    
     59         238 LOAD_CONST              36 (('pyproject', 'PyProjectData', 'dist_name', 'str | None', 'kwargs', 'TOML_RESULT', 'return', 'TOML_RESULT'))
-               240 LOAD_CONST              32 (<code object get_args_for_pyproject, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_integration\pyproject_reading.py", line 59>)
+               240 LOAD_CONST              32 (<code object get_args_for_pyproject, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_integration\pyproject_reading.py", line 59>)
                242 MAKE_FUNCTION            4 (annotations)
                244 STORE_NAME              22 (get_args_for_pyproject)
                246 LOAD_CONST               2 (None)
                248 RETURN_VALUE
    consts
       0
       ('annotations',)
@@ -198,15 +198,15 @@
                       44 LOAD_NAME                3 (__annotations__)
                       46 LOAD_CONST               6 ('section')
                       48 STORE_SUBSCR
          
           27          52 LOAD_NAME                4 (property)
          
           28          54 LOAD_CONST              11 (('return', 'str | None'))
-                      56 LOAD_CONST               9 (<code object project_name, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_integration\pyproject_reading.py", line 27>)
+                      56 LOAD_CONST               9 (<code object project_name, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_integration\pyproject_reading.py", line 27>)
                       58 MAKE_FUNCTION            4 (annotations)
          
           27          60 PRECALL                  0
                       64 CALL                     0
          
           28          74 STORE_NAME               5 (project_name)
                       76 LOAD_CONST              10 (None)
@@ -241,25 +241,25 @@
                consts
                   None
                   'name'
                names      ('project', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\pyproject_reading.py'
+               filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\pyproject_reading.py'
                name       'project_name'
                firstlineno 27
                lnotab 0x0202
             None
             ('return', 'str | None')
          names      ('__name__', '__module__', '__qualname__', '__annotations__', 'property', 'project_name')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\pyproject_reading.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\pyproject_reading.py'
          name       'PyProjectData'
          firstlineno 21
          lnotab 0x0c010a010a010a010a02020106ff0e01
       'PyProjectData'
       'data'
       'str'
       'return'
@@ -306,15 +306,15 @@
             (3, 11)
             0
             ('loads',)
          names      ('sys', 'version_info', 'tomllib', 'loads', 'tomli')
          varnames   ('data', 'loads')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\pyproject_reading.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\pyproject_reading.py'
          name       'lazy_toml_load'
          firstlineno 32
          lnotab 0x020120010e020c02
       'pyproject.toml'
       'setuptools_scm'
       'name'
       'tool_name'
@@ -461,15 +461,15 @@
             ' does not contain a tool.'
             ' section'
             'project'
          names      ('lazy_toml_load', 'open', 'read', 'get', 'LookupError', 'PyProjectData')
          varnames   ('name', 'tool_name', '_load_toml', 'strm', 'data', 'defn', 'section', 'e', 'project')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\pyproject_reading.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\pyproject_reading.py'
          name       'read_pyproject'
          firstlineno 41
          lnotab 0x020504010e01240128ff2e02160102013c01120134ff08022c01
       'pyproject'
       'dist_name'
       'str | None'
       'kwargs'
@@ -677,28 +677,28 @@
             'root '
             ' is overridden by the cli arg '
             'root'
          names      ('section', 'copy', 'pop', 'warnings', 'warn', 'name', 'tool_name', 'project_name', 'read_dist_name_from_setup_cfg', '_ROOT')
          varnames   ('pyproject', 'dist_name', 'kwargs', 'section', 'relative')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\pyproject_reading.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\pyproject_reading.py'
          name       'get_args_for_pyproject'
          firstlineno 59
          lnotab
             0x02063201280108012a011601200102ff06ff1005080104012c021c0106
             0104020e0104011c0112011a0138011201380116011e0118ff04ff10042c
             01
       ('data', 'str', 'return', 'TOML_RESULT')
       ('pyproject.toml', 'setuptools_scm', None)
       ('name', 'str', 'tool_name', 'str', '_load_toml', 'TOML_LOADER | None', 'return', 'PyProjectData')
       ('pyproject', 'PyProjectData', 'dist_name', 'str | None', 'kwargs', 'TOML_RESULT', 'return', 'TOML_RESULT')
    names      ('__future__', 'annotations', 'sys', 'warnings', 'typing', 'Any', 'Callable', 'Dict', 'NamedTuple', 'TYPE_CHECKING', 'setuptools', 'read_dist_name_from_setup_cfg', 'typing_extensions', 'TypeAlias', '_ROOT', 'str', 'TOML_RESULT', '__annotations__', 'TOML_LOADER', 'PyProjectData', 'lazy_toml_load', 'read_pyproject', 'get_args_for_pyproject')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\pyproject_reading.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\pyproject_reading.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010e02080108010c010c010c010c010c020c0204010c0204011e
       0120031c0b080a0201020102fd0a12
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/__pycache__/setuptools.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x3f848964 (Wed Jun 14 09:11:27 2023 UTC)
-files sz: 530
+moddate:  0x53679164 (Tue Jun 20 08:46:11 2023 UTC)
+files sz: 552
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 16777216
    code
       0x9700640064016c006d015a010100640064026c025a02640064036c036d
@@ -30,15 +30,15 @@
                 30 STORE_NAME               4 (IO)
                 32 POP_TOP
    
      8          34 NOP
    
      7          36 LOAD_CONST              10 (('setup.cfg',))
                 38 LOAD_CONST              11 (('input', 'str | os.PathLike[str] | IO[str]', 'return', 'str | None'))
-                40 LOAD_CONST               9 (<code object read_dist_name_from_setup_cfg, file "d:\documents\python scripts\scripts henry\hgutilities\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_integration\setuptools.py", line 7>)
+                40 LOAD_CONST               9 (<code object read_dist_name_from_setup_cfg, file "d:\documents\python scripts\scripts henry\hgutilities\.eggs\setuptools_scm-7.1.0-py3.11.egg\setuptools_scm\_integration\setuptools.py", line 7>)
                 42 MAKE_FUNCTION            5 (defaults, annotations)
                 44 STORE_NAME               5 (read_dist_name_from_setup_cfg)
                 46 LOAD_CONST               2 (None)
                 48 RETURN_VALUE
    consts
       0
       ('annotations',)
@@ -125,21 +125,21 @@
             'metadata'
             'name'
             ('fallback',)
          names      ('configparser', 'ConfigParser', 'isinstance', 'os', 'PathLike', 'str', 'read', 'read_file', 'get')
          varnames   ('input', 'configparser', 'parser', 'dist_name')
          freevars   ()
          cellvars   ()
-         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\setuptools.py'
+         filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\setuptools.py'
          name       'read_dist_name_from_setup_cfg'
          firstlineno 7
          lnotab 0x020508022802420132022a023001
       ('setup.cfg',)
       ('input', 'str | os.PathLike[str] | IO[str]', 'return', 'str | None')
    names      ('__future__', 'annotations', 'os', 'typing', 'IO', 'read_dist_name_from_setup_cfg')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\setuptools.py'
+   filename   'd:\\documents\\python scripts\\scripts henry\\hgutilities\\.eggs\\setuptools_scm-7.1.0-py3.11.egg\\setuptools_scm\\_integration\\setuptools.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0208010c0402ff
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_integration/pyproject_reading.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-from __future__ import annotations
-
-import sys
-import warnings
-from typing import Any
-from typing import Callable
-from typing import Dict
-from typing import NamedTuple
-from typing import TYPE_CHECKING
-
-from .setuptools import read_dist_name_from_setup_cfg
-
-if TYPE_CHECKING:
-    from typing_extensions import TypeAlias
-
-_ROOT = "root"
-TOML_RESULT: TypeAlias = Dict[str, Any]
-TOML_LOADER: TypeAlias = Callable[[str], TOML_RESULT]
-
-
-class PyProjectData(NamedTuple):
-    name: str
-    tool_name: str
-    project: TOML_RESULT
-    section: TOML_RESULT
-
-    @property
-    def project_name(self) -> str | None:
-        return self.project.get("name")
-
-
-def lazy_toml_load(data: str) -> TOML_RESULT:
-    if sys.version_info >= (3, 11):
-        from tomllib import loads
-    else:
-        from tomli import loads
-
-    return loads(data)
-
-
-def read_pyproject(
-    name: str = "pyproject.toml",
-    tool_name: str = "setuptools_scm",
-    _load_toml: TOML_LOADER | None = None,
-) -> PyProjectData:
-    if _load_toml is None:
-        _load_toml = lazy_toml_load
-    with open(name, encoding="UTF-8") as strm:
-        data = strm.read()
-    defn = _load_toml(data)
-    try:
-        section = defn.get("tool", {})[tool_name]
-    except LookupError as e:
-        raise LookupError(f"{name} does not contain a tool.{tool_name} section") from e
-    project = defn.get("project", {})
-    return PyProjectData(name, tool_name, project, section)
-
-
-def get_args_for_pyproject(
-    pyproject: PyProjectData,
-    dist_name: str | None,
-    kwargs: TOML_RESULT,
-) -> TOML_RESULT:
-    """drops problematic details and figures the distribution name"""
-    section = pyproject.section.copy()
-    kwargs = kwargs.copy()
-    if "relative_to" in section:
-        relative = section.pop("relative_to")
-        warnings.warn(
-            f"{pyproject.name}: at [tool.{pyproject.tool_name}]\n"
-            f"ignoring value relative_to={relative!r}"
-            " as its always relative to the config file"
-        )
-    if "dist_name" in section:
-        if dist_name is None:
-            dist_name = section.pop("dist_name")
-        else:
-            assert dist_name == section["dist_name"]
-            del section["dist_name"]
-    if dist_name is None:
-        # minimal pep 621 support for figuring the pretend keys
-        dist_name = pyproject.project_name
-    if dist_name is None:
-        dist_name = read_dist_name_from_setup_cfg()
-    if _ROOT in kwargs:
-        if kwargs[_ROOT] is None:
-            kwargs.pop(_ROOT, None)
-        elif _ROOT in section:
-            if section[_ROOT] != kwargs[_ROOT]:
-                warnings.warn(
-                    f"root {section[_ROOT]} is overridden"
-                    f" by the cli arg {kwargs[_ROOT]}"
-                )
-            section.pop("root", None)
-    return {"dist_name": dist_name, **section, **kwargs}
+from __future__ import annotations
+
+import sys
+import warnings
+from typing import Any
+from typing import Callable
+from typing import Dict
+from typing import NamedTuple
+from typing import TYPE_CHECKING
+
+from .setuptools import read_dist_name_from_setup_cfg
+
+if TYPE_CHECKING:
+    from typing_extensions import TypeAlias
+
+_ROOT = "root"
+TOML_RESULT: TypeAlias = Dict[str, Any]
+TOML_LOADER: TypeAlias = Callable[[str], TOML_RESULT]
+
+
+class PyProjectData(NamedTuple):
+    name: str
+    tool_name: str
+    project: TOML_RESULT
+    section: TOML_RESULT
+
+    @property
+    def project_name(self) -> str | None:
+        return self.project.get("name")
+
+
+def lazy_toml_load(data: str) -> TOML_RESULT:
+    if sys.version_info >= (3, 11):
+        from tomllib import loads
+    else:
+        from tomli import loads
+
+    return loads(data)
+
+
+def read_pyproject(
+    name: str = "pyproject.toml",
+    tool_name: str = "setuptools_scm",
+    _load_toml: TOML_LOADER | None = None,
+) -> PyProjectData:
+    if _load_toml is None:
+        _load_toml = lazy_toml_load
+    with open(name, encoding="UTF-8") as strm:
+        data = strm.read()
+    defn = _load_toml(data)
+    try:
+        section = defn.get("tool", {})[tool_name]
+    except LookupError as e:
+        raise LookupError(f"{name} does not contain a tool.{tool_name} section") from e
+    project = defn.get("project", {})
+    return PyProjectData(name, tool_name, project, section)
+
+
+def get_args_for_pyproject(
+    pyproject: PyProjectData,
+    dist_name: str | None,
+    kwargs: TOML_RESULT,
+) -> TOML_RESULT:
+    """drops problematic details and figures the distribution name"""
+    section = pyproject.section.copy()
+    kwargs = kwargs.copy()
+    if "relative_to" in section:
+        relative = section.pop("relative_to")
+        warnings.warn(
+            f"{pyproject.name}: at [tool.{pyproject.tool_name}]\n"
+            f"ignoring value relative_to={relative!r}"
+            " as its always relative to the config file"
+        )
+    if "dist_name" in section:
+        if dist_name is None:
+            dist_name = section.pop("dist_name")
+        else:
+            assert dist_name == section["dist_name"]
+            del section["dist_name"]
+    if dist_name is None:
+        # minimal pep 621 support for figuring the pretend keys
+        dist_name = pyproject.project_name
+    if dist_name is None:
+        dist_name = read_dist_name_from_setup_cfg()
+    if _ROOT in kwargs:
+        if kwargs[_ROOT] is None:
+            kwargs.pop(_ROOT, None)
+        elif _ROOT in section:
+            if section[_ROOT] != kwargs[_ROOT]:
+                warnings.warn(
+                    f"root {section[_ROOT]} is overridden"
+                    f" by the cli arg {kwargs[_ROOT]}"
+                )
+            section.pop("root", None)
+    return {"dist_name": dist_name, **section, **kwargs}
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_overrides.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from __future__ import annotations
-
-import os
-
-from .config import Configuration
-from .utils import trace
-from .version import meta
-from .version import ScmVersion
-
-
-PRETEND_KEY = "SETUPTOOLS_SCM_PRETEND_VERSION"
-PRETEND_KEY_NAMED = PRETEND_KEY + "_FOR_{name}"
-
-
-def _read_pretended_version_for(config: Configuration) -> ScmVersion | None:
-    """read a a overridden version from the environment
-
-    tries ``SETUPTOOLS_SCM_PRETEND_VERSION``
-    and ``SETUPTOOLS_SCM_PRETEND_VERSION_FOR_$UPPERCASE_DIST_NAME``
-    """
-    trace("dist name:", config.dist_name)
-    pretended: str | None
-    if config.dist_name is not None:
-        pretended = os.environ.get(
-            PRETEND_KEY_NAMED.format(name=config.dist_name.upper())
-        )
-    else:
-        pretended = None
-
-    if pretended is None:
-        pretended = os.environ.get(PRETEND_KEY)
-
-    if pretended:
-        # we use meta here since the pretended version
-        # must adhere to the pep to begin with
-        return meta(tag=pretended, preformatted=True, config=config)
-    else:
-        return None
+from __future__ import annotations
+
+import os
+
+from .config import Configuration
+from .utils import trace
+from .version import meta
+from .version import ScmVersion
+
+
+PRETEND_KEY = "SETUPTOOLS_SCM_PRETEND_VERSION"
+PRETEND_KEY_NAMED = PRETEND_KEY + "_FOR_{name}"
+
+
+def _read_pretended_version_for(config: Configuration) -> ScmVersion | None:
+    """read a a overridden version from the environment
+
+    tries ``SETUPTOOLS_SCM_PRETEND_VERSION``
+    and ``SETUPTOOLS_SCM_PRETEND_VERSION_FOR_$UPPERCASE_DIST_NAME``
+    """
+    trace("dist name:", config.dist_name)
+    pretended: str | None
+    if config.dist_name is not None:
+        pretended = os.environ.get(
+            PRETEND_KEY_NAMED.format(name=config.dist_name.upper())
+        )
+    else:
+        pretended = None
+
+    if pretended is None:
+        pretended = os.environ.get(PRETEND_KEY)
+
+    if pretended:
+        # we use meta here since the pretended version
+        # must adhere to the pep to begin with
+        return meta(tag=pretended, preformatted=True, config=config)
+    else:
+        return None
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/_types.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from __future__ import annotations
-
-from typing import Any
-from typing import Callable
-from typing import List
-from typing import TYPE_CHECKING
-from typing import TypeVar
-from typing import Union
-
-
-if TYPE_CHECKING:
-    from setuptools_scm import version
-    import os
-
-from typing_extensions import ParamSpec, TypeAlias, Protocol
-
-PathT = Union["os.PathLike[str]", str]
-
-CMD_TYPE: TypeAlias = Union[List[str], str]
-
-VERSION_SCHEME = Union[str, Callable[["version.ScmVersion"], str]]
-
-
-class EntrypointProtocol(Protocol):
-    name: str
-
-    def load(self) -> Any:
-        pass
-
-
-T = TypeVar("T")
-T2 = TypeVar("T2")
-P = ParamSpec("P")
-
-
-def transfer_input_args(
-    template: Callable[P, T],
-) -> Callable[[Callable[..., T]], Callable[P, T]]:
-    def decorate(func: Callable[..., T2]) -> Callable[P, T2]:
-        return func
-
-    return decorate
+from __future__ import annotations
+
+from typing import Any
+from typing import Callable
+from typing import List
+from typing import TYPE_CHECKING
+from typing import TypeVar
+from typing import Union
+
+
+if TYPE_CHECKING:
+    from setuptools_scm import version
+    import os
+
+from typing_extensions import ParamSpec, TypeAlias, Protocol
+
+PathT = Union["os.PathLike[str]", str]
+
+CMD_TYPE: TypeAlias = Union[List[str], str]
+
+VERSION_SCHEME = Union[str, Callable[["version.ScmVersion"], str]]
+
+
+class EntrypointProtocol(Protocol):
+    name: str
+
+    def load(self) -> Any:
+        pass
+
+
+T = TypeVar("T")
+T2 = TypeVar("T2")
+P = ParamSpec("P")
+
+
+def transfer_input_args(
+    template: Callable[P, T],
+) -> Callable[[Callable[..., T]], Callable[P, T]]:
+    def decorate(func: Callable[..., T2]) -> Callable[P, T2]:
+        return func
+
+    return decorate
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from __future__ import annotations
-
-import os
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing_extensions import TypeGuard
-    from . import _types as _t
-
-from .utils import trace
-
-
-def scm_find_files(
-    path: _t.PathT,
-    scm_files: set[str],
-    scm_dirs: set[str],
-    force_all_files: bool = False,
-) -> list[str]:
-    """ setuptools compatible file finder that follows symlinks
-
-    - path: the root directory from which to search
-    - scm_files: set of scm controlled files and symlinks
-      (including symlinks to directories)
-    - scm_dirs: set of scm controlled directories
-      (including directories containing no scm controlled files)
-    - force_all_files: ignore ``scm_files`` and ``scm_dirs`` and list everything.
-
-    scm_files and scm_dirs must be absolute with symlinks resolved (realpath),
-    with normalized case (normcase)
-
-    Spec here: http://setuptools.readthedocs.io/en/latest/setuptools.html#\
-        adding-support-for-revision-control-systems
-    """
-    realpath = os.path.normcase(os.path.realpath(path))
-    seen: set[str] = set()
-    res: list[str] = []
-    for dirpath, dirnames, filenames in os.walk(realpath, followlinks=True):
-        # dirpath with symlinks resolved
-        realdirpath = os.path.normcase(os.path.realpath(dirpath))
-
-        def _link_not_in_scm(n: str) -> bool:
-            fn = os.path.join(realdirpath, os.path.normcase(n))
-            return os.path.islink(fn) and fn not in scm_files
-
-        if not force_all_files and realdirpath not in scm_dirs:
-            # directory not in scm, don't walk it's content
-            dirnames[:] = []
-            continue
-        if os.path.islink(dirpath) and not os.path.relpath(
-            realdirpath, realpath
-        ).startswith(os.pardir):
-            # a symlink to a directory not outside path:
-            # we keep it in the result and don't walk its content
-            res.append(os.path.join(path, os.path.relpath(dirpath, path)))
-            dirnames[:] = []
-            continue
-        if realdirpath in seen:
-            # symlink loop protection
-            dirnames[:] = []
-            continue
-        dirnames[:] = [
-            dn for dn in dirnames if force_all_files or not _link_not_in_scm(dn)
-        ]
-        for filename in filenames:
-            if not force_all_files and _link_not_in_scm(filename):
-                continue
-            # dirpath + filename with symlinks preserved
-            fullfilename = os.path.join(dirpath, filename)
-            is_tracked = os.path.normcase(os.path.realpath(fullfilename)) in scm_files
-            if force_all_files or is_tracked:
-                res.append(os.path.join(path, os.path.relpath(fullfilename, realpath)))
-        seen.add(realdirpath)
-    return res
-
-
-def is_toplevel_acceptable(toplevel: str | None) -> TypeGuard[str]:
-    """ """
-    if toplevel is None:
-        return False
-
-    ignored = os.environ.get("SETUPTOOLS_SCM_IGNORE_VCS_ROOTS", "").split(os.pathsep)
-    ignored = [os.path.normcase(p) for p in ignored]
-
-    trace(toplevel, ignored)
-
-    return toplevel not in ignored
+from __future__ import annotations
+
+import os
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing_extensions import TypeGuard
+    from . import _types as _t
+
+from .utils import trace
+
+
+def scm_find_files(
+    path: _t.PathT,
+    scm_files: set[str],
+    scm_dirs: set[str],
+    force_all_files: bool = False,
+) -> list[str]:
+    """ setuptools compatible file finder that follows symlinks
+
+    - path: the root directory from which to search
+    - scm_files: set of scm controlled files and symlinks
+      (including symlinks to directories)
+    - scm_dirs: set of scm controlled directories
+      (including directories containing no scm controlled files)
+    - force_all_files: ignore ``scm_files`` and ``scm_dirs`` and list everything.
+
+    scm_files and scm_dirs must be absolute with symlinks resolved (realpath),
+    with normalized case (normcase)
+
+    Spec here: http://setuptools.readthedocs.io/en/latest/setuptools.html#\
+        adding-support-for-revision-control-systems
+    """
+    realpath = os.path.normcase(os.path.realpath(path))
+    seen: set[str] = set()
+    res: list[str] = []
+    for dirpath, dirnames, filenames in os.walk(realpath, followlinks=True):
+        # dirpath with symlinks resolved
+        realdirpath = os.path.normcase(os.path.realpath(dirpath))
+
+        def _link_not_in_scm(n: str) -> bool:
+            fn = os.path.join(realdirpath, os.path.normcase(n))
+            return os.path.islink(fn) and fn not in scm_files
+
+        if not force_all_files and realdirpath not in scm_dirs:
+            # directory not in scm, don't walk it's content
+            dirnames[:] = []
+            continue
+        if os.path.islink(dirpath) and not os.path.relpath(
+            realdirpath, realpath
+        ).startswith(os.pardir):
+            # a symlink to a directory not outside path:
+            # we keep it in the result and don't walk its content
+            res.append(os.path.join(path, os.path.relpath(dirpath, path)))
+            dirnames[:] = []
+            continue
+        if realdirpath in seen:
+            # symlink loop protection
+            dirnames[:] = []
+            continue
+        dirnames[:] = [
+            dn for dn in dirnames if force_all_files or not _link_not_in_scm(dn)
+        ]
+        for filename in filenames:
+            if not force_all_files and _link_not_in_scm(filename):
+                continue
+            # dirpath + filename with symlinks preserved
+            fullfilename = os.path.join(dirpath, filename)
+            is_tracked = os.path.normcase(os.path.realpath(fullfilename)) in scm_files
+            if force_all_files or is_tracked:
+                res.append(os.path.join(path, os.path.relpath(fullfilename, realpath)))
+        seen.add(realdirpath)
+    return res
+
+
+def is_toplevel_acceptable(toplevel: str | None) -> TypeGuard[str]:
+    """ """
+    if toplevel is None:
+        return False
+
+    ignored = os.environ.get("SETUPTOOLS_SCM_IGNORE_VCS_ROOTS", "").split(os.pathsep)
+    ignored = [os.path.normcase(p) for p in ignored]
+
+    trace(toplevel, ignored)
+
+    return toplevel not in ignored
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_git.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-from __future__ import annotations
-
-import logging
-import os
-import subprocess
-import tarfile
-from typing import IO
-from typing import TYPE_CHECKING
-
-from .file_finder import is_toplevel_acceptable
-from .file_finder import scm_find_files
-from .utils import data_from_mime
-from .utils import do_ex
-from .utils import trace
-
-if TYPE_CHECKING:
-    from . import _types as _t
-
-
-log = logging.getLogger(__name__)
-
-
-def _git_toplevel(path: str) -> str | None:
-    try:
-        cwd = os.path.abspath(path or ".")
-        out, err, ret = do_ex(["git", "rev-parse", "HEAD"], cwd=cwd)
-        if ret != 0:
-            # BAIL if there is no commit
-            log.error("listing git files failed - pretending there aren't any")
-            return None
-        out, err, ret = do_ex(
-            ["git", "rev-parse", "--show-prefix"],
-            cwd=cwd,
-        )
-        if ret != 0:
-            return None
-        out = out.strip()[:-1]  # remove the trailing pathsep
-        if not out:
-            out = cwd
-        else:
-            # Here, ``out`` is a relative path to root of git.
-            # ``cwd`` is absolute path to current working directory.
-            # the below method removes the length of ``out`` from
-            # ``cwd``, which gives the git toplevel
-            assert cwd.replace("\\", "/").endswith(out), f"cwd={cwd!r}\nout={out!r}"
-            # In windows cwd contains ``\`` which should be replaced by ``/``
-            # for this assertion to work. Length of string isn't changed by replace
-            # ``\\`` is just and escape for `\`
-            out = cwd[: -len(out)]
-        trace("find files toplevel", out)
-        return os.path.normcase(os.path.realpath(out.strip()))
-    except subprocess.CalledProcessError:
-        # git returned error, we are not in a git repo
-        return None
-    except OSError:
-        # git command not found, probably
-        return None
-
-
-def _git_interpret_archive(fd: IO[bytes], toplevel: str) -> tuple[set[str], set[str]]:
-    with tarfile.open(fileobj=fd, mode="r|*") as tf:
-        git_files = set()
-        git_dirs = {toplevel}
-        for member in tf.getmembers():
-            name = os.path.normcase(member.name).replace("/", os.path.sep)
-            if member.type == tarfile.DIRTYPE:
-                git_dirs.add(name)
-            else:
-                git_files.add(name)
-        return git_files, git_dirs
-
-
-def _git_ls_files_and_dirs(toplevel: str) -> tuple[set[str], set[str]]:
-    # use git archive instead of git ls-file to honor
-    # export-ignore git attribute
-
-    cmd = ["git", "archive", "--prefix", toplevel + os.path.sep, "HEAD"]
-    proc = subprocess.Popen(
-        cmd, stdout=subprocess.PIPE, cwd=toplevel, stderr=subprocess.DEVNULL
-    )
-    assert proc.stdout is not None
-    try:
-        try:
-            return _git_interpret_archive(proc.stdout, toplevel)
-        finally:
-            # ensure we avoid resource warnings by cleaning up the process
-            proc.stdout.close()
-            proc.terminate()
-    except Exception:
-        if proc.wait() != 0:
-            log.error("listing git files failed - pretending there aren't any")
-        return set(), set()
-
-
-def git_find_files(path: _t.PathT = "") -> list[str]:
-    toplevel = _git_toplevel(os.fspath(path))
-    if not is_toplevel_acceptable(toplevel):
-        return []
-    assert toplevel is not None  # mypy ignores typeguard
-    fullpath = os.path.abspath(os.path.normpath(path))
-    if not fullpath.startswith(toplevel):
-        trace("toplevel mismatch", toplevel, fullpath)
-    git_files, git_dirs = _git_ls_files_and_dirs(toplevel)
-    return scm_find_files(path, git_files, git_dirs)
-
-
-def git_archive_find_files(path: _t.PathT = "") -> list[str]:
-    # This function assumes that ``path`` is obtained from a git archive
-    # and therefore all the files that should be ignored were already removed.
-    archival = os.path.join(path, ".git_archival.txt")
-    if not os.path.exists(archival):
-        return []
-
-    data = data_from_mime(archival)
-
-    if "$Format" in data.get("node", ""):
-        # Substitutions have not been performed, so not a reliable archive
-        return []
-
-    trace("git archive detected - fallback to listing all files")
-    return scm_find_files(path, set(), set(), force_all_files=True)
+from __future__ import annotations
+
+import logging
+import os
+import subprocess
+import tarfile
+from typing import IO
+from typing import TYPE_CHECKING
+
+from .file_finder import is_toplevel_acceptable
+from .file_finder import scm_find_files
+from .utils import data_from_mime
+from .utils import do_ex
+from .utils import trace
+
+if TYPE_CHECKING:
+    from . import _types as _t
+
+
+log = logging.getLogger(__name__)
+
+
+def _git_toplevel(path: str) -> str | None:
+    try:
+        cwd = os.path.abspath(path or ".")
+        out, err, ret = do_ex(["git", "rev-parse", "HEAD"], cwd=cwd)
+        if ret != 0:
+            # BAIL if there is no commit
+            log.error("listing git files failed - pretending there aren't any")
+            return None
+        out, err, ret = do_ex(
+            ["git", "rev-parse", "--show-prefix"],
+            cwd=cwd,
+        )
+        if ret != 0:
+            return None
+        out = out.strip()[:-1]  # remove the trailing pathsep
+        if not out:
+            out = cwd
+        else:
+            # Here, ``out`` is a relative path to root of git.
+            # ``cwd`` is absolute path to current working directory.
+            # the below method removes the length of ``out`` from
+            # ``cwd``, which gives the git toplevel
+            assert cwd.replace("\\", "/").endswith(out), f"cwd={cwd!r}\nout={out!r}"
+            # In windows cwd contains ``\`` which should be replaced by ``/``
+            # for this assertion to work. Length of string isn't changed by replace
+            # ``\\`` is just and escape for `\`
+            out = cwd[: -len(out)]
+        trace("find files toplevel", out)
+        return os.path.normcase(os.path.realpath(out.strip()))
+    except subprocess.CalledProcessError:
+        # git returned error, we are not in a git repo
+        return None
+    except OSError:
+        # git command not found, probably
+        return None
+
+
+def _git_interpret_archive(fd: IO[bytes], toplevel: str) -> tuple[set[str], set[str]]:
+    with tarfile.open(fileobj=fd, mode="r|*") as tf:
+        git_files = set()
+        git_dirs = {toplevel}
+        for member in tf.getmembers():
+            name = os.path.normcase(member.name).replace("/", os.path.sep)
+            if member.type == tarfile.DIRTYPE:
+                git_dirs.add(name)
+            else:
+                git_files.add(name)
+        return git_files, git_dirs
+
+
+def _git_ls_files_and_dirs(toplevel: str) -> tuple[set[str], set[str]]:
+    # use git archive instead of git ls-file to honor
+    # export-ignore git attribute
+
+    cmd = ["git", "archive", "--prefix", toplevel + os.path.sep, "HEAD"]
+    proc = subprocess.Popen(
+        cmd, stdout=subprocess.PIPE, cwd=toplevel, stderr=subprocess.DEVNULL
+    )
+    assert proc.stdout is not None
+    try:
+        try:
+            return _git_interpret_archive(proc.stdout, toplevel)
+        finally:
+            # ensure we avoid resource warnings by cleaning up the process
+            proc.stdout.close()
+            proc.terminate()
+    except Exception:
+        if proc.wait() != 0:
+            log.error("listing git files failed - pretending there aren't any")
+        return set(), set()
+
+
+def git_find_files(path: _t.PathT = "") -> list[str]:
+    toplevel = _git_toplevel(os.fspath(path))
+    if not is_toplevel_acceptable(toplevel):
+        return []
+    assert toplevel is not None  # mypy ignores typeguard
+    fullpath = os.path.abspath(os.path.normpath(path))
+    if not fullpath.startswith(toplevel):
+        trace("toplevel mismatch", toplevel, fullpath)
+    git_files, git_dirs = _git_ls_files_and_dirs(toplevel)
+    return scm_find_files(path, git_files, git_dirs)
+
+
+def git_archive_find_files(path: _t.PathT = "") -> list[str]:
+    # This function assumes that ``path`` is obtained from a git archive
+    # and therefore all the files that should be ignored were already removed.
+    archival = os.path.join(path, ".git_archival.txt")
+    if not os.path.exists(archival):
+        return []
+
+    data = data_from_mime(archival)
+
+    if "$Format" in data.get("node", ""):
+        # Substitutions have not been performed, so not a reliable archive
+        return []
+
+    trace("git archive detected - fallback to listing all files")
+    return scm_find_files(path, set(), set(), force_all_files=True)
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/file_finder_hg.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-from __future__ import annotations
-
-import os
-import subprocess
-from typing import TYPE_CHECKING
-
-from .file_finder import is_toplevel_acceptable
-from .file_finder import scm_find_files
-from .utils import data_from_mime
-from .utils import do_ex
-from .utils import trace
-
-if TYPE_CHECKING:
-    from . import _types as _t
-
-
-def _hg_toplevel(path: str) -> str | None:
-    try:
-        out: str = subprocess.check_output(
-            ["hg", "root"],
-            cwd=(path or "."),
-            text=True,
-            stderr=subprocess.DEVNULL,
-        )
-        return os.path.normcase(os.path.realpath(out.strip()))
-    except subprocess.CalledProcessError:
-        # hg returned error, we are not in a mercurial repo
-        return None
-    except OSError:
-        # hg command not found, probably
-        return None
-
-
-def _hg_ls_files_and_dirs(toplevel: str) -> tuple[set[str], set[str]]:
-    hg_files: set[str] = set()
-    hg_dirs = {toplevel}
-    out, err, ret = do_ex(["hg", "files"], cwd=toplevel)
-    if ret:
-        (), ()
-    for name in out.splitlines():
-        name = os.path.normcase(name).replace("/", os.path.sep)
-        fullname = os.path.join(toplevel, name)
-        hg_files.add(fullname)
-        dirname = os.path.dirname(fullname)
-        while len(dirname) > len(toplevel) and dirname not in hg_dirs:
-            hg_dirs.add(dirname)
-            dirname = os.path.dirname(dirname)
-    return hg_files, hg_dirs
-
-
-def hg_find_files(path: str = "") -> list[str]:
-    toplevel = _hg_toplevel(path)
-    if not is_toplevel_acceptable(toplevel):
-        return []
-    assert toplevel is not None
-    hg_files, hg_dirs = _hg_ls_files_and_dirs(toplevel)
-    return scm_find_files(path, hg_files, hg_dirs)
-
-
-def hg_archive_find_files(path: _t.PathT = "") -> list[str]:
-    # This function assumes that ``path`` is obtained from a mercurial archive
-    # and therefore all the files that should be ignored were already removed.
-    archival = os.path.join(path, ".hg_archival.txt")
-    if not os.path.exists(archival):
-        return []
-
-    data = data_from_mime(archival)
-
-    if "node" not in data:
-        # Ensure file is valid
-        return []
-
-    trace("hg archive detected - fallback to listing all files")
-    return scm_find_files(path, set(), set(), force_all_files=True)
+from __future__ import annotations
+
+import os
+import subprocess
+from typing import TYPE_CHECKING
+
+from .file_finder import is_toplevel_acceptable
+from .file_finder import scm_find_files
+from .utils import data_from_mime
+from .utils import do_ex
+from .utils import trace
+
+if TYPE_CHECKING:
+    from . import _types as _t
+
+
+def _hg_toplevel(path: str) -> str | None:
+    try:
+        out: str = subprocess.check_output(
+            ["hg", "root"],
+            cwd=(path or "."),
+            text=True,
+            stderr=subprocess.DEVNULL,
+        )
+        return os.path.normcase(os.path.realpath(out.strip()))
+    except subprocess.CalledProcessError:
+        # hg returned error, we are not in a mercurial repo
+        return None
+    except OSError:
+        # hg command not found, probably
+        return None
+
+
+def _hg_ls_files_and_dirs(toplevel: str) -> tuple[set[str], set[str]]:
+    hg_files: set[str] = set()
+    hg_dirs = {toplevel}
+    out, err, ret = do_ex(["hg", "files"], cwd=toplevel)
+    if ret:
+        (), ()
+    for name in out.splitlines():
+        name = os.path.normcase(name).replace("/", os.path.sep)
+        fullname = os.path.join(toplevel, name)
+        hg_files.add(fullname)
+        dirname = os.path.dirname(fullname)
+        while len(dirname) > len(toplevel) and dirname not in hg_dirs:
+            hg_dirs.add(dirname)
+            dirname = os.path.dirname(dirname)
+    return hg_files, hg_dirs
+
+
+def hg_find_files(path: str = "") -> list[str]:
+    toplevel = _hg_toplevel(path)
+    if not is_toplevel_acceptable(toplevel):
+        return []
+    assert toplevel is not None
+    hg_files, hg_dirs = _hg_ls_files_and_dirs(toplevel)
+    return scm_find_files(path, hg_files, hg_dirs)
+
+
+def hg_archive_find_files(path: _t.PathT = "") -> list[str]:
+    # This function assumes that ``path`` is obtained from a mercurial archive
+    # and therefore all the files that should be ignored were already removed.
+    archival = os.path.join(path, ".hg_archival.txt")
+    if not os.path.exists(archival):
+        return []
+
+    data = data_from_mime(archival)
+
+    if "node" not in data:
+        # Ensure file is valid
+        return []
+
+    trace("hg archive detected - fallback to listing all files")
+    return scm_find_files(path, set(), set(), force_all_files=True)
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/git.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,323 +1,323 @@
-from __future__ import annotations
-
-import os
-import re
-import warnings
-from datetime import date
-from datetime import datetime
-from os.path import isfile
-from os.path import join
-from os.path import samefile
-from typing import Callable
-from typing import TYPE_CHECKING
-
-from .config import Configuration
-from .scm_workdir import Workdir
-from .utils import _CmdResult
-from .utils import data_from_mime
-from .utils import do_ex
-from .utils import require_command
-from .utils import trace
-from .version import meta
-from .version import ScmVersion
-from .version import tags_to_versions
-
-if TYPE_CHECKING:
-    from . import _types as _t
-
-    from setuptools_scm.hg_git import GitWorkdirHgClient
-
-REF_TAG_RE = re.compile(r"(?<=\btag: )([^,]+)\b")
-DESCRIBE_UNSUPPORTED = "%(describe"
-
-# If testing command in shell make sure to quote the match argument like
-# '*[0-9]*' as it will expand before being sent to git if there are any matching
-# files in current directory.
-DEFAULT_DESCRIBE = [
-    "git",
-    "describe",
-    "--dirty",
-    "--tags",
-    "--long",
-    "--match",
-    "*[0-9]*",
-]
-
-
-class GitWorkdir(Workdir):
-    """experimental, may change at any time"""
-
-    COMMAND = "git"
-
-    @classmethod
-    def from_potential_worktree(cls, wd: _t.PathT) -> GitWorkdir | None:
-        require_command(cls.COMMAND)
-        wd = os.path.abspath(wd)
-        git_dir = join(wd, ".git")
-        real_wd, _, ret = do_ex(
-            ["git", "--git-dir", git_dir, "rev-parse", "--show-prefix"], wd
-        )
-        real_wd = real_wd[:-1]  # remove the trailing pathsep
-        if ret:
-            return None
-        if not real_wd:
-            real_wd = wd
-        else:
-            assert wd.replace("\\", "/").endswith(real_wd)
-            # In windows wd contains ``\`` which should be replaced by ``/``
-            # for this assertion to work.  Length of string isn't changed by replace
-            # ``\\`` is just and escape for `\`
-            real_wd = wd[: -len(real_wd)]
-        trace("real root", real_wd)
-        if not samefile(real_wd, wd):
-            return None
-
-        return cls(real_wd)
-
-    def do_ex_git(self, cmd: list[str]) -> _CmdResult:
-        return self.do_ex(["git", "--git-dir", join(self.path, ".git")] + cmd)
-
-    def is_dirty(self) -> bool:
-        out, _, _ = self.do_ex_git(["status", "--porcelain", "--untracked-files=no"])
-        return bool(out)
-
-    def get_branch(self) -> str | None:
-        branch, err, ret = self.do_ex_git(["rev-parse", "--abbrev-ref", "HEAD"])
-        if ret:
-            trace("branch err", branch, err, ret)
-            branch, err, ret = self.do_ex_git(["symbolic-ref", "--short", "HEAD"])
-            if ret:
-                trace("branch err (symbolic-ref)", branch, err, ret)
-                return None
-        return branch
-
-    def get_head_date(self) -> date | None:
-        timestamp, err, ret = self.do_ex_git(
-            ["-c", "log.showSignature=false", "log", "-n", "1", "HEAD", "--format=%cI"]
-        )
-        if ret:
-            trace("timestamp err", timestamp, err, ret)
-            return None
-        # TODO, when dropping python3.6 use fromiso
-        date_part = timestamp.split("T")[0]
-        if "%c" in date_part:
-            trace("git too old -> timestamp is ", timestamp)
-            return None
-        return datetime.strptime(date_part, r"%Y-%m-%d").date()
-
-    def is_shallow(self) -> bool:
-        return isfile(join(self.path, ".git/shallow"))
-
-    def fetch_shallow(self) -> None:
-        self.do_ex_git(["fetch", "--unshallow"])
-
-    def node(self) -> str | None:
-        node, _, ret = self.do_ex_git(["rev-parse", "--verify", "--quiet", "HEAD"])
-        if not ret:
-            return node[:7]
-        else:
-            return None
-
-    def count_all_nodes(self) -> int:
-        revs, _, _ = self.do_ex_git(["rev-list", "HEAD"])
-        return revs.count("\n") + 1
-
-    def default_describe(self) -> _CmdResult:
-        git_dir = join(self.path, ".git")
-        return self.do_ex(
-            DEFAULT_DESCRIBE[:1] + ["--git-dir", git_dir] + DEFAULT_DESCRIBE[1:]
-        )
-
-
-def warn_on_shallow(wd: GitWorkdir) -> None:
-    """experimental, may change at any time"""
-    if wd.is_shallow():
-        warnings.warn(f'"{wd.path}" is shallow and may cause errors')
-
-
-def fetch_on_shallow(wd: GitWorkdir) -> None:
-    """experimental, may change at any time"""
-    if wd.is_shallow():
-        warnings.warn(f'"{wd.path}" was shallow, git fetch was used to rectify')
-        wd.fetch_shallow()
-
-
-def fail_on_shallow(wd: GitWorkdir) -> None:
-    """experimental, may change at any time"""
-    if wd.is_shallow():
-        raise ValueError(
-            f'{wd.path} is shallow, please correct with "git fetch --unshallow"'
-        )
-
-
-def get_working_directory(config: Configuration) -> GitWorkdir | None:
-    """
-    Return the working directory (``GitWorkdir``).
-    """
-
-    if config.parent:
-        return GitWorkdir.from_potential_worktree(config.parent)
-
-    if config.search_parent_directories:
-        return search_parent(config.absolute_root)
-
-    return GitWorkdir.from_potential_worktree(config.absolute_root)
-
-
-def parse(
-    root: str,
-    describe_command: str | list[str] | None = None,
-    pre_parse: Callable[[GitWorkdir], None] = warn_on_shallow,
-    config: Configuration | None = None,
-) -> ScmVersion | None:
-    """
-    :param pre_parse: experimental pre_parse action, may change at any time
-    """
-    if not config:
-        config = Configuration(root=root)
-
-    wd = get_working_directory(config)
-    if wd:
-        return _git_parse_inner(
-            config, wd, describe_command=describe_command, pre_parse=pre_parse
-        )
-    else:
-        return None
-
-
-def _git_parse_inner(
-    config: Configuration,
-    wd: GitWorkdir | GitWorkdirHgClient,
-    pre_parse: None | (Callable[[GitWorkdir | GitWorkdirHgClient], None]) = None,
-    describe_command: _t.CMD_TYPE | None = None,
-) -> ScmVersion:
-    if pre_parse:
-        pre_parse(wd)
-
-    if config.git_describe_command is not None:
-        describe_command = config.git_describe_command
-
-    if describe_command is not None:
-        out, _, ret = wd.do_ex(describe_command)
-    else:
-        out, _, ret = wd.default_describe()
-    distance: int | None
-    node: str | None
-    if ret == 0:
-        tag, distance, node, dirty = _git_parse_describe(out)
-        if distance == 0 and not dirty:
-            distance = None
-    else:
-        # If 'git git_describe_command' failed, try to get the information otherwise.
-        tag = "0.0"
-        node = wd.node()
-        if node is None:
-            distance = 0
-        else:
-            distance = wd.count_all_nodes()
-            node = "g" + node
-        dirty = wd.is_dirty()
-
-    branch = wd.get_branch()
-    node_date = wd.get_head_date() or date.today()
-
-    return meta(
-        tag,
-        branch=branch,
-        node=node,
-        node_date=node_date,
-        distance=distance,
-        dirty=dirty,
-        config=config,
-    )
-
-
-def _git_parse_describe(
-    describe_output: str,
-) -> tuple[str, int | None, str | None, bool]:
-    # 'describe_output' looks e.g. like 'v1.5.0-0-g4060507' or
-    # 'v1.15.1rc1-37-g9bd1298-dirty'.
-    # It may also just be a bare tag name if this is a tagged commit and we are
-    # parsing a .git_archival.txt file.
-
-    if describe_output.endswith("-dirty"):
-        dirty = True
-        describe_output = describe_output[:-6]
-    else:
-        dirty = False
-
-    split = describe_output.rsplit("-", 2)
-    if len(split) < 3:  # probably a tagged commit
-        tag = describe_output
-        number = None
-        node = None
-    else:
-        tag, number_, node = split
-        number = int(number_)
-    return tag, number, node, dirty
-
-
-def search_parent(dirname: _t.PathT) -> GitWorkdir | None:
-    """
-    Walk up the path to find the `.git` directory.
-    :param dirname: Directory from which to start searching.
-    """
-
-    # Code based on:
-    # https://github.com/gitpython-developers/GitPython/blob/main/git/repo/base.py
-
-    curpath = os.path.abspath(dirname)
-
-    while curpath:
-
-        try:
-            wd = GitWorkdir.from_potential_worktree(curpath)
-        except Exception:
-            wd = None
-
-        if wd is not None:
-            return wd
-
-        curpath, tail = os.path.split(curpath)
-
-        if not tail:
-            return None
-    return None
-
-
-def archival_to_version(
-    data: dict[str, str], config: Configuration | None = None
-) -> ScmVersion | None:
-    node: str | None
-    trace("data", data)
-    archival_describe = data.get("describe-name", DESCRIBE_UNSUPPORTED)
-    if DESCRIBE_UNSUPPORTED in archival_describe:
-        warnings.warn("git archive did not support describe output")
-    else:
-        tag, number, node, _ = _git_parse_describe(archival_describe)
-        return meta(
-            tag,
-            config=config,
-            distance=None if number == 0 else number,
-            node=node,
-        )
-    versions = tags_to_versions(REF_TAG_RE.findall(data.get("ref-names", "")))
-    if versions:
-        return meta(versions[0], config=config)
-    else:
-        node = data.get("node")
-        if node is None:
-            return None
-        elif "$FORMAT" in node.upper():
-            warnings.warn("unexported git archival found")
-            return None
-        else:
-            return meta("0.0", node=node, config=config)
-
-
-def parse_archival(
-    root: _t.PathT, config: Configuration | None = None
-) -> ScmVersion | None:
-    archival = os.path.join(root, ".git_archival.txt")
-    data = data_from_mime(archival)
-    return archival_to_version(data, config=config)
+from __future__ import annotations
+
+import os
+import re
+import warnings
+from datetime import date
+from datetime import datetime
+from os.path import isfile
+from os.path import join
+from os.path import samefile
+from typing import Callable
+from typing import TYPE_CHECKING
+
+from .config import Configuration
+from .scm_workdir import Workdir
+from .utils import _CmdResult
+from .utils import data_from_mime
+from .utils import do_ex
+from .utils import require_command
+from .utils import trace
+from .version import meta
+from .version import ScmVersion
+from .version import tags_to_versions
+
+if TYPE_CHECKING:
+    from . import _types as _t
+
+    from setuptools_scm.hg_git import GitWorkdirHgClient
+
+REF_TAG_RE = re.compile(r"(?<=\btag: )([^,]+)\b")
+DESCRIBE_UNSUPPORTED = "%(describe"
+
+# If testing command in shell make sure to quote the match argument like
+# '*[0-9]*' as it will expand before being sent to git if there are any matching
+# files in current directory.
+DEFAULT_DESCRIBE = [
+    "git",
+    "describe",
+    "--dirty",
+    "--tags",
+    "--long",
+    "--match",
+    "*[0-9]*",
+]
+
+
+class GitWorkdir(Workdir):
+    """experimental, may change at any time"""
+
+    COMMAND = "git"
+
+    @classmethod
+    def from_potential_worktree(cls, wd: _t.PathT) -> GitWorkdir | None:
+        require_command(cls.COMMAND)
+        wd = os.path.abspath(wd)
+        git_dir = join(wd, ".git")
+        real_wd, _, ret = do_ex(
+            ["git", "--git-dir", git_dir, "rev-parse", "--show-prefix"], wd
+        )
+        real_wd = real_wd[:-1]  # remove the trailing pathsep
+        if ret:
+            return None
+        if not real_wd:
+            real_wd = wd
+        else:
+            assert wd.replace("\\", "/").endswith(real_wd)
+            # In windows wd contains ``\`` which should be replaced by ``/``
+            # for this assertion to work.  Length of string isn't changed by replace
+            # ``\\`` is just and escape for `\`
+            real_wd = wd[: -len(real_wd)]
+        trace("real root", real_wd)
+        if not samefile(real_wd, wd):
+            return None
+
+        return cls(real_wd)
+
+    def do_ex_git(self, cmd: list[str]) -> _CmdResult:
+        return self.do_ex(["git", "--git-dir", join(self.path, ".git")] + cmd)
+
+    def is_dirty(self) -> bool:
+        out, _, _ = self.do_ex_git(["status", "--porcelain", "--untracked-files=no"])
+        return bool(out)
+
+    def get_branch(self) -> str | None:
+        branch, err, ret = self.do_ex_git(["rev-parse", "--abbrev-ref", "HEAD"])
+        if ret:
+            trace("branch err", branch, err, ret)
+            branch, err, ret = self.do_ex_git(["symbolic-ref", "--short", "HEAD"])
+            if ret:
+                trace("branch err (symbolic-ref)", branch, err, ret)
+                return None
+        return branch
+
+    def get_head_date(self) -> date | None:
+        timestamp, err, ret = self.do_ex_git(
+            ["-c", "log.showSignature=false", "log", "-n", "1", "HEAD", "--format=%cI"]
+        )
+        if ret:
+            trace("timestamp err", timestamp, err, ret)
+            return None
+        # TODO, when dropping python3.6 use fromiso
+        date_part = timestamp.split("T")[0]
+        if "%c" in date_part:
+            trace("git too old -> timestamp is ", timestamp)
+            return None
+        return datetime.strptime(date_part, r"%Y-%m-%d").date()
+
+    def is_shallow(self) -> bool:
+        return isfile(join(self.path, ".git/shallow"))
+
+    def fetch_shallow(self) -> None:
+        self.do_ex_git(["fetch", "--unshallow"])
+
+    def node(self) -> str | None:
+        node, _, ret = self.do_ex_git(["rev-parse", "--verify", "--quiet", "HEAD"])
+        if not ret:
+            return node[:7]
+        else:
+            return None
+
+    def count_all_nodes(self) -> int:
+        revs, _, _ = self.do_ex_git(["rev-list", "HEAD"])
+        return revs.count("\n") + 1
+
+    def default_describe(self) -> _CmdResult:
+        git_dir = join(self.path, ".git")
+        return self.do_ex(
+            DEFAULT_DESCRIBE[:1] + ["--git-dir", git_dir] + DEFAULT_DESCRIBE[1:]
+        )
+
+
+def warn_on_shallow(wd: GitWorkdir) -> None:
+    """experimental, may change at any time"""
+    if wd.is_shallow():
+        warnings.warn(f'"{wd.path}" is shallow and may cause errors')
+
+
+def fetch_on_shallow(wd: GitWorkdir) -> None:
+    """experimental, may change at any time"""
+    if wd.is_shallow():
+        warnings.warn(f'"{wd.path}" was shallow, git fetch was used to rectify')
+        wd.fetch_shallow()
+
+
+def fail_on_shallow(wd: GitWorkdir) -> None:
+    """experimental, may change at any time"""
+    if wd.is_shallow():
+        raise ValueError(
+            f'{wd.path} is shallow, please correct with "git fetch --unshallow"'
+        )
+
+
+def get_working_directory(config: Configuration) -> GitWorkdir | None:
+    """
+    Return the working directory (``GitWorkdir``).
+    """
+
+    if config.parent:
+        return GitWorkdir.from_potential_worktree(config.parent)
+
+    if config.search_parent_directories:
+        return search_parent(config.absolute_root)
+
+    return GitWorkdir.from_potential_worktree(config.absolute_root)
+
+
+def parse(
+    root: str,
+    describe_command: str | list[str] | None = None,
+    pre_parse: Callable[[GitWorkdir], None] = warn_on_shallow,
+    config: Configuration | None = None,
+) -> ScmVersion | None:
+    """
+    :param pre_parse: experimental pre_parse action, may change at any time
+    """
+    if not config:
+        config = Configuration(root=root)
+
+    wd = get_working_directory(config)
+    if wd:
+        return _git_parse_inner(
+            config, wd, describe_command=describe_command, pre_parse=pre_parse
+        )
+    else:
+        return None
+
+
+def _git_parse_inner(
+    config: Configuration,
+    wd: GitWorkdir | GitWorkdirHgClient,
+    pre_parse: None | (Callable[[GitWorkdir | GitWorkdirHgClient], None]) = None,
+    describe_command: _t.CMD_TYPE | None = None,
+) -> ScmVersion:
+    if pre_parse:
+        pre_parse(wd)
+
+    if config.git_describe_command is not None:
+        describe_command = config.git_describe_command
+
+    if describe_command is not None:
+        out, _, ret = wd.do_ex(describe_command)
+    else:
+        out, _, ret = wd.default_describe()
+    distance: int | None
+    node: str | None
+    if ret == 0:
+        tag, distance, node, dirty = _git_parse_describe(out)
+        if distance == 0 and not dirty:
+            distance = None
+    else:
+        # If 'git git_describe_command' failed, try to get the information otherwise.
+        tag = "0.0"
+        node = wd.node()
+        if node is None:
+            distance = 0
+        else:
+            distance = wd.count_all_nodes()
+            node = "g" + node
+        dirty = wd.is_dirty()
+
+    branch = wd.get_branch()
+    node_date = wd.get_head_date() or date.today()
+
+    return meta(
+        tag,
+        branch=branch,
+        node=node,
+        node_date=node_date,
+        distance=distance,
+        dirty=dirty,
+        config=config,
+    )
+
+
+def _git_parse_describe(
+    describe_output: str,
+) -> tuple[str, int | None, str | None, bool]:
+    # 'describe_output' looks e.g. like 'v1.5.0-0-g4060507' or
+    # 'v1.15.1rc1-37-g9bd1298-dirty'.
+    # It may also just be a bare tag name if this is a tagged commit and we are
+    # parsing a .git_archival.txt file.
+
+    if describe_output.endswith("-dirty"):
+        dirty = True
+        describe_output = describe_output[:-6]
+    else:
+        dirty = False
+
+    split = describe_output.rsplit("-", 2)
+    if len(split) < 3:  # probably a tagged commit
+        tag = describe_output
+        number = None
+        node = None
+    else:
+        tag, number_, node = split
+        number = int(number_)
+    return tag, number, node, dirty
+
+
+def search_parent(dirname: _t.PathT) -> GitWorkdir | None:
+    """
+    Walk up the path to find the `.git` directory.
+    :param dirname: Directory from which to start searching.
+    """
+
+    # Code based on:
+    # https://github.com/gitpython-developers/GitPython/blob/main/git/repo/base.py
+
+    curpath = os.path.abspath(dirname)
+
+    while curpath:
+
+        try:
+            wd = GitWorkdir.from_potential_worktree(curpath)
+        except Exception:
+            wd = None
+
+        if wd is not None:
+            return wd
+
+        curpath, tail = os.path.split(curpath)
+
+        if not tail:
+            return None
+    return None
+
+
+def archival_to_version(
+    data: dict[str, str], config: Configuration | None = None
+) -> ScmVersion | None:
+    node: str | None
+    trace("data", data)
+    archival_describe = data.get("describe-name", DESCRIBE_UNSUPPORTED)
+    if DESCRIBE_UNSUPPORTED in archival_describe:
+        warnings.warn("git archive did not support describe output")
+    else:
+        tag, number, node, _ = _git_parse_describe(archival_describe)
+        return meta(
+            tag,
+            config=config,
+            distance=None if number == 0 else number,
+            node=node,
+        )
+    versions = tags_to_versions(REF_TAG_RE.findall(data.get("ref-names", "")))
+    if versions:
+        return meta(versions[0], config=config)
+    else:
+        node = data.get("node")
+        if node is None:
+            return None
+        elif "$FORMAT" in node.upper():
+            warnings.warn("unexported git archival found")
+            return None
+        else:
+            return meta("0.0", node=node, config=config)
+
+
+def parse_archival(
+    root: _t.PathT, config: Configuration | None = None
+) -> ScmVersion | None:
+    archival = os.path.join(root, ".git_archival.txt")
+    data = data_from_mime(archival)
+    return archival_to_version(data, config=config)
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/hg_git.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-from __future__ import annotations
-
-import os
-from contextlib import suppress
-from datetime import date
-from datetime import datetime
-
-from . import _types as _t
-from .git import GitWorkdir
-from .hg import HgWorkdir
-from .utils import _CmdResult
-from .utils import do_ex
-from .utils import require_command
-from .utils import trace
-
-
-_FAKE_GIT_DESCRIBE_ERROR = _CmdResult("<>hg git failed", "", 1)
-
-
-class GitWorkdirHgClient(GitWorkdir, HgWorkdir):
-    COMMAND = "hg"
-
-    @classmethod
-    def from_potential_worktree(cls, wd: _t.PathT) -> GitWorkdirHgClient | None:
-        require_command(cls.COMMAND)
-        root, _, ret = do_ex(["hg", "root"], wd)
-        if ret:
-            return None
-        return cls(root)
-
-    def is_dirty(self) -> bool:
-        out, _, _ = self.do_ex('hg id -T "{dirty}"')
-        return bool(out)
-
-    def get_branch(self) -> str | None:
-        res = self.do_ex('hg id -T "{bookmarks}"')
-        if res.returncode:
-            trace("branch err", res)
-            return None
-        return res.out
-
-    def get_head_date(self) -> date | None:
-        date_part, err, ret = self.do_ex('hg log -r . -T "{shortdate(date)}"')
-        if ret:
-            trace("head date err", date_part, err, ret)
-            return None
-        return datetime.strptime(date_part, r"%Y-%m-%d").date()
-
-    def is_shallow(self) -> bool:
-        return False
-
-    def fetch_shallow(self) -> None:
-        pass
-
-    def get_hg_node(self) -> str | None:
-        node, _, ret = self.do_ex('hg log -r . -T "{node}"')
-        if not ret:
-            return node
-        else:
-            return None
-
-    def _hg2git(self, hg_node: str) -> str | None:
-        with suppress(FileNotFoundError):
-            with open(os.path.join(self.path, ".hg/git-mapfile")) as map_items:
-                for item in map_items:
-                    if hg_node in item:
-                        git_node, hg_node = item.split()
-                        return git_node
-        return None
-
-    def node(self) -> str | None:
-        hg_node = self.get_hg_node()
-        if hg_node is None:
-            return None
-
-        git_node = self._hg2git(hg_node)
-
-        if git_node is None:
-            # trying again after hg -> git
-            self.do_ex("hg gexport")
-            git_node = self._hg2git(hg_node)
-
-            if git_node is None:
-                trace("Cannot get git node so we use hg node", hg_node)
-
-                if hg_node == "0" * len(hg_node):
-                    # mimic Git behavior
-                    return None
-
-                return hg_node
-
-        return git_node[:7]
-
-    def count_all_nodes(self) -> int:
-        revs, _, _ = self.do_ex(["hg", "log", "-r", "ancestors(.)", "-T", "."])
-        return len(revs)
-
-    def default_describe(self) -> _CmdResult:
-        """
-        Tentative to reproduce the output of
-
-        `git describe --dirty --tags --long --match *[0-9]*`
-
-        """
-        hg_tags_str, _, ret = self.do_ex(
-            [
-                "hg",
-                "log",
-                "-r",
-                "(reverse(ancestors(.)) and tag(r're:v?[0-9].*'))",
-                "-T",
-                "{tags}{if(tags, ' ', '')}",
-            ]
-        )
-        if ret:
-            return _FAKE_GIT_DESCRIBE_ERROR
-        hg_tags: list[str] = hg_tags_str.split()
-
-        if not hg_tags:
-            return _FAKE_GIT_DESCRIBE_ERROR
-
-        with open(os.path.join(self.path, ".hg/git-tags")) as fp:
-            git_tags: dict[str, str] = dict(line.split()[::-1] for line in fp)
-
-        tag: str
-        for hg_tag in hg_tags:
-            if hg_tag in git_tags:
-                tag = hg_tag
-                break
-        else:
-            trace("tag not found", hg_tags, git_tags)
-            return _FAKE_GIT_DESCRIBE_ERROR
-
-        out, _, ret = self.do_ex(["hg", "log", "-r", f"'{tag}'::.", "-T", "."])
-        if ret:
-            return _FAKE_GIT_DESCRIBE_ERROR
-        distance = len(out) - 1
-
-        node = self.node()
-        assert node is not None
-        desc = f"{tag}-{distance}-g{node}"
-
-        if self.is_dirty():
-            desc += "-dirty"
-        trace("desc", desc)
-        return _CmdResult(desc, "", 0)
+from __future__ import annotations
+
+import os
+from contextlib import suppress
+from datetime import date
+from datetime import datetime
+
+from . import _types as _t
+from .git import GitWorkdir
+from .hg import HgWorkdir
+from .utils import _CmdResult
+from .utils import do_ex
+from .utils import require_command
+from .utils import trace
+
+
+_FAKE_GIT_DESCRIBE_ERROR = _CmdResult("<>hg git failed", "", 1)
+
+
+class GitWorkdirHgClient(GitWorkdir, HgWorkdir):
+    COMMAND = "hg"
+
+    @classmethod
+    def from_potential_worktree(cls, wd: _t.PathT) -> GitWorkdirHgClient | None:
+        require_command(cls.COMMAND)
+        root, _, ret = do_ex(["hg", "root"], wd)
+        if ret:
+            return None
+        return cls(root)
+
+    def is_dirty(self) -> bool:
+        out, _, _ = self.do_ex('hg id -T "{dirty}"')
+        return bool(out)
+
+    def get_branch(self) -> str | None:
+        res = self.do_ex('hg id -T "{bookmarks}"')
+        if res.returncode:
+            trace("branch err", res)
+            return None
+        return res.out
+
+    def get_head_date(self) -> date | None:
+        date_part, err, ret = self.do_ex('hg log -r . -T "{shortdate(date)}"')
+        if ret:
+            trace("head date err", date_part, err, ret)
+            return None
+        return datetime.strptime(date_part, r"%Y-%m-%d").date()
+
+    def is_shallow(self) -> bool:
+        return False
+
+    def fetch_shallow(self) -> None:
+        pass
+
+    def get_hg_node(self) -> str | None:
+        node, _, ret = self.do_ex('hg log -r . -T "{node}"')
+        if not ret:
+            return node
+        else:
+            return None
+
+    def _hg2git(self, hg_node: str) -> str | None:
+        with suppress(FileNotFoundError):
+            with open(os.path.join(self.path, ".hg/git-mapfile")) as map_items:
+                for item in map_items:
+                    if hg_node in item:
+                        git_node, hg_node = item.split()
+                        return git_node
+        return None
+
+    def node(self) -> str | None:
+        hg_node = self.get_hg_node()
+        if hg_node is None:
+            return None
+
+        git_node = self._hg2git(hg_node)
+
+        if git_node is None:
+            # trying again after hg -> git
+            self.do_ex("hg gexport")
+            git_node = self._hg2git(hg_node)
+
+            if git_node is None:
+                trace("Cannot get git node so we use hg node", hg_node)
+
+                if hg_node == "0" * len(hg_node):
+                    # mimic Git behavior
+                    return None
+
+                return hg_node
+
+        return git_node[:7]
+
+    def count_all_nodes(self) -> int:
+        revs, _, _ = self.do_ex(["hg", "log", "-r", "ancestors(.)", "-T", "."])
+        return len(revs)
+
+    def default_describe(self) -> _CmdResult:
+        """
+        Tentative to reproduce the output of
+
+        `git describe --dirty --tags --long --match *[0-9]*`
+
+        """
+        hg_tags_str, _, ret = self.do_ex(
+            [
+                "hg",
+                "log",
+                "-r",
+                "(reverse(ancestors(.)) and tag(r're:v?[0-9].*'))",
+                "-T",
+                "{tags}{if(tags, ' ', '')}",
+            ]
+        )
+        if ret:
+            return _FAKE_GIT_DESCRIBE_ERROR
+        hg_tags: list[str] = hg_tags_str.split()
+
+        if not hg_tags:
+            return _FAKE_GIT_DESCRIBE_ERROR
+
+        with open(os.path.join(self.path, ".hg/git-tags")) as fp:
+            git_tags: dict[str, str] = dict(line.split()[::-1] for line in fp)
+
+        tag: str
+        for hg_tag in hg_tags:
+            if hg_tag in git_tags:
+                tag = hg_tag
+                break
+        else:
+            trace("tag not found", hg_tags, git_tags)
+            return _FAKE_GIT_DESCRIBE_ERROR
+
+        out, _, ret = self.do_ex(["hg", "log", "-r", f"'{tag}'::.", "-T", "."])
+        if ret:
+            return _FAKE_GIT_DESCRIBE_ERROR
+        distance = len(out) - 1
+
+        node = self.node()
+        assert node is not None
+        desc = f"{tag}-{distance}-g{node}"
+
+        if self.is_dirty():
+            desc += "-dirty"
+        trace("desc", desc)
+        return _CmdResult(desc, "", 0)
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/scm_workdir.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from __future__ import annotations
-
-from typing import ClassVar
-from typing import TYPE_CHECKING
-
-from .utils import _CmdResult
-from .utils import do
-from .utils import do_ex
-from .utils import require_command
-
-if TYPE_CHECKING:
-    from . import _types as _t
-
-
-class Workdir:
-    COMMAND: ClassVar[str]
-
-    def __init__(self, path: _t.PathT):
-        require_command(self.COMMAND)
-        self.path = path
-
-    def do_ex(self, cmd: _t.CMD_TYPE) -> _CmdResult:
-        return do_ex(cmd, cwd=self.path)
-
-    def do(self, cmd: _t.CMD_TYPE) -> str:
-        return do(cmd, cwd=self.path)
+from __future__ import annotations
+
+from typing import ClassVar
+from typing import TYPE_CHECKING
+
+from .utils import _CmdResult
+from .utils import do
+from .utils import do_ex
+from .utils import require_command
+
+if TYPE_CHECKING:
+    from . import _types as _t
+
+
+class Workdir:
+    COMMAND: ClassVar[str]
+
+    def __init__(self, path: _t.PathT):
+        require_command(self.COMMAND)
+        self.path = path
+
+    def do_ex(self, cmd: _t.CMD_TYPE) -> _CmdResult:
+        return do_ex(cmd, cwd=self.path)
+
+    def do(self, cmd: _t.CMD_TYPE) -> str:
+        return do(cmd, cwd=self.path)
```

### Comparing `hgutilities-1.0.8.6/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py` & `hgutilities-1.0.9/.eggs/setuptools_scm-7.1.0-py3.11.egg/setuptools_scm/utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-"""
-utils
-"""
-from __future__ import annotations
-
-import os
-import platform
-import shlex
-import subprocess
-import sys
-import textwrap
-import warnings
-from types import CodeType
-from types import FunctionType
-from typing import Iterator
-from typing import Mapping
-from typing import NamedTuple
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-
-    from . import _types as _t
-
-DEBUG = bool(os.environ.get("SETUPTOOLS_SCM_DEBUG"))
-IS_WINDOWS = platform.system() == "Windows"
-
-
-class _CmdResult(NamedTuple):
-    out: str
-    err: str
-    returncode: int
-
-
-def no_git_env(env: Mapping[str, str]) -> dict[str, str]:
-    # adapted from pre-commit
-    # Too many bugs dealing with environment variables and GIT:
-    # https://github.com/pre-commit/pre-commit/issues/300
-    # In git 2.6.3 (maybe others), git exports GIT_WORK_TREE while running
-    # pre-commit hooks
-    # In git 1.9.1 (maybe others), git exports GIT_DIR and GIT_INDEX_FILE
-    # while running pre-commit hooks in submodules.
-    # GIT_DIR: Causes git clone to clone wrong thing
-    # GIT_INDEX_FILE: Causes 'error invalid object ...' during commit
-    for k, v in env.items():
-        if k.startswith("GIT_"):
-            trace(k, v)
-    return {
-        k: v
-        for k, v in env.items()
-        if not k.startswith("GIT_")
-        or k in ("GIT_EXEC_PATH", "GIT_SSH", "GIT_SSH_COMMAND")
-    }
-
-
-def avoid_pip_isolation(env: Mapping[str, str]) -> dict[str, str]:
-    """
-    pip build isolation can break Mercurial
-    (see https://github.com/pypa/pip/issues/10635)
-
-    pip uses PYTHONNOUSERSITE and a path in PYTHONPATH containing "pip-build-env-".
-    """
-    new_env = {k: v for k, v in env.items() if k != "PYTHONNOUSERSITE"}
-    if "PYTHONPATH" not in new_env:
-        return new_env
-
-    new_env["PYTHONPATH"] = os.pathsep.join(
-        [
-            path
-            for path in new_env["PYTHONPATH"].split(os.pathsep)
-            if "pip-build-env-" not in path
-        ]
-    )
-    return new_env
-
-
-def trace(*k: object, indent: bool = False) -> None:
-    if DEBUG:
-        if indent and len(k) > 1:
-            k = (k[0],) + tuple(textwrap.indent(str(s), "    ") for s in k[1:])
-        print(*k, file=sys.stderr, flush=True)
-
-
-def ensure_stripped_str(str_or_bytes: str | bytes) -> str:
-    if isinstance(str_or_bytes, str):
-        return str_or_bytes.strip()
-    else:
-        return str_or_bytes.decode("utf-8", "surrogateescape").strip()
-
-
-def _run(cmd: _t.CMD_TYPE, cwd: _t.PathT) -> subprocess.CompletedProcess[str]:
-    return subprocess.run(
-        cmd,
-        capture_output=True,
-        cwd=str(cwd),
-        env=dict(
-            avoid_pip_isolation(no_git_env(os.environ)),
-            # os.environ,
-            # try to disable i18n
-            LC_ALL="C",
-            LANGUAGE="",
-            HGPLAIN="1",
-        ),
-        text=True,
-    )
-
-
-def do_ex(cmd: _t.CMD_TYPE, cwd: _t.PathT = ".") -> _CmdResult:
-    if not DEBUG or not isinstance(cmd, list):
-        cmd_4_trace = cmd
-    else:
-        # give better results than shlex.join in our cases
-        cmd_4_trace = " ".join(
-            [s if all(c not in s for c in " {[:") else f'"{s}"' for s in cmd]
-        )
-    trace("----\ncmd:\n", cmd_4_trace, indent=True)
-    trace(" in:", cwd)
-    if os.name == "posix" and not isinstance(cmd, (list, tuple)):
-        cmd = shlex.split(cmd)
-
-    res = _run(cmd, cwd)
-    if res.stdout:
-        trace("out:\n", res.stdout, indent=True)
-    if res.stderr:
-        trace("err:\n", res.stderr, indent=True)
-    if res.returncode:
-        trace("ret:", res.returncode)
-    return _CmdResult(
-        ensure_stripped_str(res.stdout), ensure_stripped_str(res.stderr), res.returncode
-    )
-
-
-def do(cmd: list[str] | str, cwd: str | _t.PathT = ".") -> str:
-    out, err, ret = do_ex(cmd, cwd)
-    if ret and not DEBUG:
-        print(err)
-    return out
-
-
-def data_from_mime(path: _t.PathT) -> dict[str, str]:
-    with open(path, encoding="utf-8") as fp:
-        content = fp.read()
-    trace("content", repr(content))
-    # the complex conditions come from reading pseudo-mime-messages
-    data = dict(x.split(": ", 1) for x in content.splitlines() if ": " in x)
-    trace("data", data)
-    return data
-
-
-def function_has_arg(fn: object | FunctionType, argname: str) -> bool:
-    assert isinstance(fn, FunctionType)
-    code: CodeType = fn.__code__
-    return argname in code.co_varnames
-
-
-def has_command(name: str, args: list[str] | None = None, warn: bool = True) -> bool:
-    try:
-        cmd = [name, "help"] if args is None else [name, *args]
-        p = _run(cmd, ".")
-    except OSError:
-        trace(*sys.exc_info())
-        res = False
-    else:
-        res = not p.returncode
-    if not res and warn:
-        warnings.warn("%r was not found" % name, category=RuntimeWarning)
-    return res
-
-
-def require_command(name: str) -> None:
-    if not has_command(name, warn=False):
-        raise OSError("%r was not found" % name)
-
-
-def iter_entry_points(
-    group: str, name: str | None = None
-) -> Iterator[_t.EntrypointProtocol]:
-
-    from ._entrypoints import iter_entry_points
-
-    return iter_entry_points(group, name)
+"""
+utils
+"""
+from __future__ import annotations
+
+import os
+import platform
+import shlex
+import subprocess
+import sys
+import textwrap
+import warnings
+from types import CodeType
+from types import FunctionType
+from typing import Iterator
+from typing import Mapping
+from typing import NamedTuple
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+
+    from . import _types as _t
+
+DEBUG = bool(os.environ.get("SETUPTOOLS_SCM_DEBUG"))
+IS_WINDOWS = platform.system() == "Windows"
+
+
+class _CmdResult(NamedTuple):
+    out: str
+    err: str
+    returncode: int
+
+
+def no_git_env(env: Mapping[str, str]) -> dict[str, str]:
+    # adapted from pre-commit
+    # Too many bugs dealing with environment variables and GIT:
+    # https://github.com/pre-commit/pre-commit/issues/300
+    # In git 2.6.3 (maybe others), git exports GIT_WORK_TREE while running
+    # pre-commit hooks
+    # In git 1.9.1 (maybe others), git exports GIT_DIR and GIT_INDEX_FILE
+    # while running pre-commit hooks in submodules.
+    # GIT_DIR: Causes git clone to clone wrong thing
+    # GIT_INDEX_FILE: Causes 'error invalid object ...' during commit
+    for k, v in env.items():
+        if k.startswith("GIT_"):
+            trace(k, v)
+    return {
+        k: v
+        for k, v in env.items()
+        if not k.startswith("GIT_")
+        or k in ("GIT_EXEC_PATH", "GIT_SSH", "GIT_SSH_COMMAND")
+    }
+
+
+def avoid_pip_isolation(env: Mapping[str, str]) -> dict[str, str]:
+    """
+    pip build isolation can break Mercurial
+    (see https://github.com/pypa/pip/issues/10635)
+
+    pip uses PYTHONNOUSERSITE and a path in PYTHONPATH containing "pip-build-env-".
+    """
+    new_env = {k: v for k, v in env.items() if k != "PYTHONNOUSERSITE"}
+    if "PYTHONPATH" not in new_env:
+        return new_env
+
+    new_env["PYTHONPATH"] = os.pathsep.join(
+        [
+            path
+            for path in new_env["PYTHONPATH"].split(os.pathsep)
+            if "pip-build-env-" not in path
+        ]
+    )
+    return new_env
+
+
+def trace(*k: object, indent: bool = False) -> None:
+    if DEBUG:
+        if indent and len(k) > 1:
+            k = (k[0],) + tuple(textwrap.indent(str(s), "    ") for s in k[1:])
+        print(*k, file=sys.stderr, flush=True)
+
+
+def ensure_stripped_str(str_or_bytes: str | bytes) -> str:
+    if isinstance(str_or_bytes, str):
+        return str_or_bytes.strip()
+    else:
+        return str_or_bytes.decode("utf-8", "surrogateescape").strip()
+
+
+def _run(cmd: _t.CMD_TYPE, cwd: _t.PathT) -> subprocess.CompletedProcess[str]:
+    return subprocess.run(
+        cmd,
+        capture_output=True,
+        cwd=str(cwd),
+        env=dict(
+            avoid_pip_isolation(no_git_env(os.environ)),
+            # os.environ,
+            # try to disable i18n
+            LC_ALL="C",
+            LANGUAGE="",
+            HGPLAIN="1",
+        ),
+        text=True,
+    )
+
+
+def do_ex(cmd: _t.CMD_TYPE, cwd: _t.PathT = ".") -> _CmdResult:
+    if not DEBUG or not isinstance(cmd, list):
+        cmd_4_trace = cmd
+    else:
+        # give better results than shlex.join in our cases
+        cmd_4_trace = " ".join(
+            [s if all(c not in s for c in " {[:") else f'"{s}"' for s in cmd]
+        )
+    trace("----\ncmd:\n", cmd_4_trace, indent=True)
+    trace(" in:", cwd)
+    if os.name == "posix" and not isinstance(cmd, (list, tuple)):
+        cmd = shlex.split(cmd)
+
+    res = _run(cmd, cwd)
+    if res.stdout:
+        trace("out:\n", res.stdout, indent=True)
+    if res.stderr:
+        trace("err:\n", res.stderr, indent=True)
+    if res.returncode:
+        trace("ret:", res.returncode)
+    return _CmdResult(
+        ensure_stripped_str(res.stdout), ensure_stripped_str(res.stderr), res.returncode
+    )
+
+
+def do(cmd: list[str] | str, cwd: str | _t.PathT = ".") -> str:
+    out, err, ret = do_ex(cmd, cwd)
+    if ret and not DEBUG:
+        print(err)
+    return out
+
+
+def data_from_mime(path: _t.PathT) -> dict[str, str]:
+    with open(path, encoding="utf-8") as fp:
+        content = fp.read()
+    trace("content", repr(content))
+    # the complex conditions come from reading pseudo-mime-messages
+    data = dict(x.split(": ", 1) for x in content.splitlines() if ": " in x)
+    trace("data", data)
+    return data
+
+
+def function_has_arg(fn: object | FunctionType, argname: str) -> bool:
+    assert isinstance(fn, FunctionType)
+    code: CodeType = fn.__code__
+    return argname in code.co_varnames
+
+
+def has_command(name: str, args: list[str] | None = None, warn: bool = True) -> bool:
+    try:
+        cmd = [name, "help"] if args is None else [name, *args]
+        p = _run(cmd, ".")
+    except OSError:
+        trace(*sys.exc_info())
+        res = False
+    else:
+        res = not p.returncode
+    if not res and warn:
+        warnings.warn("%r was not found" % name, category=RuntimeWarning)
+    return res
+
+
+def require_command(name: str) -> None:
+    if not has_command(name, warn=False):
+        raise OSError("%r was not found" % name)
+
+
+def iter_entry_points(
+    group: str, name: str | None = None
+) -> Iterator[_t.EntrypointProtocol]:
+
+    from ._entrypoints import iter_entry_points
+
+    return iter_entry_points(group, name)
```

### Comparing `hgutilities-1.0.8.6/LICENSE.md` & `hgutilities-1.0.9/LICENSE.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `hgutilities-1.0.8.6/PKG-INFO` & `hgutilities-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1
-Name: hgutilities
-Version: 1.0.8.6
-Summary: A triple of tools used for plotting, handling key-words, and utilities
-Author: Henry Ginn
-Author-email: <henryginn137@gmail.com>
-Keywords: python,matplotlib,plotting,default,keywords,utils
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-
-# HGUtilities
-This is a collection of useful tools I use regularly. There are three parts to this package:
-
-- Defaults: manages settings for classes that can be controlled easily from an interface.
-- Plotting: a front end for matplotlib to easily create subplots.
-- Utils: a collection of generally useful functions
-
-## Contents
-
-1. [Defaults](#defaults)
-1. [Plotting](#plotting)
-1. [Utils](#utils)
-1. [Development](#development)
-
-## Defaults
-
-### The Problem
-
-Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
-
-- To view all the defaults you need to go into the script itself
-- It is awkward to change the value of those variables from an interface
-- It is impossible to change the default values without digging into the code itself.
-- Passing in many arguments to functions is messy
-- Mutable default values need to be implemented more carefully
-
-Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
-
-In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
-
-### The Solution
-
-For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
-
-Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
-
-    from hgutilities import defaults
-
-    class MyClass():
-
-        def __init__(self, **kwargs):
-            defaults.kwargs(self, **kwargs)
-
-    defaults.load(MyClass)
-
-We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
-
-The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
-
-## Plotting
-
-For full documentation, see the specific README inside the "plotting" module folder.
-
-When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
-
-The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
-
-It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
-
-## Utils
-
-The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
-
-## Development
-
-### Features and functionality to add in V1.1
-
-- automatic prefixing to axes
-- more control over subplot placement
-- automatic paragraph organisation for documentation
-- better distribution of subplots over multiple figures
-- control over tick labels
-- horizontal bar charts
-- better file extension handling for Defaults package
-- inherit function should be able to take in a single attribute as a non-iterable
-- animations need to be made compatible with more plot types
-- add README to defaults subpackage
+Metadata-Version: 2.1
+Name: hgutilities
+Version: 1.0.9
+Summary: A triple of tools used for plotting, handling key-words, and utilities
+Author: Henry Ginn
+Author-email: <henryginn137@gmail.com>
+Keywords: python,matplotlib,plotting,default,keywords,utils
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+
+# HGUtilities
+This is a collection of useful tools I use regularly. There are three parts to this package:
+
+- Defaults: manages settings for classes that can be controlled easily from an interface.
+- Plotting: a front end for matplotlib to easily create subplots.
+- Utils: a collection of generally useful functions
+
+## Contents
+
+1. [Defaults](#defaults)
+1. [Plotting](#plotting)
+1. [Utils](#utils)
+1. [Development](#development)
+
+## Defaults
+
+### The Problem
+
+Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
+
+- To view all the defaults you need to go into the script itself
+- It is awkward to change the value of those variables from an interface
+- It is impossible to change the default values without digging into the code itself.
+- Passing in many arguments to functions is messy
+- Mutable default values need to be implemented more carefully
+
+Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
+
+In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
+
+### The Solution
+
+For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
+
+Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
+
+    from hgutilities import defaults
+
+    class MyClass():
+
+        def __init__(self, **kwargs):
+            defaults.kwargs(self, **kwargs)
+
+    defaults.load(MyClass)
+
+We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
+
+The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
+
+## Plotting
+
+For full documentation, see the specific README inside the "plotting" module folder.
+
+When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
+
+The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
+
+It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
+
+## Utils
+
+The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
+
+## Development
+
+### Features and functionality to add in V1.1
+
+- automatic prefixing to axes
+- more control over subplot placement
+- automatic paragraph organisation for documentation
+- better distribution of subplots over multiple figures
+- control over tick labels
+- horizontal bar charts
+- better file extension handling for Defaults package
+- inherit function should be able to take in a single attribute as a non-iterable
+- animations need to be made compatible with more plot types
+- add README to defaults subpackage
```

### Comparing `hgutilities-1.0.8.6/README.md` & `hgutilities-1.0.9/README.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-# HGUtilities
-This is a collection of useful tools I use regularly. There are three parts to this package:
-
-- Defaults: manages settings for classes that can be controlled easily from an interface.
-- Plotting: a front end for matplotlib to easily create subplots.
-- Utils: a collection of generally useful functions
-
-## Contents
-
-1. [Defaults](#defaults)
-1. [Plotting](#plotting)
-1. [Utils](#utils)
-1. [Development](#development)
-
-## Defaults
-
-### The Problem
-
-Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
-
-- To view all the defaults you need to go into the script itself
-- It is awkward to change the value of those variables from an interface
-- It is impossible to change the default values without digging into the code itself.
-- Passing in many arguments to functions is messy
-- Mutable default values need to be implemented more carefully
-
-Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
-
-In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
-
-### The Solution
-
-For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
-
-Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
-
-    from hgutilities import defaults
-
-    class MyClass():
-
-        def __init__(self, **kwargs):
-            defaults.kwargs(self, **kwargs)
-
-    defaults.load(MyClass)
-
-We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
-
-The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
-
-## Plotting
-
-For full documentation, see the specific README inside the "plotting" module folder.
-
-When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
-
-The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
-
-It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
-
-## Utils
-
-The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
-
-## Development
-
-### Features and functionality to add in V1.1
-
-- automatic prefixing to axes
-- more control over subplot placement
-- automatic paragraph organisation for documentation
-- better distribution of subplots over multiple figures
-- control over tick labels
-- horizontal bar charts
-- better file extension handling for Defaults package
-- inherit function should be able to take in a single attribute as a non-iterable
-- animations need to be made compatible with more plot types
+# HGUtilities
+This is a collection of useful tools I use regularly. There are three parts to this package:
+
+- Defaults: manages settings for classes that can be controlled easily from an interface.
+- Plotting: a front end for matplotlib to easily create subplots.
+- Utils: a collection of generally useful functions
+
+## Contents
+
+1. [Defaults](#defaults)
+1. [Plotting](#plotting)
+1. [Utils](#utils)
+1. [Development](#development)
+
+## Defaults
+
+### The Problem
+
+Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
+
+- To view all the defaults you need to go into the script itself
+- It is awkward to change the value of those variables from an interface
+- It is impossible to change the default values without digging into the code itself.
+- Passing in many arguments to functions is messy
+- Mutable default values need to be implemented more carefully
+
+Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
+
+In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
+
+### The Solution
+
+For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
+
+Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
+
+    from hgutilities import defaults
+
+    class MyClass():
+
+        def __init__(self, **kwargs):
+            defaults.kwargs(self, **kwargs)
+
+    defaults.load(MyClass)
+
+We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
+
+The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
+
+## Plotting
+
+For full documentation, see the specific README inside the "plotting" module folder.
+
+When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
+
+The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
+
+It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
+
+## Utils
+
+The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
+
+## Development
+
+### Features and functionality to add in V1.1
+
+- automatic prefixing to axes
+- more control over subplot placement
+- automatic paragraph organisation for documentation
+- better distribution of subplots over multiple figures
+- control over tick labels
+- horizontal bar charts
+- better file extension handling for Defaults package
+- inherit function should be able to take in a single attribute as a non-iterable
+- animations need to be made compatible with more plot types
 - add README to defaults subpackage
```

### Comparing `hgutilities-1.0.8.6/hgutilities/Documentation/hgutilities.txt` & `hgutilities-1.0.9/hgutilities/Documentation/hgutilities.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-This is a collection of useful tools I use regularly.
-
-There are three parts to this package:
-
-- Defaults: manages settings for classes that can be controlled easily from an interface.
-- Plotting: a front end for matplotlib to easily create subplots.
-- Utils: a collection of generally useful functions
-
-Defaults:
-This part of the package aims to make passing in keyword value pairs into classes easier. A list of keywords with their default values are stored in files and are loaded in upon creation of the class. When keywords are passed into a class, they can be fed into this sub-package along with the object instance where they are processed. Classes also inherit default values from parent classes. Tools for documentation and inheriting attributes from one object to another are also included.
-
-Plotting:
-When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of the plotting part of the package is to make the creation of such figures easier.
-
-Utils:
-The aim of the utils part of this package is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed and it has been left undocumented. Where suitable spellings and names are consistent with matplotlib.
-
-For further documentation see the following:
-hgutils.defaults, hgutils.plotting
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+This is a collection of useful tools I use regularly.
+
+There are three parts to this package:
+
+- Defaults: manages settings for classes that can be controlled easily from an interface.
+- Plotting: a front end for matplotlib to easily create subplots.
+- Utils: a collection of generally useful functions
+
+Defaults:
+This part of the package aims to make passing in keyword value pairs into classes easier. A list of keywords with their default values are stored in files and are loaded in upon creation of the class. When keywords are passed into a class, they can be fed into this sub-package along with the object instance where they are processed. Classes also inherit default values from parent classes. Tools for documentation and inheriting attributes from one object to another are also included.
+
+Plotting:
+When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of the plotting part of the package is to make the creation of such figures easier.
+
+Utils:
+The aim of the utils part of this package is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed and it has been left undocumented. Where suitable spellings and names are consistent with matplotlib.
+
+For further documentation see the following:
+hgutils.defaults, hgutils.plotting
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.8.6/hgutilities/defaults/Documentation/docs.txt` & `hgutilities-1.0.9/hgutilities/defaults/Documentation/docs.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-The purpose of this function is to prevent bloated doc strings
-at the start of modules, classes, and functions by storing the
-doc strings in text files.
-
-By placing "defaults.docs()" in a package __init__.py file, all the
-modules, classes, and functions that were imported within that file
-that are part of the package will have their doc strings set. The
-doc strings are set from text files stored in folders called
-"Documentation", and these folders are in the same directory as
-the script for the corresponding module, class, or function.
-
-For further documentation see the following:
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
+The purpose of this function is to prevent bloated doc strings
+at the start of modules, classes, and functions by storing the
+doc strings in text files.
+
+By placing "defaults.docs()" in a package __init__.py file, all the
+modules, classes, and functions that were imported within that file
+that are part of the package will have their doc strings set. The
+doc strings are set from text files stored in folders called
+"Documentation", and these folders are in the same directory as
+the script for the corresponding module, class, or function.
+
+For further documentation see the following:
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
```

### Comparing `hgutilities-1.0.8.6/hgutilities/defaults/Documentation/loaddefaults.txt` & `hgutilities-1.0.9/hgutilities/defaults/Documentation/loaddefaults.txt`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Load
-
-Takes key-word value pairs in a json file and sets them as
-class attributes. The file will have the same name as the class
-and should be located in a folder called "Default Settings" in
-the same folder as the script where the class is defined.
-
-After a class, (e.g. "MyClass") has been defined, calling
-"Defaults.load(MyClass)" will load from the file if it exists.
-
-Any keyword-value pairs defined in parent classes will be
-inherited.
-
-For further documentation see the following:
-kwargs
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
+Load
+
+Takes key-word value pairs in a json file and sets them as
+class attributes. The file will have the same name as the class
+and should be located in a folder called "Default Settings" in
+the same folder as the script where the class is defined.
+
+After a class, (e.g. "MyClass") has been defined, calling
+"Defaults.load(MyClass)" will load from the file if it exists.
+
+Any keyword-value pairs defined in parent classes will be
+inherited.
+
+For further documentation see the following:
+kwargs
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
```

### Comparing `hgutilities-1.0.8.6/hgutilities/defaults/Documentation/processkwargs.txt` & `hgutilities-1.0.9/hgutilities/defaults/Documentation/processkwargs.txt`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Allows the user to easily set the key-words passed in to classes
-as object attributes.
-
-Calling "defaults.kwargs(self, **kwargs)" or
-"defaults.kwargs(self, kwargs)" will take any key-word value pairs
-in the kwargs dict and assign them as object variables. If these
-key-words had default values set, they will be overruled by the new
-values passed in.
-
-For further documentation see the following:
-load, inherit
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
+Allows the user to easily set the key-words passed in to classes
+as object attributes.
+
+Calling "defaults.kwargs(self, **kwargs)" or
+"defaults.kwargs(self, kwargs)" will take any key-word value pairs
+in the kwargs dict and assign them as object variables. If these
+key-words had default values set, they will be overruled by the new
+values passed in.
+
+For further documentation see the following:
+load, inherit
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
```

### Comparing `hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/docs.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/defaults/__pycache__/docs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/defaults/docs.py` & `hgutilities-1.0.9/hgutilities/defaults/docs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/defaults/inherit.py` & `hgutilities-1.0.9/hgutilities/defaults/inherit.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/defaults/loaddefaults.py` & `hgutilities-1.0.9/hgutilities/defaults/loaddefaults.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/defaults/processkwargs.py` & `hgutilities-1.0.9/hgutilities/defaults/processkwargs.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/Default Settings/Figure.txt` & `hgutilities-1.0.9/hgutilities/plotting/Default Settings/Figure.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/Documentation/Animate.txt` & `hgutilities-1.0.9/hgutilities/plotting/Documentation/Animate.txt`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-A subclass of Figures, this is responsible for creating
-short animations.
-
-create_animations is an interface for this class.
-
-Takes in a list of Data objects. These are just like
-regular Data objects, but the dependent variable should
-instead be an iterable where each element gives the values
-for a single frame.
-
-Currently this is only implemented for Surface objects.
-
-Animate.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+A subclass of Figures, this is responsible for creating
+short animations.
+
+create_animations is an interface for this class.
+
+Takes in a list of Data objects. These are just like
+regular Data objects, but the dependent variable should
+instead be an iterable where each element gives the values
+for a single frame.
+
+Currently this is only implemented for Surface objects.
+
+Animate.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/Documentation/create_animations.txt` & `hgutilities-1.0.9/hgutilities/plotting/Documentation/create_animations.txt`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-This function will take in a list of data objects
-and produce an animation. These Data objects are just
-like regular Data objects, but the dependent variable
-should instead be an iterable where each element gives
-the values for a single frame.
-
-This is an interface for the Animate class, and to
-see a list of optional key-word arguments you can
-look at Animate.defaults, Figures.defaults and
-Figure.defaults.
-
-This also returns the Figures object produced if
-the user wants to work with it directly, but this
-is not encouraged, and should only be necessary if
-a feature has not been implemented.
-
-For further documentation see the following:
-Animate, Figures, and Data classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+This function will take in a list of data objects
+and produce an animation. These Data objects are just
+like regular Data objects, but the dependent variable
+should instead be an iterable where each element gives
+the values for a single frame.
+
+This is an interface for the Animate class, and to
+see a list of optional key-word arguments you can
+look at Animate.defaults, Figures.defaults and
+Figure.defaults.
+
+This also returns the Figures object produced if
+the user wants to work with it directly, but this
+is not encouraged, and should only be necessary if
+a feature has not been implemented.
+
+For further documentation see the following:
+Animate, Figures, and Data classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/Documentation/create_figures.txt` & `hgutilities-1.0.9/hgutilities/plotting/Documentation/create_figures.txt`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-This function will take in a list of data objects
-and produce a set of figures showing them.
-
-This is an interface for the Figures class, and to
-see a list of optional key-word arguments you can
-look at Figures.defaults and Figure.defaults.
-
-This also returns the Figures object produced if
-the user wants to work with it directly, but this
-is not encouraged, and should only be necessary if
-a feature has not been implemented.
-
-For further documentation see the following:
-Figures and Data classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+This function will take in a list of data objects
+and produce a set of figures showing them.
+
+This is an interface for the Figures class, and to
+see a list of optional key-word arguments you can
+look at Figures.defaults and Figure.defaults.
+
+This also returns the Figures object produced if
+the user wants to work with it directly, but this
+is not encouraged, and should only be necessary if
+a feature has not been implemented.
+
+For further documentation see the following:
+Figures and Data classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/Documentation/plotting.txt` & `hgutilities-1.0.9/hgutilities/plotting/Documentation/plotting.txt`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-This package is an interface for matplotlib and is designed to make
-creation and processing of figures with subplots easier. The data and
-settings are specified, and they are arranged on figures where the user
-can control the maximum number of subplots on each figure and prescribe
-a target aspect ratio. If the subplots do not fit on one figure, they
-will be spread over multiple figures. The number of figures is no more
-than the ceiling of the total number of plots divided by the maximum
-number of plots per figure.
-
-While this package offers a lot of flexibility, it is mainly intended for
-convenient production of figures. For publication quality plots, it is
-recommended that the full flexibility of matplotlib or other plotting
-packages should be used instead. This package performs best for purposes
-such as analysing data and making powerpoints to be shared among
-colleages and students.
-
-Functions defined here:
-
-create_figures
-create_animations
-
-For further documentation see the following:
-Data and Figures classes and functions from the above list
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Plotting
+This package is an interface for matplotlib and is designed to make
+creation and processing of figures with subplots easier. The data and
+settings are specified, and they are arranged on figures where the user
+can control the maximum number of subplots on each figure and prescribe
+a target aspect ratio. If the subplots do not fit on one figure, they
+will be spread over multiple figures. The number of figures is no more
+than the ceiling of the total number of plots divided by the maximum
+number of plots per figure.
+
+While this package offers a lot of flexibility, it is mainly intended for
+convenient production of figures. For publication quality plots, it is
+recommended that the full flexibility of matplotlib or other plotting
+packages should be used instead. This package performs best for purposes
+such as analysing data and making powerpoints to be shared among
+colleages and students.
+
+Functions defined here:
+
+create_figures
+create_animations
+
+For further documentation see the following:
+Data and Figures classes and functions from the above list
+https://github.com/HenryGinn/HGUtils
+https://github.com/HenryGinn/HGUtils/tree/main/Plotting
```

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/README.md` & `hgutilities-1.0.9/hgutilities/plotting/README.md`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/__init__.py` & `hgutilities-1.0.9/hgutilities/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/animate.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/__pycache__/animate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/figure.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/__pycache__/figure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/figures.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/__pycache__/figures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/__pycache__/quick.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/__pycache__/quick.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/animate.py` & `hgutilities-1.0.9/hgutilities/plotting/animate.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Data.txt` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/Data.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Line.txt` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/Line.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Default Settings/Surface.txt` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/Default Settings/Surface.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Bar.txt` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Bar.txt`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Contains information about a single data series on a bar chart.
-Anything that affects the entire chart should be specied upon creation
-of Bars objects. Almost all features of matplotlib bar charts are
-supported, and the key-word arguments are the same. Care must be
-taken to enter the key-word arguments in relevant object (Bars
-properties not entered into Bar properties and vice versa).
-
-Bar.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
+Contains information about a single data series on a bar chart.
+Anything that affects the entire chart should be specied upon creation
+of Bars objects. Almost all features of matplotlib bar charts are
+supported, and the key-word arguments are the same. Care must be
+taken to enter the key-word arguments in relevant object (Bars
+properties not entered into Bar properties and vice versa).
+
+Bar.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
```

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Bars.txt` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Bars.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-This is a subclass of Data used to create bar charts.
-It takes in a bar object, or an iterable of bar objects,
-and keyword arguments thar are relevant only to the entire
-plot. If you wanted every data series to be the same color,
-you would need to specify that for each bar object, but if
-you wanted a log scale, you would specify that at this level.
-If it does not make sense for two distinct data series to
-have different values for a property, then it should be a
-property of this object. For more detail, look at the
-default values for Bars and Bar objects.
-
-Bars.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Bar, Data, and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
+This is a subclass of Data used to create bar charts.
+It takes in a bar object, or an iterable of bar objects,
+and keyword arguments thar are relevant only to the entire
+plot. If you wanted every data series to be the same color,
+you would need to specify that for each bar object, but if
+you wanted a log scale, you would specify that at this level.
+If it does not make sense for two distinct data series to
+have different values for a property, then it should be a
+property of this object. For more detail, look at the
+default values for Bars and Bar objects.
+
+Bars.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Bar, Data, and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
```

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Line.txt` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Line.txt`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Contains information about a single data series
-on a line or scatter graph. Anything that affects
-the entire chart should be specified upon creation
-of Lines objects. Properties such as line color,
-line style, line thickness, and errors in x or y
-should be specified here.If a line is given a label
-then this label will be used in the chart legend.
-
-Line.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Lines, Data, and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+Contains information about a single data series
+on a line or scatter graph. Anything that affects
+the entire chart should be specified upon creation
+of Lines objects. Properties such as line color,
+line style, line thickness, and errors in x or y
+should be specified here.If a line is given a label
+then this label will be used in the chart legend.
+
+Line.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Lines, Data, and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
```

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Lines.txt` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Lines.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-This is used to create line and scatter graphs and takes in a Line
-object or an iterable of line objects. The scope of this object is the
-entire plot, and data about individual lines should be specified by
-Line objects. Properties such as whether the plot has a legend, what
-the title and axis labels are, and the plot type are relevant at this
-level. If it does not make sense for two distinct data series to have
-different values for a property, then it should be a property of this
-object. For more detail, look at the default values for Lines and Line objects.
-
-The plot_type key-word controls which matplotlib plotting function is
-used to create the plot. The options are "plot", "semilogx", "semilogy",
-"loglog", "scatter", and "errorbar". If values for xerr and yerr are
-given for any line object, this will not be detected. The keyword
-plot_type="errorbar" needs to be passed in explicitily.
-
-lines.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Line, Data, and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+This is used to create line and scatter graphs and takes in a Line
+object or an iterable of line objects. The scope of this object is the
+entire plot, and data about individual lines should be specified by
+Line objects. Properties such as whether the plot has a legend, what
+the title and axis labels are, and the plot type are relevant at this
+level. If it does not make sense for two distinct data series to have
+different values for a property, then it should be a property of this
+object. For more detail, look at the default values for Lines and Line objects.
+
+The plot_type key-word controls which matplotlib plotting function is
+used to create the plot. The options are "plot", "semilogx", "semilogy",
+"loglog", "scatter", and "errorbar". If values for xerr and yerr are
+given for any line object, this will not be detected. The keyword
+plot_type="errorbar" needs to be passed in explicitily.
+
+lines.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Line, Data, and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
```

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Pie.txt` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Pie.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-This is a Data subclass used to create pie charts. A pie chart can only
-display one data series, and so this takes in a list of values and
-labels directly unlike the Lines and Bars classes. Almost all
-matplotlib pie chart keyword arguments are accepted, and information
-about the plot legend should also be passed in, either upon creation
-or set directly.
-
-Pie.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Data and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.pie.html
+This is a Data subclass used to create pie charts. A pie chart can only
+display one data series, and so this takes in a list of values and
+labels directly unlike the Lines and Bars classes. Almost all
+matplotlib pie chart keyword arguments are accepted, and information
+about the plot legend should also be passed in, either upon creation
+or set directly.
+
+Pie.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Data and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.pie.html
```

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/Documentation/Surface.txt` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/Documentation/Surface.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-This is a Data subclass used to create surfaces in 3D. It takes in x, y, and z values, all of which are 2D arrays of the same shape. Only one data series can be shown on each plot. All keyword arguments are the same as the matplotlib keyword arguments. This accepts the following arguments for the plot_type keyword, all of which are the names of the corresponding matplotlib plotting function:
-
-plot_surface: standard surface plotter
-plot_wireframe: shows the surface as a wire frame
-contour: shows the level sets of a function
-
-Surface.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Data and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.mplot3d.axes3d.Axes3D.plot_surface.html
+This is a Data subclass used to create surfaces in 3D. It takes in x, y, and z values, all of which are 2D arrays of the same shape. Only one data series can be shown on each plot. All keyword arguments are the same as the matplotlib keyword arguments. This accepts the following arguments for the plot_type keyword, all of which are the names of the corresponding matplotlib plotting function:
+
+plot_surface: standard surface plotter
+plot_wireframe: shows the surface as a wire frame
+contour: shows the level sets of a function
+
+Surface.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Data and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.mplot3d.axes3d.Axes3D.plot_surface.html
```

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/bars.py` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/bars.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/colorplot.py` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/colorplot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/lines.py` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/lines.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/datatypes/surface.py` & `hgutilities-1.0.9/hgutilities/plotting/datatypes/surface.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/figure.py` & `hgutilities-1.0.9/hgutilities/plotting/figure.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/figures.py` & `hgutilities-1.0.9/hgutilities/plotting/figures.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plotfunctions.py` & `hgutilities-1.0.9/hgutilities/plotting/plotfunctions.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plot.py` & `hgutilities-1.0.9/hgutilities/plotting/plottypes/plot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotbars.py` & `hgutilities-1.0.9/hgutilities/plotting/plottypes/plotbars.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotcolorplot.py` & `hgutilities-1.0.9/hgutilities/plotting/plottypes/plotcolorplot.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotlines.py` & `hgutilities-1.0.9/hgutilities/plotting/plottypes/plotlines.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotpie.py` & `hgutilities-1.0.9/hgutilities/plotting/plottypes/plotpie.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plottypes/plotsurface.py` & `hgutilities-1.0.9/hgutilities/plotting/plottypes/plotsurface.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/figuresize.py` & `hgutilities-1.0.9/hgutilities/plotting/plotutils/figuresize.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/griddimensions.py` & `hgutilities-1.0.9/hgutilities/plotting/plotutils/griddimensions.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/plotshape.py` & `hgutilities-1.0.9/hgutilities/plotting/plotutils/plotshape.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/plotting/plotutils/savefigure.py` & `hgutilities-1.0.9/hgutilities/plotting/plotutils/savefigure.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/utils/__pycache__/groups.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/utils/__pycache__/groups.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/utils/__pycache__/paths.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/utils/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/utils/__pycache__/readwrite.cpython-310.pyc` & `hgutilities-1.0.9/hgutilities/utils/__pycache__/readwrite.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/utils/filenames.py` & `hgutilities-1.0.9/hgutilities/utils/filenames.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities/utils/paths.py` & `hgutilities-1.0.9/hgutilities/utils/paths.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import os
-import json
-
-def make_file(file_path):
-    if not os.path.exists(file_path):
-        folder_path = os.path.split(file_path)[0]
-        make_folder(folder_path)
-        make_empty_file(file_path)
-
-def make_empty_file(file_path):
-    with open(file_path, "w") as file:
-        pass
-
-def make_folder(folder_path):
-    if not os.path.exists(folder_path):
-        parent_folder_path = os.path.split(folder_path)[0]
-        make_folder(parent_folder_path)
-        os.mkdir(folder_path)
-
-def make_folder_path(path):
-    if os.path.isfile(path):
-        path = os.path.split(path)[0]
-    make_file(path)
-
-def load_json(path, ignore_empty_or_none=True):
-    if ignore_empty_or_none:
-        if not os.path.exists(path) or os.stat(path).st_size == 0:
-            return {}
-    return do_load_json(path)
-
-def do_load_json(path):
-    with open(path, "r") as file:
-        file_contents = json.load(file)
-    return file_contents
+import os
+import json
+
+def make_file(file_path):
+    if not os.path.exists(file_path):
+        folder_path = os.path.split(file_path)[0]
+        make_folder(folder_path)
+        make_empty_file(file_path)
+
+def make_empty_file(file_path):
+    with open(file_path, "w") as file:
+        pass
+
+def make_folder(folder_path):
+    if not os.path.exists(folder_path):
+        parent_folder_path = os.path.split(folder_path)[0]
+        make_folder(parent_folder_path)
+        os.mkdir(folder_path)
+
+def make_folder_path(path):
+    if os.path.isfile(path):
+        path = os.path.split(path)[0]
+    make_file(path)
+
+def load_json(path, ignore_empty_or_none=True):
+    if ignore_empty_or_none:
+        if not os.path.exists(path) or os.stat(path).st_size == 0:
+            return {}
+    return do_load_json(path)
+
+def do_load_json(path):
+    with open(path, "r") as file:
+        file_contents = json.load(file)
+    return file_contents
```

### Comparing `hgutilities-1.0.8.6/hgutilities/utils/readwrite.py` & `hgutilities-1.0.9/hgutilities/utils/readwrite.py`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/hgutilities.egg-info/PKG-INFO` & `hgutilities-1.0.9/hgutilities.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1
-Name: hgutilities
-Version: 1.0.8.6
-Summary: A triple of tools used for plotting, handling key-words, and utilities
-Author: Henry Ginn
-Author-email: <henryginn137@gmail.com>
-Keywords: python,matplotlib,plotting,default,keywords,utils
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-
-# HGUtilities
-This is a collection of useful tools I use regularly. There are three parts to this package:
-
-- Defaults: manages settings for classes that can be controlled easily from an interface.
-- Plotting: a front end for matplotlib to easily create subplots.
-- Utils: a collection of generally useful functions
-
-## Contents
-
-1. [Defaults](#defaults)
-1. [Plotting](#plotting)
-1. [Utils](#utils)
-1. [Development](#development)
-
-## Defaults
-
-### The Problem
-
-Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
-
-- To view all the defaults you need to go into the script itself
-- It is awkward to change the value of those variables from an interface
-- It is impossible to change the default values without digging into the code itself.
-- Passing in many arguments to functions is messy
-- Mutable default values need to be implemented more carefully
-
-Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
-
-In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
-
-### The Solution
-
-For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
-
-Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
-
-    from hgutilities import defaults
-
-    class MyClass():
-
-        def __init__(self, **kwargs):
-            defaults.kwargs(self, **kwargs)
-
-    defaults.load(MyClass)
-
-We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
-
-The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
-
-## Plotting
-
-For full documentation, see the specific README inside the "plotting" module folder.
-
-When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
-
-The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
-
-It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
-
-## Utils
-
-The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
-
-## Development
-
-### Features and functionality to add in V1.1
-
-- automatic prefixing to axes
-- more control over subplot placement
-- automatic paragraph organisation for documentation
-- better distribution of subplots over multiple figures
-- control over tick labels
-- horizontal bar charts
-- better file extension handling for Defaults package
-- inherit function should be able to take in a single attribute as a non-iterable
-- animations need to be made compatible with more plot types
-- add README to defaults subpackage
+Metadata-Version: 2.1
+Name: hgutilities
+Version: 1.0.9
+Summary: A triple of tools used for plotting, handling key-words, and utilities
+Author: Henry Ginn
+Author-email: <henryginn137@gmail.com>
+Keywords: python,matplotlib,plotting,default,keywords,utils
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+
+# HGUtilities
+This is a collection of useful tools I use regularly. There are three parts to this package:
+
+- Defaults: manages settings for classes that can be controlled easily from an interface.
+- Plotting: a front end for matplotlib to easily create subplots.
+- Utils: a collection of generally useful functions
+
+## Contents
+
+1. [Defaults](#defaults)
+1. [Plotting](#plotting)
+1. [Utils](#utils)
+1. [Development](#development)
+
+## Defaults
+
+### The Problem
+
+Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
+
+- To view all the defaults you need to go into the script itself
+- It is awkward to change the value of those variables from an interface
+- It is impossible to change the default values without digging into the code itself.
+- Passing in many arguments to functions is messy
+- Mutable default values need to be implemented more carefully
+
+Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
+
+In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
+
+### The Solution
+
+For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
+
+Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
+
+    from hgutilities import defaults
+
+    class MyClass():
+
+        def __init__(self, **kwargs):
+            defaults.kwargs(self, **kwargs)
+
+    defaults.load(MyClass)
+
+We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
+
+The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
+
+## Plotting
+
+For full documentation, see the specific README inside the "plotting" module folder.
+
+When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
+
+The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
+
+It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
+
+## Utils
+
+The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
+
+## Development
+
+### Features and functionality to add in V1.1
+
+- automatic prefixing to axes
+- more control over subplot placement
+- automatic paragraph organisation for documentation
+- better distribution of subplots over multiple figures
+- control over tick labels
+- horizontal bar charts
+- better file extension handling for Defaults package
+- inherit function should be able to take in a single attribute as a non-iterable
+- animations need to be made compatible with more plot types
+- add README to defaults subpackage
```

### Comparing `hgutilities-1.0.8.6/hgutilities.egg-info/SOURCES.txt` & `hgutilities-1.0.9/hgutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hgutilities-1.0.8.6/setup.py` & `hgutilities-1.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from setuptools import setup, find_packages
-import codecs
-import os
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-VERSION = "1.0.8.6"
-DESCRIPTION = "A triple of tools used for plotting, handling key-words, and utilities"
-LONG_DESCRIPTION = ("Defaults: manages settings for classes that can be controlled easily from an interface.\n"
-                    "Plotting: a front end for matplotlib to easily create subplots.\n"
-                    "Utils: a collection of generally useful functions")
-
-# Setting up
-setup(
-    name="hgutilities",
-    version=VERSION,
-    author="Henry Ginn",
-    author_email="<henryginn137@gmail.com>",
-    description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
-    setup_requires=['setuptools_scm'],
-    include_package_data=True,
-    install_requires=["matplotlib", "numpy", "screeninfo", "pillow"],
-    keywords=["python", "matplotlib", "plotting", "default", "keywords", "utils"],
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Natural Language :: English",
-        "Operating System :: Unix",
-        "Operating System :: Microsoft :: Windows",
-    ]
-)
+from setuptools import setup, find_packages
+import codecs
+import os
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()
+
+VERSION = "1.0.9"
+DESCRIPTION = "A triple of tools used for plotting, handling key-words, and utilities"
+LONG_DESCRIPTION = ("Defaults: manages settings for classes that can be controlled easily from an interface.\n"
+                    "Plotting: a front end for matplotlib to easily create subplots.\n"
+                    "Utils: a collection of generally useful functions")
+
+# Setting up
+setup(
+    name="hgutilities",
+    version=VERSION,
+    author="Henry Ginn",
+    author_email="<henryginn137@gmail.com>",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=long_description,
+    setup_requires=['setuptools_scm'],
+    include_package_data=True,
+    install_requires=["matplotlib", "numpy", "screeninfo", "pillow"],
+    keywords=["python", "matplotlib", "plotting", "default", "keywords", "utils"],
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Natural Language :: English",
+        "Operating System :: Unix",
+        "Operating System :: Microsoft :: Windows",
+    ]
+)
```

