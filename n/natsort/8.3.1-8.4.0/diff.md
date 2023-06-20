# Comparing `tmp/natsort-8.3.1.tar.gz` & `tmp/natsort-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natsort-8.3.1.tar", last modified: Thu Mar  2 05:28:14 2023, max compression
+gzip compressed data, was "natsort-8.4.0.tar", last modified: Tue Jun 20 04:17:11 2023, max compression
```

## Comparing `natsort-8.3.1.tar` & `natsort-8.4.0.tar`

### file list

```diff
@@ -1,71 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 05:28:14.034968 natsort-8.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-03-02 05:28:07.000000 natsort-8.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-02 05:28:07.000000 natsort-8.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-02 05:28:07.000000 natsort-8.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21936 2023-03-02 05:28:14.034968 natsort-8.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20622 2023-03-02 05:28:07.000000 natsort-8.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-02 05:28:07.000000 natsort-8.3.1/RELEASING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 05:28:14.026969 natsort-8.3.1/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-02 05:28:07.000000 natsort-8.3.1/dev/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2318 2023-03-02 05:28:07.000000 natsort-8.3.1/dev/bump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-03-02 05:28:07.000000 natsort-8.3.1/dev/clean.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1299 2023-03-02 05:28:07.000000 natsort-8.3.1/dev/generate_new_unicode_numbers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 05:28:14.026969 natsort-8.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-03-02 05:28:07.000000 natsort-8.3.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-02 05:28:07.000000 natsort-8.3.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-03-02 05:28:07.000000 natsort-8.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-02 05:28:07.000000 natsort-8.3.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-02 05:28:07.000000 natsort-8.3.1/docs/howitworks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-02 05:28:07.000000 natsort-8.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-02 05:28:07.000000 natsort-8.3.1/docs/locale_issues.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-02 05:28:07.000000 natsort-8.3.1/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-02 05:28:07.000000 natsort-8.3.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-02 05:28:07.000000 natsort-8.3.1/docs/shell.rst
--rw-r--r--   0 runner    (1001) docker     (123)    45242 2023-03-02 05:28:07.000000 natsort-8.3.1/docs/special_cases_everywhere.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 05:28:14.026969 natsort-8.3.1/mypy_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-02 05:28:07.000000 natsort-8.3.1/mypy_stubs/icu.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 05:28:14.030969 natsort-8.3.1/natsort/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-02 05:28:07.000000 natsort-8.3.1/natsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-03-02 05:28:07.000000 natsort-8.3.1/natsort/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 05:28:14.030969 natsort-8.3.1/natsort/compat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 05:28:07.000000 natsort-8.3.1/natsort/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-03-02 05:28:07.000000 natsort-8.3.1/natsort/compat/fake_fastnumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-02 05:28:07.000000 natsort-8.3.1/natsort/compat/fastnumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-03-02 05:28:07.000000 natsort-8.3.1/natsort/compat/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)    23768 2023-03-02 05:28:07.000000 natsort-8.3.1/natsort/natsort.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-03-02 05:28:07.000000 natsort-8.3.1/natsort/ns_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 05:28:07.000000 natsort-8.3.1/natsort/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-02 05:28:07.000000 natsort-8.3.1/natsort/unicode_numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23451 2023-03-02 05:28:07.000000 natsort-8.3.1/natsort/unicode_numeric_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)    28267 2023-03-02 05:28:07.000000 natsort-8.3.1/natsort/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 05:28:14.030969 natsort-8.3.1/natsort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21936 2023-03-02 05:28:13.000000 natsort-8.3.1/natsort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-02 05:28:14.000000 natsort-8.3.1/natsort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 05:28:13.000000 natsort-8.3.1/natsort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-02 05:28:13.000000 natsort-8.3.1/natsort.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 05:28:13.000000 natsort-8.3.1/natsort.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-02 05:28:13.000000 natsort-8.3.1/natsort.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-02 05:28:13.000000 natsort-8.3.1/natsort.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-02 05:28:14.034968 natsort-8.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-02 05:28:07.000000 natsort-8.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 05:28:14.034968 natsort-8.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/profile_natsorted.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_fake_fastnumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_final_data_transform_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_input_string_transform_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_natsort_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_natsort_keygen.py
--rw-r--r--   0 runner    (1001) docker     (123)    13565 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_natsorted.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_natsorted_convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_ns_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_os_sorted.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_parse_bytes_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_parse_number_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_parse_string_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_string_component_transform_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_unicode_numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-03-02 05:28:07.000000 natsort-8.3.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-03-02 05:28:07.000000 natsort-8.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:11.389888 natsort-8.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    27638 2023-06-20 04:17:05.000000 natsort-8.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-20 04:17:05.000000 natsort-8.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-20 04:17:05.000000 natsort-8.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21827 2023-06-20 04:17:11.389888 natsort-8.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20513 2023-06-20 04:17:05.000000 natsort-8.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-20 04:17:05.000000 natsort-8.4.0/RELEASING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:11.385888 natsort-8.4.0/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-20 04:17:05.000000 natsort-8.4.0/dev/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2318 2023-06-20 04:17:05.000000 natsort-8.4.0/dev/bump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-06-20 04:17:05.000000 natsort-8.4.0/dev/clean.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1299 2023-06-20 04:17:05.000000 natsort-8.4.0/dev/generate_new_unicode_numbers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:11.385888 natsort-8.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-06-20 04:17:05.000000 natsort-8.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 04:17:05.000000 natsort-8.4.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-06-20 04:17:05.000000 natsort-8.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-20 04:17:05.000000 natsort-8.4.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-20 04:17:05.000000 natsort-8.4.0/docs/howitworks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-20 04:17:05.000000 natsort-8.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 04:17:05.000000 natsort-8.4.0/docs/locale_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-20 04:17:05.000000 natsort-8.4.0/docs/shell.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:11.385888 natsort-8.4.0/mypy_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-20 04:17:05.000000 natsort-8.4.0/mypy_stubs/icu.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:11.385888 natsort-8.4.0/natsort/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-20 04:17:05.000000 natsort-8.4.0/natsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-06-20 04:17:05.000000 natsort-8.4.0/natsort/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:11.389888 natsort-8.4.0/natsort/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:05.000000 natsort-8.4.0/natsort/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-20 04:17:05.000000 natsort-8.4.0/natsort/compat/fake_fastnumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-20 04:17:05.000000 natsort-8.4.0/natsort/compat/fastnumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-20 04:17:05.000000 natsort-8.4.0/natsort/compat/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23834 2023-06-20 04:17:05.000000 natsort-8.4.0/natsort/natsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-06-20 04:17:05.000000 natsort-8.4.0/natsort/ns_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:05.000000 natsort-8.4.0/natsort/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-20 04:17:05.000000 natsort-8.4.0/natsort/unicode_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23451 2023-06-20 04:17:05.000000 natsort-8.4.0/natsort/unicode_numeric_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28544 2023-06-20 04:17:05.000000 natsort-8.4.0/natsort/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:11.389888 natsort-8.4.0/natsort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21827 2023-06-20 04:17:11.000000 natsort-8.4.0/natsort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-20 04:17:11.000000 natsort-8.4.0/natsort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:17:11.000000 natsort-8.4.0/natsort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 04:17:11.000000 natsort-8.4.0/natsort.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:17:11.000000 natsort-8.4.0/natsort.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 04:17:11.000000 natsort-8.4.0/natsort.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 04:17:11.000000 natsort-8.4.0/natsort.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-20 04:17:11.393888 natsort-8.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 04:17:05.000000 natsort-8.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:17:11.389888 natsort-8.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/profile_natsorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_fake_fastnumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_final_data_transform_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_input_string_transform_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_natsort_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_natsort_keygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13565 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_natsorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_natsorted_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_ns_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_os_sorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_parse_bytes_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_parse_number_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_parse_string_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_string_component_transform_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_unicode_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-06-20 04:17:05.000000 natsort-8.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-20 04:17:05.000000 natsort-8.4.0/tox.ini
```

### Comparing `natsort-8.3.1/LICENSE` & `natsort-8.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/PKG-INFO` & `natsort-8.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natsort
-Version: 8.3.1
+Version: 8.4.0
 Summary: Simple yet flexible natural sorting in Python.
 Home-page: https://github.com/SethMMorton/natsort
 Author: Seth M. Morton
 Author-email: drtuba78@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -501,15 +501,15 @@
 ------
 
 Seth M. Morton
 
 History
 -------
 
