# Comparing `tmp/microsoft_kiota_http-0.4.3.tar.gz` & `tmp/microsoft_kiota_http-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft_kiota_http-0.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "microsoft_kiota_http-0.4.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft_kiota_http-0.4.3.tar` & `microsoft_kiota_http-0.4.4.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0      117 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1800 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.github/workflows/build_publish.yml
--rw-r--r--   0        0        0     2538 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.gitignore
--rw-r--r--   0        0        0    15946 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.pylintrc
--rw-r--r--   0        0        0     1108 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/LICENSE
--rw-r--r--   0        0        0      447 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/Pipfile
--rw-r--r--   0        0        0    39758 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/Pipfile.lock
--rw-r--r--   0        0        0     2376 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/README.md
--rw-r--r--   0        0        0     2757 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/SUPPORT.md
--rw-r--r--   0        0        0      121 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/__init__.py
--rw-r--r--   0        0        0       23 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/_version.py
--rw-r--r--   0        0        0    14637 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/httpx_request_adapter.py
--rw-r--r--   0        0        0     4823 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/kiota_client_factory.py
--rw-r--r--   0        0        0      276 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/__init__.py
--rw-r--r--   0        0        0      652 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/async_kiota_transport.py
--rw-r--r--   0        0        0     2011 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/middleware.py
--rw-r--r--   0        0        0      321 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/options/__init__.py
--rw-r--r--   0        0        0     1621 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/options/parameters_name_decoding_handler_option.py
--rw-r--r--   0        0        0     2127 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/options/redirect_handler_option.py
--rw-r--r--   0        0        0      858 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/options/response_handler_option.py
--rw-r--r--   0        0        0     3067 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/options/retry_handler_option.py
--rw-r--r--   0        0        0      714 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/options/telemetry_handler_option.py
--rw-r--r--   0        0        0     2303 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/parameters_name_decoding_handler.py
--rw-r--r--   0        0        0     8588 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/redirect_handler.py
--rw-r--r--   0        0        0     8057 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/retry_handler.py
--rw-r--r--   0        0        0     1286 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1844 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/__init__.py
--rw-r--r--   0        0        0     4882 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/conftest.py
--rw-r--r--   0        0        0      114 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/helpers/__init__.py
--rw-r--r--   0        0        0     4498 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/helpers/mock_response_object.py
--rw-r--r--   0        0        0      105 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/helpers/office_location.py
--rw-r--r--   0        0        0        0 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/middleware_tests/__init__.py
--rw-r--r--   0        0        0      989 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/middleware_tests/test_parameters_name_decoding_handler.py
--rw-r--r--   0        0        0     2207 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/middleware_tests/test_redirect_handler.py
--rw-r--r--   0        0        0     4324 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/middleware_tests/test_retry_handler.py
--rw-r--r--   0        0        0    10952 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/test_httpx_request_adapter.py
--rw-r--r--   0        0        0     3277 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/test_kiota_client_factory.py
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 microsoft_kiota_http-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      117 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1804 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.github/workflows/build_publish.yml
+-rw-r--r--   0        0        0     2538 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1799 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.gitignore
+-rw-r--r--   0        0        0    15946 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/.pylintrc
+-rw-r--r--   0        0        0     1216 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/LICENSE
+-rw-r--r--   0        0        0     2376 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/README.md
+-rw-r--r--   0        0        0     2757 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/SUPPORT.md
+-rw-r--r--   0        0        0      121 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/_version.py
+-rw-r--r--   0        0        0    14637 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/httpx_request_adapter.py
+-rw-r--r--   0        0        0     5189 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/kiota_client_factory.py
+-rw-r--r--   0        0        0      327 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/__init__.py
+-rw-r--r--   0        0        0      652 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/async_kiota_transport.py
+-rw-r--r--   0        0        0     2011 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/middleware.py
+-rw-r--r--   0        0        0      377 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/__init__.py
+-rw-r--r--   0        0        0     1621 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/parameters_name_decoding_handler_option.py
+-rw-r--r--   0        0        0     2127 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/redirect_handler_option.py
+-rw-r--r--   0        0        0      858 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/response_handler_option.py
+-rw-r--r--   0        0        0     3067 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/retry_handler_option.py
+-rw-r--r--   0        0        0      714 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/telemetry_handler_option.py
+-rw-r--r--   0        0        0     1344 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/options/url_replace_option.py
+-rw-r--r--   0        0        0     2303 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/parameters_name_decoding_handler.py
+-rw-r--r--   0        0        0     8588 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/redirect_handler.py
+-rw-r--r--   0        0        0     8057 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/retry_handler.py
+-rw-r--r--   0        0        0     2307 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/kiota_http/middleware/url_replace_handler.py
+-rw-r--r--   0        0        0     1286 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      885 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0     4882 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0      114 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     4498 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/tests/helpers/mock_response_object.py
+-rw-r--r--   0        0        0      105 2023-06-20 12:28:30.903978 microsoft_kiota_http-0.4.4/tests/helpers/office_location.py
+-rw-r--r--   0        0        0        0 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/middleware_tests/__init__.py
+-rw-r--r--   0        0        0      989 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/middleware_tests/test_parameters_name_decoding_handler.py
+-rw-r--r--   0        0        0     2207 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/middleware_tests/test_redirect_handler.py
+-rw-r--r--   0        0        0     4324 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/middleware_tests/test_retry_handler.py
+-rw-r--r--   0        0        0     1681 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/middleware_tests/test_url_replace_handler.py
+-rw-r--r--   0        0        0    10952 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/test_httpx_request_adapter.py
+-rw-r--r--   0        0        0     3355 2023-06-20 12:28:30.907978 microsoft_kiota_http-0.4.4/tests/test_kiota_client_factory.py
+-rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 microsoft_kiota_http-0.4.4/PKG-INFO
```

### Comparing `microsoft_kiota_http-0.4.3/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_http-0.4.4/.github/workflows/auto-merge-dependabot.yml`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     runs-on: ubuntu-latest
 
     if: ${{ github.actor == 'dependabot[bot]' }}
 
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.4.0
+        uses: dependabot/fetch-metadata@v1.5.1
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
 
       - name: Enable auto-merge for Dependabot PRs
         # Only if version bump is not a major version change
         if: ${{steps.metadata.outputs.update-type != 'version-update:semver-major'}}
         run: gh pr merge --auto --merge "$PR_URL"
```

