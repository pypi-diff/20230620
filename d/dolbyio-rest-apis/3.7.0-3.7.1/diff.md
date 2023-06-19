# Comparing `tmp/dolbyio-rest-apis-3.7.0.tar.gz` & `tmp/dolbyio-rest-apis-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolbyio-rest-apis-3.7.0.tar", last modified: Wed Jun  7 18:07:48 2023, max compression
+gzip compressed data, was "dolbyio-rest-apis-3.7.1.tar", last modified: Mon Jun 19 22:00:50 2023, max compression
```

## Comparing `dolbyio-rest-apis-3.7.0.tar` & `dolbyio-rest-apis-3.7.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.372013 dolbyio-rest-apis-3.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.376013 dolbyio-rest-apis-3.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/ISSUE_TEMPLATE/report-an-issue.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.372013 dolbyio-rest-apis-3.7.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.380013 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/oidc-exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/print-hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.380013 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime-prerequisites.in
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime-prerequisites.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.in
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     4067 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/twine-upload.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/workflows/build-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.github/workflows/publish-package-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/client/
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.372013 dolbyio-rest-apis-3.7.0/client/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/conference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/internal/http_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/conferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/remix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.384013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/http_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/http_request_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/analyze_music.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/analyze_speech.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/enhance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/internal/http_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/mastering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/analyze_music_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/analyze_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/analyze_speech_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/diagnose_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/enhance_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/mastering_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/result_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/transcode_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/transcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/internal/http_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/publish_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/subscribe_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/publish_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/subscribe_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-07 18:07:32.000000 dolbyio-rest-apis-3.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:07:48.388013 dolbyio-rest-apis-3.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.951564 dolbyio-rest-apis-3.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.939564 dolbyio-rest-apis-3.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.943564 dolbyio-rest-apis-3.7.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/ISSUE_TEMPLATE/report-an-issue.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.939564 dolbyio-rest-apis-3.7.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.943564 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/oidc-exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/print-hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.943564 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime-prerequisites.in
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime-prerequisites.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4067 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/twine-upload.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.943564 dolbyio-rest-apis-3.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/workflows/build-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/workflows/publish-package-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-06-19 22:00:50.951564 dolbyio-rest-apis-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.939564 dolbyio-rest-apis-3.7.1/client/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/conference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/internal/http_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/conferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/remix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/http_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/http_request_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/analyze_music.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/analyze_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/diagnose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/enhance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/internal/http_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/mastering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/analyze_music_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/analyze_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/analyze_speech_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/diagnose_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/enhance_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/mastering_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/result_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/transcode_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/transcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.951564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.951564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/internal/http_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.951564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/publish_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/subscribe_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/publish_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/subscribe_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 22:00:50.951564 dolbyio-rest-apis-3.7.1/setup.cfg
```

### Comparing `dolbyio-rest-apis-3.7.0/.github/ISSUE_TEMPLATE/report-an-issue.md` & `dolbyio-rest-apis-3.7.1/.github/ISSUE_TEMPLATE/report-an-issue.md`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/.gitignore` & `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/.pre-commit-config.yaml` & `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/Dockerfile` & `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/LICENSE.md` & `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/README.md` & `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/action.yml` & `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/action.yml`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/oidc-exchange.py` & `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/oidc-exchange.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/print-hash.py` & `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/print-hash.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.in` & `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.in`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.txt` & `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.txt`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/actions/gh-action-pypi-publish-1.8.6/twine-upload.sh` & `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/twine-upload.sh`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/workflows/build-package.yml` & `dolbyio-rest-apis-3.7.1/.github/workflows/build-package.yml`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/workflows/codeql-analysis.yml` & `dolbyio-rest-apis-3.7.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.github/workflows/publish-package-to-pypi.yml` & `dolbyio-rest-apis-3.7.1/.github/workflows/publish-package-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.gitignore` & `dolbyio-rest-apis-3.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/.pylintrc` & `dolbyio-rest-apis-3.7.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/LICENSE` & `dolbyio-rest-apis-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/PKG-INFO` & `dolbyio-rest-apis-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolbyio-rest-apis
-Version: 3.7.0
+Version: 3.7.1
 Summary: A Python wrapper for the Dolby.io REST APIs.
 Home-page: https://github.com/dolbyio/dolbyio-rest-apis-client-python
 Author: Dolby.io
 Author-email: fabien.lavocat@dolby.com
 License: MIT
 Project-URL: Documentation, https://docs.dolby.io/communications-apis/reference
 Project-URL: Source, https://github.com/dolbyio/dolbyio-rest-apis-client-python
