# Comparing `tmp/embedchain-0.0.1.tar.gz` & `tmp/embedchain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedchain-0.0.1.tar", last modified: Mon Jun 19 09:46:53 2023, max compression
+gzip compressed data, was "embedchain-0.0.2.tar", last modified: Tue Jun 20 12:35:12 2023, max compression
```

## Comparing `embedchain-0.0.1.tar` & `embedchain-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,27 @@
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-19 09:46:53.213980 embedchain-0.0.1/
--rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-19 09:36:33.000000 embedchain-0.0.1/LICENCE
--rw-r--r--   0 tj         (501) staff       (20)      355 2023-06-19 09:46:53.213864 embedchain-0.0.1/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)       12 2023-06-19 09:41:49.000000 embedchain-0.0.1/README.md
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-19 09:46:53.213155 embedchain-0.0.1/embedchain/
--rw-r--r--   0 tj         (501) staff       (20)       20 2023-06-19 09:41:18.000000 embedchain-0.0.1/embedchain/__init__.py
-drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-19 09:46:53.213718 embedchain-0.0.1/embedchain.egg-info/
--rw-r--r--   0 tj         (501) staff       (20)      355 2023-06-19 09:46:53.000000 embedchain-0.0.1/embedchain.egg-info/PKG-INFO
--rw-r--r--   0 tj         (501) staff       (20)      185 2023-06-19 09:46:53.000000 embedchain-0.0.1/embedchain.egg-info/SOURCES.txt
--rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-19 09:46:53.000000 embedchain-0.0.1/embedchain.egg-info/dependency_links.txt
--rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-19 09:46:53.000000 embedchain-0.0.1/embedchain.egg-info/top_level.txt
--rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-19 09:46:53.214012 embedchain-0.0.1/setup.cfg
--rw-r--r--   0 tj         (501) staff       (20)      607 2023-06-19 09:44:35.000000 embedchain-0.0.1/setup.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 12:35:12.321033 embedchain-0.0.2/
+-rw-r--r--   0 tj         (501) staff       (20)    11349 2023-06-20 11:57:43.000000 embedchain-0.0.2/LICENSE
+-rw-r--r--   0 tj         (501) staff       (20)     5278 2023-06-20 12:35:12.320897 embedchain-0.0.2/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)     4795 2023-06-20 12:34:13.000000 embedchain-0.0.2/README.md
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 12:35:12.318299 embedchain-0.0.2/embedchain/
+-rw-r--r--   0 tj         (501) staff       (20)       27 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/__init__.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 12:35:12.320022 embedchain-0.0.2/embedchain/chunkers/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/chunkers/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      819 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/chunkers/base_chunker.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/chunkers/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      421 2023-06-20 11:23:20.000000 embedchain-0.0.2/embedchain/chunkers/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      426 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/chunkers/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)     4417 2023-06-20 11:23:20.000000 embedchain-0.0.2/embedchain/embedchain.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 12:35:12.320685 embedchain-0.0.2/embedchain/loaders/
+-rw-r--r--   0 tj         (501) staff       (20)        0 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/loaders/__init__.py
+-rw-r--r--   0 tj         (501) staff       (20)      639 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/loaders/pdf_file.py
+-rw-r--r--   0 tj         (501) staff       (20)      731 2023-06-20 11:23:20.000000 embedchain-0.0.2/embedchain/loaders/web_page.py
+-rw-r--r--   0 tj         (501) staff       (20)      618 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/loaders/youtube_video.py
+-rw-r--r--   0 tj         (501) staff       (20)      312 2023-06-20 11:09:25.000000 embedchain-0.0.2/embedchain/utils.py
+drwxr-xr-x   0 tj         (501) staff       (20)        0 2023-06-20 12:35:12.319158 embedchain-0.0.2/embedchain.egg-info/
+-rw-r--r--   0 tj         (501) staff       (20)     5278 2023-06-20 12:35:12.000000 embedchain-0.0.2/embedchain.egg-info/PKG-INFO
+-rw-r--r--   0 tj         (501) staff       (20)      561 2023-06-20 12:35:12.000000 embedchain-0.0.2/embedchain.egg-info/SOURCES.txt
+-rw-r--r--   0 tj         (501) staff       (20)        1 2023-06-20 12:35:12.000000 embedchain-0.0.2/embedchain.egg-info/dependency_links.txt
+-rw-r--r--   0 tj         (501) staff       (20)       95 2023-06-20 12:35:12.000000 embedchain-0.0.2/embedchain.egg-info/requires.txt
+-rw-r--r--   0 tj         (501) staff       (20)       11 2023-06-20 12:35:12.000000 embedchain-0.0.2/embedchain.egg-info/top_level.txt
+-rw-r--r--   0 tj         (501) staff       (20)       38 2023-06-20 12:35:12.321069 embedchain-0.0.2/setup.cfg
+-rw-r--r--   0 tj         (501) staff       (20)      958 2023-06-20 12:12:37.000000 embedchain-0.0.2/setup.py
```

