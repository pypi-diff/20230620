# Comparing `tmp/ddev-2.1.0.tar.gz` & `tmp/ddev-3.0.0.tar.gz`

## Comparing `ddev-2.1.0.tar` & `ddev-3.0.0.tar`

### file list

```diff
@@ -1,94 +1,111 @@
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 ddev-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/__about__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/py.typed
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/__init__.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/application.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/terminal.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/ci/__init__.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/config/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/docs/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/env/__init__.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/meta/__init__.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/meta/scripts/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/release/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/release/agent/__init__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/release/show/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/release/stats/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/status/__init__.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/validate/__init__.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/validate/ci.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/validate/manifest.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/cli/validate/openmetrics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/config/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/config/constants.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/config/file.py
--rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/config/model.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/config/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/integration/__init__.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/integration/core.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/integration/manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/api.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/specs.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/external/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/external/starship/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/external/starship/__main__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/plugin/external/starship/prompt.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/repo/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/repo/config.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/repo/constants.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/repo/core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/ci.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/fs.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/git.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/json.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/network.py
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/platform.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/structures.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/toml.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/scripts/__init__.py
--rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/utils/scripts/ci_matrix.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/validation/__init__.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-2.1.0/src/ddev/validation/tracker.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/conftest.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/test__utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/test_edit.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/test_explore.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/test_find.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/test_restore.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/test_set.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/config/test_show.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/status/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/status/test_status.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/validate/__init__.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/validate/test_manifest.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/cli/validate/test_openmetrics.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/config/__init__.py
--rw-r--r--   0        0        0    40933 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/config/test_model.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/helpers/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/helpers/api.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/integration/test_core.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/integration/test_manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/repo/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/repo/test_config.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/repo/test_core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/utils/test_fs.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/utils/test_git.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/utils/test_json.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/utils/test_platform.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/utils/test_structures.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/validation/__init__.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ddev-2.1.0/tests/validation/test_tracker.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 ddev-2.1.0/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-2.1.0/README.md
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 ddev-2.1.0/hatch.toml
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 ddev-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 ddev-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 ddev-3.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 ddev-3.0.0/pyoxidizer.bzl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/py.typed
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/__init__.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/application.py
+-rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/terminal.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/ci/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/clean/__init__.py
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/config/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/docs/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/env/__init__.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/meta/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/meta/scripts/__init__.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/meta/scripts/upgrade_python.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/release/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/release/agent/__init__.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/release/list_versions/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/release/show/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/release/stats/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/status/__init__.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/validate/__init__.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/validate/ci.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/validate/licenses.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/validate/manifest.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/validate/openmetrics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/config/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/config/constants.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/config/file.py
+-rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/config/model.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/config/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/integration/__init__.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/integration/core.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/integration/manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/api.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/specs.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/external/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/external/starship/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/external/starship/__main__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/external/starship/prompt.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/repo/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/repo/config.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/repo/constants.py
+-rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/repo/core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/ci.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/fs.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/git.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/json.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/network.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/platform.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/structures.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/toml.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/scripts/__init__.py
+-rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/scripts/ci_matrix.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/validation/__init__.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/validation/tracker.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     5865 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/test__utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/clean/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/clean/test_clean.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/__init__.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/test_edit.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/test_explore.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/test_find.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/test_restore.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/test_set.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/test_show.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/meta/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/meta/scripts/__init__.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/meta/scripts/test_upgrade_python.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/release/__init__.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/release/test_list_versions.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/status/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/status/test_status.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/validate/__init__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/validate/test_licenses.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/validate/test_manifest.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/validate/test_openmetrics.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/config/__init__.py
+-rw-r--r--   0        0        0    40933 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/config/test_model.py
+-rw-r--r--   0        0        0    23688 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/fixtures/network/list_versions/success_disk.yaml
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/fixtures/network/manifest/missing_app_uuid.yaml
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/fixtures/network/manifest/success.yaml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/helpers/api.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/integration/test_core.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/integration/test_manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/repo/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/repo/test_config.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/repo/test_core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/utils/test_fs.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/utils/test_json.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/utils/test_platform.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/utils/test_structures.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/validation/__init__.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/validation/test_tracker.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 ddev-3.0.0/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-3.0.0/README.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ddev-3.0.0/hatch.toml
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 ddev-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 ddev-3.0.0/PKG-INFO
```

