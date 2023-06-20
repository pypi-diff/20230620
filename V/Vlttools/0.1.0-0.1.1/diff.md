# Comparing `tmp/Vlttools-0.1.0.tar.gz` & `tmp/Vlttools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\work\tools\vlttools\dist\.tmp-qq4q73pz\Vlttools-0.1.0.tar", last modified: Tue May 30 08:30:13 2023, max compression
+gzip compressed data, was "C:\work\tools\p600_tools\dist\.tmp-lf3pd948\Vlttools-0.1.1.tar", last modified: Tue Jun 20 03:53:43 2023, max compression
```

## Comparing `Vlttools-0.1.0.tar` & `Vlttools-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 08:30:13.810939 Vlttools-0.1.0/
--rw-rw-rw-   0        0        0        0 2023-05-30 08:13:12.000000 Vlttools-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      376 2023-05-30 08:30:13.808941 Vlttools-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-30 08:13:19.000000 Vlttools-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 08:30:13.800417 Vlttools-0.1.0/Vlttools.egg-info/
--rw-rw-rw-   0        0        0      376 2023-05-30 08:30:13.000000 Vlttools-0.1.0/Vlttools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-30 08:30:13.000000 Vlttools-0.1.0/Vlttools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 08:30:13.000000 Vlttools-0.1.0/Vlttools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-30 08:30:13.000000 Vlttools-0.1.0/Vlttools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 08:30:13.000000 Vlttools-0.1.0/Vlttools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      533 2023-05-30 08:17:46.000000 Vlttools-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 08:30:13.810939 Vlttools-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-30 08:30:13.806938 Vlttools-0.1.0/vlttools/
--rw-rw-rw-   0        0        0      641 2023-05-30 08:05:24.000000 Vlttools-0.1.0/vlttools/BenchConfig.py
--rw-rw-rw-   0        0        0       17 2023-05-30 08:12:20.000000 Vlttools-0.1.0/vlttools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:53:43.935759 Vlttools-0.1.1/
+-rw-rw-rw-   0        0        0        0 2023-05-30 08:13:12.000000 Vlttools-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      376 2023-06-20 03:53:43.933761 Vlttools-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-30 08:13:19.000000 Vlttools-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 03:53:43.921171 Vlttools-0.1.1/Vlttools.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-06-20 03:53:43.000000 Vlttools-0.1.1/Vlttools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-06-20 03:53:43.000000 Vlttools-0.1.1/Vlttools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 03:53:43.000000 Vlttools-0.1.1/Vlttools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-20 03:53:43.000000 Vlttools-0.1.1/Vlttools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 03:53:43.000000 Vlttools-0.1.1/Vlttools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      533 2023-05-30 08:35:53.000000 Vlttools-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 03:53:43.935759 Vlttools-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 03:53:43.930754 Vlttools-0.1.1/vlttools/
+-rw-rw-rw-   0        0        0      641 2023-05-30 08:05:24.000000 Vlttools-0.1.1/vlttools/BenchConfig.py
+-rw-rw-rw-   0        0        0       17 2023-05-30 08:12:20.000000 Vlttools-0.1.1/vlttools/__init__.py
```

### Comparing `Vlttools-0.1.0/pyproject.toml` & `Vlttools-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Vlttools"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="tangfei", email="fei.tang@danfoss.com" },
 ]
 description = "Useful tools for Vlt drives"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `Vlttools-0.1.0/vlttools/BenchConfig.py` & `Vlttools-0.1.1/vlttools/BenchConfig.py`

 * *Files identical despite different names*

