# Comparing `tmp/altcos-common-0.0.1.tar.gz` & `tmp/altcos-common-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altcos-common-0.0.1.tar", last modified: Fri Jun  9 09:51:45 2023, max compression
+gzip compressed data, was "altcos-common-0.0.2.tar", last modified: Tue Jun 20 09:11:30 2023, max compression
```

## Comparing `altcos-common-0.0.1.tar` & `altcos-common-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-09 09:51:45.840178 altcos-common-0.0.1/
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     1070 2023-06-09 09:40:20.000000 altcos-common-0.0.1/LICENSE
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     1194 2023-06-09 09:51:45.840178 altcos-common-0.0.1/PKG-INFO
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      746 2023-06-09 07:54:06.000000 altcos-common-0.0.1/README.md
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      630 2023-06-09 09:50:42.000000 altcos-common-0.0.1/pyproject.toml
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)       38 2023-06-09 09:51:45.840178 altcos-common-0.0.1/setup.cfg
-drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-09 09:51:45.839178 altcos-common-0.0.1/src/
-drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-09 09:51:45.840178 altcos-common-0.0.1/src/altcos/
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-09 07:19:00.000000 altcos-common-0.0.1/src/altcos/__init__.py
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      676 2023-06-09 07:36:20.000000 altcos-common-0.0.1/src/altcos/build.py
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      174 2023-06-09 06:53:39.000000 altcos-common-0.0.1/src/altcos/common.py
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     7745 2023-06-09 07:36:20.000000 altcos-common-0.0.1/src/altcos/ostree.py
-drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-09 09:51:45.840178 altcos-common-0.0.1/src/altcos_common.egg-info/
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     1194 2023-06-09 09:51:45.000000 altcos-common-0.0.1/src/altcos_common.egg-info/PKG-INFO
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      342 2023-06-09 09:51:45.000000 altcos-common-0.0.1/src/altcos_common.egg-info/SOURCES.txt
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)        1 2023-06-09 09:51:45.000000 altcos-common-0.0.1/src/altcos_common.egg-info/dependency_links.txt
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)       10 2023-06-09 09:51:45.000000 altcos-common-0.0.1/src/altcos_common.egg-info/requires.txt
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)        7 2023-06-09 09:51:45.000000 altcos-common-0.0.1/src/altcos_common.egg-info/top_level.txt
-drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-09 09:51:45.840178 altcos-common-0.0.1/tests/
--rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     4873 2023-06-09 08:46:37.000000 altcos-common-0.0.1/tests/test_ostree.py
+drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-20 09:11:30.129539 altcos-common-0.0.2/
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     1070 2023-06-09 09:40:20.000000 altcos-common-0.0.2/LICENSE
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      774 2023-06-20 09:11:30.129539 altcos-common-0.0.2/PKG-INFO
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      326 2023-06-20 08:49:16.000000 altcos-common-0.0.2/README.md
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      630 2023-06-20 09:05:21.000000 altcos-common-0.0.2/pyproject.toml
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)       38 2023-06-20 09:11:30.129539 altcos-common-0.0.2/setup.cfg
+drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-20 09:11:30.128538 altcos-common-0.0.2/src/
+drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-20 09:11:30.128538 altcos-common-0.0.2/src/altcos/
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-09 07:19:00.000000 altcos-common-0.0.2/src/altcos/__init__.py
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      174 2023-06-20 08:49:16.000000 altcos-common-0.0.2/src/altcos/_common.py
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      679 2023-06-20 08:49:16.000000 altcos-common-0.0.2/src/altcos/build.py
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     7921 2023-06-20 09:01:19.000000 altcos-common-0.0.2/src/altcos/ostree.py
+drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-20 09:11:30.128538 altcos-common-0.0.2/src/altcos_common.egg-info/
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      774 2023-06-20 09:11:30.000000 altcos-common-0.0.2/src/altcos_common.egg-info/PKG-INFO
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)      343 2023-06-20 09:11:30.000000 altcos-common-0.0.2/src/altcos_common.egg-info/SOURCES.txt
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)        1 2023-06-20 09:11:30.000000 altcos-common-0.0.2/src/altcos_common.egg-info/dependency_links.txt
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)       10 2023-06-20 09:11:30.000000 altcos-common-0.0.2/src/altcos_common.egg-info/requires.txt
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)        7 2023-06-20 09:11:30.000000 altcos-common-0.0.2/src/altcos_common.egg-info/top_level.txt
+drwxr-xr-x   0 fl0pp5     (500) fl0pp5     (500)        0 2023-06-20 09:11:30.128538 altcos-common-0.0.2/tests/
+-rw-r--r--   0 fl0pp5     (500) fl0pp5     (500)     4873 2023-06-09 08:46:37.000000 altcos-common-0.0.2/tests/test_ostree.py
```

### Comparing `altcos-common-0.0.1/LICENSE` & `altcos-common-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `altcos-common-0.0.1/pyproject.toml` & `altcos-common-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "altcos-common"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Ivan Pepelyaev", email = "fl0pp5@altlinux.org" },
 ]
 description = "Components for working with altcos"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `altcos-common-0.0.1/src/altcos/build.py` & `altcos-common-0.0.2/src/altcos/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import dataclasses
 import os
 import typing
 
-from altcos import common
+from altcos import _common
 
 
-class Platform(common.StrEnum):
+class Platform(_common.StrEnum):
     QEMU = "qemu"
     METAL = "metal"
 
 
-class Format(common.StrEnum):
+class Format(_common.StrEnum):
     QCOW2 = "qcow2"
     ISO = "iso"
     RAW = "raw"
 
 
 @dataclasses.dataclass
 class Disk:
```

### Comparing `altcos-common-0.0.1/src/altcos/ostree.py` & `altcos-common-0.0.2/src/altcos/ostree.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 import gi
 
 gi.require_version("OSTree", "1.0")
 
 from gi.repository import Gio, OSTree
 
-from altcos import common
+from altcos import _common
 
 
-class OSName(common.StrEnum):
+class OSName(_common.StrEnum):
     ALTCOS = "altcos"
 
 
-class Arch(common.StrEnum):
+class Arch(_common.StrEnum):
     X86_64 = "x86_64"
 
 
-class Branch(common.StrEnum):
+class Branch(_common.StrEnum):
     SISYPHUS = "sisyphus"
     P10 = "p10"
 
 
 class Stream:
     def __init__(self,
                  streams_root: str | os.PathLike,
@@ -124,15 +124,15 @@
         """
         :return: путь до директории, примонтированной в overlay-режиме
         """
         return self.work_dir.joinpath("merged")
 
 
 class Repository:
-    class Mode(common.StrEnum):
+    class Mode(_common.StrEnum):
         BARE = "bare"
         ARCHIVE = "archive"
 
     def __init__(self, stream: Stream, mode: Repository.Mode = Mode.BARE) -> None:
         self.stream = stream
         match mode:
             case Repository.Mode.BARE:
@@ -160,14 +160,18 @@
             return commit
 
         if (parent := commit.parent()) is None:
             return None
 
         return self.commit_by_version(version, parent)
 
+    def list_streams(self) -> list[Stream]:
+        return [Stream.from_ostree_ref(self.stream.streams_root, ref)
+                for ref in self.storage.list_refs()[1]]
+
 
 class Version:
     def __init__(self,
                  major: int,
                  minor: int,
                  branch: Branch,
                  substream: str | None = None,
```

### Comparing `altcos-common-0.0.1/tests/test_ostree.py` & `altcos-common-0.0.2/tests/test_ostree.py`

 * *Files identical despite different names*

