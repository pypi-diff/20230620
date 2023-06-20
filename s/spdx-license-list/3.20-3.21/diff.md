# Comparing `tmp/spdx_license_list-3.20.tar.gz` & `tmp/spdx_license_list-3.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdx_license_list-3.20.tar", max compression
+gzip compressed data, was "spdx_license_list-3.21.tar", max compression
```

## Comparing `spdx_license_list-3.20.tar` & `spdx_license_list-3.21.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-02-21 02:23:03.820845 spdx_license_list-3.20/LICENSE
--rw-r--r--   0        0        0     1869 2023-02-21 02:23:03.820845 spdx_license_list-3.20/README.md
--rw-r--r--   0        0        0     1170 2023-02-21 02:24:40.499743 spdx_license_list-3.20/pyproject.toml
--rw-r--r--   0        0        0   103102 2023-02-21 02:23:44.806062 spdx_license_list-3.20/src/spdx_license_list/__init__.py
--rw-r--r--   0        0        0        0 2023-02-21 02:23:03.820845 spdx_license_list-3.20/src/spdx_license_list/py.tpyed
--rw-r--r--   0        0        0     2537 1970-01-01 00:00:00.000000 spdx_license_list-3.20/setup.py
--rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 spdx_license_list-3.20/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-20 04:45:02.012886 spdx_license_list-3.21/LICENSE
+-rw-r--r--   0        0        0     1869 2023-06-20 04:45:02.012886 spdx_license_list-3.21/README.md
+-rw-r--r--   0        0        0     1170 2023-06-20 04:46:56.689565 spdx_license_list-3.21/pyproject.toml
+-rw-r--r--   0        0        0   107189 2023-06-20 04:45:47.668359 spdx_license_list-3.21/src/spdx_license_list/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 04:45:02.016886 spdx_license_list-3.21/src/spdx_license_list/py.tpyed
+-rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 spdx_license_list-3.21/PKG-INFO
```

### Comparing `spdx_license_list-3.20/LICENSE` & `spdx_license_list-3.21/LICENSE`

 * *Files identical despite different names*

### Comparing `spdx_license_list-3.20/README.md` & `spdx_license_list-3.21/README.md`

 * *Files identical despite different names*

### Comparing `spdx_license_list-3.20/pyproject.toml` & `spdx_license_list-3.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -43,11 +43,11 @@
     "Typing :: Typed",
 ]
 description = "SPDX License List as a Python dictionary"
 license = "MIT"
 name = "spdx-license-list"
 readme = "README.md"
 repository = "https://github.com/JJMC89/spdx-license-list"
