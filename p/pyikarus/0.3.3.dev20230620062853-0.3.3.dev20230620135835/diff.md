# Comparing `tmp/pyikarus-0.3.3.dev20230620062853.tar.gz` & `tmp/pyikarus-0.3.3.dev20230620135835.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.3.dev20230620062853.tar", last modified: Tue Jun 20 06:28:54 2023, max compression
+gzip compressed data, was "pyikarus-0.3.3.dev20230620135835.tar", last modified: Tue Jun 20 13:58:35 2023, max compression
```

## Comparing `pyikarus-0.3.3.dev20230620062853.tar` & `pyikarus-0.3.3.dev20230620135835.tar`

### file list

```diff
@@ -1,336 +1,336 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.181004 pyikarus-0.3.3.dev20230620062853/
--rw-r--r--   0 root         (0) root         (0)      312 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.bettercodehub.yml
--rw-r--r--   0 root         (0) root         (0)     1300 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.clang-format
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.cmake-format
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.093001 pyikarus-0.3.3.dev20230620062853/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.113002 pyikarus-0.3.3.dev20230620062853/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      615 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.117002 pyikarus-0.3.3.dev20230620062853/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/workflows/codespell.yml
--rw-r--r--   0 root         (0) root         (0)     1034 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/workflows/createDockerContainer.yml
--rw-r--r--   0 root         (0) root         (0)     5615 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/workflows/createRelease.yml
--rw-r--r--   0 root         (0) root         (0)     1834 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/workflows/debian-coverage.yml
--rw-r--r--   0 root         (0) root         (0)     2612 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/workflows/debian.yml
--rw-r--r--   0 root         (0) root         (0)     2042 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/workflows/ghpages.yml
--rw-r--r--   0 root         (0) root         (0)     1712 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/workflows/releasePythonPackage.yml
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/workflows/reuseLint.yml
--rw-r--r--   0 root         (0) root         (0)     3335 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/workflows/runExamples.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.117002 pyikarus-0.3.3.dev20230620062853/.github/workflows/scripts/
--rw-r--r--   0 root         (0) root         (0)     3213 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/workflows/scripts/release.py
--rw-r--r--   0 root         (0) root         (0)     1331 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.github/workflows/style.yml
--rw-r--r--   0 root         (0) root         (0)      482 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.117002 pyikarus-0.3.3.dev20230620062853/.reuse/
--rw-r--r--   0 root         (0) root         (0)      661 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/.reuse/dep5
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1251 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5335 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/LICENSE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.117002 pyikarus-0.3.3.dev20230620062853/LICENSES/
--rw-r--r--   0 root         (0) root         (0)    18375 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/LICENSES/CC0-1.0.txt
--rw-r--r--   0 root         (0) root         (0)    42098 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/LICENSES/MIT.txt
--rw-r--r--   0 root         (0) root         (0)    16727 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/LICENSES/MPL-2.0.txt
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-20 06:28:54.181004 pyikarus-0.3.3.dev20230620062853/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3418 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.117002 pyikarus-0.3.3.dev20230620062853/cmake/
--rw-r--r--   0 root         (0) root         (0)      184 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/cmake/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      973 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/cmake/CPM.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.117002 pyikarus-0.3.3.dev20230620062853/cmake/FormatTarget/
--rw-r--r--   0 root         (0) root         (0)     1807 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.121002 pyikarus-0.3.3.dev20230620062853/cmake/modules/
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/cmake/modules/AddMatplotppFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/cmake/modules/AddSpdlogFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/cmake/modules/AddSpectraFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/cmake/modules/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      436 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/cmake/modules/IkarusMacros.cmake
--rw-r--r--   0 root         (0) root         (0)     2040 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/cmake/tools.cmake
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/codecov.yml
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/codespellignore
--rw-r--r--   0 root         (0) root         (0)     1588 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/config.h.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.121002 pyikarus-0.3.3.dev20230620062853/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.121002 pyikarus-0.3.3.dev20230620062853/docs/BuildLocally/
--rw-r--r--   0 root         (0) root         (0)      439 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/BuildLocally/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      333 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.121002 pyikarus-0.3.3.dev20230620062853/docs/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     1136 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rw-r--r--   0 root         (0) root         (0)     6961 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/literature.bib
--rw-r--r--   0 root         (0) root         (0)      117 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/literature.bib.license
--rw-r--r--   0 root         (0) root         (0)     1271 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/mkdocs-macros.py
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/mkdocs.insiders.yml
--rw-r--r--   0 root         (0) root         (0)     5042 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/mkdocs.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.097001 pyikarus-0.3.3.dev20230620062853/docs/overrides/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.121002 pyikarus-0.3.3.dev20230620062853/docs/overrides/partials/
--rw-r--r--   0 root         (0) root         (0)     1732 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/overrides/partials/comments.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.121002 pyikarus-0.3.3.dev20230620062853/docs/website/
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/.meta.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.125002 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/
--rw-r--r--   0 root         (0) root         (0)     4710 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/assembler.md
--rw-r--r--   0 root         (0) root         (0)     6387 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/controlRoutines.md
--rw-r--r--   0 root         (0) root         (0)     2024 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/dirichletBCs.md
--rw-r--r--   0 root         (0) root         (0)     3237 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/feRequirements.md
--rw-r--r--   0 root         (0) root         (0)    12894 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/finiteElements.md
--rw-r--r--   0 root         (0) root         (0)     2745 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/grids.md
--rw-r--r--   0 root         (0) root         (0)     4121 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/index.md
--rw-r--r--   0 root         (0) root         (0)     4932 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/localBasis.md
--rw-r--r--   0 root         (0) root         (0)    44213 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/localFunctions.md
--rw-r--r--   0 root         (0) root         (0)     3978 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/manifolds.md
--rw-r--r--   0 root         (0) root         (0)     2551 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/nonlinearOperator.md
--rw-r--r--   0 root         (0) root         (0)     3086 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/observer.md
--rw-r--r--   0 root         (0) root         (0)     5211 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.129002 pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/
--rw-r--r--   0 root         (0) root         (0)     6655 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/cantileverBeam.md
--rw-r--r--   0 root         (0) root         (0)     7251 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/computePi.md
--rw-r--r--   0 root         (0) root         (0)     5439 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/cooksMembrane.md
--rw-r--r--   0 root         (0) root         (0)     7323 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/incompressibleRubberBlock.md
--rw-r--r--   0 root         (0) root         (0)     2164 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/index.md
--rw-r--r--   0 root         (0) root         (0)     7722 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/kirchhoffPlate.md
--rw-r--r--   0 root         (0) root         (0)     5088 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/newtonRaphsonMethod.md
--rw-r--r--   0 root         (0) root         (0)     6164 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/nonLinearElasticity.md
--rw-r--r--   0 root         (0) root         (0)     4179 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.129002 pyikarus-0.3.3.dev20230620062853/docs/website/03_contribution/
--rw-r--r--   0 root         (0) root         (0)     2439 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/03_contribution/buildDocumentationLocally.md
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/03_contribution/codeStyle.md
--rw-r--r--   0 root         (0) root         (0)     2415 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/03_contribution/howToEdit.md
--rw-r--r--   0 root         (0) root         (0)     1736 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.129002 pyikarus-0.3.3.dev20230620062853/docs/website/04_blog/
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/04_blog/.authors.yml
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/04_blog/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.129002 pyikarus-0.3.3.dev20230620062853/docs/website/04_blog/posts/
--rw-r--r--   0 root         (0) root         (0)     7731 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.129002 pyikarus-0.3.3.dev20230620062853/docs/website/05_cppReferences/
--rw-r--r--   0 root         (0) root         (0)     2324 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.129002 pyikarus-0.3.3.dev20230620062853/docs/website/99_Literature/
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.137003 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/
--rw-r--r--   0 root         (0) root         (0)   280461 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/BigLogo.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.137003 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/
--rw-r--r--   0 root         (0) root         (0)    52795 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rw-r--r--   0 root         (0) root         (0)    46250 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rw-r--r--   0 root         (0) root         (0)     2852 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rw-r--r--   0 root         (0) root         (0)    17924 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rw-r--r--   0 root         (0) root         (0)     9455 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.137003 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/
--rw-r--r--   0 root         (0) root         (0)    35234 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rw-r--r--   0 root         (0) root         (0)    62184 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rw-r--r--   0 root         (0) root         (0)     2281 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rw-r--r--   0 root         (0) root         (0)    40033 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rw-r--r--   0 root         (0) root         (0)    25505 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rw-r--r--   0 root         (0) root         (0)   441218 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/logo_blue.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/logo_blue.png.license
--rw-r--r--   0 root         (0) root         (0)   482004 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/logo_white.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/logo_white.png.license
--rw-r--r--   0 root         (0) root         (0)     4364 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/download.md
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/gallery.md
--rw-r--r--   0 root         (0) root         (0)     1423 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.141003 pyikarus-0.3.3.dev20230620062853/docs/website/javascripts/
--rw-r--r--   0 root         (0) root         (0)      486 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.141003 pyikarus-0.3.3.dev20230620062853/docs/website/stylesheets/
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/docs/website/stylesheets/extra.css
--rw-r--r--   0 root         (0) root         (0)      504 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/dune.module
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.141003 pyikarus-0.3.3.dev20230620062853/ikarus/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.141003 pyikarus-0.3.3.dev20230620062853/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    12924 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/assembler/simpleAssemblers.hh
--rw-r--r--   0 root         (0) root         (0)    10714 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.141003 pyikarus-0.3.3.dev20230620062853/ikarus/controlRoutines/
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/controlRoutines/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2575 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/controlRoutines/loadControl.hh
--rw-r--r--   0 root         (0) root         (0)     2970 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.141003 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.141003 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/feBases/
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/feBases/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5309 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/feBases/autodiffFE.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/feBases/powerBasisFE.hh
--rw-r--r--   0 root         (0) root         (0)     1827 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/feBases/scalarFE.hh
--rw-r--r--   0 root         (0) root         (0)     9346 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/feRequirements.hh
--rw-r--r--   0 root         (0) root         (0)     1338 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.141003 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    21360 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rw-r--r--   0 root         (0) root         (0)    11389 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/kirchhoffloveshell.hh
--rw-r--r--   0 root         (0) root         (0)    14204 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.145003 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/
--rw-r--r--   0 root         (0) root         (0)      397 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5699 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/interface.hh
--rw-r--r--   0 root         (0) root         (0)     2718 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rw-r--r--   0 root         (0) root         (0)     4635 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rw-r--r--   0 root         (0) root         (0)     3809 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rw-r--r--   0 root         (0) root         (0)     5734 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/svk.hh
--rw-r--r--   0 root         (0) root         (0)      473 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/tags.hh
--rw-r--r--   0 root         (0) root         (0)     7995 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rw-r--r--   0 root         (0) root         (0)     1196 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials.hh
--rw-r--r--   0 root         (0) root         (0)    15979 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rw-r--r--   0 root         (0) root         (0)    12678 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.145003 pyikarus-0.3.3.dev20230620062853/ikarus/io/
--rw-r--r--   0 root         (0) root         (0)      258 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/io/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2350 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/io/resultEvaluators.hh
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/io/resultFunction.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.149003 pyikarus-0.3.3.dev20230620062853/ikarus/linearAlgebra/
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/linearAlgebra/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6735 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/linearAlgebra/dirichletValues.hh
--rw-r--r--   0 root         (0) root         (0)     7698 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/linearAlgebra/nonLinearOperator.hh
--rw-r--r--   0 root         (0) root         (0)    12303 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.149003 pyikarus-0.3.3.dev20230620062853/ikarus/python/
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.149003 pyikarus-0.3.3.dev20230620062853/ikarus/python/assembler/
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6752 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.149003 pyikarus-0.3.3.dev20230620062853/ikarus/python/basis/
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/basis/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/basis/basis.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.149003 pyikarus-0.3.3.dev20230620062853/ikarus/python/dirichletValues/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/dirichletValues/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4371 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.149003 pyikarus-0.3.3.dev20230620062853/ikarus/python/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     7858 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.149003 pyikarus-0.3.3.dev20230620062853/ikarus/python/finiteElements/materials/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/finiteElements/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     9949 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/finiteElements/materials/material.hh
--rw-r--r--   0 root         (0) root         (0)     5271 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.153003 pyikarus-0.3.3.dev20230620062853/ikarus/python/test/
--rw-r--r--   0 root         (0) root         (0)      688 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3989 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/test/kltest.py
--rw-r--r--   0 root         (0) root         (0)     3813 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/test/linearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)     4319 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/test/nonLinearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/test/setpath.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.153003 pyikarus-0.3.3.dev20230620062853/ikarus/python/utils/
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.153003 pyikarus-0.3.3.dev20230620062853/ikarus/solver/
--rw-r--r--   0 root         (0) root         (0)      211 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.153003 pyikarus-0.3.3.dev20230620062853/ikarus/solver/linearSolver/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/solver/linearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     8891 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.153003 pyikarus-0.3.3.dev20230620062853/ikarus/solver/nonLinearSolver/
--rw-r--r--   0 root         (0) root         (0)      272 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5406 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rw-r--r--   0 root         (0) root         (0)     8297 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rw-r--r--   0 root         (0) root         (0)    18574 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.161003 pyikarus-0.3.3.dev20230620062853/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      712 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/algorithms.hh
--rw-r--r--   0 root         (0) root         (0)      878 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/autodiffHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/basis.hh
--rw-r--r--   0 root         (0) root         (0)     6930 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/concepts.hh
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.161003 pyikarus-0.3.3.dev20230620062853/ikarus/utils/drawing/
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/drawing/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/drawing/griddrawer.hh
--rw-r--r--   0 root         (0) root         (0)      544 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/drawing/matplotHelper.cpp
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/drawing/matplotHelper.hh
--rw-r--r--   0 root         (0) root         (0)     2484 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/duneUtilities.hh
--rw-r--r--   0 root         (0) root         (0)     2347 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/eigenDuneTransformations.hh
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/eigenSparseAddon.hh
--rw-r--r--   0 root         (0) root         (0)     1367 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/findLineSegment.cpp
--rw-r--r--   0 root         (0) root         (0)      724 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/findLineSegment.hh
--rw-r--r--   0 root         (0) root         (0)     3611 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/flatPreBasis.hh
--rw-r--r--   0 root         (0) root         (0)     2171 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/functionSanityChecks.cpp
--rw-r--r--   0 root         (0) root         (0)     6359 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/functionSanityChecks.hh
--rw-r--r--   0 root         (0) root         (0)     3152 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/init.hh
--rw-r--r--   0 root         (0) root         (0)    15244 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/linearAlgebraHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1711 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.165003 pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/controlLogger.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/controlVTKWriter.hh
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/genericControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/gridDrawerObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1132 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/loadControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/nonLinearSolverLogger.hh
--rw-r--r--   0 root         (0) root         (0)     5497 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/observer.hh
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/observerMessages.hh
--rw-r--r--   0 root         (0) root         (0)     4159 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/pathFollowingFunctions.hh
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/polyfit.cpp
--rw-r--r--   0 root         (0) root         (0)      570 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/polyfit.hh
--rw-r--r--   0 root         (0) root         (0)    10515 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/tensorUtils.hh
--rw-r--r--   0 root         (0) root         (0)    15149 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus/utils/traits.hh
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/ikarus.pc.in
--rw-r--r--   0 root         (0) root         (0)      196 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/iwyu.imp
--rw-r--r--   0 root         (0) root         (0)      422 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.165003 pyikarus-0.3.3.dev20230620062853/python/
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.169004 pyikarus-0.3.3.dev20230620062853/python/ikarus/
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.169004 pyikarus-0.3.3.dev20230620062853/python/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/assembler/__init__.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/basis.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.169004 pyikarus-0.3.3.dev20230620062853/python/ikarus/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6762 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/finiteElements/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/generator.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/materials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.169004 pyikarus-0.3.3.dev20230620062853/python/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      768 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.169004 pyikarus-0.3.3.dev20230620062853/python/pyikarus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-20 06:28:54.000000 pyikarus-0.3.3.dev20230620062853/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10214 2023-06-20 06:28:54.000000 pyikarus-0.3.3.dev20230620062853/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 06:28:54.000000 pyikarus-0.3.3.dev20230620062853/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 06:28:54.000000 pyikarus-0.3.3.dev20230620062853/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-20 06:28:54.000000 pyikarus-0.3.3.dev20230620062853/python/pyikarus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/python/setup.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.169004 pyikarus-0.3.3.dev20230620062853/sandbox/
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/sandbox/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.173004 pyikarus-0.3.3.dev20230620062853/sandbox/src/
--rw-r--r--   0 root         (0) root         (0)     1220 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.173004 pyikarus-0.3.3.dev20230620062853/sandbox/src/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)   674469 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/sandbox/src/auxiliaryFiles/circle.msh
--rw-r--r--   0 root         (0) root         (0)      320 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/sandbox/src/sandbox.cpp
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 06:28:54.181004 pyikarus-0.3.3.dev20230620062853/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1080 2023-06-20 06:28:53.000000 pyikarus-0.3.3.dev20230620062853/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.173004 pyikarus-0.3.3.dev20230620062853/tests/
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.181004 pyikarus-0.3.3.dev20230620062853/tests/src/
--rw-r--r--   0 root         (0) root         (0)     1408 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3907 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testAssembler.cpp
--rw-r--r--   0 root         (0) root         (0)     1292 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testAutodiffHelper.cpp
--rw-r--r--   0 root         (0) root         (0)    14291 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testCommon.hh
--rw-r--r--   0 root         (0) root         (0)     2639 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testDependencies.cpp
--rw-r--r--   0 root         (0) root         (0)     6520 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testDirichletValue.cpp
--rw-r--r--   0 root         (0) root         (0)     4795 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testEAS.hh
--rw-r--r--   0 root         (0) root         (0)     1600 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testEnhancedAssumedStrains.cpp
--rw-r--r--   0 root         (0) root         (0)     5805 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testFEElement.hh
--rw-r--r--   0 root         (0) root         (0)      571 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testFactories.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 06:28:54.181004 pyikarus-0.3.3.dev20230620062853/tests/src/testFiles/
--rw-r--r--   0 root         (0) root         (0)     9028 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testFiles/unstructuredQuadscoarse.msh
--rw-r--r--   0 root         (0) root         (0)      395 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testFiles/unstructuredTest.geo
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testFiles/unstructuredTest.msh
--rw-r--r--   0 root         (0) root         (0)      546 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testFiles/unstructuredTest2.geo
--rw-r--r--   0 root         (0) root         (0)    11431 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testFiles/unstructuredTrianglesfine.msh
--rw-r--r--   0 root         (0) root         (0)     1870 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testFunctionTraits.cpp
--rw-r--r--   0 root         (0) root         (0)     1114 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testHelpers.hh
--rw-r--r--   0 root         (0) root         (0)     3190 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testLinearElasticity.cpp
--rw-r--r--   0 root         (0) root         (0)     2278 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testManifolds.cpp
--rw-r--r--   0 root         (0) root         (0)     7949 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testMaterial.cpp
--rw-r--r--   0 root         (0) root         (0)    15845 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testNonLinearElasticity.hh
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testNonLinearElasticityNeoHooke.cpp
--rw-r--r--   0 root         (0) root         (0)     1121 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testNonLinearElasticitySVK.cpp
--rw-r--r--   0 root         (0) root         (0)     9846 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testNonLinearOperator.cpp
--rw-r--r--   0 root         (0) root         (0)     6251 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testPathFollowing.cpp
--rw-r--r--   0 root         (0) root         (0)     1651 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testPolyFit.cpp
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testPythonConversion.cpp
--rw-r--r--   0 root         (0) root         (0)    17531 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testTrustRegion.cpp
--rw-r--r--   0 root         (0) root         (0)     7005 2023-06-20 06:28:44.000000 pyikarus-0.3.3.dev20230620062853/tests/src/testklshell.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.703859 pyikarus-0.3.3.dev20230620135835/
+-rw-r--r--   0 root         (0) root         (0)      312 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.bettercodehub.yml
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.clang-format
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.cmake-format
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.659860 pyikarus-0.3.3.dev20230620135835/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      615 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/codespell.yml
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/createDockerContainer.yml
+-rw-r--r--   0 root         (0) root         (0)     5615 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/createRelease.yml
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 root         (0) root         (0)     2612 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/debian.yml
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/ghpages.yml
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/releasePythonPackage.yml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/reuseLint.yml
+-rw-r--r--   0 root         (0) root         (0)     3335 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/runExamples.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/.github/workflows/scripts/
+-rw-r--r--   0 root         (0) root         (0)     3213 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/scripts/release.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.github/workflows/style.yml
+-rw-r--r--   0 root         (0) root         (0)      482 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/.reuse/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/.reuse/dep5
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)    18375 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)    42098 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/LICENSES/MIT.txt
+-rw-r--r--   0 root         (0) root         (0)    16727 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-20 13:58:35.703859 pyikarus-0.3.3.dev20230620135835/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3418 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/cmake/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      973 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/CPM.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/cmake/FormatTarget/
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.667860 pyikarus-0.3.3.dev20230620135835/cmake/modules/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/AddMatplotppFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/AddSpdlogFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/AddSpectraFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      436 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/modules/IkarusMacros.cmake
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/cmake/tools.cmake
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/codecov.yml
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/codespellignore
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/config.h.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.671860 pyikarus-0.3.3.dev20230620135835/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.671860 pyikarus-0.3.3.dev20230620135835/docs/BuildLocally/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/BuildLocally/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.671860 pyikarus-0.3.3.dev20230620135835/docs/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rw-r--r--   0 root         (0) root         (0)     6961 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/literature.bib
+-rw-r--r--   0 root         (0) root         (0)      117 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/literature.bib.license
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/mkdocs-macros.py
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/mkdocs.insiders.yml
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/mkdocs.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.659860 pyikarus-0.3.3.dev20230620135835/docs/overrides/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.671860 pyikarus-0.3.3.dev20230620135835/docs/overrides/partials/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/overrides/partials/comments.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.671860 pyikarus-0.3.3.dev20230620135835/docs/website/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/.meta.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.671860 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/
+-rw-r--r--   0 root         (0) root         (0)     4710 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/assembler.md
+-rw-r--r--   0 root         (0) root         (0)     6387 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/controlRoutines.md
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/dirichletBCs.md
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/feRequirements.md
+-rw-r--r--   0 root         (0) root         (0)    12894 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/finiteElements.md
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/grids.md
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/index.md
+-rw-r--r--   0 root         (0) root         (0)     4932 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/localBasis.md
+-rw-r--r--   0 root         (0) root         (0)    44213 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/localFunctions.md
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/manifolds.md
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/nonlinearOperator.md
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/observer.md
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/cantileverBeam.md
+-rw-r--r--   0 root         (0) root         (0)     7251 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/computePi.md
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/cooksMembrane.md
+-rw-r--r--   0 root         (0) root         (0)     7323 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/incompressibleRubberBlock.md
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/index.md
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/kirchhoffPlate.md
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/newtonRaphsonMethod.md
+-rw-r--r--   0 root         (0) root         (0)     6164 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/nonLinearElasticity.md
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/buildDocumentationLocally.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/codeStyle.md
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/howToEdit.md
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/04_blog/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/04_blog/.authors.yml
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/04_blog/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/04_blog/posts/
+-rw-r--r--   0 root         (0) root         (0)     7731 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/05_cppReferences/
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/99_Literature/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.675860 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/
+-rw-r--r--   0 root         (0) root         (0)   280461 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/BigLogo.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.679859 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/
+-rw-r--r--   0 root         (0) root         (0)    52795 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)    46250 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rw-r--r--   0 root         (0) root         (0)    17924 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)     9455 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.679859 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/
+-rw-r--r--   0 root         (0) root         (0)    35234 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rw-r--r--   0 root         (0) root         (0)    62184 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rw-r--r--   0 root         (0) root         (0)    40033 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rw-r--r--   0 root         (0) root         (0)    25505 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rw-r--r--   0 root         (0) root         (0)   441218 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/logo_blue.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/logo_blue.png.license
+-rw-r--r--   0 root         (0) root         (0)   482004 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/logo_white.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/logo_white.png.license
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/download.md
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/gallery.md
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.679859 pyikarus-0.3.3.dev20230620135835/docs/website/javascripts/
+-rw-r--r--   0 root         (0) root         (0)      486 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.679859 pyikarus-0.3.3.dev20230620135835/docs/website/stylesheets/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/docs/website/stylesheets/extra.css
+-rw-r--r--   0 root         (0) root         (0)      504 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/dune.module
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.679859 pyikarus-0.3.3.dev20230620135835/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.679859 pyikarus-0.3.3.dev20230620135835/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    12924 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/assembler/simpleAssemblers.hh
+-rw-r--r--   0 root         (0) root         (0)    10714 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.683859 pyikarus-0.3.3.dev20230620135835/ikarus/controlRoutines/
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/controlRoutines/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/controlRoutines/loadControl.hh
+-rw-r--r--   0 root         (0) root         (0)     2970 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.683859 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.683859 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5309 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/autodiffFE.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/scalarFE.hh
+-rw-r--r--   0 root         (0) root         (0)     9346 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feRequirements.hh
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.683859 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    21360 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rw-r--r--   0 root         (0) root         (0)    11389 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/kirchhoffloveshell.hh
+-rw-r--r--   0 root         (0) root         (0)    14204 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.683859 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/interface.hh
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/svk.hh
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/tags.hh
+-rw-r--r--   0 root         (0) root         (0)     7995 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials.hh
+-rw-r--r--   0 root         (0) root         (0)    15979 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rw-r--r--   0 root         (0) root         (0)    12678 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.683859 pyikarus-0.3.3.dev20230620135835/ikarus/io/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/io/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/io/resultEvaluators.hh
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/io/resultFunction.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6735 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/dirichletValues.hh
+-rw-r--r--   0 root         (0) root         (0)     7698 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/nonLinearOperator.hh
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/assembler/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6752 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/basis/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/basis/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/basis/basis.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/dirichletValues/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/dirichletValues/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4371 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     7858 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/materials/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     9949 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/materials/material.hh
+-rw-r--r--   0 root         (0) root         (0)     5271 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/test/
+-rw-r--r--   0 root         (0) root         (0)      688 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3989 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/test/kltest.py
+-rw-r--r--   0 root         (0) root         (0)     3813 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/test/linearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)     4319 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/test/nonLinearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/test/setpath.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/python/utils/
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/solver/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/solver/linearSolver/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/linearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     8891 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.687859 pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5406 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rw-r--r--   0 root         (0) root         (0)     8297 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rw-r--r--   0 root         (0) root         (0)    18574 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.691859 pyikarus-0.3.3.dev20230620135835/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/algorithms.hh
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/autodiffHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/basis.hh
+-rw-r--r--   0 root         (0) root         (0)     6930 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/concepts.hh
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.691859 pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/griddrawer.hh
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/matplotHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/matplotHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/duneUtilities.hh
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/eigenDuneTransformations.hh
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/eigenSparseAddon.hh
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/findLineSegment.cpp
+-rw-r--r--   0 root         (0) root         (0)      724 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/findLineSegment.hh
+-rw-r--r--   0 root         (0) root         (0)     3611 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/flatPreBasis.hh
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/functionSanityChecks.cpp
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/functionSanityChecks.hh
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/init.hh
+-rw-r--r--   0 root         (0) root         (0)    15244 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/linearAlgebraHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/controlLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/controlVTKWriter.hh
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/genericControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/gridDrawerObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/loadControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/observer.hh
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/observerMessages.hh
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/pathFollowingFunctions.hh
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/polyfit.cpp
+-rw-r--r--   0 root         (0) root         (0)      570 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/polyfit.hh
+-rw-r--r--   0 root         (0) root         (0)    10515 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/tensorUtils.hh
+-rw-r--r--   0 root         (0) root         (0)    15149 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus/utils/traits.hh
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/ikarus.pc.in
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/iwyu.imp
+-rw-r--r--   0 root         (0) root         (0)      422 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/python/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/python/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/python/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/assembler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/basis.py
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/python/ikarus/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6762 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/finiteElements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/generator.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/materials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/python/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      768 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-20 13:58:35.000000 pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10214 2023-06-20 13:58:35.000000 pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 13:58:35.000000 pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-20 13:58:35.000000 pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-20 13:58:35.000000 pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/python/setup.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/sandbox/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/sandbox/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/sandbox/src/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.695859 pyikarus-0.3.3.dev20230620135835/sandbox/src/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)   674469 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/sandbox/src/auxiliaryFiles/circle.msh
+-rw-r--r--   0 root         (0) root         (0)      320 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/sandbox/src/sandbox.cpp
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 13:58:35.703859 pyikarus-0.3.3.dev20230620135835/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-06-20 13:58:35.000000 pyikarus-0.3.3.dev20230620135835/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.699859 pyikarus-0.3.3.dev20230620135835/tests/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.699859 pyikarus-0.3.3.dev20230620135835/tests/src/
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testAssembler.cpp
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testAutodiffHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)    14291 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testCommon.hh
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testDependencies.cpp
+-rw-r--r--   0 root         (0) root         (0)     6520 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testDirichletValue.cpp
+-rw-r--r--   0 root         (0) root         (0)     4795 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testEAS.hh
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testEnhancedAssumedStrains.cpp
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFEElement.hh
+-rw-r--r--   0 root         (0) root         (0)      571 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFactories.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:58:35.703859 pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/
+-rw-r--r--   0 root         (0) root         (0)     9028 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rw-r--r--   0 root         (0) root         (0)      395 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredTest.geo
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredTest.msh
+-rw-r--r--   0 root         (0) root         (0)      546 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredTest2.geo
+-rw-r--r--   0 root         (0) root         (0)    11431 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testFunctionTraits.cpp
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testHelpers.hh
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testLinearElasticity.cpp
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testManifolds.cpp
+-rw-r--r--   0 root         (0) root         (0)     7949 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testMaterial.cpp
+-rw-r--r--   0 root         (0) root         (0)    15845 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearElasticityNeoHooke.cpp
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearElasticitySVK.cpp
+-rw-r--r--   0 root         (0) root         (0)     9846 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearOperator.cpp
+-rw-r--r--   0 root         (0) root         (0)     6251 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testPathFollowing.cpp
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testPolyFit.cpp
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testPythonConversion.cpp
+-rw-r--r--   0 root         (0) root         (0)    17531 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testTrustRegion.cpp
+-rw-r--r--   0 root         (0) root         (0)     7005 2023-06-20 13:58:27.000000 pyikarus-0.3.3.dev20230620135835/tests/src/testklshell.cpp
```

### Comparing `pyikarus-0.3.3.dev20230620062853/.clang-format` & `pyikarus-0.3.3.dev20230620135835/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/.cmake-format` & `pyikarus-0.3.3.dev20230620135835/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.3.dev20230620135835/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.3.dev20230620135835/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/.github/workflows/createRelease.yml` & `pyikarus-0.3.3.dev20230620135835/.github/workflows/createRelease.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.3.dev20230620135835/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/.github/workflows/debian.yml` & `pyikarus-0.3.3.dev20230620135835/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/.github/workflows/ghpages.yml` & `pyikarus-0.3.3.dev20230620135835/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/.github/workflows/releasePythonPackage.yml` & `pyikarus-0.3.3.dev20230620135835/.github/workflows/releasePythonPackage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/.github/workflows/runExamples.yml` & `pyikarus-0.3.3.dev20230620135835/.github/workflows/runExamples.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/.github/workflows/scripts/release.py` & `pyikarus-0.3.3.dev20230620135835/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/.github/workflows/style.yml` & `pyikarus-0.3.3.dev20230620135835/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/.reuse/dep5` & `pyikarus-0.3.3.dev20230620135835/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/CHANGELOG.md` & `pyikarus-0.3.3.dev20230620135835/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/CMakeLists.txt` & `pyikarus-0.3.3.dev20230620135835/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/CODE_OF_CONDUCT.md` & `pyikarus-0.3.3.dev20230620135835/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/LICENSE.md` & `pyikarus-0.3.3.dev20230620135835/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.3.dev20230620135835/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.3.dev20230620135835/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.3.dev20230620135835/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/LICENSES/MIT.txt` & `pyikarus-0.3.3.dev20230620135835/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.3.dev20230620135835/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/PKG-INFO` & `pyikarus-0.3.3.dev20230620135835/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.3.dev20230620062853
+Version: 0.3.3.dev20230620135835
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230620062853 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230620135835 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
 markdown License-File: LICENSE.md  # Ikarus [docs/website/auxiliaryImages/
 BigLogo.png]
