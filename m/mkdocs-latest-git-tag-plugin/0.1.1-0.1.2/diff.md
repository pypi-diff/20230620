# Comparing `tmp/mkdocs_latest_git_tag_plugin-0.1.1.tar.gz` & `tmp/mkdocs_latest_git_tag_plugin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_latest_git_tag_plugin-0.1.1.tar", max compression
+gzip compressed data, was "mkdocs_latest_git_tag_plugin-0.1.2.tar", max compression
```

## Comparing `mkdocs_latest_git_tag_plugin-0.1.1.tar` & `mkdocs_latest_git_tag_plugin-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-06-19 18:33:38.830238 mkdocs_latest_git_tag_plugin-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1617 2023-06-20 16:23:50.892464 mkdocs_latest_git_tag_plugin-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-19 17:00:54.001145 mkdocs_latest_git_tag_plugin-0.1.1/mkdocs_latest_git_tag_plugin/__init__.py
--rw-r--r--   0        0        0     1394 2023-06-20 17:23:52.898788 mkdocs_latest_git_tag_plugin-0.1.1/mkdocs_latest_git_tag_plugin/plugin.py
--rw-r--r--   0        0        0     2810 2023-06-20 16:45:25.030718 mkdocs_latest_git_tag_plugin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3056 1970-01-01 00:00:00.000000 mkdocs_latest_git_tag_plugin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-19 18:33:38.830238 mkdocs_latest_git_tag_plugin-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     1617 2023-06-20 16:23:50.892464 mkdocs_latest_git_tag_plugin-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 17:00:54.001145 mkdocs_latest_git_tag_plugin-0.1.2/mkdocs_latest_git_tag_plugin/__init__.py
+-rw-r--r--   0        0        0     1394 2023-06-20 17:23:52.898788 mkdocs_latest_git_tag_plugin-0.1.2/mkdocs_latest_git_tag_plugin/plugin.py
+-rw-r--r--   0        0        0     2810 2023-06-20 17:45:23.376227 mkdocs_latest_git_tag_plugin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3056 1970-01-01 00:00:00.000000 mkdocs_latest_git_tag_plugin-0.1.2/PKG-INFO
```

### Comparing `mkdocs_latest_git_tag_plugin-0.1.1/LICENSE.txt` & `mkdocs_latest_git_tag_plugin-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_latest_git_tag_plugin-0.1.1/README.md` & `mkdocs_latest_git_tag_plugin-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_latest_git_tag_plugin-0.1.1/mkdocs_latest_git_tag_plugin/plugin.py` & `mkdocs_latest_git_tag_plugin-0.1.2/mkdocs_latest_git_tag_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_latest_git_tag_plugin-0.1.1/pyproject.toml` & `mkdocs_latest_git_tag_plugin-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "mkdocs-latest-git-tag-plugin"
-version = "0.1.1"
+version = "0.1.2"
 description = "MkDocs plugin to get the latest git tag from the local repository"
 authors = ["Grant Ramsay <seapagan@gmail.com>"]
 readme = "README.md"
 
-repository = "https://github.com/seapagan/mkdocs_latest_git_tag_plugin"
-homepage = "https://github.com/seapagan/mkdocs_latest_git_tag_plugin"
+repository = "https://github.com/seapagan/mkdocs-latest-git-tag-plugin"
+homepage = "https://github.com/seapagan/mkdocs-latest-git-tag-plugin"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
@@ -27,16 +27,16 @@
 
 packages = [{include = "mkdocs_latest_git_tag_plugin"}]
 
 [tool.poetry.plugins."mkdocs.plugins"]
 latest-git-tag = "mkdocs_latest_git_tag_plugin.plugin:LatestGitTagPlugin"
 
 [tool.poetry.urls]
-"Pull Requests" = "https://github.com/seapagan/mkdocs_latest_git_tag_plugin/pulls"
-"Bug Tracker" = "https://github.com/seapagan/mkdocs_latest_git_tag_plugin/issues"
+"Pull Requests" = "https://github.com/seapagan/mkdocs-latest-git-tag-plugin/pulls"
+"Bug Tracker" = "https://github.com/seapagan/mkdocs-latest-git-tag-plugin/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 mkdocs = "^1.4.3"
 gitpython = "^3.1.31"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `mkdocs_latest_git_tag_plugin-0.1.1/PKG-INFO` & `mkdocs_latest_git_tag_plugin-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mkdocs-latest-git-tag-plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: MkDocs plugin to get the latest git tag from the local repository
-Home-page: https://github.com/seapagan/mkdocs_latest_git_tag_plugin
+Home-page: https://github.com/seapagan/mkdocs-latest-git-tag-plugin
 Author: Grant Ramsay
 Author-email: seapagan@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,17 +19,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: mkdocs (>=1.4.3,<2.0.0)
-Project-URL: Bug Tracker, https://github.com/seapagan/mkdocs_latest_git_tag_plugin/issues
-Project-URL: Pull Requests, https://github.com/seapagan/mkdocs_latest_git_tag_plugin/pulls
-Project-URL: Repository, https://github.com/seapagan/mkdocs_latest_git_tag_plugin
+Project-URL: Bug Tracker, https://github.com/seapagan/mkdocs-latest-git-tag-plugin/issues
+Project-URL: Pull Requests, https://github.com/seapagan/mkdocs-latest-git-tag-plugin/pulls
+Project-URL: Repository, https://github.com/seapagan/mkdocs-latest-git-tag-plugin
 Description-Content-Type: text/markdown
 
 # MkDocs Plugin : `latest-git-tag`
 
 [![PyPI version](https://badge.fury.io/py/mkdocs-latest-git-tag-plugin.svg)](https://badge.fury.io/py/mkdocs-latest-git-tag-plugin)
 
 This is a simple [MkDocs](https://www.mkdocs.org/) plugin that just gets the
```