-version = "3.20"
+version = "3.21"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `spdx_license_list-3.20/src/spdx_license_list/__init__.py` & `spdx_license_list-3.21/src/spdx_license_list/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,28 @@
     "Artistic-2.0": License(
         id="Artistic-2.0",
         name="Artistic License 2.0",
         deprecated_id=False,
         fsf_libre=True,
         osi_approved=True,
     ),
+    "ASWF-Digital-Assets-1.0": License(
+        id="ASWF-Digital-Assets-1.0",
+        name="ASWF Digital Assets License version 1.0",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
+    "ASWF-Digital-Assets-1.1": License(
+        id="ASWF-Digital-Assets-1.1",
+        name="ASWF Digital Assets License 1.1",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "Baekmuk": License(
         id="Baekmuk",
         name="Baekmuk License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -361,14 +375,21 @@
     "BlueOak-1.0.0": License(
         id="BlueOak-1.0.0",
         name="Blue Oak Model License 1.0.0",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "Boehm-GC": License(
+        id="Boehm-GC",
+        name="Boehm-Demers-Weiser GC License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "Borceux": License(
         id="Borceux",
         name="Borceux license",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -949,14 +970,21 @@
     "CC-BY-SA-3.0-DE": License(
         id="CC-BY-SA-3.0-DE",
         name="Creative Commons Attribution Share Alike 3.0 Germany",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "CC-BY-SA-3.0-IGO": License(
+        id="CC-BY-SA-3.0-IGO",
+        name="Creative Commons Attribution-ShareAlike 3.0 IGO",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "CC-BY-SA-4.0": License(
         id="CC-BY-SA-4.0",
         name="Creative Commons Attribution Share Alike 4.0 International",
         deprecated_id=False,
         fsf_libre=True,
         osi_approved=False,
     ),
@@ -1292,14 +1320,21 @@
     "DSDP": License(
         id="DSDP",
         name="DSDP License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "dtoa": License(
+        id="dtoa",
+        name="David M. Gay dtoa License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "dvipdfm": License(
         id="dvipdfm",
         name="dvipdfm License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -1483,15 +1518,15 @@
         name="FSF Unlimited License (with License Retention)",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
     "FSFULLRWD": License(
         id="FSFULLRWD",
-        name="FSF Unlimited License (With License Retention    and Warranty Disclaimer)",
+        name="FSF Unlimited License (With License Retention and Warranty Disclaimer)",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
     "FTL": License(
         id="FTL",
         name="Freetype Project License",
@@ -1964,14 +1999,21 @@
     "Info-ZIP": License(
         id="Info-ZIP",
         name="Info-ZIP License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "Inner-Net-2.0": License(
+        id="Inner-Net-2.0",
+        name="Inner Net License v2.0",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "Intel": License(
         id="Intel",
         name="Intel Open Source License",
         deprecated_id=False,
         fsf_libre=True,
         osi_approved=True,
     ),
@@ -2076,14 +2118,21 @@
     "Latex2e": License(
         id="Latex2e",
         name="Latex2e License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "Latex2e-translated-notice": License(
+        id="Latex2e-translated-notice",
+        name="Latex2e with translated notice permission",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "Leptonica": License(
         id="Leptonica",
         name="Leptonica License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -2230,21 +2279,42 @@
     "LiLiQ-Rplus-1.1": License(
         id="LiLiQ-Rplus-1.1",
         name="Licence Libre du Québec – Réciprocité forte version 1.1",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=True,
     ),
+    "Linux-man-pages-1-para": License(
+        id="Linux-man-pages-1-para",
+        name="Linux man-pages - 1 paragraph",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "Linux-man-pages-copyleft": License(
         id="Linux-man-pages-copyleft",
         name="Linux man-pages Copyleft",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "Linux-man-pages-copyleft-2-para": License(
+        id="Linux-man-pages-copyleft-2-para",
+        name="Linux man-pages Copyleft - 2 paragraphs",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
+    "Linux-man-pages-copyleft-var": License(
+        id="Linux-man-pages-copyleft-var",
+        name="Linux man-pages Copyleft Variant",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "Linux-OpenIB": License(
         id="Linux-OpenIB",
         name="Linux Kernel Variant of OpenIB.org license",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -2328,14 +2398,21 @@
     "Martin-Birgmeier": License(
         id="Martin-Birgmeier",
         name="Martin Birgmeier License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "metamail": License(
+        id="metamail",
+        name="metamail License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "Minpack": License(
         id="Minpack",
         name="Minpack License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -2384,14 +2461,21 @@
     "MIT-feh": License(
         id="MIT-feh",
         name="feh License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "MIT-Festival": License(
+        id="MIT-Festival",
+        name="MIT Festival Variant",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "MIT-Modern-Variant": License(
         id="MIT-Modern-Variant",
         name="MIT License Modern Variant",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=True,
     ),
@@ -2615,14 +2699,21 @@
     "NIST-PD-fallback": License(
         id="NIST-PD-fallback",
         name="NIST Public Domain Notice with license fallback",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "NIST-Software": License(
+        id="NIST-Software",
+        name="NIST Software License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "NLOD-1.0": License(
         id="NLOD-1.0",
         name="Norwegian Licence for Open Government Data (NLOD) 1.0",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -2951,14 +3042,21 @@
     "OLDAP-2.8": License(
         id="OLDAP-2.8",
         name="Open LDAP Public License v2.8",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=True,
     ),
+    "OLFL-1.3": License(
+        id="OLFL-1.3",
+        name="Open Logistics Foundation License Version 1.3",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=True,
+    ),
     "OML": License(
         id="OML",
         name="Open Market License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -2979,14 +3077,21 @@
     "OPL-1.0": License(
         id="OPL-1.0",
         name="Open Public License v1.0",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "OPL-UK-3.0": License(
+        id="OPL-UK-3.0",
+        name="United    Kingdom Open Parliament Licence v3.0",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "OPUBL-1.0": License(
         id="OPUBL-1.0",
         name="Open Publication License v1.0",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -3266,14 +3371,21 @@
     "SGI-B-2.0": License(
         id="SGI-B-2.0",
         name="SGI Free Software License B v2.0",
         deprecated_id=False,
         fsf_libre=True,
         osi_approved=False,
     ),
+    "SGP4": License(
+        id="SGP4",
+        name="SGP4 Permission Notice",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "SHL-0.5": License(
         id="SHL-0.5",
         name="Solderpad Hardware License v0.5",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -3441,14 +3553,21 @@
     "TCP-wrappers": License(
         id="TCP-wrappers",
         name="TCP Wrappers License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "TermReadKey": License(
+        id="TermReadKey",
+        name="TermReadKey License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "TMate": License(
         id="TMate",
         name="TMate Open Source License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -3532,14 +3651,21 @@
     "Unicode-TOU": License(
         id="Unicode-TOU",
         name="Unicode Terms of Use",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "UnixCrypt": License(
+        id="UnixCrypt",
+        name="UnixCrypt License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "Unlicense": License(
         id="Unlicense",
         name="The Unlicense",
         deprecated_id=False,
         fsf_libre=True,
         osi_approved=True,
     ),
@@ -3602,14 +3728,21 @@
     "Watcom-1.0": License(
         id="Watcom-1.0",
         name="Sybase Open Watcom Public License 1.0",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=True,
     ),
+    "Widget-Workshop": License(
+        id="Widget-Workshop",
+        name="Widget Workshop License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "Wsuipa": License(
         id="Wsuipa",
         name="Wsuipa License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
@@ -3637,21 +3770,35 @@
     "X11-distribute-modifications-variant": License(
         id="X11-distribute-modifications-variant",
         name="X11 License Distribution Modification Variant",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "Xdebug-1.03": License(
+        id="Xdebug-1.03",
+        name="Xdebug License v 1.03",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "Xerox": License(
         id="Xerox",
         name="Xerox License",
         deprecated_id=False,
         fsf_libre=False,
         osi_approved=False,
     ),
+    "Xfig": License(
+        id="Xfig",
+        name="Xfig License",
+        deprecated_id=False,
+        fsf_libre=False,
+        osi_approved=False,
+    ),
     "XFree86-1.1": License(
         id="XFree86-1.1",
         name="XFree86 License 1.1",
         deprecated_id=False,
         fsf_libre=True,
         osi_approved=False,
     ),
```

