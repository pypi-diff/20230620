# Comparing `tmp/PyScaffold-4.4.1.tar.gz` & `tmp/PyScaffold-4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pyscaffold/pyscaffold/dist/.tmp-9k67q_dv/PyScaffold-4.4.1.tar", last modified: Tue Apr 18 16:08:44 2023, max compression
+gzip compressed data, was "/home/runner/work/pyscaffold/pyscaffold/dist/.tmp-7do441f9/PyScaffold-4.5.tar", last modified: Tue Jun 20 16:24:51 2023, max compression
```

## Comparing `PyScaffold-4.4.1.tar` & `PyScaffold-4.5.tar`

### file list

```diff
@@ -1,237 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.cirrus.yml
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/workflows/make-demo-repo.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.github/workflows/publish-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    23399 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/control
--rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/debian/source/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/source/format
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/source/options
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/debian/watch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/_static/pyscaffold-custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/action-pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21433 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/dev-guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/example_setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/examples/cirrus-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/examples/gitlab-ci-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/examples/namespace-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/examples/no-skeleton-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/examples/no-tox-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/examples/pre-commit-extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/features.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/docs/gfx/
--rwxr-xr-x   0 runner    (1001) docker     (123)   159443 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/action-pipeline-paths.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    36777 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/action-pipeline.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)   165295 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/api-paths.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    34942 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/api.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)   134198 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/demo.cast
--rwxr-xr-x   0 runner    (1001) docker     (123)  4772106 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/demo.gif
--rw-r--r--   0 runner    (1001) docker     (123)   115081 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/github_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    71500 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/github_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/sidebar.png
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/gfx/simple-icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/project-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/reasons.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/updating.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:08:43.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/PyScaffold.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/pyscaffold/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/cirrus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    11422 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/no_pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/no_skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/no_tox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/pre_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/extensions/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/src/pyscaffold/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/__init__.template
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/authors.template
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/changelog.template
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/cirrus.template
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/conftest_py.template
--rw-r--r--   0 runner    (1001) docker     (123)    13814 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/contributing.template
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/coveragerc.template
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/github_ci_workflow.template
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/gitignore.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/gitignore_empty.template
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/gitlab_ci.template
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/header_interactive.template
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/isort_cfg.template
--rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_affero_3.0.template
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_apache.template
--rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_artistic_2.0.template
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_bsd0.template
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_cc0_1.0.template
--rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_eclipse_1.0.template
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_gpl_2.0.template
--rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_gpl_3.0.template
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_isc.template
--rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_lgpl_2.1.template
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_lgpl_3.0.template
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_mit.template
--rw-r--r--   0 runner    (1001) docker     (123)    15922 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_mozilla.template
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_new_bsd.template
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_none.template
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_public_domain.template
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/license_simplified_bsd.template
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/pre-commit-config.template
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/pyproject_toml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/readme.template
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/rtd_cfg.template
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/rtd_requirements.template
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/setup_cfg.template
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/setup_py.template
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/skeleton.template
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_authors.template
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_changelog.template
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_conf.template
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_contributing.template
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_index.template
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_license.template
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_makefile.template
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_readme.template
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/test_skeleton.template
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/templates/tox_ini.template
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/src/pyscaffold/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/demoapp/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/demoapp_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/demoapp_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp_data/data/hello_world.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp_data/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp_data/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp_data/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/demoapp_data/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/examples/issue-506/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/examples/issue-506/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/incompatible_v3_api_fake_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_cirrus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_github_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_interactive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8481 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_no_pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_no_skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_no_tox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_pre_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/extensions/test_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/log_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:44.000000 PyScaffold-4.4.1/tests/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/system/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/system/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/system/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/system/test_dependency_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_install.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11611 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2890 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_termui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-18 16:08:28.000000 PyScaffold-4.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-20 16:24:35.000000 PyScaffold-4.5/.cirrus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-20 16:24:35.000000 PyScaffold-4.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-20 16:24:35.000000 PyScaffold-4.5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 16:24:35.000000 PyScaffold-4.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-20 16:24:35.000000 PyScaffold-4.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-20 16:24:35.000000 PyScaffold-4.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-20 16:24:35.000000 PyScaffold-4.5/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-20 16:24:35.000000 PyScaffold-4.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-20 16:24:35.000000 PyScaffold-4.5/.github/workflows/make-demo-repo.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-20 16:24:35.000000 PyScaffold-4.5/.github/workflows/publish-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-20 16:24:35.000000 PyScaffold-4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-20 16:24:35.000000 PyScaffold-4.5/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-20 16:24:35.000000 PyScaffold-4.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 16:24:35.000000 PyScaffold-4.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-20 16:24:35.000000 PyScaffold-4.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23851 2023-06-20 16:24:35.000000 PyScaffold-4.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24441 2023-06-20 16:24:35.000000 PyScaffold-4.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-20 16:24:35.000000 PyScaffold-4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-06-20 16:24:51.000000 PyScaffold-4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-06-20 16:24:35.000000 PyScaffold-4.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-20 16:24:35.000000 PyScaffold-4.5/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-20 16:24:35.000000 PyScaffold-4.5/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-20 16:24:35.000000 PyScaffold-4.5/debian/control
+-rwxr-xr-x   0 runner    (1001) docker     (123)      117 2023-06-20 16:24:35.000000 PyScaffold-4.5/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 16:24:35.000000 PyScaffold-4.5/debian/source/format
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 16:24:35.000000 PyScaffold-4.5/debian/source/options
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-20 16:24:35.000000 PyScaffold-4.5/debian/watch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/_static/pyscaffold-custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/action-pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21433 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/dev-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/example_setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/examples/cirrus-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/examples/gitlab-ci-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/examples/namespace-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/examples/no-skeleton-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/examples/no-tox-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/examples/pre-commit-extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/features.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/docs/gfx/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   159443 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/action-pipeline-paths.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36777 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/action-pipeline.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   165295 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/api-paths.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34942 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/api.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   134198 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/demo.cast
+-rwxr-xr-x   0 runner    (1001) docker     (123)  4772106 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   115081 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/github_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71500 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/github_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15073 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/sidebar.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/gfx/simple-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/project-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/reasons.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/updating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-06-20 16:24:35.000000 PyScaffold-4.5/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-20 16:24:35.000000 PyScaffold-4.5/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-20 16:24:35.000000 PyScaffold-4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-20 16:24:51.000000 PyScaffold-4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-20 16:24:35.000000 PyScaffold-4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/src/PyScaffold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-06-20 16:24:51.000000 PyScaffold-4.5/src/PyScaffold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-20 16:24:51.000000 PyScaffold-4.5/src/PyScaffold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:24:51.000000 PyScaffold-4.5/src/PyScaffold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-20 16:24:51.000000 PyScaffold-4.5/src/PyScaffold.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:24:51.000000 PyScaffold-4.5/src/PyScaffold.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-20 16:24:51.000000 PyScaffold-4.5/src/PyScaffold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 16:24:51.000000 PyScaffold-4.5/src/PyScaffold.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/src/pyscaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/src/pyscaffold/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/extensions/cirrus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/extensions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/extensions/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/extensions/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11422 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/extensions/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/extensions/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/extensions/no_pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/extensions/no_skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/extensions/no_tox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/extensions/pre_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/extensions/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/src/pyscaffold/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/__init__.template
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/authors.template
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/changelog.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/cirrus.template
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/conftest_py.template
+-rw-r--r--   0 runner    (1001) docker     (123)    13814 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/contributing.template
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/coveragerc.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/github_ci_workflow.template
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/gitignore_empty.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/gitlab_ci.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/header_interactive.template
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/isort_cfg.template
+-rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_affero_3.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_apache.template
+-rw-r--r--   0 runner    (1001) docker     (123)     8917 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_artistic_2.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_bsd0.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_cc0_1.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_eclipse_1.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_gpl_2.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_gpl_3.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_isc.template
+-rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_lgpl_2.1.template
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_lgpl_3.0.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_mit.template
+-rw-r--r--   0 runner    (1001) docker     (123)    15922 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_mozilla.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_new_bsd.template
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_none.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_public_domain.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/license_simplified_bsd.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/pre-commit-config.template
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/pyproject_toml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/readme.template
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/rtd_cfg.template
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/rtd_requirements.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/setup_cfg.template
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/setup_py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/skeleton.template
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/sphinx_authors.template
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/sphinx_changelog.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/sphinx_conf.template
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/sphinx_contributing.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/sphinx_index.template
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/sphinx_license.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/sphinx_makefile.template
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/sphinx_readme.template
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/test_skeleton.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/templates/tox_ini.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-06-20 16:24:35.000000 PyScaffold-4.5/src/pyscaffold/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/tests/demoapp/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/demoapp/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/demoapp/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/demoapp/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/demoapp/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/tests/demoapp_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/tests/demoapp_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/demoapp_data/data/hello_world.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/demoapp_data/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/demoapp_data/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/demoapp_data/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/demoapp_data/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/tests/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/tests/examples/issue-506/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/examples/issue-506/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/incompatible_v3_api_fake_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/test_cirrus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/test_github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/test_gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/test_interactive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8481 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/test_no_pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/test_no_skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/test_no_tox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/test_pre_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/extensions/test_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/log_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:51.000000 PyScaffold-4.5/tests/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/system/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/system/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/system/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/system/test_dependency_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_install.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11611 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2890 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-20 16:24:35.000000 PyScaffold-4.5/tests/virtualenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-20 16:24:35.000000 PyScaffold-4.5/tox.ini
```

### Comparing `PyScaffold-4.4.1/.cirrus.yml` & `PyScaffold-4.5/.cirrus.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ---
 # ---- Default values to be merged into tasks ----
 
 env:
