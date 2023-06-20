# Comparing `tmp/scmrepo-1.0.3.tar.gz` & `tmp/scmrepo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmrepo-1.0.3.tar", last modified: Thu May  4 08:20:10 2023, max compression
+gzip compressed data, was "scmrepo-1.0.4.tar", last modified: Tue Jun 20 06:26:29 2023, max compression
```

## Comparing `scmrepo-1.0.3.tar` & `scmrepo-1.0.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.911702 scmrepo-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.903702 scmrepo-1.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.903702 scmrepo-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-04 08:19:43.000000 scmrepo-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-04 08:19:43.000000 scmrepo-1.0.3/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-04 08:19:43.000000 scmrepo-1.0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-04 08:19:43.000000 scmrepo-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-04 08:20:10.911702 scmrepo-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-04 08:19:43.000000 scmrepo-1.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-04 08:19:43.000000 scmrepo-1.0.3/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-04 08:19:43.000000 scmrepo-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-04 08:20:10.911702 scmrepo-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.899701 scmrepo-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.907702 scmrepo-1.0.3/src/scmrepo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/asyn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.907702 scmrepo-1.0.3/src/scmrepo/git/
--rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.907702 scmrepo-1.0.3/src/scmrepo/git/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.907702 scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/
--rw-r--r--   0 runner    (1001) docker     (123)    29311 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21888 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/gitpython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.907702 scmrepo-1.0.3/src/scmrepo/git/backend/pygit2/
--rw-r--r--   0 runner    (1001) docker     (123)    27611 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/pygit2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/backend/pygit2/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    20943 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/git/stash.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/noscm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-04 08:19:43.000000 scmrepo-1.0.3/src/scmrepo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.907702 scmrepo-1.0.3/src/scmrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-04 08:20:10.000000 scmrepo-1.0.3/src/scmrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-04 08:20:10.000000 scmrepo-1.0.3/src/scmrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:20:10.000000 scmrepo-1.0.3/src/scmrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:20:10.000000 scmrepo-1.0.3/src/scmrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-04 08:20:10.000000 scmrepo-1.0.3/src/scmrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 08:20:10.000000 scmrepo-1.0.3/src/scmrepo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.911702 scmrepo-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:20:10.911702 scmrepo-1.0.3/tests/git-init/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_dulwich.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34105 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_noscm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_pygit2.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_scmrepo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/test_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/user.key
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-04 08:19:43.000000 scmrepo-1.0.3/tests/user.key.pub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.901444 scmrepo-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.893444 scmrepo-1.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.893444 scmrepo-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-20 06:26:07.000000 scmrepo-1.0.4/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-20 06:26:07.000000 scmrepo-1.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-20 06:26:07.000000 scmrepo-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-20 06:26:29.901444 scmrepo-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-20 06:26:07.000000 scmrepo-1.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-20 06:26:07.000000 scmrepo-1.0.4/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-20 06:26:07.000000 scmrepo-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-20 06:26:29.901444 scmrepo-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.893444 scmrepo-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.897444 scmrepo-1.0.4/src/scmrepo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.897444 scmrepo-1.0.4/src/scmrepo/git/
+-rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.897444 scmrepo-1.0.4/src/scmrepo/git/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.897444 scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/
+-rw-r--r--   0 runner    (1001) docker     (123)    29311 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21888 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/gitpython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.897444 scmrepo-1.0.4/src/scmrepo/git/backend/pygit2/
+-rw-r--r--   0 runner    (1001) docker     (123)    27611 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/pygit2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/pygit2/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20986 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/noscm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.897444 scmrepo-1.0.4/src/scmrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-20 06:26:29.000000 scmrepo-1.0.4/src/scmrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-20 06:26:29.000000 scmrepo-1.0.4/src/scmrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 06:26:29.000000 scmrepo-1.0.4/src/scmrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 06:26:29.000000 scmrepo-1.0.4/src/scmrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-20 06:26:29.000000 scmrepo-1.0.4/src/scmrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 06:26:29.000000 scmrepo-1.0.4/src/scmrepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.901444 scmrepo-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.901444 scmrepo-1.0.4/tests/git-init/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_dulwich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34105 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_noscm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_pygit2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_scmrepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/user.key
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/user.key.pub
```

### Comparing `scmrepo-1.0.3/.cruft.json` & `scmrepo-1.0.4/.cruft.json`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/.github/dependabot.yml` & `scmrepo-1.0.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/.github/workflows/release.yaml` & `scmrepo-1.0.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/.github/workflows/tests.yaml` & `scmrepo-1.0.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/.gitignore` & `scmrepo-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/.pre-commit-config.yaml` & `scmrepo-1.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/CODE_OF_CONDUCT.rst` & `scmrepo-1.0.4/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/CONTRIBUTING.rst` & `scmrepo-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/LICENSE` & `scmrepo-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/PKG-INFO` & `scmrepo-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 1.0.3
+Version: 1.0.4
 Summary: SCM wrapper and fsspec filesystem for Git for use in DVC
 Home-page: https://github.com/iterative/scmrepo
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scmrepo-1.0.3/README.rst` & `scmrepo-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/noxfile.py` & `scmrepo-1.0.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/pyproject.toml` & `scmrepo-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/setup.cfg` & `scmrepo-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 	pytest-test-utils==0.0.8
 	pytest-asyncio==0.18.3
 	pytest-docker==0.12.0; python_version < '3.10' or sys_platform != 'win32'
 	mock==5.0.1
 	paramiko==3.1.0
 	types-certifi==2021.10.8.3
 	types-mock==5.0.0.6
-	types-paramiko==3.0.0.7
+	types-paramiko==3.0.0.10
 dev = 
 	%(tests)s
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
```

