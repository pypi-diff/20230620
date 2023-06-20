# Comparing `tmp/junifer-0.0.3.dev73.tar.gz` & `tmp/junifer-0.0.3.dev74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junifer-0.0.3.dev73.tar", last modified: Tue Jun 20 10:29:26 2023, max compression
+gzip compressed data, was "junifer-0.0.3.dev74.tar", last modified: Tue Jun 20 10:29:32 2023, max compression
```

## Comparing `junifer-0.0.3.dev73.tar` & `junifer-0.0.3.dev74.tar`

### file list

```diff
@@ -1,373 +1,374 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.934368 junifer-0.0.3.dev73/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.902368 junifer-0.0.3.dev73/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.902368 junifer-0.0.3.dev73/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/ISSUE_TEMPLATE/dataset-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/ISSUE_TEMPLATE/documention-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/ISSUE_TEMPLATE/marker-request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.902368 junifer-0.0.3.dev73/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34353 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-20 10:29:26.934368 junifer-0.0.3.dev73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/conda-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.906368 junifer-0.0.3.dev73/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.894368 junifer-0.0.3.dev73/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.906368 junifer-0.0.3.dev73/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.906368 junifer-0.0.3.dev73/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.906368 junifer-0.0.3.dev73/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.906368 junifer-0.0.3.dev73/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/configs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/datagrabbers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/datareaders.rst
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/markers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/nilearn.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/builtin.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.906368 junifer-0.0.3.dev73/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.906368 junifer-0.0.3.dev73/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/changes/newsfragments/220.doc
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/changes/newsfragments/222.change
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/changes/newsfragments/222.enh
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/changes/newsfragments/223.bugfix
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/changes/newsfragments/223.enh
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/changes/newsfragments/226.enh
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/changes/newsfragments/230.misc
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.906368 junifer-0.0.3.dev73/docs/extending/
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/extending/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/extending/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/extending/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/extending/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/extending/marker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/extending/masks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/extending/parcellations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/help.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.906368 junifer-0.0.3.dev73/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    62148 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/images/junifer_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.906368 junifer-0.0.3.dev73/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/sphinxext/gh_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/starting.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.910368 junifer-0.0.3.dev73/docs/understanding/
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/understanding/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/understanding/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/understanding/datareader.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/understanding/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/understanding/marker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/understanding/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/understanding/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/understanding/storage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.910368 junifer-0.0.3.dev73/docs/using/
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/using/codeless.rst
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/using/masks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/using/queueing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/using/running.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.910368 junifer-0.0.3.dev73/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/examples/norun_hcpfc_pearson.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/examples/norun_ukbvm_gmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/examples/run_compute_parcel_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/examples/run_datagrabber_bids_datalad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/examples/run_ets_rss_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/examples/run_junifer_julearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/examples/run_run_gmd_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.910368 junifer-0.0.3.dev73/examples/yamls/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/examples/yamls/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/examples/yamls/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/examples/yamls/ukb_gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.910368 junifer-0.0.3.dev73/junifer/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 10:29:26.000000 junifer-0.0.3.dev73/junifer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.914368 junifer-0.0.3.dev73/junifer/api/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    22518 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.914368 junifer-0.0.3.dev73/junifer/api/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.914368 junifer-0.0.3.dev73/junifer/api/res/afni/
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/res/afni/3dAFNItoNIFTI
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/res/afni/3dRSFC
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/res/afni/3dReHo
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/res/afni/afni
--rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/res/afni/run_afni_docker.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/res/run_conda.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.914368 junifer-0.0.3.dev73/junifer/api/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.914368 junifer-0.0.3.dev73/junifer/api/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/tests/data/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/tests/data/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/tests/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    24484 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.914368 junifer-0.0.3.dev73/junifer/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.914368 junifer-0.0.3.dev73/junifer/configs/juseless/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/juseless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.914368 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/ixi_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.914368 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/ucla.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/ukb_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.914368 junifer-0.0.3.dev73/junifer/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.898368 junifer-0.0.3.dev73/junifer/data/VOIs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.918367 junifer-0.0.3.dev73/junifer/data/VOIs/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/CogAC_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/CogAR_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/Empathy_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/Motor_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/MultiTask_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/Rew_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/ToM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/VigAtt_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/WM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/eMDN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/eSAD_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/VOIs/meta/extDMN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.898368 junifer-0.0.3.dev73/junifer/data/masks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.918367 junifer-0.0.3.dev73/junifer/data/masks/vickery-patil/
--rw-r--r--   0 runner    (1001) docker     (123)    88270 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    27401 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/parcellations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.918367 junifer-0.0.3.dev73/junifer/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/tests/test_parcellations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.918367 junifer-0.0.3.dev73/junifer/datagrabber/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.918367 junifer-0.0.3.dev73/junifer/datagrabber/aomic/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/aomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/aomic/id1000.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/aomic/piop1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/aomic/piop2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.918367 junifer-0.0.3.dev73/junifer/datagrabber/aomic/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/aomic/tests/test_id1000.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/aomic/tests/test_piop1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/aomic/tests/test_piop2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/datalad_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.922367 junifer-0.0.3.dev73/junifer/datagrabber/hcp1200/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/hcp1200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/hcp1200/datalad_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/hcp1200/hcp1200.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.922367 junifer-0.0.3.dev73/junifer/datagrabber/hcp1200/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/pattern_datalad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.922367 junifer-0.0.3.dev73/junifer/datagrabber/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/tests/test_datagrabber_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/tests/test_datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/tests/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/tests/test_pattern_datalad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datagrabber/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.922367 junifer-0.0.3.dev73/junifer/datareader/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datareader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datareader/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.922367 junifer-0.0.3.dev73/junifer/datareader/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/datareader/tests/test_default_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.922367 junifer-0.0.3.dev73/junifer/external/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.898368 junifer-0.0.3.dev73/junifer/external/h5io/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.922367 junifer-0.0.3.dev73/junifer/external/h5io/h5io/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 10:29:17.000000 junifer-0.0.3.dev73/junifer/external/h5io/h5io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28748 2023-06-20 10:29:17.000000 junifer-0.0.3.dev73/junifer/external/h5io/h5io/_h5io.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 10:29:17.000000 junifer-0.0.3.dev73/junifer/external/h5io/h5io/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-20 10:29:17.000000 junifer-0.0.3.dev73/junifer/external/h5io/h5io/chunked_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-20 10:29:17.000000 junifer-0.0.3.dev73/junifer/external/h5io/h5io/chunked_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.922367 junifer-0.0.3.dev73/junifer/external/nilearn/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/external/nilearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/external/nilearn/junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.922367 junifer-0.0.3.dev73/junifer/external/nilearn/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.922367 junifer-0.0.3.dev73/junifer/markers/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/ets_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.922367 junifer-0.0.3.dev73/junifer/markers/falff/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/falff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/falff/falff_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/falff/falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/falff/falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/falff/falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.922367 junifer-0.0.3.dev73/junifer/markers/falff/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/falff/tests/test_falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/falff/tests/test_falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/falff/tests/test_falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.926367 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.926367 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/parcel_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.926367 junifer-0.0.3.dev73/junifer/markers/reho/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/reho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/reho/reho_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/reho/reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/reho/reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/reho/reho_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.926367 junifer-0.0.3.dev73/junifer/markers/reho/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/reho/tests/test_reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/reho/tests/test_reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/reho/tests/test_reho_spheres.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/sphere_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.926367 junifer-0.0.3.dev73/junifer/markers/temporal_snr/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/temporal_snr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/temporal_snr/temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/temporal_snr/temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/temporal_snr/temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.926367 junifer-0.0.3.dev73/junifer/markers/temporal_snr/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.926367 junifer-0.0.3.dev73/junifer/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/tests/test_ets_rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/tests/test_marker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/tests/test_markers_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/tests/test_parcel_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/tests/test_sphere_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/markers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.930368 junifer-0.0.3.dev73/junifer/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/pipeline/pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/pipeline/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.930368 junifer-0.0.3.dev73/junifer/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/pipeline/tests/test_pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/pipeline/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/pipeline/tests/test_update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/pipeline/update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.930368 junifer-0.0.3.dev73/junifer/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/preprocess/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.930368 junifer-0.0.3.dev73/junifer/preprocess/confounds/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/preprocess/confounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21846 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/preprocess/confounds/fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.930368 junifer-0.0.3.dev73/junifer/preprocess/confounds/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21614 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.930368 junifer-0.0.3.dev73/junifer/preprocess/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/preprocess/tests/test_preprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.930368 junifer-0.0.3.dev73/junifer/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/storage/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/storage/pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20231 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/storage/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.930368 junifer-0.0.3.dev73/junifer/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/storage/tests/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/storage/tests/test_pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    27919 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/storage/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/storage/tests/test_storage_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/storage/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.930368 junifer-0.0.3.dev73/junifer/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.930368 junifer-0.0.3.dev73/junifer/testing/data/
--rw-r--r--   0 runner    (1001) docker     (123)   406849 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/testing/datagrabbers.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/testing/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.934368 junifer-0.0.3.dev73/junifer/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/testing/tests/test_spmauditory_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/testing/tests/test_testing_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.934368 junifer-0.0.3.dev73/junifer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.934368 junifer-0.0.3.dev73/junifer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.934368 junifer-0.0.3.dev73/junifer/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/utils/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/junifer/utils/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.910368 junifer-0.0.3.dev73/junifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-20 10:29:26.000000 junifer-0.0.3.dev73/junifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-06-20 10:29:26.000000 junifer-0.0.3.dev73/junifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:29:26.000000 junifer-0.0.3.dev73/junifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 10:29:26.000000 junifer-0.0.3.dev73/junifer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 10:29:26.000000 junifer-0.0.3.dev73/junifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 10:29:26.000000 junifer-0.0.3.dev73/junifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:29:26.934368 junifer-0.0.3.dev73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:26.934368 junifer-0.0.3.dev73/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/tools/create_aomic1000_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/tools/create_aomicpiop1_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/tools/create_aomicpiop2_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/tools/create_bids_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/tools/create_bids_example_dataset_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/tools/create_hcp1200_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-20 10:29:16.000000 junifer-0.0.3.dev73/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.338103 junifer-0.0.3.dev74/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.298102 junifer-0.0.3.dev74/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.298102 junifer-0.0.3.dev74/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/ISSUE_TEMPLATE/dataset-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/ISSUE_TEMPLATE/documention-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/ISSUE_TEMPLATE/marker-request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.302102 junifer-0.0.3.dev74/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34353 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-20 10:29:32.338103 junifer-0.0.3.dev74/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.302102 junifer-0.0.3.dev74/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.290102 junifer-0.0.3.dev74/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.302102 junifer-0.0.3.dev74/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.302102 junifer-0.0.3.dev74/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.302102 junifer-0.0.3.dev74/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.302102 junifer-0.0.3.dev74/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/datagrabbers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/datareaders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/nilearn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/builtin.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.302102 junifer-0.0.3.dev74/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.306102 junifer-0.0.3.dev74/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/changes/newsfragments/220.doc
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/changes/newsfragments/222.change
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/changes/newsfragments/222.enh
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/changes/newsfragments/223.bugfix
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/changes/newsfragments/223.enh
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/changes/newsfragments/226.enh
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/changes/newsfragments/227.enh
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/changes/newsfragments/230.misc
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.306102 junifer-0.0.3.dev74/docs/extending/
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/extending/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/extending/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/extending/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/extending/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/extending/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/extending/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/extending/parcellations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/help.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.306102 junifer-0.0.3.dev74/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    62148 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/images/junifer_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.306102 junifer-0.0.3.dev74/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/sphinxext/gh_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/starting.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.306102 junifer-0.0.3.dev74/docs/understanding/
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/understanding/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/understanding/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/understanding/datareader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/understanding/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/understanding/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/understanding/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/understanding/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/understanding/storage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.310102 junifer-0.0.3.dev74/docs/using/
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/using/codeless.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/using/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/using/queueing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/using/running.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.310102 junifer-0.0.3.dev74/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/examples/norun_hcpfc_pearson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/examples/norun_ukbvm_gmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/examples/run_compute_parcel_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/examples/run_datagrabber_bids_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/examples/run_ets_rss_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/examples/run_junifer_julearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/examples/run_run_gmd_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.310102 junifer-0.0.3.dev74/examples/yamls/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/examples/yamls/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/examples/yamls/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/examples/yamls/ukb_gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.310102 junifer-0.0.3.dev74/junifer/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 10:29:32.000000 junifer-0.0.3.dev74/junifer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.310102 junifer-0.0.3.dev74/junifer/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22518 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.310102 junifer-0.0.3.dev74/junifer/api/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.314102 junifer-0.0.3.dev74/junifer/api/res/afni/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/res/afni/3dAFNItoNIFTI
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/res/afni/3dRSFC
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/res/afni/3dReHo
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/res/afni/afni
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/res/afni/run_afni_docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/res/run_conda.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.314102 junifer-0.0.3.dev74/junifer/api/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.314102 junifer-0.0.3.dev74/junifer/api/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/tests/data/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/tests/data/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/tests/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24484 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.314102 junifer-0.0.3.dev74/junifer/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.314102 junifer-0.0.3.dev74/junifer/configs/juseless/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/juseless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.314102 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/ixi_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.314102 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/ucla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/ukb_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.314102 junifer-0.0.3.dev74/junifer/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.294102 junifer-0.0.3.dev74/junifer/data/VOIs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.318102 junifer-0.0.3.dev74/junifer/data/VOIs/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/CogAC_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/CogAR_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/Empathy_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/Motor_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/MultiTask_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/Rew_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/ToM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/VigAtt_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/WM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/eMDN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/eSAD_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/VOIs/meta/extDMN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.294102 junifer-0.0.3.dev74/junifer/data/masks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.318102 junifer-0.0.3.dev74/junifer/data/masks/vickery-patil/
+-rw-r--r--   0 runner    (1001) docker     (123)    88270 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27401 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/parcellations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.318102 junifer-0.0.3.dev74/junifer/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/tests/test_parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.322102 junifer-0.0.3.dev74/junifer/datagrabber/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.322102 junifer-0.0.3.dev74/junifer/datagrabber/aomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/aomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/aomic/id1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/aomic/piop1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/aomic/piop2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.322102 junifer-0.0.3.dev74/junifer/datagrabber/aomic/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/aomic/tests/test_id1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/aomic/tests/test_piop1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/aomic/tests/test_piop2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/datalad_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.322102 junifer-0.0.3.dev74/junifer/datagrabber/hcp1200/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/hcp1200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/hcp1200/datalad_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/hcp1200/hcp1200.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.322102 junifer-0.0.3.dev74/junifer/datagrabber/hcp1200/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/pattern_datalad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.322102 junifer-0.0.3.dev74/junifer/datagrabber/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/tests/test_datagrabber_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/tests/test_datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/tests/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/tests/test_pattern_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datagrabber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.322102 junifer-0.0.3.dev74/junifer/datareader/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datareader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datareader/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.322102 junifer-0.0.3.dev74/junifer/datareader/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/datareader/tests/test_default_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.322102 junifer-0.0.3.dev74/junifer/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.294102 junifer-0.0.3.dev74/junifer/external/h5io/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.322102 junifer-0.0.3.dev74/junifer/external/h5io/h5io/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 10:29:23.000000 junifer-0.0.3.dev74/junifer/external/h5io/h5io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28748 2023-06-20 10:29:23.000000 junifer-0.0.3.dev74/junifer/external/h5io/h5io/_h5io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 10:29:23.000000 junifer-0.0.3.dev74/junifer/external/h5io/h5io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-20 10:29:23.000000 junifer-0.0.3.dev74/junifer/external/h5io/h5io/chunked_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-20 10:29:23.000000 junifer-0.0.3.dev74/junifer/external/h5io/h5io/chunked_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.326103 junifer-0.0.3.dev74/junifer/external/nilearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/external/nilearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/external/nilearn/junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.326103 junifer-0.0.3.dev74/junifer/external/nilearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.326103 junifer-0.0.3.dev74/junifer/markers/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/ets_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.326103 junifer-0.0.3.dev74/junifer/markers/falff/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/falff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/falff/falff_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/falff/falff_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/falff/falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/falff/falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.326103 junifer-0.0.3.dev74/junifer/markers/falff/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/falff/tests/test_falff_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/falff/tests/test_falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/falff/tests/test_falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.326103 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.326103 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/parcel_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.330103 junifer-0.0.3.dev74/junifer/markers/reho/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/reho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/reho/reho_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/reho/reho_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/reho/reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/reho/reho_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.330103 junifer-0.0.3.dev74/junifer/markers/reho/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/reho/tests/test_reho_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/reho/tests/test_reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/reho/tests/test_reho_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/sphere_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.330103 junifer-0.0.3.dev74/junifer/markers/temporal_snr/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/temporal_snr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/temporal_snr/temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/temporal_snr/temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/temporal_snr/temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.330103 junifer-0.0.3.dev74/junifer/markers/temporal_snr/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.330103 junifer-0.0.3.dev74/junifer/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/tests/test_ets_rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/tests/test_marker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/tests/test_markers_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/tests/test_parcel_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/tests/test_sphere_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/markers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.330103 junifer-0.0.3.dev74/junifer/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/pipeline/pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/pipeline/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.330103 junifer-0.0.3.dev74/junifer/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/pipeline/tests/test_pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/pipeline/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/pipeline/tests/test_update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/pipeline/update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.334102 junifer-0.0.3.dev74/junifer/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/preprocess/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.334102 junifer-0.0.3.dev74/junifer/preprocess/confounds/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/preprocess/confounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21846 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/preprocess/confounds/fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.334102 junifer-0.0.3.dev74/junifer/preprocess/confounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21614 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.334102 junifer-0.0.3.dev74/junifer/preprocess/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/preprocess/tests/test_preprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.334102 junifer-0.0.3.dev74/junifer/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/storage/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/storage/pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20231 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/storage/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.334102 junifer-0.0.3.dev74/junifer/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28370 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/storage/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/storage/tests/test_pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27919 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/storage/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/storage/tests/test_storage_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/storage/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.334102 junifer-0.0.3.dev74/junifer/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.334102 junifer-0.0.3.dev74/junifer/testing/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   406849 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/testing/datagrabbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/testing/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.338103 junifer-0.0.3.dev74/junifer/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/testing/tests/test_spmauditory_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/testing/tests/test_testing_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.338103 junifer-0.0.3.dev74/junifer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.338103 junifer-0.0.3.dev74/junifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.338103 junifer-0.0.3.dev74/junifer/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/utils/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/junifer/utils/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.310102 junifer-0.0.3.dev74/junifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-20 10:29:32.000000 junifer-0.0.3.dev74/junifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-20 10:29:32.000000 junifer-0.0.3.dev74/junifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:29:32.000000 junifer-0.0.3.dev74/junifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 10:29:32.000000 junifer-0.0.3.dev74/junifer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 10:29:32.000000 junifer-0.0.3.dev74/junifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 10:29:32.000000 junifer-0.0.3.dev74/junifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:29:32.338103 junifer-0.0.3.dev74/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:29:32.338103 junifer-0.0.3.dev74/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/tools/create_aomic1000_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/tools/create_aomicpiop1_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/tools/create_aomicpiop2_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/tools/create_bids_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/tools/create_bids_example_dataset_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/tools/create_hcp1200_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-20 10:29:22.000000 junifer-0.0.3.dev74/tox.ini
```

### Comparing `junifer-0.0.3.dev73/.github/ISSUE_TEMPLATE/bug-report.yml` & `junifer-0.0.3.dev74/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/.github/ISSUE_TEMPLATE/dataset-request.yml` & `junifer-0.0.3.dev74/.github/ISSUE_TEMPLATE/dataset-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/.github/ISSUE_TEMPLATE/documention-request.yml` & `junifer-0.0.3.dev74/.github/ISSUE_TEMPLATE/documention-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/.github/ISSUE_TEMPLATE/feature-request.yml` & `junifer-0.0.3.dev74/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/.github/ISSUE_TEMPLATE/marker-request.yml` & `junifer-0.0.3.dev74/.github/ISSUE_TEMPLATE/marker-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/.github/workflows/ci-docs.yml` & `junifer-0.0.3.dev74/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/.github/workflows/ci.yml` & `junifer-0.0.3.dev74/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/.github/workflows/docs-preview.yml` & `junifer-0.0.3.dev74/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/.github/workflows/docs.yml` & `junifer-0.0.3.dev74/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/.github/workflows/lint.yml` & `junifer-0.0.3.dev74/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/.github/workflows/pypi.yml` & `junifer-0.0.3.dev74/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/.gitignore` & `junifer-0.0.3.dev74/.gitignore`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/LICENSE.md` & `junifer-0.0.3.dev74/LICENSE.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/PKG-INFO` & `junifer-0.0.3.dev74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.3.dev73
+Version: 0.0.3.dev74
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/junifer
 Project-URL: documentation, https://juaml.github.io/junifer
 Project-URL: repository, https://github.com/juaml/junifer
```