-  LC_ALL: C.UTF-8
-  LANG: C.UTF-8
+  LC_ALL: C
+  LC_CTYPE: UTF-8
+  LANG: C
   PIP_CACHE_DIR: ${CIRRUS_WORKING_DIR}/.cache/pip
   PRE_COMMIT_HOME: ${CIRRUS_WORKING_DIR}/.cache/pre-commit
   # Coveralls configuration
   CI_NAME: cirrus-ci
   CI_BRANCH: ${CIRRUS_BRANCH}
   CI_PULL_REQUEST: ${CIRRUS_PR}
   CI_BUILD_NUMBER: ${CIRRUS_BUILD_ID}
```

### Comparing `PyScaffold-4.4.1/.coveragerc` & `PyScaffold-4.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/.github/FUNDING.yml` & `PyScaffold-4.5/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `PyScaffold-4.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/.github/workflows/codeql-analysis.yml` & `PyScaffold-4.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/.github/workflows/make-demo-repo.yml` & `PyScaffold-4.5/.github/workflows/make-demo-repo.yml`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/.github/workflows/publish-package.yml` & `PyScaffold-4.5/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/.gitignore` & `PyScaffold-4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/.pre-commit-config.yaml` & `PyScaffold-4.5/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -14,49 +14,49 @@
   - id: debug-statements
   - id: end-of-file-fixer
   - id: requirements-txt-fixer
   - id: mixed-line-ending
     args: ['--fix=lf']
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
+  rev: v3.7.0
   hooks:
   - id: pyupgrade
     args: ['--py36-plus']
 
 - repo: https://github.com/PyCQA/autoflake
-  rev: v2.1.0
+  rev: v2.1.1
   hooks:
   - id: autoflake
     args: [
       --in-place,
       --remove-all-unused-imports,
       --remove-unused-variables,
     ]
 
 - repo: https://github.com/PyCQA/isort
-  rev: 5.11.5
+  rev: 5.12.0
   hooks:
   - id: isort
 
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/asottile/blacken-docs
-  rev: 1.13.0
+  rev: 1.14.0
   hooks:
   - id: blacken-docs
     additional_dependencies: [black]
 
 - repo: https://github.com/PyCQA/flake8
-  rev: 5.0.4
+  rev: 6.0.0
   hooks:
   - id: flake8
     additional_dependencies: [flake8-bugbear!=23.1.14]
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.4
+  rev: v2.2.5
   hooks:
   - id: codespell
```

### Comparing `PyScaffold-4.4.1/.readthedocs.yml` & `PyScaffold-4.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/CHANGELOG.rst` & `PyScaffold-4.5/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,27 @@
     Development version
     ===================
 
     Version 4.X.X, 2023-XX-XX
     -------------------------
 
 
+Development version
+===================
+
+Version 4.5.0, 2023-06-20
+-------------------------
+
+- Change macOS default configuration dir from
+  ``~/Library/Preferences`` to ``~/Library/Application Support``, :pr:`721`.
+  This change is motivated by the upgrade in the ``platformdirs`` dependency.
+  You can read more about the motivation in :github:`platformdirs/platformdirs#98`
+- Simplify ``git`` command, by letting exceptions go through, :pr:`714`
+
+
 Current versions
 ================
 
 Version 4.4.1, 2023-04-18
 -------------------------
 
 - Re-use pre-built wheels in CI for upgrade tests in :pr:`702`
```

### Comparing `PyScaffold-4.4.1/CONTRIBUTING.rst` & `PyScaffold-4.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/LICENSE.txt` & `PyScaffold-4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/PKG-INFO` & `PyScaffold-4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyScaffold
-Version: 4.4.1
+Version: 4.5
 Summary: Template tool for putting up the scaffold of a Python project
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Florian Wilhelm
 Author-email: Florian.Wilhelm@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/pyscaffold/pyscaffold/
```

### Comparing `PyScaffold-4.4.1/README.rst` & `PyScaffold-4.5/README.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/Makefile` & `PyScaffold-4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/_static/pyscaffold-custom.css` & `PyScaffold-4.5/docs/_static/pyscaffold-custom.css`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/action-pipeline.rst` & `PyScaffold-4.5/docs/action-pipeline.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/conf.py` & `PyScaffold-4.5/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     "sphinx.ext.doctest",
     "sphinx.ext.ifconfig",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
     "sphinx.ext.extlinks",
     "sphinx_copybutton",
     "sphinxemoji.sphinxemoji",
+    "sphinx_github_role",
 ]
 
 # TODO: Autodoc cannot leave type hints alone (without expansion), as result the docs
 #       become unreadable (unfortunately). For the time being, let's skip annotations
 #       and hope support for type aliases gets better in the near future.
 autodoc_typehints = "none"
 
@@ -311,11 +312,11 @@
     "configupdater": ("https://configupdater.readthedocs.io/en/stable/", None),
 }
 extlinks = {
     "issue": (f"{repository}/issues/%s", "issue #%s"),
     "pr": (f"{repository}/pull/%s", "PR #%s"),
     "discussion": (f"{repository}/discussions/%s", "discussion #%s"),
     "pypi": ("https://pypi.org/project/%s", "%s"),
-    "github": ("https://github.com/%s", "%s"),
+    # "github" is handled by sphinx_github_role
 }
 
 print(f"loading configurations for {project} {version} ...", file=sys.stderr)
```

### Comparing `PyScaffold-4.4.1/docs/dependencies.rst` & `PyScaffold-4.5/docs/dependencies.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/dev-guide.rst` & `PyScaffold-4.5/docs/dev-guide.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/example_setup.cfg` & `PyScaffold-4.5/docs/example_setup.cfg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/extensions.rst` & `PyScaffold-4.5/docs/extensions.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/faq.rst` & `PyScaffold-4.5/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/features.rst` & `PyScaffold-4.5/docs/features.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/action-pipeline-paths.svg` & `PyScaffold-4.5/docs/gfx/action-pipeline-paths.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/action-pipeline.svg` & `PyScaffold-4.5/docs/gfx/action-pipeline.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/api-paths.svg` & `PyScaffold-4.5/docs/gfx/api-paths.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/api.svg` & `PyScaffold-4.5/docs/gfx/api.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/demo.cast` & `PyScaffold-4.5/docs/gfx/demo.cast`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/demo.gif` & `PyScaffold-4.5/docs/gfx/demo.gif`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/github_logo.png` & `PyScaffold-4.5/docs/gfx/github_logo.png`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/github_logo.svg` & `PyScaffold-4.5/docs/gfx/github_logo.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/logo.ico` & `PyScaffold-4.5/docs/gfx/logo.ico`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/logo.png` & `PyScaffold-4.5/docs/gfx/logo.png`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/logo.svg` & `PyScaffold-4.5/docs/gfx/logo.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/sidebar.png` & `PyScaffold-4.5/docs/gfx/sidebar.png`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/gfx/simple-icon.svg` & `PyScaffold-4.5/docs/gfx/simple-icon.svg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/index.rst` & `PyScaffold-4.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/install.rst` & `PyScaffold-4.5/docs/install.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/migration.rst` & `PyScaffold-4.5/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/project-structure.rst` & `PyScaffold-4.5/docs/project-structure.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/reasons.rst` & `PyScaffold-4.5/docs/reasons.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/updating.rst` & `PyScaffold-4.5/docs/updating.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/docs/usage.rst` & `PyScaffold-4.5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/setup.cfg` & `PyScaffold-4.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 packages = find_namespace:
 python_requires = >=3.6
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	platformdirs>=2,<3
+	platformdirs>=2,<4
 	configupdater>=3.0,<4  # pyscaffoldext-custom-extension should have a compatible range
 	setuptools>=46.1.0
 	setuptools_scm>=5
 	tomlkit>=0.7.0,<2
 	packaging>=20.7
 	colorama>=0.4.4; sys_platform == "win32"
 