### Comparing `scmrepo-1.0.3/src/scmrepo/asyn.py` & `scmrepo-1.0.4/src/scmrepo/asyn.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/base.py` & `scmrepo-1.0.4/src/scmrepo/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/exceptions.py` & `scmrepo-1.0.4/src/scmrepo/exceptions.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/fs.py` & `scmrepo-1.0.4/src/scmrepo/fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/git/__init__.py` & `scmrepo-1.0.4/src/scmrepo/git/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/git/backend/base.py` & `scmrepo-1.0.4/src/scmrepo/git/backend/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/__init__.py` & `scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py` & `scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/git/backend/dulwich/client.py` & `scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/client.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/git/backend/gitpython.py` & `scmrepo-1.0.4/src/scmrepo/git/backend/gitpython.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/git/backend/pygit2/__init__.py` & `scmrepo-1.0.4/src/scmrepo/git/backend/pygit2/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/git/backend/pygit2/callbacks.py` & `scmrepo-1.0.4/src/scmrepo/git/backend/pygit2/callbacks.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/git/credentials.py` & `scmrepo-1.0.4/src/scmrepo/git/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         helper_input.append("")
 
         try:
             res = subprocess.run(  # type: ignore # nosec B603 # breaks on 3.6
                 cmd,
                 check=True,
                 capture_output=True,
-                input=os.linesep.join(helper_input),
+                input="\n".join(helper_input),
                 encoding=self._encoding,
                 **self._run_kwargs,
             )
         except subprocess.CalledProcessError as exc:
             raise CredentialNotFoundError(exc.stderr) from exc
         except FileNotFoundError as exc:
             raise CredentialNotFoundError("Helper not found") from exc
@@ -200,15 +200,15 @@
         ]
         helper_input.append("")
 
         try:
             res = subprocess.run(  # type: ignore # nosec B603 # pylint: disable=W1510
                 cmd,
                 capture_output=True,
-                input=os.linesep.join(helper_input),
+                input="\n".join(helper_input),
                 encoding=self._encoding,
                 **self._run_kwargs,
             )
             if res.stderr:
                 logger.debug(res.stderr)
         except FileNotFoundError:
             logger.debug("Helper not found", exc_info=True)
@@ -224,15 +224,15 @@
         ]
         helper_input.append("")
 
         try:
             res = subprocess.run(  # type: ignore # nosec B603 # pylint: disable=W1510
                 cmd,
                 capture_output=True,
-                input=os.linesep.join(helper_input),
+                input="\n".join(helper_input),
                 encoding=self._encoding,
                 **self._run_kwargs,
             )
             if res.stderr:
                 logger.debug(res.stderr)
         except FileNotFoundError:
             logger.debug("Helper not found", exc_info=True)