### Comparing `junifer-0.0.3.dev73/README.md` & `junifer-0.0.3.dev74/README.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/codecov.yml` & `junifer-0.0.3.dev74/codecov.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/conda-env.yml` & `junifer-0.0.3.dev74/conda-env.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/Makefile` & `junifer-0.0.3.dev74/docs/Makefile`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/_static/css/custom.css` & `junifer-0.0.3.dev74/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/_templates/versions.html` & `junifer-0.0.3.dev74/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/builtin.rst` & `junifer-0.0.3.dev74/docs/builtin.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/changes/contributors.inc` & `junifer-0.0.3.dev74/docs/changes/contributors.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/conf.py` & `junifer-0.0.3.dev74/docs/conf.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/contribution.rst` & `junifer-0.0.3.dev74/docs/contribution.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/extending/coordinates.rst` & `junifer-0.0.3.dev74/docs/extending/coordinates.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/extending/datagrabber.rst` & `junifer-0.0.3.dev74/docs/extending/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/extending/extension.rst` & `junifer-0.0.3.dev74/docs/extending/extension.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/extending/index.rst` & `junifer-0.0.3.dev74/docs/extending/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/extending/marker.rst` & `junifer-0.0.3.dev74/docs/extending/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/extending/masks.rst` & `junifer-0.0.3.dev74/docs/extending/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/extending/parcellations.rst` & `junifer-0.0.3.dev74/docs/extending/parcellations.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/faq.rst` & `junifer-0.0.3.dev74/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/help.rst` & `junifer-0.0.3.dev74/docs/help.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/images/junifer_logo.png` & `junifer-0.0.3.dev74/docs/images/junifer_logo.png`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/index.rst` & `junifer-0.0.3.dev74/docs/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/installation.rst` & `junifer-0.0.3.dev74/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/links.inc` & `junifer-0.0.3.dev74/docs/links.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/maintaining.rst` & `junifer-0.0.3.dev74/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/sphinxext/gh_substitutions.py` & `junifer-0.0.3.dev74/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/starting.rst` & `junifer-0.0.3.dev74/docs/starting.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/understanding/data.rst` & `junifer-0.0.3.dev74/docs/understanding/data.rst`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                                      'types': ['BOLD', 'T1w']},
                      'dependencies': set(),
                      'element': {'subject': 'sub001'}},
             'path': PosixPath('/var/folders/dv/2lbr8f8j0q12zrx3mz3ll5m40000gp/T/tmpgxcyjfo1/sub001_T1w.nii.gz')}}
 
 The :ref:`Data Reader <datareader>` step adds the ``data`` second-level key
 which is the actual data loaded into memory. The ``meta`` key in this step