@@ -76,17 +76,14 @@
 	tox         # system tests use tox inside tox
 	pre-commit  # system tests run pre-commit
 	sphinx      # system tests build docs
 	flake8      # system tests run flake8
 	virtualenv  # virtualenv as dependency for the venv extension in `-e fast`
 	pytest
 	pytest-cov
-	pytest-shutil
-	pytest-virtualenv
-	pytest-fixture-config
 	pytest-xdist
 	pytest-randomly
 
 [options.entry_points]
 console_scripts = 
 	putup = pyscaffold.cli:run
 pyscaffold.cli =
```

### Comparing `PyScaffold-4.4.1/src/PyScaffold.egg-info/PKG-INFO` & `PyScaffold-4.5/src/PyScaffold.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyScaffold
-Version: 4.4.1
+Version: 4.5
 Summary: Template tool for putting up the scaffold of a Python project
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Florian Wilhelm
 Author-email: Florian.Wilhelm@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/pyscaffold/pyscaffold/
```

### Comparing `PyScaffold-4.4.1/src/PyScaffold.egg-info/SOURCES.txt` & `PyScaffold-4.5/src/PyScaffold.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -178,14 +178,15 @@
 tests/test_repo.py
 tests/test_shell.py
 tests/test_structure.py
 tests/test_templates.py
 tests/test_termui.py
 tests/test_toml.py
 tests/test_update.py
+tests/virtualenv.py
 tests/demoapp/pyproject.toml
 tests/demoapp/runner.py
 tests/demoapp/setup.cfg
 tests/demoapp/setup.py
 tests/demoapp_data/pyproject.toml
 tests/demoapp_data/runner.py
 tests/demoapp_data/setup.cfg
```

### Comparing `PyScaffold-4.4.1/src/PyScaffold.egg-info/entry_points.txt` & `PyScaffold-4.5/src/PyScaffold.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/actions.py` & `PyScaffold-4.5/src/pyscaffold/actions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/api.py` & `PyScaffold-4.5/src/pyscaffold/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     opts.update(kwargs)
 
     # Clean up:
     opts = {k: v for k, v in opts.items() if v or v is False}
     # ^  remove empty items, so we ensure setdefault works
 
     # Add options stored in config files:
+    info._migrate_old_macos_config()
     default_files = [info.config_file(default=None)]
     opts.setdefault("config_files", [f for f in default_files if f and f.exists()])
     # ^  make sure the file exists before passing it ahead
     opts = _read_existing_config(opts)
 
     # Add defaults last, so they don't overwrite:
     opts.update({k: v for k, v in DEFAULT_OPTIONS.items() if k not in opts})
```

### Comparing `PyScaffold-4.4.1/src/pyscaffold/cli.py` & `PyScaffold-4.5/src/pyscaffold/cli.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/dependencies.py` & `PyScaffold-4.5/src/pyscaffold/dependencies.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/exceptions.py` & `PyScaffold-4.5/src/pyscaffold/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/extensions/__init__.py` & `PyScaffold-4.5/src/pyscaffold/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/extensions/cirrus.py` & `PyScaffold-4.5/src/pyscaffold/extensions/cirrus.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/extensions/config.py` & `PyScaffold-4.5/src/pyscaffold/extensions/config.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/extensions/github_actions.py` & `PyScaffold-4.5/src/pyscaffold/extensions/github_actions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/extensions/gitlab_ci.py` & `PyScaffold-4.5/src/pyscaffold/extensions/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/extensions/interactive.py` & `PyScaffold-4.5/src/pyscaffold/extensions/interactive.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/extensions/namespace.py` & `PyScaffold-4.5/src/pyscaffold/extensions/namespace.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/extensions/no_pyproject.py` & `PyScaffold-4.5/src/pyscaffold/extensions/no_pyproject.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/extensions/no_skeleton.py` & `PyScaffold-4.5/src/pyscaffold/extensions/no_skeleton.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/extensions/no_tox.py` & `PyScaffold-4.5/src/pyscaffold/extensions/no_tox.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/extensions/pre_commit.py` & `PyScaffold-4.5/src/pyscaffold/extensions/pre_commit.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/extensions/venv.py` & `PyScaffold-4.5/src/pyscaffold/extensions/venv.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/file_system.py` & `PyScaffold-4.5/src/pyscaffold/file_system.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/identification.py` & `PyScaffold-4.5/src/pyscaffold/identification.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/info.py` & `PyScaffold-4.5/src/pyscaffold/info.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Provide general information about the system, user and the package itself.
 """
 
 import copy
 import getpass
 import os
 import socket
+import sys
 from enum import Enum
 from operator import itemgetter
 from pathlib import Path
 from typing import Optional, Set, cast, overload
 
 import platformdirs
 from configupdater import ConfigUpdater
@@ -82,16 +83,14 @@
                 raise GitNotConfigured from ex
     return mail
 
 
 def is_git_installed() -> bool:
     """Check if git is installed"""
     logger.report("check", "is git installed...")
-    if shell.git is None:
-        return False
     try:
         shell.git("--version")
     except ShellCommandException:
         return False
     return True
 
 
@@ -383,7 +382,38 @@
         default = None
 
     dir = config_dir(prog, org, default)
     if dir is None:
         return default_file
 
     return dir / name
+
+
+def _old_macos_config_dir(new_dir: Path) -> Path:
+    return Path(
+        str(new_dir)
+        .replace(os.sep, "/")
+        .replace("/Library/Application Support/", "/Library/Preferences/")
+    )
+
+
+def _migrate_old_macos_config(prog: str = PKG_NAME, org: Optional[str] = None):
+    """Compensate for macOS backward incompatible change in platformdirs 3.0.0"""
+    if not sys.platform.startswith("darwin"):
+        return
+
+    try:
+        new_dir = config_dir(prog, org)
+        old_dir = _old_macos_config_dir(new_dir)
+        if new_dir.exists() or not old_dir.exists():
+            return
+
+        logger.report("move", str(old_dir), target=str(new_dir))
+        new_dir.parent.mkdir(parents=True, exist_ok=True)
+        old_dir.rename(new_dir)
+    except Exception:  # pragma: no cover
+        logger.debug(
+            "Error trying to migrate old macOS config dir. "
+            "If you have an older PyScaffold config file, please make sure to "
+            f"manually copy it to `~/Library/Application Support/{prog}/`",
+            exc_info=True,
+        )
```

### Comparing `PyScaffold-4.4.1/src/pyscaffold/log.py` & `PyScaffold-4.5/src/pyscaffold/log.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/operations.py` & `PyScaffold-4.5/src/pyscaffold/operations.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/repo.py` & `PyScaffold-4.5/src/pyscaffold/repo.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,13 +88,11 @@
 
     Args:
         default: if no git root is found, default is returned
 
     Returns:
         str: top-level path or *default*
     """
-    if shell.git is None:
-        return default
     try:
         return next(shell.git("rev-parse", "--show-toplevel"))
     except ShellCommandException:
         return default
```

### Comparing `PyScaffold-4.4.1/src/pyscaffold/shell.py` & `PyScaffold-4.5/src/pyscaffold/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,18 @@
     "vi": [],  # POSIX
 }
 """Programs to be tried (in sequence) when calling :obj:`edit` and :obj:`get_editor` in
 the case the environment variables EDITOR and VISUAL are not set.
 """
 
 
