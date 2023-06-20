# Comparing `tmp/teapy-0.1.6.tar.gz` & `tmp/teapy-0.1.7.tar.gz`

## Comparing `teapy-0.1.6.tar` & `teapy-0.1.7.tar`

### file list

```diff
@@ -1,83 +1,85 @@
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 teapy-0.1.6/Cargo.toml
--rw-r--r--   0     1001      123      763 2023-06-13 09:45:06.000000 teapy-0.1.6/.github/workflows/build.yaml
--rw-r--r--   0     1001      123      974 2023-06-13 09:45:06.000000 teapy-0.1.6/.github/workflows/coverage.yaml
--rw-r--r--   0     1001      123     3555 2023-06-13 09:45:06.000000 teapy-0.1.6/.github/workflows/release_python.yaml
--rw-r--r--   0     1001      123     1303 2023-06-13 09:45:06.000000 teapy-0.1.6/.github/workflows/test_python.yaml
--rw-r--r--   0     1001      123      105 2023-06-13 09:45:06.000000 teapy-0.1.6/.gitignore
--rw-r--r--   0     1001      123     1049 2023-06-13 09:45:06.000000 teapy-0.1.6/LICENSE
--rw-r--r--   0     1001      123     1228 2023-06-13 09:45:06.000000 teapy-0.1.6/Makefile
--rw-r--r--   0     1001      123      441 2023-06-13 09:45:06.000000 teapy-0.1.6/README.md
--rw-r--r--   0     1001      123      194 2023-06-13 09:45:06.000000 teapy-0.1.6/build.requirements.txt
--rw-r--r--   0     1001      123      464 2023-06-13 09:45:06.000000 teapy-0.1.6/pyproject.toml
--rwxr-xr-x   0     1001      123      848 2023-06-13 09:45:35.000000 teapy-0.1.6/run-maturin-action.sh
--rw-r--r--   0     1001      123       99 2023-06-13 09:45:06.000000 teapy-0.1.6/rust-toolchain.toml
--rw-r--r--   0     1001      123    14689 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/agg.rs
--rw-r--r--   0     1001      123    33054 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/arr_func.rs
--rw-r--r--   0     1001      123     4672 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/corr.rs
--rw-r--r--   0     1001      123     8744 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/datatype.rs
--rw-r--r--   0     1001      123      548 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/export.rs
--rw-r--r--   0     1001      123     9128 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/groupby.rs
--rw-r--r--   0     1001      123    15524 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/impls/impl_1d_method.rs
--rw-r--r--   0     1001      123     5221 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/impls/impl_linalg.rs
--rw-r--r--   0     1001      123    10397 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/impls/impl_method.rs
--rw-r--r--   0     1001      123     6606 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/impls/impl_numeric.rs
--rw-r--r--   0     1001      123     3399 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/impls/impl_traits.rs
--rw-r--r--   0     1001      123      114 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/impls/mod.rs
--rw-r--r--   0     1001      123    10337 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/iterators.rs
--rw-r--r--   0     1001      123     2886 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/join.rs
--rw-r--r--   0     1001      123     4867 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/auto_impl_own.rs
--rw-r--r--   0     1001      123     3247 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/expr_view.rs
--rw-r--r--   0     1001      123    14759 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/exprs.rs
--rw-r--r--   0     1001      123     1570 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/impl_cmp.rs
--rw-r--r--   0     1001      123      397 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/impl_mut.rs
--rw-r--r--   0     1001      123     2800 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/impl_ops.rs
--rw-r--r--   0     1001      123    25019 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/impl_own.rs
--rw-r--r--   0     1001      123    11567 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/impl_view.rs
--rw-r--r--   0     1001      123     8918 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/linalg.rs
--rw-r--r--   0     1001      123    41252 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/mod.rs
--rw-r--r--   0     1001      123    11490 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/macros.rs
--rw-r--r--   0     1001      123    21693 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/mod.rs
--rw-r--r--   0     1001      123      451 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/option_datetype.rs
--rw-r--r--   0     1001      123    11108 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/time.rs
--rw-r--r--   0     1001      123     1618 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/util_trait.rs
--rw-r--r--   0     1001      123     3680 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/utils/algos.rs
--rw-r--r--   0     1001      123     1746 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/utils/alloc.rs
--rw-r--r--   0     1001      123      195 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/utils/default_new.rs
--rw-r--r--   0     1001      123      185 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/utils/mod.rs
--rw-r--r--   0     1001      123    13468 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/window/compare.rs
--rw-r--r--   0     1001      123     6390 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/window/corr.rs
--rw-r--r--   0     1001      123    24023 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/window/feature.rs
--rw-r--r--   0     1001      123       75 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/window/mod.rs
--rw-r--r--   0     1001      123     9226 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/window/norm.rs
--rw-r--r--   0     1001      123    12965 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/window/reg.rs
--rw-r--r--   0     1001      123      110 2023-06-13 09:45:06.000000 teapy-0.1.6/src/eager_api.rs
--rw-r--r--   0     1001      123    13833 2023-06-13 09:45:06.000000 teapy-0.1.6/src/equity.rs
--rw-r--r--   0     1001      123     7617 2023-06-13 09:45:06.000000 teapy-0.1.6/src/from_py.rs
--rw-r--r--   0     1001      123     1310 2023-06-13 09:45:06.000000 teapy-0.1.6/src/lib.rs
--rw-r--r--   0     1001      123    37387 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/datadict.rs
--rw-r--r--   0     1001      123      530 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/export.rs
--rw-r--r--   0     1001      123     2628 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/groupby.rs
--rw-r--r--   0     1001      123    87804 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/impl_pyexpr.rs
--rw-r--r--   0     1001      123     1200 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/mod.rs
--rw-r--r--   0     1001      123    19759 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/pyexpr.rs
--rw-r--r--   0     1001      123    14983 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/pyfunc.rs
--rw-r--r--   0     1001      123      454 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/time.rs
--rw-r--r--   0     1001      123      407 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/__init__.py
--rw-r--r--   0     1001      123     4911 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/array_func.py
--rw-r--r--   0     1001      123     3184 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/converter.py
--rw-r--r--   0     1001      123     4264 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/datadict.py
--rw-r--r--   0     1001      123     6985 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/regression.py
--rw-r--r--   0     1001      123     3440 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/testing.py
--rw-r--r--   0     1001      123    10728 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      123     3380 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/test_common.py
--rw-r--r--   0     1001      123     2240 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/test_equity.py
--rw-r--r--   0     1001      123      245 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/test_memory.py
--rw-r--r--   0     1001      123     3211 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      123     1418 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      123     5772 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      123     1995 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      123     3165 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      123     3695 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/window_func.py
--rw-r--r--   0     1001      123     6509 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/wrapper.py
--rw-r--r--   0     1001      123    44634 2023-06-13 09:45:06.000000 teapy-0.1.6/Cargo.lock
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 teapy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 teapy-0.1.7/Cargo.toml
+-rw-r--r--   0     1001      123      763 2023-06-20 16:14:17.000000 teapy-0.1.7/.github/workflows/build.yaml
+-rw-r--r--   0     1001      123      975 2023-06-20 16:14:17.000000 teapy-0.1.7/.github/workflows/coverage.yaml
+-rw-r--r--   0     1001      123     3561 2023-06-20 16:14:17.000000 teapy-0.1.7/.github/workflows/release_python.yaml
+-rw-r--r--   0     1001      123     1303 2023-06-20 16:14:17.000000 teapy-0.1.7/.github/workflows/test_python.yaml
+-rw-r--r--   0     1001      123      105 2023-06-20 16:14:17.000000 teapy-0.1.7/.gitignore
+-rw-r--r--   0     1001      123     1049 2023-06-20 16:14:17.000000 teapy-0.1.7/LICENSE
+-rw-r--r--   0     1001      123     1276 2023-06-20 16:14:17.000000 teapy-0.1.7/Makefile
+-rw-r--r--   0     1001      123      520 2023-06-20 16:14:17.000000 teapy-0.1.7/README.md
+-rw-r--r--   0     1001      123      214 2023-06-20 16:14:17.000000 teapy-0.1.7/build.requirements.txt
+-rw-r--r--   0     1001      123      444 2023-06-20 16:14:17.000000 teapy-0.1.7/pyproject.toml
+-rwxr-xr-x   0     1001      123      848 2023-06-20 16:14:47.000000 teapy-0.1.7/run-maturin-action.sh
+-rw-r--r--   0     1001      123       99 2023-06-20 16:14:17.000000 teapy-0.1.7/rust-toolchain.toml
+-rw-r--r--   0     1001      123    14724 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/agg.rs
+-rw-r--r--   0     1001      123    33304 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/arr_func.rs
+-rw-r--r--   0     1001      123     4672 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/corr.rs
+-rw-r--r--   0     1001      123     8744 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/datatype.rs
+-rw-r--r--   0     1001      123      535 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/export.rs
+-rw-r--r--   0     1001      123     9128 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/groupby.rs
+-rw-r--r--   0     1001      123    15524 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/impls/impl_1d_method.rs
+-rw-r--r--   0     1001      123     5221 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/impls/impl_linalg.rs
+-rw-r--r--   0     1001      123    10412 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/impls/impl_method.rs
+-rw-r--r--   0     1001      123     6606 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/impls/impl_numeric.rs
+-rw-r--r--   0     1001      123     4100 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/impls/impl_traits.rs
+-rw-r--r--   0     1001      123      114 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/impls/mod.rs
+-rw-r--r--   0     1001      123    10337 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/iterators.rs
+-rw-r--r--   0     1001      123     2886 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/join.rs
+-rw-r--r--   0     1001      123     4837 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/lazy/auto_impl_own.rs
+-rw-r--r--   0     1001      123     3247 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/lazy/expr_view.rs
+-rw-r--r--   0     1001      123    14759 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/lazy/exprs.rs
+-rw-r--r--   0     1001      123     1570 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/lazy/impl_cmp.rs
+-rw-r--r--   0     1001      123      348 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/lazy/impl_mut.rs
+-rw-r--r--   0     1001      123     2800 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/lazy/impl_ops.rs
+-rw-r--r--   0     1001      123    26598 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/lazy/impl_own.rs
+-rw-r--r--   0     1001      123    10989 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/lazy/impl_view.rs
+-rw-r--r--   0     1001      123     8918 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/lazy/linalg.rs
+-rw-r--r--   0     1001      123    41252 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/lazy/mod.rs
+-rw-r--r--   0     1001      123    11591 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/macros.rs
+-rw-r--r--   0     1001      123    23080 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/mod.rs
+-rw-r--r--   0     1001      123      451 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/option_datetype.rs
+-rw-r--r--   0     1001      123    11274 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/time.rs
+-rw-r--r--   0     1001      123     1618 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/util_trait.rs
+-rw-r--r--   0     1001      123     3680 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/utils/algos.rs
+-rw-r--r--   0     1001      123     1746 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/utils/alloc.rs
+-rw-r--r--   0     1001      123      195 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/utils/default_new.rs
+-rw-r--r--   0     1001      123      185 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/utils/mod.rs
+-rw-r--r--   0     1001      123    13468 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/window/compare.rs
+-rw-r--r--   0     1001      123     6390 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/window/corr.rs
+-rw-r--r--   0     1001      123    24023 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/window/feature.rs
+-rw-r--r--   0     1001      123       75 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/window/mod.rs
+-rw-r--r--   0     1001      123     9226 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/window/norm.rs
+-rw-r--r--   0     1001      123    12965 2023-06-20 16:14:17.000000 teapy-0.1.7/src/arr/window/reg.rs
+-rw-r--r--   0     1001      123      110 2023-06-20 16:14:17.000000 teapy-0.1.7/src/eager_api.rs
+-rw-r--r--   0     1001      123    13833 2023-06-20 16:14:17.000000 teapy-0.1.7/src/equity.rs
+-rw-r--r--   0     1001      123     7964 2023-06-20 16:14:17.000000 teapy-0.1.7/src/from_py.rs
+-rw-r--r--   0     1001      123      988 2023-06-20 16:14:17.000000 teapy-0.1.7/src/lib.rs
+-rw-r--r--   0     1001      123    41221 2023-06-20 16:14:17.000000 teapy-0.1.7/src/pylazy/datadict.rs
+-rw-r--r--   0     1001      123      530 2023-06-20 16:14:17.000000 teapy-0.1.7/src/pylazy/export.rs
+-rw-r--r--   0     1001      123     2618 2023-06-20 16:14:17.000000 teapy-0.1.7/src/pylazy/groupby.rs
+-rw-r--r--   0     1001      123    88666 2023-06-20 16:14:17.000000 teapy-0.1.7/src/pylazy/impl_pyexpr.rs
+-rw-r--r--   0     1001      123     1277 2023-06-20 16:14:17.000000 teapy-0.1.7/src/pylazy/mod.rs
+-rw-r--r--   0     1001      123    19916 2023-06-20 16:14:17.000000 teapy-0.1.7/src/pylazy/pyexpr.rs
+-rw-r--r--   0     1001      123    16510 2023-06-20 16:14:17.000000 teapy-0.1.7/src/pylazy/pyfunc.rs
+-rw-r--r--   0     1001      123      454 2023-06-20 16:14:17.000000 teapy-0.1.7/src/pylazy/time.rs
+-rw-r--r--   0     1001      123      414 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/__init__.py
+-rw-r--r--   0     1001      123     4513 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/array_func.py
+-rw-r--r--   0     1001      123     3184 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/converter.py
+-rw-r--r--   0     1001      123     6341 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/datadict.py
+-rw-r--r--   0     1001      123     6985 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/regression.py
+-rw-r--r--   0     1001      123     3440 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/testing.py
+-rw-r--r--   0     1001      123    10728 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      123     3406 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/tests/test_common.py
+-rw-r--r--   0     1001      123     3924 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/tests/test_datadict.py
+-rw-r--r--   0     1001      123     2240 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/tests/test_equity.py
+-rw-r--r--   0     1001      123      747 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/tests/test_expr.py
+-rw-r--r--   0     1001      123      245 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/tests/test_memory.py
+-rw-r--r--   0     1001      123     3211 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      123     1418 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      123     5772 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      123     1995 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      123     3165 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      123     3695 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/window_func.py
+-rw-r--r--   0     1001      123     6509 2023-06-20 16:14:17.000000 teapy-0.1.7/teapy/wrapper.py
+-rw-r--r--   0     1001      123    48415 2023-06-20 16:14:17.000000 teapy-0.1.7/Cargo.lock
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 teapy-0.1.7/PKG-INFO
```

### Comparing `teapy-0.1.6/Cargo.toml` & `teapy-0.1.7/Cargo.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 [package]
 name = "teapy"
-version = "0.1.6"
+version = "0.1.7"
 edition = "2021"
 
 [lib]
 name = "teapy"
 crate-type = ["cdylib", "rlib"]
 
 [features]
 default = ["lazy", "blas"]
 lazy = ["window_func"]
-# eager_api = ["window_func"]
 window_func = []
 blas = ["ndarray-linalg", "ndarray/blas", "lazy", "statrs", "lapack-sys"]
 
 [profile.release]
 lto = true
 
 [dependencies]
-pyo3 = {version = "0.18.0", features = ["extension-module", "abi3-py38", "macros"]}
-# numpy = {git = "https://github.com/PyO3/rust-numpy.git", branch = "main"}
-numpy = "0.18"
+pyo3 = {version = "0.19.0", features = ["extension-module", "abi3-py38", "macros", "serde"]}
+numpy = "0.19"
 num = "0.4"
 cxx = "1.0"
 rayon = "1.5"
 ahash = "0.8.2"
-chrono = "0.4.23"
+regex = "1"
+chrono = {version = "0.4.23", features = ["serde"]}
+serde = { version = "1.0", features = ["derive"] }
+serde_with = {version = "3.0", features = ["chrono"]}
+serde-pickle = "1.1"
+bincode = "1.3"
 once_cell = "1"
-ndarray = {features=['rayon'], version="0.15"}
-ndarray-linalg = { version = "0.16.0", features = ["intel-mkl-static"], optional=true}
+ndarray = {features=['rayon', 'serde'], version="0.15"}
+ndarray-linalg = {git = "https://github.com/Teamon9161/ndarray-linalg.git", branch = "arm-cross-compile", features = ["intel-mkl-static"], optional=true}
 ndarray-npy = {version = "0.8.1"}
 statrs = {version = "0.16", optional=true}
 lapack-sys = {version="0.14.0", optional=true}
```

### Comparing `teapy-0.1.6/.github/workflows/build.yaml` & `teapy-0.1.7/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/.github/workflows/coverage.yaml` & `teapy-0.1.7/.github/workflows/coverage.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -31,13 +31,14 @@
       - uses: Swatinem/rust-cache@v2
         with:
           key: coverage-cargo-${{ matrix.os }}
         continue-on-error: true
 
       - name: Run coverage
         run: make coverage
+
       - uses: codecov/codecov-action@v3
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           files: coverage.lcov,coverage.xml
           name: ${{ matrix.os }}
           fail_ci_if_error: true
```

### Comparing `teapy-0.1.6/.github/workflows/release_python.yaml` & `teapy-0.1.7/.github/workflows/release_python.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -93,27 +93,27 @@
           maturin-version: ${{ env.MATURIN_VERSION }}
           command: publish
           args: --target aarch64-apple-darwin --skip-existing --no-sdist -o wheels -i python -u teamon
 
 
   # # the dependency of ndarry-linalg crate can not be build on manylinux-arrch64 currently
   
-  # # Needed for Docker on Apple M1
-  # manylinux-aarch64:
-  #   runs-on: ubuntu-latest
-  #   steps:
-  #     - uses: actions/checkout@v3
-  #     - uses: actions/setup-python@v4
-  #       with:
-  #         python-version: '3.8'
+  # Needed for Docker on Apple M1
+  manylinux-aarch64:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v4
+        with:
+          python-version: ${{ env.PYTHON_VERSION }}
 
-  #     - name: Publish wheel
-  #       uses: messense/maturin-action@v1
-  #       env:
-  #         MATURIN_PASSWORD: ${{ secrets.PYPI_SECRET }}
-  #         JEMALLOC_SYS_WITH_LG_PAGE: 16
-  #       with:
-  #         rust-toolchain: nightly-2023-01-19
-  #         target: aarch64-unknown-linux-gnu
-  #         maturin-version: '0.14.10'
-  #         command: publish
-  #         args: --skip-existing --no-sdist -o wheels -i python -u teamon
+      - name: Publish wheel
+        uses: messense/maturin-action@v1
+        env:
+          MATURIN_PASSWORD: ${{ secrets.PYPI_SECRET }}
+          JEMALLOC_SYS_WITH_LG_PAGE: 16
+        with:
+          rust-toolchain: ${{ env.RUST_TOOLCHAIN }}
+          maturin-version: ${{ env.MATURIN_VERSION }}
+          target: aarch64-unknown-linux-gnu
+          command: publish
+          args: --skip-existing --no-sdist -o wheels -i python -u teamon
```

### Comparing `teapy-0.1.6/.github/workflows/test_python.yaml` & `teapy-0.1.7/.github/workflows/test_python.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/LICENSE` & `teapy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/Makefile` & `teapy-0.1.7/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,23 @@
 clean: ## clean useless folders
 	@rm -rf venv/
 	@rm -rf target/
 	@rm -rf .hypothesis/
 	@rm -rf .pytest_cache/
 	@cargo clean
 
+.PHONY: test
+test: 
+	@pytest -n auto
+
+
 .PHONY: pytest-cov
 pytest-cov: venv  ## test with coverage report
 	@pytest teapy/tests \
+	-n auto \
 	--cov=teapy \
 	--cov-report xml \
 	--import-mode=importlib
 
 .PHONY: format
 format:  ## format and check
 	isort . --profile black
@@ -34,15 +40,15 @@
 		source venv/bin/activate; \
 		source <(cargo llvm-cov show-env --export-prefix); \
 		export CARGO_TARGET_DIR=\$$CARGO_LLVM_COV_TARGET_DIR; \
 		export CARGO_INCREMENTAL=1; \
 		cargo llvm-cov clean --workspace; \
 		maturin develop; \
 		$(MAKE) pytest-cov; \
-		cargo llvm-cov --no-run --lcov --output-path coverage.lcov; \
+		cargo llvm-cov report --lcov --output-path coverage.lcov; \
 		"
 
 .PHONY: release
 release:
 	maturin develop --release -- -C target-cpu=native
 
 .PHONY: debug
```

### Comparing `teapy-0.1.6/run-maturin-action.sh` & `teapy-0.1.7/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/agg.rs` & `teapy-0.1.7/src/arr/agg.rs`

 * *Files 1% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 }
 
 impl<T, S, D> ArrBase<S, D>
 where
     S: Data<Elem = T>,
     D: Dimension,
 {
-    pub fn take_1_on_axis(&self, index: usize, axis: usize, par: bool) -> Arr<T, D::Smaller>
+    pub fn take_1_on_axis(&self, index: usize, axis: i32, par: bool) -> Arr<T, D::Smaller>
     where
         T: Send + Sync + Clone,
         D: RemoveAxis,
     {
-        assert!(index < self.shape()[axis], "Index out of bound.");
+        let axis = self.norm_axis(axis);
+        assert!(index < self.shape()[axis.index()], "Index out of bound.");
         // Safety: we have checked that 0 <= index <= the length of axis - 1
         if !par {
-            Zip::from(self.lanes(Axis(axis)))
+            Zip::from(self.lanes(axis))
                 .map_collect(|lane| unsafe { lane.uget(index).clone() })
                 .into()
         } else {
-            Zip::from(self.lanes(Axis(axis)))
+            Zip::from(self.lanes(axis))
                 .par_map_collect(|lane| unsafe { lane.uget(index).clone() })
                 .into()
         }
     }
 }
 
 impl<T, S: Data<Elem = T>> ArrBase<S, Ix1> {
```

