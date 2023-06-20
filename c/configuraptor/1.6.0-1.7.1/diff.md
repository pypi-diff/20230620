# Comparing `tmp/configuraptor-1.6.0.tar.gz` & `tmp/configuraptor-1.7.1.tar.gz`

## Comparing `configuraptor-1.6.0.tar` & `configuraptor-1.7.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 configuraptor-1.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.6.0/coverage.svg
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.6.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.6.0/_static/configuraptor_circle.png
--rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.6.0/_static/configuraptor_original.jpeg
--rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.6.0/_static/configuraptor_round.png
--rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.6.0/_static/configuraptor_transparent.png
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/ages.toml
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/dataclass.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/dumping.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/dumping.yml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/example_from_readme.json
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/example_from_readme.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/example_from_readme.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/example_from_readme.yaml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/existing_instance.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/main.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/postponed.py
--rw-r--r--   0        0        0     9464 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/readme.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/singleton.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.6.0/examples/typedconfig_class.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_31a2a1dc9b603870___init___py.html
--rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_47560703719c1d9e___about___py.html
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_47560703719c1d9e___init___py.html
--rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_47560703719c1d9e_cls_py.html
--rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_47560703719c1d9e_core_py.html
--rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_47560703719c1d9e_errors_py.html
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_47560703719c1d9e_helpers_py.html
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_47560703719c1d9e_main_py.html
--rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_47560703719c1d9e_singleton_py.html
--rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_6c7dc8b73849fb97___init___py.html
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_6c7dc8b73849fb97__types_py.html
--rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
--rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
--rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html
--rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html
--rw-r--r--   0        0        0    17130 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
--rw-r--r--   0        0        0   131736 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html
--rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_dump_py.html
--rw-r--r--   0        0        0    30314 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
--rw-r--r--   0        0        0    12046 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html
--rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     8038 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.6.0/htmlcov/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.6.0/pytest_examples/empty.toml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.6.0/pytest_examples/example.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.6.0/pytest_examples/example.toml
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.6.0/pytest_examples/example.yaml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.6.0/pytest_examples/some.toml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.6.0/pytest_examples/with_dict_of_custom.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.6.0/pytest_examples/with_multiple_toplevel_keys.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/__about__.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/__init__.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/cls.py
--rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/core.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/dump.py
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/errors.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/helpers.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/postpone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/py.typed
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/singleton.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/loaders/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/loaders/_types.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/loaders/loaders_310.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/loaders/loaders_311.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/loaders/loaders_shared.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.6.0/src/configuraptor/loaders/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/constants.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/test_about.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/test_core.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/test_dumps.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/test_json_yaml.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/test_mypy.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/test_postponed.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/test_singleton.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/test_toml_basic.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/test_toml_dataclass.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/test_toml_existing.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 configuraptor-1.6.0/tests/test_toml_typedconfig_class.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.6.0/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.6.0/LICENSE.txt
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 configuraptor-1.6.0/README.md
--rw-r--r--   0        0        0     4759 2020-02-02 00:00:00.000000 configuraptor-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 configuraptor-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 configuraptor-1.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 configuraptor-1.7.1/coverage.svg
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 configuraptor-1.7.1/.github/workflows/su6.yml
+-rw-r--r--   0        0        0   160051 2020-02-02 00:00:00.000000 configuraptor-1.7.1/_static/configuraptor_circle.png
+-rw-r--r--   0        0        0    35366 2020-02-02 00:00:00.000000 configuraptor-1.7.1/_static/configuraptor_original.jpeg
+-rw-r--r--   0        0        0   187350 2020-02-02 00:00:00.000000 configuraptor-1.7.1/_static/configuraptor_round.png
+-rw-r--r--   0        0        0    61713 2020-02-02 00:00:00.000000 configuraptor-1.7.1/_static/configuraptor_transparent.png
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/ages.toml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/dataclass.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/dumping.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/dumping.yml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/example_from_readme.json
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/example_from_readme.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/example_from_readme.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/example_from_readme.yaml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/existing_instance.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/main.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/postponed.py
+-rw-r--r--   0        0        0     9464 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/readme.md
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/singleton.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 configuraptor-1.7.1/examples/typedconfig_class.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_31a2a1dc9b603870___init___py.html
+-rw-r--r--   0        0        0     9349 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_47560703719c1d9e___about___py.html
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_47560703719c1d9e___init___py.html
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_47560703719c1d9e_cls_py.html
+-rw-r--r--   0        0        0   118124 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_47560703719c1d9e_core_py.html
+-rw-r--r--   0        0        0    19529 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_47560703719c1d9e_errors_py.html
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_47560703719c1d9e_helpers_py.html
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_47560703719c1d9e_main_py.html
+-rw-r--r--   0        0        0    15631 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_47560703719c1d9e_singleton_py.html
+-rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_6c7dc8b73849fb97___init___py.html
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_6c7dc8b73849fb97__types_py.html
+-rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html
+-rw-r--r--   0        0        0     8566 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html
+-rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40___about___py.html
+-rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40___init___py.html
+-rw-r--r--   0        0        0    17130 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_cls_py.html
+-rw-r--r--   0        0        0   131736 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_core_py.html
+-rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_dump_py.html
+-rw-r--r--   0        0        0    30314 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_errors_py.html
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html
+-rw-r--r--   0        0        0    12046 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html
+-rw-r--r--   0        0        0    15643 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     8038 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 configuraptor-1.7.1/htmlcov/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.7.1/pytest_examples/empty.toml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 configuraptor-1.7.1/pytest_examples/example.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 configuraptor-1.7.1/pytest_examples/example.toml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 configuraptor-1.7.1/pytest_examples/example.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 configuraptor-1.7.1/pytest_examples/some.toml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 configuraptor-1.7.1/pytest_examples/with_dict_of_custom.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 configuraptor-1.7.1/pytest_examples/with_multiple_toplevel_keys.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/__about__.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/__init__.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/cls.py
+-rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/core.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/dump.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/errors.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/helpers.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/postpone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/py.typed
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/singleton.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/loaders/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/loaders/_types.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/loaders/loaders_310.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/loaders/loaders_311.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/loaders/loaders_shared.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 configuraptor-1.7.1/src/configuraptor/loaders/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/constants.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/test_about.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/test_core.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/test_dumps.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/test_json_yaml.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/test_mypy.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/test_postponed.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/test_singleton.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/test_toml_basic.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/test_toml_dataclass.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/test_toml_existing.py
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 configuraptor-1.7.1/tests/test_toml_typedconfig_class.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 configuraptor-1.7.1/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 configuraptor-1.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 configuraptor-1.7.1/README.md
+-rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 configuraptor-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 configuraptor-1.7.1/PKG-INFO
```

### Comparing `configuraptor-1.6.0/CHANGELOG.md` & `configuraptor-1.7.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.7.1 (2023-06-20)
+### Fix
+* **310:** Backwards compatible code ([`8f90aec`](https://github.com/trialandsuccess/configuraptor/commit/8f90aec43fd1fcd403f1b68d26e4d605ea346014))
+
+## v1.7.0 (2023-06-20)
+
+
 ## v1.6.0 (2023-06-19)
 ### Feature
 * **TypedConfig:** Added config.update ([`57a21c2`](https://github.com/trialandsuccess/configuraptor/commit/57a21c29cc12185dcc4a406eef3c77d9dbd056d5))
 
 ## v1.5.1 (2023-06-15)
 ### Fix
 * **core:** Patch issue with `is_optional` ([`fd4a897`](https://github.com/trialandsuccess/configuraptor/commit/fd4a8972b847ac69eb012041188420a02880e696))
```

### Comparing `configuraptor-1.6.0/coverage.svg` & `configuraptor-1.7.1/coverage.svg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/_static/configuraptor_circle.png` & `configuraptor-1.7.1/_static/configuraptor_circle.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/_static/configuraptor_original.jpeg` & `configuraptor-1.7.1/_static/configuraptor_original.jpeg`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/_static/configuraptor_round.png` & `configuraptor-1.7.1/_static/configuraptor_round.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/_static/configuraptor_transparent.png` & `configuraptor-1.7.1/_static/configuraptor_transparent.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/examples/dataclass.py` & `configuraptor-1.7.1/examples/dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/examples/dumping.py` & `configuraptor-1.7.1/examples/dumping.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/examples/example_from_readme.py` & `configuraptor-1.7.1/examples/example_from_readme.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/examples/main.py` & `configuraptor-1.7.1/examples/main.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/examples/postponed.py` & `configuraptor-1.7.1/examples/postponed.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/examples/readme.md` & `configuraptor-1.7.1/examples/readme.md`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/examples/singleton.py` & `configuraptor-1.7.1/examples/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/examples/typedconfig_class.py` & `configuraptor-1.7.1/examples/typedconfig_class.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/coverage_html.js` & `configuraptor-1.7.1/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_31a2a1dc9b603870___init___py.html` & `configuraptor-1.7.1/htmlcov/d_31a2a1dc9b603870___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html` & `configuraptor-1.7.1/htmlcov/d_31a2a1dc9b603870_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html` & `configuraptor-1.7.1/htmlcov/d_31a2a1dc9b603870_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_47560703719c1d9e___about___py.html` & `configuraptor-1.7.1/htmlcov/d_47560703719c1d9e___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_47560703719c1d9e___init___py.html` & `configuraptor-1.7.1/htmlcov/d_47560703719c1d9e___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_47560703719c1d9e_cls_py.html` & `configuraptor-1.7.1/htmlcov/d_47560703719c1d9e_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_47560703719c1d9e_core_py.html` & `configuraptor-1.7.1/htmlcov/d_47560703719c1d9e_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_47560703719c1d9e_errors_py.html` & `configuraptor-1.7.1/htmlcov/d_47560703719c1d9e_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_47560703719c1d9e_helpers_py.html` & `configuraptor-1.7.1/htmlcov/d_47560703719c1d9e_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_47560703719c1d9e_main_py.html` & `configuraptor-1.7.1/htmlcov/d_47560703719c1d9e_main_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_47560703719c1d9e_singleton_py.html` & `configuraptor-1.7.1/htmlcov/d_47560703719c1d9e_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_6c7dc8b73849fb97___init___py.html` & `configuraptor-1.7.1/htmlcov/d_6c7dc8b73849fb97___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_6c7dc8b73849fb97__types_py.html` & `configuraptor-1.7.1/htmlcov/d_6c7dc8b73849fb97__types_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html` & `configuraptor-1.7.1/htmlcov/d_6c7dc8b73849fb97_loaders_310_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html` & `configuraptor-1.7.1/htmlcov/d_6c7dc8b73849fb97_loaders_311_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html` & `configuraptor-1.7.1/htmlcov/d_6c7dc8b73849fb97_loaders_shared_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40___about___py.html` & `configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40___about___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40___init___py.html` & `configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40___init___py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_cls_py.html` & `configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_cls_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_core_py.html` & `configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_core_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_dump_py.html` & `configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_dump_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_errors_py.html` & `configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_errors_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html` & `configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_helpers_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html` & `configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_postpone_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html` & `configuraptor-1.7.1/htmlcov/d_eb75b6cf8f5eab40_singleton_py.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/favicon_32.png` & `configuraptor-1.7.1/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/index.html` & `configuraptor-1.7.1/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/keybd_closed.png` & `configuraptor-1.7.1/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/keybd_open.png` & `configuraptor-1.7.1/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/status.json` & `configuraptor-1.7.1/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/htmlcov/style.css` & `configuraptor-1.7.1/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/pytest_examples/some.toml` & `configuraptor-1.7.1/pytest_examples/some.toml`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/src/configuraptor/__init__.py` & `configuraptor-1.7.1/src/configuraptor/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Exposes TypedConfig and load_into for this library.
 """
 
 # SPDX-FileCopyrightText: 2023-present Robin van der Noord <robinvandernoord@gmail.com>
 #
 # SPDX-License-Identifier: MIT
-from .cls import TypedConfig
+from .cls import TypedConfig, update
 from .core import (
     all_annotations,
     check_and_convert_data,
     convert_config,
     ensure_types,
     load_into,
     load_into_class,
@@ -18,14 +18,15 @@
 from .dump import asdict, asjson, astoml, asyaml
 from .postpone import postpone
 from .singleton import Singleton, SingletonMeta
 
 __all__ = [
     # cls
     "TypedConfig",
+    "update",
     # singleton
     "Singleton",
     "SingletonMeta",
     # core
     "all_annotations",
     "check_and_convert_data",
     "convert_config",
```

### Comparing `configuraptor-1.6.0/src/configuraptor/cls.py` & `configuraptor-1.7.1/src/configuraptor/cls.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,30 +22,49 @@
         """
         Load a class' config values from the config file.
 
         SomeClass.load(data, ...) = load_into(SomeClass, data, ...).
         """
         return load_into(cls, data, key=key, init=init, strict=strict)
 
-    def update(self, strict: bool = True, allow_none: bool = False, **values: typing.Any) -> None:
+    def _update(self, _strict: bool = True, _allow_none: bool = False, **values: typing.Any) -> None:
         """
-        Update values on this config.
-
-        Args:
-            strict: allow wrong types?
-            allow_none: allow None or skip those entries?
-            **values: key: value pairs in the right types to update.
-
+        Can be used if .update is overwritten with another value in the config.
         """
         annotations = all_annotations(self.__class__)
 
         for key, value in values.items():
-            if value is None and not allow_none:
+            if value is None and not _allow_none:
                 continue
 
-            if strict and key not in annotations:
+            if _strict and key not in annotations:
                 raise ConfigErrorExtraKey(cls=self.__class__, key=key, value=value)
 
-            if strict and not check_type(value, annotations[key]) and not (value is None and allow_none):
+            if _strict and not check_type(value, annotations[key]) and not (value is None and _allow_none):
                 raise ConfigErrorInvalidType(expected_type=annotations[key], key=key, value=value)
 
             setattr(self, key, value)
+
+    def update(self, _strict: bool = True, _allow_none: bool = False, **values: typing.Any) -> None:
+        """
+        Update values on this config.
+
+        Args:
+            _strict: allow wrong types?
+            _allow_none: allow None or skip those entries?
+            **values: key: value pairs in the right types to update.
+        """
+        return self._update(_strict, _allow_none, **values)
+
+
+# also expose as separate function:
+def update(instance: typing.Any, _strict: bool = True, _allow_none: bool = False, **values: typing.Any) -> None:
+    """
+    Update values on a config.
+
+    Args:
+        instance: config instance to update
+        _strict: allow wrong types?
+        _allow_none: allow None or skip those entries?
+        **values: key: value pairs in the right types to update.
+    """
+    return TypedConfig._update(instance, _strict, _allow_none, **values)
```

### Comparing `configuraptor-1.6.0/src/configuraptor/core.py` & `configuraptor-1.7.1/src/configuraptor/core.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/src/configuraptor/dump.py` & `configuraptor-1.7.1/src/configuraptor/dump.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/src/configuraptor/errors.py` & `configuraptor-1.7.1/src/configuraptor/errors.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/src/configuraptor/postpone.py` & `configuraptor-1.7.1/src/configuraptor/postpone.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
 File contains logic to do with the 'postpone' feature.
 """
 
-import typing
+from typing import Any
+
+from typing_extensions import Never
 
 from .errors import IsPostponedError
 from .singleton import Singleton
 
 
 class Postponed(Singleton):
     """
     Class returned by `postpone` below.
     """
 
-    def __get__(self, instance: type[typing.Any], owner: type[typing.Any]) -> typing.Never:
+    def __get__(self, instance: type[Any], owner: type[Any]) -> Never:
         """
         This magic method is called when a property is accessed.
 
         Example:
              someclass.someprop will trigger the __get__ of `someprop`
 
         Args:
             instance: the class on which the postponed property is defined,
             owner: `SingletonMeta`
         """
         raise IsPostponedError()
 
 
-def postpone() -> typing.Any:
+def postpone() -> Any:
     """
     Can be used to mark a property as postponed, meaning the user will fill it in later (they promose).
 
     If they don't fill it in and still try to use it, they will be met with a IsPostponedError.
     """
     return Postponed()
```

### Comparing `configuraptor-1.6.0/src/configuraptor/singleton.py` & `configuraptor-1.7.1/src/configuraptor/singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/src/configuraptor/loaders/__init__.py` & `configuraptor-1.7.1/src/configuraptor/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/src/configuraptor/loaders/loaders_shared.py` & `configuraptor-1.7.1/src/configuraptor/loaders/loaders_shared.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/tests/test_core.py` & `configuraptor-1.7.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/tests/test_dumps.py` & `configuraptor-1.7.1/tests/test_dumps.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/tests/test_json_yaml.py` & `configuraptor-1.7.1/tests/test_json_yaml.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/tests/test_postponed.py` & `configuraptor-1.7.1/tests/test_postponed.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/tests/test_singleton.py` & `configuraptor-1.7.1/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/tests/test_toml_basic.py` & `configuraptor-1.7.1/tests/test_toml_basic.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/tests/test_toml_dataclass.py` & `configuraptor-1.7.1/tests/test_toml_dataclass.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/tests/test_toml_existing.py` & `configuraptor-1.7.1/tests/test_toml_existing.py`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/tests/test_toml_typedconfig_class.py` & `configuraptor-1.7.1/tests/test_toml_typedconfig_class.py`

 * *Files 10% similar despite different names*

```diff
@@ -114,25 +114,38 @@
     assert first.string != "updated"
     first.update(string="updated")
     assert first.string == "updated"
 
     first.update(string=None)
     assert first.string == "updated"
 
-    first.update(string=None, allow_none=True)
+    first.update(string=None, _allow_none=True)
     assert first.string is None
 
     with pytest.raises(ConfigErrorInvalidType):
         first.update(string=123)
 
-    first.update(string=123, strict=False)
+    first.update(string=123, _strict=False)
     assert first.string == 123
 
     with pytest.raises(ConfigErrorExtraKey):
         try:
             first.update(new_key="some value")
         except ConfigErrorExtraKey as e:
             assert "new_key" in str(e)
             raise e
 
-    first.update(new_key="some value", strict=False)
+    first.update(new_key="some value", _strict=False)
     assert first.new_key == "some value"
+
+class MyConfig(configuraptor.TypedConfig):
+    update: bool = False
+
+def test_typedconfig_update_name_collision():
+    config = MyConfig.load({"update": True}, key="")
+
+    assert config.update == True
+    config._update(update=False)
+    assert config.update == False
+
+    configuraptor.update(config, update=True)
+    assert config.update == True
```

### Comparing `configuraptor-1.6.0/LICENSE.txt` & `configuraptor-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/README.md` & `configuraptor-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `configuraptor-1.6.0/pyproject.toml` & `configuraptor-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 src-layout = true
 
 [tool.setuptools.package-data]
 "configuraptor" = ["py.typed"]
 
 [project.optional-dependencies]
 dev = [
-    "su6[all]",
+    "su6[all]; python_version >= '3.11'",
     "hatch",
     "types-PyYAML",
     "pytest-mypy-testing",
 ]
 
 [project.urls]
 Documentation = "https://github.com/trialandsuccess/configuraptor#readme"
```

### Comparing `configuraptor-1.6.0/PKG-INFO` & `configuraptor-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configuraptor
-Version: 1.6.0
+Version: 1.7.1
 Summary: Load toml/yaml/json config files into classes for a typed config (type hinting etc.)
 Project-URL: Documentation, https://github.com/trialandsuccess/configuraptor#readme
 Project-URL: Issues, https://github.com/trialandsuccess/configuraptor/issues
 Project-URL: Source, https://github.com/trialandsuccess/configuraptor
 Author-email: Robin van der Noord <robin@trialandsuccess.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -18,15 +18,15 @@
 Requires-Python: >=3.10
 Requires-Dist: pyyaml
 Requires-Dist: tomlkit
 Requires-Dist: typeguard
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: pytest-mypy-testing; extra == 'dev'
-Requires-Dist: su6[all]; extra == 'dev'
+Requires-Dist: su6[all]; python_version >= '3.11' and extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img 
         align="center" 
         src="https://raw.githubusercontent.com/trialandsuccess/configuraptor/master/_static/configuraptor_circle.png"
```

