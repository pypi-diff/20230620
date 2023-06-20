# Comparing `tmp/roo-0.17.0.tar.gz` & `tmp/roo-0.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roo-0.17.0.tar", last modified: Wed Jun 14 14:38:11 2023, max compression
+gzip compressed data, was "roo-0.17.1.tar", max compression
```

## Comparing `roo-0.17.0.tar` & `roo-0.17.1.tar`

### file list

```diff
@@ -1,69 +1,68 @@
--rw-r--r--   0        0        0    11359 2021-09-21 14:07:34.073753 roo-0.17.0/LICENSE.md
--rw-r--r--   0        0        0     1212 2023-05-16 11:28:04.297584 roo-0.17.0/README.md
--rw-r--r--   0        0        0     1330 2023-06-14 14:37:53.895857 roo-0.17.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-08-09 15:05:08.798034 roo-0.17.0/src/roo/__init__.py
--rw-r--r--   0        0        0        0 2021-08-09 15:05:08.927710 roo-0.17.0/src/roo/caches/__init__.py
--rw-r--r--   0        0        0     5758 2023-01-11 16:49:22.774952 roo-0.17.0/src/roo/caches/build_cache.py
--rw-r--r--   0        0        0     9013 2023-01-11 16:49:22.777084 roo-0.17.0/src/roo/caches/source_cache.py
--rw-r--r--   0        0        0     1711 2022-11-10 21:47:05.969673 roo-0.17.0/src/roo/caches/vcs_store.py
--rw-r--r--   0        0        0        0 2021-08-09 15:05:08.823447 roo-0.17.0/src/roo/cli/__init__.py
--rw-r--r--   0        0        0     1019 2022-11-10 22:18:32.545040 roo-0.17.0/src/roo/cli/__main__.py
--rw-r--r--   0        0        0      999 2022-01-19 09:59:48.442478 roo-0.17.0/src/roo/cli/add/__init__.py
--rw-r--r--   0        0        0     2745 2023-01-11 16:49:22.778675 roo-0.17.0/src/roo/cli/cache/__init__.py
--rw-r--r--   0        0        0     5100 2022-11-10 21:47:05.974887 roo-0.17.0/src/roo/cli/environment/__init__.py
--rw-r--r--   0        0        0     1551 2023-05-16 11:27:52.887887 roo-0.17.0/src/roo/cli/export/__init__.py
--rw-r--r--   0        0        0      569 2022-01-19 09:59:48.445880 roo-0.17.0/src/roo/cli/init/__init__.py
--rw-r--r--   0        0        0     4163 2023-05-16 11:27:52.888969 roo-0.17.0/src/roo/cli/install/__init__.py
--rw-r--r--   0        0        0     2764 2023-05-16 11:27:52.890173 roo-0.17.0/src/roo/cli/lock/__init__.py
--rw-r--r--   0        0        0     2274 2022-11-10 22:18:32.547963 roo-0.17.0/src/roo/cli/package/__init__.py
--rw-r--r--   0        0        0     2758 2022-11-10 22:18:32.549018 roo-0.17.0/src/roo/cli/rswitch/__init__.py
--rw-r--r--   0        0        0     1330 2022-11-10 22:18:32.550119 roo-0.17.0/src/roo/cli/run/__init__.py
--rw-r--r--   0        0        0       22 2022-10-26 11:44:39.992134 roo-0.17.0/src/roo/cli/x
--rw-r--r--   0        0        0      666 2022-11-10 22:18:32.551337 roo-0.17.0/src/roo/console.py
--rw-r--r--   0        0        0        0 2021-08-09 15:05:08.765181 roo-0.17.0/src/roo/deptree/__init__.py
--rw-r--r--   0        0        0     3355 2022-11-10 21:47:05.984293 roo-0.17.0/src/roo/deptree/dependencies.py
--rw-r--r--   0        0        0     7042 2022-11-10 21:47:05.986238 roo-0.17.0/src/roo/deptree/transforms.py
--rw-r--r--   0        0        0     2209 2021-08-09 15:23:46.856211 roo-0.17.0/src/roo/deptree/traverse.py
--rw-r--r--   0        0        0    17353 2022-11-10 22:18:32.552703 roo-0.17.0/src/roo/environment.py
--rw-r--r--   0        0        0        0 2021-08-09 15:05:08.795887 roo-0.17.0/src/roo/exporters/__init__.py
--rw-r--r--   0        0        0       39 2021-08-09 15:05:08.797619 roo-0.17.0/src/roo/exporters/exceptions.py
--rw-r--r--   0        0        0        0 2021-08-09 15:05:08.791440 roo-0.17.0/src/roo/exporters/lock/__init__.py
--rw-r--r--   0        0        0      138 2021-08-09 15:34:34.944499 roo-0.17.0/src/roo/exporters/lock/base_exporter.py
--rw-r--r--   0        0        0     1404 2022-11-10 21:47:05.987811 roo-0.17.0/src/roo/exporters/lock/lock_csv_exporter.py
--rw-r--r--   0        0        0     2098 2021-08-09 15:37:09.104002 roo-0.17.0/src/roo/exporters/lock/lock_packrat_exporter.py
--rw-r--r--   0        0        0     2026 2022-11-10 21:47:05.988921 roo-0.17.0/src/roo/exporters/lock/lock_renv_exporter.py
--rw-r--r--   0        0        0        0 2021-08-09 15:05:08.899972 roo-0.17.0/src/roo/files/__init__.py
--rw-r--r--   0        0        0     3069 2021-12-15 15:42:09.432373 roo-0.17.0/src/roo/files/rprofile.py
--rw-r--r--   0        0        0     1230 2022-11-10 21:47:05.990754 roo-0.17.0/src/roo/hashing.py
--rw-r--r--   0        0        0    14585 2023-05-16 11:27:52.891405 roo-0.17.0/src/roo/installer.py
--rw-r--r--   0        0        0     4294 2023-05-16 11:27:52.892475 roo-0.17.0/src/roo/locker.py
--rw-r--r--   0        0        0      732 2021-08-09 15:05:08.897841 roo-0.17.0/src/roo/network.py
--rw-r--r--   0        0        0        0 2021-08-09 15:05:08.774252 roo-0.17.0/src/roo/parsers/__init__.py
--rw-r--r--   0        0        0     3857 2023-06-14 14:33:43.819619 roo-0.17.0/src/roo/parsers/description.py
--rw-r--r--   0        0        0       40 2021-08-09 15:05:08.789239 roo-0.17.0/src/roo/parsers/exceptions.py
--rw-r--r--   0        0        0     8325 2022-11-10 21:47:05.996575 roo-0.17.0/src/roo/parsers/lock.py
--rw-r--r--   0        0        0     9342 2022-11-10 21:47:05.997968 roo-0.17.0/src/roo/parsers/rproject.py
--rw-r--r--   0        0        0     1603 2021-08-09 15:05:08.922172 roo-0.17.0/src/roo/parsing_utils.py
--rw-r--r--   0        0        0     6471 2022-11-10 22:18:32.554099 roo-0.17.0/src/roo/r_executor.py
--rw-r--r--   0        0        0    15048 2022-11-10 21:47:06.001055 roo-0.17.0/src/roo/resolver.py
--rw-r--r--   0        0        0      159 2021-08-09 15:05:08.852757 roo-0.17.0/src/roo/semver/README.md
--rw-r--r--   0        0        0     4847 2021-08-09 15:05:08.839083 roo-0.17.0/src/roo/semver/__init__.py
--rw-r--r--   0        0        0      562 2021-08-09 15:05:08.895243 roo-0.17.0/src/roo/semver/empty_constraint.py
--rw-r--r--   0        0        0       97 2021-08-09 15:05:08.894002 roo-0.17.0/src/roo/semver/exceptions.py
--rw-r--r--   0        0        0      803 2021-08-09 15:05:08.837823 roo-0.17.0/src/roo/semver/patterns.py
--rw-r--r--   0        0        0    12425 2021-08-09 15:05:08.837165 roo-0.17.0/src/roo/semver/version.py
--rw-r--r--   0        0        0      982 2021-08-09 15:05:08.894828 roo-0.17.0/src/roo/semver/version_constraint.py
--rw-r--r--   0        0        0    13896 2021-08-09 15:05:08.894450 roo-0.17.0/src/roo/semver/version_range.py
--rw-r--r--   0        0        0     8191 2021-08-09 15:05:08.838477 roo-0.17.0/src/roo/semver/version_union.py
--rw-r--r--   0        0        0        0 2021-08-09 15:05:08.906842 roo-0.17.0/src/roo/sources/__init__.py
--rw-r--r--   0        0        0     1315 2022-11-10 21:47:06.002315 roo-0.17.0/src/roo/sources/dir_package.py
--rw-r--r--   0        0        0       80 2021-08-09 15:05:08.921675 roo-0.17.0/src/roo/sources/exceptions.py
--rw-r--r--   0        0        0     8081 2022-11-10 22:18:32.555355 roo-0.17.0/src/roo/sources/local_source.py
--rw-r--r--   0        0        0     1045 2022-11-10 21:47:06.004676 roo-0.17.0/src/roo/sources/package_abc.py
--rw-r--r--   0        0        0     9698 2022-11-10 22:18:32.556674 roo-0.17.0/src/roo/sources/remote_source.py
--rw-r--r--   0        0        0     1686 2022-11-10 22:18:32.557978 roo-0.17.0/src/roo/sources/source_abc.py
--rw-r--r--   0        0        0     5308 2022-11-10 21:47:06.009688 roo-0.17.0/src/roo/sources/source_group.py
--rw-r--r--   0        0        0     4768 2022-11-10 21:47:06.011614 roo-0.17.0/src/roo/sources/source_package.py
--rw-r--r--   0        0        0      815 2021-08-09 15:05:08.921275 roo-0.17.0/src/roo/sources/vcs.py
--rw-r--r--   0        0        0     2590 2023-06-14 14:38:13.199619 roo-0.17.0/setup.py
--rw-r--r--   0        0        0     2467 2023-06-14 14:38:13.200577 roo-0.17.0/PKG-INFO
+-rw-r--r--   0        0        0    11359 2021-09-21 14:07:34.073753 roo-0.17.1/LICENSE.md
+-rw-r--r--   0        0        0     1212 2023-05-16 11:28:04.297584 roo-0.17.1/README.md
+-rw-r--r--   0        0        0     1330 2023-06-20 13:26:30.388820 roo-0.17.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-08-09 15:05:08.798034 roo-0.17.1/src/roo/__init__.py
+-rw-r--r--   0        0        0        0 2021-08-09 15:05:08.927710 roo-0.17.1/src/roo/caches/__init__.py
+-rw-r--r--   0        0        0     5758 2023-01-11 16:49:22.774952 roo-0.17.1/src/roo/caches/build_cache.py
+-rw-r--r--   0        0        0     9013 2023-01-11 16:49:22.777084 roo-0.17.1/src/roo/caches/source_cache.py
+-rw-r--r--   0        0        0     1711 2022-11-10 21:47:05.969673 roo-0.17.1/src/roo/caches/vcs_store.py
+-rw-r--r--   0        0        0        0 2021-08-09 15:05:08.823447 roo-0.17.1/src/roo/cli/__init__.py
+-rw-r--r--   0        0        0     1019 2022-11-10 22:18:32.545040 roo-0.17.1/src/roo/cli/__main__.py
+-rw-r--r--   0        0        0      999 2022-01-19 09:59:48.442478 roo-0.17.1/src/roo/cli/add/__init__.py
+-rw-r--r--   0        0        0     2745 2023-01-11 16:49:22.778675 roo-0.17.1/src/roo/cli/cache/__init__.py
+-rw-r--r--   0        0        0     5100 2022-11-10 21:47:05.974887 roo-0.17.1/src/roo/cli/environment/__init__.py
+-rw-r--r--   0        0        0     1551 2023-05-16 11:27:52.887887 roo-0.17.1/src/roo/cli/export/__init__.py
+-rw-r--r--   0        0        0      569 2022-01-19 09:59:48.445880 roo-0.17.1/src/roo/cli/init/__init__.py
+-rw-r--r--   0        0        0     4163 2023-05-16 11:27:52.888969 roo-0.17.1/src/roo/cli/install/__init__.py
+-rw-r--r--   0        0        0     2764 2023-05-16 11:27:52.890173 roo-0.17.1/src/roo/cli/lock/__init__.py
+-rw-r--r--   0        0        0     2274 2022-11-10 22:18:32.547963 roo-0.17.1/src/roo/cli/package/__init__.py
+-rw-r--r--   0        0        0     2758 2022-11-10 22:18:32.549018 roo-0.17.1/src/roo/cli/rswitch/__init__.py
+-rw-r--r--   0        0        0     1330 2022-11-10 22:18:32.550119 roo-0.17.1/src/roo/cli/run/__init__.py
+-rw-r--r--   0        0        0       22 2022-10-26 11:44:39.992134 roo-0.17.1/src/roo/cli/x
+-rw-r--r--   0        0        0      666 2022-11-10 22:18:32.551337 roo-0.17.1/src/roo/console.py
+-rw-r--r--   0        0        0        0 2021-08-09 15:05:08.765181 roo-0.17.1/src/roo/deptree/__init__.py
+-rw-r--r--   0        0        0     3355 2022-11-10 21:47:05.984293 roo-0.17.1/src/roo/deptree/dependencies.py
+-rw-r--r--   0        0        0     7042 2022-11-10 21:47:05.986238 roo-0.17.1/src/roo/deptree/transforms.py
+-rw-r--r--   0        0        0     2209 2021-08-09 15:23:46.856211 roo-0.17.1/src/roo/deptree/traverse.py
+-rw-r--r--   0        0        0    17353 2022-11-10 22:18:32.552703 roo-0.17.1/src/roo/environment.py
+-rw-r--r--   0        0        0        0 2021-08-09 15:05:08.795887 roo-0.17.1/src/roo/exporters/__init__.py
+-rw-r--r--   0        0        0       39 2021-08-09 15:05:08.797619 roo-0.17.1/src/roo/exporters/exceptions.py
+-rw-r--r--   0        0        0        0 2021-08-09 15:05:08.791440 roo-0.17.1/src/roo/exporters/lock/__init__.py
+-rw-r--r--   0        0        0      138 2021-08-09 15:34:34.944499 roo-0.17.1/src/roo/exporters/lock/base_exporter.py
+-rw-r--r--   0        0        0     1404 2022-11-10 21:47:05.987811 roo-0.17.1/src/roo/exporters/lock/lock_csv_exporter.py
+-rw-r--r--   0        0        0     2098 2021-08-09 15:37:09.104002 roo-0.17.1/src/roo/exporters/lock/lock_packrat_exporter.py
+-rw-r--r--   0        0        0     2026 2022-11-10 21:47:05.988921 roo-0.17.1/src/roo/exporters/lock/lock_renv_exporter.py
+-rw-r--r--   0        0        0        0 2021-08-09 15:05:08.899972 roo-0.17.1/src/roo/files/__init__.py
+-rw-r--r--   0        0        0     3069 2021-12-15 15:42:09.432373 roo-0.17.1/src/roo/files/rprofile.py
+-rw-r--r--   0        0        0     1230 2022-11-10 21:47:05.990754 roo-0.17.1/src/roo/hashing.py
+-rw-r--r--   0        0        0    14585 2023-05-16 11:27:52.891405 roo-0.17.1/src/roo/installer.py
+-rw-r--r--   0        0        0     4294 2023-05-16 11:27:52.892475 roo-0.17.1/src/roo/locker.py
+-rw-r--r--   0        0        0      732 2021-08-09 15:05:08.897841 roo-0.17.1/src/roo/network.py
+-rw-r--r--   0        0        0        0 2021-08-09 15:05:08.774252 roo-0.17.1/src/roo/parsers/__init__.py
+-rw-r--r--   0        0        0     3857 2023-06-14 14:33:43.819619 roo-0.17.1/src/roo/parsers/description.py
+-rw-r--r--   0        0        0       40 2021-08-09 15:05:08.789239 roo-0.17.1/src/roo/parsers/exceptions.py
+-rw-r--r--   0        0        0     8325 2022-11-10 21:47:05.996575 roo-0.17.1/src/roo/parsers/lock.py
+-rw-r--r--   0        0        0     9342 2022-11-10 21:47:05.997968 roo-0.17.1/src/roo/parsers/rproject.py
+-rw-r--r--   0        0        0     1603 2021-08-09 15:05:08.922172 roo-0.17.1/src/roo/parsing_utils.py
+-rw-r--r--   0        0        0     6471 2022-11-10 22:18:32.554099 roo-0.17.1/src/roo/r_executor.py
+-rw-r--r--   0        0        0    15048 2022-11-10 21:47:06.001055 roo-0.17.1/src/roo/resolver.py
+-rw-r--r--   0        0        0      159 2021-08-09 15:05:08.852757 roo-0.17.1/src/roo/semver/README.md
+-rw-r--r--   0        0        0     4847 2021-08-09 15:05:08.839083 roo-0.17.1/src/roo/semver/__init__.py
+-rw-r--r--   0        0        0      562 2021-08-09 15:05:08.895243 roo-0.17.1/src/roo/semver/empty_constraint.py
+-rw-r--r--   0        0        0       97 2021-08-09 15:05:08.894002 roo-0.17.1/src/roo/semver/exceptions.py
+-rw-r--r--   0        0        0      803 2021-08-09 15:05:08.837823 roo-0.17.1/src/roo/semver/patterns.py
+-rw-r--r--   0        0        0    12425 2021-08-09 15:05:08.837165 roo-0.17.1/src/roo/semver/version.py
+-rw-r--r--   0        0        0      982 2021-08-09 15:05:08.894828 roo-0.17.1/src/roo/semver/version_constraint.py
+-rw-r--r--   0        0        0    13896 2021-08-09 15:05:08.894450 roo-0.17.1/src/roo/semver/version_range.py
+-rw-r--r--   0        0        0     8191 2021-08-09 15:05:08.838477 roo-0.17.1/src/roo/semver/version_union.py
+-rw-r--r--   0        0        0        0 2021-08-09 15:05:08.906842 roo-0.17.1/src/roo/sources/__init__.py
+-rw-r--r--   0        0        0     1315 2022-11-10 21:47:06.002315 roo-0.17.1/src/roo/sources/dir_package.py
+-rw-r--r--   0        0        0       80 2021-08-09 15:05:08.921675 roo-0.17.1/src/roo/sources/exceptions.py
+-rw-r--r--   0        0        0     8081 2022-11-10 22:18:32.555355 roo-0.17.1/src/roo/sources/local_source.py
+-rw-r--r--   0        0        0     1045 2022-11-10 21:47:06.004676 roo-0.17.1/src/roo/sources/package_abc.py
+-rw-r--r--   0        0        0     9640 2023-06-20 13:26:11.408483 roo-0.17.1/src/roo/sources/remote_source.py
+-rw-r--r--   0        0        0     1686 2022-11-10 22:18:32.557978 roo-0.17.1/src/roo/sources/source_abc.py
+-rw-r--r--   0        0        0     5308 2022-11-10 21:47:06.009688 roo-0.17.1/src/roo/sources/source_group.py
+-rw-r--r--   0        0        0     4768 2022-11-10 21:47:06.011614 roo-0.17.1/src/roo/sources/source_package.py
+-rw-r--r--   0        0        0      815 2021-08-09 15:05:08.921275 roo-0.17.1/src/roo/sources/vcs.py
+-rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 roo-0.17.1/PKG-INFO
```

### Comparing `roo-0.17.0/LICENSE.md` & `roo-0.17.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/README.md` & `roo-0.17.1/README.md`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/pyproject.toml` & `roo-0.17.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "roo"
-version = "0.17.0"
+version = "0.17.1"
 description = "A package manager to handle R environments"
 authors = ["Stefano Borini <stefano.borini@astrazeneca.com>"]
 license = "Apache-2.0"
 keywords = [
     "R",
     "packaging",
     "environment",
```