```

### Comparing `pyikarus-0.3.3.dev20230620062853/README.md` & `pyikarus-0.3.3.dev20230620135835/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/cmake/CPM.cmake` & `pyikarus-0.3.3.dev20230620135835/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.3.dev20230620135835/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.3.dev20230620135835/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.3.dev20230620135835/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.3.dev20230620135835/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.3.dev20230620135835/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/cmake/modules/AddSpectraFlags.cmake` & `pyikarus-0.3.3.dev20230620135835/cmake/modules/AddSpectraFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/cmake/tools.cmake` & `pyikarus-0.3.3.dev20230620135835/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/config.h.cmake` & `pyikarus-0.3.3.dev20230620135835/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.3.dev20230620135835/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/literature.bib` & `pyikarus-0.3.3.dev20230620135835/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/mkdocs-macros.py` & `pyikarus-0.3.3.dev20230620135835/docs/mkdocs-macros.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/mkdocs.yml` & `pyikarus-0.3.3.dev20230620135835/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/overrides/partials/comments.html` & `pyikarus-0.3.3.dev20230620135835/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/assembler.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/finiteElements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/grids.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/index.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/localFunctions.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/nonlinearOperator.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/observer.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/01_framework/solvers.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/cantileverBeam.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/computePi.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/computePi.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/cooksMembrane.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/index.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/kirchhoffPlate.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/nonLinearElasticity.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/02_examples/vonMisesTruss.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/03_contribution/openTask.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/BigLogo.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/BigLogo.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/logo_blue.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/logo_blue.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/auxiliaryImages/logo_white.png` & `pyikarus-0.3.3.dev20230620135835/docs/website/auxiliaryImages/logo_white.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/download.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/docs/website/index.md` & `pyikarus-0.3.3.dev20230620135835/docs/website/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/CMakeLists.txt` & `pyikarus-0.3.3.dev20230620135835/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/assembler/simpleAssemblers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.3.dev20230620135835/ikarus/assembler/simpleAssemblers.inl`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/feBases/autodiffFE.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/autodiffFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feRequirements.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/kirchhoffloveshell.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/kirchhoffloveshell.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/materials.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/mechanics/nonLinearElastic.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/mechanics/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/finiteElements/physicsHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/io/resultEvaluators.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/io/resultEvaluators.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/io/resultFunction.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/io/resultFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/python/assembler/flatAssembler.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/python/assembler/flatAssembler.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/python/basis/basis.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/python/basis/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/python/finiteElements/materials/material.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/materials/material.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/python/finiteElements/nonLinearElastic.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/python/test/CMakeLists.txt` & `pyikarus-0.3.3.dev20230620135835/ikarus/python/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/python/test/kltest.py` & `pyikarus-0.3.3.dev20230620135835/ikarus/python/test/kltest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.3.dev20230620135835/ikarus/python/test/linearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.3.dev20230620135835/ikarus/python/test/nonLinearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.3.dev20230620135835/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/python/utils/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/algorithms.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/basis.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/concepts.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/flatPreBasis.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/flatPreBasis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/init.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/polyfit.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/ikarus/utils/traits.hh` & `pyikarus-0.3.3.dev20230620135835/ikarus/utils/traits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/python/ikarus/__init__.py` & `pyikarus-0.3.3.dev20230620135835/python/ikarus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/python/ikarus/_ikarus.cc` & `pyikarus-0.3.3.dev20230620135835/python/ikarus/_ikarus.cc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/python/ikarus/assembler/__init__.py` & `pyikarus-0.3.3.dev20230620135835/python/ikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/python/ikarus/basis.py` & `pyikarus-0.3.3.dev20230620135835/python/ikarus/basis.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/python/ikarus/dirichletValues.py` & `pyikarus-0.3.3.dev20230620135835/python/ikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/python/ikarus/finiteElements/__init__.py` & `pyikarus-0.3.3.dev20230620135835/python/ikarus/finiteElements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/python/ikarus/generator.py` & `pyikarus-0.3.3.dev20230620135835/python/ikarus/generator.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/python/ikarus/materials.py` & `pyikarus-0.3.3.dev20230620135835/python/ikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/python/ikarus/utils/__init__.py` & `pyikarus-0.3.3.dev20230620135835/python/ikarus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.3.dev20230620062853
+Version: 0.3.3.dev20230620135835
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230620062853 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230620135835 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
 markdown License-File: LICENSE.md  # Ikarus [docs/website/auxiliaryImages/
 BigLogo.png]
```

