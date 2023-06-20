# Comparing `tmp/slap_cli-1.9.6.tar.gz` & `tmp/slap_cli-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slap_cli-1.9.6.tar", max compression
+gzip compressed data, was "slap_cli-1.9.7.tar", max compression
```

## Comparing `slap_cli-1.9.6.tar` & `slap_cli-1.9.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1002 2023-01-29 11:43:11.729548 slap_cli-1.9.6/LICENSE
--rw-r--r--   0        0        0     4981 2023-06-19 22:42:33.057597 slap_cli-1.9.6/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-19 22:42:33.057597 slap_cli-1.9.6/src/slap/__init__.py
--rw-r--r--   0        0        0      122 2023-05-15 14:08:15.856560 slap_cli-1.9.6/src/slap/__main__.py
--rw-r--r--   0        0        0    13007 2023-06-19 22:41:08.284988 slap_cli-1.9.6/src/slap/application.py
--rw-r--r--   0        0        0     9163 2023-02-09 13:39:04.453992 slap_cli-1.9.6/src/slap/changelog.py
--rw-r--r--   0        0        0     3353 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/check.py
--rw-r--r--   0        0        0     2533 2023-05-15 15:02:36.078985 slap_cli-1.9.6/src/slap/configuration.py
--rw-r--r--   0        0        0     5337 2023-05-15 13:54:26.739024 slap_cli-1.9.6/src/slap/ext/application/add.py
--rw-r--r--   0        0        0    27292 2023-05-15 16:43:58.997086 slap_cli-1.9.6/src/slap/ext/application/changelog.py
--rw-r--r--   0        0        0     6330 2023-05-15 14:28:58.852972 slap_cli-1.9.6/src/slap/ext/application/check.py
--rw-r--r--   0        0        0     3177 2023-05-15 14:02:47.957819 slap_cli-1.9.6/src/slap/ext/application/info.py
--rw-r--r--   0        0        0     4911 2023-05-19 08:24:24.059256 slap_cli-1.9.6/src/slap/ext/application/init.py
--rw-r--r--   0        0        0    13694 2023-06-19 22:40:02.624511 slap_cli-1.9.6/src/slap/ext/application/install.py
--rw-r--r--   0        0        0     5982 2023-05-15 14:16:35.467350 slap_cli-1.9.6/src/slap/ext/application/link.py
--rw-r--r--   0        0        0     4230 2023-05-15 14:29:48.828826 slap_cli-1.9.6/src/slap/ext/application/publish.py
--rw-r--r--   0        0        0    21667 2023-05-15 14:33:39.328295 slap_cli-1.9.6/src/slap/ext/application/release.py
--rw-r--r--   0        0        0     3243 2023-05-15 14:30:47.388698 slap_cli-1.9.6/src/slap/ext/application/report.py
--rw-r--r--   0        0        0     3555 2023-05-15 14:59:30.475460 slap_cli-1.9.6/src/slap/ext/application/run.py
--rw-r--r--   0        0        0     8129 2023-06-19 22:37:07.591338 slap_cli-1.9.6/src/slap/ext/application/test.py
--rw-r--r--   0        0        0    19880 2023-05-15 14:20:06.182817 slap_cli-1.9.6/src/slap/ext/application/venv.py
--rw-r--r--   0        0        0     2075 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/ext/checks/changelog.py
--rw-r--r--   0        0        0     2215 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/ext/checks/general.py
--rw-r--r--   0        0        0     6060 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/ext/checks/poetry.py
--rw-r--r--   0        0        0     2815 2023-05-15 14:08:26.480527 slap_cli-1.9.6/src/slap/ext/checks/release.py
--rw-r--r--   0        0        0     8491 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/ext/project_handlers/base.py
--rw-r--r--   0        0        0     3799 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/ext/project_handlers/flit.py
--rw-r--r--   0        0        0     6462 2023-05-15 13:23:04.316661 slap_cli-1.9.6/src/slap/ext/project_handlers/poetry.py
--rw-r--r--   0        0        0     5751 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/ext/project_handlers/setuptools.py
--rw-r--r--   0        0        0     1208 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/ext/release/changelog.py
--rw-r--r--   0        0        0     2046 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/ext/release/source_code_version.py
--rw-r--r--   0        0        0    16205 2023-05-15 13:23:04.316661 slap_cli-1.9.6/src/slap/ext/repository_ci/github_actions.py
--rw-r--r--   0        0        0     4065 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/ext/repository_handlers/default.py
--rw-r--r--   0        0        0     4479 2023-02-20 12:50:15.737708 slap_cli-1.9.6/src/slap/ext/repository_hosts/github.py
--rw-r--r--   0        0        0     1357 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/ext/version_incrementing_rule.py
--rw-r--r--   0        0        0    10869 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/install/installer.py
--rw-r--r--   0        0        0     8308 2023-05-15 13:52:59.875225 slap_cli-1.9.6/src/slap/plugins.py
--rw-r--r--   0        0        0     8623 2023-05-15 15:05:38.122588 slap_cli-1.9.6/src/slap/project.py
--rw-r--r--   0        0        0        0 2023-01-29 11:43:11.729548 slap_cli-1.9.6/src/slap/py.typed
--rw-r--r--   0        0        0    14965 2023-05-15 13:23:04.316661 slap_cli-1.9.6/src/slap/python/dependency.py
--rw-r--r--   0        0        0     9711 2023-01-29 11:43:11.733548 slap_cli-1.9.6/src/slap/python/environment.py
--rw-r--r--   0        0        0     6833 2023-01-29 11:43:11.733548 slap_cli-1.9.6/src/slap/python/pep508.py
--rw-r--r--   0        0        0     2535 2023-01-29 11:43:11.733548 slap_cli-1.9.6/src/slap/release.py
--rw-r--r--   0        0        0     5629 2023-05-15 15:05:54.734548 slap_cli-1.9.6/src/slap/repository.py
--rw-r--r--   0        0        0     1091 2023-05-15 13:23:04.316661 slap_cli-1.9.6/src/slap/templates/github/.github/workflows/changelog.yaml
--rw-r--r--   0        0        0      972 2023-05-15 13:23:04.316661 slap_cli-1.9.6/src/slap/templates/github/.github/workflows/python.yaml
--rw-r--r--   0        0        0      246 2023-05-15 13:23:04.316661 slap_cli-1.9.6/src/slap/templates/poetry/.flake8
--rw-r--r--   0        0        0       78 2023-05-15 13:23:04.316661 slap_cli-1.9.6/src/slap/templates/poetry/.gitignore
--rw-r--r--   0        0        0        0 2023-05-15 13:23:04.316661 slap_cli-1.9.6/src/slap/templates/poetry/LICENSE
--rw-r--r--   0        0        0        9 2023-05-15 13:23:04.316661 slap_cli-1.9.6/src/slap/templates/poetry/README.md
--rw-r--r--   0        0        0     1472 2023-05-19 08:33:11.881692 slap_cli-1.9.6/src/slap/templates/poetry/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-15 13:23:04.320661 slap_cli-1.9.6/src/slap/templates/poetry/src/{path}/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 13:23:04.320661 slap_cli-1.9.6/src/slap/templates/poetry/src/{path}/py.typed
--rw-r--r--   0        0        0       67 2023-05-15 13:23:04.320661 slap_cli-1.9.6/src/slap/templates/poetry/tests/test_import.py
--rw-r--r--   0        0        0     1847 2023-01-29 11:43:11.733548 slap_cli-1.9.6/src/slap/util/cleo.py
--rw-r--r--   0        0        0     4309 2023-01-29 11:43:11.733548 slap_cli-1.9.6/src/slap/util/external/licenses.py
--rw-r--r--   0        0        0     2172 2023-01-29 11:43:11.733548 slap_cli-1.9.6/src/slap/util/external/pypi_classifiers.py
--rw-r--r--   0        0        0      418 2023-01-29 11:43:11.733548 slap_cli-1.9.6/src/slap/util/pygments.py
--rw-r--r--   0        0        0      114 2023-06-19 22:37:07.591338 slap_cli-1.9.6/src/slap/util/strings.py
--rw-r--r--   0        0        0     2113 2023-01-29 11:43:11.733548 slap_cli-1.9.6/src/slap/util/toml_file.py
--rw-r--r--   0        0        0     7363 2023-01-29 11:43:11.733548 slap_cli-1.9.6/src/slap/util/vcs.py
--rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 slap_cli-1.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-06-20 13:32:58.376097 slap_cli-1.9.7/LICENSE
+-rw-r--r--   0        0        0     4981 2023-06-20 13:36:00.993760 slap_cli-1.9.7/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-20 13:36:00.993967 slap_cli-1.9.7/src/slap/__init__.py
+-rw-r--r--   0        0        0      122 2023-06-20 13:32:58.383372 slap_cli-1.9.7/src/slap/__main__.py
+-rw-r--r--   0        0        0    13007 2023-06-20 13:32:58.383633 slap_cli-1.9.7/src/slap/application.py
+-rw-r--r--   0        0        0     9163 2023-06-20 13:32:58.383917 slap_cli-1.9.7/src/slap/changelog.py
+-rw-r--r--   0        0        0     3353 2023-06-20 13:32:58.384178 slap_cli-1.9.7/src/slap/check.py
+-rw-r--r--   0        0        0     2533 2023-06-20 13:32:58.384343 slap_cli-1.9.7/src/slap/configuration.py
+-rw-r--r--   0        0        0     5337 2023-06-20 13:32:58.384694 slap_cli-1.9.7/src/slap/ext/application/add.py
+-rw-r--r--   0        0        0    27292 2023-06-20 13:32:58.384909 slap_cli-1.9.7/src/slap/ext/application/changelog.py
+-rw-r--r--   0        0        0     6330 2023-06-20 13:32:58.385071 slap_cli-1.9.7/src/slap/ext/application/check.py
+-rw-r--r--   0        0        0     3177 2023-06-20 13:32:58.385320 slap_cli-1.9.7/src/slap/ext/application/info.py
+-rw-r--r--   0        0        0     4976 2023-06-20 13:35:56.901718 slap_cli-1.9.7/src/slap/ext/application/init.py
+-rw-r--r--   0        0        0    13694 2023-06-20 13:32:58.385666 slap_cli-1.9.7/src/slap/ext/application/install.py
+-rw-r--r--   0        0        0     5982 2023-06-20 13:32:58.385828 slap_cli-1.9.7/src/slap/ext/application/link.py
+-rw-r--r--   0        0        0     4230 2023-06-20 13:32:58.385968 slap_cli-1.9.7/src/slap/ext/application/publish.py
+-rw-r--r--   0        0        0    21667 2023-06-20 13:32:58.386154 slap_cli-1.9.7/src/slap/ext/application/release.py
+-rw-r--r--   0        0        0     3243 2023-06-20 13:32:58.386321 slap_cli-1.9.7/src/slap/ext/application/report.py
+-rw-r--r--   0        0        0     3555 2023-06-20 13:32:58.386460 slap_cli-1.9.7/src/slap/ext/application/run.py
+-rw-r--r--   0        0        0     8129 2023-06-20 13:32:58.386638 slap_cli-1.9.7/src/slap/ext/application/test.py
+-rw-r--r--   0        0        0    19880 2023-06-20 13:32:58.386830 slap_cli-1.9.7/src/slap/ext/application/venv.py
+-rw-r--r--   0        0        0     2075 2023-06-20 13:32:58.387077 slap_cli-1.9.7/src/slap/ext/checks/changelog.py
+-rw-r--r--   0        0        0     2215 2023-06-20 13:32:58.387231 slap_cli-1.9.7/src/slap/ext/checks/general.py
+-rw-r--r--   0        0        0     6060 2023-06-20 13:32:58.387435 slap_cli-1.9.7/src/slap/ext/checks/poetry.py
+-rw-r--r--   0        0        0     2815 2023-06-20 13:32:58.387611 slap_cli-1.9.7/src/slap/ext/checks/release.py
+-rw-r--r--   0        0        0     8491 2023-06-20 13:32:58.387962 slap_cli-1.9.7/src/slap/ext/project_handlers/base.py
+-rw-r--r--   0        0        0     3799 2023-06-20 13:32:58.388144 slap_cli-1.9.7/src/slap/ext/project_handlers/flit.py
+-rw-r--r--   0        0        0     6462 2023-06-20 13:32:58.388289 slap_cli-1.9.7/src/slap/ext/project_handlers/poetry.py
+-rw-r--r--   0        0        0     5751 2023-06-20 13:32:58.388545 slap_cli-1.9.7/src/slap/ext/project_handlers/setuptools.py
+-rw-r--r--   0        0        0     1208 2023-06-20 13:32:58.388913 slap_cli-1.9.7/src/slap/ext/release/changelog.py
+-rw-r--r--   0        0        0     2046 2023-06-20 13:32:58.389104 slap_cli-1.9.7/src/slap/ext/release/source_code_version.py
+-rw-r--r--   0        0        0    16205 2023-06-20 13:32:58.389458 slap_cli-1.9.7/src/slap/ext/repository_ci/github_actions.py
+-rw-r--r--   0        0        0     4065 2023-06-20 13:32:58.389756 slap_cli-1.9.7/src/slap/ext/repository_handlers/default.py
+-rw-r--r--   0        0        0     4479 2023-06-20 13:32:58.390092 slap_cli-1.9.7/src/slap/ext/repository_hosts/github.py
+-rw-r--r--   0        0        0     1357 2023-06-20 13:32:58.390281 slap_cli-1.9.7/src/slap/ext/version_incrementing_rule.py
+-rw-r--r--   0        0        0    10869 2023-06-20 13:32:58.390802 slap_cli-1.9.7/src/slap/install/installer.py
+-rw-r--r--   0        0        0     8308 2023-06-20 13:32:58.391026 slap_cli-1.9.7/src/slap/plugins.py
+-rw-r--r--   0        0        0     8623 2023-06-20 13:32:58.391199 slap_cli-1.9.7/src/slap/project.py
+-rw-r--r--   0        0        0        0 2023-06-20 13:32:58.391288 slap_cli-1.9.7/src/slap/py.typed
+-rw-r--r--   0        0        0    14965 2023-06-20 13:32:58.391567 slap_cli-1.9.7/src/slap/python/dependency.py
+-rw-r--r--   0        0        0     9711 2023-06-20 13:32:58.391728 slap_cli-1.9.7/src/slap/python/environment.py
+-rw-r--r--   0        0        0     6833 2023-06-20 13:32:58.391915 slap_cli-1.9.7/src/slap/python/pep508.py
+-rw-r--r--   0        0        0     2535 2023-06-20 13:32:58.392086 slap_cli-1.9.7/src/slap/release.py
+-rw-r--r--   0        0        0     5629 2023-06-20 13:32:58.392231 slap_cli-1.9.7/src/slap/repository.py
+-rw-r--r--   0        0        0     1091 2023-06-20 13:32:58.392906 slap_cli-1.9.7/src/slap/templates/github/.github/workflows/changelog.yaml
+-rw-r--r--   0        0        0      972 2023-06-20 13:32:58.393041 slap_cli-1.9.7/src/slap/templates/github/.github/workflows/python.yaml
+-rw-r--r--   0        0        0      246 2023-06-20 13:32:58.393303 slap_cli-1.9.7/src/slap/templates/poetry/.flake8
+-rw-r--r--   0        0        0       78 2023-06-20 13:32:58.393479 slap_cli-1.9.7/src/slap/templates/poetry/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-20 13:32:58.393569 slap_cli-1.9.7/src/slap/templates/poetry/LICENSE
+-rw-r--r--   0        0        0        9 2023-06-20 13:32:58.393696 slap_cli-1.9.7/src/slap/templates/poetry/README.md
+-rw-r--r--   0        0        0     1472 2023-06-20 13:32:58.393819 slap_cli-1.9.7/src/slap/templates/poetry/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-20 13:32:58.394288 slap_cli-1.9.7/src/slap/templates/poetry/src/{path}/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 13:32:58.394392 slap_cli-1.9.7/src/slap/templates/poetry/src/{path}/py.typed
+-rw-r--r--   0        0        0       67 2023-06-20 13:32:58.394614 slap_cli-1.9.7/src/slap/templates/poetry/tests/test_import.py
+-rw-r--r--   0        0        0     1847 2023-06-20 13:32:58.394937 slap_cli-1.9.7/src/slap/util/cleo.py
+-rw-r--r--   0        0        0     4309 2023-06-20 13:32:58.395513 slap_cli-1.9.7/src/slap/util/external/licenses.py
+-rw-r--r--   0        0        0     2172 2023-06-20 13:32:58.395768 slap_cli-1.9.7/src/slap/util/external/pypi_classifiers.py
+-rw-r--r--   0        0        0      418 2023-06-20 13:32:58.395903 slap_cli-1.9.7/src/slap/util/pygments.py
+-rw-r--r--   0        0        0      114 2023-06-20 13:32:58.396186 slap_cli-1.9.7/src/slap/util/strings.py
+-rw-r--r--   0        0        0     2113 2023-06-20 13:32:58.396434 slap_cli-1.9.7/src/slap/util/toml_file.py
+-rw-r--r--   0        0        0     7363 2023-06-20 13:32:58.396668 slap_cli-1.9.7/src/slap/util/vcs.py
+-rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 slap_cli-1.9.7/PKG-INFO
```

### Comparing `slap_cli-1.9.6/LICENSE` & `slap_cli-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/pyproject.toml` & `slap_cli-1.9.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "slap-cli"
-version = "1.9.6"
+version = "1.9.7"
 description = "Slap is a command-line utility for developing Python applications."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 packages = [{ include = "slap", from = "src" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
```

### Comparing `slap_cli-1.9.6/src/slap/application.py` & `slap_cli-1.9.7/src/slap/application.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/changelog.py` & `slap_cli-1.9.7/src/slap/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/check.py` & `slap_cli-1.9.7/src/slap/check.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/configuration.py` & `slap_cli-1.9.7/src/slap/configuration.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/application/add.py` & `slap_cli-1.9.7/src/slap/ext/application/add.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/application/changelog.py` & `slap_cli-1.9.7/src/slap/ext/application/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/application/check.py` & `slap_cli-1.9.7/src/slap/ext/application/check.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/application/info.py` & `slap_cli-1.9.7/src/slap/ext/application/info.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/application/init.py` & `slap_cli-1.9.7/src/slap/ext/application/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
     import slap
 
     path = Path(slap.__file__).parent / "templates" / name
     for filename in path.glob("**/*"):
         if filename.is_dir():
             continue
+        if "__pycache__" in filename.parts:
+            continue
         yield str(filename.relative_to(path)), filename.read_text()
 
 
 class InitCommandPlugin(Command, ApplicationPlugin):
     """Bootstrap some files for a Python project.
 
     Currently available templates:
```

### Comparing `slap_cli-1.9.6/src/slap/ext/application/install.py` & `slap_cli-1.9.7/src/slap/ext/application/install.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/application/link.py` & `slap_cli-1.9.7/src/slap/ext/application/link.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/application/publish.py` & `slap_cli-1.9.7/src/slap/ext/application/publish.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/application/release.py` & `slap_cli-1.9.7/src/slap/ext/application/release.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/application/report.py` & `slap_cli-1.9.7/src/slap/ext/application/report.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/application/run.py` & `slap_cli-1.9.7/src/slap/ext/application/run.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/application/test.py` & `slap_cli-1.9.7/src/slap/ext/application/test.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/application/venv.py` & `slap_cli-1.9.7/src/slap/ext/application/venv.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/checks/changelog.py` & `slap_cli-1.9.7/src/slap/ext/checks/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/checks/general.py` & `slap_cli-1.9.7/src/slap/ext/checks/general.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/checks/poetry.py` & `slap_cli-1.9.7/src/slap/ext/checks/poetry.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/checks/release.py` & `slap_cli-1.9.7/src/slap/ext/checks/release.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/project_handlers/base.py` & `slap_cli-1.9.7/src/slap/ext/project_handlers/base.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/project_handlers/flit.py` & `slap_cli-1.9.7/src/slap/ext/project_handlers/flit.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/project_handlers/poetry.py` & `slap_cli-1.9.7/src/slap/ext/project_handlers/poetry.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/project_handlers/setuptools.py` & `slap_cli-1.9.7/src/slap/ext/project_handlers/setuptools.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/release/changelog.py` & `slap_cli-1.9.7/src/slap/ext/release/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/release/source_code_version.py` & `slap_cli-1.9.7/src/slap/ext/release/source_code_version.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/repository_ci/github_actions.py` & `slap_cli-1.9.7/src/slap/ext/repository_ci/github_actions.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/repository_handlers/default.py` & `slap_cli-1.9.7/src/slap/ext/repository_handlers/default.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/repository_hosts/github.py` & `slap_cli-1.9.7/src/slap/ext/repository_hosts/github.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/ext/version_incrementing_rule.py` & `slap_cli-1.9.7/src/slap/ext/version_incrementing_rule.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/install/installer.py` & `slap_cli-1.9.7/src/slap/install/installer.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/plugins.py` & `slap_cli-1.9.7/src/slap/plugins.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/project.py` & `slap_cli-1.9.7/src/slap/project.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/python/dependency.py` & `slap_cli-1.9.7/src/slap/python/dependency.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/python/environment.py` & `slap_cli-1.9.7/src/slap/python/environment.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/python/pep508.py` & `slap_cli-1.9.7/src/slap/python/pep508.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/release.py` & `slap_cli-1.9.7/src/slap/release.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/repository.py` & `slap_cli-1.9.7/src/slap/repository.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/templates/github/.github/workflows/changelog.yaml` & `slap_cli-1.9.7/src/slap/templates/github/.github/workflows/changelog.yaml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/templates/github/.github/workflows/python.yaml` & `slap_cli-1.9.7/src/slap/templates/github/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/templates/poetry/pyproject.toml` & `slap_cli-1.9.7/src/slap/templates/poetry/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/util/cleo.py` & `slap_cli-1.9.7/src/slap/util/cleo.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/util/external/licenses.py` & `slap_cli-1.9.7/src/slap/util/external/licenses.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/util/external/pypi_classifiers.py` & `slap_cli-1.9.7/src/slap/util/external/pypi_classifiers.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/util/toml_file.py` & `slap_cli-1.9.7/src/slap/util/toml_file.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/src/slap/util/vcs.py` & `slap_cli-1.9.7/src/slap/util/vcs.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.6/PKG-INFO` & `slap_cli-1.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slap-cli
-Version: 1.9.6
+Version: 1.9.7
 Summary: Slap is a command-line utility for developing Python applications.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