### Comparing `microsoft_kiota_http-0.4.3/.github/workflows/build_publish.yml` & `microsoft_kiota_http-0.4.4/.github/workflows/build_publish.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 name: Python HTTP
 
 on:
   workflow_dispatch:
   push:
-    branches: [ main ]
+    branches: [main]
   pull_request:
-    branches: [ main, dev ]
+    branches: [main, dev]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10']
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - name: Checkout
         uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install pipenv
-          pipenv install --dev --skip-lock
+          pipenv install -r requirements-dev.txt
       - name: Check code format
         run: |
           pipenv run yapf -dr kiota_http
       - name: Check import order
         run: |
           pipenv run isort kiota_http
       - name: Lint with Pylint
@@ -58,8 +58,8 @@
         run: |
           pip install flit
       - name: Publish the distibution to PyPI
         run: flit publish
         env:
           FLIT_INDEX_URL: https://upload.pypi.org/legacy/
           FLIT_USERNAME: __token__
-          FLIT_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
+          FLIT_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `microsoft_kiota_http-0.4.3/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_http-0.4.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_http-0.4.4/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/.gitignore` & `microsoft_kiota_http-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/.pylintrc` & `microsoft_kiota_http-0.4.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/CHANGELOG.md` & `microsoft_kiota_http-0.4.4/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.4] - 2023-05-31
+
+### Added
+
+- Added a url replace handler for replacing url segments.
+
+### Changed
+
 ## [0.4.3] - 2023-05-16
 
 ### Added
 
 ### Changed
 
 - Fixes bug in getting content from redirected request.
```