### Comparing `pyikarus-0.3.3.dev20230620062853/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.3.dev20230620135835/python/pyikarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/python/setup.py.in` & `pyikarus-0.3.3.dev20230620135835/python/setup.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.3.dev20230620135835/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.3.dev20230620135835/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/setup.py` & `pyikarus-0.3.3.dev20230620135835/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # build _ikarus
 # cd /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
 # /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 
-ikarusVersion = "0.3.3.dev20230620062853"
+ikarusVersion = "0.3.3.dev20230620135835"
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
 # refactor since ikarus pypi package already exists
 metadata["name"] = "pyikarus"
```

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/CMakeLists.txt` & `pyikarus-0.3.3.dev20230620135835/tests/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testAssembler.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testAssembler.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testCommon.hh` & `pyikarus-0.3.3.dev20230620135835/tests/src/testCommon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testDependencies.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testDependencies.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testDirichletValue.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testDirichletValue.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testEAS.hh` & `pyikarus-0.3.3.dev20230620135835/tests/src/testEAS.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testEnhancedAssumedStrains.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testEnhancedAssumedStrains.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testFEElement.hh` & `pyikarus-0.3.3.dev20230620135835/tests/src/testFEElement.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testFactories.hh` & `pyikarus-0.3.3.dev20230620135835/tests/src/testFactories.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.3.dev20230620135835/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testFunctionTraits.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testFunctionTraits.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testHelpers.hh` & `pyikarus-0.3.3.dev20230620135835/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testLinearElasticity.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testLinearElasticity.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testManifolds.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testManifolds.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testMaterial.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testMaterial.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testNonLinearElasticity.hh` & `pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testNonLinearElasticityNeoHooke.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearElasticityNeoHooke.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testNonLinearElasticitySVK.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearElasticitySVK.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testNonLinearOperator.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testNonLinearOperator.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testPathFollowing.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testPathFollowing.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testPolyFit.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testPolyFit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testPythonConversion.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testPythonConversion.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testTrustRegion.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testTrustRegion.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230620062853/tests/src/testklshell.cpp` & `pyikarus-0.3.3.dev20230620135835/tests/src/testklshell.cpp`

 * *Files identical despite different names*