### Comparing `teapy-0.1.6/src/arr/arr_func.rs` & `teapy-0.1.7/src/arr/arr_func.rs`

 * *Files 1% similar despite different names*

```diff
@@ -231,32 +231,33 @@
     pub fn not_nan(&self) -> Arr<bool, D>
     where
         T: Number,
     {
         self.mapv(|v| v.notnan())
     }
 
-    pub fn filter<S2>(&self, mask: &ArrBase<S2, Ix1>, axis: usize, par: bool) -> Arr<T, D>
+    pub fn filter<S2>(&self, mask: &ArrBase<S2, Ix1>, axis: i32, par: bool) -> Arr<T, D>
     where
         T: Default + Send + Sync + Clone,
         D: Dimension,
         S2: Data<Elem = bool> + Send + Sync,
     {
         let f_flag = !self.is_standard_layout();
         let mut new_dim = self.raw_dim();
+        let axis = self.norm_axis(axis);
         assert_eq!(
-            new_dim.slice()[axis],
+            new_dim.slice()[axis.index()],
             mask.len(),
             "Number of elements on the axis must equal to the length of mask array"
         );
-        new_dim.slice_mut()[axis] = mask.count_v_1d(true) as usize;
+        new_dim.slice_mut()[axis.index()] = mask.count_v_1d(true) as usize;
         let shape = new_dim.into_shape().set_f(f_flag);
         let mut out = Arr::<T, D>::default(shape);
         let mut out_wr = out.view_mut();
-        self.apply_along_axis(&mut out_wr, Axis(axis), par, |x_1d, out_1d| {
+        self.apply_along_axis(&mut out_wr, axis, par, |x_1d, out_1d| {
             x_1d.wrap().filter_1d(out_1d, mask.view())
         });
         out
     }
 
     /// Take value on a given axis and clone to a new array,
     ///
@@ -265,106 +266,110 @@
     ///
     /// # Safety
     ///
     /// The index in `slc` must be correct.
     pub unsafe fn take_clone_unchecked<S2>(
         &self,
         slc: ArrBase<S2, Ix1>,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Arr<T, D>
     where
         T: Clone + Default + Send + Sync,
         D: Dimension,
         S2: Data<Elem = usize> + Send + Sync,
     {
         let f_flag = !self.is_standard_layout();
+        let axis = self.norm_axis(axis);
         let mut new_dim = self.raw_dim();
-        new_dim.slice_mut()[axis] = slc.len();
+        new_dim.slice_mut()[axis.index()] = slc.len();
         let shape = new_dim.into_shape().set_f(f_flag);
         let mut out = Arr::<T, D>::default(shape);
         let mut out_wr = out.view_mut();
-        self.apply_along_axis(&mut out_wr, Axis(axis), par, |x_1d, out_1d| {
+        self.apply_along_axis(&mut out_wr, axis, par, |x_1d, out_1d| {
             x_1d.wrap().take_clone_1d_unchecked(out_1d, slc.view())
         });
         out
     }
 
     /// Take value on a given axis and clone to a new array,
     ///
     /// # Safety
     ///
     /// The index in `slc` must be correct.
     pub unsafe fn take_option_clone_unchecked<S2>(
         &self,
         slc: ArrBase<S2, Ix1>,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Arr<T, D>
     where
         T: Clone + Default + GetNone + Send + Sync,
         D: Dimension,
         S2: Data<Elem = Option<usize>> + Send + Sync,
     {
         let f_flag = !self.is_standard_layout();
+        let axis = self.norm_axis(axis);
         let mut new_dim = self.raw_dim();
-        new_dim.slice_mut()[axis] = slc.len();
+        new_dim.slice_mut()[axis.index()] = slc.len();
         let shape = new_dim.into_shape().set_f(f_flag);
         let mut out = Arr::<T, D>::default(shape);
         let mut out_wr = out.view_mut();
-        self.apply_along_axis(&mut out_wr, Axis(axis), par, |x_1d, out_1d| {
+        self.apply_along_axis(&mut out_wr, axis, par, |x_1d, out_1d| {
             x_1d.wrap()
                 .take_option_clone_1d_unchecked(out_1d, slc.view())
         });
         out
     }
 
     /// Take value on a given axis and clone to a new array,
     ///
     /// if you want to along axis, select arbitrary subviews corresponding to indices and and
     /// copy them into a new array, use select instead.
     ///
     /// This function is safe because the slice are checked.
-    pub fn take_clone<S2>(&self, slc: ArrBase<S2, Ix1>, axis: usize, par: bool) -> Arr<T, D>
+    pub fn take_clone<S2>(&self, slc: ArrBase<S2, Ix1>, axis: i32, par: bool) -> Arr<T, D>
     where
         T: Clone + Default + Send + Sync,
         D: Dimension,
         S2: Data<Elem = usize> + Send + Sync,
     {
-        let max_idx = self.shape()[axis] - 1;
+        let axis = self.norm_axis(axis);
+        let max_idx = self.shape()[axis.index()] - 1;
         assert!(slc.max_1d() <= max_idx, "The index to take is out of bound");
-        unsafe { self.take_clone_unchecked(slc, axis, par) }
+        unsafe { self.take_clone_unchecked(slc, axis.index() as i32, par) }
     }
 
     pub fn arg_partition(
         &self,
         kth: usize,
         sort: bool,
         rev: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Arr<i32, D>
     where
         T: Number + Send + Sync,
         D: Dimension,
     {
         let f_flag = !self.is_standard_layout();
         let mut new_dim = self.raw_dim();
-        if kth >= new_dim.slice_mut()[axis] {
+        let axis = self.norm_axis(axis);
+        if kth >= new_dim.slice_mut()[axis.index()] {
             panic!(
                 "kth(={}) out of bounds ({})",
                 kth,
-                new_dim.slice_mut()[axis]
+                new_dim.slice_mut()[axis.index()]
             )
         }
-        new_dim.slice_mut()[axis] = kth + 1;
+        new_dim.slice_mut()[axis.index()] = kth + 1;
         let shape = new_dim.into_shape().set_f(f_flag);
         let mut out = Arr::<i32, D>::default(shape);
         let mut out_wr = out.view_mut();
-        self.apply_along_axis(&mut out_wr, Axis(axis), par, |x_1d, out_1d| {
+        self.apply_along_axis(&mut out_wr, axis, par, |x_1d, out_1d| {
             x_1d.arg_partition_1d(out_1d, kth, sort, rev)
         });
         out
     }
 }
 
 impl_map_nd!(
```

### Comparing `teapy-0.1.6/src/arr/corr.rs` & `teapy-0.1.7/src/arr/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/datatype.rs` & `teapy-0.1.7/src/arr/datatype.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/export.rs` & `teapy-0.1.7/src/arr/export.rs`

 * *Files 17% similar despite different names*

```diff
@@ -4,12 +4,10 @@
 pub(super) use super::utils;
 pub(super) use super::utils::kh_sum;
 pub(super) use super::CollectTrustedToVec;
 pub(super) use super::{
     ArbArray, Arr, Arr1, ArrBase, ArrD, ArrOk, ArrViewD, ArrViewMutD, DataType, GetDataType,
     WrapNdarray,
 };
-pub(super) use ndarray::{
-    Axis, Data, DataMut, DimMax, Dimension, Ix1, RemoveAxis, ShapeBuilder, Zip,
-};
+pub(super) use ndarray::{Data, DataMut, DimMax, Dimension, Ix1, RemoveAxis, ShapeBuilder, Zip};
 pub(super) use num::traits::{AsPrimitive, MulAdd};
 pub(super) use std::iter::zip;
```

### Comparing `teapy-0.1.6/src/arr/groupby.rs` & `teapy-0.1.7/src/arr/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/impls/impl_1d_method.rs` & `teapy-0.1.7/src/arr/impls/impl_1d_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/impls/impl_linalg.rs` & `teapy-0.1.7/src/arr/impls/impl_linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/impls/impl_method.rs` & `teapy-0.1.7/src/arr/impls/impl_method.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use super::super::{Arr, ArrBase, ArrView, Data, RawData, WrapNdarray};
-use ndarray::{Axis, DataMut, DimMax, Dimension, ErrorKind, IntoDimension, ShapeError, Zip};
+use ndarray::{DataMut, DimMax, Dimension, ErrorKind, IntoDimension, ShapeError, Zip};
 // use std::fmt::Debug;
 
 type DimMaxOf<A, B> = <A as DimMax<B>>::Output;
 
 /// Create an iterator running multiple iterators in lockstep.
 ///
 /// The `izip!` iterator yields elements until any subiterator
@@ -197,24 +197,25 @@
 where
     S: Data<Elem = A>,
 {
     pub fn put_mask<S2, S3, D2, D3>(
         &mut self,
         mask: &ArrBase<S2, D2>,
         value: &ArrBase<S3, D3>,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) where
         A: Clone + Send + Sync,
         D2: Dimension,
         D3: Dimension,
         S: DataMut<Elem = A>,
         S2: Data<Elem = bool>,
         S3: Data<Elem = A>,
     {
+        let axis = self.norm_axis(axis);
         let value = if self.ndim() == value.ndim() && self.shape() == value.shape() {
             value.view().to_dim::<D>().unwrap()
         } else if let Some(value) = value.broadcast(self.raw_dim()) {
             value
         } else {
             // the number of value array's elements are equal to the number of true values in mask
             let mask = mask
@@ -224,23 +225,23 @@
             let value = value
                 .view()
                 .to_dim1()
                 .expect("value should be dim1 when set value to masked data");
             let true_num = mask.count_v_1d(true) as usize;
             assert_eq!(
                 true_num,
-                value.len_of(Axis(axis)),
+                value.len_of(axis),
                 "number of value are not equal to number of true mask"
             );
             let ndim = self.ndim();
             return if par && (ndim > 1) {
-                Zip::from(self.lanes_mut(Axis(axis)))
+                Zip::from(self.lanes_mut(axis))
                     .par_for_each(|x_1d| x_1d.wrap().put_mask_1d(&mask, &value));
             } else {
-                Zip::from(self.lanes_mut(Axis(axis)))
+                Zip::from(self.lanes_mut(axis))
                     .for_each(|x_1d| x_1d.wrap().put_mask_1d(&mask, &value));
             };
         };
         let mask = if self.ndim() == mask.ndim() && self.shape() == mask.shape() {
             mask.view().to_dim::<D>().unwrap()
         } else {
             mask.broadcast(self.raw_dim()).unwrap()
```

### Comparing `teapy-0.1.6/src/arr/impls/impl_numeric.rs` & `teapy-0.1.7/src/arr/impls/impl_numeric.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/iterators.rs` & `teapy-0.1.7/src/arr/iterators.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/join.rs` & `teapy-0.1.7/src/arr/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/lazy/auto_impl_own.rs` & `teapy-0.1.7/src/arr/lazy/auto_impl_own.rs`

 * *Files 8% similar despite different names*

```diff
@@ -53,68 +53,68 @@
     f64: AsPrimitive<T>,
 {
     // in1: lazy function with one input array,
     // mean -> f64: eager function name in Arr, and the dtype of output is f64
     // (stable: bool): other arguments of the function
     // impl_view_lazy!(in1, [remove_nan_1d -> f64], ());
     impl_view_lazy!(in1, [is_nan -> bool, not_nan -> bool], ());
-    impl_view_lazy!(in1, [diff -> f64, pct_change -> f64], (n: i32, axis: usize, par: bool));
+    impl_view_lazy!(in1, [diff -> f64, pct_change -> f64], (n: i32, axis: i32, par: bool));
     impl_view_lazy!(in1,
         [
             count_notnan -> i32, count_nan -> i32, median -> f64, max -> T,
             min -> T, prod -> T, cumprod -> T,
         ],
-        (axis: usize, par: bool)
+        (axis: i32, par: bool)
     );
     impl_view_lazy!(in1,
         [
             sum -> T, mean -> f64, var -> f64, std -> f64,
             skew -> f64, kurt -> f64, cumsum -> T,
         ],
-        (stable: bool, axis: usize, par: bool)
+        (stable: bool, axis: i32, par: bool)
     );
     impl_view_lazy!(in1-inplace,
         [
             zscore, zscore_inplace -> T,
         ],
-        (stable: bool, axis: usize, par: bool)
+        (stable: bool, axis: i32, par: bool)
     );
     impl_view_lazy!(in1-inplace,
         [
             winsorize, winsorize_inplace -> T,
         ],
-        (method: WinsorizeMethod, method_params: Option<f64>, stable: bool, axis: usize, par: bool)
+        (method: WinsorizeMethod, method_params: Option<f64>, stable: bool, axis: i32, par: bool)
     );
 
-    impl_view_lazy!(in1, quantile -> f64, (q: f64, method: QuantileMethod, axis: usize, par: bool));
-    impl_view_lazy!(in1, rank -> f64, (pct: bool, rev: bool, axis: usize, par: bool));
-    impl_view_lazy!(in1, argsort -> i32, (rev: bool, axis: usize, par: bool));
-    impl_view_lazy!(in1, split_group -> i32, (group: usize, rev: bool, axis: usize, par: bool));
-    impl_view_lazy!(in1, arg_partition -> i32, (kth: usize, sort: bool, rev: bool, axis: usize, par: bool));
-    impl_view_lazy!(in2, cov -> f64, (stable: bool, axis: usize, par: bool));
-    impl_view_lazy!(in2, corr -> f64, (method: CorrMethod, stable: bool, axis: usize, par: bool));
+    impl_view_lazy!(in1, quantile -> f64, (q: f64, method: QuantileMethod, axis: i32, par: bool));
+    impl_view_lazy!(in1, rank -> f64, (pct: bool, rev: bool, axis: i32, par: bool));
+    impl_view_lazy!(in1, argsort -> i32, (rev: bool, axis: i32, par: bool));
+    impl_view_lazy!(in1, split_group -> i32, (group: usize, rev: bool, axis: i32, par: bool));
+    impl_view_lazy!(in1, arg_partition -> i32, (kth: usize, sort: bool, rev: bool, axis: i32, par: bool));
+    impl_view_lazy!(in2, cov -> f64, (stable: bool, axis: i32, par: bool));
+    impl_view_lazy!(in2, corr -> f64, (method: CorrMethod, stable: bool, axis: i32, par: bool));
 
     // === window expression ===
     // window function without stable argument
     impl_view_lazy!(in1,
         [
             ts_argmin -> f64, ts_argmax -> f64, ts_min -> f64,
             ts_max -> f64, ts_rank -> f64, ts_rank_pct -> f64,
             ts_prod -> f64, ts_prod_mean -> f64, ts_minmaxnorm -> f64,
         ],
-        (window: usize, min_periods: usize, axis: usize, par: bool)
+        (window: usize, min_periods: usize, axis: i32, par: bool)
     );
     // window corr and cov
     impl_view_lazy!(in2, [ts_cov -> f64, ts_corr -> f64],
-        (window: usize, min_periods: usize, stable: bool, axis: usize, par: bool)
+        (window: usize, min_periods: usize, stable: bool, axis: i32, par: bool)
     );
     // window function with stable argument
     impl_view_lazy!(in1,
         [
             ts_sum -> f64, ts_sma -> f64, ts_ewm -> f64, ts_wma -> f64,
             ts_std -> f64, ts_var -> f64, ts_skew -> f64, ts_kurt -> f64,
             ts_stable -> f64, ts_meanstdnorm -> f64, ts_reg -> f64,
             ts_tsf -> f64, ts_reg_slope -> f64, ts_reg_intercept -> f64,
         ],
-        (window: usize, min_periods: usize, stable: bool, axis: usize, par: bool)
+        (window: usize, min_periods: usize, stable: bool, axis: i32, par: bool)
     );
 }
```

### Comparing `teapy-0.1.6/src/arr/lazy/expr_view.rs` & `teapy-0.1.7/src/arr/lazy/expr_view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/lazy/exprs.rs` & `teapy-0.1.7/src/arr/lazy/exprs.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/lazy/impl_cmp.rs` & `teapy-0.1.7/src/arr/lazy/impl_cmp.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/lazy/impl_ops.rs` & `teapy-0.1.7/src/arr/lazy/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/lazy/impl_own.rs` & `teapy-0.1.7/src/arr/lazy/impl_own.rs`

 * *Files 3% similar despite different names*

```diff
@@ -78,30 +78,30 @@
             .wrap()
             .to_dimd()
             .unwrap()
             .into()
         })
     }
 
-    pub fn count_v(self, value: T, axis: usize, par: bool) -> Expr<'a, i32>
+    pub fn count_v(self, value: T, axis: i32, par: bool) -> Expr<'a, i32>
     where
         T: Eq + Clone,
     {
         self.chain_view_f(move |arr| arr.count_v(value, axis, par).into())
     }
 
     // deep clone expression
     pub fn deep_copy(self) -> Self
     where
         T: Clone,
     {
         self.chain_view_f(move |arr| arr.to_owned().into())
     }
 
-    pub fn fillna<T2>(self, method: FillMethod, value: Option<T2>, axis: usize, par: bool) -> Self
+    pub fn fillna<T2>(self, method: FillMethod, value: Option<T2>, axis: i32, par: bool) -> Self
     where
         T: Number,
         T2: AsPrimitive<T> + Send + Sync,
         f64: AsPrimitive<T>,
     {
         self.chain_arr_f(move |arb_arr| {
             use ArbArray::*;
@@ -115,15 +115,15 @@
                     arr.view_mut().fillna_inplace(method, value, axis, par);
                     Owned(arr)
                 }
             }
         })
     }
 
-    pub fn clip<T2, T3>(self, min: T2, max: T3, axis: usize, par: bool) -> Self
+    pub fn clip<T2, T3>(self, min: T2, max: T3, axis: i32, par: bool) -> Self
     where
         T: Number,
         T2: Number + AsPrimitive<T>,
         T3: Number + AsPrimitive<T>,
     {
         // self.chain_view_f(move |arr| arr.clip(min, max, axis, par).into())
         self.chain_arr_f(move |arb_arr| {
@@ -138,23 +138,26 @@
                     arr.view_mut().clip_inplace(min, max, axis, par);
                     Owned(arr)
                 }
             }
         })
     }
 
-    pub fn last(self, axis: usize, par: bool) -> Self
+    pub fn last(self, axis: i32, par: bool) -> Self
     where
         T: Clone,
     {
-        self.no_dim0()
-            .chain_view_f(move |arr| arr.take_1_on_axis(arr.shape()[axis] - 1, axis, par).into())
+        self.no_dim0().chain_view_f(move |arr| {
+            let axis_n = arr.norm_axis(axis);
+            arr.take_1_on_axis(arr.shape()[axis_n.index()] - 1, axis, par)
+                .into()
+        })
     }
 