### Comparing `microsoft_kiota_http-0.4.3/LICENSE` & `microsoft_kiota_http-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/README.md` & `microsoft_kiota_http-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/SECURITY.md` & `microsoft_kiota_http-0.4.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/SUPPORT.md` & `microsoft_kiota_http-0.4.4/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/kiota_http/httpx_request_adapter.py` & `microsoft_kiota_http-0.4.4/kiota_http/httpx_request_adapter.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/kiota_http/kiota_client_factory.py` & `microsoft_kiota_http-0.4.4/kiota_http/kiota_client_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 from .middleware import (
     AsyncKiotaTransport,
     BaseMiddleware,
     MiddlewarePipeline,
     ParametersNameDecodingHandler,
     RedirectHandler,
     RetryHandler,
+    UrlReplaceHandler,
 )
 from .middleware.options import (
     ParametersNameDecodingHandlerOption,
     RedirectHandlerOption,
     RetryHandlerOption,
+    UrlReplaceHandlerOption,
 )
 
 DEFAULT_CONNECTION_TIMEOUT: int = 30
 DEFAULT_REQUEST_TIMEOUT: int = 100
 
 
 class KiotaClientFactory:
@@ -90,33 +92,40 @@
         """
         Helper method that returns a list of default middleware instantiated with
         appropriate options
         """
         redirect_handler = RedirectHandler()
         retry_handler = RetryHandler()
         parameters_name_decoding_handler = ParametersNameDecodingHandler()
+        url_replace_handler = UrlReplaceHandler()
 
         if options:
-            redirect_handler_options = options.get(RedirectHandlerOption().get_key())
+            redirect_handler_options = options.get(RedirectHandlerOption.get_key())
             if redirect_handler_options:
                 redirect_handler = RedirectHandler(options=redirect_handler_options)
 
-            retry_handler_options = options.get(RetryHandlerOption().get_key())
+            retry_handler_options = options.get(RetryHandlerOption.get_key())
             if retry_handler_options:
                 retry_handler = RetryHandler(options=retry_handler_options)
 
             parameters_name_decoding_handler_options = options.get(
-                ParametersNameDecodingHandlerOption().get_key()
+                ParametersNameDecodingHandlerOption.get_key()
             )
             if parameters_name_decoding_handler_options:
                 parameters_name_decoding_handler = ParametersNameDecodingHandler(
                     options=parameters_name_decoding_handler_options
                 )
 