-adds information about the datareader used to read the data.
+adds information about the DataReader used to read the data.
 
 .. code-block:: python
 
    {'BOLD': {'data': <nibabel.nifti1.Nifti1Image object at 0x16b5d8910>,
              'meta': {'datagrabber': {'class': 'SPMAuditoryTestingDataGrabber',
                                       'types': ['BOLD', 'T1w']},
                       'datareader': {'class': 'DefaultDataReader'},
```

### Comparing `junifer-0.0.3.dev73/docs/understanding/datagrabber.rst` & `junifer-0.0.3.dev74/docs/understanding/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/understanding/datareader.rst` & `junifer-0.0.3.dev74/docs/understanding/datareader.rst`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 The ``DataReader`` is an object that is responsible for actually reading data
 files in junifer. It reads the value of the key ``path`` for each
 :ref:`data type <data_types>` in the :ref:`Data object <data_object>` and loads
 them into memory. After reading the data into memory, it adds the key ``data``
 to the same level as ``path`` and the value is the actual data in the memory.
 
-Datareaders are meant to be used inside the datagrabber context but you can
+DataReaders are meant to be used inside the datagrabber context but you can
 operate on them outside the context as long as the actual data is in the memory
 and the Python runtime has not garbage-collected it.
 
 For data formats not supported by junifer yet, you can either make your own
 *Data Reader* or open an issue on `junifer Github`_ and we can help you out.
 
 File Formats
```

### Comparing `junifer-0.0.3.dev73/docs/understanding/index.rst` & `junifer-0.0.3.dev74/docs/understanding/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/understanding/marker.rst` & `junifer-0.0.3.dev74/docs/understanding/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/understanding/pipeline.rst` & `junifer-0.0.3.dev74/docs/understanding/pipeline.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/understanding/preprocess.rst` & `junifer-0.0.3.dev74/docs/understanding/preprocess.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/understanding/storage.rst` & `junifer-0.0.3.dev74/docs/understanding/storage.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/using/codeless.rst` & `junifer-0.0.3.dev74/docs/using/codeless.rst`

 * *Files 1% similar despite different names*

```diff
@@ -104,20 +104,20 @@
     kind: OasisVBMTestingDataGrabber
 
 
 Data Reader
 ^^^^^^^^^^^
 
 As mentioned before, this section is entirely optional, as junifer only provides
-one data reader (:class:`.DefaultDataReader`), which is the default in case the
+one DataReader (:class:`.DefaultDataReader`), which is the default in case the
 section is not specified.
 
 In any case, the syntax of the section is the same as for the ``datagrabber``
-section, using the ``kind`` key to specify the datareader to use, and additional
-keys to pass parameters to the datareader:
+section, using the ``kind`` key to specify the DataReader to use, and additional
+keys to pass parameters to the DataReader constructor:
 
 .. code-block:: yaml
 
     datareader:
       kind: DefaultDataReader
```

### Comparing `junifer-0.0.3.dev73/docs/using/index.rst` & `junifer-0.0.3.dev74/docs/using/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/using/masks.rst` & `junifer-0.0.3.dev74/docs/using/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/using/queueing.rst` & `junifer-0.0.3.dev74/docs/using/queueing.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/using/running.rst` & `junifer-0.0.3.dev74/docs/using/running.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/docs/whats_new.rst` & `junifer-0.0.3.dev74/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/examples/norun_hcpfc_pearson.py` & `junifer-0.0.3.dev74/examples/norun_hcpfc_pearson.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/examples/norun_ukbvm_gmd.py` & `junifer-0.0.3.dev74/examples/norun_ukbvm_gmd.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/examples/run_compute_parcel_mean.py` & `junifer-0.0.3.dev74/examples/run_compute_parcel_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/examples/run_datagrabber_bids_datalad.py` & `junifer-0.0.3.dev74/examples/run_datagrabber_bids_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/examples/run_ets_rss_marker.py` & `junifer-0.0.3.dev74/examples/run_ets_rss_marker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/examples/run_junifer_julearn.py` & `junifer-0.0.3.dev74/examples/run_junifer_julearn.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/examples/run_run_gmd_mean.py` & `junifer-0.0.3.dev74/examples/run_run_gmd_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/examples/yamls/gmd_mean.yaml` & `junifer-0.0.3.dev74/examples/yamls/gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/examples/yamls/ukb_gmd_mean.yaml` & `junifer-0.0.3.dev74/examples/yamls/ukb_gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/api/cli.py` & `junifer-0.0.3.dev74/junifer/api/cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/api/decorators.py` & `junifer-0.0.3.dev74/junifer/api/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,28 +35,32 @@
         name=klass.__name__,
         klass=klass,
     )
     return klass
 
 
 def register_datareader(klass: Type) -> Type:
-    """Datareader registration decorator.
+    """Register DataReader.
 
-    Registers the datareader so it can be used by name.
+    Registers the DataReader so it can be used by name.
 
     Parameters
     ----------
     klass: class
-        The class of the datareader to register.
+        The class of the DataReader to register.
 
     Returns
     -------
     klass: class
         The unmodified input class.
 
+    Notes
+    -----
+    It should only be used as a decorator.
+
     """
     register(
         step="datareader",
         name=klass.__name__,
         klass=klass,
     )
     return klass
```

### Comparing `junifer-0.0.3.dev73/junifer/api/functions.py` & `junifer-0.0.3.dev74/junifer/api/functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/api/parser.py` & `junifer-0.0.3.dev74/junifer/api/parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/api/res/afni/run_afni_docker.sh` & `junifer-0.0.3.dev74/junifer/api/res/afni/run_afni_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/api/tests/test_api_utils.py` & `junifer-0.0.3.dev74/junifer/api/tests/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/api/tests/test_cli.py` & `junifer-0.0.3.dev74/junifer/api/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/api/tests/test_functions.py` & `junifer-0.0.3.dev74/junifer/api/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/api/tests/test_parser.py` & `junifer-0.0.3.dev74/junifer/api/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/api/utils.py` & `junifer-0.0.3.dev74/junifer/api/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py` & `junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/camcan_vbm.py` & `junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/ixi_vbm.py` & `junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py` & `junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py` & `junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py` & `junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/tests/test_ucla.py` & `junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/tests/test_ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py` & `junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/ucla.py` & `junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/configs/juseless/datagrabbers/ukb_vbm.py` & `junifer-0.0.3.dev74/junifer/configs/juseless/datagrabbers/ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt` & `junifer-0.0.3.dev74/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt` & `junifer-0.0.3.dev74/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/VOIs/meta/Rew_VOIs.txt` & `junifer-0.0.3.dev74/junifer/data/VOIs/meta/Rew_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/VOIs/meta/WM_VOIs.txt` & `junifer-0.0.3.dev74/junifer/data/VOIs/meta/WM_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/coordinates.py` & `junifer-0.0.3.dev74/junifer/data/coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz` & `junifer-0.0.3.dev74/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz` & `junifer-0.0.3.dev74/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz` & `junifer-0.0.3.dev74/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/masks.py` & `junifer-0.0.3.dev74/junifer/data/masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/parcellations.py` & `junifer-0.0.3.dev74/junifer/data/parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/tests/test_coordinates.py` & `junifer-0.0.3.dev74/junifer/data/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/tests/test_data_utils.py` & `junifer-0.0.3.dev74/junifer/data/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/tests/test_masks.py` & `junifer-0.0.3.dev74/junifer/data/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/tests/test_parcellations.py` & `junifer-0.0.3.dev74/junifer/data/tests/test_parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/data/utils.py` & `junifer-0.0.3.dev74/junifer/data/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/__init__.py` & `junifer-0.0.3.dev74/junifer/datagrabber/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/aomic/id1000.py` & `junifer-0.0.3.dev74/junifer/datagrabber/aomic/id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/aomic/piop1.py` & `junifer-0.0.3.dev74/junifer/datagrabber/aomic/piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/aomic/piop2.py` & `junifer-0.0.3.dev74/junifer/datagrabber/aomic/piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/aomic/tests/test_id1000.py` & `junifer-0.0.3.dev74/junifer/datagrabber/aomic/tests/test_id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/aomic/tests/test_piop1.py` & `junifer-0.0.3.dev74/junifer/datagrabber/aomic/tests/test_piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/aomic/tests/test_piop2.py` & `junifer-0.0.3.dev74/junifer/datagrabber/aomic/tests/test_piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/base.py` & `junifer-0.0.3.dev74/junifer/datagrabber/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/datalad_base.py` & `junifer-0.0.3.dev74/junifer/datagrabber/datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/hcp1200/datalad_hcp1200.py` & `junifer-0.0.3.dev74/junifer/datagrabber/hcp1200/datalad_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/hcp1200/hcp1200.py` & `junifer-0.0.3.dev74/junifer/datagrabber/hcp1200/hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/hcp1200/tests/test_hcp1200.py` & `junifer-0.0.3.dev74/junifer/datagrabber/hcp1200/tests/test_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/multiple.py` & `junifer-0.0.3.dev74/junifer/datagrabber/multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/pattern.py` & `junifer-0.0.3.dev74/junifer/datagrabber/pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/pattern_datalad.py` & `junifer-0.0.3.dev74/junifer/datagrabber/pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/tests/test_base.py` & `junifer-0.0.3.dev74/junifer/datagrabber/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/tests/test_datagrabber_utils.py` & `junifer-0.0.3.dev74/junifer/datagrabber/tests/test_datagrabber_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/tests/test_datalad_base.py` & `junifer-0.0.3.dev74/junifer/datagrabber/tests/test_datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/tests/test_multiple.py` & `junifer-0.0.3.dev74/junifer/datagrabber/tests/test_multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/tests/test_pattern.py` & `junifer-0.0.3.dev74/junifer/datagrabber/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/tests/test_pattern_datalad.py` & `junifer-0.0.3.dev74/junifer/datagrabber/tests/test_pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datagrabber/utils.py` & `junifer-0.0.3.dev74/junifer/datagrabber/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/datareader/default.py` & `junifer-0.0.3.dev74/junifer/datareader/default.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Provide class for default data reader."""
+"""Provide concrete implementation for default DataReader."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
 from typing import Dict, List, Optional
@@ -28,15 +28,15 @@
 _readers["NIFTI"] = {"func": nib.load, "params": None}
 _readers["CSV"] = {"func": pd.read_csv, "params": None}
 _readers["TSV"] = {"func": pd.read_csv, "params": {"sep": "\t"}}
 
 
 @register_datareader
 class DefaultDataReader(PipelineStepMixin, UpdateMetaMixin):
-    """Mixin class for default data reader."""
+    """Concrete implementation for common data reading."""
 
     def validate_input(self, input: List[str]) -> List[str]:
         """Validate input.
 
         Parameters
         ----------
         input : list of str
@@ -44,14 +44,15 @@
             available Junifer Data dictionary keys.
 
         Returns
         -------
         list of str
             The actual elements of the input that will be processed by this
             pipeline step.
+
         """
         # Nothing to validate, any input is fine
         return input
 
     def get_output_type(self, input: List[str]) -> List[str]:
         """Get output type.
```

### Comparing `junifer-0.0.3.dev73/junifer/datareader/tests/test_default_reader.py` & `junifer-0.0.3.dev74/junifer/datareader/tests/test_default_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Provide tests for default data reader."""
+"""Provide tests for DefaultDataReader."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
 
@@ -15,31 +15,31 @@
 
 from junifer.datareader import DefaultDataReader
 
 
 @pytest.mark.parametrize(
     "type_", [["T1w", "BOLD", "T2", "dwi"], [], ["whatever"]]
 )
-def test_validation(type_) -> None:
-    """Test validating input/output.
+def test_DefaultDataReader_validation(type_) -> None:
+    """Test DefaultDataReader validating input/output.
 
     Parameters
     ----------
     type_ : list of str or str or None
         The parametrized type_ of data.
 
     """
     reader = DefaultDataReader()
     assert reader.validate_input(type_) == type_
     assert reader.get_output_type(type_) == type_
     assert reader.validate(type_) == type_
 
 
-def test_meta() -> None:
-    """Test reader metadata."""
+def test_DefaultDataReader_meta() -> None:
+    """Test DefaultDataReader metadata."""
     reader = DefaultDataReader()
 
     nib_data_path = Path(nib_testing.data_path)
     t_path = nib_data_path / "example4d.nii.gz"
     input = {"BOLD": {"path": t_path}}
     output = reader.fit_transform(input)
     assert "meta" in output["BOLD"]
@@ -48,16 +48,16 @@
     assert "class" in meta["datareader"]
     assert meta["datareader"]["class"] == "DefaultDataReader"
 
 
 @pytest.mark.parametrize(
     "fname", ["example4d.nii.gz", "reoriented_anat_moved.nii"]
 )
-def test_read_nifti(fname: str) -> None:
-    """Test reading NIFTI files.
+def test_DefaultDataReader_nifti(fname: str) -> None:
+    """Test DefaultDataReader reading NIfTI files.
 
     Parameters
     ----------
     fname : str
         The parametrized NIfTI file names for testing.
 
     """
@@ -81,16 +81,16 @@
     assert_array_equal(read_img.get_fdata(), t_read_img.get_fdata())
 
     input = {"BOLD": {"path": t_path.as_posix()}}
     output2 = reader.fit_transform(input)
     assert output["BOLD"]["path"] == output2["BOLD"]["path"]
 
 
-def test_read_unknown() -> None:
-    """Test (not) reading unknown files."""
+def test_DefaultDataReader_unknown() -> None:
+    """Test DefaultDataReader (not) reading unknown files."""
     reader = DefaultDataReader()
     nib_data_path = Path(nib_testing.data_path)
 
     anat_path = nib_data_path / "reoriented_anat_moved.nii"
     whatever_path = nib_data_path / "unexistent.unkwnownextension"
 
     input = {"anat": {"path": anat_path}, "whatever": {"path": whatever_path}}
@@ -111,16 +111,16 @@
     assert output["whatever"]["data"] is None
 
     input = {"whatever": {"nopath": whatever_path}}
     with pytest.warns(RuntimeWarning, match="does not provide a path"):
         reader.fit_transform(input)
 
 
-def test_read_csv(tmp_path: Path) -> None:
-    """Test reading CSV files.
+def test_DefaultDataReader_csv(tmp_path: Path) -> None:
+    """Test DefaultDataReader reading CSV files.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
```

### Comparing `junifer-0.0.3.dev73/junifer/external/h5io/h5io/_h5io.py` & `junifer-0.0.3.dev74/junifer/external/h5io/h5io/_h5io.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/external/h5io/h5io/chunked_array.py` & `junifer-0.0.3.dev74/junifer/external/h5io/h5io/chunked_array.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/external/h5io/h5io/chunked_list.py` & `junifer-0.0.3.dev74/junifer/external/h5io/h5io/chunked_list.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/external/nilearn/junifer_nifti_spheres_masker.py` & `junifer-0.0.3.dev74/junifer/external/nilearn/junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py` & `junifer-0.0.3.dev74/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/__init__.py` & `junifer-0.0.3.dev74/junifer/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/base.py` & `junifer-0.0.3.dev74/junifer/markers/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/collection.py` & `junifer-0.0.3.dev74/junifer/markers/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 class MarkerCollection:
     """Class for marker collection.
 
     Parameters
     ----------
     markers : list of marker-like
         The markers to compute.
-    datareader : datareader-like, optional
-        The datareader to use (default None).
+    datareader : DataReader-like object, optional
+        The DataReader to use (default None).
     preprocessing : preprocessing-like, optional
         The preprocessing steps to apply.
     storage : storage-like, optional
         The storage to use (default None).
 
     """
```

### Comparing `junifer-0.0.3.dev73/junifer/markers/ets_rss.py` & `junifer-0.0.3.dev74/junifer/markers/ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/falff/falff_base.py` & `junifer-0.0.3.dev74/junifer/markers/falff/falff_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/falff/falff_estimator.py` & `junifer-0.0.3.dev74/junifer/markers/falff/falff_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/falff/falff_parcels.py` & `junifer-0.0.3.dev74/junifer/markers/falff/falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/falff/falff_spheres.py` & `junifer-0.0.3.dev74/junifer/markers/falff/falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/falff/tests/test_falff_estimator.py` & `junifer-0.0.3.dev74/junifer/markers/falff/tests/test_falff_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/falff/tests/test_falff_parcels.py` & `junifer-0.0.3.dev74/junifer/markers/falff/tests/test_falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/falff/tests/test_falff_spheres.py` & `junifer-0.0.3.dev74/junifer/markers/falff/tests/test_falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py` & `junifer-0.0.3.dev74/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py` & `junifer-0.0.3.dev74/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py` & `junifer-0.0.3.dev74/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/functional_connectivity/functional_connectivity_base.py` & `junifer-0.0.3.dev74/junifer/markers/functional_connectivity/functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/functional_connectivity/functional_connectivity_parcels.py` & `junifer-0.0.3.dev74/junifer/markers/functional_connectivity/functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/functional_connectivity/functional_connectivity_spheres.py` & `junifer-0.0.3.dev74/junifer/markers/functional_connectivity/functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py` & `junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py` & `junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py` & `junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py` & `junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py` & `junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py` & `junifer-0.0.3.dev74/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/parcel_aggregation.py` & `junifer-0.0.3.dev74/junifer/markers/parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/reho/reho_base.py` & `junifer-0.0.3.dev74/junifer/markers/reho/reho_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/reho/reho_estimator.py` & `junifer-0.0.3.dev74/junifer/markers/reho/reho_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/reho/reho_parcels.py` & `junifer-0.0.3.dev74/junifer/markers/reho/reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/reho/reho_spheres.py` & `junifer-0.0.3.dev74/junifer/markers/reho/reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/reho/tests/test_reho_estimator.py` & `junifer-0.0.3.dev74/junifer/markers/reho/tests/test_reho_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/reho/tests/test_reho_parcels.py` & `junifer-0.0.3.dev74/junifer/markers/reho/tests/test_reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/reho/tests/test_reho_spheres.py` & `junifer-0.0.3.dev74/junifer/markers/reho/tests/test_reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/sphere_aggregation.py` & `junifer-0.0.3.dev74/junifer/markers/sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/temporal_snr/temporal_snr_base.py` & `junifer-0.0.3.dev74/junifer/markers/temporal_snr/temporal_snr_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/temporal_snr/temporal_snr_parcels.py` & `junifer-0.0.3.dev74/junifer/markers/temporal_snr/temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/temporal_snr/temporal_snr_spheres.py` & `junifer-0.0.3.dev74/junifer/markers/temporal_snr/temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py` & `junifer-0.0.3.dev74/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py` & `junifer-0.0.3.dev74/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/tests/test_collection.py` & `junifer-0.0.3.dev74/junifer/markers/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/tests/test_ets_rss.py` & `junifer-0.0.3.dev74/junifer/markers/tests/test_ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/tests/test_marker_utils.py` & `junifer-0.0.3.dev74/junifer/markers/tests/test_marker_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/tests/test_markers_base.py` & `junifer-0.0.3.dev74/junifer/markers/tests/test_markers_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/tests/test_parcel_aggregation.py` & `junifer-0.0.3.dev74/junifer/markers/tests/test_parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/tests/test_sphere_aggregation.py` & `junifer-0.0.3.dev74/junifer/markers/tests/test_sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/markers/utils.py` & `junifer-0.0.3.dev74/junifer/markers/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/pipeline/pipeline_step_mixin.py` & `junifer-0.0.3.dev74/junifer/pipeline/pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/pipeline/registry.py` & `junifer-0.0.3.dev74/junifer/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/pipeline/tests/test_pipeline_step_mixin.py` & `junifer-0.0.3.dev74/junifer/pipeline/tests/test_pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/pipeline/tests/test_registry.py` & `junifer-0.0.3.dev74/junifer/pipeline/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/pipeline/tests/test_update_meta_mixin.py` & `junifer-0.0.3.dev74/junifer/pipeline/tests/test_update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/pipeline/update_meta_mixin.py` & `junifer-0.0.3.dev74/junifer/pipeline/update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/pipeline/utils.py` & `junifer-0.0.3.dev74/junifer/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/preprocess/base.py` & `junifer-0.0.3.dev74/junifer/preprocess/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/preprocess/confounds/fmriprep_confound_remover.py` & `junifer-0.0.3.dev74/junifer/preprocess/confounds/fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py` & `junifer-0.0.3.dev74/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/preprocess/tests/test_preprocess_base.py` & `junifer-0.0.3.dev74/junifer/preprocess/tests/test_preprocess_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/stats.py` & `junifer-0.0.3.dev74/junifer/stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/storage/base.py` & `junifer-0.0.3.dev74/junifer/storage/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/storage/hdf5.py` & `junifer-0.0.3.dev74/junifer/storage/hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/storage/pandas_base.py` & `junifer-0.0.3.dev74/junifer/storage/pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/storage/sqlite.py` & `junifer-0.0.3.dev74/junifer/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/storage/tests/test_hdf5.py` & `junifer-0.0.3.dev74/junifer/storage/tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/storage/tests/test_pandas_base.py` & `junifer-0.0.3.dev74/junifer/storage/tests/test_pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/storage/tests/test_sqlite.py` & `junifer-0.0.3.dev74/junifer/storage/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/storage/tests/test_storage_base.py` & `junifer-0.0.3.dev74/junifer/storage/tests/test_storage_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/storage/tests/test_utils.py` & `junifer-0.0.3.dev74/junifer/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/storage/utils.py` & `junifer-0.0.3.dev74/junifer/storage/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv` & `junifer-0.0.3.dev74/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/testing/datagrabbers.py` & `junifer-0.0.3.dev74/junifer/testing/datagrabbers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/testing/registry.py` & `junifer-0.0.3.dev74/junifer/testing/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py` & `junifer-0.0.3.dev74/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/testing/tests/test_partlycloudytesting_datagrabber.py` & `junifer-0.0.3.dev74/junifer/testing/tests/test_partlycloudytesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/testing/tests/test_spmauditory_datagrabber.py` & `junifer-0.0.3.dev74/junifer/testing/tests/test_spmauditory_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/testing/tests/test_testing_registry.py` & `junifer-0.0.3.dev74/junifer/testing/tests/test_testing_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/testing/utils.py` & `junifer-0.0.3.dev74/junifer/testing/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/tests/test_stats.py` & `junifer-0.0.3.dev74/junifer/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/utils/logging.py` & `junifer-0.0.3.dev74/junifer/utils/logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/utils/tests/test_fs.py` & `junifer-0.0.3.dev74/junifer/utils/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer/utils/tests/test_logging.py` & `junifer-0.0.3.dev74/junifer/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/junifer.egg-info/PKG-INFO` & `junifer-0.0.3.dev74/junifer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.3.dev73
+Version: 0.0.3.dev74
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/junifer
 Project-URL: documentation, https://juaml.github.io/junifer
 Project-URL: repository, https://github.com/juaml/junifer
```

### Comparing `junifer-0.0.3.dev73/junifer.egg-info/SOURCES.txt` & `junifer-0.0.3.dev74/junifer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 docs/changes/newsfragments/.gitignore
 docs/changes/newsfragments/220.doc
 docs/changes/newsfragments/222.change
 docs/changes/newsfragments/222.enh
 docs/changes/newsfragments/223.bugfix
 docs/changes/newsfragments/223.enh
 docs/changes/newsfragments/226.enh
+docs/changes/newsfragments/227.enh
 docs/changes/newsfragments/230.misc
 docs/extending/coordinates.rst
 docs/extending/datagrabber.rst
 docs/extending/extension.rst
 docs/extending/index.rst
 docs/extending/marker.rst
 docs/extending/masks.rst
```

### Comparing `junifer-0.0.3.dev73/pyproject.toml` & `junifer-0.0.3.dev74/pyproject.toml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/tools/create_aomic1000_example_dataset.py` & `junifer-0.0.3.dev74/tools/create_aomic1000_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/tools/create_aomicpiop1_example_dataset.py` & `junifer-0.0.3.dev74/tools/create_aomicpiop1_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/tools/create_aomicpiop2_example_dataset.py` & `junifer-0.0.3.dev74/tools/create_aomicpiop2_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/tools/create_bids_example_dataset.py` & `junifer-0.0.3.dev74/tools/create_bids_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/tools/create_bids_example_dataset_sessions.py` & `junifer-0.0.3.dev74/tools/create_bids_example_dataset_sessions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/tools/create_hcp1200_example_dataset.py` & `junifer-0.0.3.dev74/tools/create_hcp1200_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.3.dev73/tox.ini` & `junifer-0.0.3.dev74/tox.ini`

 * *Files identical despite different names*