-Please visit the changelog `on GitHub`_ or `in the documentation`_.
+Please visit the changelog `on GitHub`_.
 
 .. _natsort: https://natsort.readthedocs.io/en/stable/index.html
 .. _natsorted(): https://natsort.readthedocs.io/en/stable/api.html#natsort.natsorted
 .. _natsort_keygen(): https://natsort.readthedocs.io/en/stable/api.html#natsort.natsort_keygen
 .. _realsorted(): https://natsort.readthedocs.io/en/stable/api.html#natsort.realsorted
 .. _humansorted(): https://natsort.readthedocs.io/en/stable/api.html#natsort.humansorted
 .. _os_sorted(): https://natsort.readthedocs.io/en/stable/api.html#natsort.os_sorted
@@ -530,15 +530,14 @@
 .. _"extras" notation: https://packaging.python.org/tutorials/installing-packages/#installing-setuptools-extras
 .. _PyICU: https://pypi.org/project/PyICU
 .. _tox: https://tox.readthedocs.io/en/latest/
 .. _Examples and Recipes: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes
 .. _How Does Natsort Work?: https://github.com/SethMMorton/natsort/wiki/How-Does-Natsort-Work%3F
 .. _API: https://natsort.readthedocs.io/en/stable/api.html
 .. _on GitHub: https://github.com/SethMMorton/natsort/blob/main/CHANGELOG.md
