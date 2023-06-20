# Comparing `tmp/DeepLogTimedelta-0.1.2.tar.gz` & `tmp/DeepLogTimedelta-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepLogTimedelta-0.1.2.tar", last modified: Mon Jun 19 13:47:26 2023, max compression
+gzip compressed data, was "DeepLogTimedelta-0.2.0.tar", last modified: Tue Jun 20 07:07:18 2023, max compression
```

## Comparing `DeepLogTimedelta-0.1.2.tar` & `DeepLogTimedelta-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:47:26.296082 DeepLogTimedelta-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-19 13:47:26.259357 DeepLogTimedelta-0.1.2/DeepLogTimedelta/
--rw-rw-rw-   0        0        0     1100 2023-06-19 13:31:46.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta/DeepLogTimedelta.py
--rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta/__init__.py
--rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta/main.py
--rw-rw-rw-   0        0        0     2311 2023-06-19 13:46:57.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta/preproccesing.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:47:26.292900 DeepLogTimedelta-0.1.2/DeepLogTimedelta.egg-info/
--rw-rw-rw-   0        0        0      207 2023-06-19 13:47:26.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-19 13:47:26.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:47:26.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-19 13:47:26.000000 DeepLogTimedelta-0.1.2/DeepLogTimedelta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      207 2023-06-19 13:47:26.295899 DeepLogTimedelta-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-19 13:47:26.297090 DeepLogTimedelta-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      335 2023-06-19 13:47:21.000000 DeepLogTimedelta-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:07:18.509819 DeepLogTimedelta-0.2.0/
+drwxrwxrwx   0        0        0        0 2023-06-20 07:07:18.463077 DeepLogTimedelta-0.2.0/DeepLogTimedelta/
+-rw-rw-rw-   0        0        0     3629 2023-06-20 07:06:04.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta/DeepLogTimedelta.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 12:37:56.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta/__init__.py
+-rw-rw-rw-   0        0        0       97 2023-06-19 11:56:09.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta/main.py
+-rw-rw-rw-   0        0        0     2311 2023-06-19 13:46:57.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta/preproccesing.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:07:18.501819 DeepLogTimedelta-0.2.0/DeepLogTimedelta.egg-info/
+-rw-rw-rw-   0        0        0      207 2023-06-20 07:07:17.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-20 07:07:18.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:07:17.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 07:07:17.000000 DeepLogTimedelta-0.2.0/DeepLogTimedelta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      207 2023-06-20 07:07:18.509819 DeepLogTimedelta-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:07:18.509819 DeepLogTimedelta-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      335 2023-06-20 07:06:38.000000 DeepLogTimedelta-0.2.0/setup.py
```

### Comparing `DeepLogTimedelta-0.1.2/DeepLogTimedelta/preproccesing.py` & `DeepLogTimedelta-0.2.0/DeepLogTimedelta/preproccesing.py`

 * *Files identical despite different names*