### Comparing `roo-0.17.0/src/roo/caches/build_cache.py` & `roo-0.17.1/src/roo/caches/build_cache.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/caches/source_cache.py` & `roo-0.17.1/src/roo/caches/source_cache.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/caches/vcs_store.py` & `roo-0.17.1/src/roo/caches/vcs_store.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/cli/__main__.py` & `roo-0.17.1/src/roo/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/cli/add/__init__.py` & `roo-0.17.1/src/roo/cli/add/__init__.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/cli/cache/__init__.py` & `roo-0.17.1/src/roo/cli/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/cli/environment/__init__.py` & `roo-0.17.1/src/roo/cli/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/cli/export/__init__.py` & `roo-0.17.1/src/roo/cli/export/__init__.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/cli/init/__init__.py` & `roo-0.17.1/src/roo/cli/init/__init__.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/cli/install/__init__.py` & `roo-0.17.1/src/roo/cli/install/__init__.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/cli/lock/__init__.py` & `roo-0.17.1/src/roo/cli/lock/__init__.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/cli/package/__init__.py` & `roo-0.17.1/src/roo/cli/package/__init__.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/cli/rswitch/__init__.py` & `roo-0.17.1/src/roo/cli/rswitch/__init__.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/cli/run/__init__.py` & `roo-0.17.1/src/roo/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/console.py` & `roo-0.17.1/src/roo/console.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/deptree/dependencies.py` & `roo-0.17.1/src/roo/deptree/dependencies.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/deptree/transforms.py` & `roo-0.17.1/src/roo/deptree/transforms.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/deptree/traverse.py` & `roo-0.17.1/src/roo/deptree/traverse.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/environment.py` & `roo-0.17.1/src/roo/environment.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/exporters/lock/lock_csv_exporter.py` & `roo-0.17.1/src/roo/exporters/lock/lock_csv_exporter.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/exporters/lock/lock_packrat_exporter.py` & `roo-0.17.1/src/roo/exporters/lock/lock_packrat_exporter.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/exporters/lock/lock_renv_exporter.py` & `roo-0.17.1/src/roo/exporters/lock/lock_renv_exporter.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/files/rprofile.py` & `roo-0.17.1/src/roo/files/rprofile.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/hashing.py` & `roo-0.17.1/src/roo/hashing.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/installer.py` & `roo-0.17.1/src/roo/installer.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/locker.py` & `roo-0.17.1/src/roo/locker.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/network.py` & `roo-0.17.1/src/roo/network.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/parsers/description.py` & `roo-0.17.1/src/roo/parsers/description.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/parsers/lock.py` & `roo-0.17.1/src/roo/parsers/lock.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/parsers/rproject.py` & `roo-0.17.1/src/roo/parsers/rproject.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/parsing_utils.py` & `roo-0.17.1/src/roo/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/r_executor.py` & `roo-0.17.1/src/roo/r_executor.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/resolver.py` & `roo-0.17.1/src/roo/resolver.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/semver/__init__.py` & `roo-0.17.1/src/roo/semver/__init__.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/semver/empty_constraint.py` & `roo-0.17.1/src/roo/semver/empty_constraint.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/semver/patterns.py` & `roo-0.17.1/src/roo/semver/patterns.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/semver/version.py` & `roo-0.17.1/src/roo/semver/version.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/semver/version_constraint.py` & `roo-0.17.1/src/roo/semver/version_constraint.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/semver/version_range.py` & `roo-0.17.1/src/roo/semver/version_range.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/semver/version_union.py` & `roo-0.17.1/src/roo/semver/version_union.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/sources/dir_package.py` & `roo-0.17.1/src/roo/sources/dir_package.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/sources/local_source.py` & `roo-0.17.1/src/roo/sources/local_source.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/sources/package_abc.py` & `roo-0.17.1/src/roo/sources/package_abc.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/sources/remote_source.py` & `roo-0.17.1/src/roo/sources/remote_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,23 +245,22 @@
 
 
 def _is_package_entry(entry: Any) -> bool:
     """Returns True if the html entry describes a package."""
     href = entry["href"]
     return cast(bool, (
         href.endswith("gz")
-        and href == entry.string
         and href != "PACKAGES.gz"
     ))
 
 
 def _is_dir_entry(entry: Any) -> bool:
     """Returns true if the html entry refers to a directory."""
     href = entry["href"]