-.. _in the documentation: https://natsort.readthedocs.io/en/stable/changelog.html
 .. _file an issue: https://github.com/SethMMorton/natsort/issues/new
 .. _look at this issue describing how to debug: https://github.com/SethMMorton/natsort/issues/13#issuecomment-50422375
 .. _controlling the case-sensitivity: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#controlling-case-when-sorting
 .. _sorting file paths correctly: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#sort-os-generated-paths
 .. _allow custom sorting keys: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#using-a-custom-sorting-key
 .. _accounting for units: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#accounting-for-units-when-sorting
 .. _these version sorting examples: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#sorting-more-expressive-versioning-schemes
```

### Comparing `natsort-8.3.1/README.rst` & `natsort-8.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -467,15 +467,15 @@
 ------
 
 Seth M. Morton
 
 History
 -------
 
-Please visit the changelog `on GitHub`_ or `in the documentation`_.
+Please visit the changelog `on GitHub`_.
 
 .. _natsort: https://natsort.readthedocs.io/en/stable/index.html
 .. _natsorted(): https://natsort.readthedocs.io/en/stable/api.html#natsort.natsorted
 .. _natsort_keygen(): https://natsort.readthedocs.io/en/stable/api.html#natsort.natsort_keygen
 .. _realsorted(): https://natsort.readthedocs.io/en/stable/api.html#natsort.realsorted
 .. _humansorted(): https://natsort.readthedocs.io/en/stable/api.html#natsort.humansorted
 .. _os_sorted(): https://natsort.readthedocs.io/en/stable/api.html#natsort.os_sorted
@@ -496,15 +496,14 @@
 .. _"extras" notation: https://packaging.python.org/tutorials/installing-packages/#installing-setuptools-extras
 .. _PyICU: https://pypi.org/project/PyICU
 .. _tox: https://tox.readthedocs.io/en/latest/
 .. _Examples and Recipes: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes
 .. _How Does Natsort Work?: https://github.com/SethMMorton/natsort/wiki/How-Does-Natsort-Work%3F
 .. _API: https://natsort.readthedocs.io/en/stable/api.html
 .. _on GitHub: https://github.com/SethMMorton/natsort/blob/main/CHANGELOG.md
-.. _in the documentation: https://natsort.readthedocs.io/en/stable/changelog.html
 .. _file an issue: https://github.com/SethMMorton/natsort/issues/new
 .. _look at this issue describing how to debug: https://github.com/SethMMorton/natsort/issues/13#issuecomment-50422375
 .. _controlling the case-sensitivity: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#controlling-case-when-sorting
 .. _sorting file paths correctly: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#sort-os-generated-paths
 .. _allow custom sorting keys: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#using-a-custom-sorting-key
 .. _accounting for units: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#accounting-for-units-when-sorting
 .. _these version sorting examples: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#sorting-more-expressive-versioning-schemes
