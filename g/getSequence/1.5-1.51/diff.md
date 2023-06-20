# Comparing `tmp/getSequence-1.5.tar.gz` & `tmp/getSequence-1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getSequence-1.5.tar", last modified: Wed Jun 14 13:44:05 2023, max compression
+gzip compressed data, was "getSequence-1.51.tar", last modified: Tue Jun 20 15:21:00 2023, max compression
```

## Comparing `getSequence-1.5.tar` & `getSequence-1.51.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.760501 getSequence-1.5/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      257 2022-02-07 14:17:58.000000 getSequence-1.5/.codecov.yml
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.756073 getSequence-1.5/.github/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2257 2022-02-07 14:17:58.000000 getSequence-1.5/.github/CONTRIBUTING.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      224 2022-02-07 14:17:58.000000 getSequence-1.5/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.756172 getSequence-1.5/.github/workflows/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2049 2022-03-09 18:03:44.000000 getSequence-1.5/.github/workflows/CI.yaml
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1403 2023-06-14 13:39:19.000000 getSequence-1.5/.gitignore
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      328 2022-02-07 14:17:58.000000 getSequence-1.5/.lgtm.yml
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3556 2022-02-07 14:17:58.000000 getSequence-1.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1072 2022-02-07 14:17:58.000000 getSequence-1.5/LICENSE
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      145 2022-02-07 14:17:58.000000 getSequence-1.5/MANIFEST.in
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     6035 2023-06-14 13:44:05.760566 getSequence-1.5/PKG-INFO
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     5724 2022-07-08 16:41:31.000000 getSequence-1.5/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.756310 getSequence-1.5/devtools/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3518 2022-02-07 14:17:58.000000 getSequence-1.5/devtools/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.756439 getSequence-1.5/devtools/conda-envs/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      208 2022-02-07 14:17:58.000000 getSequence-1.5/devtools/conda-envs/test_env.yaml
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.756551 getSequence-1.5/devtools/legacy-miniconda-setup/
--rwxr-xr-x   0 ryanemenecker   (501) staff       (20)     1344 2022-02-07 14:17:58.000000 getSequence-1.5/devtools/legacy-miniconda-setup/before_install.sh
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.756653 getSequence-1.5/devtools/scripts/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3860 2022-02-07 14:17:58.000000 getSequence-1.5/devtools/scripts/create_conda_env.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.757285 getSequence-1.5/docs/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      608 2022-02-07 14:17:58.000000 getSequence-1.5/docs/Makefile
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      590 2022-02-07 14:17:58.000000 getSequence-1.5/docs/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.757396 getSequence-1.5/docs/_static/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      507 2022-02-07 14:17:58.000000 getSequence-1.5/docs/_static/README.md
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.757504 getSequence-1.5/docs/_templates/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      470 2022-02-07 14:17:58.000000 getSequence-1.5/docs/_templates/README.md
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     5343 2022-02-07 14:17:58.000000 getSequence-1.5/docs/conf.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1472 2022-03-09 18:25:45.000000 getSequence-1.5/docs/getting_started.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      536 2022-03-09 18:03:00.000000 getSequence-1.5/docs/index.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      779 2022-02-07 14:17:58.000000 getSequence-1.5/docs/make.bat
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.757724 getSequence-1.5/docs/usage/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     3433 2022-03-09 17:56:01.000000 getSequence-1.5/docs/usage/command-line.rst
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1620 2022-03-09 17:55:47.000000 getSequence-1.5/docs/usage/using-in-python.rst
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.760924 getSequence-1.5/getSequence/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      306 2022-03-09 17:44:54.000000 getSequence-1.5/getSequence/__init__.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      496 2023-06-14 13:44:05.760954 getSequence-1.5/getSequence/_version.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)   523827 2023-06-14 13:38:31.000000 getSequence-1.5/getSequence/get_sequence.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1681 2022-11-22 19:59:39.000000 getSequence-1.5/getSequence/getseq.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)       47 2022-03-09 16:51:05.000000 getSequence-1.5/getSequence/getsequence_exceptions.py
--rw-------   0 ryanemenecker   (501) staff       (20)  1154428 2022-11-22 16:52:54.000000 getSequence-1.5/getSequence/screenshot.png
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.760204 getSequence-1.5/getSequence/tests/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      113 2022-02-07 14:17:58.000000 getSequence-1.5/getSequence/tests/__init__.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      319 2022-02-07 14:17:58.000000 getSequence-1.5/getSequence/tests/test_getSequence.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     4366 2023-06-14 13:39:26.000000 getSequence-1.5/getSequence/vis_sequence.py
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.760012 getSequence-1.5/getSequence.egg-info/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     6035 2023-06-14 13:44:05.000000 getSequence-1.5/getSequence.egg-info/PKG-INFO
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1005 2023-06-14 13:44:05.000000 getSequence-1.5/getSequence.egg-info/SOURCES.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)        1 2023-06-14 13:44:05.000000 getSequence-1.5/getSequence.egg-info/dependency_links.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)       17 2023-06-14 13:44:05.000000 getSequence-1.5/getSequence.egg-info/requires.txt
--rw-r--r--   0 ryanemenecker   (501) staff       (20)       12 2023-06-14 13:44:05.000000 getSequence-1.5/getSequence.egg-info/top_level.txt
-drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-14 13:44:05.760413 getSequence-1.5/scripts/
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1460 2022-07-08 16:37:31.000000 getSequence-1.5/scripts/getseq
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     1342 2022-11-22 20:02:42.000000 getSequence-1.5/scripts/visseq
--rw-r--r--   0 ryanemenecker   (501) staff       (20)      360 2023-06-14 13:44:05.760796 getSequence-1.5/setup.cfg
--rw-r--r--   0 ryanemenecker   (501) staff       (20)     2299 2022-11-22 19:56:28.000000 getSequence-1.5/setup.py
--rw-r--r--   0 ryanemenecker   (501) staff       (20)    68611 2022-02-07 14:17:58.000000 getSequence-1.5/versioneer.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.160869 getSequence-1.51/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      257 2022-02-07 14:17:58.000000 getSequence-1.51/.codecov.yml
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.155893 getSequence-1.51/.github/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2257 2022-02-07 14:17:58.000000 getSequence-1.51/.github/CONTRIBUTING.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      224 2022-02-07 14:17:58.000000 getSequence-1.51/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.156033 getSequence-1.51/.github/workflows/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2049 2022-03-09 18:03:44.000000 getSequence-1.51/.github/workflows/CI.yaml
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1403 2023-06-14 13:39:19.000000 getSequence-1.51/.gitignore
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      328 2022-02-07 14:17:58.000000 getSequence-1.51/.lgtm.yml
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3556 2022-02-07 14:17:58.000000 getSequence-1.51/CODE_OF_CONDUCT.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1072 2022-02-07 14:17:58.000000 getSequence-1.51/LICENSE
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      145 2022-02-07 14:17:58.000000 getSequence-1.51/MANIFEST.in
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     6036 2023-06-20 15:21:00.160929 getSequence-1.51/PKG-INFO
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5724 2022-07-08 16:41:31.000000 getSequence-1.51/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.156276 getSequence-1.51/devtools/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3518 2022-02-07 14:17:58.000000 getSequence-1.51/devtools/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.156402 getSequence-1.51/devtools/conda-envs/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      208 2022-02-07 14:17:58.000000 getSequence-1.51/devtools/conda-envs/test_env.yaml
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.156553 getSequence-1.51/devtools/legacy-miniconda-setup/
+-rwxr-xr-x   0 ryanemenecker   (501) staff       (20)     1344 2022-02-07 14:17:58.000000 getSequence-1.51/devtools/legacy-miniconda-setup/before_install.sh
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.156698 getSequence-1.51/devtools/scripts/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3860 2022-02-07 14:17:58.000000 getSequence-1.51/devtools/scripts/create_conda_env.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.157582 getSequence-1.51/docs/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      608 2022-02-07 14:17:58.000000 getSequence-1.51/docs/Makefile
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      590 2022-02-07 14:17:58.000000 getSequence-1.51/docs/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.157738 getSequence-1.51/docs/_static/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      507 2022-02-07 14:17:58.000000 getSequence-1.51/docs/_static/README.md
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.157881 getSequence-1.51/docs/_templates/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      470 2022-02-07 14:17:58.000000 getSequence-1.51/docs/_templates/README.md
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     5343 2022-02-07 14:17:58.000000 getSequence-1.51/docs/conf.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1472 2022-03-09 18:25:45.000000 getSequence-1.51/docs/getting_started.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      536 2022-03-09 18:03:00.000000 getSequence-1.51/docs/index.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      779 2022-02-07 14:17:58.000000 getSequence-1.51/docs/make.bat
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.158184 getSequence-1.51/docs/usage/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     3433 2022-03-09 17:56:01.000000 getSequence-1.51/docs/usage/command-line.rst
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1620 2022-03-09 17:55:47.000000 getSequence-1.51/docs/usage/using-in-python.rst
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.161283 getSequence-1.51/getSequence/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      306 2022-03-09 17:44:54.000000 getSequence-1.51/getSequence/__init__.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      497 2023-06-20 15:21:00.161314 getSequence-1.51/getSequence/_version.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)   523968 2023-06-20 15:18:03.000000 getSequence-1.51/getSequence/get_sequence.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1681 2023-06-20 15:18:01.000000 getSequence-1.51/getSequence/getseq.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)       47 2022-03-09 16:51:05.000000 getSequence-1.51/getSequence/getsequence_exceptions.py
+-rw-------   0 ryanemenecker   (501) staff       (20)  1154428 2022-11-22 16:52:54.000000 getSequence-1.51/getSequence/screenshot.png
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.160565 getSequence-1.51/getSequence/tests/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      113 2022-02-07 14:17:58.000000 getSequence-1.51/getSequence/tests/__init__.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      319 2022-02-07 14:17:58.000000 getSequence-1.51/getSequence/tests/test_getSequence.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     4366 2023-06-14 13:39:26.000000 getSequence-1.51/getSequence/vis_sequence.py
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.160326 getSequence-1.51/getSequence.egg-info/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     6036 2023-06-20 15:21:00.000000 getSequence-1.51/getSequence.egg-info/PKG-INFO
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1005 2023-06-20 15:21:00.000000 getSequence-1.51/getSequence.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)        1 2023-06-20 15:21:00.000000 getSequence-1.51/getSequence.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)       17 2023-06-20 15:21:00.000000 getSequence-1.51/getSequence.egg-info/requires.txt
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)       12 2023-06-20 15:21:00.000000 getSequence-1.51/getSequence.egg-info/top_level.txt
+drwxr-xr-x   0 ryanemenecker   (501) staff       (20)        0 2023-06-20 15:21:00.160784 getSequence-1.51/scripts/
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1460 2022-07-08 16:37:31.000000 getSequence-1.51/scripts/getseq
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     1342 2022-11-22 20:02:42.000000 getSequence-1.51/scripts/visseq
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)      360 2023-06-20 15:21:00.161157 getSequence-1.51/setup.cfg
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)     2299 2022-11-22 19:56:28.000000 getSequence-1.51/setup.py
+-rw-r--r--   0 ryanemenecker   (501) staff       (20)    68611 2022-02-07 14:17:58.000000 getSequence-1.51/versioneer.py
```

### Comparing `getSequence-1.5/.github/CONTRIBUTING.md` & `getSequence-1.51/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/.github/workflows/CI.yaml` & `getSequence-1.51/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/.gitignore` & `getSequence-1.51/.gitignore`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/CODE_OF_CONDUCT.md` & `getSequence-1.51/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/LICENSE` & `getSequence-1.51/LICENSE`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/PKG-INFO` & `getSequence-1.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getSequence
-Version: 1.5
+Version: 1.51
 Summary: A CLI to get a uniprot sequence returned to terminal
 Home-page: UNKNOWN
 Author: Ryan Emenecker
 Author-email: remenecker@wustl.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