-    return cast(bool, (href.endswith("/") and href == entry.string))
+    return cast(bool, (href.endswith("/")))
 
 
 def _get_pkgfiles_and_dirs_at_url(session: Any, url: str) -> tuple:
     """Utility function to get the tar.gz files and the directories
     at a given URL.
     """
     res = session.get(url)
```

### Comparing `roo-0.17.0/src/roo/sources/source_abc.py` & `roo-0.17.1/src/roo/sources/source_abc.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/sources/source_group.py` & `roo-0.17.1/src/roo/sources/source_group.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/sources/source_package.py` & `roo-0.17.1/src/roo/sources/source_package.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/src/roo/sources/vcs.py` & `roo-0.17.1/src/roo/sources/vcs.py`

 * *Files identical despite different names*

### Comparing `roo-0.17.0/PKG-INFO` & `roo-0.17.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roo
-Version: 0.17.0
+Version: 0.17.1
 Summary: A package manager to handle R environments
 Home-page: https://github.com/AstraZeneca/roo
 License: Apache-2.0
 Keywords: R,packaging,environment,validation
 Author: Stefano Borini
 Author-email: stefano.borini@astrazeneca.com
 Requires-Python: >=3.7,<4.0
@@ -13,14 +13,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: R
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: GitPython (>=3.1.13,<4.0.0)
 Requires-Dist: atomicwrites (>=1.4,<2.0)
 Requires-Dist: beautifulsoup4 (>=4.8.2,<5.0.0)
 Requires-Dist: click (>=7.0,<8.0)
 Requires-Dist: packaging (>=20.1,<21.0)
```