@@ -252,14 +252,16 @@
             # falling back to the generic section if there's no match
             for section in urlmatch_credential_sections(conf, base_url):
                 try:
                     command = conf.get(section, "helper")
                 except KeyError:
                     # no helper configured
                     continue
+                if not command:
+                    continue
                 use_http_path = conf.get_boolean(section, "usehttppath", False)
                 yield (
                     command.decode(conf.encoding or sys.getdefaultencoding()),
                     use_http_path,
                 )
```

### Comparing `scmrepo-1.0.3/src/scmrepo/git/objects.py` & `scmrepo-1.0.4/src/scmrepo/git/objects.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/git/stash.py` & `scmrepo-1.0.4/src/scmrepo/git/stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/progress.py` & `scmrepo-1.0.4/src/scmrepo/progress.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo/utils.py` & `scmrepo-1.0.4/src/scmrepo/utils.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo.egg-info/PKG-INFO` & `scmrepo-1.0.4/src/scmrepo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 1.0.3
+Version: 1.0.4
 Summary: SCM wrapper and fsspec filesystem for Git for use in DVC
 Home-page: https://github.com/iterative/scmrepo
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scmrepo-1.0.3/src/scmrepo.egg-info/SOURCES.txt` & `scmrepo-1.0.4/src/scmrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/src/scmrepo.egg-info/requires.txt` & `scmrepo-1.0.4/src/scmrepo.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 mypy==0.971
 pytest-test-utils==0.0.8
 pytest-asyncio==0.18.3
 mock==5.0.1
 paramiko==3.1.0
 types-certifi==2021.10.8.3
 types-mock==5.0.0.6
-types-paramiko==3.0.0.7
+types-paramiko==3.0.0.10
 
 [dev:python_version < "3.10" or sys_platform != "win32"]
 pytest-docker==0.12.0
 
 [tests]
 pytest==7.2.0
 pytest-sugar==0.9.5
@@ -35,11 +35,11 @@
 mypy==0.971
 pytest-test-utils==0.0.8
 pytest-asyncio==0.18.3
 mock==5.0.1
 paramiko==3.1.0
 types-certifi==2021.10.8.3
 types-mock==5.0.0.6
-types-paramiko==3.0.0.7
+types-paramiko==3.0.0.10
 
 [tests:python_version < "3.10" or sys_platform != "win32"]
 pytest-docker==0.12.0