### Comparing `ddev-2.1.0/CHANGELOG.md` & `ddev-3.0.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # CHANGELOG - ddev
 
+## 3.0.0 / 2023-06-20
+
+* [Added] Bump the minimum version of datadog-checks-dev. See [#14785](https://github.com/DataDog/integrations-core/pull/14785).
+* [Added] Upgrade Pydantic model code generator. See [#14779](https://github.com/DataDog/integrations-core/pull/14779).
+* [Added] Use Git for versioning. See [#14778](https://github.com/DataDog/integrations-core/pull/14778).
+* [Added] Add validations for removed dependencies. See [#14556](https://github.com/DataDog/integrations-core/pull/14556).
+* [Added] Migrate `clean` command. See [#14726](https://github.com/DataDog/integrations-core/pull/14726).
+* [Added] Add `release list` command to list integration version releases. See [#14687](https://github.com/DataDog/integrations-core/pull/14687).
+* [Added] Migrate command to upgrade Python. See [#14700](https://github.com/DataDog/integrations-core/pull/14700).
+* [Fixed] Bump python version from py3.8 to py3.9. See [#14701](https://github.com/DataDog/integrations-core/pull/14701).
+* [Changed] Remove `pyperclip` dependency and clipboard functionality. See [#14782](https://github.com/DataDog/integrations-core/pull/14782).
+
 ## 2.1.0 / 2023-05-26
 
 * [Added] Add validation for metric limit. See [#14528](https://github.com/DataDog/integrations-core/pull/14528).
 * [Fixed] Consider changes to `metadata.csv` as testable. See [#14429](https://github.com/DataDog/integrations-core/pull/14429).
 * [Fixed] Account for dependency upgrades in CI matrix logic. See [#14366](https://github.com/DataDog/integrations-core/pull/14366).
 * [Fixed] Fix edge case in CI matrix construction. See [#14355](https://github.com/DataDog/integrations-core/pull/14355).
```

### Comparing `ddev-2.1.0/src/ddev/cli/__init__.py` & `ddev-3.0.0/src/ddev/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import os
 
 import click
 import pluggy
-from datadog_checks.dev.tooling.commands.clean import clean
 from datadog_checks.dev.tooling.commands.create import create
 from datadog_checks.dev.tooling.commands.dep import dep
 from datadog_checks.dev.tooling.commands.run import run
 from datadog_checks.dev.tooling.commands.test import test
 
-from ddev.__about__ import __version__
+from ddev._version import __version__
 from ddev.cli.application import Application
 from ddev.cli.ci import ci
+from ddev.cli.clean import clean
 from ddev.cli.config import config
 from ddev.cli.docs import docs
 from ddev.cli.env import env
 from ddev.cli.meta import meta
 from ddev.cli.release import release
 from ddev.cli.status import status
 from ddev.cli.validate import validate
@@ -140,22 +140,26 @@
 ddev.add_command(meta)
 ddev.add_command(release)
 ddev.add_command(run)
 ddev.add_command(status)
 ddev.add_command(test)
 ddev.add_command(validate)
 
+__management_command = os.environ.get('PYAPP_COMMAND_NAME', '')
+if __management_command:
+    ddev.add_command(click.Command(name=__management_command, help='Manage this application'))
+
 
 def main():  # no cov
     manager = pluggy.PluginManager('ddev')
     manager.add_hookspecs(specs)
     manager.load_setuptools_entrypoints('ddev')
     manager.hook.register_commands()
 
     try:
-        return ddev(windows_expand_args=False)
+        return ddev(prog_name='ddev', windows_expand_args=False)
     except Exception:
         from rich.console import Console
 
         console = Console()
         console.print_exception(suppress=[click])
         return 1
```

### Comparing `ddev-2.1.0/src/ddev/cli/application.py` & `ddev-3.0.0/src/ddev/cli/application.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/cli/terminal.py` & `ddev-3.0.0/src/ddev/cli/terminal.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/cli/config/__init__.py` & `ddev-3.0.0/src/ddev/cli/config/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,27 +22,18 @@
 @click.pass_obj
 def explore(app):
     """Open the config location in your file manager."""
     click.launch(str(app.config_file.path), locate=True)
 
 
 @config.command(short_help='Show the location of the config file')
-@click.option('--copy', '-c', is_flag=True, help='Copy the path to the config file to the clipboard')
 @click.pass_obj
-def find(app, copy):
+def find(app):
     """Show the location of the config file."""
-    config_path = str(app.config_file.path)
-    if copy:
-        import pyperclip
-
-        pyperclip.copy(config_path)
-    elif ' ' in config_path:
-        app.display(f'"{config_path}"')
-    else:
-        app.display(config_path)
+    app.display(str(app.config_file.path))
 
 
 @config.command(short_help='Show the contents of the config file')
 @click.option('--all', '-a', 'all_keys', is_flag=True, help='Do not scrub secret fields')
 @click.pass_obj
 def show(app, all_keys):
     """Show the contents of the config file."""
```

### Comparing `ddev-2.1.0/src/ddev/cli/env/__init__.py` & `ddev-3.0.0/src/ddev/cli/env/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/cli/meta/__init__.py` & `ddev-3.0.0/src/ddev/cli/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/cli/meta/scripts/__init__.py` & `ddev-3.0.0/src/ddev/cli/meta/scripts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import click
 from datadog_checks.dev.tooling.commands.meta.scripts.github_user import email2ghuser
 from datadog_checks.dev.tooling.commands.meta.scripts.metrics2md import metrics2md
 from datadog_checks.dev.tooling.commands.meta.scripts.remove_labels import remove_labels
-from datadog_checks.dev.tooling.commands.meta.scripts.upgrade_python import upgrade_python
+
+from ddev.cli.meta.scripts.upgrade_python import upgrade_python
 
 
 @click.group(short_help='Miscellaneous scripts that may be useful')
 def scripts():
     """
     Miscellaneous scripts that may be useful.
     """
```

### Comparing `ddev-2.1.0/src/ddev/cli/release/__init__.py` & `ddev-3.0.0/src/ddev/cli/release/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 from datadog_checks.dev.tooling.commands.release.changelog import changelog
 from datadog_checks.dev.tooling.commands.release.make import make
 from datadog_checks.dev.tooling.commands.release.tag import tag
 from datadog_checks.dev.tooling.commands.release.trello import trello
 from datadog_checks.dev.tooling.commands.release.upload import upload
 
 from ddev.cli.release.agent import agent
+from ddev.cli.release.list_versions import list_versions
 from ddev.cli.release.show import show
 from ddev.cli.release.stats import stats
 
 
 @click.group(short_help='Manage the release of integrations')
 def release():
     """
     Manage the release of integrations.
     """
 
 
 release.add_command(agent)
 release.add_command(build)
 release.add_command(changelog)
+release.add_command(list_versions)
 release.add_command(make)
 release.add_command(show)
 release.add_command(stats)
 release.add_command(tag)
 release.add_command(trello)
 release.add_command(upload)
```

### Comparing `ddev-2.1.0/src/ddev/cli/release/agent/__init__.py` & `ddev-3.0.0/src/ddev/cli/release/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/cli/release/show/__init__.py` & `ddev-3.0.0/src/ddev/cli/release/show/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/cli/status/__init__.py` & `ddev-3.0.0/src/ddev/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/cli/validate/__init__.py` & `ddev-3.0.0/src/ddev/cli/validate/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 from datadog_checks.dev.tooling.commands.validate.dep import dep
 from datadog_checks.dev.tooling.commands.validate.eula import eula
 from datadog_checks.dev.tooling.commands.validate.http import http
 from datadog_checks.dev.tooling.commands.validate.imports import imports
 from datadog_checks.dev.tooling.commands.validate.integration_style import integration_style
 from datadog_checks.dev.tooling.commands.validate.jmx_metrics import jmx_metrics
 from datadog_checks.dev.tooling.commands.validate.license_headers import license_headers
-from datadog_checks.dev.tooling.commands.validate.licenses import licenses
 from datadog_checks.dev.tooling.commands.validate.metadata import metadata
 from datadog_checks.dev.tooling.commands.validate.models import models
 from datadog_checks.dev.tooling.commands.validate.package import package
 from datadog_checks.dev.tooling.commands.validate.readmes import readmes
 from datadog_checks.dev.tooling.commands.validate.recommended_monitors import recommended_monitors
 from datadog_checks.dev.tooling.commands.validate.saved_views import saved_views
 from datadog_checks.dev.tooling.commands.validate.service_checks import service_checks
 from datadog_checks.dev.tooling.commands.validate.typos import typos
 
 from ddev.cli.validate.ci import ci
+from ddev.cli.validate.licenses import licenses
 from ddev.cli.validate.manifest import manifest
 from ddev.cli.validate.openmetrics import openmetrics
 
 
 @click.group(short_help='Verify certain aspects of the repo')
 def validate():
     """
```

### Comparing `ddev-2.1.0/src/ddev/cli/validate/ci.py` & `ddev-3.0.0/src/ddev/cli/validate/ci.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/cli/validate/manifest.py` & `ddev-3.0.0/src/ddev/cli/validate/manifest.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/cli/validate/openmetrics.py` & `ddev-3.0.0/src/ddev/cli/validate/openmetrics.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/config/file.py` & `ddev-3.0.0/src/ddev/config/file.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/config/model.py` & `ddev-3.0.0/src/ddev/config/model.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/config/utils.py` & `ddev-3.0.0/src/ddev/config/utils.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/integration/core.py` & `ddev-3.0.0/src/ddev/integration/core.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/repo/core.py` & `ddev-3.0.0/src/ddev/repo/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,18 @@
 
     @cached_property
     def config(self) -> RepositoryConfig:
         from ddev.repo.config import RepositoryConfig
 
         return RepositoryConfig(self.path / CONFIG_DIRECTORY / 'config.toml')
 
+    @cached_property
+    def agent_requirements(self) -> Path:
+        return self.path / 'datadog_checks_base' / 'datadog_checks' / 'base' / 'data' / 'agent_requirements.in'
+
 
 class IntegrationRegistry:
     def __init__(self, repo: Repository):
         self.__repo = repo
         self.__cache: Dict[str, Integration] = {}
 
     @property
```

### Comparing `ddev-2.1.0/src/ddev/utils/fs.py` & `ddev-3.0.0/src/ddev/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/utils/git.py` & `ddev-3.0.0/src/ddev/utils/git.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/utils/json.py` & `ddev-3.0.0/src/ddev/utils/json.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/utils/platform.py` & `ddev-3.0.0/src/ddev/utils/platform.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/utils/structures.py` & `ddev-3.0.0/src/ddev/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/utils/scripts/ci_matrix.py` & `ddev-3.0.0/src/ddev/utils/scripts/ci_matrix.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/src/ddev/validation/tracker.py` & `ddev-3.0.0/src/ddev/validation/tracker.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/conftest.py` & `ddev-3.0.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,16 +80,14 @@
 def valid_integration(valid_integrations) -> str:
     return random.choice(valid_integrations)
 
 
 @pytest.fixture(autouse=True)
 def config_file(tmp_path, monkeypatch) -> ConfigFile:
     for env_var in (
-        'DD_GITHUB_USER',
-        'DD_GITHUB_TOKEN',
         'DD_SITE',
         'DD_LOGS_CONFIG_DD_URL',
         'DD_DD_URL',
         'DD_API_KEY',
         'DD_APP_KEY',
     ):
         monkeypatch.delenv(env_var, raising=False)
@@ -142,18 +140,23 @@
     finally:
         set_root('')
         local_clone.reset_branch()
 
 
 @pytest.fixture
 def network_replay(local_repo):
+    """
+    To use, run once without record_mode='none' as an argument and then add it in for subsequent runs.
+    """
     stack = ExitStack()
 
     def add_cassette(relative_path, *args, **kwargs):
-        cassette = vcr.use_cassette(str(local_repo / relative_path), *args, **kwargs)
+        cassette = vcr.use_cassette(
+            str(local_repo / "ddev" / "tests" / "fixtures" / "network" / relative_path), *args, **kwargs
+        )
         stack.enter_context(cassette)
         return cassette
 
     with stack:
         yield add_cassette
```

### Comparing `ddev-2.1.0/tests/test__utils.py` & `ddev-3.0.0/tests/test__utils.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/cli/config/test_find.py` & `ddev-3.0.0/tests/cli/config/test_restore.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
-import os
-
-import pytest
-from ddev.config.constants import ConfigEnvVars
-
+def test_standard(ddev, config_file):
+    config_file.model.repo = 'marketplace'
+    config_file.save()
 
-def test_copy(ddev, config_file, mocker):
-    mock = mocker.patch('pyperclip.copy')
-    result = ddev('config', 'find', '-c')
+    result = ddev('config', 'restore')
 
     assert result.exit_code == 0, result.output
-    mock.assert_called_once_with(str(config_file.path))
-
+    assert result.output == 'Settings were successfully restored.\n'
 
-def test_pipe_to_editor(ddev, config_file):
-    config_file.path = config_file.path.parent / 'a space' / 'config.toml'
-    config_file.path.ensure_parent_dir_exists()
-    config_file.restore()
-    os.environ[ConfigEnvVars.CONFIG] = str(config_file.path)
+    config_file.load()
+    assert config_file.model.repo.name == 'core'
 
-    result = ddev('config', 'find')
 
-    assert result.exit_code == 0, result.output
-    assert result.output == f'"{str(config_file.path)}"\n'
-
-
-def test_standard(ddev, config_file):
-    config_path = str(config_file.path)
-    if ' ' in config_path:  # no cov
-        pytest.xfail('Path to system temporary directory contains spaces')
+def test_allow_invalid_config(ddev, config_file, helpers):
+    config_file.model.agent = ['foo']
+    config_file.save()
 
-    result = ddev('config', 'find')
+    result = ddev('config', 'restore')
 
     assert result.exit_code == 0, result.output
-    assert result.output == f'{config_path}\n'
+    assert result.output == helpers.dedent(
+        """
+        Settings were successfully restored.
+        """
+    )
```

### Comparing `ddev-2.1.0/tests/cli/config/test_set.py` & `ddev-3.0.0/tests/cli/config/test_set.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/cli/config/test_show.py` & `ddev-3.0.0/tests/cli/config/test_show.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Licensed under a 3-clause BSD style license (see LICENSE)
 import os
 
 
 def test_default_scrubbed(ddev, config_file, helpers):
     config_file.model.orgs['default']['api_key'] = 'foo'
     config_file.model.orgs['default']['app_key'] = 'bar'
+    config_file.model.github = {'user': '', 'token': ''}
     config_file.save()
 
     result = ddev('config', 'show')
 
     sep = os.sep.replace('\\', '\\\\')
 
     assert result.exit_code == 0, result.output
@@ -64,14 +65,15 @@
         """
     )
 
 
 def test_reveal(ddev, config_file, helpers):
     config_file.model.orgs['default']['api_key'] = 'foo'
     config_file.model.orgs['default']['app_key'] = 'bar'
+    config_file.model.github = {'user': '', 'token': ''}
     config_file.save()
 
     result = ddev('config', 'show', '-a')
 
     sep = os.sep.replace('\\', '\\\\')
 
     assert result.exit_code == 0, result.output
```

### Comparing `ddev-2.1.0/tests/cli/status/test_status.py` & `ddev-3.0.0/tests/cli/status/test_status.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/cli/validate/test_manifest.py` & `ddev-3.0.0/tests/cli/validate/test_manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         """
         No `dd_url` has been set for org `default`
         """
     )
 
 
 def test_error_single_integration(ddev, repository, helpers, network_replay):
-    network_replay('fixtures/network/manifest/missing_app_uuid.yaml', record_mode='none')
+    network_replay('manifest/missing_app_uuid.yaml', record_mode='none')
 
     check = 'mongo'
     manifest_file = repository.path / check / 'manifest.json'
     manifest = json.loads(manifest_file.read_text())
     del manifest['app_uuid']
     manifest_file.write_text(json.dumps(manifest))
 
@@ -49,15 +49,15 @@
 
         Errors: 1
         """
     )
 
 
 def test_error_multiple_integrations(ddev, repository, helpers, network_replay):
-    network_replay('fixtures/network/manifest/missing_app_uuid.yaml', record_mode='none')
+    network_replay('manifest/missing_app_uuid.yaml', record_mode='none')
 
     for check in ('mongo', 'vsphere'):
         manifest_file = repository.path / check / 'manifest.json'
         manifest = json.loads(manifest_file.read_text())
         del manifest['app_uuid']
         manifest_file.write_text(json.dumps(manifest))
 
@@ -78,15 +78,15 @@
 
         Errors: 2
         """
     )
 
 
 def test_passing(ddev, repository, helpers, network_replay):
-    network_replay('fixtures/network/manifest/success.yaml', record_mode='none')
+    network_replay('manifest/success.yaml', record_mode='none')
 
     result = ddev('validate', 'manifest', 'postgres')
 
     assert result.exit_code == 0, result.output
     assert helpers.remove_trailing_spaces(result.output) == helpers.dedent(
         """
         Validating manifest.json files for 1 checks ...
```

### Comparing `ddev-2.1.0/tests/cli/validate/test_openmetrics.py` & `ddev-3.0.0/tests/cli/validate/test_openmetrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     "check_name",
     [
         pytest.param("aerospike", id="Aerospike check.py OpenMetricsV2"),
         pytest.param("amazon_msk", id="Amazon MSK amazon_msk.py OpenMetricsV1 and V2"),
     ],
 )
 def test_openmetrics_pass_single_parameter(ddev, repository, check_name, helpers, network_replay):
-    network_replay('fixtures/openmetrics/metric_limit/success.yaml', record_mode='none')
     result = ddev("validate", "openmetrics", check_name)
 
     assert result.exit_code == 0, result.output
 
     assert helpers.remove_trailing_spaces(result.output) == helpers.dedent(
         """
         Validating default metric limit for OpenMetrics integrations ...
@@ -27,15 +26,14 @@
 def test_openmetrics_fail_single_parameter(ddev, helpers, repository, network_replay):
     missing_metric_limit = '''
             class ArangodbCheck(OpenMetricsBaseCheckV2, ConfigMixin):
             __NAMESPACE__ = 'arangodb'
             def __init__(self, name, init_config, instances):
                 super(ArangodbCheck, self).__init__(name, init_config, instances)
         '''
-    network_replay('fixtures/openmetrics/metric_limit/fail.yaml', record_mode='none')
 
     check = "arangodb"
     check_file = repository.path / check / "datadog_checks" / check / "check.py"
 
     with open(check_file, "w") as f:
         f.write(missing_metric_limit)
 
@@ -43,16 +41,14 @@
 
     assert result.exit_code == 1, result.output
 
     assert "Errors: 1" in helpers.remove_trailing_spaces(result.output)
 
 
 def test_openmetrics_skip_openmetrics(ddev, helpers, repository, network_replay):
-    network_replay('fixtures/openmetrics/metric_limit/skip_openmetrics.yaml', record_mode='none')
-
     result = ddev("validate", "openmetrics", "openmetrics")
 
     assert result.exit_code == 0, result.output
 
     assert "Passed" not in helpers.remove_trailing_spaces(result.output)
     assert "Errors" not in helpers.remove_trailing_spaces(result.output)
```

### Comparing `ddev-2.1.0/tests/config/test_model.py` & `ddev-3.0.0/tests/config/test_model.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/helpers/api.py` & `ddev-3.0.0/tests/helpers/api.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/integration/test_core.py` & `ddev-3.0.0/tests/integration/test_core.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/repo/test_core.py` & `ddev-3.0.0/tests/repo/test_core.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/utils/test_fs.py` & `ddev-3.0.0/tests/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/utils/test_git.py` & `ddev-3.0.0/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/utils/test_json.py` & `ddev-3.0.0/tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/utils/test_platform.py` & `ddev-3.0.0/tests/utils/test_platform.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/utils/test_structures.py` & `ddev-3.0.0/tests/utils/test_structures.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/tests/validation/test_tracker.py` & `ddev-3.0.0/tests/validation/test_tracker.py`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/.gitignore` & `ddev-3.0.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -124,7 +124,10 @@
 
 
 ## Kind
 .kube
 
 ## Direnv
 .envrc
+
+# Auto-generated during builds
+/ddev/src/ddev/_version.py
```

### Comparing `ddev-2.1.0/README.md` & `ddev-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ddev-2.1.0/pyproject.toml` & `ddev-3.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 [build-system]
-requires = [
-    "hatchling>=1.5.0",
-]
+requires = ["hatchling>=1.17.1", "hatch-vcs>=0.3.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ddev"
 description = "The Datadog Agent integration developer tool"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = "BSD-3-Clause"
 keywords = [
     "datadog",
     "agent",
     "integration",
 ]
 authors = [
@@ -21,22 +19,21 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
-    "datadog-checks-dev[cli]~=19.0",
+    "datadog-checks-dev[cli]~=20.0",
     "hatch>=1.6.3",
     "httpx",
     "jsonpointer",
-    "pyperclip",
     "rich>=12.5.1",
     "tomli; python_version < '3.11'",
     "tomli-w",
     "tomlkit",
 ]
 dynamic = ["version"]
 
@@ -44,32 +41,37 @@
 ddev = "ddev.cli:main"
 ddev-starship = "ddev.plugin.external.starship.prompt:main"
 
 [project.urls]
 Source = "https://github.com/DataDog/integrations-core"
 
 [tool.hatch.version]
-path = "src/ddev/__about__.py"
+source = "vcs"
+
+[tool.hatch.version.raw-options]
+root = ".."
+version_scheme = "python-simplified-semver"
+local_scheme = "no-local-version"
+parentdir_prefix_version = "ddev-"
+git_describe_command = ["git", "describe", "--dirty", "--tags", "--long", "--match", "ddev-v*"]
+
+[tool.hatch.build.hooks.vcs]
+version-file = "src/ddev/_version.py"
+
+[tool.hatch.build.targets.app]
+scripts = ["ddev"]
 
 [tool.black]
 include = '\.pyi?$'
 line-length = 120
 skip-string-normalization = true
 target-version = ["py38"]
 
 [tool.ruff]
-exclude = [
-    ".eggs",
-    ".tox",
-    "build",
-    "compat.py",
-    "__init__.py",
-    "**/datadog_checks/dev/tooling/templates/*",
-    "**/datadog_checks/*/vendor/*",
-]
+exclude = []
 target-version = "py38"
 line-length = 120
 # Rules were ported over from the legacy flake8 settings for parity
 # All the rules can be found here: https://beta.ruff.rs/docs/rules/
 select = [
   "B",
   "C",
@@ -99,8 +101,8 @@
 known-first-party = ["{template_config['package_name']}"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 #Tests can use assertions and relative imports
-"**/tests/**/*" = ["I252"]
+"**/tests/**/*" = ["I252"]
```

### Comparing `ddev-2.1.0/PKG-INFO` & `ddev-3.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: ddev
-Version: 2.1.0
+Version: 3.0.0
 Summary: The Datadog Agent integration developer tool
 Project-URL: Source, https://github.com/DataDog/integrations-core
 Author-email: Datadog <packages@datadoghq.com>
 License-Expression: BSD-3-Clause
 Keywords: agent,datadog,integration
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Requires-Dist: datadog-checks-dev[cli]~=19.0
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Requires-Dist: datadog-checks-dev[cli]~=20.0
 Requires-Dist: hatch>=1.6.3
 Requires-Dist: httpx
 Requires-Dist: jsonpointer
-Requires-Dist: pyperclip
 Requires-Dist: rich>=12.5.1
 Requires-Dist: tomli-w
 Requires-Dist: tomli; python_version < '3.11'
 Requires-Dist: tomlkit
 Description-Content-Type: text/markdown
 
 # ddev
```