-        middleware = [redirect_handler, retry_handler, parameters_name_decoding_handler]
+            url_replace_handler_options = options.get(UrlReplaceHandlerOption.get_key())
+            if url_replace_handler_options:
+                url_replace_handler = UrlReplaceHandler(options=url_replace_handler_options)
+
+        middleware = [
+            redirect_handler, retry_handler, parameters_name_decoding_handler, url_replace_handler
+        ]
         return middleware
 
     @staticmethod
     def create_middleware_pipeline(
         middleware: Optional[List[BaseMiddleware]], transport: httpx.AsyncBaseTransport
     ) -> MiddlewarePipeline:
         """
```

### Comparing `microsoft_kiota_http-0.4.3/kiota_http/middleware/async_kiota_transport.py` & `microsoft_kiota_http-0.4.4/kiota_http/middleware/async_kiota_transport.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/kiota_http/middleware/middleware.py` & `microsoft_kiota_http-0.4.4/kiota_http/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/kiota_http/middleware/options/parameters_name_decoding_handler_option.py` & `microsoft_kiota_http-0.4.4/kiota_http/middleware/options/parameters_name_decoding_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/kiota_http/middleware/options/redirect_handler_option.py` & `microsoft_kiota_http-0.4.4/kiota_http/middleware/options/redirect_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/kiota_http/middleware/options/response_handler_option.py` & `microsoft_kiota_http-0.4.4/kiota_http/middleware/options/response_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/kiota_http/middleware/options/retry_handler_option.py` & `microsoft_kiota_http-0.4.4/kiota_http/middleware/options/retry_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/kiota_http/middleware/options/telemetry_handler_option.py` & `microsoft_kiota_http-0.4.4/kiota_http/middleware/options/telemetry_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/kiota_http/middleware/parameters_name_decoding_handler.py` & `microsoft_kiota_http-0.4.4/kiota_http/middleware/parameters_name_decoding_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/kiota_http/middleware/redirect_handler.py` & `microsoft_kiota_http-0.4.4/kiota_http/middleware/redirect_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/kiota_http/middleware/retry_handler.py` & `microsoft_kiota_http-0.4.4/kiota_http/middleware/retry_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/pyproject.toml` & `microsoft_kiota_http-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/tests/conftest.py` & `microsoft_kiota_http-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/tests/helpers/mock_response_object.py` & `microsoft_kiota_http-0.4.4/tests/helpers/mock_response_object.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/tests/middleware_tests/test_parameters_name_decoding_handler.py` & `microsoft_kiota_http-0.4.4/tests/middleware_tests/test_parameters_name_decoding_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/tests/middleware_tests/test_redirect_handler.py` & `microsoft_kiota_http-0.4.4/tests/middleware_tests/test_redirect_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/tests/middleware_tests/test_retry_handler.py` & `microsoft_kiota_http-0.4.4/tests/middleware_tests/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/tests/test_httpx_request_adapter.py` & `microsoft_kiota_http-0.4.4/tests/test_httpx_request_adapter.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_http-0.4.3/tests/test_kiota_client_factory.py` & `microsoft_kiota_http-0.4.4/tests/test_kiota_client_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from kiota_http.kiota_client_factory import KiotaClientFactory
 from kiota_http.middleware import (
     AsyncKiotaTransport,
     MiddlewarePipeline,
     ParametersNameDecodingHandler,
     RedirectHandler,
     RetryHandler,
+    UrlReplaceHandler
 )
 from kiota_http.middleware.options import RedirectHandlerOption, RetryHandlerOption
 
 
 def test_create_with_default_middleware():
     """Test creation of HTTP Client using default middleware"""
     client = KiotaClientFactory.create_with_default_middleware()
@@ -49,32 +50,33 @@
     assert isinstance(pipeline._first_middleware, RetryHandler)
 
 
 def test_get_default_middleware():
     """Test fetching of default middleware with no custom options passed"""
     middleware = KiotaClientFactory.get_default_middleware(None)
 
-    assert len(middleware) == 3
+    assert len(middleware) == 4
     assert isinstance(middleware[0], RedirectHandler)
     assert isinstance(middleware[1], RetryHandler)
     assert isinstance(middleware[2], ParametersNameDecodingHandler)
+    assert isinstance(middleware[3], UrlReplaceHandler)
 
 
 def test_get_default_middleware_with_options():
     """Test fetching of default middleware with custom options passed"""
     retry_options = RetryHandlerOption(max_retries=7)
     redirect_options = RedirectHandlerOption(should_redirect=False)
     options = {
         f'{retry_options.get_key()}': retry_options,
         f'{redirect_options.get_key()}': redirect_options
     }
 
     middleware = KiotaClientFactory.get_default_middleware(options=options)
 
-    assert len(middleware) == 3
+    assert len(middleware) == 4
     assert isinstance(middleware[0], RedirectHandler)
     assert middleware[0].options.should_redirect is False
     assert isinstance(middleware[1], RetryHandler)
     assert middleware[1].options.max_retry == 7
     assert isinstance(middleware[2], ParametersNameDecodingHandler)
```

### Comparing `microsoft_kiota_http-0.4.3/PKG-INFO` & `microsoft_kiota_http-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-http
-Version: 0.4.3
+Version: 0.4.4
 Summary: Kiota http request adapter implementation for httpx library
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