### Comparing `spdx_license_list-3.20/setup.py` & `spdx_license_list-3.21/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,55 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: spdx-license-list
+Version: 3.21
+Summary: SPDX License List as a Python dictionary
+Home-page: https://github.com/JJMC89/spdx-license-list
+License: MIT
+Author: JJMC89
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Typing :: Typed
+Project-URL: Repository, https://github.com/JJMC89/spdx-license-list
+Description-Content-Type: text/markdown
+
+[![Latest PyPI release](https://img.shields.io/pypi/v/spdx-license-list?logo=pypi)](https://pypi.org/project/spdx-license-list) ![Latest GitHub release](https://img.shields.io/github/v/release/JJMC89/spdx-license-list?logo=github) ![Latest tag](https://img.shields.io/github/v/tag/JJMC89/spdx-license-list?logo=git)
+
+![License](https://img.shields.io/pypi/l/spdx-license-list?color=blue) ![Python versions](https://img.shields.io/pypi/pyversions/spdx-license-list?logo=python)
+
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/JJMC89/spdx-license-list/main.svg)](https://results.pre-commit.ci/latest/github/JJMC89/pywikibot-extensions/main)
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+# SPDX License List
+
+Provides the SPDX License List as a Python dictionary
+
+Data source: [spdx/license-list-data](https://github.com/spdx/license-list-data)
+
+Designed as a replacement for [Michael Pöhn's spdx-license-list](https://gitlab.com/uniqx/spdx-license-list) but does not have the same API
+
+## Installation
+
+```console
+pip install spdx-license-list
+```
+
+## API
+
+`spdx_license_list.LICENSES` is a dictionary of all the licenses.
+
+The dictionary uses the identifier (**id**) as the keys, and the values are (typed) named tuples with the following attributes:
+- **id** (*str*) - short identifier to identify a match to licenses in the context of an SPDX file, a source file, or elsewhere
+- **name** (*str*) - full name that should be the title found in the license file or consistent with naming from other well-known sources
+- **deprecated_id** (*bool*) - idendifier is deprecated
+- **fsf_libre** (*bool*) - license is [listed as free by the FSF](https://www.gnu.org/licenses/license-list.en.html)
+- **osi_approved** (*bool*) - license is [OSI-approved](https://opensource.org/licenses)
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['spdx_license_list']
-
-package_data = \
-{'': ['*']}
-
-setup_kwargs = {
-    'name': 'spdx-license-list',
-    'version': '3.20',
-    'description': 'SPDX License List as a Python dictionary',
-    'long_description': "[![Latest PyPI release](https://img.shields.io/pypi/v/spdx-license-list?logo=pypi)](https://pypi.org/project/spdx-license-list) ![Latest GitHub release](https://img.shields.io/github/v/release/JJMC89/spdx-license-list?logo=github) ![Latest tag](https://img.shields.io/github/v/tag/JJMC89/spdx-license-list?logo=git)\n\n![License](https://img.shields.io/pypi/l/spdx-license-list?color=blue) ![Python versions](https://img.shields.io/pypi/pyversions/spdx-license-list?logo=python)\n\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/JJMC89/spdx-license-list/main.svg)](https://results.pre-commit.ci/latest/github/JJMC89/pywikibot-extensions/main)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# SPDX License List\n\nProvides the SPDX License List as a Python dictionary\n\nData source: [spdx/license-list-data](https://github.com/spdx/license-list-data)\n\nDesigned as a replacement for [Michael Pöhn's spdx-license-list](https://gitlab.com/uniqx/spdx-license-list) but does not have the same API\n\n## Installation\n\n```console\npip install spdx-license-list\n```\n\n## API\n\n`spdx_license_list.LICENSES` is a dictionary of all the licenses.\n\nThe dictionary uses the identifier (**id**) as the keys, and the values are (typed) named tuples with the following attributes:\n- **id** (*str*) - short identifier to identify a match to licenses in the context of an SPDX file, a source file, or elsewhere\n- **name** (*str*) - full name that should be the title found in the license file or consistent with naming from other well-known sources\n- **deprecated_id** (*bool*) - idendifier is deprecated\n- **fsf_libre** (*bool*) - license is [listed as free by the FSF](https://www.gnu.org/licenses/license-list.en.html)\n- **osi_approved** (*bool*) - license is [OSI-approved](https://opensource.org/licenses)\n",
-    'author': 'JJMC89',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/JJMC89/spdx-license-list',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

