# Comparing `tmp/content_tracker-0.0.2.tar.gz` & `tmp/content_tracker-0.1.0.tar.gz`

## Comparing `content_tracker-0.0.2.tar` & `content_tracker-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,26 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 content_tracker-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 content_tracker-0.0.2/Makefile
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 content_tracker-0.0.2/requirements.txt
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 content_tracker-0.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 content_tracker-0.0.2/.github/release.yml
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 content_tracker-0.0.2/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 content_tracker-0.0.2/src/content_tracker/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 content_tracker-0.0.2/src/content_tracker/_version.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 content_tracker-0.0.2/tests/test_version.py
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 content_tracker-0.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 content_tracker-0.0.2/LICENSE
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 content_tracker-0.0.2/README.md
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 content_tracker-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 content_tracker-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 content_tracker-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 content_tracker-0.1.0/Makefile
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 content_tracker-0.1.0/requirements.txt
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 content_tracker-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 content_tracker-0.1.0/.github/release.yml
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 content_tracker-0.1.0/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/_version.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/cli.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/main.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/models.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/databases/__init__.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/databases/base.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/databases/bigquery.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/databases/instance_store.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/notifiers/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/notifiers/base.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/notifiers/webhook.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/providers/__init__.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 content_tracker-0.1.0/src/content_tracker/providers/base.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 content_tracker-0.1.0/tests/test_version.py
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 content_tracker-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 content_tracker-0.1.0/LICENSE
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 content_tracker-0.1.0/README.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 content_tracker-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 content_tracker-0.1.0/PKG-INFO
```

### Comparing `content_tracker-0.0.2/.github/workflows/python-tests.yml` & `content_tracker-0.1.0/.github/workflows/python-tests.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 name: Python Tests
 
 on:
+  push:
+    branches: [main]
   pull_request:
   release:
     types: [published]
 
 jobs:
   build:
     runs-on: ubuntu-latest
@@ -47,30 +49,36 @@
       - name: Download artifact
         uses: actions/download-artifact@v3
         with:
           name: packages
           path: ./dist
 
       - name: Install dependencies
-        run: python3 -m pip install "$(find ./dist -name '*-py3-none-any.whl' | tail -1)[test]"
+        run: |
+          python3 -m pip install --upgrade pip setuptools wheel
+          python3 -m pip install -r ./requirements.txt
+          python3 -m pip install "$(find ./dist -name '*-py3-none-any.whl' | tail -1)[test]"
 
       - name: Test
         run: make test
 
       - name: Upload coverage reports
         uses: codecov/codecov-action@v3
 
   publish:
     needs: test
     if: github.event_name == 'release' && github.event.action == 'published'
+    permissions:
+      id-token: write
+    environment:
+      name: release
+      url: https://pypi.org/project/${{ github.event.repository.name }}/
     runs-on: ubuntu-latest
     steps:
       - name: Download artifact
         uses: actions/download-artifact@v3
         with:
           name: packages
           path: ./dist
 
       - name: Publish
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `content_tracker-0.0.2/.gitignore` & `content_tracker-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `content_tracker-0.0.2/LICENSE` & `content_tracker-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `content_tracker-0.0.2/README.md` & `content_tracker-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,7 +9,12 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/speg03/content-tracker/main.svg)](https://results.pre-commit.ci/latest/github/speg03/content-tracker/main)
 
 ## Installation
 
 ```console
 $ pip install content-tracker
 ```
+
+If you use BigQuery as database:
+```console
+$ pip install content-tracker[bigquery]
+```
```

### Comparing `content_tracker-0.0.2/pyproject.toml` & `content_tracker-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,18 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing",
 ]
 
 dynamic = ["version"]
 
-dependencies = []
+dependencies = ["typer>=0.9,<1.0"]
 
 [project.optional-dependencies]
+bigquery = ["google-cloud-bigquery~=3.10"]
 test = ["pytest", "pytest-cov"]
 
 [project.urls]
 Homepage = "https://github.com/speg03/content-tracker"
 Repository = "https://github.com/speg03/content-tracker"
 
 [tool.hatch.version]
```

### Comparing `content_tracker-0.0.2/PKG-INFO` & `content_tracker-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: content-tracker
-Version: 0.0.2
+Version: 0.1.0
 Summary: Tracking changes in arbitrary content.
 Project-URL: Homepage, https://github.com/speg03/content-tracker
 Project-URL: Repository, https://github.com/speg03/content-tracker
 Author-email: Takahiro Yano <speg03@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: changes,content,diff,tracking
@@ -17,14 +17,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.7
+Requires-Dist: typer<1.0,>=0.9
+Provides-Extra: bigquery
+Requires-Dist: google-cloud-bigquery~=3.10; extra == 'bigquery'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 # content-tracker
 
@@ -37,7 +40,12 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/speg03/content-tracker/main.svg)](https://results.pre-commit.ci/latest/github/speg03/content-tracker/main)
 
 ## Installation
 
 ```console
 $ pip install content-tracker
 ```
+
+If you use BigQuery as database:
+```console
+$ pip install content-tracker[bigquery]
+```
```