```

### Comparing `natsort-8.3.1/RELEASING.md` & `natsort-8.4.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/dev/README.md` & `natsort-8.4.0/dev/README.md`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/dev/bump.py` & `natsort-8.4.0/dev/bump.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/dev/clean.py` & `natsort-8.4.0/dev/clean.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/dev/generate_new_unicode_numbers.py` & `natsort-8.4.0/dev/generate_new_unicode_numbers.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/docs/api.rst` & `natsort-8.4.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/docs/conf.py` & `natsort-8.4.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,23 +29,22 @@
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
-    "m2r2",
 ]
 autodoc_typehints = "none"
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = [".rst", ".md"]
+source_suffix = [".rst"]
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
@@ -55,15 +54,15 @@
 copyright = "2014, Seth M. Morton"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = "8.3.1"
+release = "8.4.0"
 # The short X.Y version.
 version = ".".join(release.split(".")[0:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
```

### Comparing `natsort-8.3.1/docs/index.rst` & `natsort-8.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/mypy_stubs/icu.pyi` & `natsort-8.4.0/mypy_stubs/icu.pyi`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/natsort/__init__.py` & `natsort-8.4.0/natsort/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     os_sort_keygen,
     os_sorted,
     realsorted,
 )
 from natsort.ns_enum import NSType, ns
 from natsort.utils import KeyType, NatsortInType, NatsortOutType, chain_functions
 