+_GIT_CMD = "git"
+_GIT_CMD_WIN = "git.exe"
+
+
 class ShellCommand:
     """Shell command that can be called with flags like git('add', 'file')
 
     Args:
         command: command to handle
         shell: run the command in the shell (``True`` by default).
         cwd: current working dir to run the command
@@ -100,17 +104,16 @@
         # ^ Joining and then splitting is the only way of supporting all the cases
 
     def __call__(self, *args, **kwargs) -> Iterator[str]:
         """Execute the command, returning an iterator for the resulting text output"""
         try:
             completed = self.run(*args, **kwargs)
         except FileNotFoundError as e:
-            msg = f"{e.strerror}: {e.filename}"
-            logger.report("info", f'last command failed with "{msg}"')
-            raise ShellCommandException(msg) from e
+            logger.report("info", f'last command failed with "{e!s}"')
+            raise ShellCommandException(str(e)) from e
 
         try:
             completed.check_returncode()
         except subprocess.CalledProcessError as e:
             stdout, stderr = (e or "" for e in (completed.stdout, completed.stderr))
             stdout, stderr = (e.strip() for e in (stdout, stderr))
             sep = "; " if stdout and stderr else ""
@@ -138,50 +141,40 @@
             sys.exit(1)
 
     return func_wrapper
 
 
 # ToDo: Change this to just `cache` from Python 3.9 on.
 @lru_cache(maxsize=None)
-def get_git_cmd(**args):
+def get_git_cmd(**args) -> ShellCommand:
     """Retrieve the git shell command depending on the current platform
 
     Args:
         **args: additional keyword arguments to :obj:`~.ShellCommand`
     """
     if IS_WINDOWS:  # pragma: no cover
         # ^  CI setup does not aggregate Windows coverage
         for shell in (True, False):
-            git = ShellCommand("git.exe", shell=shell, **args)
+            cmd = ShellCommand(_GIT_CMD_WIN, shell=shell, **args)
             try:
-                git("--version")
+                cmd("--version")
             except ShellCommandException:
                 continue
-            return git
-        else:
-            return None
-    else:
-        git = ShellCommand("git", **args)
-        try:
-            git("--version")
-        except ShellCommandException:
-            return None
-        return git
+            return cmd  # available and works with either shell=True or shell=False
+        return cmd  # not available, but we return it anyway for better error messages
+    return ShellCommand(_GIT_CMD, **args)
 
 
 def command_exists(cmd: str) -> bool:
     """Check if command exists
 
     Args:
         cmd: executable name
     """
-    if shutil.which(cmd) is None:
-        return False
-    else:
-        return True
+    return shutil.which(cmd) is not None
 
 
 def get_executable(
     name: str, prefix: PathLike = sys.prefix, include_path=True
 ) -> Optional[str]:
     """Find an executable in the system, if available.
 
@@ -225,15 +218,15 @@
     if shell:
         executable = join([executable])
 
     kwargs["shell"] = shell
     return ShellCommand(executable, **kwargs)
 
 
-def get_editor(**kwargs):
+def get_editor(**kwargs) -> str:
     """Get an available text editor program"""
     from_env = os.getenv("VISUAL") or os.getenv("EDITOR")
     if from_env:
         return from_env  # user is responsible for proper quoting
 
     candidates = ((get_executable(e), opts) for e, opts in EDITORS.items())
     editor, opts = next((c for c in candidates if c[0]), (None, [""]))
@@ -260,12 +253,12 @@
 
     return " ".join(shlex.quote(str(p)) for p in parts)
     # ^  TODO: Replace with `shlex.join(map(str, parts))` when Python >= 3.8
 
 
 def git(*args, **kwargs) -> Iterator[str]:
     """Command for git"""
-    return get_git_cmd()(*args, **kwargs)
+    return get_git_cmd()(*args, **kwargs)  # delayed, so errors show up with --verbose
 
 
 #: Command for python
 python = ShellCommand(sys.executable)
```

### Comparing `PyScaffold-4.4.1/src/pyscaffold/structure.py` & `PyScaffold-4.5/src/pyscaffold/structure.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/__init__.py` & `PyScaffold-4.5/src/pyscaffold/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/__init__.template` & `PyScaffold-4.5/src/pyscaffold/templates/__init__.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/cirrus.template` & `PyScaffold-4.5/src/pyscaffold/templates/cirrus.template`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 # - https://cirrus-ci.org/guide/writing-tasks/
 # THIS FILE IS SUPPOSED TO BE AN EXAMPLE. MODIFY IT ACCORDING TO YOUR NEEDS!
 
 ---
 # ---- Default values to be merged into tasks ----
 
 env:
-  LC_ALL: C.UTF-8
-  LANG: C.UTF-8
+  LC_ALL: C
+  LC_CTYPE: UTF-8
+  LANG: C
   PIP_CACHE_DIR: ${CIRRUS_WORKING_DIR}/.cache/pip
   PRE_COMMIT_HOME: ${CIRRUS_WORKING_DIR}/.cache/pre-commit
   # Coveralls configuration
   CI_NAME: cirrus-ci
   CI_BRANCH: ${CIRRUS_BRANCH}
   CI_PULL_REQUEST: ${CIRRUS_PR}
   CI_BUILD_NUMBER: ${CIRRUS_BUILD_ID}
@@ -187,8 +188,8 @@
     #       in Cirrus CI web interface using an encrypted variable.
     # See:
     # - https://pypi.org/help/#apitoken
     # - https://cirrus-ci.org/guide/writing-tasks/#encrypted-variables
   install_script: pip install tox
   publish_script:
     - ls dist/*
-    - tox -e publish
+    - tox -e publis
```

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/contributing.template` & `PyScaffold-4.5/src/pyscaffold/templates/contributing.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/coveragerc.template` & `PyScaffold-4.5/src/pyscaffold/templates/coveragerc.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/github_ci_workflow.template` & `PyScaffold-4.5/src/pyscaffold/templates/github_ci_workflow.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/gitignore.template` & `PyScaffold-4.5/src/pyscaffold/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/gitlab_ci.template` & `PyScaffold-4.5/src/pyscaffold/templates/gitlab_ci.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/header_interactive.template` & `PyScaffold-4.5/src/pyscaffold/templates/header_interactive.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_affero_3.0.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_affero_3.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_apache.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_apache.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_artistic_2.0.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_artistic_2.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_bsd0.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_bsd0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_cc0_1.0.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_cc0_1.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_eclipse_1.0.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_eclipse_1.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_gpl_2.0.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_gpl_2.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_gpl_3.0.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_gpl_3.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_isc.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_isc.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_lgpl_2.1.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_lgpl_2.1.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_lgpl_3.0.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_lgpl_3.0.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_mit.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_mit.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_mozilla.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_mozilla.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_new_bsd.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_new_bsd.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_public_domain.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_public_domain.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/license_simplified_bsd.template` & `PyScaffold-4.5/src/pyscaffold/templates/license_simplified_bsd.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/pre-commit-config.template` & `PyScaffold-4.5/src/pyscaffold/templates/pre-commit-config.template`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
   - id: end-of-file-fixer
   - id: requirements-txt-fixer
   - id: mixed-line-ending
     args: ['--fix=auto']  # replace 'auto' with 'lf' to enforce Linux/Mac line endings or 'crlf' for Windows
 
 ## If you want to automatically "modernize" your Python code:
 # - repo: https://github.com/asottile/pyupgrade
-#   rev: v3.3.1
+#   rev: v3.7.0
 #   hooks:
 #   - id: pyupgrade
 #     args: ['--py37-plus']
 
 ## If you want to avoid flake8 errors due to unused vars or imports:
 # - repo: https://github.com/PyCQA/autoflake
-#   rev: v2.0.2
+#   rev: v2.1.1
 #   hooks:
 #   - id: autoflake
 #     args: [
 #       --in-place,
 #       --remove-all-unused-imports,
 #       --remove-unused-variables,
 #     ]
@@ -58,10 +58,10 @@
   hooks:
   - id: flake8
   ## You can add flake8 plugins via `additional_dependencies`:
   #  additional_dependencies: [flake8-bugbear]
 
 ## Check for misspells in documentation files:
 # - repo: https://github.com/codespell-project/codespell
-#   rev: v2.2.4
+#   rev: v2.2.5
 #   hooks:
 #   - id: codespell
```

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/readme.template` & `PyScaffold-4.5/src/pyscaffold/templates/readme.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/rtd_cfg.template` & `PyScaffold-4.5/src/pyscaffold/templates/rtd_cfg.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/setup_cfg.template` & `PyScaffold-4.5/src/pyscaffold/templates/setup_cfg.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/setup_py.template` & `PyScaffold-4.5/src/pyscaffold/templates/setup_py.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/skeleton.template` & `PyScaffold-4.5/src/pyscaffold/templates/skeleton.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_conf.template` & `PyScaffold-4.5/src/pyscaffold/templates/sphinx_conf.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_index.template` & `PyScaffold-4.5/src/pyscaffold/templates/sphinx_index.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/sphinx_makefile.template` & `PyScaffold-4.5/src/pyscaffold/templates/sphinx_makefile.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/test_skeleton.template` & `PyScaffold-4.5/src/pyscaffold/templates/test_skeleton.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/templates/tox_ini.template` & `PyScaffold-4.5/src/pyscaffold/templates/tox_ini.template`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/termui.py` & `PyScaffold-4.5/src/pyscaffold/termui.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/toml.py` & `PyScaffold-4.5/src/pyscaffold/toml.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/src/pyscaffold/update.py` & `PyScaffold-4.5/src/pyscaffold/update.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/conftest.py` & `PyScaffold-4.5/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import os
-import shlex
 import sys
 from distutils.util import strtobool
 from importlib import reload
 from pathlib import Path
 from tempfile import mkdtemp
 from types import SimpleNamespace as Object
 
@@ -20,14 +19,15 @@
     command_exception,
     disable_import,
     nop,
     replace_import,
     rmpath,
     uniqstr,
 )
+from .virtualenv import VirtualEnv
 
 IS_POSIX = os.name == "posix"
 
 
 def _config_git(home):
     config = """
         [user]
@@ -103,57 +103,38 @@
     confdir = Path(mkdtemp(prefix="conf", dir=str(tmp_path)))
     monkeypatch.setattr("pyscaffold.info.config_dir", lambda *_, **__: confdir)
     yield confdir
     rmpath(confdir)
 
 
 @pytest.fixture
-def venv(fake_home, fake_xdg_config_home):
+def venv(tmp_path, fake_home, fake_xdg_config_home):
     """Create a virtualenv for each test"""
-    from pytest_virtualenv import VirtualEnv
-
-    virtualenv = VirtualEnv()
+    virtualenv = VirtualEnv(".venv", tmp_path)
     virtualenv.env["HOME"] = str(fake_home)
     virtualenv.env["USERPROFILE"] = str(fake_home)
     virtualenv.env["XDG_CONFIG_HOME"] = str(fake_xdg_config_home)
 
     trusted = os.environ.get("PIP_TRUSTED_HOST")
     if trusted:
         virtualenv.env["PIP_TRUSTED_HOST"] = trusted
 
     cache = os.environ.get("PIP_CACHE")
     if cache:
         virtualenv.env["PIP_CACHE"] = cache
 
-    return virtualenv
-
-
-@pytest.fixture
-def venv_run(venv):
-    """Run a command inside the venv"""
-
-    class Functor:
-        def __init__(self):
-            self.venv = venv
-
-        def __call__(self, *args, **kwargs):
-            # pytest-virtualenv doesn't play nicely with external os.chdir
-            # so let's be explicit about it...
-            kwargs["cd"] = os.getcwd()
-            kwargs["capture"] = True
-            if len(args) == 1 and isinstance(args[0], str):
-                args = shlex.split(args[0], posix=IS_POSIX)
-            return self.venv.run(args, **kwargs).strip()
+    virtualenv.create()
 
-    return Functor()
+    return virtualenv
 
 
 @pytest.fixture
-def venv_path(venv):
-    return str(venv.virtualenv)
+def existing_venv(venv):
+    """Alias of ``venv`` to avoid clashes with ``pyscaffold.extensions.venv``"""
+    return venv
 
 
 @pytest.fixture
 def pyscaffold():
     return __import__("pyscaffold")
 
 
@@ -270,17 +251,25 @@
         raise command_exception("No git mock!")
 
     monkeypatch.setattr("pyscaffold.shell.git", raise_error)
     yield
 
 
 @pytest.fixture
-def nonegit_mock(monkeypatch):
-    monkeypatch.setattr("pyscaffold.shell.git", None)
+def nogit_cmd_mock(monkeypatch):
+    # With this fixture we still allow all the code paths in `get_git_cmd` to be
+    # traversed during tests, so we improve the chances of catching errors.
+    monkeypatch.setattr("pyscaffold.shell._GIT_CMD", "git-cmd.not-installed")
+    monkeypatch.setattr("pyscaffold.shell._GIT_CMD_WIN", "git-cmd.not-installed.exe")
+
+    from pyscaffold import shell
+
+    shell.get_git_cmd.cache_clear()  # force reloading _GIT_CMD
     yield
+    shell.get_git_cmd.cache_clear()  # force reloading _GIT_CMD
 
 
 @pytest.fixture
 def noconfgit_mock(monkeypatch):
     def raise_error(*argv):
         if "config" in argv:
             raise command_exception("No git mock!")
```

