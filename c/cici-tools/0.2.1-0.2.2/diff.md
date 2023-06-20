# Comparing `tmp/cici-tools-0.2.1.tar.gz` & `tmp/cici-tools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cici-tools-0.2.1.tar", last modified: Tue Jun 20 10:38:00 2023, max compression
+gzip compressed data, was "cici-tools-0.2.2.tar", last modified: Tue Jun 20 10:42:41 2023, max compression
```

## Comparing `cici-tools-0.2.1.tar` & `cici-tools-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:38:00.101065 cici-tools-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-20 10:37:57.000000 cici-tools-0.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 10:37:57.000000 cici-tools-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2035 2023-06-20 10:38:00.101065 cici-tools-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-06-20 10:37:57.000000 cici-tools-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:38:00.098065 cici-tools-0.2.1/cici/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/__main__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:38:00.099065 cici-tools-0.2.1/cici/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1510 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/cli/build.py
--rwxrwxrwx   0 root         (0) root         (0)     3073 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/cli/bundle.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/cli/fmt.py
--rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/cli/update.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:38:00.099065 cici-tools-0.2.1/cici/providers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:38:00.100065 cici-tools-0.2.1/cici/providers/gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/providers/gitlab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/providers/gitlab/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     5002 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/providers/gitlab/converter.py
--rw-rw-rw-   0 root         (0) root         (0)     6415 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/providers/gitlab/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2973 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/providers/gitlab/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/providers/gitlab/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:38:00.100065 cici-tools-0.2.1/cici/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/schema/LICENSE.gitlab
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    70638 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/schema/gitlab-ci.json
--rw-rw-rw-   0 root         (0) root         (0)     1755 2023-06-20 10:37:57.000000 cici-tools-0.2.1/cici/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:38:00.101065 cici-tools-0.2.1/cici_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2035 2023-06-20 10:38:00.000000 cici-tools-0.2.1/cici_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-20 10:38:00.000000 cici-tools-0.2.1/cici_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 10:38:00.000000 cici-tools-0.2.1/cici_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-20 10:38:00.000000 cici-tools-0.2.1/cici_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-20 10:38:00.000000 cici-tools-0.2.1/cici_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-20 10:38:00.000000 cici-tools-0.2.1/cici_tools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-20 10:38:00.102065 cici-tools-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1360 2023-06-20 10:37:57.000000 cici-tools-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.809664 cici-tools-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-06-20 10:42:39.000000 cici-tools-0.2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-20 10:42:39.000000 cici-tools-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-06-20 10:42:41.809664 cici-tools-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2023-06-20 10:42:39.000000 cici-tools-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.805664 cici-tools-0.2.2/cici/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.806665 cici-tools-0.2.2/cici/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/cli/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     3073 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/cli/bundle.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/cli/fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3140 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/cli/update.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.806665 cici-tools-0.2.2/cici/providers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.807664 cici-tools-0.2.2/cici/providers/gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/gitlab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/gitlab/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/gitlab/converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6415 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/gitlab/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2973 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/gitlab/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/providers/gitlab/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.807664 cici-tools-0.2.2/cici/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/schema/LICENSE.gitlab
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    70638 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/schema/gitlab-ci.json
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2023-06-20 10:42:39.000000 cici-tools-0.2.2/cici/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:42:41.809664 cici-tools-0.2.2/cici_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-06-20 10:42:41.000000 cici-tools-0.2.2/cici_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-20 10:42:41.000000 cici-tools-0.2.2/cici_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 10:42:41.000000 cici-tools-0.2.2/cici_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-20 10:42:41.000000 cici-tools-0.2.2/cici_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-20 10:42:41.000000 cici-tools-0.2.2/cici_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-20 10:42:41.000000 cici-tools-0.2.2/cici_tools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-20 10:42:41.809664 cici-tools-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1360 2023-06-20 10:42:39.000000 cici-tools-0.2.2/setup.py
```

### Comparing `cici-tools-0.2.1/LICENSE` & `cici-tools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/PKG-INFO` & `cici-tools-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Power tools for CI/CD.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
@@ -23,15 +23,15 @@
 License-File: LICENSE
 
 # cici-tools
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
-[![pipeline status](https://img.shields.io/gitlab/pipeline-status/brettops/tools/cici?branch=main)](https://gitlab.com/brettops/tools/cici/-/commits/main)
+[![pipeline status](https://img.shields.io/gitlab/pipeline-status/brettops/tools/cici-tools?branch=main)](https://gitlab.com/brettops/tools/cici-tools/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![code style: black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)
 [![imports: isort](https://img.shields.io/badge/imports-isort-1674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 
 <!-- END BADGIE TIME -->
```

### Comparing `cici-tools-0.2.1/README.md` & `cici-tools-0.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # cici-tools
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
-[![pipeline status](https://img.shields.io/gitlab/pipeline-status/brettops/tools/cici?branch=main)](https://gitlab.com/brettops/tools/cici/-/commits/main)
+[![pipeline status](https://img.shields.io/gitlab/pipeline-status/brettops/tools/cici-tools?branch=main)](https://gitlab.com/brettops/tools/cici-tools/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![code style: black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)
 [![imports: isort](https://img.shields.io/badge/imports-isort-1674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 
 <!-- END BADGIE TIME -->
```

### Comparing `cici-tools-0.2.1/cici/cli/build.py` & `cici-tools-0.2.2/cici/cli/build.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici/cli/bundle.py` & `cici-tools-0.2.2/cici/cli/bundle.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici/cli/fmt.py` & `cici-tools-0.2.2/cici/cli/fmt.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici/cli/update.py` & `cici-tools-0.2.2/cici/cli/update.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici/constants.py` & `cici-tools-0.2.2/cici/constants.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici/providers/gitlab/constants.py` & `cici-tools-0.2.2/cici/providers/gitlab/constants.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici/providers/gitlab/converter.py` & `cici-tools-0.2.2/cici/providers/gitlab/converter.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici/providers/gitlab/models.py` & `cici-tools-0.2.2/cici/providers/gitlab/models.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici/providers/gitlab/serializers.py` & `cici-tools-0.2.2/cici/providers/gitlab/serializers.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici/providers/gitlab/utils.py` & `cici-tools-0.2.2/cici/providers/gitlab/utils.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici/schema/LICENSE.gitlab` & `cici-tools-0.2.2/cici/schema/LICENSE.gitlab`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici/schema/gitlab-ci.json` & `cici-tools-0.2.2/cici/schema/gitlab-ci.json`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici/utils.py` & `cici-tools-0.2.2/cici/utils.py`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/cici_tools.egg-info/PKG-INFO` & `cici-tools-0.2.2/cici_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cici-tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Power tools for CI/CD.
 Home-page: https://gitlab.com/brettops/tools/cici
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: ci pipeline python
 Platform: UNKNOWN
@@ -23,15 +23,15 @@
 License-File: LICENSE
 
 # cici-tools
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
-[![pipeline status](https://img.shields.io/gitlab/pipeline-status/brettops/tools/cici?branch=main)](https://gitlab.com/brettops/tools/cici/-/commits/main)
+[![pipeline status](https://img.shields.io/gitlab/pipeline-status/brettops/tools/cici-tools?branch=main)](https://gitlab.com/brettops/tools/cici-tools/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![code style: black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)
 [![imports: isort](https://img.shields.io/badge/imports-isort-1674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
 
 <!-- END BADGIE TIME -->
```

### Comparing `cici-tools-0.2.1/cici_tools.egg-info/SOURCES.txt` & `cici-tools-0.2.2/cici_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cici-tools-0.2.1/setup.py` & `cici-tools-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```