-__version__ = "8.3.1"
+__version__ = "8.4.0"
 
 __all__ = [
     "natsort_key",
     "natsort_keygen",
     "natsorted",
     "humansorted",
     "realsorted",
```

### Comparing `natsort-8.3.1/natsort/__main__.py` & `natsort-8.4.0/natsort/__main__.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/natsort/compat/fake_fastnumbers.py` & `natsort-8.4.0/natsort/compat/fake_fastnumbers.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/natsort/compat/fastnumbers.py` & `natsort-8.4.0/natsort/compat/fastnumbers.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/natsort/compat/locale.py` & `natsort-8.4.0/natsort/compat/locale.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 null_string_max = chr(sys.maxunicode) * 20
 
 # This variable could be str or bytes depending on the locale library
 # being used, so give the type-checker this information.
 null_string_locale: StrOrBytes
 null_string_locale_max: StrOrBytes
 
-# strxfrm can be buggy (especially on BSD-based systems),
-# so prefer icu if available.
+# strxfrm can be buggy (especially on OSX and *possibly* some other
+# BSD-based systems), so prefer icu if available.
 try:  # noqa: C901
     import icu
     from locale import getlocale
 
     null_string_locale = b""
 
     # This string should in theory be sorted after any other byte
```

### Comparing `natsort-8.3.1/natsort/natsort.py` & `natsort-8.4.0/natsort/natsort.py`

 * *Files 2% similar despite different names*

```diff
@@ -666,21 +666,21 @@
 
     """
     # Remove the leading and trailing parens
     return utils.regex_chooser(alg).pattern[1:-1]
 
 
 def _split_apply(
-    v: Any, key: Optional[Callable[[T], NatsortInType]] = None
+    v: Any, key: Optional[Callable[[T], NatsortInType]] = None, treat_base: bool = True
 ) -> Iterator[str]:
     if key is not None:
         v = key(v)
     if not isinstance(v, (str, PurePath)):
         v = str(v)
-    return utils.path_splitter(v)
+    return utils.path_splitter(v, treat_base=treat_base)
 
 
 # Choose the implementation based on the host OS
 if platform.system() == "Windows":
     from ctypes import wintypes, windll  # type: ignore
     from functools import cmp_to_key
 
@@ -690,15 +690,15 @@
     _winsort_key = cmp_to_key(_windows_sort_cmp)
 
     def os_sort_keygen(
         key: Optional[Callable[[Any], NatsortInType]] = None
     ) -> Callable[[Any], NatsortOutType]:
         return cast(
             Callable[[Any], NatsortOutType],
-            lambda x: tuple(map(_winsort_key, _split_apply(x, key))),
+            lambda x: tuple(map(_winsort_key, _split_apply(x, key, treat_base=False))),
         )
 
 else:
     # For UNIX-based platforms, ICU performs MUCH better than locale
     # at replicating the file explorer's sort order. We will use
     # ICU's ability to do basic natural sorting as it also better
     # replicates than what natsort does by default.
```

### Comparing `natsort-8.3.1/natsort/ns_enum.py` & `natsort-8.4.0/natsort/ns_enum.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/natsort/unicode_numbers.py` & `natsort-8.4.0/natsort/unicode_numbers.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/natsort/unicode_numeric_hex.py` & `natsort-8.4.0/natsort/unicode_numeric_hex.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/natsort/utils.py` & `natsort-8.4.0/natsort/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -872,24 +872,28 @@
         return s.decode(encoding)
     else:
         return s
 
 
 # noinspection PyIncorrectDocstring
 def path_splitter(
-    s: PathArg, _d_match: MatchFn = re.compile(r"\.\d").match
+    s: PathArg, treat_base: bool = True, _d_match: MatchFn = re.compile(r"\.\d").match
 ) -> Iterator[str]:
     """
     Split a string into its path components.
 
     Assumes a string is a path or is path-like.
 
     Parameters
     ----------
     s : str | pathlib.Path
+    treat_base: bool, optional
+        If True, treat the base of component of the file path as
+        special and split off extensions. If False, do not do this.
+        The default is True.
 
     Returns
     -------
     split : tuple
         The path split by directory components and extensions.
 
     Examples
@@ -905,25 +909,26 @@
     # Split the path into parts.
     try:
         *path_parts, base = s.parts
     except ValueError:
         path_parts = []
         base = str(s)
 
-    # Now, split off the file extensions until
-    #  - we reach a decimal number at the beginning of the suffix
-    #  - more than two suffixes have been seen
-    #  - a suffix is more than five characters (including leading ".")
-    #  - there are no more extensions
     suffixes = []
-    for i, suffix in enumerate(reversed(PurePath(base).suffixes)):
-        if _d_match(suffix) or i > 1 or len(suffix) > 5:
-            break
-        suffixes.append(suffix)
-    suffixes.reverse()
+    if treat_base:
+        # Now, split off the file extensions until
+        #  - we reach a decimal number at the beginning of the suffix
+        #  - more than two suffixes have been seen
+        #  - a suffix is more than five characters (including leading ".")
+        #  - there are no more extensions
+        for i, suffix in enumerate(reversed(PurePath(base).suffixes)):
+            if _d_match(suffix) or i > 1 or len(suffix) > 5:
+                break
+            suffixes.append(suffix)
+        suffixes.reverse()
 
     # Remove the suffixes from the base component
     base = base.replace("".join(suffixes), "")
     base_component = [base] if base else []
 
     # Join all path comonents in an iterator
     return filter(None, ichain(path_parts, base_component, suffixes))
```

### Comparing `natsort-8.3.1/natsort.egg-info/PKG-INFO` & `natsort-8.4.0/natsort.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natsort
-Version: 8.3.1
+Version: 8.4.0
 Summary: Simple yet flexible natural sorting in Python.
 Home-page: https://github.com/SethMMorton/natsort
 Author: Seth M. Morton
 Author-email: drtuba78@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -501,15 +501,15 @@
 ------
 
 Seth M. Morton
 
 History
 -------
 
-Please visit the changelog `on GitHub`_ or `in the documentation`_.
+Please visit the changelog `on GitHub`_.
 
 .. _natsort: https://natsort.readthedocs.io/en/stable/index.html
 .. _natsorted(): https://natsort.readthedocs.io/en/stable/api.html#natsort.natsorted
 .. _natsort_keygen(): https://natsort.readthedocs.io/en/stable/api.html#natsort.natsort_keygen
 .. _realsorted(): https://natsort.readthedocs.io/en/stable/api.html#natsort.realsorted
 .. _humansorted(): https://natsort.readthedocs.io/en/stable/api.html#natsort.humansorted
 .. _os_sorted(): https://natsort.readthedocs.io/en/stable/api.html#natsort.os_sorted
@@ -530,15 +530,14 @@
 .. _"extras" notation: https://packaging.python.org/tutorials/installing-packages/#installing-setuptools-extras
 .. _PyICU: https://pypi.org/project/PyICU
 .. _tox: https://tox.readthedocs.io/en/latest/
 .. _Examples and Recipes: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes
 .. _How Does Natsort Work?: https://github.com/SethMMorton/natsort/wiki/How-Does-Natsort-Work%3F
 .. _API: https://natsort.readthedocs.io/en/stable/api.html
 .. _on GitHub: https://github.com/SethMMorton/natsort/blob/main/CHANGELOG.md
-.. _in the documentation: https://natsort.readthedocs.io/en/stable/changelog.html
 .. _file an issue: https://github.com/SethMMorton/natsort/issues/new
 .. _look at this issue describing how to debug: https://github.com/SethMMorton/natsort/issues/13#issuecomment-50422375
 .. _controlling the case-sensitivity: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#controlling-case-when-sorting
 .. _sorting file paths correctly: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#sort-os-generated-paths
 .. _allow custom sorting keys: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#using-a-custom-sorting-key
 .. _accounting for units: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#accounting-for-units-when-sorting
 .. _these version sorting examples: https://github.com/SethMMorton/natsort/wiki/Examples-and-Recipes#sorting-more-expressive-versioning-schemes
```

### Comparing `natsort-8.3.1/natsort.egg-info/SOURCES.txt` & `natsort-8.4.0/natsort.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 docs/api.rst
 docs/changelog.rst
 docs/conf.py
 docs/examples.rst
 docs/howitworks.rst
 docs/index.rst
 docs/locale_issues.rst
-docs/requirements.in
-docs/requirements.txt
 docs/shell.rst
-docs/special_cases_everywhere.jpg
 mypy_stubs/icu.pyi
 natsort/__init__.py
 natsort/__main__.py
 natsort/natsort.py
 natsort/ns_enum.py
 natsort/py.typed
 natsort/unicode_numbers.py
```

### Comparing `natsort-8.3.1/setup.cfg` & `natsort-8.4.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 8.3.1
+current_version = 8.4.0
 commit = True
 tag = True
 tag_name = {new_version}
 
 [metadata]
 author = Seth M. Morton
 author_email = drtuba78@gmail.com
```

### Comparing `natsort-8.3.1/tests/conftest.py` & `natsort-8.4.0/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,19 +15,16 @@
 # slow then causes the tests to fail.
 hypothesis.settings.register_profile(
     "slow-tests", suppress_health_check=[hypothesis.HealthCheck.too_slow]
 )
 
 
 def load_locale(x: str) -> None:
-    """Convenience to load a locale, trying ISO8859-1 first."""
-    try:
-        locale.setlocale(locale.LC_ALL, str("{}.ISO8859-1".format(x)))
-    except locale.Error:
-        locale.setlocale(locale.LC_ALL, str("{}.UTF-8".format(x)))
+    """Convenience to load a locale."""
+    locale.setlocale(locale.LC_ALL, str("{}.UTF-8".format(x)))
 
 
 @pytest.fixture()
 def with_locale_en_us() -> Iterator[None]:
     """Convenience to load the en_US locale - reset when complete."""
     orig = locale.getlocale()
     load_locale("en_US")
```

### Comparing `natsort-8.3.1/tests/profile_natsorted.py` & `natsort-8.4.0/tests/profile_natsorted.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_fake_fastnumbers.py` & `natsort-8.4.0/tests/test_fake_fastnumbers.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_final_data_transform_factory.py` & `natsort-8.4.0/tests/test_final_data_transform_factory.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_input_string_transform_factory.py` & `natsort-8.4.0/tests/test_input_string_transform_factory.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_main.py` & `natsort-8.4.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_natsort_key.py` & `natsort-8.4.0/tests/test_natsort_key.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_natsort_keygen.py` & `natsort-8.4.0/tests/test_natsort_keygen.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_natsorted.py` & `natsort-8.4.0/tests/test_natsorted.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_natsorted_convenience.py` & `natsort-8.4.0/tests/test_natsorted_convenience.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_ns_enum.py` & `natsort-8.4.0/tests/test_ns_enum.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_os_sorted.py` & `natsort-8.4.0/tests/test_os_sorted.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,22 +20,32 @@
         "/p/Folder (10)/file.tar.gz",
         "/p/Folder (1)/file (1).tar.gz",
         "/p/Folder/file.x1.9.tar.gz",
         "/p/Folder (2)/file.tar.gz",
         "/p/Folder (1)/file.tar.gz",
         "/p/Folder/file.x1.10.tar.gz",
     ]