### Comparing `PyScaffold-4.4.1/tests/demoapp/runner.py` & `PyScaffold-4.5/tests/demoapp/runner.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/demoapp/setup.cfg` & `PyScaffold-4.5/tests/demoapp/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/demoapp_data/runner.py` & `PyScaffold-4.5/tests/demoapp_data/runner.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/demoapp_data/setup.cfg` & `PyScaffold-4.5/tests/demoapp_data/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/examples/issue-506/setup.cfg` & `PyScaffold-4.5/tests/examples/issue-506/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/extensions/incompatible_v3_api_fake_extension.py` & `PyScaffold-4.5/tests/extensions/incompatible_v3_api_fake_extension.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/extensions/test_cirrus.py` & `PyScaffold-4.5/tests/extensions/test_cirrus.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/extensions/test_config.py` & `PyScaffold-4.5/tests/extensions/test_config.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/extensions/test_github_actions.py` & `PyScaffold-4.5/tests/extensions/test_github_actions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/extensions/test_gitlab_ci.py` & `PyScaffold-4.5/tests/extensions/test_gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/extensions/test_interactive.py` & `PyScaffold-4.5/tests/extensions/test_interactive.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/extensions/test_namespace.py` & `PyScaffold-4.5/tests/extensions/test_namespace.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/extensions/test_no_pyproject.py` & `PyScaffold-4.5/tests/extensions/test_no_pyproject.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/extensions/test_no_skeleton.py` & `PyScaffold-4.5/tests/extensions/test_no_skeleton.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/extensions/test_no_tox.py` & `PyScaffold-4.5/tests/extensions/test_no_tox.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/extensions/test_pre_commit.py` & `PyScaffold-4.5/tests/extensions/test_pre_commit.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/extensions/test_venv.py` & `PyScaffold-4.5/tests/extensions/test_venv.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,16 @@
             assert list(path.glob("*/python*"))
             assert list(chain(path.glob("*/pip*"), path.glob("*/activate*")))
 
     rmpath(folder)
 
 
 @pytest.mark.slow
-def test_install_packages(venv_path, tmpfolder):
-    venv_path = Path(str(venv_path)).resolve()
+def test_install_packages(existing_venv, tmpfolder):
+    venv_path = existing_venv.path.resolve()
     tmp = Path(str(tmpfolder)).resolve()
 
     # Given packages are not installed
     for pkg in "pytest pip-compile".split():
         assert venv.get_executable(pkg, venv_path, False) is None
 
     # when we run install_packages
@@ -143,25 +143,24 @@
 
     # then they should be installed
     for pkg in "pytest pip-compile".split():
         bin_dir = str(Path(venv.get_executable(pkg, venv_path, False)).parent)
         assert bin_dir.lower().startswith(str(venv_path).lower())
 
 
-def test_install_packages_no_pip(venv_path, tmpfolder, monkeypatch):
-    venv_path = Path(str(venv_path)).resolve()
+def test_install_packages_no_pip(tmpfolder, monkeypatch):
     tmp = Path(str(tmpfolder)).resolve()
 
     # Given pip is not installed
     monkeypatch.setattr(venv, "get_command", Mock(return_value=None))
 
     # when we run install_packages
     opts = {
         "project_path": tmp,
-        "venv": venv_path,
+        "venv": tmp / ".venv",
         "venv_install": ["pytest>=6.0.0", "pip-tools"],
     }
     with pytest.raises(venv.NotInstalled) as ex:
         # Then it should throw an exception
         venv.install_packages({}, opts)
 
     assert "pip cannot be found" in str(ex)
```

### Comparing `PyScaffold-4.4.1/tests/helpers.py` & `PyScaffold-4.5/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/log_helpers.py` & `PyScaffold-4.5/tests/log_helpers.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/system/helpers.py` & `PyScaffold-4.5/tests/system/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 import traceback
 from importlib.util import find_spec
 from os import environ
 from pathlib import Path
 from shutil import which
 from subprocess import STDOUT, CalledProcessError, check_output
