# Comparing `tmp/cici.tools-0.1.4.tar.gz` & `tmp/cici-tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cici.tools-0.1.4.tar", last modified: Sun Jun 11 18:08:44 2023, max compression
+gzip compressed data, was "cici-tools-0.2.0.tar", last modified: Tue Jun 20 10:26:15 2023, max compression
```

## Comparing `cici.tools-0.1.4.tar` & `cici-tools-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.898304 cici.tools-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-11 18:08:42.000000 cici.tools-0.1.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-11 18:08:42.000000 cici.tools-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6232 2023-06-11 18:08:44.898304 cici.tools-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5401 2023-06-11 18:08:42.000000 cici.tools-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.895300 cici.tools-0.1.4/cici/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/__main__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.896302 cici.tools-0.1.4/cici/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/cli/build.py
--rwxrwxrwx   0 root         (0) root         (0)     7260 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/cli/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/cli/update.py
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.897303 cici.tools-0.1.4/cici/providers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.897303 cici.tools-0.1.4/cici/providers/brettops/
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/providers/brettops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/providers/brettops/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1645 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/providers/brettops/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1502 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/providers/brettops/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     4868 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/providers/gitlab.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.898304 cici.tools-0.1.4/cici/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/schema/LICENSE.gitlab
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    70638 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/schema/gitlab-ci.json
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-06-11 18:08:42.000000 cici.tools-0.1.4/cici/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 18:08:44.896302 cici.tools-0.1.4/cici.tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6232 2023-06-11 18:08:44.000000 cici.tools-0.1.4/cici.tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-11 18:08:44.000000 cici.tools-0.1.4/cici.tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 18:08:44.000000 cici.tools-0.1.4/cici.tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-11 18:08:44.000000 cici.tools-0.1.4/cici.tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-11 18:08:44.000000 cici.tools-0.1.4/cici.tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-11 18:08:44.000000 cici.tools-0.1.4/cici.tools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-11 18:08:44.899306 cici.tools-0.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1358 2023-06-11 18:08:42.000000 cici.tools-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:26:15.802510 cici-tools-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-20 10:26:13.000000 cici-tools-0.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 10:26:13.000000 cici-tools-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-06-20 10:26:15.802510 cici-tools-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-06-20 10:26:13.000000 cici-tools-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:26:15.798510 cici-tools-0.2.0/cici/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:26:15.799510 cici-tools-0.2.0/cici/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/cli/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     3073 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/cli/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/cli/fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/cli/update.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:26:15.799510 cici-tools-0.2.0/cici/providers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:26:15.800510 cici-tools-0.2.0/cici/providers/gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/providers/gitlab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/providers/gitlab/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/providers/gitlab/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6415 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/providers/gitlab/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2973 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/providers/gitlab/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/providers/gitlab/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:26:15.801510 cici-tools-0.2.0/cici/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/schema/LICENSE.gitlab
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    70638 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/schema/gitlab-ci.json
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2023-06-20 10:26:13.000000 cici-tools-0.2.0/cici/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:26:15.802510 cici-tools-0.2.0/cici_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-06-20 10:26:15.000000 cici-tools-0.2.0/cici_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-20 10:26:15.000000 cici-tools-0.2.0/cici_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 10:26:15.000000 cici-tools-0.2.0/cici_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-20 10:26:15.000000 cici-tools-0.2.0/cici_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-20 10:26:15.000000 cici-tools-0.2.0/cici_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-20 10:26:15.000000 cici-tools-0.2.0/cici_tools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-20 10:26:15.803510 cici-tools-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1360 2023-06-20 10:26:13.000000 cici-tools-0.2.0/setup.py
```

### Comparing `cici.tools-0.1.4/LICENSE` & `cici-tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.4/cici/cli/update.py` & `cici-tools-0.2.0/cici/cli/update.py`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.4/cici/schema/LICENSE.gitlab` & `cici-tools-0.2.0/cici/schema/LICENSE.gitlab`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.4/cici/schema/gitlab-ci.json` & `cici-tools-0.2.0/cici/schema/gitlab-ci.json`

 * *Files identical despite different names*

### Comparing `cici.tools-0.1.4/cici/utils.py` & `cici-tools-0.2.0/cici/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import typing
+from typing import Any, Union
 
 from ruamel.yaml.scalarstring import (
     DoubleQuotedScalarString,
     FoldedScalarString,
     PreservedScalarString,
 )
 
@@ -34,13 +34,27 @@
     elif len(line) >= 80:
         return FoldedScalarString(line)
     elif quote:
         return DoubleQuotedScalarString(line)
     return line
 
 
-def make_quoted_scalar_string(line):
+def make_quoted_string(line):
     return make_scalar_string(line, quote=True)
 
 
-def make_scalar_list(value: list[str]) -> list[typing.Any]:
+def make_scalar_list(value: list[str]) -> list[Any]:
     return [make_scalar_string(line) for line in value]
+
+
+def make_quoted_list(value: list[str]) -> list[Any]:
+    return [make_scalar_string(line, quote=True) for line in value]
+
+
+def make_quoted_list_or_string(object: Union[str, list[str]]) -> list[Any]:
+    if isinstance(object, str):
+        return make_quoted_string(object)
+    return make_quoted_list(object)
+
+
+def make_quoted_dict(object):
+    return {key: make_quoted_string(value) for key, value in object.items()}
```

### Comparing `cici.tools-0.1.4/setup.py` & `cici-tools-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.1.4"
+__version__ = "0.2.0"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
 
 setup(
-    name="cici.tools",
+    name="cici-tools",
     version=__version__,
     author="Brett Weir",
     author_email="brett@brettops.io",
-    description="CI pipeline toolkit.",
+    description="Power tools for CI/CD.",
     license="MIT",
     url="https://gitlab.com/brettops/tools/cici",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
     entry_points={
```