-    expected = [
-        "/p/Folder/file.x1.9.tar.gz",
-        "/p/Folder/file.x1.10.tar.gz",
-        "/p/Folder (1)/file.tar.gz",
-        "/p/Folder (1)/file (1).tar.gz",
-        "/p/Folder (2)/file.tar.gz",
-        "/p/Folder (10)/file.tar.gz",
-    ]
+    if platform.system() == "Windows":
+        expected = [
+            "/p/Folder/file.x1.9.tar.gz",
+            "/p/Folder/file.x1.10.tar.gz",
+            "/p/Folder (1)/file (1).tar.gz",
+            "/p/Folder (1)/file.tar.gz",
+            "/p/Folder (2)/file.tar.gz",
+            "/p/Folder (10)/file.tar.gz",
+        ]
+    else:
+        expected = [
+            "/p/Folder/file.x1.9.tar.gz",
+            "/p/Folder/file.x1.10.tar.gz",
+            "/p/Folder (1)/file.tar.gz",
+            "/p/Folder (1)/file (1).tar.gz",
+            "/p/Folder (2)/file.tar.gz",
+            "/p/Folder (10)/file.tar.gz",
+        ]
     result = natsort.os_sorted(given)
     assert result == expected
 
 
 def test_os_sorted_misc_no_fail() -> None:
     natsort.os_sorted([9, 4.3, None, float("nan")])