+from typing import List, Tuple
 
 import pytest
 
 IS_POSIX = os.name == "posix"
 
 PYTHON = sys.executable
 """Same python executable executing the tests... Hopefully the one inside the virtualenv
@@ -46,41 +47,48 @@
     """Create a dict from merging items to the current ``os.environ``"""
     env = {k: v for k, v in environ.items()}  # Clone the environ as a dict
     env.update(other or {})
     env.update(kwargs)
     return env
 
 
-def run(*args, **kwargs):
-    """Run the external command. See ``subprocess.check_output``."""
+def normalize_run_args(args: List[str], kwargs: dict) -> Tuple[List[str], dict]:
     # normalize args
     if len(args) == 1:
         if isinstance(args[0], str):
             args = shlex.split(args[0], posix=IS_POSIX)
-        else:
-            args = args[0]
-
-    if args[0] in ("python", "putup", "pip", "tox", "pytest", "pre-commit"):
-        raise SystemError("Please specify an executable with explicit path")
 
     opts = dict(stderr=STDOUT, universal_newlines=True, encoding="utf-8")
     opts.update(kwargs)
 
+    return [str(x) for x in args], opts
+
+
+def run_with_debug(args: List[str], kwargs: dict):
+    """Run the external command. See ``subprocess.check_output``."""
     try:
-        return check_output(args, **opts)
+        return check_output(args if len(args) > 1 else args[0], **kwargs).strip()
     except CalledProcessError as ex:
         print("Error while running command:")
         print(args)
-        print(opts)
+        print(kwargs)
         traceback.print_exc()
         msg = "******************** Terminal ($? = {}) ********************\n{}"
         print(msg.format(ex.returncode, ex.output))
         raise
 
 
+def run(*args, **kwargs):
+    """Run the external command. See ``subprocess.check_output``."""
+    args, kwargs = normalize_run_args(args, kwargs)
+    if args[0] in ("python", "putup", "pip", "tox", "pytest", "pre-commit"):
+        raise SystemError("Please specify an executable with explicit path")
+    return run_with_debug(args, kwargs)
+
+
 def sphinx_cmd(build):
     docs_dir = Path("docs")
     build_dir = docs_dir / "_build"
     doctrees = build_dir / "doctrees"
     output_dir = build_dir / build
     return f"{PYTHON} -m sphinx -b {build} -d {doctrees} {docs_dir} {output_dir}"
```

### Comparing `PyScaffold-4.4.1/tests/system/test_common.py` & `PyScaffold-4.5/tests/system/test_common.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/system/test_dependency_managers.py` & `PyScaffold-4.5/tests/system/test_dependency_managers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import os
 import sys
 from functools import partial
-from os import environ
 from pathlib import Path
 from subprocess import CalledProcessError
 
 import pytest
 
 from pyscaffold import __version__ as pyscaffold_version
 from pyscaffold.api import create_project
@@ -14,52 +13,55 @@
 
 from .helpers import find_venv_bin, run
 
 pytestmark = [pytest.mark.slow, pytest.mark.system]
 
 
 @pytest.fixture(autouse=True)
-def dont_load_dotenv():
+def dont_load_dotenv(monkeypatch):
     """pytest-virtualenv creates a `.env` directory by default, but `.env`
     entries in the file system are loaded by Pipenv as dotenv files.
 
     To prevent errors for happening we have to disable this feature.
 
     Additionally, it seems that env vars have to be changed before using
     venv, so an autouse fixture is required (cannot put this part in the
     beginning of the test function.
     """
-    environ["PIPENV_DONT_LOAD_ENV"] = "1"
+    monkeypatch.setenv("PIPENV_DONT_LOAD_ENV", "1")
+    monkeypatch.setenv("PIPENV_IGNORE_VIRTUALENVS", "1")
+    monkeypatch.setenv("PIP_IGNORE_INSTALLED", "1")
+    monkeypatch.setenv("PIPENV_VERBOSITY", "-1")
 
 
 @pytest.mark.skipif(
     os.name == "nt", reason="pipenv fails due to colors (non-utf8) under Windows 10"
 )
-def test_pipenv_works_with_pyscaffold(tmpfolder, venv_path, venv_run):
+def test_pipenv_works_with_pyscaffold(tmpfolder, monkeypatch, venv):
     # Given a project is created with pyscaffold
     # and it has some dependencies in setup.cfg
     create_project(project_path="myproj", requirements=["platformdirs"])
 
     if any(ch in pyscaffold_version for ch in ("b", "a", "pre", "rc")):
         flags = "--pre"
     else:
         flags = ""
 
     with tmpfolder.join("myproj").as_cwd():
         # When we install pipenv,
-        venv_run("pip install -v pipenv")
+        venv.run("pip install -v pipenv")
 
         try:
-            venv_run("pipenv --bare install certifi")
+            venv.run("pipenv --bare install certifi")
             # use it to proxy setup.cfg
-            venv_run(f"pipenv --bare install {flags} -e .")
+            venv.run(f"pipenv --bare install {flags} -e .")
             # and install things to the dev env,
-            venv_run("pipenv --bare install --dev flake8")
+            venv.run("pipenv --bare install --dev flake8")
             # Then it should be able to generate a Pipfile.lock
-            venv_run("pipenv lock")
+            venv.run("pipenv lock")
         except Exception:
             if sys.version_info[:2] <= (3, 6):
                 # TODO: Remove try...except when 3.6 is no longer supported
                 pytest.skip("Skip Pipenv specific problem for 3.6")
             else:
                 raise
 
@@ -68,30 +70,34 @@
         # with the correct dependencies
         with open("Pipfile.lock") as fp:
             content = json.load(fp)
             assert content["default"]["platformdirs"]
             assert content["develop"]["flake8"]
 
         # and run things from inside pipenv's venv
-        assert venv_path in venv_run("pipenv run which flake8")
-        venv_run("pipenv --bare run flake8 src/myproj/skeleton.py")
+        pipenv_path = venv.run("pipenv --venv")
+        assert pipenv_path in venv.run("pipenv run which flake8")
+        venv.run("pipenv --bare run flake8 src/myproj/skeleton.py")
 
 
+@pytest.mark.xfail(
+    sys.version_info < (3, 7), reason="pip-compile may fail in old Python"
+)
 def test_piptools_works_with_pyscaffold(tmpfolder, monkeypatch):
     venv_path = Path(str(tmpfolder), "myproj/.venv").resolve()
     find = partial(find_venv_bin, venv_path)
     # Given a project is created with pyscaffold
     # and it has some dependencies in setup.cfg
     create_project(
         project_path="myproj", extensions=[Venv()], requirements=["platformdirs"]
     )
     with tmpfolder.join("myproj").as_cwd():
         requirements_in = Path("requirements.in")
         # When we install pip-tools
-        run(f"{find('pip')} install -v pip-tools certifi")
+        run(f"{find('python')} -m pip install -v pip-tools certifi")
         # and write a requirements.in file that proxies setup.cfg
         # and install other things,
         requirements_in.write_text("-e file:.\nflake8")
         # Then we should be able to generate a requirements.txt
         run(find("pip-compile"))
         requirements_txt = Path("requirements.txt")
         assert requirements_txt.exists()
```

### Comparing `PyScaffold-4.4.1/tests/test_actions.py` & `PyScaffold-4.5/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_api.py` & `PyScaffold-4.5/tests/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from os.path import getmtime
 from pathlib import Path
+from tempfile import TemporaryDirectory
 from textwrap import dedent
 
 import pytest
 
 from pyscaffold import cli, info, operations, structure, templates
 from pyscaffold.actions import get_default_options
 from pyscaffold.api import NO_CONFIG, bootstrap_options, create_project
@@ -224,31 +225,31 @@
     assert new_opts["name"] == "my-proj"
     assert new_opts["package"] == "my_proj"
     assert new_opts["license"] == "MPL-2.0"
     assert str(new_opts["project_path"]) == "another"
     assert all(k in new_opts for k in "author email url".split())
 
 
+DEFAULT_CONFIG = """\
+[metadata]
+author = John Doe
+author-email = john.joe@gmail.com
+
+[pyscaffold]
+extensions =
+    namespace
+    cirrus
+namespace = my_namespace.my_sub_namespace
+"""
+
+
 @pytest.fixture
 def with_default_config(fake_config_dir):
-    config = dedent(
-        """\
-        [metadata]
-        author = John Doe
-        author-email = john.joe@gmail.com
-
-        [pyscaffold]
-        extensions =
-            namespace
-            cirrus
-        namespace = my_namespace.my_sub_namespace
-        """
-    )
     cfg = fake_config_dir / info.CONFIG_FILE
-    cfg.write_text(config)
+    cfg.write_text(DEFAULT_CONFIG)
 
     yield cfg
 
 
 def test_bootstrap_with_default_config(tmpfolder, with_default_config):
     # Given a default config file exists and contains stuff
     _ = with_default_config
@@ -277,14 +278,51 @@
     assert new_opts.get("namespace") != "my_namespace.my_sub_namespace"
     extensions = new_opts.get("extensions", [])
     assert len(extensions) != 2
     extensions_names = sorted(e.name for e in extensions)
     assert " ".join(extensions_names) != "cirrus namespace"
 
 
+@pytest.fixture
+def macos_config_dir(tmp_path, monkeypatch, fake_config_dir):
+    with TemporaryDirectory(prefix="config", dir=str(tmp_path)) as tmp:
+        confdir = Path(tmp, "Library/Application Support/pyscaffold")
+
+    _ = fake_config_dir  # included for reproducible ordering of fixture evaluation
+    monkeypatch.setattr("pyscaffold.info.config_dir", lambda *_, **__: confdir)
+    yield confdir
+
+
+def test_bootstrap_with_legacy_macos_default_config(
+    monkeypatch, tmpfolder, macos_config_dir
+):
+    monkeypatch.setattr("sys.platform", "darwin_test")  # pretend to be on macOS
+    # Given a default config file in an outdated config dir on macOS
+    # (see platformdirs v3.0.0)
+    new_dir = macos_config_dir
+    assert not new_dir.exists()  # sanity check
+    old_dir = info._old_macos_config_dir(new_dir)
+    old_dir.mkdir(parents=True, exist_ok=False)
+    (old_dir / "default.cfg").write_text(DEFAULT_CONFIG)
+    # when bootstrapping options
+    opts = dict(project_path="xoxo")
+    new_opts = bootstrap_options(opts)
+    # the old directory will be moved to the new location
+    assert new_dir.exists()
+    assert not old_dir.exists()
+    # and the stuff in the old config will be considered
+    assert new_opts["author"] == "John Doe"
+    assert new_opts["email"] == "john.joe@gmail.com"
+    assert new_opts["namespace"] == "my_namespace.my_sub_namespace"
+    extensions = new_opts["extensions"]
+    assert len(extensions) == 2
+    extensions_names = sorted(e.name for e in extensions)
+    assert " ".join(extensions_names) == "cirrus namespace"
+
+
 def test_create_project_with_default_config(tmpfolder, with_default_config):
     # Given a default config file exists and contains stuff
     _ = with_default_config
     project = Path(str(tmpfolder)) / "xoxo"
     # when a new project is created
     create_project(project_path="xoxo", name="project")
     # then the default config is considered
```

### Comparing `PyScaffold-4.4.1/tests/test_cli.py` & `PyScaffold-4.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_dependencies.py` & `PyScaffold-4.5/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_examples.py` & `PyScaffold-4.5/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_exceptions.py` & `PyScaffold-4.5/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_extensions.py` & `PyScaffold-4.5/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_file_system.py` & `PyScaffold-4.5/tests/test_file_system.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_identification.py` & `PyScaffold-4.5/tests/test_identification.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_info.py` & `PyScaffold-4.5/tests/test_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     assert info.is_git_installed()
 
 
 def test_git_is_wrongely_installed(nogit_mock):
     assert not info.is_git_installed()
 
 
-def test_git_is_not_installed(nonegit_mock):
+def test_git_is_not_installed(nogit_cmd_mock):
     assert not info.is_git_installed()
 
 
 def test_is_git_configured(git_mock):
     assert info.is_git_configured()
 
 
@@ -72,15 +72,15 @@
     assert info.is_git_configured()
 
 
 def test_is_git_not_configured(noconfgit_mock):
     assert not info.is_git_configured()
 
 
-def test_check_git_not_installed(nonegit_mock):
+def test_check_git_not_installed(nogit_cmd_mock):
     with pytest.raises(exceptions.GitNotInstalled):
         info.check_git()
 
 
 def test_check_git_not_configured(noconfgit_mock):
     with pytest.raises(exceptions.GitNotConfigured):
         info.check_git()
```

### Comparing `PyScaffold-4.4.1/tests/test_install.py` & `PyScaffold-4.5/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_log.py` & `PyScaffold-4.5/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_operations.py` & `PyScaffold-4.5/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_repo.py` & `PyScaffold-4.5/tests/test_repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,19 +129,7 @@
         "my_file": "Some other content",
         "my_dir": {"my_file": "Some more content"},
     }
     structure.create_structure(struct, {"project_path": project})
     with chdir(project):
         git_root = repo.get_git_root(default=".")
     assert git_root == "."
-
-
-def test_get_git_root_with_nonegit(tmpfolder, nonegit_mock):
-    project = "my_project"
-    struct = {
-        "my_file": "Some other content",
-        "my_dir": {"my_file": "Some more content"},
-    }
-    structure.create_structure(struct, {"project_path": project})
-    with chdir(project):
-        git_root = repo.get_git_root(default=".")
-    assert git_root == "."
```

### Comparing `PyScaffold-4.4.1/tests/test_shell.py` & `PyScaffold-4.5/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_structure.py` & `PyScaffold-4.5/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_templates.py` & `PyScaffold-4.5/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_termui.py` & `PyScaffold-4.5/tests/test_termui.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_toml.py` & `PyScaffold-4.5/tests/test_toml.py`

 * *Files identical despite different names*

### Comparing `PyScaffold-4.4.1/tests/test_update.py` & `PyScaffold-4.5/tests/test_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 import logging
 import os
 import re
+import subprocess
+import sys
 from configparser import ConfigParser
 from pathlib import Path
 from textwrap import dedent
 from types import SimpleNamespace as Object
 
 import pytest
 from packaging.version import Version
 
 from pyscaffold import __path__ as pyscaffold_paths
 from pyscaffold import __version__, actions, info, update
 from pyscaffold.file_system import chdir
 
 from .helpers import in_ci, path_as_uri, skip_on_conda_build
+from .system.helpers import normalize_run_args
 
 EDITABLE_PYSCAFFOLD = re.compile(r"^-e.+pyscaffold.*$", re.M | re.I)
 
 
 class VenvManager:
-    def __init__(self, tmpdir, venv, pytestconfig):
-        self.tmpdir = str(tmpdir)  # convert Path to str
+    def __init__(self, venv):
         self.installed = False
         self.venv = venv
-        self.venv_path = str(venv.virtualenv)
-        self.pytestconfig = pytestconfig
-        self.install("coverage")
         self.running_version = Version(__version__)
+        self._orig_workdir = Path(".").resolve()
 
     def install(self, pkg=None, editable=False, **kwargs):
-        pkg = f'"{pkg}"'  # Windows requires double quotes to work properly with ranges
+        target = [str(pkg)]
         if editable:
-            pkg = f"--editable {pkg}"
+            target = ["--editable", *target]
 
-        python = self.venv.python
-        assert Path(python).exists()
+        assert Path(self.venv.exe("python")).exists()
+        assert str(self.venv.path) in str(self.venv.exe("python"))
 
         # Sometimes Windows complain about SSL, despite all the efforts on using a env
         # var for trusted hosts
-        return self.run(
-            f"{python} -m pip install {pkg} --trusted-host pypi.python.org "
-            "--trusted-host files.pythonhosted.org --trusted-host pypi.org",
-            **kwargs,
-        )
+        cmd = [
+            *("pip", "install", *target),
+            *("--trusted-host", "files.pythonhosted.org"),
+            *("--trusted-host", "pypi.python.org"),
+            *("--trusted-host", "files.pythonhosted.org"),
+            *("--trusted-host", "pypi.org"),
+        ]
+        return self.run(*cmd, **kwargs)
 
     def _get_proj_dir(self) -> Path:
         if "TOXINIDIR" in os.environ:
             # so pytest runs within tox
             proj_dir = Path(os.environ["TOXINIDIR"])
             logging.debug("SRC via TOXINIDIR: %s", proj_dir)
         else:
@@ -69,15 +72,15 @@
         assert wheel, "PyScaffold should be pre-built by CI, but it is not..."
         return self.install(path_as_uri(wheel))
 
     def _install_from_src(self, proj_dir: Path):
         env = {**os.environ, "SETUPTOOLS_SCM_PRETEND_VERSION": __version__}
         assert proj_dir.exists(), f"{proj_dir} is supposed to exist"
         out = self.install(proj_dir, editable=True, env=env)
-        pkg_list = self.run(f"{self.venv.python} -m pip freeze")
+        pkg_list = self.run("pip freeze")
         assert EDITABLE_PYSCAFFOLD.findall(pkg_list)
         return out
 
     def install_this_pyscaffold(self):
         # Normally the following command should do the trick
         # self.venv.install_package('PyScaffold')
         # but sadly pytest-virtualenv chokes on the src-layout of PyScaffold
@@ -91,130 +94,117 @@
         assert self.running_version.public <= self.pyscaffold_version().public
         self.installed = True
         return self
 
     def install_pyscaffold(self, major, minor):
         ver = f"pyscaffold>={major}.{minor},<{major}.{minor + 1}a0"
         self.install(ver)
-        installed_version = self.pyscaffold_version()._version.release[:2]
+        installed_version = self.pyscaffold_version().release[:2]
         assert installed_version == (major, minor)
         self.installed = True
         return self
 
     def uninstall_pyscaffold(self):
-        self.run(f"{self.venv.python} -m pip uninstall -y pyscaffold")
-        assert "PyScaffold" not in self.venv.installed_packages().keys()
+        self.run("pip uninstall -y pyscaffold")
+        putup = self.venv.exe("putup")
+        assert str(self.venv.path.resolve()) not in str(Path(putup).resolve())
         self.installed = False
         return self
 
     def pyscaffold_version(self):
-        version = self.venv.installed_packages().get("PyScaffold", None)
-        if version:
-            return Version(version.version)
-        else:
-            return None
-
-    def putup(self, *args, with_coverage=False, **kwargs):
-        if with_coverage:
-            # need to pass here as list since its args to coverage.py
-            args = [subarg for arg in args for subarg in arg.split()]
-            putup_path = Path(self.venv_path, "bin", "putup")
-            cmd = list(map(str, [putup_path] + args))
-        else:
-            # need to pass here as string since it's the cmd itself
-            cmd = " ".join(["putup"] + list(map(str, args)))
-        self.run(cmd, with_coverage=with_coverage, **kwargs)
+        try:
+            cli_version = self.run("python -m pyscaffold.cli --version").lower()
+            return Version(cli_version.replace("pyscaffold ", ""))
+        except subprocess.CalledProcessError as ex:
+            if (
+                sys.version_info >= (3, 12)
+                and "No module named 'pyscaffold.contrib.six.moves'" in ex.output
+            ):
+                pytest.skip("Cannot import from six.moves in Python >= 3.12")
+            raise
+
+    def putup(self, *args, **kwargs):
+        args, kwargs = normalize_run_args(args, kwargs)
+        print("putup", *args)
+        print(self.venv.run("putup", *args, **kwargs))
         return self
 
-    def run(self, cmd, with_coverage=False, **kwargs):
-        if with_coverage:
-            kwargs.setdefault("pytestconfig", self.pytestconfig)
-            # change to directory where .coverage needs to be created
-            kwargs.setdefault("cd", os.getcwd())
-            return self.venv.run_with_coverage(cmd, **kwargs).strip()
-        else:
-            with chdir(self.tmpdir):
-                kwargs.setdefault("cwd", self.tmpdir)
-                return self.venv.run(cmd, capture=True, **kwargs).strip()
-
-    def get_file(self, path):
-        with chdir(self.tmpdir):
-            return Path(path).read_text()
+    def run(self, *args, **kwargs):
+        return self.venv.run(*args, **kwargs)
 
 
 @pytest.fixture
-def venv_mgr(tmpdir, venv, pytestconfig):
-    return VenvManager(tmpdir, venv, pytestconfig)
+def venv_mgr(venv):
+    return VenvManager(venv)
 
 
 @pytest.mark.slow
 @pytest.mark.requires_src
 @skip_on_conda_build
-def test_update_version_3_0_to_3_1(with_coverage, venv_mgr):
-    project = Path(venv_mgr.venv_path, "my_old_project")
-    (
-        venv_mgr.install_pyscaffold(3, 0)
-        .putup(project)
-        .uninstall_pyscaffold()
-        .install_this_pyscaffold()
-        .putup(f"--update {project}", with_coverage=with_coverage)
-    )
-    setup_cfg = venv_mgr.get_file(Path(project, "setup.cfg"))
+def test_update_version_3_0_to_3_1(tmp_path, with_coverage, venv_mgr):
+    with chdir(str(tmp_path)):
+        name = "my_old_project"
+        project = tmp_path / "my_old_project"
+        (
+            venv_mgr.install_pyscaffold(3, 0)
+            .putup(name)
+            .uninstall_pyscaffold()
+            .install_this_pyscaffold()
+            .putup(f"--update {project}", with_coverage=with_coverage)
+        )
+    setup_cfg = Path(project, "setup.cfg").read_text(encoding="utf-8")
     assert "[options.entry_points]" in setup_cfg
 
 
 @pytest.mark.slow
 @pytest.mark.requires_src
 @skip_on_conda_build
-def test_update_version_3_0_to_3_1_pretend(with_coverage, venv_mgr):
-    project = Path(venv_mgr.venv_path, "my_old_project")
-    (
-        venv_mgr.install_pyscaffold(3, 0)
-        .putup(project)
-        .uninstall_pyscaffold()
-        .install_this_pyscaffold()
-        .putup(f"--pretend --update {project}", with_coverage=with_coverage)
-    )
-    setup_cfg = venv_mgr.get_file(Path(project, "setup.cfg"))
+def test_update_version_3_0_to_3_1_pretend(tmp_path, with_coverage, venv_mgr):
+    with chdir(str(tmp_path)):
+        name = "my_old_project"
+        project = tmp_path / "my_old_project"
+        (
+            venv_mgr.install_pyscaffold(3, 0)
+            .putup(name)
+            .uninstall_pyscaffold()
+            .install_this_pyscaffold()
+            .putup(f"--pretend --update {project}", with_coverage=with_coverage)
+        )
+    setup_cfg = Path(project, "setup.cfg").read_text(encoding="utf-8")
     assert "[options.entry_points]" not in setup_cfg
 
 
 @pytest.mark.slow
 @pytest.mark.requires_src
 @skip_on_conda_build
-def test_inplace_update(with_coverage, venv_mgr):
+def test_inplace_update(tmp_path, with_coverage, venv_mgr):
     # Given an existing project
-    project = Path(venv_mgr.tmpdir) / "my-ns-proj"
-    (
-        venv_mgr.install_this_pyscaffold().putup(
-            f"--package project --namespace my_ns {project}"
-        )
-    )
+    project = tmp_path / "my_old_project"
+    cmd = f"--name my-ns-proj --package project --namespace my_ns {project}"
+    venv_mgr.install_this_pyscaffold().putup(cmd)
 
     # With an existing configuration
+    assert project / "setup.cfg"
     parser = ConfigParser()
     parser.read(project / "setup.cfg")
     assert parser["metadata"]["name"] == "my-ns-proj"
     assert parser["pyscaffold"]["package"] == "project"
     assert parser["pyscaffold"]["namespace"] == "my_ns"
 
     # And without some extensions
     for file in (".pre-commit-config.yaml", ".isort.cfg"):
         assert not Path(project, file).exists()
 
     # When the project is updated
     # without repeating the information already given
     # but adding some information/extensions
     with chdir(str(project)):
-        (
-            venv_mgr.putup(
-                "-vv --description asdf --pre-commit --update .",
-                with_coverage=with_coverage,
-                cwd=str(project),
-            )
+        venv_mgr.putup(
+            "-vv --description asdf --pre-commit --update .",
+            with_coverage=with_coverage,
         )
 
     # Then existing configuration should be preserved + the additions
     parser = ConfigParser()
     parser.read(project / "setup.cfg")
     assert parser["metadata"]["name"] == "my-ns-proj"
     assert parser["pyscaffold"]["package"] == "project"
```

### Comparing `PyScaffold-4.4.1/tox.ini` & `PyScaffold-4.5/tox.ini`

 * *Files identical despite different names*