```

### Comparing `dolbyio-rest-apis-3.7.0/README.md` & `dolbyio-rest-apis-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/README.md` & `dolbyio-rest-apis-3.7.1/client/README.md`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/setup.py` & `dolbyio-rest-apis-3.7.1/client/setup.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/authentication.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/authentication.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/authentication.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/authentication.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/conference.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/conference.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This module contains the functions to work with the conference API.
 """
 
 from dataclasses import asdict
 from dolbyio_rest_apis.communications.internal.http_context import CommunicationsHttpContext
 from dolbyio_rest_apis.core.helpers import get_value, add_if_not_none
 from dolbyio_rest_apis.core.urls import get_comms_url_v2
-from .models import UserToken, Conference, SpatialAudioEnvironment, SpatialAudioListener, SpatialAudioUser, RTCPMode, Participant, VideoCodec
+from .models import UserToken, Conference, SpatialAudioEnvironment, SpatialAudioListener, SpatialAudioUser, RTCPMode, Participant, VideoCodec, GetParticipantsResponse
 from typing import List
 
 async def create_conference(
         access_token: str,
         owner_external_id: str,
         alias: str=None,
         pincode: str=None,
@@ -332,14 +332,40 @@
     user_tokens = []
     for key in json_response.keys():
         user_token = UserToken(key, json_response[key])
         user_tokens.append(user_token)
 
     return user_tokens
 
+async def list_participants(
+        access_token: str,
+        conference_id: str,
+    ) -> GetParticipantsResponse:
+    r"""
+    Returns the current participant list.
+
+    See: https://docs.dolby.io/communications-apis/reference/return-participant-list
+
+    Args:
+        access_token: Access token to use for authentication.
+        conference_id: Identifier of the conference.
+
+    Raises:
+        HttpRequestError: If a client error one occurred.
+        HTTPError: If one occurred.
+    """
+
+    async with CommunicationsHttpContext() as http_context:
+        json_response = await http_context.requests_get(
+            access_token=access_token,
+            url=f'{get_comms_url_v2()}/conferences/{conference_id}/participants',
+        )
+
+    return GetParticipantsResponse(json_response)
+
 async def terminate(
         access_token: str,
         conference_id: str,
     ) -> None:
     r"""
     Terminates an ongoing conference and removes all remaining participants from the conference.
```

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/internal/http_context.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/internal/http_context.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/models.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -95,14 +95,40 @@
 
         self.user_tokens: List[UserToken] = []
         if in_and_not_none(self, 'usersTokens'):
             for key in self['usersTokens'].keys():
                 user_token = UserToken(key, self['usersTokens'][key])
                 self.user_tokens.append(user_token)
 
+class ConferenceParticipant(dict):
+    """Representation of a participant."""
+
+    def __init__(self, dictionary: dict):
+        dict.__init__(self, dictionary)
+
+        self.user_id = get_value_or_default(self, 'userId', None)
+        self.external_id = get_value_or_default(self, 'externalId', None)
+        self.name = get_value_or_default(self, 'name', None)
+        self.avatar_url = get_value_or_default(self, 'avatarUrl', None)
+        self.ip_address = get_value_or_default(self, 'ipAddress', None)
+        self.user_agent = get_value_or_default(self, 'userAgent', None)
+        self.last_join_timestamp = get_value_or_default(self, 'lastJoinTimestamp', 0)
+        self.nb_session = get_value_or_default(self, 'nbSession', 0)
+
+class GetParticipantsResponse(dict):
+    """Representation of a Participants response."""
+
+    def __init__(self, dictionary: dict):
+        dict.__init__(self, dictionary)
+
+        self.participants: List[ConferenceParticipant] = []
+        if in_and_not_none(self, 'participants'):
+            for participant in self['participants']:
+                self.participants.append(ConferenceParticipant(participant))
+
 class RemixStatus(dict):
     """Representation of a Remix Status."""
 
     def __init__(self, dictionary: dict):
         dict.__init__(self, dictionary)
 
         self.status = get_value_or_default(self, 'status', None)
```

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/conferences.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/conferences.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/models.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/models.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/recordings.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/recordings.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/monitor/webhooks.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/webhooks.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/recording.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/recording.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/remix.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/remix.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/communications/streaming.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/streaming.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/helpers.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/helpers.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/http_context.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/http_context.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/http_request_error.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/http_request_error.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/rate_limiter.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/core/urls.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/urls.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/analyze.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/analyze.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/analyze_music.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/analyze_music.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/analyze_speech.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/analyze_speech.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/diagnose.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/diagnose.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/enhance.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/enhance.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/internal/http_context.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/internal/http_context.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/io.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/io.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/jobs.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/jobs.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/mastering.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/mastering.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/analyze_music_response.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/analyze_music_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/analyze_response.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/analyze_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/analyze_speech_response.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/analyze_speech_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/diagnose_response.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/diagnose_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/enhance_response.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/enhance_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/job_response.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/job_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/jobs_response.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/jobs_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/mastering_response.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/mastering_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/result_error.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/result_error.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/transcode_response.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/transcode_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/models/webhook.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/webhook.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/transcode.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/transcode.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/media/webhooks.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/webhooks.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/models.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/models.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/cluster.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/cluster.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/internal/http_context.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/internal/http_context.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/cluster.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/cluster.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/core.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/core.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/publish_token.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/publish_token.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/models/subscribe_token.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/subscribe_token.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/publish_token.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/publish_token.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/stream.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/stream.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.0/client/src/dolbyio_rest_apis/streaming/subscribe_token.py` & `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/subscribe_token.py`

 * *Files identical despite different names*

