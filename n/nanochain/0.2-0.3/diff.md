# Comparing `tmp/nanochain-0.2.tar.gz` & `tmp/nanochain-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanochain-0.2.tar", last modified: Mon Jun 19 10:58:01 2023, max compression
+gzip compressed data, was "nanochain-0.3.tar", last modified: Tue Jun 20 02:00:46 2023, max compression
```

## Comparing `nanochain-0.2.tar` & `nanochain-0.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxr-xr-x   0 guodongzhao   (501) staff       (20)        0 2023-06-19 10:58:01.626146 nanochain-0.2/
--rw-r--r--   0 guodongzhao   (501) staff       (20)      404 2023-06-19 10:58:01.625564 nanochain-0.2/PKG-INFO
-drwxr-xr-x   0 guodongzhao   (501) staff       (20)        0 2023-06-19 10:58:01.624528 nanochain-0.2/nanochain.egg-info/
--rw-r--r--   0 guodongzhao   (501) staff       (20)      404 2023-06-19 10:58:01.000000 nanochain-0.2/nanochain.egg-info/PKG-INFO
--rw-r--r--   0 guodongzhao   (501) staff       (20)      159 2023-06-19 10:58:01.000000 nanochain-0.2/nanochain.egg-info/SOURCES.txt
--rw-r--r--   0 guodongzhao   (501) staff       (20)        1 2023-06-19 10:58:01.000000 nanochain-0.2/nanochain.egg-info/dependency_links.txt
--rw-r--r--   0 guodongzhao   (501) staff       (20)       10 2023-06-19 10:58:01.000000 nanochain-0.2/nanochain.egg-info/top_level.txt
--rw-r--r--   0 guodongzhao   (501) staff       (20)    11031 2023-06-19 09:44:07.000000 nanochain-0.2/nanochain.py
--rw-r--r--   0 guodongzhao   (501) staff       (20)      612 2023-06-19 10:57:47.000000 nanochain-0.2/pyproject.toml
--rw-r--r--   0 guodongzhao   (501) staff       (20)       38 2023-06-19 10:58:01.626399 nanochain-0.2/setup.cfg
+drwxr-xr-x   0 guodongzhao   (501) staff       (20)        0 2023-06-20 02:00:46.594102 nanochain-0.3/
+-rw-r--r--   0 guodongzhao   (501) staff       (20)     7911 2023-06-20 02:00:46.593625 nanochain-0.3/PKG-INFO
+-rw-r--r--   0 guodongzhao   (501) staff       (20)     7272 2023-06-19 11:31:43.000000 nanochain-0.3/README.md
+drwxr-xr-x   0 guodongzhao   (501) staff       (20)        0 2023-06-20 02:00:46.592374 nanochain-0.3/nanochain.egg-info/
+-rw-r--r--   0 guodongzhao   (501) staff       (20)     7911 2023-06-20 02:00:46.000000 nanochain-0.3/nanochain.egg-info/PKG-INFO
+-rw-r--r--   0 guodongzhao   (501) staff       (20)      197 2023-06-20 02:00:46.000000 nanochain-0.3/nanochain.egg-info/SOURCES.txt
+-rw-r--r--   0 guodongzhao   (501) staff       (20)        1 2023-06-20 02:00:46.000000 nanochain-0.3/nanochain.egg-info/dependency_links.txt
+-rw-r--r--   0 guodongzhao   (501) staff       (20)       41 2023-06-20 02:00:46.000000 nanochain-0.3/nanochain.egg-info/requires.txt
+-rw-r--r--   0 guodongzhao   (501) staff       (20)        1 2023-06-20 02:00:46.000000 nanochain-0.3/nanochain.egg-info/top_level.txt
+-rw-r--r--   0 guodongzhao   (501) staff       (20)      637 2023-06-19 11:36:05.000000 nanochain-0.3/pyproject.toml
+-rw-r--r--   0 guodongzhao   (501) staff       (20)       38 2023-06-20 02:00:46.594294 nanochain-0.3/setup.cfg
+-rw-r--r--   0 guodongzhao   (501) staff       (20)     1001 2023-06-19 11:36:06.000000 nanochain-0.3/setup.py
```

### Comparing `nanochain-0.2/pyproject.toml` & `nanochain-0.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
-[project]
+[tool.poetry]
 name = "nanochain"
-version = "0.2"
+version = "0.3"
 description = "NanoChain is a Python library designed to provide a suite of useful tools for text processing, vector indexing, and utilizing OpenAI's GPT API to perform various tasks. This is a minimalistic implementation of LangChain because it's too complicated and difficult to customize."
-
-[project.urls]
 repository = "https://github.com/Troyanovsky/nano_chain"
-
-[options]
-install_requires = [
+dependencies = [
     "openai",
     "demjson3",
     "tiktoken",
     "chromadb",
     "PyPDF2",
 ]
+
+[tool.poetry.scripts]
+nanochain = "nanochain:main"
```