-    pub fn shift(self, n: i32, fill: Expr<'a, T>, axis: usize, par: bool) -> Self
+    pub fn shift(self, n: i32, fill: Expr<'a, T>, axis: i32, par: bool) -> Self
     where
         T: Clone,
     {
         self.chain_view_f(move |arr| {
             arr.shift(
                 n,
                 fill.eval()
@@ -350,31 +353,31 @@
     pub fn log(self, base: f64) -> Expr<'a, f64>
     where
         T: Number,
     {
         self.chain_view_f(move |arr| arr.mapv(|v| v.f64().log(base)).into())
     }
 
-    pub fn valid_last(self, axis: usize, par: bool) -> Self
+    pub fn valid_last(self, axis: i32, par: bool) -> Self
     where
         T: Number,
         f64: AsPrimitive<T>,
     {
         self.chain_view_f(move |arr| arr.valid_last(axis, par).into())
     }
 
-    pub fn first(self, axis: usize, par: bool) -> Self
+    pub fn first(self, axis: i32, par: bool) -> Self
     where
         T: Clone,
     {
         self.no_dim0()
             .chain_view_f(move |arr| arr.take_1_on_axis(0, axis, par).into())
     }
 
-    pub fn valid_first(self, axis: usize, par: bool) -> Self
+    pub fn valid_first(self, axis: i32, par: bool) -> Self
     where
         T: Number,
         f64: AsPrimitive<T>,
     {
         self.chain_view_f(move |arr| arr.valid_first(axis, par).into())
     }
 
@@ -438,15 +441,15 @@
             let df1 = *df1.eval().view_arr().to_dim0().unwrap().into_scalar();
             let df2 = *df2.eval().view_arr().to_dim0().unwrap().into_scalar();
             let n = FisherSnedecor::new(df1, df2).unwrap();
             arr.map(|v| n.cdf(v.f64())).into()
         })
     }
 
-    pub fn filter(self, mask: Expr<'a, bool>, axis: Expr<'a, usize>, par: bool) -> Self
+    pub fn filter(self, mask: Expr<'a, bool>, axis: Expr<'a, i32>, par: bool) -> Self
     where
         T: Clone,
     {
         self.chain_view_f(move |arr| {
             arr.filter(
                 &mask
                     .eval()
@@ -461,15 +464,15 @@
                     .into_scalar(),
                 par,
             )
             .into()
         })
     }
 
-    pub fn dropna<'b: 'a>(self, axis: Expr<'a, usize>, how: DropNaMethod, par: bool) -> Self
+    pub fn dropna<'b: 'a>(self, axis: Expr<'a, i32>, how: DropNaMethod, par: bool) -> Self
     where
         T: Clone + Number,
     {
         self.chain_view_f(move |arr| {
             let ndim = arr.ndim();
             let axis = *axis
                 .eval()
@@ -483,32 +486,33 @@
                     .unwrap()
                     .remove_nan_1d()
                     .to_dimd()
                     .unwrap()
                     .into(),
                 2 => {
                     let arr = arr.to_dim2().unwrap();
-                    let mask = match (axis, how) {
-                        (0, DropNaMethod::Any) => arr.not_nan().all(1, par),
-                        (0, DropNaMethod::All) => arr.not_nan().any(1, par),
-                        (1, DropNaMethod::Any) => arr.not_nan().all(0, par),
-                        (1, DropNaMethod::All) => arr.not_nan().any(0, par),
+                    let axis_n = arr.norm_axis(axis);
+                    let mask = match (axis_n, how) {
+                        (Axis(0), DropNaMethod::Any) => arr.not_nan().all(1, par),
+                        (Axis(0), DropNaMethod::All) => arr.not_nan().any(1, par),
+                        (Axis(1), DropNaMethod::Any) => arr.not_nan().all(0, par),
+                        (Axis(1), DropNaMethod::All) => arr.not_nan().any(0, par),
                         _ => panic!("axis should be 0 or 1 and how should be any or all"),
                     };
                     arr.filter(&mask, axis, par).to_dimd().unwrap().into()
                 }
                 dim => unimplemented!(
                     "dropna only support 1d and 2d array currently, but the array is dim {dim}"
                 ),
             }
         })
     }
 
     /// select on a given axis by a slice expression
-    pub fn select_on_axis_by_expr(self, slc: Expr<'a, usize>, axis: Expr<'a, usize>) -> Self
+    pub fn select_on_axis_by_expr(self, slc: Expr<'a, usize>, axis: Expr<'a, i32>) -> Self
     where
         T: Clone,
     {
         self.chain_view_f(move |arr| {
             let slc = slc.no_dim0().eval();
             let slc_eval = slc.view_arr();
             let axis = *axis
@@ -517,29 +521,66 @@
                 .to_dim0()
                 .expect("axis should be dim 0")
                 .into_scalar();
             assert!(
                 slc_eval.ndim() <= 1,
                 "The slice must be dim 0 or dim 1 when select on axis"
             );
+            let axis = arr.norm_axis(axis);
             if slc_eval.len() == 1 {
-                arr.index_axis(Axis(axis), slc_eval.to_dim1().unwrap()[0])
+                arr.index_axis(axis, slc_eval.to_dim1().unwrap()[0])
                     .to_owned()
                     .wrap()
                     .into()
             } else {
-                arr.select(Axis(axis), slc_eval.as_slice().unwrap())
-                    .wrap()
-                    .into()
+                arr.select(axis, slc_eval.as_slice().unwrap()).wrap().into()
+            }
+        })
+    }
+
+    /// select on a given axis by a slice expression
+    pub fn select_on_axis_by_i32_expr(self, slc: Expr<'a, i32>, axis: Expr<'a, i32>) -> Self
+    where
+        T: Clone,
+    {
+        self.chain_view_f(move |arr| {
+            let slc = slc.no_dim0().eval();
+            let slc_eval = slc.view_arr();
+            let axis = *axis
+                .eval()
+                .view_arr()
+                .to_dim0()
+                .expect("axis should be dim 0")
+                .into_scalar();
+            assert!(
+                slc_eval.ndim() <= 1,
+                "The slice must be dim 0 or dim 1 when select on axis"
+            );
+            let axis = arr.norm_axis(axis);
+            let length = arr.len_of(axis);
+            if slc_eval.len() == 1 {
+                arr.index_axis(
+                    axis,
+                    arr.ensure_index(slc_eval.to_dim1().unwrap()[0], length),
+                )
+                .to_owned()
+                .wrap()
+                .into()
+            } else {
+                let slc = slc_eval
+                    .to_dim1()
+                    .unwrap()
+                    .mapv(|i| arr.ensure_index(i, length));
+                arr.select(axis, slc.as_slice().unwrap()).wrap().into()
             }
         })
     }
 
     /// take values on a given axis
-    pub fn take_on_axis_by_expr(self, slc: Expr<'a, usize>, axis: usize, par: bool) -> Self
+    pub fn take_on_axis_by_expr(self, slc: Expr<'a, usize>, axis: i32, par: bool) -> Self
     where
         T: Clone,
     {
         self.chain_view_f(move |arr| {
             let slc = slc.no_dim0().eval();
             let slc_eval = slc.view_arr();
             assert!(
@@ -560,15 +601,15 @@
     ///
     /// # Safety
     ///
     /// The slice should be valid.
     pub unsafe fn take_on_axis_by_expr_unchecked(
         self,
         slc: Expr<'a, usize>,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self
     where
         T: Clone,
     {
         self.chain_view_f(move |arr| {
             let slc = slc.no_dim0().eval();
@@ -591,15 +632,15 @@
     ///
     /// # Safety
     ///
     /// The index in slc must be correct.
     pub unsafe fn take_option_on_axis_by_expr_unchecked(
         self,
         slc: Expr<'a, Option<usize>>,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self
     where
         T: Clone + GetNone,
     {
         self.chain_view_f(move |arr| {
             let slc = slc.no_dim0().eval();
@@ -641,78 +682,84 @@
     pub fn shape(self) -> Expr<'a, usize> {
         self.chain_view_f(move |arr| {
             let shape = arr.shape().to_owned();
             Arr1::from_vec(shape).to_dimd().unwrap().into()
         })
     }
 
-    pub fn concat(self, other: Vec<Expr<'a, T>>, axis: usize) -> Expr<'a, T>
+    pub fn concat(self, other: Vec<Expr<'a, T>>, axis: i32) -> Expr<'a, T>
     where
         T: Clone,
     {
         self.no_dim0().chain_view_f(move |arr| {
             // evaluate in parallel
+            let axis = arr.norm_axis(axis);
             let mut other: Vec<Expr<'a, T>> =
                 other.into_iter().map(|e| e.no_dim0()).collect_trusted();
             other.par_iter_mut().for_each(|e| e.eval_inplace());
             let arr1 = vec![arr.0];
             // safety: array view other exists in lifetime '_, and concatenate will create a own array later
             let arrays: Vec<ArrayViewD<'_, T>> = unsafe {
                 arr1.into_iter()
                     .chain(other.iter().map(|e| mem::transmute(e.view().into_arr().0)))
                     .collect()
             };
-            ndarray::concatenate(Axis(axis), &arrays)
+            ndarray::concatenate(axis, &arrays)
                 .expect("Shape error when concatenate")
                 .wrap()
                 .into()
         })
     }
 
-    pub fn stack(self, mut other: Vec<Expr<'a, T>>, axis: usize) -> Expr<'a, T>
+    pub fn stack(self, mut other: Vec<Expr<'a, T>>, axis: i32) -> Expr<'a, T>
     where
         T: Clone,
     {
         self.chain_view_f(move |arr| {
             // evaluate in parallel
+            let axis = if axis < 0 {
+                Axis(arr.norm_axis(axis).index() + 1)
+            } else {
+                Axis(axis as usize)
+            };
             other.par_iter_mut().for_each(|e| e.eval_inplace());
             let arr1 = vec![arr.0];
             // safety: array view other exists in lifetime '_, and stack will create a own array later
             let arrays: Vec<ArrayViewD<'_, T>> = unsafe {
                 arr1.into_iter()
                     .chain(other.iter().map(|e| mem::transmute(e.view().into_arr().0)))
                     .collect()
             };
-            ndarray::stack(Axis(axis), &arrays)
-                .expect("Shape error when concatenate")
+            ndarray::stack(axis, &arrays)
+                .expect("Shape error when stack")
                 .wrap()
                 .into()
         })
     }
 
-    // pub fn apply_on_vec_arr<F>(self, func: F, axis: usize) -> Expr<'a, T>
+    // pub fn apply_on_vec_arr<F>(self, func: F, axis: i32) -> Expr<'a, T>
     // {
     //     self.chain_f(|input| {
     //         if let ExprOut::ArrVec(arr_vec) = input {
     //             let view_vec = arr_vec.iter().map(|arr| arr.view()).collect_trusted();
     //             use ndarray::Zip;
     //             let shape =
     //             let out = Vec::with_capacity(arr_vec.len());
     //         }
 
     //     })
     // }
 }
 
 impl<'a> Expr<'a, bool> {
-    pub fn any(self, axis: usize, par: bool) -> Self {
+    pub fn any(self, axis: i32, par: bool) -> Self {
         self.chain_view_f(move |arr| arr.any(axis, par).into())
     }
 
-    pub fn all(self, axis: usize, par: bool) -> Self {
+    pub fn all(self, axis: i32, par: bool) -> Self {
         self.chain_view_f(move |arr| arr.all(axis, par).into())
     }
 }
 
 impl<'a> Expr<'a, PyValue> {
     pub fn object_to_string(self, py: Python) -> Expr<'a, String> {
         let e = self.eval();
```

### Comparing `teapy-0.1.6/src/arr/lazy/impl_view.rs` & `teapy-0.1.7/src/arr/lazy/impl_view.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 //! impl methods that may return an array view.
 //! these method are unsafe because the data of the array
 //! view should not be dropped.
 //! the memory should be managed on python heap if using in python.
 
-use super::super::{ArbArray, Axis, WrapNdarray};
+use super::super::{ArbArray, WrapNdarray};
 use super::{Expr, ExprElement};
 use ndarray::{s, IxDyn, NewAxis, SliceInfo, SliceInfoElem};
 use std::marker::PhantomData;
 use std::mem;
 
 impl<'a, T> Expr<'a, T>
 where
@@ -193,19 +193,20 @@
     /// Swap axes ax and bx.
     ///
     /// This does not move any data, it just adjusts the array’s dimensions and strides.
     ///
     /// # Safety
     ///
     /// the data for the array view should exist
-    pub unsafe fn swap_axes(self, ax: usize, bx: usize) -> Self {
+    pub unsafe fn swap_axes(self, ax: i32, bx: i32) -> Self {
         self.chain_view_out_f(move |arr| {
+            let ax = arr.norm_axis(ax);
+            let bx = arr.norm_axis(bx);
             let mut arr = arr.0;
-            arr.swap_axes(ax, bx);
-            // let out: ArbArray<'_, T> = arr.wrap().into();
+            arr.swap_axes(ax.index(), bx.index());
             let out = arr.wrap();
             mem::transmute(out)
         })
     }
 
     /// Permute the axes.
     ///
@@ -231,65 +232,53 @@
     }
 
     /// Insert new array axis at axis and return the result.
     ///
     /// # Safety
     ///
     /// the data for the array view should exist
-    pub unsafe fn insert_axis(self, axis: usize) -> Self {
+    pub unsafe fn insert_axis(self, axis: i32) -> Self {
         self.chain_view_out_f(move |arr| {
-            // let out: ArbArray<'_, T> = arr.0.insert_axis(Axis(axis)).wrap().into();
-            let out = arr.0.insert_axis(Axis(axis)).wrap();
+            let axis = arr.norm_axis(axis);
+            let out = arr.0.insert_axis(axis).wrap();
             mem::transmute(out)
         })
     }
 
     /// Remove new array axis at axis and return the result.
     ///
     /// # Safety
     ///
     /// the data for the array view should exist
-    pub unsafe fn remove_axis(self, axis: usize) -> Self {
+    pub unsafe fn remove_axis(self, axis: i32) -> Self {
         self.chain_view_out_f(move |arr| {
-            // let out: ArbArray<'_, T> = arr.0.remove_axis(Axis(axis)).wrap().into();
-            let out = arr.0.remove_axis(Axis(axis)).wrap();
+            let axis = arr.norm_axis(axis);
+            let out = arr.0.remove_axis(axis).wrap();
             mem::transmute(out)
         })
     }
 
     /// # Safety
     ///
     /// the data for the array view should exist
     pub unsafe fn broadcast(self, shape: Expr<'a, usize>) -> Self {
         self.chain_view_out_f(move |arr| {
             let shape = shape.eval();
             let sh = shape.view_arr();
             let ndim = sh.ndim();
             if ndim == 0 {
                 let shape = sh.to_dim0().unwrap().into_scalar();
-                // let out: ArbArray<'_, T> = arr
-                //     .broadcast(*shape)
-                //     .expect("broadcast error")
-                //     .to_dimd()
-                //     .unwrap()
-                //     .into();
                 let out = arr
                     .broadcast(*shape)
                     .expect("broadcast error")
                     .to_dimd()
                     .unwrap();
                 mem::transmute(out)
             } else if ndim == 1 {
                 let shape = sh.to_dim1().unwrap();
-                // let out: ArbArray<'_, T> = arr
-                //     .broadcast(shape.to_slice().unwrap())
-                //     .expect("broadcast error")
-                //     .to_dimd()
-                //     .unwrap()
-                //     .into();
                 let out = arr
                     .broadcast(shape.to_slice().unwrap())
                     .expect("broadcast error")
                     .to_dimd()
                     .unwrap();
                 mem::transmute(out)
             } else {
```

### Comparing `teapy-0.1.6/src/arr/lazy/linalg.rs` & `teapy-0.1.7/src/arr/lazy/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/lazy/mod.rs` & `teapy-0.1.7/src/arr/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/macros.rs` & `teapy-0.1.7/src/arr/macros.rs`

 * *Files 7% similar despite different names*

```diff
@@ -39,23 +39,24 @@
         impl<T: Clone, S, D> ArrBase<S, D>
         where
             S: Data<Elem = T>,
             D: Dimension,
         {
              // make 1d function can be used in ndarray
             $(#[$meta])*
-            pub fn $func $(<$($t),*>)? (&$self $(, $p: $p_ty)*, axis: usize, par: bool) -> Arr<$otype, D::Smaller>
+            pub fn $func $(<$($t),*>)? (&$self $(, $p: $p_ty)*, axis: i32, par: bool) -> Arr<$otype, D::Smaller>
             where
                 D: RemoveAxis,
                 $($generic: $bound $(+ $other_bnd)*,)*
             {
+                let axis = $self.norm_axis(axis);
                 if !par {
-                    Zip::from($self.lanes(Axis(axis))).map_collect(move |lane| lane.wrap().$func_1d($($p.clone()),*)).into()
+                    Zip::from($self.lanes(axis)).map_collect(move |lane| lane.wrap().$func_1d($($p.clone()),*)).into()
                 } else {
-                    Zip::from($self.lanes(Axis(axis))).par_map_collect(move |lane| lane.wrap().$func_1d($($p.clone()),*)).into()
+                    Zip::from($self.lanes(axis)).par_map_collect(move |lane| lane.wrap().$func_1d($($p.clone()),*)).into()
                 }
             }
         }
 
 
     };
 }
@@ -85,23 +86,24 @@
         impl<T, S, D> ArrBase<S, D>
         where
             T: Default + Clone,
             S: Data<Elem = T>,
             D: Dimension,
         {
             $(#[$meta])*
-            pub fn $func $(<$($t),*>)? (&$self $(, $p: $p_ty)*, axis: usize, par: bool) -> Arr<$otype, D>
+            pub fn $func $(<$($t),*>)? (&$self $(, $p: $p_ty)*, axis: i32, par: bool) -> Arr<$otype, D>
             where
                 $($generic: $bound $(+ $other_bnd)*,)*
             {
+                let axis = $self.norm_axis(axis);
                 let f_flag = !$self.is_standard_layout();
                 let shape = $self.raw_dim().into_shape().set_f(f_flag);
                 let mut out = Arr::<$otype, D>::default(shape);
                 let mut out_wr = out.view_mut();
-                $self.apply_along_axis(&mut out_wr, Axis(axis), par, move |x_1d, mut out_1d| {
+                $self.apply_along_axis(&mut out_wr, axis, par, move |x_1d, mut out_1d| {
                     x_1d.$func_1d(&mut out_1d $(,$p.clone())*)
                 });
                 out
             }
         }
     };
 
@@ -126,23 +128,24 @@
         impl<T, S, D> ArrBase<S, D>
         where
             T: Default + Clone,
             S: Data<Elem = T>,
             D: Dimension,
         {
             $(#[$meta])*
-            pub unsafe fn $func $(<$($t),*>)? (&$self $(, $p: $p_ty)*, axis: usize, par: bool) -> Arr<$otype, D>
+            pub unsafe fn $func $(<$($t),*>)? (&$self $(, $p: $p_ty)*, axis: i32, par: bool) -> Arr<$otype, D>
             where
                 $($generic: $bound $(+ $other_bnd)*,)*
             {
+                let axis = $self.norm_axis(axis);
                 let f_flag = !$self.is_standard_layout();
                 let shape = $self.raw_dim().into_shape().set_f(f_flag);
                 let mut out = Arr::<$otype, D>::default(shape);
                 let mut out_wr = out.view_mut();
-                $self.apply_along_axis(&mut out_wr, Axis(axis), par, |x_1d, mut out_1d| {
+                $self.apply_along_axis(&mut out_wr, axis, par, |x_1d, mut out_1d| {
                     x_1d.$func_1d(&mut out_1d $(,$p.clone())*)
                 });
                 out
             }
         }
     };
 }
@@ -170,29 +173,29 @@
         }
         impl<T: Clone, S, D> ArrBase<S, D>
         where
             S: Data<Elem = T>,
             D: Dimension,
         {
             $(#[$meta])*
-            pub fn $func $(<S2, D2 $(,$t)*>)? (&$self, $other: &ArrBase<S2, D2> $(, $p: $p_ty)*, axis: usize, par: bool) -> Arr<$otype, <<D as DimMax<D2>>::Output as Dimension>::Smaller>
+            pub fn $func $(<S2, D2 $(,$t)*>)? (&$self, $other: &ArrBase<S2, D2> $(, $p: $p_ty)*, axis: i32, par: bool) -> Arr<$otype, <<D as DimMax<D2>>::Output as Dimension>::Smaller>
             where
                 D: DimMax<D2> + RemoveAxis,
                 D2: Dimension,
                 $($generic: $bound $(+ $other_bnd)*,)*
             {
                 let (lhs, rhs) = if $self.ndim() == $other.ndim() && $self.shape() == $other.shape() {
                     let lhs = $self.view().to_dim::<<D as DimMax<D2>>::Output>().unwrap();
                     let rhs = $other.view().to_dim::<<D as DimMax<D2>>::Output>().unwrap();
                     (lhs, rhs)
                 } else {
                     $self.broadcast_with(&$other).unwrap()
                 };
 
-                let axis = Axis(axis);
+                let axis = lhs.norm_axis(axis);
                 if !par {
                     Zip::from(lhs.lanes(axis)).and(rhs.lanes(axis)).map_collect(|lane1, lane2| lane1.wrap().$func_1d(&lane2.wrap() $(,$p.clone())*)).into()
                 } else {
                     Zip::from(lhs.lanes(axis)).and(rhs.lanes(axis)).par_map_collect(|lane1, lane2| lane1.wrap().$func_1d(&lane2.wrap() $(,$p.clone())*)).into()
                 }
             }
         }
@@ -226,34 +229,34 @@
         impl<T, S, D> ArrBase<S, D>
         where
             T: Default + Clone,
             S: Data<Elem = T>,
             D: Dimension,
         {
             $(#[$meta])*
-            pub fn $func $(<S2, D2, T2 $(,$t)*>)? (&$self, $other: &ArrBase<S2, D2> $(, $p: $p_ty)*, axis: usize, par: bool) -> Arr<$otype, <D as DimMax<D2>>::Output>
+            pub fn $func $(<S2, D2, T2 $(,$t)*>)? (&$self, $other: &ArrBase<S2, D2> $(, $p: $p_ty)*, axis: i32, par: bool) -> Arr<$otype, <D as DimMax<D2>>::Output>
             where
                 S2: Data<Elem = T2>,
                 D: DimMax<D2>,
                 D2: Dimension,
                 $($generic: $bound $(+ $other_bnd)*,)*
             {
                 let f_flag = !$self.is_standard_layout();
                 let (lhs, rhs) = if $self.ndim() == $other.ndim() && $self.shape() == $other.shape() {
                     let lhs = $self.view().to_dim::<<D as DimMax<D2>>::Output>().unwrap();
                     let rhs = $other.view().to_dim::<<D as DimMax<D2>>::Output>().unwrap();
                     (lhs, rhs)
                 } else {
                     $self.broadcast_with(&$other).unwrap()
                 };
+                let axis = lhs.norm_axis(axis);
                 let shape = lhs.raw_dim().into_shape().set_f(f_flag);
-                // let shape = $self.raw_dim().into_shape().set_f(f_flag);
                 let mut out = Arr::<$otype, <D as DimMax<D2>>::Output>::default(shape);
                 let mut out_wr = out.view_mut();
-                lhs.apply_along_axis_with(rhs, &mut out_wr, Axis(axis), par, |x_1d, y_1d, mut out_1d| {
+                lhs.apply_along_axis_with(rhs, &mut out_wr, axis, par, |x_1d, y_1d, mut out_1d| {
                     x_1d.$func_1d(&y_1d, &mut out_1d $(,$p.clone())*)
                 });
                 out
             }
         }
     };
 }
@@ -281,19 +284,19 @@
         }
         impl<T: Clone, S, D> ArrBase<S, D>
         where
             S: DataMut<Elem = T>,
             D: Dimension,
         {
             $(#[$meta])*
-            pub fn $func $(<$($t),*>)? (&mut $self $(, $p: $p_ty)*, axis: usize, par: bool)
+            pub fn $func $(<$($t),*>)? (&mut $self $(, $p: $p_ty)*, axis: i32, par: bool)
             where
                 $($generic: $bound $(+ $other_bnd)*,)*
             {
-                let axis = Axis(axis);
+                let axis = $self.norm_axis(axis);
                 if !par {
                     Zip::from($self.lanes_mut(axis)).for_each(|lane| lane.wrap().$func_1d($($p.clone()),*)).into()
                 } else {
                     Zip::from($self.lanes_mut(axis)).par_for_each(|lane| lane.wrap().$func_1d($($p.clone()),*)).into()
                 }
             }
         }
```

### Comparing `teapy-0.1.6/src/arr/mod.rs` & `teapy-0.1.7/src/arr/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -21,34 +21,35 @@
 pub mod utils;
 
 pub use agg::QuantileMethod;
 pub use arr_func::{FillMethod, WinsorizeMethod};
 pub use corr::CorrMethod;
 pub(crate) use datatype::match_datatype_arm;
 pub use datatype::{BoolType, DataType, GetDataType, GetNone, Number};
-pub use groupby::{groupby, groupby_par};
+pub use groupby::{flatten, groupby, groupby_par};
 pub use iterators::{Iter, IterMut};
 pub use join::{join_left, JoinType};
 pub use util_trait::{CollectTrusted, CollectTrustedToVec, TrustedLen};
 pub use utils::{kh_sum, DefaultNew, EmptyNew};
 
 #[cfg(feature = "lazy")]
 pub use lazy::{DropNaMethod, Expr, ExprElement, ExprOut, ExprOutView, Exprs};
 
 pub use time::{DateTime, TimeDelta, TimeUnit};
 
 use ndarray::{
-    Array, Array1, ArrayBase, Axis, Data, DataMut, DataOwned, Dimension, Ix0, Ix1, Ix2, IxDyn,
-    OwnedRepr, RawArrayView, RawArrayViewMut, RawData, RawDataClone, RemoveAxis, ShapeBuilder,
-    ShapeError, StrideShape, ViewRepr, Zip,
+    Array, Array1, ArrayBase, ArrayD, Axis, Data, DataMut, DataOwned, Dimension, Ix0, Ix1, Ix2,
+    IxDyn, OwnedRepr, RawArrayView, RawArrayViewMut, RawData, RawDataClone, RemoveAxis,
+    ShapeBuilder, ShapeError, StrideShape, ViewRepr, Zip,
 };
 use ndarray_npy::{write_npy, WritableElement, WriteNpyError};
 use num::{traits::AsPrimitive, Zero};
 use pyo3::{Python, ToPyObject};
 use rayon::prelude::{IntoParallelIterator, ParallelIterator};
+use serde::{Deserialize, Deserializer, Serialize, Serializer};
 use std::fmt::Debug;
 use std::sync::Arc;
 
 pub struct ArrBase<S, D>(pub ArrayBase<S, D>)
 where
     S: RawData;
 
@@ -72,14 +73,37 @@
     D: Dimension,
 {
     #[inline]
     pub fn new(a: ArrayBase<S, D>) -> Self {
         Self(a)
     }
 
+    #[inline]
+    pub fn ensure_axis(&self, axis: i32) -> usize {
+        if axis < 0 {
+            (self.ndim() as i32 + axis) as usize
+        } else {
+            axis as usize
+        }
+    }
+
+    #[inline]
+    pub fn norm_axis(&self, axis: i32) -> Axis {
+        Axis(self.ensure_axis(axis))
+    }
+
+    #[inline]
+    pub fn ensure_index(&self, index: i32, length: usize) -> usize {
+        if index < 0 {
+            (length as i32 + index) as usize
+        } else {
+            index as usize
+        }
+    }
+
     pub fn write_npy<P>(self, path: P) -> Result<(), WriteNpyError>
     where
         P: AsRef<std::path::Path>,
         T: WritableElement,
         S: Data,
     {
         write_npy(path, &self.0)
@@ -538,14 +562,44 @@
 #[derive(Debug)]
 pub enum ArbArray<'a, T> {
     View(ArrViewD<'a, T>),
     ViewMut(ArrViewMutD<'a, T>),
     Owned(ArrD<T>),
 }
 
+impl<'a, T> Serialize for ArbArray<'a, T>
+where
+    T: Serialize + Clone,
+{
+    fn serialize<Se>(&self, serializer: Se) -> Result<Se::Ok, Se::Error>
+    where
+        Se: Serializer,
+    {
+        match self {
+            ArbArray::View(arr_view) => arr_view.to_owned().serialize(serializer),
+            ArbArray::ViewMut(arr_view) => arr_view.to_owned().serialize(serializer),
+            ArbArray::Owned(arr) => arr.serialize(serializer),
+        }
+    }
+}
+
+impl<'a, 'de, T> Deserialize<'de> for ArbArray<'a, T>
+where
+    T: Deserialize<'de> + Clone,
+{
+    fn deserialize<D>(deserializer: D) -> Result<ArbArray<'a, T>, D::Error>
+    where
+        D: Deserializer<'de>,
+    {
+        Ok(ArbArray::<T>::Owned(
+            ArrayD::<T>::deserialize(deserializer)?.wrap(),
+        ))
+    }
+}
+
 impl<'a, T: Default> Default for ArbArray<'a, T> {
     fn default() -> Self {
         ArbArray::Owned(Default::default())
     }
 }
 
 // impl<'a, T: Clone> Clone for ArbArray<'a, T> {
```

### Comparing `teapy-0.1.6/src/arr/time.rs` & `teapy-0.1.7/src/arr/time.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 use chrono::{Datelike, Duration, Months, NaiveDateTime};
 use ndarray::ScalarOperand;
 use numpy::{
     datetime::{Datetime as NPDatetime, Unit as NPUnit},
     npyffi::NPY_DATETIMEUNIT,
 };
 use pyo3::prelude::*;
+use serde::{Deserialize, Serialize};
 use std::{
     cmp::Ordering,
     hash::Hash,
     ops::{Add, Deref, Div, Mul, Neg, Sub},
 };
 
 /// The number of nanoseconds in a microsecond.
@@ -26,15 +27,15 @@
 /// The number of seconds in an hour.
 const SECS_PER_HOUR: i64 = 3600;
 /// The number of (non-leap) seconds in days.
 const SECS_PER_DAY: i64 = 86400;
 /// The number of (non-leap) seconds in a week.
 const SECS_PER_WEEK: i64 = 604800;
 
-#[derive(Clone, Copy, Default, Debug, Hash, Eq, PartialEq, PartialOrd)]
+#[derive(Clone, Copy, Default, Debug, Hash, Eq, PartialEq, PartialOrd, Serialize, Deserialize)]
 pub struct DateTime(pub NaiveDateTime);
 
 impl Deref for DateTime {
     type Target = NaiveDateTime;
     fn deref(&self) -> &Self::Target {
         &self.0
     }
@@ -192,17 +193,19 @@
 
 // impl Default for TimeUnit {
 //     fn default() -> Self {
 //         TimeUnit::Millisecond
 //     }
 // }
 
-#[derive(Clone, Debug, Hash, Eq, PartialEq)]
+#[serde_with::serde_as]
+#[derive(Clone, Debug, Hash, Eq, PartialEq, Serialize, Deserialize)]
 pub struct TimeDelta {
     pub months: i32,
+    #[serde_as(as = "serde_with::DurationSeconds<i64>")]
     pub inner: Duration,
 }
 
 impl Default for TimeDelta {
     fn default() -> Self {
         Self {
             months: 0,
```

### Comparing `teapy-0.1.6/src/arr/util_trait.rs` & `teapy-0.1.7/src/arr/util_trait.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/utils/algos.rs` & `teapy-0.1.7/src/arr/utils/algos.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/utils/alloc.rs` & `teapy-0.1.7/src/arr/utils/alloc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/window/compare.rs` & `teapy-0.1.7/src/arr/window/compare.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/window/corr.rs` & `teapy-0.1.7/src/arr/window/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/window/feature.rs` & `teapy-0.1.7/src/arr/window/feature.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/window/norm.rs` & `teapy-0.1.7/src/arr/window/norm.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/arr/window/reg.rs` & `teapy-0.1.7/src/arr/window/reg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/equity.rs` & `teapy-0.1.7/src/equity.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/from_py.rs` & `teapy-0.1.7/src/from_py.rs`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,34 @@
     JoinType,
 };
 use numpy::{
     datetime::{units, Datetime},
     Element, PyArray, PyArray1, PyArrayDescr, PyArrayDyn,
 };
 use pyo3::{exceptions::PyValueError, FromPyObject, PyAny, PyObject, PyResult, Python, ToPyObject};
+// use serde::{Serialize, Deserialize, Serializer};
 
 #[cfg(feature = "lazy")]
 use crate::arr::DropNaMethod;
 use crate::arr::{CorrMethod, FillMethod, QuantileMethod, WinsorizeMethod};
 
 #[derive(Debug, Clone)]
 #[repr(transparent)]
 pub struct PyValue(pub PyObject);
 
+// impl Serialize for PyValue {
+//     fn serialize<S: Serializer>(&self, serializer: S) -> Result<S::Ok, S::Error>
+//     {
+//         Python::with_gil(|py| {
+//             let obj = self.0.as_ref(py);
+//             serde_pickle::to_vec(&obj, Default::default())
+//         })
+//     }
+// }
+
 impl ToPyObject for PyValue {
     fn to_object(&self, py: Python<'_>) -> PyObject {
         self.0.to_object(py)
     }
 }
 
 impl Default for PyValue {
```

### Comparing `teapy-0.1.6/src/pylazy/datadict.rs` & `teapy-0.1.7/src/pylazy/datadict.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 use pyo3::exceptions::PyTypeError;
+use regex::Regex;
+use std::cmp::Ordering;
 use std::collections::hash_map::RawEntryMut;
 use std::iter::repeat;
 use std::sync::{Arc, Mutex};
 
 use crate::arr::{join_left, JoinType};
 
 use super::export::*;
@@ -59,14 +61,19 @@
 
     #[inline(always)]
     pub fn len(&self) -> usize {
         self.data.len()
     }
 
     #[inline(always)]
+    pub fn into_data(self) -> Vec<PyExpr> {
+        self.data
+    }
+
+    #[inline(always)]
     pub fn is_empty(&self) -> bool {
         self.len() == 0
     }
 
     // fn create_column_map(&mut self) {
     //     let mut column_map = HashMap::<String, usize>::with_capacity(self.data.len());
     //     let mut name_auto = 0;
@@ -112,33 +119,37 @@
     /// Copy the column map
     pub fn map_to_own(&mut self) {
         let map = self.column_map.lock().unwrap().clone();
         self.column_map = Arc::new(Mutex::new(map));
     }
 
     pub fn _drop(&mut self, columns: Vec<&str>, inplace: bool) -> Option<Self> {
+        let columns: Vec<String> = columns
+            .into_iter()
+            .flat_map(|col| self.get_matched_regex_column(col))
+            .collect();
         if inplace {
             let mut column_map = self.column_map.lock().unwrap();
             for col in &columns {
-                column_map.remove(*col);
+                column_map.remove(col);
             }
             self.data = self
                 .data
-                .drain_filter(|e| !columns.contains(&e.get_name().unwrap().as_str()))
+                .drain_filter(|e| !columns.contains(&e.get_name().unwrap()))
                 .collect::<Vec<_>>();
             None
         } else {
             let mut column_map = self.column_map.lock().unwrap().clone();
             for col in &columns {
-                column_map.remove(*col);
+                column_map.remove(col);
             }
             let data = self
                 .data
                 .clone()
-                .drain_filter(|e| !columns.contains(&e.get_name().unwrap().as_str()))
+                .drain_filter(|e| !columns.contains(&e.get_name().unwrap()))
                 .collect::<Vec<_>>();
             Some(PyDataDict {
                 data,
                 column_map: Arc::new(Mutex::new(column_map)),
             })
         }
     }
@@ -184,14 +195,43 @@
                     .unwrap()
                     .get(col_name)
                     .unwrap_or_else(|| panic!("{col_name} isn't a column")),
             )
             .unwrap()
     }
 
+    pub fn get_matched_regex_column(&self, col_name: &str) -> Vec<String> {
+        if col_name.starts_with('^') & col_name.ends_with('$') {
+            let re = Regex::new(col_name).expect("Invalid regex");
+            self.data
+                .iter()
+                .filter(|e| re.is_match(e.get_name().unwrap().as_str()))
+                .map(|e| e.get_name().unwrap())
+                .collect()
+        } else {
+            vec![col_name.to_string()]
+        }
+    }
+
+    pub fn get_by_regex(&self, col_name: &str) -> Result<Vec<PyExpr>, &'static str> {
+        if col_name.starts_with('^') & col_name.ends_with('$') {
+            let re = Regex::new(col_name).expect("Invalid regex");
+            let out: Vec<PyExpr> = self
+                .data
+                .iter()
+                .filter(|e| re.is_match(e.get_name().unwrap().as_str()))
+                .cloned()
+                // .map(|e| e.clone())
+                .collect();
+            Ok(out)
+        } else {
+            Ok(vec![self.get_by_str(col_name).clone()])
+        }
+    }
+
     pub fn get_mut_by_str(&mut self, col_name: &str) -> &mut PyExpr {
         self.data
             .get_mut(
                 *self
                     .column_map
                     .lock()
                     .unwrap()
@@ -272,15 +312,15 @@
                 value.set_name(self.len().to_string())
             }
             self._insert(value);
         }
     }
 
     #[allow(unreachable_patterns)]
-    pub fn select_on_axis(&self, slc: Vec<usize>, axis: Option<usize>) -> PyDataDict {
+    pub fn select_on_axis(&self, slc: Vec<usize>, axis: Option<i32>) -> PyDataDict {
         let mut out_data = Vec::<PyExpr>::with_capacity(slc.len());
         let axis = axis.unwrap_or(0);
         let slc_expr: Expr<'static, usize> = slc.into();
         for expr in &self.data {
             out_data.push(match_exprs!(&expr.inner, e, {
                 e.clone()
                     .select_on_axis_by_expr(slc_expr.clone(), axis.into())
@@ -453,62 +493,95 @@
             // but one should not use the original DataDict after evaluating it.
             Ok(Some(self.clone()))
         }
     }
 
     fn __getitem__(&self, ob: &PyAny, py: Python) -> PyResult<PyObject> {
         if let Ok(col_name) = ob.extract::<&str>() {
-            Ok(self.get_by_str(col_name).clone().into_py(py))
+            let out = self.get_by_regex(col_name).map_err(PyValueError::new_err)?;
+            if out.len() == 1 {
+                Ok(out[0].clone().into_py(py))
+            } else {
+                Ok(PyDataDict::new(out, None).into_py(py))
+            }
         } else if let Ok(col_idx) = ob.extract::<i32>() {
             Ok(self.get_by_idx(col_idx).clone().into_py(py))
         } else if let Ok(col_name_vec) = ob.extract::<Vec<&str>>() {
             let out = col_name_vec
                 .into_iter()
-                .map(|col_name| self.get_by_str(col_name).clone())
-                .collect_trusted();
+                .flat_map(|col_name| self.get_by_regex(col_name).unwrap())
+                .collect();
             Ok(PyDataDict::new(out, None).into_py(py))
         } else if let Ok(col_idx_vec) = ob.extract::<Vec<i32>>() {
             let out = col_idx_vec
                 .into_iter()
                 .map(|col_idx| self.get_by_idx(col_idx).clone())
                 .collect_trusted();
             Ok(PyDataDict::new(out, None).into_py(py))
         } else {
             Err(PyValueError::new_err("Not support type in get item"))
         }
     }
 
-    pub unsafe fn __setitem__(&mut self, key: &PyAny, value: &PyAny) -> PyResult<()> {
+    pub unsafe fn __setitem__(&mut self, key: &PyAny, value: &PyAny, py: Python) -> PyResult<()> {
         if let Ok(col_name) = key.extract::<String>() {
-            let value = parse_expr_nocopy(value)?;
-            self.set_by_name(col_name, value);
-            Ok(())
+            let col_name_vec = self.get_matched_regex_column(&col_name);
+            match col_name_vec.len().cmp(&1) {
+                Ordering::Greater => {
+                    let key = col_name_vec.into_py(py);
+                    self.__setitem__(key.as_ref(py), value, py)
+                }
+                Ordering::Equal => {
+                    let value = parse_expr_nocopy(value)?;
+                    self.set_by_name(col_name_vec[0].clone(), value);
+                    Ok(())
+                }
+                Ordering::Less => Err(PyValueError::new_err("The column name doesn't exist")),
+            }
         } else if let Ok(col_idx) = key.extract::<i32>() {
             let value = parse_expr_nocopy(value)?;
             self.set_by_idx(col_idx, value);
             Ok(())
         } else if let Ok(col_name_vec) = key.extract::<Vec<String>>() {
+            let col_name_vec: Vec<String> = col_name_vec
+                .into_iter()
+                .flat_map(|col| self.get_matched_regex_column(&col))
+                .collect();
             let value_vec = parse_expr_list(value, false)?;
             if value_vec.len() != col_name_vec.len() {
-                return Err(PyValueError::new_err(
-                    "The length of columns and values are not equal",
-                ));
+                if value_vec.len() == 1 {
+                    col_name_vec
+                        .into_iter()
+                        .for_each(|col_name| self.set_by_name(col_name, value_vec[0].deep_copy()));
+                } else {
+                    return Err(PyValueError::new_err(
+                        "The length of columns and values are not equal",
+                    ));
+                }
+            } else {
+                zip(col_name_vec, value_vec)
+                    .for_each(|(col_name, value)| self.set_by_name(col_name, value));
             }
-            zip(col_name_vec, value_vec)
-                .for_each(|(col_name, value)| self.set_by_name(col_name, value));
             Ok(())
         } else if let Ok(col_idx_vec) = key.extract::<Vec<i32>>() {
             let value_vec = parse_expr_list(value, false)?;
             if value_vec.len() != col_idx_vec.len() {
-                return Err(PyValueError::new_err(
-                    "The length of columns and values are not equal",
-                ));
+                if value_vec.len() == 1 {
+                    col_idx_vec
+                        .into_iter()
+                        .for_each(|col_idx| self.set_by_idx(col_idx, value_vec[0].deep_copy()));
+                } else {
+                    return Err(PyValueError::new_err(
+                        "The length of columns and values are not equal",
+                    ));
+                }
+            } else {
+                zip(col_idx_vec, value_vec)
+                    .for_each(|(col_idx, value)| self.set_by_idx(col_idx, value));
             }
-            zip(col_idx_vec, value_vec)
-                .for_each(|(col_idx, value)| self.set_by_idx(col_idx, value));
             Ok(())
         } else {
             Err(PyValueError::new_err("Not support type in set item"))
         }
     }
 
     pub fn __delitem__(&mut self, item: &PyAny) -> PyResult<()> {
@@ -543,49 +616,75 @@
             Ok(Some(out))
         } else {
             exprs.into_iter().for_each(|e| self._insert(e));
             Ok(None)
         }
     }
 
+    #[pyo3(signature=(func, **py_kwargs))]
+    pub fn apply(&self, func: &PyAny, py_kwargs: Option<&PyDict>) -> PyResult<Self> {
+        if self.is_empty() {
+            return Ok(self.clone());
+        }
+        let out_data = unsafe {
+            self.data
+                .iter()
+                .map(|e| {
+                    parse_expr_nocopy(
+                        func.call((e.clone(),), py_kwargs)
+                            .expect("Call python function error!"),
+                    )
+                    .expect("Can not parse fucntion return as Expr")
+                })
+                .collect_trusted()
+        };
+        Ok(PyDataDict::new(out_data, None))
+    }
+
     #[pyo3(signature=(window, func, axis=0, check=true, **py_kwargs))]
     #[allow(unreachable_patterns)]
     pub fn rolling_apply(
         &mut self,
         window: usize,
         func: &PyAny,
-        axis: usize,
+        axis: i32,
         check: bool,
         py_kwargs: Option<&PyDict>,
     ) -> PyResult<Self> {
         if self.is_empty() {
             return Ok(self.clone());
         }
         if window == 0 {
             return Err(PyValueError::new_err("Window should be greater than 0"));
         }
         self.eval_all()?;
-        let length = match_exprs!(&self.data[0].inner, expr, { expr.view_arr().shape()[axis] });
+        let axis = match_exprs!(&self.data[0].inner, expr, {
+            expr.view_arr().norm_axis(axis)
+        });
+        let axis_i = axis.index() as i32;
+        let length = match_exprs!(&self.data[0].inner, expr, {
+            expr.view_arr().shape()[axis.index()]
+        });
         if check {
             for e in &self.data {
-                let len_ = match_exprs!(&e.inner, expr, { expr.view_arr().shape()[axis] });
+                let len_ = match_exprs!(&e.inner, expr, { expr.view_arr().shape()[axis.index()] });
                 if length != len_ {
                     return Err(PyValueError::new_err(
                         "Each Expressions should have the same length on given axis",
                     ));
                 }
             }
         }
         let mut column_num = 0;
         let mut output = zip(repeat(0).take(window - 1), 0..window - 1)
             .chain((window - 1..length).enumerate())
             .map(|(start, end)| {
                 let mut step_df = Vec::with_capacity(self.len());
                 self.data.iter().for_each(|pyexpr| unsafe {
-                    step_df.push(pyexpr.take_by_slice(Some(axis), start, end, None));
+                    step_df.push(pyexpr.take_by_slice(Some(axis_i), start, end, None));
                 });
                 let step_df = PyDataDict {
                     data: step_df,
                     column_map: self.column_map.clone(),
                 };
                 let res = func
                     .call((step_df,), py_kwargs)
@@ -604,28 +703,28 @@
         let out_data = (0..column_num)
             .into_par_iter()
             .map(|i| {
                 let group_vec = output
                     .iter()
                     .map(|single_output_exprs| single_output_exprs.get(i).unwrap().no_dim0())
                     .collect_trusted();
-                concat_expr(group_vec, axis).expect("Concat expr error")
+                concat_expr(group_vec, axis_i).expect("Concat expr error")
             })
             .collect();
         Ok(PyDataDict::new(out_data, None))
     }
 
     #[pyo3(signature=(duration, func, index=None, axis=0, check=true, **py_kwargs))]
     #[allow(unreachable_patterns)]
     pub fn rolling_apply_by_time(
         &mut self,
         duration: &str,
         func: &PyAny,
         index: Option<&str>,
-        axis: usize,
+        axis: i32,
         check: bool,
         py_kwargs: Option<&PyDict>,
     ) -> PyResult<Self> {
         if self.is_empty() {
             return Ok(self.clone());
         }
         self.eval_all()?;
@@ -644,18 +743,24 @@
                 return Err(PyValueError::new_err(
                     "The Number of DateTime Expression in DataDict should be 1",
                 ));
             } else {
                 out.unwrap()
             }
         };
-        let length = match_exprs!(&self.data[0].inner, expr, { expr.view_arr().shape()[axis] });
+        let axis = match_exprs!(&self.data[0].inner, expr, {
+            expr.view_arr().norm_axis(axis)
+        });
+        let axis_i = axis.index() as i32;
+        let length = match_exprs!(&self.data[0].inner, expr, {
+            expr.view_arr().shape()[axis.index()]
+        });
         if check {
             for e in &self.data {
-                let len_ = match_exprs!(&e.inner, expr, { expr.view_arr().shape()[axis] });
+                let len_ = match_exprs!(&e.inner, expr, { expr.view_arr().shape()[axis.index()] });
                 if length != len_ {
                     return Err(PyValueError::new_err(
                         "Each Expressions should have the same length on given axis",
                     ));
                 }
             }
         }
@@ -667,15 +772,15 @@
             .to_dim1()
             .unwrap()
             .into_iter()
             .enumerate()
             .map(|(end, start)| {
                 let mut step_df = Vec::with_capacity(self.len());
                 self.data.iter().for_each(|pyexpr| unsafe {
-                    step_df.push(pyexpr.take_by_slice(Some(axis), start, end, None));
+                    step_df.push(pyexpr.take_by_slice(Some(axis_i), start, end, None));
                 });
                 let step_df = PyDataDict {
                     data: step_df,
                     column_map: self.column_map.clone(),
                 };
                 let res = func
                     .call((step_df,), py_kwargs)
@@ -693,15 +798,15 @@
         let out_data = (0..column_num)
             .into_par_iter()
             .map(|i| {
                 let group_vec = output
                     .iter()
                     .map(|single_output_exprs| single_output_exprs.get(i).unwrap().no_dim0())
                     .collect_trusted();
-                concat_expr(group_vec, axis).expect("Concat expr error")
+                concat_expr(group_vec, axis_i).expect("Concat expr error")
             })
             .collect();
         Ok(PyDataDict::new(out_data, None))
     }
 
     #[pyo3(signature=(by, rev=false, inplace=false))]
     pub fn sort_by(&mut self, by: Vec<&str>, rev: bool, inplace: bool) -> Option<Self> {
@@ -722,33 +827,27 @@
             Some(self.clone())
         } else {
             None
         }
     }
 
     #[pyo3(signature=(by, axis=0, sort=true, par=false))]
-    pub fn groupby(
-        &mut self,
-        by: &PyAny,
-        axis: usize,
-        sort: bool,
-        par: bool,
-    ) -> PyResult<PyGroupBy> {
+    pub fn groupby(&mut self, by: &PyAny, axis: i32, sort: bool, par: bool) -> PyResult<PyGroupBy> {
         let by = parse_one_or_more_str(by)?;
         Ok(PyGroupBy::new(self._groupby(by, axis, sort, par)?, axis))
     }
 
     /// Groupby and consume the dfs generated during the groupby process
     /// this is faster as we don't need to clone `Vec<PyDataDict>`
     #[pyo3(signature=(py_func, by, axis=0, sort=true, par=false, **py_kwargs))]
     pub fn groupby_apply(
         &mut self,
         py_func: &PyAny,
         by: &PyAny,
-        axis: usize,
+        axis: i32,
         sort: bool,
         par: bool,
         py_kwargs: Option<&PyDict>,
     ) -> PyResult<PyDataDict> {
         let by = parse_one_or_more_str(by)?;
         let group_dfs = self._groupby(by, axis, sort, par)?;
         super::groupby::groupby_apply(group_dfs, py_func, axis, py_kwargs)
@@ -863,15 +962,15 @@
     #[pyo3(signature=(subset, keep="first", inplace=false, axis=0))]
     #[allow(unreachable_patterns)]
     pub fn unique(
         &mut self,
         subset: &PyAny,
         keep: &str,
         inplace: bool,
-        axis: usize,
+        axis: i32,
     ) -> PyResult<Option<Self>> {
         let subset = parse_one_or_more_str(subset)?;
         if subset.is_empty() {
             return Err(PyValueError::new_err("subset cannot be empty"));
         }
         self.eval_multi(&subset)?;
         let subset_exprs = subset
@@ -992,11 +1091,11 @@
 fn parse_one_or_more_str(s: &PyAny) -> PyResult<Vec<&str>> {
     if let Ok(s) = s.extract::<&str>() {
         Ok(vec![s])
     } else if let Ok(s) = s.extract::<Vec<&str>>() {
         Ok(s)
     } else {
         Err(PyValueError::new_err(
-            "the type of param on is not supported",
+            "the param cann't be parsed as a vector of string",
         ))
     }
 }
```

### Comparing `teapy-0.1.6/src/pylazy/export.rs` & `teapy-0.1.7/src/pylazy/export.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/src/pylazy/groupby.rs` & `teapy-0.1.7/src/pylazy/groupby.rs`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 use super::export::*;
 
 impl PyDataDict {
     pub(crate) fn _groupby(
         &mut self,
         keys: Vec<&str>,
-        axis: usize,
+        axis: i32,
         sort: bool,
         par: bool,
     ) -> PyResult<Vec<PyDataDict>> {
         self.eval_multi(&keys)?;
         let keys = keys
             .into_iter()
             .map(|key| &self.get_by_str(key).inner)
@@ -27,15 +27,15 @@
         Ok(output)
     }
 }
 
 pub(super) fn groupby_apply(
     group_dfs: Vec<PyDataDict>,
     py_func: &PyAny,
-    axis: usize,
+    axis: i32,
     py_kwargs: Option<&PyDict>,
 ) -> PyResult<PyDataDict> {
     assert!(
         py_func.is_callable(),
         "must pass a callable object to apply"
     );
     let mut exprs = Vec::<Vec<PyExpr>>::with_capacity(group_dfs.len());
@@ -45,15 +45,15 @@
             .expect("call python function error!");
         let expr_list = unsafe { parse_expr_list(expr_list, false) }?;
         exprs.push(expr_list);
     }
     Ok(groupby_eval(exprs, axis))
 }
 
-fn groupby_eval(mut exprs: Vec<Vec<PyExpr>>, axis: usize) -> PyDataDict {
+fn groupby_eval(mut exprs: Vec<Vec<PyExpr>>, axis: i32) -> PyDataDict {
     let column_num = exprs[0].len(); // each group should have the same column num
     exprs
         .par_iter_mut()
         .for_each(|vec_e| vec_e.par_iter_mut().for_each(|e| e.eval_inplace()));
 
     let out_data = (0..column_num)
         .into_par_iter()
@@ -67,22 +67,22 @@
         .collect();
     PyDataDict::new(out_data, None)
 }
 
 #[pyclass]
 pub struct PyGroupBy {
     data: Vec<PyDataDict>,
-    axis: usize,
+    axis: i32,
 }
 
 #[pymethods]
 impl PyGroupBy {
     #[new]
     #[pyo3(signature=(data, axis=0))]
-    pub fn new(data: Vec<PyDataDict>, axis: usize) -> Self {
+    pub fn new(data: Vec<PyDataDict>, axis: i32) -> Self {
         PyGroupBy { data, axis }
     }
 
     pub fn data(&self) -> Vec<PyDataDict> {
         self.data.clone()
     }
```

### Comparing `teapy-0.1.6/src/pylazy/impl_pyexpr.rs` & `teapy-0.1.7/src/pylazy/impl_pyexpr.rs`

 * *Files 3% similar despite different names*

```diff
@@ -137,62 +137,72 @@
         // Clear reference, this decrements ref counter.
         self.obj = None;
     }
 
     #[allow(unreachable_patterns)]
     pub unsafe fn __getitem__(self: PyRef<Self>, obj: &PyAny, py: Python) -> PyResult<Self> {
         use pyo3::types::{PyList, PySlice, PyTuple};
-        if obj.is_instance_of::<PyList>()? || obj.is_instance_of::<PyTuple>()? {
-            let obj_vec = obj.extract::<Vec<&PyAny>>().unwrap();
-            // if item is slice, slice first
+        if let Ok(length) = obj.len() {
             let mut slc_vec = Vec::with_capacity(10);
-            let mut no_slice_idx_vec = Vec::with_capacity(obj_vec.len());
-            let mut no_slice_slc_obj_vec = Vec::with_capacity(obj_vec.len());
-            for (idx, obj) in obj_vec.into_iter().enumerate() {
-                if let Ok(slc) = obj.extract::<&PySlice>() {
-                    let start = slc
-                        .getattr("start")?
-                        .extract::<Option<isize>>()?
-                        .unwrap_or(0);
-                    let end = slc.getattr("stop")?.extract::<Option<isize>>()?;
-                    let step = slc
-                        .getattr("step")?
-                        .extract::<Option<isize>>()?
-                        .unwrap_or(1);
-                    slc_vec.push(SliceInfoElem::Slice { start, end, step });
-                } else if obj.is_none() {
-                    slc_vec.push(SliceInfoElem::NewAxis);
-                } else {
-                    no_slice_idx_vec.push(idx);
-                    no_slice_slc_obj_vec.push(obj);
-                    slc_vec.push(SliceInfoElem::Slice {
-                        start: 0,
-                        end: None,
-                        step: 1,
-                    });
+            let mut no_slice_idx_vec = Vec::with_capacity(length);
+            let mut no_slice_slc_obj_vec = Vec::with_capacity(length);
+            // if item is slice, slice first
+            if obj.is_instance_of::<PyList>() {
+                no_slice_idx_vec.push(0);
+                no_slice_slc_obj_vec.push(obj);
+                slc_vec.push(SliceInfoElem::Slice {
+                    start: 0,
+                    end: None,
+                    step: 1,
+                });
+            } else if obj.is_instance_of::<PyTuple>() {
+                let obj_vec = obj.extract::<Vec<&PyAny>>().unwrap();
+                for (idx, obj) in obj_vec.into_iter().enumerate() {
+                    if let Ok(slc) = obj.extract::<&PySlice>() {
+                        let start = slc
+                            .getattr("start")?
+                            .extract::<Option<isize>>()?
+                            .unwrap_or(0);
+                        let end = slc.getattr("stop")?.extract::<Option<isize>>()?;
+                        let step = slc
+                            .getattr("step")?
+                            .extract::<Option<isize>>()?
+                            .unwrap_or(1);
+                        slc_vec.push(SliceInfoElem::Slice { start, end, step });
+                    } else if obj.is_none() {
+                        slc_vec.push(SliceInfoElem::NewAxis);
+                    } else {
+                        no_slice_idx_vec.push(idx);
+                        no_slice_slc_obj_vec.push(obj);
+                        slc_vec.push(SliceInfoElem::Slice {
+                            start: 0,
+                            end: None,
+                            step: 1,
+                        });
+                    }
                 }
             }
-            let ori_dim = self.ndim().cast_usize()?;
+            let ori_dim = self.ndim().cast_i32()?;
             let mut out = self.view_by_slice(slc_vec, py);
             for (idx, slc_obj) in zip(no_slice_idx_vec, no_slice_slc_obj_vec) {
                 let slc = parse_expr_nocopy(slc_obj)?;
                 let obj = slc.obj();
-                let idx: Expr<'static, usize> = idx.into();
-                let idx = idx - (ori_dim.clone() - out.ndim().cast_usize()?);
+                let idx: Expr<'static, i32> = (idx as i32).into();
+                let idx = idx - (ori_dim.clone() - out.ndim().cast_i32()?);
                 out = if slc.is_bool() {
                     match_exprs!(&out.inner, expr, {
                         expr.clone()
                             .filter(slc.cast_bool()?, idx, false)
                             .to_py(out.obj())
                             .add_obj(obj)
                     })
                 } else {
                     match_exprs!(&out.inner, expr, {
                         expr.clone()
-                            .select_on_axis_by_expr(slc.cast_usize()?, idx)
+                            .select_on_axis_by_i32_expr(slc.cast_i32()?, idx)
                             .to_py(out.obj())
                             .add_obj(obj)
                     })
                 }
             }
             Ok(out)
         } else {
@@ -823,14 +833,28 @@
         match_exprs!(&mut self.inner, expr, {
             let mut e = expr.clone();
             e.rename(name);
             e.to_py(self.obj())
         })
     }
 
+    // pub fn __setstate__(&mut self, py: Python, state: PyObject) -> PyResult<()> {
+    //     match state.extract::<&pyo3::types::PyBytes>(py) {
+    //         Ok(s) => {
+    //             self.foo = bincode::deserialize(s.as_bytes()).unwrap();
+    //             Ok(())
+    //         }
+    //         Err(e) => Err(e),
+    //     }
+    // }
+
+    // pub fn __getstate__(&self, py: Python) -> PyResult<PyObject> {
+    //     Ok(PyBytes::new(py, &bincode::serialize(&self.foo).unwrap()).to_object(py))
+    // }
+
     /// Returns the square root of a number.
     ///
     /// Returns NaN if self is a negative number other than -0.0.
     pub fn sqrt(&self) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().sqrt().to_py(self.obj())
         })
@@ -1000,48 +1024,48 @@
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().log(base).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(axis=0, par=false))]
     #[allow(unreachable_patterns)]
-    pub fn first(&self, axis: usize, par: bool) -> Self {
+    pub fn first(&self, axis: i32, par: bool) -> Self {
         match_exprs!(&self.inner, expr, {
             expr.clone().first(axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(axis=0, par=false))]
     #[allow(unreachable_patterns)]
-    pub fn last(&self, axis: usize, par: bool) -> Self {
+    pub fn last(&self, axis: i32, par: bool) -> Self {
         match_exprs!(&self.inner, expr, {
             expr.clone().last(axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(axis=0, par=false))]
-    pub fn valid_first(&self, axis: usize, par: bool) -> Self {
+    pub fn valid_first(&self, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().valid_first(axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(axis=0, par=false))]
-    pub fn valid_last(&self, axis: usize, par: bool) -> Self {
+    pub fn valid_last(&self, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().valid_last(axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(n=1, fill=None, axis=0, par=false))]
     pub fn shift(
         &self,
         n: i32,
         fill: Option<&PyAny>,
-        axis: usize,
+        axis: i32,
         par: bool,
         py: Python,
     ) -> PyResult<Self> {
         let fill = if let Some(fill) = fill {
             if fill.is_none() {
                 None
             } else {
@@ -1167,55 +1191,55 @@
             Ok(out.add_obj(obj))
         } else {
             Ok(out)
         }
     }
 
     #[pyo3(signature=(n=1, axis=0, par=false))]
-    pub fn diff(&self, n: i32, axis: usize, par: bool) -> Self {
+    pub fn diff(&self, n: i32, axis: i32, par: bool) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             { expr.clone().diff(n, axis, par).to_py(self.obj()) },
             F32,
             I64,
             F64,
             I32
         )
     }
 
     #[pyo3(signature=(n=1, axis=0, par=false))]
-    pub fn pct_change(&self, n: i32, axis: usize, par: bool) -> Self {
+    pub fn pct_change(&self, n: i32, axis: i32, par: bool) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             { expr.clone().pct_change(n, axis, par).to_py(self.obj()) },
             F32,
             I64,
             F64,
             I32
         )
     }
 
     #[pyo3(signature=(axis=0, par=false))]
-    pub fn count_nan(&self, axis: usize, par: bool) -> Self {
+    pub fn count_nan(&self, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().count_nan(axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(axis=0, par=false))]
-    pub fn count_notnan(&self, axis: usize, par: bool) -> Self {
+    pub fn count_notnan(&self, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().count_notnan(axis, par).to_py(self.obj())
         })
     }
 
     // #[args(self, value, axis="0", par=false)]
-    // pub fn count_v(&self, value, axis: usize, par: bool) -> Self {
+    // pub fn count_v(&self, value, axis: i32, par: bool) -> Self {
     //     match_exprs!(&self.inner, expr, {expr.clone().count_v(value, axis, par).to_py(self.obj())}, F64, I32)
     // }
 
     #[allow(unreachable_patterns)]
     #[pyo3(signature=(mask, axis=None, par=false))]
     pub unsafe fn filter(&self, mask: &PyAny, axis: Option<&PyAny>, par: bool) -> PyResult<Self> {
         let mask = parse_expr_nocopy(mask)?;
@@ -1224,15 +1248,15 @@
         } else {
             0.into()
         };
         let obj = mask.obj();
         let obj2 = axis.obj();
         Ok(match_exprs!(&self.inner, expr, {
             expr.clone()
-                .filter(mask.cast_bool()?, axis.cast_usize()?, par)
+                .filter(mask.cast_bool()?, axis.cast_i32()?, par)
                 .to_py(self.obj())
                 .add_obj(obj)
                 .add_obj(obj2)
         }))
     }
 
     #[pyo3(signature=(axis=None, how=DropNaMethod::Any, par=false))]
@@ -1249,15 +1273,15 @@
         };
         let obj = axis.obj();
         Ok(match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
-                    .dropna(axis.cast_usize()?, how, par)
+                    .dropna(axis.cast_i32()?, how, par)
                     .to_py(self.obj())
                     .add_obj(obj)
             },
             F32,
             F64,
             I32,
             I64,
@@ -1274,32 +1298,32 @@
     pub fn not_nan(&self) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().not_nan().to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(axis=0, par=false))]
-    pub fn median(&self, axis: usize, par: bool) -> Self {
+    pub fn median(&self, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().median(axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(axis=0, par=false))]
-    pub fn all(&self, axis: usize, par: bool) -> Self {
+    pub fn all(&self, axis: i32, par: bool) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             { expr.clone().all(axis, par).to_py(self.obj()) },
             Bool
         )
     }
 
     #[pyo3(signature=(axis=0, par=false))]
-    pub fn any(&self, axis: usize, par: bool) -> Self {
+    pub fn any(&self, axis: i32, par: bool) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             { expr.clone().any(axis, par).to_py(self.obj()) },
             Bool
         )
     }
@@ -1315,31 +1339,31 @@
         match_exprs!(&self.inner, expr, {
             expr.clone().diag().to_py_ref(self, py)
         })
     }
 
     #[allow(unreachable_patterns)]
     /// Insert new array axis at axis and return the result.
-    pub unsafe fn insert_axis(self: PyRef<Self>, axis: usize, py: Python) -> Self {
+    pub unsafe fn insert_axis(self: PyRef<Self>, axis: i32, py: Python) -> Self {
         match_exprs!(&self.inner, expr, {
             expr.clone().insert_axis(axis).to_py_ref(self, py)
         })
     }
 
     // #[allow(unreachable_patterns)]
     // /// Insert new array axis at axis and return the result.
-    // pub unsafe fn insert_axis(&self, axis: usize) -> Self {
+    // pub unsafe fn insert_axis(&self, axis: i32) -> Self {
     //     match_exprs!(&self.inner, expr, {
     //         expr.clone().insert_axis(axis).to_py(None)
     //     })
     // }
 
     #[allow(unreachable_patterns)]
     /// Remove new array axis at axis and return the result.
-    pub unsafe fn remove_axis(self: PyRef<Self>, axis: usize, py: Python) -> Self {
+    pub unsafe fn remove_axis(self: PyRef<Self>, axis: i32, py: Python) -> Self {
         match_exprs!(&self.inner, expr, {
             expr.clone().remove_axis(axis).to_py_ref(self, py)
         })
     }
 
     #[allow(unreachable_patterns)]
     /// Return a transposed view of the array.
@@ -1347,15 +1371,15 @@
         match_exprs!(&self.inner, expr, { expr.clone().t().to_py_ref(self, py) })
     }
 
     #[allow(unreachable_patterns)]
     /// Swap axes ax and bx.
     ///
     /// This does not move any data, it just adjusts the array’s dimensions and strides.
-    pub unsafe fn swap_axes(self: PyRef<Self>, ax: usize, bx: usize, py: Python) -> Self {
+    pub unsafe fn swap_axes(self: PyRef<Self>, ax: i32, bx: i32, py: Python) -> Self {
         match_exprs!(&self.inner, expr, {
             expr.clone().swap_axes(ax, bx).to_py_ref(self, py)
         })
     }
 
     #[allow(unreachable_patterns)]
     /// Permute the axes.
@@ -1387,67 +1411,67 @@
     pub fn shape(&self) -> Self {
         match_exprs!(&self.inner, expr, {
             expr.clone().shape().to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(axis=0, par=false))]
-    pub fn max(&self, axis: usize, par: bool) -> Self {
+    pub fn max(&self, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().max(axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(axis=0, par=false))]
-    pub fn min(&self, axis: usize, par: bool) -> Self {
+    pub fn min(&self, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().min(axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(stable=false, axis=0, par=false))]
-    pub fn sum(&self, stable: bool, axis: usize, par: bool) -> Self {
+    pub fn sum(&self, stable: bool, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().sum(stable, axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(stable=false, axis=0, par=false))]
-    pub fn cumsum(&self, stable: bool, axis: usize, par: bool) -> Self {
+    pub fn cumsum(&self, stable: bool, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().cumsum(stable, axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(axis=0, par=false))]
-    pub fn prod(&self, axis: usize, par: bool) -> Self {
+    pub fn prod(&self, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().prod(axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(axis=0, par=false))]
-    pub fn cumprod(&self, axis: usize, par: bool) -> Self {
+    pub fn cumprod(&self, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().cumprod(axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(stable=false, axis=0, par=false))]
-    pub fn mean(&self, stable: bool, axis: usize, par: bool) -> Self {
+    pub fn mean(&self, stable: bool, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().mean(stable, axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(stable=false, axis=0, par=false, warning=true))]
     pub fn zscore(
         &self,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
         warning: bool,
         py: Python,
     ) -> PyResult<Self> {
         if warning && !self.is_float() {
             let warnings = py.import("warnings")?;
             warnings.call_method1(
@@ -1470,15 +1494,15 @@
     #[pyo3(signature=(method=WinsorizeMethod::Quantile, method_params=0.01, stable=false, axis=0, par=false, warning=true))]
     #[allow(clippy::too_many_arguments)]
     pub fn winsorize(
         &self,
         method: WinsorizeMethod,
         method_params: Option<f64>,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
         warning: bool,
         py: Python,
     ) -> PyResult<Self> {
         if warning && !self.is_float() {
             let warnings = py.import("warnings")?;
             warnings.call_method1(
@@ -1499,114 +1523,108 @@
             F32,
             I64
         );
         Ok(out)
     }
 
     #[pyo3(signature=(stable=false, axis=0, par=false))]
-    pub fn var(&self, stable: bool, axis: usize, par: bool) -> Self {
+    pub fn var(&self, stable: bool, axis: i32, par: bool) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             { expr.clone().var(stable, axis, par).to_py(self.obj()) },
             F64,
             I32,
             F32,
             I64
         )
     }
 
     #[pyo3(signature=(stable=false, axis=0, par=false))]
-    pub fn std(&self, stable: bool, axis: usize, par: bool) -> Self {
+    pub fn std(&self, stable: bool, axis: i32, par: bool) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             { expr.clone().std(stable, axis, par).to_py(self.obj()) },
             F64,
             I32,
             F32,
             I64
         )
     }
 
     #[pyo3(signature=(stable=false, axis=0, par=false))]
-    pub fn skew(&self, stable: bool, axis: usize, par: bool) -> Self {
+    pub fn skew(&self, stable: bool, axis: i32, par: bool) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             { expr.clone().skew(stable, axis, par).to_py(self.obj()) },
             F64,
             I32,
             F32,
             I64
         )
     }
 
     #[pyo3(signature=(stable=false, axis=0, par=false))]
-    pub fn kurt(&self, stable: bool, axis: usize, par: bool) -> Self {
+    pub fn kurt(&self, stable: bool, axis: i32, par: bool) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             { expr.clone().kurt(stable, axis, par).to_py(self.obj()) },
             F64,
             I32,
             F32,
             I64
         )
     }
 
     #[pyo3(signature=(pct=false, rev=false, axis=0, par=false))]
-    pub fn rank(&self, pct: bool, rev: bool, axis: usize, par: bool) -> Self {
+    pub fn rank(&self, pct: bool, rev: bool, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().rank(pct, rev, axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(q, method=QuantileMethod::Linear, axis=0, par=false))]
-    pub fn quantile(&self, q: f64, method: QuantileMethod, axis: usize, par: bool) -> Self {
+    pub fn quantile(&self, q: f64, method: QuantileMethod, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .quantile(q, method, axis, par)
                 .to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(rev=false, axis=0, par=false))]
-    pub fn argsort(&self, rev: bool, axis: usize, par: bool) -> Self {
+    pub fn argsort(&self, rev: bool, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().argsort(rev, axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(kth, sort=true, rev=false, axis=0, par=false))]
-    pub fn arg_partition(&self, kth: usize, sort: bool, rev: bool, axis: usize, par: bool) -> Self {
+    pub fn arg_partition(&self, kth: usize, sort: bool, rev: bool, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .arg_partition(kth, sort, rev, axis, par)
                 .to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(group, rev=false, axis=0, par=false))]
-    pub fn split_group(&self, group: usize, rev: bool, axis: usize, par: bool) -> Self {
+    pub fn split_group(&self, group: usize, rev: bool, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .split_group(group, rev, axis, par)
                 .to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(other, stable=false, axis=0, par=false))]
-    pub unsafe fn cov(
-        &self,
-        other: &PyAny,
-        stable: bool,
-        axis: usize,
-        par: bool,
-    ) -> PyResult<Self> {
+    pub unsafe fn cov(&self, other: &PyAny, stable: bool, axis: i32, par: bool) -> PyResult<Self> {
         let other = parse_expr_nocopy(other)?;
         let obj = other.obj();
         let res = match_exprs!(
             (&self.inner, e1, F64, F32, I64, I32),
             (&other.inner, e2, F64, F32, I64, I32),
             {
                 e1.clone()
@@ -1620,15 +1638,15 @@
 
     #[pyo3(signature=(other, method=CorrMethod::Pearson, stable=false, axis=0, par=false))]
     pub unsafe fn corr(
         &self,
         other: &PyAny,
         method: CorrMethod,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> PyResult<Self> {
         let other = parse_expr_nocopy(other)?;
         let obj = other.obj();
         let res = match_exprs!(
             (&self.inner, e1, F64, F32, I64, I32),
             (&other.inner, e2, F64, F32, I64, I32),
@@ -1640,60 +1658,60 @@
             }
         );
         Ok(res)
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, axis=0, par=false))]
-    pub fn ts_argmin(&self, window: usize, min_periods: usize, axis: usize, par: bool) -> Self {
+    pub fn ts_argmin(&self, window: usize, min_periods: usize, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .ts_argmin(window, min_periods, axis, par)
                 .to_py(self.obj())
         })
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, axis=0, par=false))]
-    pub fn ts_argmax(&self, window: usize, min_periods: usize, axis: usize, par: bool) -> Self {
+    pub fn ts_argmax(&self, window: usize, min_periods: usize, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .ts_argmax(window, min_periods, axis, par)
                 .to_py(self.obj())
         })
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, axis=0, par=false))]
-    pub fn ts_min(&self, window: usize, min_periods: usize, axis: usize, par: bool) -> Self {
+    pub fn ts_min(&self, window: usize, min_periods: usize, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .ts_min(window, min_periods, axis, par)
                 .to_py(self.obj())
         })
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, axis=0, par=false))]
-    pub fn ts_max(&self, window: usize, min_periods: usize, axis: usize, par: bool) -> Self {
+    pub fn ts_max(&self, window: usize, min_periods: usize, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .ts_max(window, min_periods, axis, par)
                 .to_py(self.obj())
         })
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, pct=false, axis=0, par=false))]
     pub fn ts_rank(
         &self,
         window: usize,
         min_periods: usize,
         pct: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         if !pct {
             match_exprs!(numeric & self.inner, expr, {
                 expr.clone()
                     .ts_rank(window, min_periods, axis, par)
                     .to_py(self.obj())
@@ -1705,35 +1723,35 @@
                     .to_py(self.obj())
             })
         }
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, axis=0, par=false))]
-    pub fn ts_prod(&self, window: usize, min_periods: usize, axis: usize, par: bool) -> Self {
+    pub fn ts_prod(&self, window: usize, min_periods: usize, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .ts_prod(window, min_periods, axis, par)
                 .to_py(self.obj())
         })
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, axis=0, par=false))]
-    pub fn ts_prod_mean(&self, window: usize, min_periods: usize, axis: usize, par: bool) -> Self {
+    pub fn ts_prod_mean(&self, window: usize, min_periods: usize, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .ts_prod_mean(window, min_periods, axis, par)
                 .to_py(self.obj())
         })
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, axis=0, par=false))]
-    pub fn ts_minmaxnorm(&self, window: usize, min_periods: usize, axis: usize, par: bool) -> Self {
+    pub fn ts_minmaxnorm(&self, window: usize, min_periods: usize, axis: i32, par: bool) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
                     .ts_minmaxnorm(window, min_periods, axis, par)
                     .to_py(self.obj())
@@ -1749,15 +1767,15 @@
     #[pyo3(signature=(other, window, min_periods=1, stable=false, axis=0, par=false))]
     pub unsafe fn ts_cov(
         &self,
         other: &PyAny,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> PyResult<Self> {
         let other = parse_expr_nocopy(other)?;
         let obj = other.obj();
         let res = match_exprs!(
             (&self.inner, e1, F64, F32, I64, I32),
             (&other.inner, e2, F64, F32, I64, I32),
@@ -1775,15 +1793,15 @@
     #[pyo3(signature=(other, window, min_periods=1, stable=false, axis=0, par=false))]
     pub unsafe fn ts_corr(
         &self,
         other: &PyAny,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> PyResult<Self> {
         let other = parse_expr_nocopy(other)?;
         let obj = other.obj();
         let res = match_exprs!(
             (&self.inner, e1, F64, F32, I64, I32),
             (&other.inner, e2, F64, F32, I64, I32),
@@ -1800,15 +1818,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_sum(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .ts_sum(window, min_periods, stable, axis, par)
                 .to_py(self.obj())
         })
@@ -1817,15 +1835,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_sma(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .ts_sma(window, min_periods, stable, axis, par)
                 .to_py(self.obj())
         })
@@ -1834,15 +1852,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_ewm(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .ts_ewm(window, min_periods, stable, axis, par)
                 .to_py(self.obj())
         })
@@ -1851,15 +1869,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_wma(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .ts_wma(window, min_periods, stable, axis, par)
                 .to_py(self.obj())
         })
@@ -1868,15 +1886,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_std(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
@@ -1893,15 +1911,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_var(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
@@ -1918,15 +1936,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_skew(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
@@ -1943,15 +1961,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_kurt(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
@@ -1968,15 +1986,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_stable(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
@@ -1993,15 +2011,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_meanstdnorm(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
@@ -2018,15 +2036,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_reg(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
@@ -2043,15 +2061,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_tsf(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
@@ -2068,15 +2086,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_reg_slope(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
@@ -2093,15 +2111,15 @@
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_reg_intercept(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> Self {
         match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
@@ -2113,37 +2131,37 @@
             F32,
             I64
         )
     }
 
     #[cfg(feature = "window_func")]
     #[pyo3(signature=(method=FillMethod::Ffill, value=None, axis=0, par=false))]
-    pub fn fillna(&self, method: FillMethod, value: Option<f64>, axis: usize, par: bool) -> Self {
+    pub fn fillna(&self, method: FillMethod, value: Option<f64>, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone()
                 .fillna(method, value, axis, par)
                 .to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(min, max, axis=0, par=false))]
-    pub fn clip(&self, min: f64, max: f64, axis: usize, par: bool) -> Self {
+    pub fn clip(&self, min: f64, max: f64, axis: i32, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().clip(min, max, axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(slc, axis=0))]
-    pub unsafe fn select(&self, slc: &PyAny, axis: usize) -> PyResult<Self> {
+    pub unsafe fn select(&self, slc: &PyAny, axis: i32) -> PyResult<Self> {
         let slc = parse_expr_nocopy(slc)?;
         self._select_on_axis_by_expr(slc, axis.into())
     }
 
     #[pyo3(signature=(slc, axis=0, par=false))]
-    pub unsafe fn take(&self, slc: &PyAny, axis: usize, par: bool) -> PyResult<Self> {
+    pub unsafe fn take(&self, slc: &PyAny, axis: i32, par: bool) -> PyResult<Self> {
         let slc = parse_expr_nocopy(slc)?;
         self._take_on_axis_by_expr(slc, axis, par)
     }
 
     #[pyo3(signature=(df, loc=None, scale=None))]
     pub unsafe fn t_cdf(&self, df: &PyAny, loc: Option<f64>, scale: Option<f64>) -> PyResult<Self> {
         let df = parse_expr_nocopy(df)?;
@@ -2199,15 +2217,15 @@
     }
 
     #[pyo3(signature=(mask, value, axis=0, par=false))]
     pub unsafe fn put_mask(
         self: PyRef<Self>,
         mask: &PyAny,
         value: &PyAny,
-        axis: usize,
+        axis: i32,
         par: bool,
         py: Python,
     ) -> PyResult<Self> {
         let (mask, value) = (parse_expr_nocopy(mask)?, parse_expr_nocopy(value)?);
         let (obj1, obj2) = (mask.obj(), value.obj());
         let mask = mask.cast_bool().expect("Can not cast mask to bool.");
         let rtn = match self.inner() {
@@ -2440,22 +2458,22 @@
                 .to_py_ref(self, py)
                 .add_obj(obj))
         })
     }
 
     #[pyo3(name = "concat")]
     #[pyo3(signature=(other, axis=0))]
-    pub unsafe fn concat_py(&self, other: &PyAny, axis: usize) -> PyResult<Self> {
+    pub unsafe fn concat_py(&self, other: &PyAny, axis: i32) -> PyResult<Self> {
         let other = parse_expr_list(other, false)?;
         self.concat(other, axis)
     }
 
     #[pyo3(name = "stack")]
     #[pyo3(signature=(other, axis=0))]
-    pub unsafe fn stack_py(&self, other: &PyAny, axis: usize) -> PyResult<Self> {
+    pub unsafe fn stack_py(&self, other: &PyAny, axis: i32) -> PyResult<Self> {
         let other = parse_expr_list(other, false)?;
         self.stack(other, axis)
     }
 
     pub fn offset_by(&self, delta: &str) -> PyResult<Self> {
         let delta: Expr<'static, TimeDelta> = TimeDelta::parse(delta).into();
         Ok((self.clone().cast_datetime(None)? + delta).to_py(self.obj()))
@@ -2515,15 +2533,15 @@
 
     #[pyo3(signature=(index, duration, func, axis=0, **py_kwargs))]
     pub unsafe fn rolling_apply_by_time(
         &self,
         index: &PyAny,
         duration: &str,
         func: &PyAny,
-        axis: usize,
+        axis: i32,
         py_kwargs: Option<&PyDict>,
         py: Python,
     ) -> PyResult<PyObject> {
         let index_expr = parse_expr_nocopy(index)?;
         let mut rolling_idx = index_expr.cast_datetime(None)?.time_rolling(duration);
         rolling_idx.eval_inplace();
         let mut column_num = 0;
@@ -2568,24 +2586,27 @@
 
     #[allow(unreachable_patterns)]
     #[pyo3(signature=(window, func, axis=0, **py_kwargs))]
     pub unsafe fn rolling_apply(
         &mut self,
         window: usize,
         func: &PyAny,
-        axis: usize,
+        axis: i32,
         py_kwargs: Option<&PyDict>,
         py: Python,
     ) -> PyResult<PyObject> {
         if window == 0 {
             return Err(PyValueError::new_err("Window should be greater than 0"));
         }
         let mut column_num = 0;
         self.eval_inplace();
-        let length = match_exprs!(&self.inner, expr, { expr.view_arr().shape()[axis] });
+        let axis_n = match_exprs!(&self.inner, expr, { expr.view_arr().norm_axis(axis) });
+        let length = match_exprs!(&self.inner, expr, {
+            expr.view_arr().shape()[axis_n.index()]
+        });
         let mut output = zip(repeat(0).take(window - 1), 0..window - 1)
             .chain((window - 1..length).enumerate())
             .map(|(end, start)| {
                 let pye = self.take_by_slice(Some(axis), start, end, None);
                 let res = func
                     .call((pye,), py_kwargs)
                     .expect("Call python function error!");
```

### Comparing `teapy-0.1.6/src/pylazy/mod.rs` & `teapy-0.1.7/src/pylazy/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 mod time;
 
 pub use datadict::PyDataDict;
 pub use groupby::PyGroupBy;
 pub use pyexpr::PyExpr;
 pub use pyfunc::{
     arange, concat_expr, concat_expr_py, datetime, eval, from_pandas, full,
-    get_newey_west_adjust_s, parse_expr, parse_expr_list, parse_expr_nocopy, timedelta, where_py,
+    get_newey_west_adjust_s, parse_expr, parse_expr_list, parse_expr_nocopy, stack_expr_py,
+    timedelta, where_py,
 };
 
 use pyo3::prelude::{wrap_pyfunction, PyModule, PyResult};
 
 pub(crate) fn add_lazy(m: &PyModule) -> PyResult<()> {
     m.add_class::<PyExpr>()?;
     m.add_class::<PyDataDict>()?;
     m.add_class::<PyGroupBy>()?;
     m.add_function(wrap_pyfunction!(concat_expr_py, m)?)?;
+    m.add_function(wrap_pyfunction!(stack_expr_py, m)?)?;
     m.add_function(wrap_pyfunction!(eval, m)?)?;
     m.add_function(wrap_pyfunction!(where_py, m)?)?;
     m.add_function(wrap_pyfunction!(full, m)?)?;
     m.add_function(wrap_pyfunction!(arange, m)?)?;
     m.add_function(wrap_pyfunction!(datetime, m)?)?;
     m.add_function(wrap_pyfunction!(timedelta, m)?)?;
     m.add_function(wrap_pyfunction!(from_pandas, m)?)?;
```

### Comparing `teapy-0.1.6/src/pylazy/pyexpr.rs` & `teapy-0.1.7/src/pylazy/pyexpr.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use std::cmp::Ordering;
 use std::ops::Deref;
 
-use ndarray::{Axis, Slice, SliceInfoElem};
+use ndarray::{Slice, SliceInfoElem};
 
 use super::export::*;
 use crate::{
     arr::{ArbArray, DateTime, ExprElement, Number, TimeDelta, TimeUnit},
     from_py::PyValue,
 };
 
@@ -248,21 +248,21 @@
 
     #[allow(unreachable_patterns)]
     pub fn _select_on_axis_by_expr(&self, slc: Self, axis: Self) -> PyResult<Self> {
         let obj = slc.obj();
         match_exprs!(&self.inner, expr, {
             Ok(expr
                 .clone()
-                .select_on_axis_by_expr(slc.cast_usize()?, axis.cast_usize()?)
+                .select_on_axis_by_expr(slc.cast_usize()?, axis.cast_i32()?)
                 .to_py(self.obj())
                 .add_obj(obj))
         })
     }
 
-    pub fn _select_on_axis(&self, slc: Vec<usize>, axis: usize) -> Self {
+    pub fn _select_on_axis(&self, slc: Vec<usize>, axis: i32) -> Self {
         let slc_expr: Expr<usize> = slc.into();
         self._select_on_axis_by_expr(slc_expr.into(), axis.into())
             .unwrap()
     }
 
     /// take values using slice
     ///
@@ -273,15 +273,15 @@
     pub unsafe fn view_by_slice(self: PyRef<Self>, slc: Vec<SliceInfoElem>, py: Python) -> Self {
         match_exprs!(&self.inner, expr, {
             expr.clone().view_by_slice(slc).to_py_ref(self, py)
         })
     }
 
     #[allow(unreachable_patterns)]
-    pub fn _take_on_axis_by_expr(&self, slc: Self, axis: usize, par: bool) -> PyResult<Self> {
+    pub fn _take_on_axis_by_expr(&self, slc: Self, axis: i32, par: bool) -> PyResult<Self> {
         let obj = slc.obj();
         match_exprs!(&self.inner, expr, {
             Ok(expr
                 .clone()
                 .take_on_axis_by_expr(slc.cast_usize()?, axis, par)
                 .to_py(self.obj())
                 .add_obj(obj))
@@ -291,28 +291,28 @@
     #[allow(unreachable_patterns)]
     /// # Safety
     ///
     /// The slice must be valid
     pub unsafe fn _take_on_axis_by_expr_unchecked(
         &self,
         slc: Self,
-        axis: usize,
+        axis: i32,
         par: bool,
     ) -> PyResult<Self> {
         let obj = slc.obj();
         match_exprs!(&self.inner, expr, {
             Ok(expr
                 .clone()
                 .take_on_axis_by_expr_unchecked(slc.cast_usize()?, axis, par)
                 .to_py(self.obj())
                 .add_obj(obj))
         })
     }
 
-    pub fn _take_on_axis(&self, slc: Vec<usize>, axis: usize, par: bool) -> Self {
+    pub fn _take_on_axis(&self, slc: Vec<usize>, axis: i32, par: bool) -> Self {
         let slc_expr: Expr<usize> = slc.into();
         self._take_on_axis_by_expr(slc_expr.into(), axis, par)
             .unwrap()
     }
 
     #[allow(unreachable_patterns)]
     pub fn sort_by_expr(&self, by: Vec<PyExpr>, rev: bool) -> Self {
@@ -378,15 +378,17 @@
         };
         Ok(out)
     }
 
     pub(crate) fn cast_by_str(&self, ty_name: &str, py: Python) -> PyResult<Self> {
         match ty_name.to_lowercase().as_str() {
             "float" | "f64" => Ok(self.clone().cast_f64()?.to_py(self.obj())),
+            "f32" => Ok(self.clone().cast_f32()?.to_py(self.obj())),
             "int" | "i32" => Ok(self.clone().cast_i32()?.to_py(self.obj())),
+            "i64" => Ok(self.clone().cast_i64()?.to_py(self.obj())),
             "usize" | "uint" => Ok(self.clone().cast_usize()?.to_py(self.obj())),
             "bool" => Ok(self.clone().cast_bool()?.to_py(self.obj())),
             "object" => Ok(self.clone().cast_object_eager(py)?.to_py(self.obj())),
             "str" => {
                 if self.is_object() {
                     Ok(self
                         .clone()
@@ -402,15 +404,15 @@
             _ => Err(PyValueError::new_err(format!(
                 "cast to type: {ty_name} is not implemented"
             ))),
         }
     }
 
     #[allow(unreachable_patterns)]
-    pub fn concat(&self, other: Vec<PyExpr>, axis: usize) -> PyResult<PyExpr> {
+    pub fn concat(&self, other: Vec<PyExpr>, axis: i32) -> PyResult<PyExpr> {
         let obj_vec = other.iter().map(|e| e.obj()).collect_trusted();
         macro_rules! concat_macro {
             ($({$arm: ident => $cast_func: ident $(($arg: expr))?, $name: expr}),*) => {
                 match &self.inner {
                     $(Exprs::$arm(expr) => {
                         let other = other.into_iter().map(|e| e.$cast_func($($arg)?).expect(&format!("can not cast to {:?}", $name))).collect_trusted();
                         expr.clone().concat(other, axis).to_py(self.obj())
@@ -424,15 +426,15 @@
             {Bool => cast_bool, "bool"}, {Usize => cast_usize, "usize"}, {Str => cast_str, "str"}, {String => cast_string, "string"},
             {Object => cast_object, "object"}, {DateTime => cast_datetime(None), "DateTime"}, {TimeDelta => cast_timedelta, "TimeDelta"}
         );
         Ok(rtn.add_obj_vec(obj_vec))
     }
 
     #[allow(unreachable_patterns)]
-    pub fn stack(&self, other: Vec<PyExpr>, axis: usize) -> PyResult<PyExpr> {
+    pub fn stack(&self, other: Vec<PyExpr>, axis: i32) -> PyResult<PyExpr> {
         let obj_vec = other.iter().map(|e| e.obj()).collect_trusted();
         macro_rules! stack_macro {
             ($({$arm: ident => $cast_func: ident $(($arg: expr))?, $name: expr}),*) => {
                 match &self.inner {
                     $(Exprs::$arm(expr) => {
                         let other = other.into_iter().map(|e| e.$cast_func($($arg)?).expect(&format!("can not cast to {:?}", $name))).collect_trusted();
                         expr.clone().stack(other, axis).to_py(self.obj())
@@ -451,28 +453,29 @@
 
     /// # Safety
     ///
     /// Data of the base expression must exist.
     #[allow(unreachable_patterns)]
     pub unsafe fn take_by_slice(
         &self,
-        axis: Option<usize>,
+        axis: Option<i32>,
         start: usize,
         end: usize,
         step: Option<usize>,
     ) -> Self {
         match_exprs!(&self.inner, e, {
             let axis = axis.unwrap_or(0);
             let step = step.unwrap_or(1);
             let name = e.name();
             let e_view = e.view_arr();
+            let axis = e_view.norm_axis(axis);
             let e = Expr::new(
                 ArbArray::View(
                     e_view
-                        .slice_axis(Axis(axis), Slice::from(start..=end).step_by(step as isize))
+                        .slice_axis(axis, Slice::from(start..=end).step_by(step as isize))
                         .wrap(),
                 ),
                 name,
             );
             let e: Exprs<'_> = e.into();
             let e: Exprs<'static> = std::mem::transmute(e);
             e.into()
```

### Comparing `teapy-0.1.6/src/pylazy/pyfunc.rs` & `teapy-0.1.7/src/pylazy/pyfunc.rs`

 * *Files 3% similar despite different names*

```diff
@@ -177,36 +177,38 @@
     }
 }
 
 #[pyfunction]
 #[allow(clippy::missing_safety_doc)]
 #[pyo3(signature=(obj, copy=false))]
 pub unsafe fn parse_expr_list(obj: &PyAny, copy: bool) -> PyResult<Vec<PyExpr>> {
-    if obj.is_instance_of::<PyList3>()? || obj.is_instance_of::<PyTuple>()? {
+    if obj.is_instance_of::<PyList3>() || obj.is_instance_of::<PyTuple>() {
         if let Ok(seq) = obj.extract::<Vec<&PyAny>>() {
             Ok(seq
                 .into_iter()
                 .map(|obj| parse_expr(obj, copy).expect("Not support this type of Pyobject"))
                 .collect_trusted())
         } else {
             unreachable!()
         }
+    } else if let Ok(datadict) = obj.extract::<PyDataDict>() {
+        Ok(datadict.into_data())
     } else if let Ok(pyexpr) = parse_expr(obj, copy) {
         Ok(vec![pyexpr])
     } else {
         Err(PyValueError::new_err(
             "Can't parse the Object to a vector of expr",
         ))
     }
 }
 
 #[pyfunction]
 #[pyo3(signature=(exprs, axis=0))]
 #[allow(unreachable_patterns)]
-pub fn concat_expr(exprs: Vec<PyExpr>, axis: usize) -> PyResult<PyExpr> {
+pub fn concat_expr(exprs: Vec<PyExpr>, axis: i32) -> PyResult<PyExpr> {
     let e1 = exprs.get(0).unwrap().clone();
     let obj_vec = exprs.iter().skip(1).map(|e| e.obj()).collect_trusted();
     macro_rules! concat_macro {
         ($($arm: ident => $cast_func: ident $(($arg: expr))?),*) => {
             match e1.inner() {
                 $(Exprs::$arm(expr) => {
                     let other = exprs.into_iter().skip(1).map(|e| e.$cast_func($(($arg))?).unwrap()).collect_trusted();
@@ -224,23 +226,60 @@
     );
     Ok(rtn.add_obj_vec(obj_vec))
 }
 
 #[pyfunction]
 #[allow(clippy::missing_safety_doc)]
 #[pyo3(name="concat", signature=(exprs, axis=0))]
-pub unsafe fn concat_expr_py(exprs: Vec<&PyAny>, axis: usize) -> PyResult<PyExpr> {
+pub unsafe fn concat_expr_py(exprs: Vec<&PyAny>, axis: i32) -> PyResult<PyExpr> {
     let exprs = exprs
         .into_iter()
         .map(|e| parse_expr_nocopy(e))
         .collect::<PyResult<Vec<PyExpr>>>()?;
     concat_expr(exprs, axis)
 }
 
 #[pyfunction]
+#[pyo3(signature=(exprs, axis=0))]
+#[allow(unreachable_patterns)]
+pub fn stack_expr(exprs: Vec<PyExpr>, axis: i32) -> PyResult<PyExpr> {
+    let e1 = exprs.get(0).unwrap().clone();
+    let obj_vec = exprs.iter().skip(1).map(|e| e.obj()).collect_trusted();
+    macro_rules! stack_macro {
+        ($($arm: ident => $cast_func: ident $(($arg: expr))?),*) => {
+            match e1.inner() {
+                $(Exprs::$arm(expr) => {
+                    let other = exprs.into_iter().skip(1).map(|e| e.$cast_func($(($arg))?).unwrap()).collect_trusted();
+                    expr.clone().stack(other, axis).to_py(e1.obj())
+                }),*
+                _ => unimplemented!("stack is not implemented for this type.")
+            }
+        };
+    }
+    let rtn = stack_macro!(
+        F64 => cast_f64, F32 => cast_f32, I32 => cast_i32, I64 => cast_i64,
+        Bool => cast_bool, Usize => cast_usize,
+        Object => cast_object, String => cast_string, Str => cast_str,
+        DateTime => cast_datetime(None), TimeDelta => cast_timedelta
+    );
+    Ok(rtn.add_obj_vec(obj_vec))
+}
+
+#[pyfunction]
+#[allow(clippy::missing_safety_doc)]
+#[pyo3(name="stack", signature=(exprs, axis=0))]
+pub unsafe fn stack_expr_py(exprs: Vec<&PyAny>, axis: i32) -> PyResult<PyExpr> {
+    let exprs = exprs
+        .into_iter()
+        .map(|e| parse_expr_nocopy(e))
+        .collect::<PyResult<Vec<PyExpr>>>()?;
+    stack_expr(exprs, axis)
+}
+
+#[pyfunction]
 #[pyo3(signature=(exprs, inplace=false))]
 pub fn eval(mut exprs: Vec<PyExpr>, inplace: bool) -> Option<Vec<PyExpr>> {
     exprs.par_iter_mut().for_each(|e| e.eval_inplace());
     if inplace {
         None
     } else {
         Some(exprs)
```

### Comparing `teapy-0.1.6/teapy/array_func.py` & `teapy-0.1.7/teapy/array_func.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,9 @@
 from .wrapper import impl_by_lazy
 
-# __all__ = [
-#     "sum",
-#     "min",
-#     "max",
-#     "mean",
-#     "median",
-#     "quantile",
-#     "std",
-#     "var",
-#     "skew",
-#     "kurt",
-#     "count_nan",
-#     "count_notnan",
-#     "argsort",
-#     "rank",
-#     "cov",
-#     "corr",
-#     "fillna",
-#     "zscore",
-#     "winsorize",
-#     "dropna",
-#     # "remove_nan",
-#     "split_group",
-#     "clip",
-#     "shift",
-# ]
-
 
 @impl_by_lazy()
 def sum(arr, stable=False, axis=0, par=False):
     """
     Sum of array elements in a given axis.
 
     Parameters
```

### Comparing `teapy-0.1.6/teapy/converter.py` & `teapy-0.1.7/teapy/converter.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/teapy/datadict.py` & `teapy-0.1.7/teapy/datadict.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .teapy import PyDataDict as _DataDict
-from .teapy import from_pandas
+from .teapy import from_pandas, stack
 
 
 def _new_with_dd(dd=None):
     if dd is None:
         # for inplace functions
         return None
     out = DataDict()
@@ -22,14 +22,127 @@
 
 
 def from_pd(*args, **kwargs):
     dd = from_pandas(*args, **kwargs)
     return _new_with_dd(dd)
 
 
+class DataDict:
+    def __init__(self, data=None, columns=None, copy=False, **kwargs):
+        if data is not None or len(kwargs):
+            if data is None:
+                data = []
+            elif isinstance(data, dict):
+                columns = list(data.keys()) if columns is None else columns
+                data = list(data.values())
+            if len(kwargs):
+                if columns is None:
+                    columns = []
+                if isinstance(data, tuple):
+                    data = list(data)
+                for k, v in kwargs.items():
+                    data.append(v)
+                    columns.append(k)
+            self._dd = _DataDict(data=data, columns=columns, copy=copy)
+        else:
+            self._dd = _DataDict([])
+
+    def __getitem__(self, key):
+        return self._dd[key]
+
+    def __setitem__(self, item, value):
+        self._dd.__setitem__(item, value)
+
+    def __delitem__(self, item):
+        self._dd.__delitem__(item)
+
+    def __getattr__(self, attr):
+        return getattr(self._dd, attr)
+
+    @construct
+    def eval(self, cols=None, inplace=True):
+        return self._dd.eval(cols, inplace=inplace)
+
+    @construct
+    def select(self, exprs):
+        return self._dd.select(exprs)
+
+    def mean(self, axis=-1, stable=False, par=False):
+        if axis == -1:
+            return stack(self.raw_data, axis=axis).mean(axis=-1, stable=stable, par=par)
+        else:
+            axis = axis + 1 if axis < 0 else axis
+            return self.apply(lambda e: e.mean(axis=axis, stable=stable, par=par))
+
+    def sum(self, axis=-1, stable=False, par=False):
+        if axis == -1:
+            return stack(self.raw_data, axis=axis).sum(axis=-1, stable=stable, par=par)
+        else:
+            axis = axis + 1 if axis < 0 else axis
+            return self.apply(lambda e: e.sum(axis=axis, stable=stable, par=par))
+
+    def min(self, axis=-1, par=False):
+        if axis == -1:
+            return stack(self.raw_data, axis=axis).min(axis=-1, par=par)
+        else:
+            axis = axis + 1 if axis < 0 else axis
+            return self.apply(lambda e: e.min(axis=axis, par=par))
+
+    def max(self, axis=-1, par=False):
+        if axis == -1:
+            return stack(self.raw_data, axis=axis).max(axis=-1, par=par)
+        else:
+            axis = axis + 1 if axis < 0 else axis
+            return self.apply(lambda e: e.max(axis=axis, par=par))
+
+    def rename(self, mapper):
+        return self.with_columns(
+            [
+                self[key].alias(mapper[key])
+                for key in self.columns
+                if mapper.get(key) is not None
+            ]
+        )
+
+    @construct
+    def with_columns(self, exprs, inplace=False):
+        return self._dd.with_columns(exprs, inplace=inplace)
+
+    @construct
+    def join(self, right, on=None, left_on=None, right_on=None, how="left"):
+        if on is not None:
+            left_on = right_on = on
+        if how == "right":
+            return right._dd.join(
+                self._dd, left_on=right_on, right_on=left_on, method="left"
+            )
+        else:
+            return self._dd.join(right._dd, left_on, right_on, method=how)
+
+    @construct
+    def apply(self, func, **kwargs):
+        return self._dd.apply(func, **kwargs)
+
+    def rolling(self, window, dd, index=None, check=True, axis=0):
+        return Rolling(window, self._dd, index, check, axis)
+
+    @construct
+    def sort_by(self, by, rev=False, inplace=False):
+        return self._dd.sort_by(by=by, rev=rev, inplace=inplace)
+
+    def groupby(self, by, axis=0, sort=True, par=False, reuse=False):
+        return GroupBy(self._dd, by, axis, sort, par, reuse=reuse)
+
+    @construct
+    def unique(self, subset, keep="first", inplace=False, check=True, axis=0):
+        return self._dd.unique(
+            subset, keep=keep, inplace=inplace, check=check, axis=axis
+        )
+
+
 class Rolling:
     def __init__(self, window, dd, index=None, check=True, axis=0) -> None:
         """
         window: rolling window, int or str
         dd: PyDataDict
         index: time index, if None then infer automatically
         check: whether to check the length of each key is equal
@@ -47,23 +160,23 @@
             # rolling using a time duration
             return self._dd.rolling_apply_by_time(
                 index=self.index,
                 duration=self.window,
                 axis=self.axis,
                 func=func,
                 check=self.check,
-                py_kwargs=kwargs,
+                **kwargs,
             )
         else:
             return self._dd.rolling_apply(
                 window=self.window,
                 axis=self.axis,
                 func=func,
                 check=self.check,
-                py_kwargs=kwargs,
+                **kwargs,
             )
 
 
 class GroupBy:
     def __init__(self, dd, by, axis=0, sort=True, par=False, reuse=False) -> None:
         self._dd = dd
         self.by = by
@@ -78,73 +191,16 @@
         if not self.reuse:
             out = self._dd.groupby_apply(
                 by=self.by,
                 axis=self.axis,
                 sort=self.sort,
                 par=self.par,
                 py_func=func,
-                py_kwargs=kwargs,
+                **kwargs,
             )
         else:
             if self.groupby is None:
                 self.groupby = self._dd.groupby(
                     by=self.by, axis=self.axis, sort=self.sort, par=self.par
                 )
-            out = self.groupby.apply(py_func=func, py_kwargs=kwargs)
+            out = self.groupby.apply(func, **kwargs)
         return out
-
-
-class DataDict:
-    def __init__(self, *args, **kwargs):
-        if len(args) or len(kwargs):
-            self._dd = _DataDict(*args, **kwargs)
-        else:
-            self._dd = _DataDict([])
-
-    def __getitem__(self, key):
-        return self._dd[key]
-
-    def __setitem__(self, item, value):
-        self._dd.__setitem__(item, value)
-
-    def __delitem__(self, item):
-        self._dd.__delitem__(item)
-
-    def __getattr__(self, attr):
-        return getattr(self._dd, attr)
-
-    @construct
-    def eval(self, cols=None, inplace=True):
-        return self._dd.eval(cols, inplace=inplace)
-
-    @construct
-    def select(self, exprs):
-        return self._dd.select(exprs)
-
-    @construct
-    def with_columns(self, exprs, inplace=False):
-        return self._dd.with_columns(exprs, inplace=inplace)
-
-    @construct
-    def join(self, right, on=None, left_on=None, right_on=None, how="left"):
-        if on is not None:
-            left_on = right_on = on
-        if how == "right":
-            return right._dd.join(self._dd, left_on, right_on, method="left")
-        else:
-            return self._dd.join(right._dd, left_on, right_on, method=how)
-
-    def rolling(self, window, dd, index=None, check=True, axis=0):
-        return Rolling(window, self._dd, index, check, axis)
-
-    @construct
-    def sort_by(self, by, rev=False, inplace=False):
-        return self._dd.sort_by(by=by, rev=rev, inplace=inplace)
-
-    def groupby(self, by, axis=0, sort=True, par=False, reuse=False):
-        return GroupBy(self._dd, by, axis, sort, par, reuse=reuse)
-
-    @construct
-    def unique(self, subset, keep="first", inplace=False, check=True, axis=0):
-        return self._dd.unique(
-            subset, keep=keep, inplace=inplace, check=check, axis=axis
-        )
```

### Comparing `teapy-0.1.6/teapy/regression.py` & `teapy-0.1.7/teapy/regression.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/teapy/testing.py` & `teapy-0.1.7/teapy/testing.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/teapy/tests/test_array_func.py` & `teapy-0.1.7/teapy/tests/test_array_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/teapy/tests/test_common.py` & `teapy-0.1.7/teapy/tests/test_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,29 +28,29 @@
     expected_axis2 = np.array([[[0, 1], [2, 5]], [[4, 9], [6, 13]]])
 
     assert_allclose(tp.ts_sum(arr, 2, axis=0), expected_axis0)
     assert_allclose(tp.ts_sum(arr, 2, axis=1), expected_axis1)
     assert_allclose(tp.ts_sum(arr, 2, axis=2), expected_axis2)
 
 
-def test_parallel():
-    from multiprocessing import cpu_count
+# def test_parallel():
+#     from multiprocessing import cpu_count
 
-    arr = np.random.randn(16, 100000)
-    # no parallel
-    start = time()
-    tp.ts_std(arr, window=10, axis=1, par=False)
-    time1 = time() - start
-    # parallel
-    start = time()
-    tp.ts_std(arr, window=10, axis=1, par=True)
-    time2 = time() - start
+#     arr = np.random.randn(16, 100000)
+#     # no parallel
+#     start = time()
+#     tp.ts_std(arr, window=10, axis=1, par=False)
+#     time1 = time() - start
+#     # parallel
+#     start = time()
+#     tp.ts_std(arr, window=10, axis=1, par=True)
+#     time2 = time() - start
 
-    if cpu_count() > 1:
-        assert time1 > time2
+#     if cpu_count() > 1:
+#         assert time1 > time2
 
 
 def test_special():
     # test rank a array with 0 element
     assert tp.rank(np.array([])).tolist() == []
     assert tp.rank(np.array([2]))[0] == 1  # test rank a array with 1 element
     # test rank all nan array
```

### Comparing `teapy-0.1.6/teapy/tests/test_equity.py` & `teapy-0.1.7/teapy/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/teapy/tests/window/test_compare.py` & `teapy-0.1.7/teapy/tests/window/test_compare.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/teapy/tests/window/test_corr.py` & `teapy-0.1.7/teapy/tests/window/test_corr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/teapy/tests/window/test_feature.py` & `teapy-0.1.7/teapy/tests/window/test_feature.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/teapy/tests/window/test_norm.py` & `teapy-0.1.7/teapy/tests/window/test_norm.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/teapy/tests/window/test_reg.py` & `teapy-0.1.7/teapy/tests/window/test_reg.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/teapy/window_func.py` & `teapy-0.1.7/teapy/window_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/teapy/wrapper.py` & `teapy-0.1.7/teapy/wrapper.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.6/Cargo.lock` & `teapy-0.1.7/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -6,47 +6,53 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf6ccdb167abbf410dcb915cabd428929d7f6a04980b54a11f26a39f1c7f7107"
+checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
 dependencies = [
  "cfg-if",
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.19"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4f55bd91a0978cbfd91c457a164bab8b4001c833b7f323132c0a4e1922dd44e"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.65"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98161a4e3e2184da77bb14f02184cdd111e83bbbcc9979dfee3c44b9a85f5602"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "approx"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f2a05fd1bd10b2527e20a2cd32d8873d115b8b39fe219ee25f42a8aca6ba278"
 dependencies = [
@@ -72,44 +78,59 @@
 name = "base16ct"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "349a06037c7bf932dd7e7d1f653678b2038b9ad46a74102f1fc7bd7872678cce"
 
 [[package]]
 name = "base64"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "904dfeac50f3cdaba28fc6f57fdcddb75f49ed61346676a78c4ffe55877802fd"
+checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
+
+[[package]]
+name = "base64"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
+
+[[package]]
+name = "bincode"
+version = "1.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "block-buffer"
-version = "0.10.3"
+version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.11.0"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1ad822118d20d2c234f427000d5acc36eabe1e29a348c89b63dd60b13f28e5d"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "bytemuck"
-version = "1.12.3"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aaa3a8d9a1ca92e282c96a32d6511b695d7d994d1d102ba85d279f9b2756947f"
+checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
@@ -132,66 +153,51 @@
 checksum = "b6feecd82cce51b0204cf063f0041d69f24ce83f680d87514b004248e7b0fa65"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.73"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fff2a6927b3bb87f9595d67196a70493f627687a71d87a0d692242c33f58c11"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.23"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b0a3d9ed01224b22057780a37bb8c5dbfe1be8ba48678e7bf57ec4b385411f"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
  "js-sys",
- "num-integer",
  "num-traits",
- "time",
+ "serde",
+ "time 0.1.45",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
-name = "chunked_transfer"
-version = "1.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fff857943da45f546682664a79488be82e69e43c1a7a2307679ab9afb3a66d2e"
-
-[[package]]
-name = "codespan-reporting"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
-
-[[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -199,144 +205,162 @@
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.6"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "715e8152b692bba2d374b53d4875445368fdf21a94751410af607a5ac677d1fc"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
 dependencies = [
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.10"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "045ebe27666471bb549370b4b0b3e51b07f56325befa4284db65fc89c02511b1"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.6.5",
- "once_cell",
+ "memoffset",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.11"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "51887d4adc7b564537b15adcfb307936f8075dfcd5f00dde9a9f1d29383682bc"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
- "once_cell",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "cxx"
-version = "1.0.73"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "873c2e83af70859af2aaecd1f5d862f3790b747b1f4f50fb45a931d000ac0422"
+checksum = "109308c20e8445959c2792e81871054c6a17e6976489a93d2769641a2ba5839c"
 dependencies = [
  "cc",
  "cxxbridge-flags",
  "cxxbridge-macro",
  "link-cplusplus",
 ]
 
 [[package]]
-name = "cxx-build"
-version = "1.0.78"
+name = "cxxbridge-flags"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e580d70777c116df50c390d1211993f62d40302881e54d4b79727acb83d0199"
+checksum = "882074421238e84fe3b4c65d0081de34e5b323bf64555d3e61991f76eb64a7bb"
+
+[[package]]
+name = "cxxbridge-macro"
+version = "1.0.95"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4a076022ece33e7686fb76513518e219cca4fce5750a8ae6d1ce6c0f48fd1af9"
 dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
  "proc-macro2",
  "quote",
- "scratch",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
-name = "cxxbridge-flags"
-version = "1.0.73"
+name = "darling"
+version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f46b787c15af80277db5c88c6ac6c502ae545e622f010e06f95e540d34931acf"
+checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
+dependencies = [
+ "darling_core 0.14.4",
+ "darling_macro 0.14.4",
+]
 
 [[package]]
-name = "cxxbridge-macro"
-version = "1.0.73"
+name = "darling"
+version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ba3f3a7efa46626878fb5d324fabca4d19d2956b6ae97ce43044ef4515f5abc"
+checksum = "0558d22a7b463ed0241e993f76f09f30b126687447751a8638587b864e4b3944"
 dependencies = [
- "proc-macro2",
- "quote",
- "syn",
+ "darling_core 0.20.1",
+ "darling_macro 0.20.1",
 ]
 
 [[package]]
-name = "darling"
-version = "0.14.1"
+name = "darling_core"
+version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4529658bdda7fd6769b8614be250cdcfc3aeb0ee72fe66f9e41e5e5eb73eac02"
+checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
 dependencies = [
- "darling_core",
- "darling_macro",
+ "fnv",
+ "ident_case",
+ "proc-macro2",
+ "quote",
+ "strsim",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "darling_core"
-version = "0.14.1"
+version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "649c91bc01e8b1eac09fb91e8dbc7d517684ca6be8ebc75bb9cafc894f9fdb6f"
+checksum = "ab8bfa2e259f8ee1ce5e97824a3c55ec4404a0d772ca7fa96bf19f0752a046eb"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn",
+ "syn 2.0.18",
+]
+
+[[package]]
+name = "darling_macro"
+version = "0.14.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
+dependencies = [
+ "darling_core 0.14.4",
+ "quote",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "darling_macro"
-version = "0.14.1"
+version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddfc69c5bfcbd2fc09a0f38451d2daf0e372e367986a83906d1b0dbc88134fb5"
+checksum = "29a358ff9f12ec09c3e61fef9b5a9902623a695a46a917b07f269bff1445611a"
 dependencies = [
- "darling_core",
+ "darling_core 0.20.1",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "derive_builder"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d07adf7be193b71cc36b193d0f5fe60b918a3a9db4dad0449f57bcfd519704a3"
@@ -346,35 +370,35 @@
 
 [[package]]
 name = "derive_builder_core"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f91d4cfa921f1c05904dc3c57b4a32c38aed3340cce209f3a6fd1478babafc4"
 dependencies = [
- "darling",
+ "darling 0.14.4",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "derive_builder_macro"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f0314b72bed045f3a68671b3c86328386762c93f82d98c65c3cb5e5f573dd68"
 dependencies = [
  "derive_builder_core",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "digest"
-version = "0.10.5"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adfbc57365a37acbd2ebf2b64d7e69bb766e2fea813521ed536f5d0520dcf86c"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "directories"
@@ -394,70 +418,70 @@
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
 name = "either"
-version = "1.7.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f107b87b6afc2a64fd13cac55fe06d6c8859f12d4b14cbcdd2c67d0976781be"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "filetime"
-version = "0.2.17"
+version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e94a7bbaa59354bc20dd75b67f23e2797b4490e9d6928203fb105c79e448c86c"
+checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "windows-sys",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.24"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f82b0f4c27ad9f8bfd1f3208d882da2b09c301bc1c828fd3a00d0216d2fbbff6"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.7"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4eb1a864a501629691edf6c15a593b7a51eebaa1e8468e9ddc623de7c9b58ec6"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
@@ -465,71 +489,93 @@
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e45727250e75cc04ff2846a66397da8ef2b3db8e40e0cef4df67950a07621eb9"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
+name = "hashbrown"
+version = "0.12.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+
+[[package]]
 name = "hermit-abi"
-version = "0.1.19"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
+checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "hex"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
+
+[[package]]
 name = "iana-time-zone"
-version = "0.1.51"
+version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f5a6ef98976b22b3b7f2f3a806f858cb862044cfa66805aa3ad84cb3d3b785ed"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "winapi",
+ "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.0"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fde6edd6cef363e9359ed3c98ba64590ba9eecba2293eb5a723ab32aee8926aa"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
 
 [[package]]
 name = "idna"
-version = "0.3.0"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
+name = "indexmap"
+version = "1.9.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
+dependencies = [
+ "autocfg",
+ "hashbrown",
+ "serde",
+]
+
+[[package]]
 name = "indoc"
-version = "1.0.7"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adab1eaa3408fb7f0c777a73e7465fd5656136fc93b670eb6df3c88c2c1344e3"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "intel-mkl-src"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2ee70586cd5b3e772a8739a1bd43eaa90d4f4bf0fb2a4edc202e979937ee7f5e"
 dependencies = [
@@ -546,146 +592,141 @@
 dependencies = [
  "anyhow",
  "log",
  "walkdir",
 ]
 
 [[package]]
+name = "iter-read"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c397ca3ea05ad509c4ec451fea28b4771236a376ca1c69fd5143aae0cf8f93c4"
+
+[[package]]
 name = "itoa"
-version = "1.0.4"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4217ad341ebadf8d8e724e264f13e593e0648f5b3e94b3896a5df283be015ecc"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.60"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49409df3e3bf0856b916e2ceaca09ee28e6871cf7d9ce97a692cacfdb2a25a47"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "katexit"
-version = "0.1.2"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64d159b3c7a9ceb86b5b3bc9ce1d8e53fc03311f47cd67d3b4d26d4ef1c2c71a"
+checksum = "eb1304c448ce2c207c2298a34bc476ce7ae47f63c23fa2b498583b26be9bc88c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "lapack-sys"
 version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "447f56c85fb410a7a3d36701b2153c1018b1d2b908c5fbaf01c1b04fac33bcbe"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "lax"
 version = "0.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f96a229d9557112e574164f8024ce703625ad9f88a90964c1780809358e53da"
+source = "git+https://github.com/Teamon9161/ndarray-linalg.git?branch=arm-cross-compile#a4766b28528bf77a7b901cf43fa3b037798d4212"
 dependencies = [
  "cauchy",
  "intel-mkl-src",
  "katexit",
  "lapack-sys",
+ "libc",
  "num-traits",
  "thiserror",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.131"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04c3b4822ccebfa39c02fc03d1534441b22ead323fa0f48bb7ddd8e6ba076a40"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "libm"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "link-cplusplus"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f8cae2cd7ba2f3f63938b9c724475dfb7b9861b545a90324476324ed21dbc8c8"
+checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "lock_api"
-version = "0.4.7"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "327fa5b6a6940e4699ec49a9beae1ea4845c6bab9314e4f84ac68742139d8c53"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
+ "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.5.4"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96590ba8f175222643a85693f33d26e9c8a015f599c216509b1a6894af675d34"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "nalgebra"
 version = "0.29.0"
@@ -708,15 +749,15 @@
 name = "nalgebra-macros"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01fcc0b8149b4632adc89ac3b7b31a12fb6099a0317a4eb2ebff574ef7de7218"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
@@ -726,21 +767,21 @@
  "libc",
  "matrixmultiply",
  "num-complex",
  "num-integer",
  "num-traits",
  "rawpointer",
  "rayon",
+ "serde",
 ]
 
 [[package]]
 name = "ndarray-linalg"
 version = "0.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b0e8dda0c941b64a85c5deb2b3e0144aca87aced64678adfc23eacea6d2cc42"
+source = "git+https://github.com/Teamon9161/ndarray-linalg.git?branch=arm-cross-compile#a4766b28528bf77a7b901cf43fa3b037798d4212"
 dependencies = [
  "cauchy",
  "katexit",
  "lax",
  "ndarray",
  "num-complex",
  "num-traits",
@@ -785,17 +826,17 @@
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ae39348c8bc5fbd7f40c727a9925f03517afd2ab27d46702108b6a7e5414c19"
+checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
  "rand",
  "serde",
 ]
 
 [[package]]
@@ -839,27 +880,27 @@
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.13.1"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19e64526ebdee182341572e50e9ad03965aa510cd94427a4549448f285e957a1"
+checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96b0fee4571867d318651c24f4a570c3f18408cf95f16ccb576b3ce85496a46e"
+checksum = "437213adf41bbccf4aeae535fbfcdad0f6fed241e1ae182ebe97fa1f3ce19389"
 dependencies = [
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
@@ -882,15 +923,15 @@
 [[package]]
 name = "ocipkg"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60cf01280832705a4e4c4d046d9e67a54b900297c69191457a8fc6d198ddefa2"
 dependencies = [
  "base16ct",
- "base64",
+ "base64 0.13.1",
  "chrono",
  "directories",
  "flate2",
  "lazy_static",
  "log",
  "oci-spec",
  "regex",
@@ -904,113 +945,113 @@
  "url",
  "uuid",
  "walkdir",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.16.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f0b0d4bf799edbc74508c1e8bf170ff5f41238e5f8225603ca7caaae2b7860"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.3"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a279cbf25cb0757810394fbc1e359949b59e348145c643a939a525692e6929"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.9"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1de2e551fb905ac83f73f7aedf2f0cb4a0da7e35efa24a202a936269f1f18e1"
+checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pest"
-version = "2.5.4"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ab62d2fa33726dbe6321cc97ef96d8cde531e3eeaf858a058de53a8a6d40d8f"
+checksum = "e68e84bfb01f0507134eac1e9b410a12ba379d064eab48c50ba4ce329a527b70"
 dependencies = [
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_derive"
-version = "2.5.4"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8bf026e2d0581559db66d837fe5242320f525d85c76283c61f4d51a1238d65ea"
+checksum = "6b79d4c71c865a25a4322296122e3924d30bc8ee0834c8bfc8b95f7f054afbfb"
 dependencies = [
  "pest",
  "pest_generator",
 ]
 
 [[package]]
 name = "pest_generator"
-version = "2.5.4"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b27bd18aa01d91c8ed2b61ea23406a676b42d82609c6e2581fba42f0c15f17f"
+checksum = "6c435bf1076437b851ebc8edc3a18442796b30f1728ffea6262d59bbe28b077e"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.5.4"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f02b677c1859756359fc9983c2e56a0237f18624a3789528804406b7e915e5d"
+checksum = "745a452f8eb71e39ffd8ee32b3c5f51d03845f99786fa9b68db6ff509c505411"
 dependencies = [
  "once_cell",
  "pest",
  "sha2",
 ]
 
 [[package]]
 name = "ppv-lite86"
-version = "0.2.16"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb9f9e6e233e5c4a35559a617bf40a4ec447db2e84c20b55a6f83167b7e57872"
+checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro-error-attr"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1019,17 +1060,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.43"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0a2ca2c61bc9f3d74d2886294ab7b9853abd9c1ad903a3ac7815c58989bb7bab"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py_literal"
 version = "0.4.0"
@@ -1041,77 +1082,78 @@
  "num-traits",
  "pest",
  "pest_derive",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ccd4149c8c3975099622b4e1962dac27565cf5663b76452c3e2b66e0b6824277"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.8.0",
+ "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
+ "serde",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cd09fe469834db21ee60e0051030339e5d361293d8cb5ec02facf7fdcf52dbf"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c427c9a96b9c5b12156dbc11f76b14f49e9aae8905ca783ea87c249044ef137"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b822bbba9d60630a44d2109bc410489bb2f439b33e3a14ddeb8a40b378a7c4"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84ae898104f7c99db06231160770f3e40dad6eb9021daddc0fedfa3e41dff10a"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.21"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1156,29 +1198,27 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.5.3"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd99e5772ead8baa5215278c9b15bf92087709e9c1b2d1f97cdb5a183c933a7d"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
- "autocfg",
- "crossbeam-deque",
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.9.3"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "258bcdb5ac6dad48491bb2992db6b7cf74878b0384908af124823d118c99683f"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
@@ -1188,40 +1228,49 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
 name = "redox_users"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
 dependencies = [
  "getrandom",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.6.0"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c4eb3267174b8c6c2f654116623910a0fef09c4753f8dd83db29c48a0df988b"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.27"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3f87b73ce11b1619a3c6332f45341e0047173771e8b8b73f87bfeefb7b56244"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "ring"
 version = "0.16.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
 dependencies = [
@@ -1238,35 +1287,35 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustls"
-version = "0.20.6"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aab8ee6c7097ed6057f43c187a62418d0c05a4bd5f18b3571db50ee0f9ce033"
+checksum = "fff78fc74d175294f4e83b28343315ffcfb114b156f0185e9741cb5570f50e2f"
 dependencies = [
  "log",
  "ring",
  "sct",
  "webpki",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.11"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4501abdff3ae82a1c1b477a17252eb69cee9e66eb915c1abaa4f44d873df9f09"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "safe_arch"
-version = "0.6.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "794821e4ccb0d9f979512f9c1973480123f9bd62a90d74ab0f9426fcf8f4a529"
+checksum = "62a7484307bd40f8f7ccbacccac730108f2cae119a3b11c74485b48aa9ea650f"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
@@ -1279,61 +1328,96 @@
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
-name = "scratch"
-version = "1.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c8132065adcfd6e02db789d9285a0deb2f3fcb04002865ab67d5fb103533898"
-
-[[package]]
 name = "sct"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d53dcdb7c9f8158937a7981b48accfd39a43af418591a5d008c7b22b5e1b7ca4"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.145"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "728eb6351430bccb993660dfffc5a72f91ccc1295abaa8ce19b27ebe4f75568b"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
+name = "serde-pickle"
+version = "1.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c762ad136a26407c6a80825813600ceeab5e613660d93d79a41f0ec877171e71"
+dependencies = [
+ "byteorder",
+ "iter-read",
+ "num-bigint",
+ "num-traits",
+ "serde",
+]
+
+[[package]]
 name = "serde_derive"
-version = "1.0.145"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81fa1584d3d1bcacd84c277a0dfe21f5b0f6accf4a23d04d4c6d61f1af522b4c"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.86"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41feea4228a6f1cd09ec7a3593a682276702cd67b5273544757dae23c096f074"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_with"
+version = "3.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9f02d8aa6e3c385bf084924f660ce2a3a6bd333ba55b35e8590b321f35d88513"
+dependencies = [
+ "base64 0.21.2",
+ "chrono",
+ "hex",
+ "indexmap",
+ "serde",
+ "serde_json",
+ "serde_with_macros",
+ "time 0.3.22",
+]
+
+[[package]]
+name = "serde_with_macros"
+version = "3.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "edc7d5d3932fb12ce722ee5e64dd38c504efba37567f0c402f6ca728c3b8b070"
+dependencies = [
+ "darling 0.20.1",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+]
+
+[[package]]
 name = "sha2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
 dependencies = [
  "cfg-if",
  "cpufeatures",
@@ -1351,17 +1435,17 @@
  "num-traits",
  "paste",
  "wide",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fd0db749597d91ff862fd1d55ea87f7855a744a8425a64695b6fca237d1dad1"
+checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
 
@@ -1382,17 +1466,28 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "syn"
-version = "1.0.99"
+version = "1.0.109"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "syn"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58dbef6ec655055e20b86b15a8cc6d439cca19b667537ac6a1369572d151ab13"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1404,205 +1499,220 @@
  "filetime",
  "libc",
  "xattr",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.4"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "teapy"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
  "ahash",
+ "bincode",
  "chrono",
  "cxx",
  "lapack-sys",
  "ndarray",
  "ndarray-linalg",
  "ndarray-npy",
  "num",
  "numpy",
  "once_cell",
  "pyo3",
  "rayon",
+ "regex",
+ "serde",
+ "serde-pickle",
+ "serde_with",
  "statrs",
 ]
 
 [[package]]
-name = "termcolor"
-version = "1.1.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
-dependencies = [
- "winapi-util",
-]
-
-[[package]]
 name = "thiserror"
-version = "1.0.37"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10deb33631e3c9018b9baf9dcbbc4f737320d2b576bac10f6aefa048fa407e3e"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.37"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "982d17546b47146b28f7c22e3d08465f6b8903d0ea13c1660d9d84a6e7adcdbb"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "time"
-version = "0.1.44"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db9e6914ab8b1ae1c260a4ae7a49b6c5611b40328a735b21862567685e73255"
+checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
 dependencies = [
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
+name = "time"
+version = "0.3.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
+dependencies = [
+ "itoa",
+ "serde",
+ "time-core",
+ "time-macros",
+]
+
+[[package]]
+name = "time-core"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+
+[[package]]
+name = "time-macros"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
+dependencies = [
+ "time-core",
+]
+
+[[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
  "tinyvec_macros",
 ]
 
 [[package]]
 name = "tinyvec_macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cda74da7e1a664f795bb1f8a87ec406fb89a02522cf6e50620d016add6dbbf5c"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "toml"
-version = "0.5.9"
+version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d82e1a7758622a465f8cee077614c73484dac5b836c02ff6a40d5d1010324d7"
+checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "typenum"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dcf81ac59edc17cc8697ff311e8f5ef2d99fcbd9817b34cec66f90b6c3dfd987"
+checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "ucd-trie"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.8"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "099b7128301d285f79ddd55b9a83d5e6b9e97c92e0ea0daebee7263e932de992"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.3"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4f5b37a154999a8f3f98cc23a628d850e154479cd94decf3414696e12e31aaf"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
-name = "unicode-width"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
-
-[[package]]
 name = "unindent"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ee9362deb4a96cef4d437d1ad49cffc9b9e92d202b6995674e928ce684f112"
+checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
 [[package]]
 name = "ureq"
-version = "2.5.0"
+version = "2.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b97acb4c28a254fd7a4aeec976c46a7fa404eac4d7c134b30c75144846d7cb8f"
+checksum = "338b31dd1314f68f3aabf3ed57ab922df95ffcd902476ca7ba3c4ce7b908c46d"
 dependencies = [
- "base64",
- "chunked_transfer",
+ "base64 0.13.1",
  "flate2",
  "log",
  "once_cell",
  "rustls",
  "serde",
  "serde_json",
  "url",
  "webpki",
  "webpki-roots",
 ]
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.2.1"
+version = "1.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "feb41e78f93363bb2df8b0e86a2ca30eed7806ea16ea0c790d757cf93f79be83"
+checksum = "0fa2982af2eec27de306107c027578ff7f423d65f7250e40ce0fea8f45248b81"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.3.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "808cf2735cd4b6866113f648b791c6adc5714537bc222d9347bb203386ffda56"
+checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
- "winapi",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.10.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1612,71 +1722,71 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaf9f5aceeec8be17c128b2e93e031fb8a4d469bb9c4ae2d7dc1888b26887268"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "052be0f94026e6cbc75cdefc9bae13fd6052cdcaf532fa6c45e7ae33a1e6c810"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "web-sys"
-version = "0.3.60"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcda906d8be16e728fd5adc5b729afad4e444e106ab28cd1c7256e54fa61510f"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki"
@@ -1686,26 +1796,26 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "webpki-roots"
-version = "0.22.5"
+version = "0.22.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "368bfe657969fb01238bb756d351dcade285e0f6fcbd36dcb23359a5169975be"
+checksum = "b6c71e40d7d2c34a5106301fb632274ca37242cd0c9d3e64dbece371a40a2d87"
 dependencies = [
  "webpki",
 ]
 
 [[package]]
 name = "wide"
-version = "0.7.5"
+version = "0.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae41ecad2489a1655c8ef8489444b0b113c0a0c795944a3572a0931cf7d2525c"
+checksum = "40018623e2dba2602a9790faba8d33f2ebdebf4b86561b83928db735f8784728"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "winapi"
@@ -1735,55 +1845,87 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
 name = "windows-sys"
-version = "0.36.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea04155a16a59f9eab786fe12a4a450e75cdb175f9e0d80da1e17db09f55b8d2"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
+ "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
-version = "0.36.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9bb8c3fd39ade2d67e9874ac4f3db21f0d710bee00fe7cab16949ec184eeaa47"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.36.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180e6ccf01daf4c426b846dfc66db1fc518f074baa793aa7d9b9aaeffad6a3b6"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.36.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2e7917148b2812d1eeafaeb22a97e4813dfa60a3f8f78ebe204bcc88f12f024"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.36.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dcd171b8776c41b97521e5da127a2d86ad280114807d0b2ab1e462bc764d9e1"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.36.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c811ca4a8c853ef420abd8592ba53ddbbac90410fab6903b3e79972a631f7680"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "xattr"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d1526bbe5aaeb5eb06885f4d987bcdfa5e23187055de9b83fe00156a821fabc"
 dependencies = [
```

### Comparing `teapy-0.1.6/PKG-INFO` & `teapy-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: teapy
-Version: 0.1.6
+Version: 0.1.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: numpy >=1.16.0
 License-File: LICENSE
 Summary: A blazingly fast datadict library
 Author-email: Teamon <teamon9161@163.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Teapy
 [![Build](https://github.com/teamon9161/teapy/workflows/Build/badge.svg)](https://github.com/teamon9161/teapy/actions)
+[![PyPI](https://img.shields.io/pypi/v/teapy)](https://pypi.org/project/teapy)
 [![codecov](https://codecov.io/gh/teamon9161/teapy/branch/master/graph/badge.svg?token=WK0F7P1VC6)](https://codecov.io/gh/teamon9161/teapy)
 
 ## Blazingly fast datadict library in Python
 
 Teapy is a blazingly fast datadict library implemented in Rust.
 * Lazy evaluation
 * Handle NaN
```

