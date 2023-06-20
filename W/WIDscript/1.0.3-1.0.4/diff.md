# Comparing `tmp/WIDscript-1.0.3.tar.gz` & `tmp/WIDscript-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WIDscript-1.0.3.tar", last modified: Tue Jun 20 00:37:55 2023, max compression
+gzip compressed data, was "WIDscript-1.0.4.tar", last modified: Tue Jun 20 14:39:12 2023, max compression
```

## Comparing `WIDscript-1.0.3.tar` & `WIDscript-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 00:37:55.034986 WIDscript-1.0.3/
--rw-rw-rw-   0        0        0        0 2023-06-19 20:14:16.000000 WIDscript-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      507 2023-06-20 00:37:55.034986 WIDscript-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-19 20:32:17.000000 WIDscript-1.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-06-19 20:36:26.000000 WIDscript-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      648 2023-06-20 00:37:55.035991 WIDscript-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 00:37:55.016940 WIDscript-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 00:37:55.023463 WIDscript-1.0.3/src/WIDscript/
--rw-rw-rw-   0        0        0    21525 2023-06-20 00:33:04.000000 WIDscript-1.0.3/src/WIDscript/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 00:37:55.033988 WIDscript-1.0.3/src/WIDscript.egg-info/
--rw-rw-rw-   0        0        0      507 2023-06-20 00:37:55.000000 WIDscript-1.0.3/src/WIDscript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-06-20 00:37:55.000000 WIDscript-1.0.3/src/WIDscript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 00:37:55.000000 WIDscript-1.0.3/src/WIDscript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-20 00:37:55.000000 WIDscript-1.0.3/src/WIDscript.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 14:39:12.523189 WIDscript-1.0.4/
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:14:16.000000 WIDscript-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      507 2023-06-20 14:39:12.523189 WIDscript-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:32:17.000000 WIDscript-1.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-19 20:36:26.000000 WIDscript-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      648 2023-06-20 14:39:12.525189 WIDscript-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 14:39:12.501139 WIDscript-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:39:12.506643 WIDscript-1.0.4/src/WIDscript/
+-rw-rw-rw-   0        0        0    36695 2023-06-20 14:37:41.000000 WIDscript-1.0.4/src/WIDscript/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:39:12.522190 WIDscript-1.0.4/src/WIDscript.egg-info/
+-rw-rw-rw-   0        0        0      507 2023-06-20 14:39:12.000000 WIDscript-1.0.4/src/WIDscript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-06-20 14:39:12.000000 WIDscript-1.0.4/src/WIDscript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:39:12.000000 WIDscript-1.0.4/src/WIDscript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-20 14:39:12.000000 WIDscript-1.0.4/src/WIDscript.egg-info/top_level.txt
```

### Comparing `WIDscript-1.0.3/setup.cfg` & `WIDscript-1.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2057 4944 7363 7269 7074 0d0a 7665   = WIDscript..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 330d 0a61  rsion = 1.0.3..a
+00000020: 7273 696f 6e20 3d20 312e 302e 340d 0a61  rsion = 1.0.4..a
 00000030: 7574 686f 7220 3d20 4578 616d 706c 6520  uthor = Example 
 00000040: 4175 7468 6f72 0d0a 6175 7468 6f72 5f65  Author..author_e
 00000050: 6d61 696c 203d 2061 7574 686f 7240 6578  mail = author@ex
 00000060: 616d 706c 652e 636f 6d0d 0a64 6573 6372  ample.com..descr
 00000070: 6970 7469 6f6e 203d 2041 2073 6d61 6c6c  iption = A small
 00000080: 2065 7861 6d70 6c65 2070 6163 6b61 6765   example package
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