### Comparing `getSequence-1.5/README.md` & `getSequence-1.51/README.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/devtools/README.md` & `getSequence-1.51/devtools/README.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/devtools/legacy-miniconda-setup/before_install.sh` & `getSequence-1.51/devtools/legacy-miniconda-setup/before_install.sh`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/devtools/scripts/create_conda_env.py` & `getSequence-1.51/devtools/scripts/create_conda_env.py`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/docs/Makefile` & `getSequence-1.51/docs/Makefile`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/docs/README.md` & `getSequence-1.51/docs/README.md`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/docs/conf.py` & `getSequence-1.51/docs/conf.py`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/docs/getting_started.rst` & `getSequence-1.51/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/docs/index.rst` & `getSequence-1.51/docs/index.rst`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/docs/make.bat` & `getSequence-1.51/docs/make.bat`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/docs/usage/command-line.rst` & `getSequence-1.51/docs/usage/command-line.rst`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/docs/usage/using-in-python.rst` & `getSequence-1.51/docs/usage/using-in-python.rst`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/getSequence/get_sequence.py` & `getSequence-1.51/getSequence/get_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,17 @@
     '''
 
     # first format name into a url
     # uses only reviewed on first attempt.
     split_name = name.split(' ')
     if len(split_name) == 1:
         use_url=f'https://rest.uniprot.org/uniprotkb/search?size=15&format=fasta&query={split_name[0]}%20AND%20%28reviewed%3Atrue%29'
+        top_five = requests.get(use_url).text
+        query_keywords=split_name[0]
+        
     else:
         # format the search string.
         split_name = parse_input(name)
         # if you don't have a taxid, you're hitting the 'feeling lucky' button on early 2000s Google more or less TBH.
         add_vals = split_name['gene_info']
         query_keywords = split_name['gene_info']
         add_str = ''
@@ -102,22 +105,24 @@
             top_five = requests.get(use_url).text
             if top_five == '':
                 # do unreviewed.
                 use_url = f"https://rest.uniprot.org/uniprotkb/search?format=fasta&size=15&query={add_str}%20AND%20%28reviewed%3Afalse%29%20AND%20%28organism_id%3A{split_name['taxid']}%29"
                 top_five = requests.get(use_url).text    
 
     # if using org id before, take out and try agian.
-    if split_name['taxid']!='':
-        if top_five == '':
-            use_url = f'https://rest.uniprot.org/uniprotkb/search?format=fasta&size=15&query={add_str}%20AND%20%28reviewed%3Afalse%29'
-            top_five = requests.get(use_url).text
+    if type(split_name)==dict:
+        if split_name['taxid']!='':
+            if top_five == '':
+                use_url = f'https://rest.uniprot.org/uniprotkb/search?format=fasta&size=15&query={add_str}%20AND%20%28reviewed%3Afalse%29'
+                top_five = requests.get(use_url).text
 
     if top_five == '':
         raise Exception('Unable to find sequence.')
 
+
     # header placeholder
     header = ''
     final_vals = []
     # now try to get right fasta
     fastas_split = top_five.split('>')[1:]
     
     most_matches = 0
@@ -159,14 +164,15 @@
                 temp_seq=''
                 most_matches = cur_matches
                 for chars in split_by_lines[1:]:
                     temp_seq+=chars
                 best_seq = temp_seq
                 final_vals = [header, best_seq]
     
+
     if final_vals != []:
         return final_vals
 
     else:
         seq_to_use = fastas_split[0]
         split_by_lines = seq_to_use.split('\n')
         header = split_by_lines[0].lower()
```

### Comparing `getSequence-1.5/getSequence/getseq.py` & `getSequence-1.51/getSequence/getseq.py`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/getSequence/screenshot.png` & `getSequence-1.51/getSequence/screenshot.png`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/getSequence/vis_sequence.py` & `getSequence-1.51/getSequence/vis_sequence.py`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/getSequence.egg-info/PKG-INFO` & `getSequence-1.51/getSequence.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getSequence
-Version: 1.5
+Version: 1.51
 Summary: A CLI to get a uniprot sequence returned to terminal
 Home-page: UNKNOWN
 Author: Ryan Emenecker
 Author-email: remenecker@wustl.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.5
```

### Comparing `getSequence-1.5/getSequence.egg-info/SOURCES.txt` & `getSequence-1.51/getSequence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/scripts/getseq` & `getSequence-1.51/scripts/getseq`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/scripts/visseq` & `getSequence-1.51/scripts/visseq`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/setup.py` & `getSequence-1.51/setup.py`

 * *Files identical despite different names*

### Comparing `getSequence-1.5/versioneer.py` & `getSequence-1.51/versioneer.py`

 * *Files identical despite different names*

