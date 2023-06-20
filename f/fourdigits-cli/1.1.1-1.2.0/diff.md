# Comparing `tmp/fourdigits-cli-1.1.1.tar.gz` & `tmp/fourdigits-cli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fourdigits-cli-1.1.1.tar", last modified: Tue Feb 28 11:53:04 2023, max compression
+gzip compressed data, was "fourdigits-cli-1.2.0.tar", last modified: Tue Jun 20 08:00:10 2023, max compression
```

## Comparing `fourdigits-cli-1.1.1.tar` & `fourdigits-cli-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 11:53:04.321350 fourdigits-cli-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1585 2023-02-28 11:53:04.321350 fourdigits-cli-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-02-28 11:52:03.000000 fourdigits-cli-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 11:53:04.317350 fourdigits-cli-1.1.1/fourdigits_cli/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-02-28 11:52:03.000000 fourdigits-cli-1.1.1/fourdigits_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/fourdigits_cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/fourdigits_cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 11:53:04.317350 fourdigits-cli-1.1.1/fourdigits_cli/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/fourdigits_cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4823 2023-02-28 11:52:03.000000 fourdigits-cli-1.1.1/fourdigits_cli/commands/docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/fourdigits_cli/commands/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/fourdigits_cli/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 11:53:04.317350 fourdigits-cli-1.1.1/fourdigits_cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/fourdigits_cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/fourdigits_cli/utils/docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1919 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/fourdigits_cli/utils/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 11:53:04.317350 fourdigits-cli-1.1.1/fourdigits_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1585 2023-02-28 11:53:04.000000 fourdigits-cli-1.1.1/fourdigits_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      625 2023-02-28 11:53:04.000000 fourdigits-cli-1.1.1/fourdigits_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 11:53:04.000000 fourdigits-cli-1.1.1/fourdigits_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-02-28 11:53:04.000000 fourdigits-cli-1.1.1/fourdigits_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-02-28 11:53:04.000000 fourdigits-cli-1.1.1/fourdigits_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-02-28 11:53:04.000000 fourdigits-cli-1.1.1/fourdigits_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-02-28 11:53:04.321350 fourdigits-cli-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1248 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 11:53:04.321350 fourdigits-cli-1.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-02-28 11:46:40.000000 fourdigits-cli-1.1.1/tests/test_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:00:10.711737 fourdigits-cli-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-06-20 08:00:10.711737 fourdigits-cli-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:00:10.708737 fourdigits-cli-1.2.0/fourdigits_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/fourdigits_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/fourdigits_cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/fourdigits_cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:00:10.710737 fourdigits-cli-1.2.0/fourdigits_cli/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/fourdigits_cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4823 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/fourdigits_cli/commands/docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/fourdigits_cli/commands/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/fourdigits_cli/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:00:10.711737 fourdigits-cli-1.2.0/fourdigits_cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/fourdigits_cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/fourdigits_cli/utils/docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1919 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/fourdigits_cli/utils/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:00:10.709737 fourdigits-cli-1.2.0/fourdigits_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-06-20 08:00:10.000000 fourdigits-cli-1.2.0/fourdigits_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      625 2023-06-20 08:00:10.000000 fourdigits-cli-1.2.0/fourdigits_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 08:00:10.000000 fourdigits-cli-1.2.0/fourdigits_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-20 08:00:10.000000 fourdigits-cli-1.2.0/fourdigits_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-20 08:00:10.000000 fourdigits-cli-1.2.0/fourdigits_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-20 08:00:10.000000 fourdigits-cli-1.2.0/fourdigits_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-20 08:00:10.712737 fourdigits-cli-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:00:10.711737 fourdigits-cli-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-06-20 07:59:08.000000 fourdigits-cli-1.2.0/tests/test_settings.py
```

### Comparing `fourdigits-cli-1.1.1/PKG-INFO` & `fourdigits-cli-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fourdigits-cli
-Version: 1.1.1
+Version: 1.2.0
 Summary: FourDigits CLI tool
 Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # FourDigits CLI
```

### Comparing `fourdigits-cli-1.1.1/README.md` & `fourdigits-cli-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.1.1/fourdigits_cli/cli.py` & `fourdigits-cli-1.2.0/fourdigits_cli/cli.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.1.1/fourdigits_cli/commands/docker.py` & `fourdigits-cli-1.2.0/fourdigits_cli/commands/docker.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.1.1/fourdigits_cli/commands/gitlab.py` & `fourdigits-cli-1.2.0/fourdigits_cli/commands/gitlab.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.1.1/fourdigits_cli/settings.py` & `fourdigits-cli-1.2.0/fourdigits_cli/settings.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.1.1/fourdigits_cli/utils/docker.py` & `fourdigits-cli-1.2.0/fourdigits_cli/utils/docker.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.1.1/fourdigits_cli/utils/git.py` & `fourdigits-cli-1.2.0/fourdigits_cli/utils/git.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.1.1/fourdigits_cli.egg-info/PKG-INFO` & `fourdigits-cli-1.2.0/fourdigits_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fourdigits-cli
-Version: 1.1.1
+Version: 1.2.0
 Summary: FourDigits CLI tool
 Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # FourDigits CLI
```

### Comparing `fourdigits-cli-1.1.1/fourdigits_cli.egg-info/SOURCES.txt` & `fourdigits-cli-1.2.0/fourdigits_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.1.1/setup.py` & `fourdigits-cli-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.1.1/tests/test_settings.py` & `fourdigits-cli-1.2.0/tests/test_settings.py`

 * *Files identical despite different names*