```

### Comparing `natsort-8.3.1/tests/test_parse_bytes_function.py` & `natsort-8.4.0/tests/test_parse_bytes_function.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_parse_number_function.py` & `natsort-8.4.0/tests/test_parse_number_function.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_parse_string_function.py` & `natsort-8.4.0/tests/test_parse_string_function.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_regex.py` & `natsort-8.4.0/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_string_component_transform_factory.py` & `natsort-8.4.0/tests/test_string_component_transform_factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from hypothesis.strategies import floats, integers, text
 from natsort.compat.fastnumbers import try_float, try_int
 from natsort.compat.locale import get_strxfrm
 from natsort.ns_enum import NSType, NS_DUMB, ns
 from natsort.utils import groupletters, string_component_transform_factory
 
 # There are some unicode values that are known failures with the builtin locale
-# library on BSD systems that has nothing to do with natsort (a ValueError is
-# raised by strxfrm). Let's filter them out.
+# library on OSX and some other BSD-based systems that has nothing to do with
+# natsort (a ValueError is raised by strxfrm). Let's filter them out.
 try:
     bad_uni_chars = frozenset(chr(x) for x in range(0x10FEFD, 0x10FFFF + 1))
 except ValueError:
     # Narrow unicode build... no worries.
     bad_uni_chars = frozenset()
 
 
@@ -30,18 +30,15 @@
 def no_null(x: str) -> bool:
     """Ensure text does not contain a null character."""
     return "\0" not in x
 
 
 def input_is_ok_with_locale(x: str) -> bool:
     """Ensure this input won't cause locale.strxfrm to barf"""
-    # On FreeBSD, locale.strxfrm raises an OSError on input like 'Å'.
-    # You read that right - an *OSError* for invalid input.
-    # We cannot really fix that, so we just filter out any value
-    # that could cause locale.strxfrm to barf with this function.
+    # Bad input can cause an OSError if the OS doesn't support the value
     try:
         get_strxfrm()(x)
     except OSError:
         return False
     else:
         return True
 
@@ -87,13 +84,13 @@
 )
 @pytest.mark.usefixtures("with_locale_en_us")
 def test_string_component_transform_factory(
     x: Union[str, float, int], alg: NSType, example_func: Callable[[str], Any]
 ) -> None:
     string_component_transform_func = string_component_transform_factory(alg)
     x = str(x)
-    assume(input_is_ok_with_locale(x))  # handle broken locale lib on BSD.
+    assume(input_is_ok_with_locale(x))
     try:
         assert list(string_component_transform_func(x)) == list(example_func(x))
-    except ValueError as e:  # handle broken locale lib on BSD.
+    except ValueError as e:  # handle broken locale lib on OSX.
         if "is not in range" not in str(e):
             raise
```

### Comparing `natsort-8.3.1/tests/test_unicode_numbers.py` & `natsort-8.4.0/tests/test_unicode_numbers.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tests/test_utils.py` & `natsort-8.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `natsort-8.3.1/tox.ini` & `natsort-8.4.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 # Build documentation.
 # sphinx and sphinx_rtd_theme not in docs/requirements.txt because they
 # will already be installed on readthedocs.
 [testenv:docs]
 deps =
     sphinx
     sphinx_rtd_theme
-    -r docs/requirements.txt
 commands =
     {envpython} setup.py build_sphinx
 skip_install = true
 
 # Bump version
 [testenv:bump]
 passenv =
```

