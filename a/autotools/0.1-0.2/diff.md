# Comparing `tmp/autotools-0.1.tar.gz` & `tmp/autotools-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotools-0.1.tar", last modified: Tue Jun 20 12:17:28 2023, max compression
+gzip compressed data, was "autotools-0.2.tar", last modified: Tue Jun 20 16:59:39 2023, max compression
```

## Comparing `autotools-0.1.tar` & `autotools-0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 12:17:28.712573 autotools-0.1/
--rw-rw-rw-   0        0        0      168 2023-06-20 12:17:28.709573 autotools-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 12:17:28.654313 autotools-0.1/autotools/
--rw-rw-rw-   0        0        0      476 2023-06-20 11:41:33.000000 autotools-0.1/autotools/__init__.py
--rw-rw-rw-   0        0        0     5588 2023-06-20 11:41:26.000000 autotools-0.1/autotools/chatgpt.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:17:28.704615 autotools-0.1/autotools.egg-info/
--rw-rw-rw-   0        0        0      168 2023-06-20 12:17:28.000000 autotools-0.1/autotools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-06-20 12:17:28.000000 autotools-0.1/autotools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 12:17:28.000000 autotools-0.1/autotools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-20 11:57:39.000000 autotools-0.1/autotools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-20 12:17:28.000000 autotools-0.1/autotools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 12:17:28.713089 autotools-0.1/setup.cfg
--rw-rw-rw-   0        0        0      300 2023-06-20 12:00:56.000000 autotools-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:59:39.399822 autotools-0.2/
+-rw-rw-rw-   0        0        0      252 2023-06-20 16:59:39.392817 autotools-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 16:59:39.333143 autotools-0.2/autotools/
+-rw-rw-rw-   0        0        0      637 2023-06-20 16:55:04.000000 autotools-0.2/autotools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:59:39.387817 autotools-0.2/autotools.egg-info/
+-rw-rw-rw-   0        0        0      252 2023-06-20 16:59:38.000000 autotools-0.2/autotools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-06-20 16:59:39.000000 autotools-0.2/autotools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 16:59:38.000000 autotools-0.2/autotools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-20 16:59:38.000000 autotools-0.2/autotools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-20 16:59:38.000000 autotools-0.2/autotools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 16:59:39.399822 autotools-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      369 2023-06-20 16:57:11.000000 autotools-0.2/setup.py
```