```

### Comparing `scmrepo-1.0.3/tests/conftest.py` & `scmrepo-1.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/tests/test_credentials.py` & `scmrepo-1.0.4/tests/test_credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,73 +17,73 @@
     return GitCredentialHelper("foo")
 
 
 def test_subprocess_get(git_helper, mocker):
     run = mocker.patch(
         "subprocess.run",
         return_value=mocker.Mock(
-            stdout=os.linesep.join(
+            stdout="\n".join(
                 ["protocol=https", "host=foo.com", "username=foo", "password=bar", ""]
             )
         ),
     )
     creds = git_helper.get(Credential(protocol="https", host="foo.com", path="foo.git"))
     assert run.call_args.args[0] == ["git-credential-foo", "get"]
-    assert run.call_args.kwargs.get("input") == os.linesep.join(
+    assert run.call_args.kwargs.get("input") == "\n".join(
         ["protocol=https", "host=foo.com", ""]
     )
     assert creds == Credential(url="https://foo:bar@foo.com")
 
 
 def test_subprocess_get_use_http_path(git_helper, mocker):
     git_helper.use_http_path = True
     run = mocker.patch(
         "subprocess.run",
         return_value=mocker.Mock(
-            stdout=os.linesep.join(["username=foo", "password=bar", ""])
+            stdout="\n".join(["username=foo", "password=bar", ""])
         ),
     )
     creds = git_helper.get(Credential(protocol="https", host="foo.com", path="foo.git"))
     assert run.call_args.args[0] == ["git-credential-foo", "get"]
-    assert run.call_args.kwargs.get("input") == os.linesep.join(
+    assert run.call_args.kwargs.get("input") == "\n".join(
         ["protocol=https", "host=foo.com", "path=foo.git", ""]
     )
     assert creds == Credential(username="foo", password="bar")
 
 
 def test_subprocess_get_failed(git_helper, mocker):
     from subprocess import CalledProcessError
 
     mocker.patch("subprocess.run", side_effect=CalledProcessError(1, "/usr/bin/foo"))
     with pytest.raises(CredentialNotFoundError):
         git_helper.get(Credential(protocol="https", host="foo.com"))
 
 
 def test_subprocess_get_no_output(git_helper, mocker):
-    mocker.patch("subprocess.run", return_value=mocker.Mock(stdout=os.linesep))
+    mocker.patch("subprocess.run", return_value=mocker.Mock(stdout="\n"))
     with pytest.raises(CredentialNotFoundError):
         git_helper.get(Credential(protocol="https", host="foo.com"))
 
 
 def test_subprocess_store(git_helper, mocker):
     run = mocker.patch("subprocess.run")
     git_helper.store(
         Credential(protocol="https", host="foo.com", username="foo", password="bar")
     )
     assert run.call_args.args[0] == ["git-credential-foo", "store"]
-    assert run.call_args.kwargs.get("input") == os.linesep.join(
+    assert run.call_args.kwargs.get("input") == "\n".join(
         ["protocol=https", "host=foo.com", "username=foo", "password=bar", ""]
     )
 
 
 def test_subprocess_erase(git_helper, mocker):
     run = mocker.patch("subprocess.run")
     git_helper.erase(Credential(protocol="https", host="foo.com"))
     assert run.call_args.args[0] == ["git-credential-foo", "erase"]
-    assert run.call_args.kwargs.get("input") == os.linesep.join(
+    assert run.call_args.kwargs.get("input") == "\n".join(
         ["protocol=https", "host=foo.com", ""]
     )
 
 
 def test_memory_helper_get(mocker):
     from getpass import getpass
 
@@ -145,15 +145,15 @@
 def test_memory_helper_prompt_askpass(mocker):
     helper = MemoryCredentialHelper()
     mocker.patch.dict(os.environ, {"GIT_ASKPASS": "/usr/local/bin/my-askpass"})
     run = mocker.patch(
         "subprocess.run",
         side_effect=[
             mocker.Mock(stdout="foo"),
-            mocker.Mock(stdout=os.linesep.join(["bar", ""])),
+            mocker.Mock(stdout="\n".join(["bar", ""])),
         ],
     )
     expected = Credential(
         protocol="https", host="foo.com", username="foo", password="bar"
     )
     assert (
         helper.get(Credential(protocol="https", host="foo.com"), interactive=True)
@@ -197,7 +197,24 @@
         )
     )
     config_file.seek(0)
     config = ConfigFile.from_file(config_file)
     assert list(
         GitCredentialHelper.get_matching_commands("https://foo.com/foo.git", config)
     ) == [("/usr/local/bin/my-helper", False)]
+
+    config_file = io.BytesIO(
+        """
+[credential]
+    helper =
+""".encode(
+            "ascii"
+        )
+    )
+    config_file.seek(0)
+    config = ConfigFile.from_file(config_file)
+    assert (
+        list(
+            GitCredentialHelper.get_matching_commands("https://foo.com/foo.git", config)
+        )
+        == []
+    )
```

### Comparing `scmrepo-1.0.3/tests/test_dulwich.py` & `scmrepo-1.0.4/tests/test_dulwich.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/tests/test_fs.py` & `scmrepo-1.0.4/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/tests/test_git.py` & `scmrepo-1.0.4/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/tests/test_noscm.py` & `scmrepo-1.0.4/tests/test_noscm.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/tests/test_pygit2.py` & `scmrepo-1.0.4/tests/test_pygit2.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/tests/test_scmrepo.py` & `scmrepo-1.0.4/tests/test_scmrepo.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/tests/test_stash.py` & `scmrepo-1.0.4/tests/test_stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.3/tests/user.key` & `scmrepo-1.0.4/tests/user.key`

 * *Files identical despite different names*

