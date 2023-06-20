# Comparing `tmp/qiskit-symb-0.1.2.tar.gz` & `tmp/qiskit-symb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-symb-0.1.2.tar", last modified: Tue May 16 12:46:04 2023, max compression
+gzip compressed data, was "qiskit-symb-0.1.3.tar", last modified: Tue Jun 20 14:23:45 2023, max compression
```

## Comparing `qiskit-symb-0.1.2.tar` & `qiskit-symb-0.1.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:04.544389 qiskit-symb-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-05-16 12:46:04.544389 qiskit-symb-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 12:46:04.548389 qiskit-symb-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:04.536389 qiskit-symb-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:04.540389 qiskit-symb-0.1.2/src/qiskit_symb/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:04.540389 qiskit-symb-0.1.2/src/qiskit_symb/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/controlledgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/gate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:04.540389 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:04.544389 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/p.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/r.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/rx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/rxx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/ry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/ryy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/rz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/rzx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/rzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/u.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:04.544389 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/ecr.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/h.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/i.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/iswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/s.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/sx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/t.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/x.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/y.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/z.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/circuit/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:04.544389 qiskit-symb-0.1.2/src/qiskit_symb/quantum_info/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/quantum_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/quantum_info/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/quantum_info/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/quantum_info/quantumbase.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/quantum_info/statevector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/src/qiskit_symb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:04.540389 qiskit-symb-0.1.2/src/qiskit_symb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-05-16 12:46:04.000000 qiskit-symb-0.1.2/src/qiskit_symb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-16 12:46:04.000000 qiskit-symb-0.1.2/src/qiskit_symb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:46:04.000000 qiskit-symb-0.1.2/src/qiskit_symb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:46:04.000000 qiskit-symb-0.1.2/src/qiskit_symb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 12:46:04.000000 qiskit-symb-0.1.2/src/qiskit_symb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 12:46:04.000000 qiskit-symb-0.1.2/src/qiskit_symb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:04.544389 qiskit-symb-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/tests/test_ctrl_parametric_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/tests/test_ctrl_standard_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/tests/test_densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/tests/test_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/tests/test_parametric_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/tests/test_standard_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-16 12:45:51.000000 qiskit-symb-0.1.2/tests/test_statevector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:45.405780 qiskit-symb-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-20 14:23:45.405780 qiskit-symb-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 14:23:45.405780 qiskit-symb-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:45.397780 qiskit-symb-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:45.397780 qiskit-symb-0.1.3/src/qiskit_symb/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:45.401780 qiskit-symb-0.1.3/src/qiskit_symb/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/controlledgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/gate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:45.401780 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:45.401780 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/rx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/rxx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/ry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/ryy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/rz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/rzx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/rzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/u.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:45.401780 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/ecr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/h.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/i.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/iswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/sx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/y.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/circuit/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:45.405780 qiskit-symb-0.1.3/src/qiskit_symb/quantum_info/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/quantum_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/quantum_info/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/quantum_info/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/quantum_info/quantumbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/quantum_info/statevector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/src/qiskit_symb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:45.397780 qiskit-symb-0.1.3/src/qiskit_symb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-06-20 14:23:45.000000 qiskit-symb-0.1.3/src/qiskit_symb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-20 14:23:45.000000 qiskit-symb-0.1.3/src/qiskit_symb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:23:45.000000 qiskit-symb-0.1.3/src/qiskit_symb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:23:45.000000 qiskit-symb-0.1.3/src/qiskit_symb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 14:23:45.000000 qiskit-symb-0.1.3/src/qiskit_symb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 14:23:45.000000 qiskit-symb-0.1.3/src/qiskit_symb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:23:45.405780 qiskit-symb-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/tests/test_ctrl_parametric_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/tests/test_ctrl_standard_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/tests/test_densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/tests/test_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/tests/test_parametric_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/tests/test_standard_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-20 14:23:30.000000 qiskit-symb-0.1.3/tests/test_statevector.py
```

### Comparing `qiskit-symb-0.1.2/LICENSE` & `qiskit-symb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/PKG-INFO` & `qiskit-symb-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7169 736b  : 2.1.Name: qisk
 00000020: 6974 2d73 796d 620a 5665 7273 696f 6e3a  it-symb.Version:
-00000030: 2030 2e31 2e32 0a48 6f6d 652d 7061 6765   0.1.2.Home-page
+00000030: 2030 2e31 2e33 0a48 6f6d 652d 7061 6765   0.1.3.Home-page
 00000040: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
 00000050: 2e63 6f6d 2f53 696d 6f6e 6547 6173 7065  .com/SimoneGaspe
 00000060: 7269 6e69 2f71 6973 6b69 742d 7379 6d62  rini/qiskit-symb
 00000070: 0a41 7574 686f 723a 2053 696d 6f6e 6547  .Author: SimoneG
 00000080: 6173 7065 7269 6e69 0a41 7574 686f 722d  asperini.Author-
 00000090: 656d 6169 6c3a 2073 696d 6f6e 652e 6761  email: simone.ga
 000000a0: 7370 6572 696e 6934 4075 6e69 626f 2e69  sperini4@unibo.i
@@ -26,396 +26,379 @@
 00000190: 6261 6467 652f 6c69 6365 6e73 652d 4170  badge/license-Ap
 000001a0: 6163 6865 5f32 2e30 2d62 6c75 652e 7376  ache_2.0-blue.sv
 000001b0: 6722 3e0a 2020 2020 3c69 6d67 2074 6974  g">.    <img tit
 000001c0: 6c65 3d22 7079 7468 6f6e 2220 7372 633d  le="python" src=
 000001d0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
 000001e0: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
 000001f0: 7468 6f6e 2de2 89a5 332e 382d 626c 7565  thon-...3.8-blue
-00000200: 2e73 7667 223e 0a20 2020 203c 696d 6720  .svg">.    <img 
-00000210: 7469 746c 653d 2245 636f 7379 7374 656d  title="Ecosystem
-00000220: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00000230: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000240: 6467 652f 5169 736b 6974 2d45 636f 7379  dge/Qiskit-Ecosy
-00000250: 7374 656d 2d62 6c75 6576 696f 6c65 742e  stem-blueviolet.
-00000260: 7376 6722 3e0a 3c2f 703e 0a0a 3c70 2061  svg">.</p>..<p a
-00000270: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
-00000280: 2020 203c 696d 6720 7469 746c 653d 2262     <img title="b
-00000290: 7569 6c64 2220 7372 633d 2768 7474 7073  uild" src='https
-000002a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5369  ://github.com/Si
-000002b0: 6d6f 6e65 4761 7370 6572 696e 692f 7169  moneGasperini/qi
-000002c0: 736b 6974 2d73 796d 622f 6163 7469 6f6e  skit-symb/action
-000002d0: 732f 776f 726b 666c 6f77 732f 7079 7468  s/workflows/pyth
-000002e0: 6f6e 2d70 6163 6b61 6765 2e79 6d6c 2f62  on-package.yml/b
-000002f0: 6164 6765 2e73 7667 3f62 7261 6e63 683d  adge.svg?branch=
-00000300: 6d61 7374 6572 273e 0a20 2020 203c 696d  master'>.    <im
-00000310: 6720 7469 746c 653d 2263 6f76 6572 6167  g title="coverag
-00000320: 6522 2073 7263 3d27 6874 7470 733a 2f2f  e" src='https://
-00000330: 636f 7665 7261 6c6c 732e 696f 2f72 6570  coveralls.io/rep
-00000340: 6f73 2f67 6974 6875 622f 5369 6d6f 6e65  os/github/Simone
-00000350: 4761 7370 6572 696e 692f 7169 736b 6974  Gasperini/qiskit
-00000360: 2d73 796d 622f 6261 6467 652e 7376 673f  -symb/badge.svg?
-00000370: 6272 616e 6368 3d6d 6173 7465 7227 3e0a  branch=master'>.
-00000380: 3c2f 703e 0a0a 2a2a 2a0a 0a23 2054 6162  </p>..***..# Tab
-00000390: 6c65 206f 6620 636f 6e74 656e 7473 0a2d  le of contents.-
-000003a0: 205b 496e 7472 6f64 7563 7469 6f6e 5d28   [Introduction](
-000003b0: 2369 6e74 726f 6475 6374 696f 6e29 0a2d  #introduction).-
-000003c0: 205b 496e 7374 616c 6c61 7469 6f6e 5d28   [Installation](
-000003d0: 2369 6e73 7461 6c6c 6174 696f 6e29 0a20  #installation). 
-000003e0: 2020 202d 205b 5573 6572 2d6d 6f64 655d     - [User-mode]
-000003f0: 2823 7573 6572 2d6d 6f64 6529 0a20 2020  (#user-mode).   
-00000400: 202d 205b 4465 762d 6d6f 6465 5d28 2364   - [Dev-mode](#d
-00000410: 6576 2d6d 6f64 6529 0a2d 205b 5573 6167  ev-mode).- [Usag
-00000420: 6520 6578 616d 706c 6573 5d28 2375 7361  e examples](#usa
-00000430: 6765 2d65 7861 6d70 6c65 7329 0a20 2020  ge-examples).   
-00000440: 202d 205b 5f53 796d 7069 6679 5f20 6120   - [_Sympify_ a 
-00000450: 5169 736b 6974 2063 6972 6375 6974 5d28  Qiskit circuit](
-00000460: 2373 796d 7069 6679 2d61 2d71 6973 6b69  #sympify-a-qiski
-00000470: 742d 6369 7263 7569 7429 0a20 2020 202d  t-circuit).    -
-00000480: 205b 5f4c 616d 6264 6966 795f 2061 2051   [_Lambdify_ a Q
-00000490: 6973 6b69 7420 6369 7263 7569 745d 2823  iskit circuit](#
-000004a0: 6c61 6d62 6469 6679 2d61 2d71 6973 6b69  lambdify-a-qiski
-000004b0: 742d 6369 7263 7569 7429 0a2d 205b 436f  t-circuit).- [Co
-000004c0: 6e74 7269 6275 746f 7273 5d28 2363 6f6e  ntributors](#con
-000004d0: 7472 6962 7574 6f72 7329 0a0a 0a23 2049  tributors)...# I
-000004e0: 6e74 726f 6475 6374 696f 6e0a 5468 6520  ntroduction.The 
-000004f0: 6071 6973 6b69 742d 7379 6d62 6020 7061  `qiskit-symb` pa
-00000500: 636b 6167 6520 6973 206d 6561 6e74 2074  ckage is meant t
-00000510: 6f20 6265 2061 2050 7974 686f 6e20 746f  o be a Python to
-00000520: 6f6c 2074 6f20 656e 6162 6c65 2074 6865  ol to enable the
-00000530: 2073 796d 626f 6c69 6320 6576 616c 7561   symbolic evalua
-00000540: 7469 6f6e 206f 6620 7061 7261 6d65 7472  tion of parametr
-00000550: 6963 2071 7561 6e74 756d 2073 7461 7465  ic quantum state
-00000560: 7320 616e 6420 6f70 6572 6174 6f72 7320  s and operators 
-00000570: 6465 6669 6e65 6420 696e 205b 5169 736b  defined in [Qisk
-00000580: 6974 5d28 6874 7470 733a 2f2f 6769 7468  it](https://gith
-00000590: 7562 2e63 6f6d 2f51 6973 6b69 742f 7169  ub.com/Qiskit/qi
-000005a0: 736b 6974 2d74 6572 7261 2920 6279 2070  skit-terra) by p
-000005b0: 6172 616d 6574 6572 697a 6564 2071 7561  arameterized qua
-000005c0: 6e74 756d 2063 6972 6375 6974 732e 0a0a  ntum circuits...
-000005d0: 4120 5061 7261 6d65 7465 7269 7a65 6420  A Parameterized 
-000005e0: 5175 616e 7475 6d20 4369 7263 7569 7420  Quantum Circuit 
-000005f0: 2850 5143 2920 6973 2061 2071 7561 6e74  (PQC) is a quant
-00000600: 756d 2063 6972 6375 6974 2077 6865 7265  um circuit where
-00000610: 2077 6520 6861 7665 2061 7420 6c65 6173   we have at leas
-00000620: 7420 6f6e 6520 6672 6565 2070 6172 616d  t one free param
-00000630: 6574 6572 2028 652e 672e 2061 2072 6f74  eter (e.g. a rot
-00000640: 6174 696f 6e20 616e 676c 6520 245c 7468  ation angle $\th
-00000650: 6574 6124 292e 2050 5143 7320 6172 6520  eta$). PQCs are 
-00000660: 7061 7274 6963 756c 6172 6c79 2072 656c  particularly rel
-00000670: 6576 616e 7420 696e 2051 7561 6e74 756d  evant in Quantum
-00000680: 204d 6163 6869 6e65 204c 6561 726e 696e   Machine Learnin
-00000690: 6720 2851 4d4c 2920 6d6f 6465 6c73 2c20  g (QML) models, 
-000006a0: 7768 6572 6520 7468 6520 7661 6c75 6573  where the values
-000006b0: 206f 6620 7468 6573 6520 7061 7261 6d65   of these parame
-000006c0: 7465 7273 2063 616e 2062 6520 6c65 6172  ters can be lear
-000006d0: 6e65 6420 6475 7269 6e67 2074 7261 696e  ned during train
-000006e0: 696e 6720 746f 2072 6561 6368 2074 6865  ing to reach the
-000006f0: 2064 6573 6972 6564 206f 7574 7075 742e   desired output.
-00000700: 0a0a 496e 2070 6172 7469 6375 6c61 722c  ..In particular,
-00000710: 2060 7169 736b 6974 2d73 796d 6260 2063   `qiskit-symb` c
-00000720: 616e 2062 6520 7573 6564 2074 6f20 6372  an be used to cr
-00000730: 6561 7465 2061 2073 796d 626f 6c69 6320  eate a symbolic 
-00000740: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-00000750: 6620 6120 7061 7261 6d65 7472 6963 2071  f a parametric q
-00000760: 7561 6e74 756d 2073 7461 7465 7665 6374  uantum statevect
-00000770: 6f72 2c20 6465 6e73 6974 7920 6d61 7472  or, density matr
-00000780: 6978 2c20 6f72 2075 6e69 7461 7279 206f  ix, or unitary o
-00000790: 7065 7261 746f 7220 6469 7265 6374 6c79  perator directly
-000007a0: 2066 726f 6d20 7468 6520 5169 736b 6974   from the Qiskit
-000007b0: 2071 7561 6e74 756d 2063 6972 6375 6974   quantum circuit
-000007c0: 2e20 5468 6973 2068 6173 2062 6565 6e20  . This has been 
-000007d0: 6163 6869 6576 6564 2074 6872 6f75 6768  achieved through
-000007e0: 2074 6865 2072 652d 696d 706c 656d 656e   the re-implemen
-000007f0: 7461 7469 6f6e 206f 6620 736f 6d65 2062  tation of some b
-00000800: 6173 6963 2063 6c61 7373 6573 2064 6566  asic classes def
-00000810: 696e 6564 2069 6e20 7468 6520 5b60 7169  ined in the [`qi
-00000820: 736b 6974 2f71 7561 6e74 756d 5f69 6e66  skit/quantum_inf
-00000830: 6f2f 605d 2868 7474 7073 3a2f 2f67 6974  o/`](https://git
-00000840: 6875 622e 636f 6d2f 5169 736b 6974 2f71  hub.com/Qiskit/q
-00000850: 6973 6b69 742d 7465 7272 612f 7472 6565  iskit-terra/tree
-00000860: 2f6d 6169 6e2f 7169 736b 6974 2f71 7561  /main/qiskit/qua
-00000870: 6e74 756d 5f69 6e66 6f29 206d 6f64 756c  ntum_info) modul
-00000880: 6520 6279 2075 7369 6e67 205b 7379 6d70  e by using [symp
-00000890: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-000008a0: 622e 636f 6d2f 7379 6d70 792f 7379 6d70  b.com/sympy/symp
-000008b0: 7929 2061 7320 6120 6261 636b 656e 6420  y) as a backend 
-000008c0: 666f 7220 7379 6d62 6f6c 6963 2065 7870  for symbolic exp
-000008d0: 7265 7373 696f 6e73 206d 616e 6970 756c  ressions manipul
-000008e0: 6174 696f 6e2e 0a0a 0a23 2049 6e73 7461  ation....# Insta
-000008f0: 6c6c 6174 696f 6e0a 0a23 2320 5573 6572  llation..## User
-00000900: 2d6d 6f64 650a 6060 600a 7069 7020 696e  -mode.```.pip in
-00000910: 7374 616c 6c20 7169 736b 6974 2d73 796d  stall qiskit-sym
-00000920: 620a 6060 600a 0a23 2320 4465 762d 6d6f  b.```..## Dev-mo
-00000930: 6465 0a60 6060 0a67 6974 2063 6c6f 6e65  de.```.git clone
-00000940: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000950: 636f 6d2f 5369 6d6f 6e65 4761 7370 6572  com/SimoneGasper
-00000960: 696e 692f 7169 736b 6974 2d73 796d 622e  ini/qiskit-symb.
-00000970: 6769 740a 6364 2071 6973 6b69 742d 7379  git.cd qiskit-sy
-00000980: 6d62 0a70 6970 2069 6e73 7461 6c6c 202d  mb.pip install -
-00000990: 6520 2e0a 6060 600a 0a0a 2320 5573 6167  e ..```...# Usag
-000009a0: 6520 6578 616d 706c 6573 0a0a 2323 2320  e examples..### 
-000009b0: 5f53 796d 7069 6679 5f20 6120 5169 736b  _Sympify_ a Qisk
-000009c0: 6974 2063 6972 6375 6974 0a4c 6574 2773  it circuit.Let's
-000009d0: 2067 6574 2073 7461 7274 6564 206f 6e20   get started on 
-000009e0: 686f 7720 746f 2075 7365 2060 7169 736b  how to use `qisk
-000009f0: 6974 2d73 796d 6260 2074 6f20 6765 7420  it-symb` to get 
-00000a00: 7468 6520 7379 6d62 6f6c 6963 2072 6570  the symbolic rep
-00000a10: 7265 7365 6e74 6174 696f 6e20 6f66 2061  resentation of a
-00000a20: 2067 6976 656e 2051 6973 6b69 7420 6369   given Qiskit ci
-00000a30: 7263 7569 742e 2049 6e20 7061 7274 6963  rcuit. In partic
-00000a40: 756c 6172 2c20 696e 2074 6869 7320 6669  ular, in this fi
-00000a50: 7273 7420 6261 7369 6320 6578 616d 706c  rst basic exampl
-00000a60: 652c 2077 6520 636f 6e73 6964 6572 2074  e, we consider t
-00000a70: 6865 2066 6f6c 6c6f 7769 6e67 2071 7561  he following qua
-00000a80: 6e74 756d 2063 6972 6375 6974 3a0a 6060  ntum circuit:.``
-00000a90: 6070 7974 686f 6e0a 6672 6f6d 2071 6973  `python.from qis
-00000aa0: 6b69 7420 696d 706f 7274 2051 7561 6e74  kit import Quant
-00000ab0: 756d 4369 7263 7569 740a 6672 6f6d 2071  umCircuit.from q
-00000ac0: 6973 6b69 742e 6369 7263 7569 7420 696d  iskit.circuit im
-00000ad0: 706f 7274 2050 6172 616d 6574 6572 2c20  port Parameter, 
-00000ae0: 5061 7261 6d65 7465 7256 6563 746f 720a  ParameterVector.
-00000af0: 0a79 203d 2050 6172 616d 6574 6572 2827  .y = Parameter('
-00000b00: 7927 290a 7020 3d20 5061 7261 6d65 7465  y').p = Paramete
-00000b10: 7256 6563 746f 7228 2770 272c 206c 656e  rVector('p', len
-00000b20: 6774 683d 3229 0a0a 7071 6320 3d20 5175  gth=2)..pqc = Qu
-00000b30: 616e 7475 6d43 6972 6375 6974 2832 290a  antumCircuit(2).
-00000b40: 7071 632e 7279 2879 2c20 3029 0a70 7163  pqc.ry(y, 0).pqc
-00000b50: 2e63 7828 302c 2031 290a 7071 632e 7528  .cx(0, 1).pqc.u(
-00000b60: 302c 202a 702c 2031 290a 0a70 7163 2e64  0, *p, 1)..pqc.d
-00000b70: 7261 7728 276d 706c 2729 0a60 6060 0a21  raw('mpl').```.!
-00000b80: 5b5d 282f 696d 672f 6578 616d 706c 655f  [](/img/example_
-00000b90: 6369 7263 7569 742e 706e 6729 0a0a 546f  circuit.png)..To
-00000ba0: 2067 6574 2074 6865 202a 7379 6d70 792a   get the *sympy*
-00000bb0: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-00000bc0: 6f66 2074 6865 2075 6e69 7461 7279 206d  of the unitary m
-00000bd0: 6174 7269 7820 636f 7272 6573 706f 6e64  atrix correspond
-00000be0: 696e 6720 746f 2074 6865 2070 6172 616d  ing to the param
-00000bf0: 6574 6572 697a 6564 2063 6972 6375 6974  eterized circuit
-00000c00: 2c20 7765 206a 7573 7420 6861 7665 2074  , we just have t
-00000c10: 6f20 6372 6561 7465 2074 6865 2073 796d  o create the sym
-00000c20: 626f 6c69 6320 604f 7065 7261 746f 7260  bolic `Operator`
-00000c30: 2069 6e73 7461 6e63 6520 616e 6420 6361   instance and ca
-00000c40: 6c6c 2074 6865 2060 746f 5f73 796d 7079  ll the `to_sympy
-00000c50: 2829 6020 6d65 7468 6f64 3a0a 6060 6070  ()` method:.```p
-00000c60: 7974 686f 6e0a 6672 6f6d 2071 6973 6b69  ython.from qiski
-00000c70: 745f 7379 6d62 2e71 7561 6e74 756d 5f69  t_symb.quantum_i
-00000c80: 6e66 6f20 696d 706f 7274 204f 7065 7261  nfo import Opera
-00000c90: 746f 720a 0a6f 7020 3d20 4f70 6572 6174  tor..op = Operat
-00000ca0: 6f72 2870 7163 290a 6f70 2e74 6f5f 7379  or(pqc).op.to_sy
-00000cb0: 6d70 7928 290a 6060 600a 6060 606d 6174  mpy().```.```mat
-00000cc0: 680a 5c6c 6566 745b 5c62 6567 696e 7b6d  h.\left[\begin{m
-00000cd0: 6174 7269 787d 5c63 6f73 7b5c 6c65 6674  atrix}\cos{\left
-00000ce0: 285c 6672 6163 7b79 7d7b 327d 205c 7269  (\frac{y}{2} \ri
-00000cf0: 6768 7429 7d20 2620 2d20 5c73 696e 7b5c  ght)} & - \sin{\
-00000d00: 6c65 6674 285c 6672 6163 7b79 7d7b 327d  left(\frac{y}{2}
-00000d10: 205c 7269 6768 7429 7d20 2620 3020 2620   \right)} & 0 & 
-00000d20: 305c 5c30 2026 2030 2026 205c 7369 6e7b  0\\0 & 0 & \sin{
-00000d30: 5c6c 6566 7428 5c66 7261 637b 797d 7b32  \left(\frac{y}{2
-00000d40: 7d20 5c72 6967 6874 297d 2026 205c 636f  } \right)} & \co
-00000d50: 737b 5c6c 6566 7428 5c66 7261 637b 797d  s{\left(\frac{y}
-00000d60: 7b32 7d20 5c72 6967 6874 297d 5c5c 3020  {2} \right)}\\0 
-00000d70: 2620 3020 2620 655e 7b69 205c 6c65 6674  & 0 & e^{i \left
-00000d80: 2870 5b30 5d20 2b20 705b 315d 5c72 6967  (p[0] + p[1]\rig
-00000d90: 6874 297d 205c 636f 737b 5c6c 6566 7428  ht)} \cos{\left(
-00000da0: 5c66 7261 637b 797d 7b32 7d20 5c72 6967  \frac{y}{2} \rig
-00000db0: 6874 297d 2026 202d 2065 5e7b 6920 5c6c  ht)} & - e^{i \l
-00000dc0: 6566 7428 705b 305d 202b 2070 5b31 5d5c  eft(p[0] + p[1]\
-00000dd0: 7269 6768 7429 7d20 5c73 696e 7b5c 6c65  right)} \sin{\le
-00000de0: 6674 285c 6672 6163 7b79 7d7b 327d 205c  ft(\frac{y}{2} \
-00000df0: 7269 6768 7429 7d5c 5c65 5e7b 6920 5c6c  right)}\\e^{i \l
-00000e00: 6566 7428 705b 305d 202b 2070 5b31 5d5c  eft(p[0] + p[1]\
-00000e10: 7269 6768 7429 7d20 5c73 696e 7b5c 6c65  right)} \sin{\le
-00000e20: 6674 285c 6672 6163 7b79 7d7b 327d 205c  ft(\frac{y}{2} \
-00000e30: 7269 6768 7429 7d20 2620 655e 7b69 205c  right)} & e^{i \
-00000e40: 6c65 6674 2870 5b30 5d20 2b20 705b 315d  left(p[0] + p[1]
-00000e50: 5c72 6967 6874 297d 205c 636f 737b 5c6c  \right)} \cos{\l
-00000e60: 6566 7428 5c66 7261 637b 797d 7b32 7d20  eft(\frac{y}{2} 
-00000e70: 5c72 6967 6874 297d 2026 2030 2026 2030  \right)} & 0 & 0
-00000e80: 5c65 6e64 7b6d 6174 7269 787d 5c72 6967  \end{matrix}\rig
-00000e90: 6874 5d0a 6060 600a 0a49 6620 796f 7520  ht].```..If you 
-00000ea0: 7761 6e74 2074 6865 6e20 746f 2061 7373  want then to ass
-00000eb0: 6967 6e20 6120 7661 6c75 6520 746f 2073  ign a value to s
-00000ec0: 6f6d 6520 7370 6563 6966 6963 2070 6172  ome specific par
-00000ed0: 616d 6574 6572 2c20 796f 7520 6361 6e20  ameter, you can 
-00000ee0: 7573 6520 7468 6520 6073 7562 7328 3c64  use the `subs(<d
-00000ef0: 6963 743e 2960 206d 6574 686f 6420 7061  ict>)` method pa
-00000f00: 7373 696e 6720 6120 6469 6374 696f 6e61  ssing a dictiona
-00000f10: 7279 2074 6861 7420 6d61 7073 2065 6163  ry that maps eac
-00000f20: 6820 7061 7261 6d65 7465 7220 746f 2074  h parameter to t
-00000f30: 6865 2064 6573 6972 6564 2063 6f72 7265  he desired corre
-00000f40: 7370 6f6e 6469 6e67 2076 616c 7565 3a0a  sponding value:.
-00000f50: 6060 6070 7974 686f 6e0a 7061 7261 6d73  ```python.params
-00000f60: 3276 616c 7565 203d 207b 703a 205b 2d31  2value = {p: [-1
-00000f70: 2c20 325d 7d0a 6e65 775f 6f70 203d 206f  , 2]}.new_op = o
-00000f80: 702e 7375 6273 2870 6172 616d 7332 7661  p.subs(params2va
-00000f90: 6c75 6529 0a6e 6577 5f6f 702e 746f 5f73  lue).new_op.to_s
-00000fa0: 796d 7079 2829 0a60 6060 0a60 6060 6d61  ympy().```.```ma
-00000fb0: 7468 0a5c 6c65 6674 5b5c 6265 6769 6e7b  th.\left[\begin{
-00000fc0: 6d61 7472 6978 7d5c 636f 737b 5c6c 6566  matrix}\cos{\lef
-00000fd0: 7428 5c66 7261 637b 797d 7b32 7d20 5c72  t(\frac{y}{2} \r
-00000fe0: 6967 6874 297d 2026 202d 205c 7369 6e7b  ight)} & - \sin{
-00000ff0: 5c6c 6566 7428 5c66 7261 637b 797d 7b32  \left(\frac{y}{2
-00001000: 7d20 5c72 6967 6874 297d 2026 2030 2026  } \right)} & 0 &
-00001010: 2030 5c5c 3020 2620 3020 2620 5c73 696e   0\\0 & 0 & \sin
-00001020: 7b5c 6c65 6674 285c 6672 6163 7b79 7d7b  {\left(\frac{y}{
-00001030: 327d 205c 7269 6768 7429 7d20 2620 5c63  2} \right)} & \c
-00001040: 6f73 7b5c 6c65 6674 285c 6672 6163 7b79  os{\left(\frac{y
-00001050: 7d7b 327d 205c 7269 6768 7429 7d5c 5c30  }{2} \right)}\\0
-00001060: 2026 2030 2026 2065 5e7b 697d 205c 636f   & 0 & e^{i} \co
-00001070: 737b 5c6c 6566 7428 5c66 7261 637b 797d  s{\left(\frac{y}
-00001080: 7b32 7d20 5c72 6967 6874 297d 2026 202d  {2} \right)} & -
-00001090: 2065 5e7b 697d 205c 7369 6e7b 5c6c 6566   e^{i} \sin{\lef
-000010a0: 7428 5c66 7261 637b 797d 7b32 7d20 5c72  t(\frac{y}{2} \r
-000010b0: 6967 6874 297d 5c5c 655e 7b69 7d20 5c73  ight)}\\e^{i} \s
-000010c0: 696e 7b5c 6c65 6674 285c 6672 6163 7b79  in{\left(\frac{y
-000010d0: 7d7b 327d 205c 7269 6768 7429 7d20 2620  }{2} \right)} & 
-000010e0: 655e 7b69 7d20 5c63 6f73 7b5c 6c65 6674  e^{i} \cos{\left
-000010f0: 285c 6672 6163 7b79 7d7b 327d 205c 7269  (\frac{y}{2} \ri
-00001100: 6768 7429 7d20 2620 3020 2620 305c 656e  ght)} & 0 & 0\en
-00001110: 647b 6d61 7472 6978 7d5c 7269 6768 745d  d{matrix}\right]
-00001120: 0a60 6060 0a0a 2323 2320 5f4c 616d 6264  .```..### _Lambd
-00001130: 6966 795f 2061 2051 6973 6b69 7420 6369  ify_ a Qiskit ci
-00001140: 7263 7569 740a 4769 7665 6e20 6120 5169  rcuit.Given a Qi
-00001150: 736b 6974 2063 6972 6375 6974 2c20 6071  skit circuit, `q
-00001160: 6973 6b69 742d 7379 6d62 6020 616c 736f  iskit-symb` also
-00001170: 2061 6c6c 6f77 7320 746f 2067 656e 6572   allows to gener
-00001180: 6174 6520 6120 5079 7468 6f6e 206c 616d  ate a Python lam
-00001190: 6264 6120 6675 6e63 7469 6f6e 2077 6974  bda function wit
-000011a0: 6820 6163 7475 616c 2061 7267 756d 656e  h actual argumen
-000011b0: 7473 206d 6174 6368 696e 6720 7468 6520  ts matching the 
-000011c0: 5169 736b 6974 2075 6e62 6f75 6e64 6564  Qiskit unbounded
-000011d0: 2070 6172 616d 6574 6572 732e 0a4c 6574   parameters..Let
-000011e0: 2773 2063 6f6e 7369 6465 7220 7468 6520  's consider the 
-000011f0: 666f 6c6c 6f77 696e 6720 6578 616d 706c  following exampl
-00001200: 6520 7374 6172 7469 6e67 2066 726f 6d20  e starting from 
-00001210: 6120 605a 5a46 6561 7475 7265 4d61 7060  a `ZZFeatureMap`
-00001220: 2063 6972 6375 6974 2c20 636f 6d6d 6f6e   circuit, common
-00001230: 6c79 2075 7365 6420 6173 2061 2064 6174  ly used as a dat
-00001240: 6120 656d 6265 6464 696e 6720 616e 7361  a embedding ansa
-00001250: 747a 2069 6e20 514d 4c20 6170 706c 6963  tz in QML applic
-00001260: 6174 696f 6e73 3a0a 6060 6070 7974 686f  ations:.```pytho
-00001270: 6e0a 6672 6f6d 2071 6973 6b69 742e 6369  n.from qiskit.ci
-00001280: 7263 7569 742e 6c69 6272 6172 7920 696d  rcuit.library im
-00001290: 706f 7274 205a 5a46 6561 7475 7265 4d61  port ZZFeatureMa
-000012a0: 700a 0a70 7163 203d 205a 5a46 6561 7475  p..pqc = ZZFeatu
-000012b0: 7265 4d61 7028 6665 6174 7572 655f 6469  reMap(feature_di
-000012c0: 6d65 6e73 696f 6e3d 332c 2072 6570 733d  mension=3, reps=
-000012d0: 3129 0a70 7163 2e64 7261 7728 276d 706c  1).pqc.draw('mpl
-000012e0: 2729 0a60 6060 0a21 5b5d 282f 696d 672f  ').```.![](/img/
-000012f0: 7a7a 6665 6174 7572 656d 6170 5f63 6972  zzfeaturemap_cir
-00001300: 6375 6974 2e70 6e67 290a 0a54 6f20 6765  cuit.png)..To ge
-00001310: 7420 7468 6520 5079 7468 6f6e 206c 616d  t the Python lam
-00001320: 6264 6120 6675 6e63 7469 6f6e 2072 6570  bda function rep
-00001330: 7265 7365 6e74 696e 672c 2066 6f72 2069  resenting, for i
-00001340: 6e73 7461 6e63 652c 2074 6865 2066 696e  nstance, the fin
-00001350: 616c 2070 6172 616d 6574 6572 697a 6564  al parameterized
-00001360: 2073 7461 7465 7665 6374 6f72 2c20 7765   statevector, we
-00001370: 206a 7573 7420 6861 7665 2074 6f20 6372   just have to cr
-00001380: 6561 7465 2074 6865 2073 796d 626f 6c69  eate the symboli
-00001390: 6320 6053 7461 7465 7665 6374 6f72 6020  c `Statevector` 
-000013a0: 696e 7374 616e 6365 2061 6e64 2063 616c  instance and cal
-000013b0: 6c20 7468 6520 6074 6f5f 6c61 6d62 6461  l the `to_lambda
-000013c0: 2829 6020 6d65 7468 6f64 3a0a 6060 6070  ()` method:.```p
-000013d0: 7974 686f 6e0a 6672 6f6d 2071 6973 6b69  ython.from qiski
-000013e0: 745f 7379 6d62 2e71 7561 6e74 756d 5f69  t_symb.quantum_i
-000013f0: 6e66 6f20 696d 706f 7274 2053 7461 7465  nfo import State
-00001400: 7665 6374 6f72 0a0a 7376 203d 2053 7461  vector..sv = Sta
-00001410: 7465 7665 6374 6f72 2870 7163 290a 7376  tevector(pqc).sv
-00001420: 5f66 756e 6320 3d20 7376 2e74 6f5f 6c61  _func = sv.to_la
-00001430: 6d62 6461 2829 0a60 6060 0a0a 5765 2063  mbda().```..We c
-00001440: 616e 206e 6f77 2063 616c 6c20 7468 6520  an now call the 
-00001450: 6765 6e65 7261 7465 6420 6c61 6d62 6461  generated lambda
-00001460: 2066 756e 6374 696f 6e20 7061 7373 696e   function passin
-00001470: 6720 7468 6520 6163 7475 616c 2076 616c  g the actual val
-00001480: 7565 7320 7765 2077 616e 7420 746f 2061  ues we want to a
-00001490: 7373 6967 6e20 746f 2065 6163 6820 6672  ssign to each fr
-000014a0: 6565 2070 6172 616d 6574 6572 2028 696e  ee parameter (in
-000014b0: 2061 6c70 6861 6265 7469 6361 6c20 6f72   alphabetical or
-000014c0: 6465 722c 2073 616d 6520 636f 6e76 656e  der, same conven
-000014d0: 7469 6f6e 2075 7365 6420 696e 2060 7169  tion used in `qi
-000014e0: 736b 6974 2d74 6572 7261 6029 2e20 5468  skit-terra`). Th
-000014f0: 6520 7265 7475 726e 6564 206f 626a 6563  e returned objec
-00001500: 7420 7769 6c6c 2062 6520 6120 2a6e 756d  t will be a *num
-00001510: 7079 2a20 3244 2d61 7272 6179 2028 7769  py* 2D-array (wi
-00001520: 7468 2060 7368 6170 653d 2838 2c31 2960  th `shape=(8,1)`
-00001530: 2069 6e20 7468 6973 2063 6173 6529 2072   in this case) r
-00001540: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
-00001550: 6669 6e61 6c20 6f75 7470 7574 2073 7461  final output sta
-00001560: 7465 7665 6374 6f72 2e0a 6060 6070 7974  tevector..```pyt
-00001570: 686f 6e0a 7661 6c75 6573 203d 205b 312e  hon.values = [1.
-00001580: 3234 2c20 322e 3237 2c20 302e 3239 5d0a  24, 2.27, 0.29].
-00001590: 7374 6174 6576 6563 203d 2073 765f 6675  statevec = sv_fu
-000015a0: 6e63 282a 7661 6c75 6573 290a 6060 600a  nc(*values).```.
-000015b0: 0a2a 2a5f 5245 4d41 524b 5f2a 2a20 5c0a  .**_REMARK_** \.
-000015c0: 2a57 6865 6e20 7468 6520 5051 4320 6861  *When the PQC ha
-000015d0: 7320 746f 2062 6520 6576 616c 7561 7465  s to be evaluate
-000015e0: 6420 6f6e 2061 206c 6172 6765 206e 756d  d on a large num
-000015f0: 6265 7220 6f66 2064 6966 6665 7265 6e74  ber of different
-00001600: 2073 6574 7320 6f66 2070 6172 616d 6574   sets of paramet
-00001610: 6572 7320 7661 6c75 6573 2028 7479 7069  ers values (typi
-00001620: 6361 6c20 6361 7365 2069 6e20 514d 4c29  cal case in QML)
-00001630: 2c20 7468 6973 2060 7169 736b 6974 2d73  , this `qiskit-s
-00001640: 796d 6260 2066 6561 7475 7265 2063 616e  ymb` feature can
-00001650: 2068 656c 7020 746f 2073 6967 6e69 6669   help to signifi
-00001660: 6361 6e74 6c79 2069 6d70 726f 7665 2074  cantly improve t
-00001670: 6865 2028 6675 6c6c 2d73 7461 7465 7665  he (full-stateve
-00001680: 6374 6f72 2920 7369 6d75 6c61 7469 6f6e  ctor) simulation
-00001690: 2070 6572 666f 726d 6163 652e 2049 6e64   performace. Ind
-000016a0: 6565 642c 2074 6865 2073 796d 626f 6c69  eed, the symboli
-000016b0: 6320 6576 616c 7574 6174 696f 6e20 6f66  c evalutation of
-000016c0: 2074 6865 2063 6972 6375 6974 2061 6e64   the circuit and
-000016d0: 2074 6865 206c 616d 6264 6120 6765 6e65   the lambda gene
-000016e0: 7261 7469 6f6e 2074 616b 6520 706c 6163  ration take plac
-000016f0: 6520 6f6e 6c79 206f 6e63 653b 2074 6865  e only once; the
-00001700: 6e2c 2074 6865 2073 696d 756c 6174 696f  n, the simulatio
-00001710: 6e20 6f6e 6c79 2063 6f6e 7369 7374 7320  n only consists 
-00001720: 696e 2065 7865 6375 7469 6e67 206d 756c  in executing mul
-00001730: 7469 706c 6520 7469 6d65 7320 7468 6520  tiple times the 
-00001740: 7265 7475 726e 6564 2066 756e 6374 696f  returned functio
-00001750: 6e20 7061 7373 696e 6720 6120 6469 6666  n passing a diff
-00001760: 6572 656e 7420 7365 7420 6f66 2070 6172  erent set of par
-00001770: 616d 6574 6572 7320 7661 6c75 6573 2066  ameters values f
-00001780: 6f72 2065 6163 6820 6974 6572 6174 696f  or each iteratio
-00001790: 6e2e 2046 6f72 2072 656c 6174 6976 656c  n. For relativel
-000017a0: 7920 7368 616c 6c6f 7720 5051 4373 2077  y shallow PQCs w
-000017b0: 6974 6820 6120 6c69 6d69 6c74 6564 206e  ith a limilted n
-000017c0: 756d 6265 7220 6f66 2071 7562 6974 7320  umber of qubits 
-000017d0: 2865 2e67 2e20 5175 616e 7475 6d20 4b65  (e.g. Quantum Ke
-000017e0: 726e 656c 7320 6576 616c 7561 7469 6f6e  rnels evaluation
-000017f0: 292c 2074 6869 7320 6361 6e20 7265 6475  ), this can redu
-00001800: 6365 2074 6865 2065 7865 6375 7469 6f6e  ce the execution
-00001810: 2074 696d 6520 7570 2074 6f20 7477 6f20   time up to two 
-00001820: 6f72 6465 7220 6f66 206d 6167 6e69 7475  order of magnitu
-00001830: 6465 7320 2864 6570 656e 6469 6e67 206f  des (depending o
-00001840: 6e20 7468 6520 6e75 6d62 6572 206f 6620  n the number of 
-00001850: 6974 6572 6174 696f 6e73 2920 636f 6d70  iterations) comp
-00001860: 6172 6564 2074 6f20 7468 6520 7374 616e  ared to the stan
-00001870: 6461 7264 2051 6973 6b69 7420 7369 6d75  dard Qiskit simu
-00001880: 6c61 7469 6f6e 2062 6173 6564 206f 6e20  lation based on 
-00001890: 7468 6520 5b41 6572 2053 696d 756c 6174  the [Aer Simulat
-000018a0: 6f72 735d 2868 7474 7073 3a2f 2f71 6973  ors](https://qis
-000018b0: 6b69 742e 6f72 672f 646f 6375 6d65 6e74  kit.org/document
-000018c0: 6174 696f 6e2f 7475 746f 7269 616c 732f  ation/tutorials/
-000018d0: 7369 6d75 6c61 746f 7273 2f31 5f61 6572  simulators/1_aer
-000018e0: 5f70 726f 7669 6465 722e 6874 6d6c 2920  _provider.html) 
-000018f0: 6f72 2074 6865 205b 5361 6d70 6c65 725d  or the [Sampler]
-00001900: 2868 7474 7073 3a2f 2f71 6973 6b69 742e  (https://qiskit.
-00001910: 6f72 672f 646f 6375 6d65 6e74 6174 696f  org/documentatio
-00001920: 6e2f 7374 7562 732f 7169 736b 6974 2e70  n/stubs/qiskit.p
-00001930: 7269 6d69 7469 7665 732e 5361 6d70 6c65  rimitives.Sample
-00001940: 722e 6874 6d6c 2920 7072 696d 6974 6976  r.html) primitiv
-00001950: 652e 2a0a 0a0a 2320 436f 6e74 7269 6275  e.*...# Contribu
-00001960: 746f 7273 0a0a 3c74 6162 6c65 3e0a 2020  tors..<table>.  
-00001970: 3c74 723e 0a20 2020 203c 7464 2061 6c69  <tr>.    <td ali
-00001980: 676e 3d22 6365 6e74 6572 223e 3c61 2068  gn="center"><a h
-00001990: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-000019a0: 6875 622e 636f 6d2f 5369 6d6f 6e65 4761  hub.com/SimoneGa
-000019b0: 7370 6572 696e 6922 3e3c 696d 6720 7372  sperini"><img sr
-000019c0: 633d 2268 7474 7073 3a2f 2f61 7661 7461  c="https://avata
-000019d0: 7273 322e 6769 7468 7562 7573 6572 636f  rs2.githubuserco
-000019e0: 6e74 656e 742e 636f 6d2f 752f 3731 3038  ntent.com/u/7108
-000019f0: 3637 3538 3f73 3d34 3030 2676 3d34 2220  6758?s=400&v=4" 
-00001a00: 7769 6474 683d 2231 3230 7078 3b22 2f3e  width="120px;"/>
-00001a10: 3c62 722f 3e3c 623e 5369 6d6f 6e65 2047  <br/><b>Simone G
-00001a20: 6173 7065 7269 6e69 3c2f 623e 3c2f 613e  asperini</b></a>
-00001a30: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 3c2f  </td>.  </tr>.</
-00001a40: 7461 626c 653e 0a                        table>.
+00000200: 2e73 7667 223e 0a20 2020 203c 6120 6872  .svg">.    <a hr
+00000210: 6566 3d22 6874 7470 733a 2f2f 7169 736b  ef="https://qisk
+00000220: 6974 2e6f 7267 2f65 636f 7379 7374 656d  it.org/ecosystem
+00000230: 2f22 2061 6c74 3d22 4563 6f73 7973 7465  /" alt="Ecosyste
+00000240: 6d22 3e0a 2020 2020 2020 2020 3c69 6d67  m">.        <img
+00000250: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000260: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000270: 6765 2f51 6973 6b69 742d 4563 6f73 7973  ge/Qiskit-Ecosys
+00000280: 7465 6d2d 626c 7565 7669 6f6c 6574 2e73  tem-blueviolet.s
+00000290: 7667 2220 2f3e 3c2f 613e 0a3c 2f70 3e0a  vg" /></a>.</p>.
+000002a0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+000002b0: 7222 3e0a 2020 2020 3c69 6d67 2074 6974  r">.    <img tit
+000002c0: 6c65 3d22 6275 696c 6422 2073 7263 3d27  le="build" src='
+000002d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000002e0: 6f6d 2f53 696d 6f6e 6547 6173 7065 7269  om/SimoneGasperi
+000002f0: 6e69 2f71 6973 6b69 742d 7379 6d62 2f61  ni/qiskit-symb/a
+00000300: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000310: 2f70 7974 686f 6e2d 7061 636b 6167 652e  /python-package.
+00000320: 796d 6c2f 6261 6467 652e 7376 673f 6272  yml/badge.svg?br
+00000330: 616e 6368 3d6d 6173 7465 7227 3e0a 2020  anch=master'>.  
+00000340: 2020 3c69 6d67 2074 6974 6c65 3d22 636f    <img title="co
+00000350: 7665 7261 6765 2220 7372 633d 2768 7474  verage" src='htt
+00000360: 7073 3a2f 2f63 6f76 6572 616c 6c73 2e69  ps://coveralls.i
+00000370: 6f2f 7265 706f 732f 6769 7468 7562 2f53  o/repos/github/S
+00000380: 696d 6f6e 6547 6173 7065 7269 6e69 2f71  imoneGasperini/q
+00000390: 6973 6b69 742d 7379 6d62 2f62 6164 6765  iskit-symb/badge
+000003a0: 2e73 7667 3f62 7261 6e63 683d 6d61 7374  .svg?branch=mast
+000003b0: 6572 273e 0a3c 2f70 3e0a 0a2a 2a2a 0a54  er'>.</p>..***.T
+000003c0: 6869 7320 7061 636b 6167 6520 7761 7320  his package was 
+000003d0: 7072 6573 656e 7465 6420 6174 205b 5169  presented at [Qi
+000003e0: 736b 6974 2044 656d 6f44 6179 735d 2868  skit DemoDays](h
+000003f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000400: 6d2f 5169 736b 6974 2f66 6565 6462 6163  m/Qiskit/feedbac
+00000410: 6b2f 7769 6b69 2f51 6973 6b69 742d 4465  k/wiki/Qiskit-De
+00000420: 6d6f 4461 7973 2920 6f6e 204a 756e 6520  moDays) on June 
+00000430: 3135 7468 2032 3032 3320 245c 7269 6768  15th 2023 $\righ
+00000440: 7461 7272 6f77 2420 5b57 6562 6578 2072  tarrow$ [Webex r
+00000450: 6563 6f72 6469 6e67 5d28 6874 7470 733a  ecording](https:
+00000460: 2f2f 6962 6d2e 7765 6265 782e 636f 6d2f  //ibm.webex.com/
+00000470: 7265 636f 7264 696e 6773 6572 7669 6365  recordingservice
+00000480: 2f73 6974 6573 2f69 626d 2f72 6563 6f72  /sites/ibm/recor
+00000490: 6469 6e67 2f70 6c61 7962 6163 6b2f 6336  ding/playback/c6
+000004a0: 6439 3666 3235 6564 6261 3130 3362 6237  d96f25edba103bb7
+000004b0: 6436 3030 3530 3536 3831 3034 3464 2920  d600505681044d) 
+000004c0: 2870 6173 7377 6f72 643a 2060 4465 6d6f  (password: `Demo
+000004d0: 6461 7932 3032 3330 3631 3560 2920 2b20  day20230615`) + 
+000004e0: 5b4a 7570 7974 6572 206e 6f74 6562 6f6f  [Jupyter noteboo
+000004f0: 6b5d 2868 7474 7073 3a2f 2f67 6974 6875  k](https://githu
+00000500: 622e 636f 6d2f 5169 736b 6974 2f66 6565  b.com/Qiskit/fee
+00000510: 6462 6163 6b2f 626c 6f62 2f6d 6169 6e2f  dback/blob/main/
+00000520: 6465 6d6f 2d64 6179 2d6e 6f74 6562 6f6f  demo-day-noteboo
+00000530: 6b73 2f32 3032 332d 3036 2d31 352f 315f  ks/2023-06-15/1_
+00000540: 7169 736b 6974 5f73 796d 625f 6465 6d6f  qiskit_symb_demo
+00000550: 2e69 7079 6e62 290a 2a2a 2a0a 0a23 2054  .ipynb).***..# T
+00000560: 6162 6c65 206f 6620 636f 6e74 656e 7473  able of contents
+00000570: 0a2d 205b 496e 7472 6f64 7563 7469 6f6e  .- [Introduction
+00000580: 5d28 2369 6e74 726f 6475 6374 696f 6e29  ](#introduction)
+00000590: 0a2d 205b 496e 7374 616c 6c61 7469 6f6e  .- [Installation
+000005a0: 5d28 2369 6e73 7461 6c6c 6174 696f 6e29  ](#installation)
+000005b0: 0a20 2020 202d 205b 5573 6572 2d6d 6f64  .    - [User-mod
+000005c0: 655d 2823 7573 6572 2d6d 6f64 6529 0a20  e](#user-mode). 
+000005d0: 2020 202d 205b 4465 762d 6d6f 6465 5d28     - [Dev-mode](
+000005e0: 2364 6576 2d6d 6f64 6529 0a2d 205b 5573  #dev-mode).- [Us
+000005f0: 6167 6520 6578 616d 706c 6573 5d28 2375  age examples](#u
+00000600: 7361 6765 2d65 7861 6d70 6c65 7329 0a20  sage-examples). 
+00000610: 2020 202d 205b 5f53 796d 7069 6679 5f20     - [_Sympify_ 
+00000620: 6120 5169 736b 6974 2063 6972 6375 6974  a Qiskit circuit
+00000630: 5d28 2373 796d 7069 6679 2d61 2d71 6973  ](#sympify-a-qis
+00000640: 6b69 742d 6369 7263 7569 7429 0a20 2020  kit-circuit).   
+00000650: 202d 205b 5f4c 616d 6264 6966 795f 2061   - [_Lambdify_ a
+00000660: 2051 6973 6b69 7420 6369 7263 7569 745d   Qiskit circuit]
+00000670: 2823 6c61 6d62 6469 6679 2d61 2d71 6973  (#lambdify-a-qis
+00000680: 6b69 742d 6369 7263 7569 7429 0a2d 205b  kit-circuit).- [
+00000690: 436f 6e74 7269 6275 746f 7273 5d28 2363  Contributors](#c
+000006a0: 6f6e 7472 6962 7574 6f72 7329 0a0a 0a23  ontributors)...#
+000006b0: 2049 6e74 726f 6475 6374 696f 6e0a 5468   Introduction.Th
+000006c0: 6520 6071 6973 6b69 742d 7379 6d62 6020  e `qiskit-symb` 
+000006d0: 7061 636b 6167 6520 6973 206d 6561 6e74  package is meant
+000006e0: 2074 6f20 6265 2061 2050 7974 686f 6e20   to be a Python 
+000006f0: 746f 6f6c 2074 6f20 656e 6162 6c65 2074  tool to enable t
+00000700: 6865 2073 796d 626f 6c69 6320 6576 616c  he symbolic eval
+00000710: 7561 7469 6f6e 206f 6620 7061 7261 6d65  uation of parame
+00000720: 7472 6963 2071 7561 6e74 756d 2073 7461  tric quantum sta
+00000730: 7465 7320 616e 6420 6f70 6572 6174 6f72  tes and operator
+00000740: 7320 6465 6669 6e65 6420 696e 205b 5169  s defined in [Qi
+00000750: 736b 6974 5d28 6874 7470 733a 2f2f 6769  skit](https://gi
+00000760: 7468 7562 2e63 6f6d 2f51 6973 6b69 742f  thub.com/Qiskit/
+00000770: 7169 736b 6974 2d74 6572 7261 2920 6279  qiskit-terra) by
+00000780: 2070 6172 616d 6574 6572 697a 6564 2071   parameterized q
+00000790: 7561 6e74 756d 2063 6972 6375 6974 732e  uantum circuits.
+000007a0: 0a0a 4120 5061 7261 6d65 7465 7269 7a65  ..A Parameterize
+000007b0: 6420 5175 616e 7475 6d20 4369 7263 7569  d Quantum Circui
+000007c0: 7420 2850 5143 2920 6973 2061 2071 7561  t (PQC) is a qua
+000007d0: 6e74 756d 2063 6972 6375 6974 2077 6865  ntum circuit whe
+000007e0: 7265 2077 6520 6861 7665 2061 7420 6c65  re we have at le
+000007f0: 6173 7420 6f6e 6520 6672 6565 2070 6172  ast one free par
+00000800: 616d 6574 6572 2028 652e 672e 2061 2072  ameter (e.g. a r
+00000810: 6f74 6174 696f 6e20 616e 676c 6520 245c  otation angle $\
+00000820: 7468 6574 6124 292e 2050 5143 7320 6172  theta$). PQCs ar
+00000830: 6520 7061 7274 6963 756c 6172 6c79 2072  e particularly r
+00000840: 656c 6576 616e 7420 696e 2051 7561 6e74  elevant in Quant
+00000850: 756d 204d 6163 6869 6e65 204c 6561 726e  um Machine Learn
+00000860: 696e 6720 2851 4d4c 2920 6d6f 6465 6c73  ing (QML) models
+00000870: 2c20 7768 6572 6520 7468 6520 7661 6c75  , where the valu
+00000880: 6573 206f 6620 7468 6573 6520 7061 7261  es of these para
+00000890: 6d65 7465 7273 2063 616e 2062 6520 6c65  meters can be le
+000008a0: 6172 6e65 6420 6475 7269 6e67 2074 7261  arned during tra
+000008b0: 696e 696e 6720 746f 2072 6561 6368 2074  ining to reach t
+000008c0: 6865 2064 6573 6972 6564 206f 7574 7075  he desired outpu
+000008d0: 742e 0a0a 496e 2070 6172 7469 6375 6c61  t...In particula
+000008e0: 722c 2060 7169 736b 6974 2d73 796d 6260  r, `qiskit-symb`
+000008f0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+00000900: 6372 6561 7465 2061 2073 796d 626f 6c69  create a symboli
+00000910: 6320 7265 7072 6573 656e 7461 7469 6f6e  c representation
+00000920: 206f 6620 6120 7061 7261 6d65 7472 6963   of a parametric
+00000930: 2071 7561 6e74 756d 2073 7461 7465 7665   quantum stateve
+00000940: 6374 6f72 2c20 6465 6e73 6974 7920 6d61  ctor, density ma
+00000950: 7472 6978 2c20 6f72 2075 6e69 7461 7279  trix, or unitary
+00000960: 206f 7065 7261 746f 7220 6469 7265 6374   operator direct
+00000970: 6c79 2066 726f 6d20 7468 6520 5169 736b  ly from the Qisk
+00000980: 6974 2071 7561 6e74 756d 2063 6972 6375  it quantum circu
+00000990: 6974 2e20 5468 6973 2068 6173 2062 6565  it. This has bee
+000009a0: 6e20 6163 6869 6576 6564 2074 6872 6f75  n achieved throu
+000009b0: 6768 2074 6865 2072 652d 696d 706c 656d  gh the re-implem
+000009c0: 656e 7461 7469 6f6e 206f 6620 736f 6d65  entation of some
+000009d0: 2062 6173 6963 2063 6c61 7373 6573 2064   basic classes d
+000009e0: 6566 696e 6564 2069 6e20 7468 6520 5b60  efined in the [`
+000009f0: 7169 736b 6974 2f71 7561 6e74 756d 5f69  qiskit/quantum_i
+00000a00: 6e66 6f2f 605d 2868 7474 7073 3a2f 2f67  nfo/`](https://g
+00000a10: 6974 6875 622e 636f 6d2f 5169 736b 6974  ithub.com/Qiskit
+00000a20: 2f71 6973 6b69 742d 7465 7272 612f 7472  /qiskit-terra/tr
+00000a30: 6565 2f6d 6169 6e2f 7169 736b 6974 2f71  ee/main/qiskit/q
+00000a40: 7561 6e74 756d 5f69 6e66 6f29 206d 6f64  uantum_info) mod
+00000a50: 756c 6520 6279 2075 7369 6e67 205b 7379  ule by using [sy
+00000a60: 6d70 795d 2868 7474 7073 3a2f 2f67 6974  mpy](https://git
+00000a70: 6875 622e 636f 6d2f 7379 6d70 792f 7379  hub.com/sympy/sy
+00000a80: 6d70 7929 2061 7320 6120 6261 636b 656e  mpy) as a backen
+00000a90: 6420 666f 7220 7379 6d62 6f6c 6963 2065  d for symbolic e
+00000aa0: 7870 7265 7373 696f 6e73 206d 616e 6970  xpressions manip
+00000ab0: 756c 6174 696f 6e2e 0a0a 0a23 2049 6e73  ulation....# Ins
+00000ac0: 7461 6c6c 6174 696f 6e0a 0a23 2320 5573  tallation..## Us
+00000ad0: 6572 2d6d 6f64 650a 6060 600a 7069 7020  er-mode.```.pip 
+00000ae0: 696e 7374 616c 6c20 7169 736b 6974 2d73  install qiskit-s
+00000af0: 796d 620a 6060 600a 0a23 2320 4465 762d  ymb.```..## Dev-
+00000b00: 6d6f 6465 0a60 6060 0a67 6974 2063 6c6f  mode.```.git clo
+00000b10: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
+00000b20: 622e 636f 6d2f 5369 6d6f 6e65 4761 7370  b.com/SimoneGasp
+00000b30: 6572 696e 692f 7169 736b 6974 2d73 796d  erini/qiskit-sym
+00000b40: 622e 6769 740a 6364 2071 6973 6b69 742d  b.git.cd qiskit-
+00000b50: 7379 6d62 0a70 6970 2069 6e73 7461 6c6c  symb.pip install
+00000b60: 202d 6520 2e0a 6060 600a 0a0a 2320 5573   -e ..```...# Us
+00000b70: 6167 6520 6578 616d 706c 6573 0a0a 2323  age examples..##
+00000b80: 2320 5f53 796d 7069 6679 5f20 6120 5169  # _Sympify_ a Qi
+00000b90: 736b 6974 2063 6972 6375 6974 0a4c 6574  skit circuit.Let
+00000ba0: 2773 2067 6574 2073 7461 7274 6564 206f  's get started o
+00000bb0: 6e20 686f 7720 746f 2075 7365 2060 7169  n how to use `qi
+00000bc0: 736b 6974 2d73 796d 6260 2074 6f20 6765  skit-symb` to ge
+00000bd0: 7420 7468 6520 7379 6d62 6f6c 6963 2072  t the symbolic r
+00000be0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+00000bf0: 2061 2067 6976 656e 2051 6973 6b69 7420   a given Qiskit 
+00000c00: 6369 7263 7569 742e 2049 6e20 7061 7274  circuit. In part
+00000c10: 6963 756c 6172 2c20 696e 2074 6869 7320  icular, in this 
+00000c20: 6669 7273 7420 6261 7369 6320 6578 616d  first basic exam
+00000c30: 706c 652c 2077 6520 636f 6e73 6964 6572  ple, we consider
+00000c40: 2074 6865 2066 6f6c 6c6f 7769 6e67 2071   the following q
+00000c50: 7561 6e74 756d 2063 6972 6375 6974 3a0a  uantum circuit:.
+00000c60: 6060 6070 7974 686f 6e0a 6672 6f6d 2071  ```python.from q
+00000c70: 6973 6b69 7420 696d 706f 7274 2051 7561  iskit import Qua
+00000c80: 6e74 756d 4369 7263 7569 740a 6672 6f6d  ntumCircuit.from
+00000c90: 2071 6973 6b69 742e 6369 7263 7569 7420   qiskit.circuit 
+00000ca0: 696d 706f 7274 2050 6172 616d 6574 6572  import Parameter
+00000cb0: 2c20 5061 7261 6d65 7465 7256 6563 746f  , ParameterVecto
+00000cc0: 720a 0a79 203d 2050 6172 616d 6574 6572  r..y = Parameter
+00000cd0: 2827 7927 290a 7020 3d20 5061 7261 6d65  ('y').p = Parame
+00000ce0: 7465 7256 6563 746f 7228 2770 272c 206c  terVector('p', l
+00000cf0: 656e 6774 683d 3229 0a0a 7071 6320 3d20  ength=2)..pqc = 
+00000d00: 5175 616e 7475 6d43 6972 6375 6974 2832  QuantumCircuit(2
+00000d10: 290a 7071 632e 7279 2879 2c20 3029 0a70  ).pqc.ry(y, 0).p
+00000d20: 7163 2e63 7828 302c 2031 290a 7071 632e  qc.cx(0, 1).pqc.
+00000d30: 7528 302c 202a 702c 2031 290a 0a70 7163  u(0, *p, 1)..pqc
+00000d40: 2e64 7261 7728 276d 706c 2729 0a60 6060  .draw('mpl').```
+00000d50: 0a21 5b5d 282f 696d 672f 6578 616d 706c  .![](/img/exampl
+00000d60: 655f 6369 7263 7569 742e 706e 6729 0a0a  e_circuit.png)..
+00000d70: 546f 2067 6574 2074 6865 202a 7379 6d70  To get the *symp
+00000d80: 792a 2072 6570 7265 7365 6e74 6174 696f  y* representatio
+00000d90: 6e20 6f66 2074 6865 2075 6e69 7461 7279  n of the unitary
+00000da0: 206d 6174 7269 7820 636f 7272 6573 706f   matrix correspo
+00000db0: 6e64 696e 6720 746f 2074 6865 2070 6172  nding to the par
+00000dc0: 616d 6574 6572 697a 6564 2063 6972 6375  ameterized circu
+00000dd0: 6974 2c20 7765 206a 7573 7420 6861 7665  it, we just have
+00000de0: 2074 6f20 6372 6561 7465 2074 6865 2073   to create the s
+00000df0: 796d 626f 6c69 6320 604f 7065 7261 746f  ymbolic `Operato
+00000e00: 7260 2069 6e73 7461 6e63 6520 616e 6420  r` instance and 
+00000e10: 6361 6c6c 2074 6865 2060 746f 5f73 796d  call the `to_sym
+00000e20: 7079 2829 6020 6d65 7468 6f64 3a0a 6060  py()` method:.``
+00000e30: 6070 7974 686f 6e0a 6672 6f6d 2071 6973  `python.from qis
+00000e40: 6b69 745f 7379 6d62 2e71 7561 6e74 756d  kit_symb.quantum
+00000e50: 5f69 6e66 6f20 696d 706f 7274 204f 7065  _info import Ope
+00000e60: 7261 746f 720a 0a6f 7020 3d20 4f70 6572  rator..op = Oper
+00000e70: 6174 6f72 2870 7163 290a 6f70 2e74 6f5f  ator(pqc).op.to_
+00000e80: 7379 6d70 7928 290a 6060 600a 6060 606d  sympy().```.```m
+00000e90: 6174 680a 5c6c 6566 745b 5c62 6567 696e  ath.\left[\begin
+00000ea0: 7b6d 6174 7269 787d 5c63 6f73 7b5c 6c65  {matrix}\cos{\le
+00000eb0: 6674 285c 6672 6163 7b79 7d7b 327d 205c  ft(\frac{y}{2} \
+00000ec0: 7269 6768 7429 7d20 2620 2d20 5c73 696e  right)} & - \sin
+00000ed0: 7b5c 6c65 6674 285c 6672 6163 7b79 7d7b  {\left(\frac{y}{
+00000ee0: 327d 205c 7269 6768 7429 7d20 2620 3020  2} \right)} & 0 
+00000ef0: 2620 305c 5c30 2026 2030 2026 205c 7369  & 0\\0 & 0 & \si
+00000f00: 6e7b 5c6c 6566 7428 5c66 7261 637b 797d  n{\left(\frac{y}
+00000f10: 7b32 7d20 5c72 6967 6874 297d 2026 205c  {2} \right)} & \
+00000f20: 636f 737b 5c6c 6566 7428 5c66 7261 637b  cos{\left(\frac{
+00000f30: 797d 7b32 7d20 5c72 6967 6874 297d 5c5c  y}{2} \right)}\\
+00000f40: 3020 2620 3020 2620 655e 7b69 205c 6c65  0 & 0 & e^{i \le
+00000f50: 6674 2870 5b30 5d20 2b20 705b 315d 5c72  ft(p[0] + p[1]\r
+00000f60: 6967 6874 297d 205c 636f 737b 5c6c 6566  ight)} \cos{\lef
+00000f70: 7428 5c66 7261 637b 797d 7b32 7d20 5c72  t(\frac{y}{2} \r
+00000f80: 6967 6874 297d 2026 202d 2065 5e7b 6920  ight)} & - e^{i 
+00000f90: 5c6c 6566 7428 705b 305d 202b 2070 5b31  \left(p[0] + p[1
+00000fa0: 5d5c 7269 6768 7429 7d20 5c73 696e 7b5c  ]\right)} \sin{\
+00000fb0: 6c65 6674 285c 6672 6163 7b79 7d7b 327d  left(\frac{y}{2}
+00000fc0: 205c 7269 6768 7429 7d5c 5c65 5e7b 6920   \right)}\\e^{i 
+00000fd0: 5c6c 6566 7428 705b 305d 202b 2070 5b31  \left(p[0] + p[1
+00000fe0: 5d5c 7269 6768 7429 7d20 5c73 696e 7b5c  ]\right)} \sin{\
+00000ff0: 6c65 6674 285c 6672 6163 7b79 7d7b 327d  left(\frac{y}{2}
+00001000: 205c 7269 6768 7429 7d20 2620 655e 7b69   \right)} & e^{i
+00001010: 205c 6c65 6674 2870 5b30 5d20 2b20 705b   \left(p[0] + p[
+00001020: 315d 5c72 6967 6874 297d 205c 636f 737b  1]\right)} \cos{
+00001030: 5c6c 6566 7428 5c66 7261 637b 797d 7b32  \left(\frac{y}{2
+00001040: 7d20 5c72 6967 6874 297d 2026 2030 2026  } \right)} & 0 &
+00001050: 2030 5c65 6e64 7b6d 6174 7269 787d 5c72   0\end{matrix}\r
+00001060: 6967 6874 5d0a 6060 600a 0a49 6620 796f  ight].```..If yo
+00001070: 7520 7761 6e74 2074 6865 6e20 746f 2061  u want then to a
+00001080: 7373 6967 6e20 6120 7661 6c75 6520 746f  ssign a value to
+00001090: 2073 6f6d 6520 7370 6563 6966 6963 2070   some specific p
+000010a0: 6172 616d 6574 6572 2c20 796f 7520 6361  arameter, you ca
+000010b0: 6e20 7573 6520 7468 6520 6073 7562 7328  n use the `subs(
+000010c0: 3c64 6963 743e 2960 206d 6574 686f 6420  <dict>)` method 
+000010d0: 7061 7373 696e 6720 6120 6469 6374 696f  passing a dictio
+000010e0: 6e61 7279 2074 6861 7420 6d61 7073 2065  nary that maps e
+000010f0: 6163 6820 7061 7261 6d65 7465 7220 746f  ach parameter to
+00001100: 2074 6865 2064 6573 6972 6564 2063 6f72   the desired cor
+00001110: 7265 7370 6f6e 6469 6e67 2076 616c 7565  responding value
+00001120: 3a0a 6060 6070 7974 686f 6e0a 6e65 775f  :.```python.new_
+00001130: 6f70 203d 206f 702e 7375 6273 287b 703a  op = op.subs({p:
+00001140: 205b 2d31 2c20 325d 7d29 0a6e 6577 5f6f   [-1, 2]}).new_o
+00001150: 702e 746f 5f73 796d 7079 2829 0a60 6060  p.to_sympy().```
+00001160: 0a60 6060 6d61 7468 0a5c 6c65 6674 5b5c  .```math.\left[\
+00001170: 6265 6769 6e7b 6d61 7472 6978 7d5c 636f  begin{matrix}\co
+00001180: 737b 5c6c 6566 7428 5c66 7261 637b 797d  s{\left(\frac{y}
+00001190: 7b32 7d20 5c72 6967 6874 297d 2026 202d  {2} \right)} & -
+000011a0: 205c 7369 6e7b 5c6c 6566 7428 5c66 7261   \sin{\left(\fra
+000011b0: 637b 797d 7b32 7d20 5c72 6967 6874 297d  c{y}{2} \right)}
+000011c0: 2026 2030 2026 2030 5c5c 3020 2620 3020   & 0 & 0\\0 & 0 
+000011d0: 2620 5c73 696e 7b5c 6c65 6674 285c 6672  & \sin{\left(\fr
+000011e0: 6163 7b79 7d7b 327d 205c 7269 6768 7429  ac{y}{2} \right)
+000011f0: 7d20 2620 5c63 6f73 7b5c 6c65 6674 285c  } & \cos{\left(\
+00001200: 6672 6163 7b79 7d7b 327d 205c 7269 6768  frac{y}{2} \righ
+00001210: 7429 7d5c 5c30 2026 2030 2026 2065 5e7b  t)}\\0 & 0 & e^{
+00001220: 697d 205c 636f 737b 5c6c 6566 7428 5c66  i} \cos{\left(\f
+00001230: 7261 637b 797d 7b32 7d20 5c72 6967 6874  rac{y}{2} \right
+00001240: 297d 2026 202d 2065 5e7b 697d 205c 7369  )} & - e^{i} \si
+00001250: 6e7b 5c6c 6566 7428 5c66 7261 637b 797d  n{\left(\frac{y}
+00001260: 7b32 7d20 5c72 6967 6874 297d 5c5c 655e  {2} \right)}\\e^
+00001270: 7b69 7d20 5c73 696e 7b5c 6c65 6674 285c  {i} \sin{\left(\
+00001280: 6672 6163 7b79 7d7b 327d 205c 7269 6768  frac{y}{2} \righ
+00001290: 7429 7d20 2620 655e 7b69 7d20 5c63 6f73  t)} & e^{i} \cos
+000012a0: 7b5c 6c65 6674 285c 6672 6163 7b79 7d7b  {\left(\frac{y}{
+000012b0: 327d 205c 7269 6768 7429 7d20 2620 3020  2} \right)} & 0 
+000012c0: 2620 305c 656e 647b 6d61 7472 6978 7d5c  & 0\end{matrix}\
+000012d0: 7269 6768 745d 0a60 6060 0a0a 2323 2320  right].```..### 
+000012e0: 5f4c 616d 6264 6966 795f 2061 2051 6973  _Lambdify_ a Qis
+000012f0: 6b69 7420 6369 7263 7569 740a 4769 7665  kit circuit.Give
+00001300: 6e20 6120 5169 736b 6974 2063 6972 6375  n a Qiskit circu
+00001310: 6974 2c20 6071 6973 6b69 742d 7379 6d62  it, `qiskit-symb
+00001320: 6020 616c 736f 2061 6c6c 6f77 7320 746f  ` also allows to
+00001330: 2067 656e 6572 6174 6520 6120 5079 7468   generate a Pyth
+00001340: 6f6e 206c 616d 6264 6120 6675 6e63 7469  on lambda functi
+00001350: 6f6e 2077 6974 6820 6163 7475 616c 2061  on with actual a
+00001360: 7267 756d 656e 7473 206d 6174 6368 696e  rguments matchin
+00001370: 6720 7468 6520 5169 736b 6974 2075 6e62  g the Qiskit unb
+00001380: 6f75 6e64 2070 6172 616d 6574 6572 732e  ound parameters.
+00001390: 0a4c 6574 2773 2063 6f6e 7369 6465 7220  .Let's consider 
+000013a0: 7468 6520 666f 6c6c 6f77 696e 6720 6578  the following ex
+000013b0: 616d 706c 6520 7374 6172 7469 6e67 2066  ample starting f
+000013c0: 726f 6d20 6120 605a 5a46 6561 7475 7265  rom a `ZZFeature
+000013d0: 4d61 7060 2063 6972 6375 6974 2c20 636f  Map` circuit, co
+000013e0: 6d6d 6f6e 6c79 2075 7365 6420 6173 2061  mmonly used as a
+000013f0: 2064 6174 6120 656d 6265 6464 696e 6720   data embedding 
+00001400: 616e 7361 747a 2069 6e20 514d 4c20 6170  ansatz in QML ap
+00001410: 706c 6963 6174 696f 6e73 3a0a 6060 6070  plications:.```p
+00001420: 7974 686f 6e0a 6672 6f6d 2071 6973 6b69  ython.from qiski
+00001430: 742e 6369 7263 7569 742e 6c69 6272 6172  t.circuit.librar
+00001440: 7920 696d 706f 7274 205a 5a46 6561 7475  y import ZZFeatu
+00001450: 7265 4d61 700a 0a70 7163 203d 205a 5a46  reMap..pqc = ZZF
+00001460: 6561 7475 7265 4d61 7028 6665 6174 7572  eatureMap(featur
+00001470: 655f 6469 6d65 6e73 696f 6e3d 332c 2072  e_dimension=3, r
+00001480: 6570 733d 3129 0a70 7163 2e64 7261 7728  eps=1).pqc.draw(
+00001490: 276d 706c 2729 0a60 6060 0a21 5b5d 282f  'mpl').```.![](/
+000014a0: 696d 672f 7a7a 6665 6174 7572 656d 6170  img/zzfeaturemap
+000014b0: 5f63 6972 6375 6974 2e70 6e67 290a 0a54  _circuit.png)..T
+000014c0: 6f20 6765 7420 7468 6520 5079 7468 6f6e  o get the Python
+000014d0: 2066 756e 6374 696f 6e20 7265 7072 6573   function repres
+000014e0: 656e 7469 6e67 2074 6865 2066 696e 616c  enting the final
+000014f0: 2070 6172 616d 6574 6572 6963 2073 7461   parameteric sta
+00001500: 7465 7665 6374 6f72 2c20 7765 206a 7573  tevector, we jus
+00001510: 7420 6861 7665 2074 6f20 6372 6561 7465  t have to create
+00001520: 2074 6865 2073 796d 626f 6c69 6320 6053   the symbolic `S
+00001530: 7461 7465 7665 6374 6f72 6020 696e 7374  tatevector` inst
+00001540: 616e 6365 2061 6e64 2063 616c 6c20 7468  ance and call th
+00001550: 6520 6074 6f5f 6c61 6d62 6461 2829 6020  e `to_lambda()` 
+00001560: 6d65 7468 6f64 3a0a 6060 6070 7974 686f  method:.```pytho
+00001570: 6e0a 6672 6f6d 2071 6973 6b69 745f 7379  n.from qiskit_sy
+00001580: 6d62 2e71 7561 6e74 756d 5f69 6e66 6f20  mb.quantum_info 
+00001590: 696d 706f 7274 2053 7461 7465 7665 6374  import Statevect
+000015a0: 6f72 0a0a 7071 6320 3d20 7071 632e 6465  or..pqc = pqc.de
+000015b0: 636f 6d70 6f73 6528 290a 7374 6174 6576  compose().statev
+000015c0: 6563 203d 2053 7461 7465 7665 6374 6f72  ec = Statevector
+000015d0: 2870 7163 292e 746f 5f6c 616d 6264 6128  (pqc).to_lambda(
+000015e0: 290a 6060 600a 0a57 6520 6361 6e20 6e6f  ).```..We can no
+000015f0: 7720 6361 6c6c 2074 6865 206c 616d 6264  w call the lambd
+00001600: 612d 6765 6e65 7261 7465 6420 6675 6e63  a-generated func
+00001610: 7469 6f6e 2060 7374 6174 6576 6563 6020  tion `statevec` 
+00001620: 7061 7373 696e 6720 7468 6520 6078 6020  passing the `x` 
+00001630: 7661 6c75 6573 2077 6520 7761 6e74 2074  values we want t
+00001640: 6f20 6173 7369 676e 2074 6f20 6561 6368  o assign to each
+00001650: 2070 6172 616d 6574 6572 2e20 5468 6520   parameter. The 
+00001660: 7265 7475 726e 6564 206f 626a 6563 7420  returned object 
+00001670: 7769 6c6c 2062 6520 6120 2a6e 756d 7079  will be a *numpy
+00001680: 2a20 3244 2d61 7272 6179 2028 7769 7468  * 2D-array (with
+00001690: 2060 7368 6170 653d 2838 2c31 2960 2069   `shape=(8,1)` i
+000016a0: 6e20 7468 6973 2063 6173 6529 2072 6570  n this case) rep
+000016b0: 7265 7365 6e74 696e 6720 7468 6520 6669  resenting the fi
+000016c0: 6e61 6c20 6f75 7470 7574 2073 7461 7465  nal output state
+000016d0: 7665 6374 6f72 2060 7073 6960 2e0a 6060  vector `psi`..``
+000016e0: 6070 7974 686f 6e0a 7820 3d20 5b31 2e32  `python.x = [1.2
+000016f0: 342c 2032 2e32 372c 2030 2e32 395d 0a70  4, 2.27, 0.29].p
+00001700: 7369 203d 2073 7461 7465 7665 6328 2a78  si = statevec(*x
+00001710: 290a 6060 600a 0a54 6869 7320 6665 6174  ).```..This feat
+00001720: 7572 6520 6361 6e20 6265 2075 7365 6675  ure can be usefu
+00001730: 6c20 7768 656e 2c20 6769 7665 6e20 6120  l when, given a 
+00001740: 5169 736b 6974 2050 5143 2c20 7765 2077  Qiskit PQC, we w
+00001750: 616e 7420 746f 2072 756e 2069 7420 6d75  ant to run it mu
+00001760: 6c74 6970 6c65 2074 696d 6573 2077 6974  ltiple times wit
+00001770: 6820 6469 6666 6572 656e 7420 7061 7261  h different para
+00001780: 6d65 7465 7273 2076 616c 7565 732e 2049  meters values. I
+00001790: 6e64 6565 642c 2077 6520 6361 6e20 7065  ndeed, we can pe
+000017a0: 7266 6f72 6d20 6120 7369 6e67 6c65 2073  rform a single s
+000017b0: 796d 626f 6c69 6320 6576 616c 7574 6174  ymbolic evalutat
+000017c0: 696f 6e20 616e 6420 7468 656e 2063 616c  ion and then cal
+000017d0: 6c20 7468 6520 6c61 6d62 6461 2067 656e  l the lambda gen
+000017e0: 6572 6174 6564 2066 756e 6374 696f 6e20  erated function 
+000017f0: 6173 206d 616e 7920 7469 6d65 7320 6173  as many times as
+00001800: 206e 6565 6465 642c 2070 6173 7369 6e67   needed, passing
+00001810: 2064 6966 6665 7265 6e74 2076 616c 7565   different value
+00001820: 7320 6f66 2074 6865 2070 6172 616d 6574  s of the paramet
+00001830: 6572 7320 6174 2065 6163 6820 6974 6572  ers at each iter
+00001840: 6174 696f 6e2e 0a0a 2320 436f 6e74 7269  ation...# Contri
+00001850: 6275 746f 7273 0a0a 3c74 6162 6c65 3e0a  butors..<table>.
+00001860: 2020 3c74 723e 0a20 2020 203c 7464 2061    <tr>.    <td a
+00001870: 6c69 676e 3d22 6365 6e74 6572 223e 3c61  lign="center"><a
+00001880: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00001890: 6974 6875 622e 636f 6d2f 5369 6d6f 6e65  ithub.com/Simone
+000018a0: 4761 7370 6572 696e 6922 3e3c 696d 6720  Gasperini"><img 
+000018b0: 7372 633d 2268 7474 7073 3a2f 2f61 7661  src="https://ava
+000018c0: 7461 7273 322e 6769 7468 7562 7573 6572  tars2.githubuser
+000018d0: 636f 6e74 656e 742e 636f 6d2f 752f 3731  content.com/u/71
+000018e0: 3038 3637 3538 3f73 3d34 3030 2676 3d34  086758?s=400&v=4
+000018f0: 2220 7769 6474 683d 2231 3230 7078 3b22  " width="120px;"
+00001900: 2f3e 3c62 722f 3e3c 623e 5369 6d6f 6e65  /><br/><b>Simone
+00001910: 2047 6173 7065 7269 6e69 3c2f 623e 3c2f   Gasperini</b></
+00001920: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
+00001930: 3c2f 7461 626c 653e 0a                   </table>.
```

### Comparing `qiskit-symb-0.1.2/README.md` & `qiskit-symb-0.1.3/src/qiskit_symb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,402 +1,404 @@
-00000000: 215b 5d28 2f69 6d67 2f6c 6f67 6f2e 706e  ![](/img/logo.pn
-00000010: 6729 0a0a 3c70 2061 6c69 676e 3d22 6365  g)..<p align="ce
-00000020: 6e74 6572 223e 0a20 2020 203c 696d 6720  nter">.    <img 
-00000030: 7469 746c 653d 226c 6963 656e 7365 2220  title="license" 
-00000040: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000050: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000060: 652f 6c69 6365 6e73 652d 4170 6163 6865  e/license-Apache
-00000070: 5f32 2e30 2d62 6c75 652e 7376 6722 3e0a  _2.0-blue.svg">.
-00000080: 2020 2020 3c69 6d67 2074 6974 6c65 3d22      <img title="
-00000090: 7079 7468 6f6e 2220 7372 633d 2268 7474  python" src="htt
-000000a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000000b0: 2e69 6f2f 6261 6467 652f 7079 7468 6f6e  .io/badge/python
-000000c0: 2de2 89a5 332e 382d 626c 7565 2e73 7667  -...3.8-blue.svg
-000000d0: 223e 0a20 2020 203c 696d 6720 7469 746c  ">.    <img titl
-000000e0: 653d 2245 636f 7379 7374 656d 2220 7372  e="Ecosystem" sr
-000000f0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00000100: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000110: 5169 736b 6974 2d45 636f 7379 7374 656d  Qiskit-Ecosystem
-00000120: 2d62 6c75 6576 696f 6c65 742e 7376 6722  -blueviolet.svg"
-00000130: 3e0a 3c2f 703e 0a0a 3c70 2061 6c69 676e  >.</p>..<p align
-00000140: 3d22 6365 6e74 6572 223e 0a20 2020 203c  ="center">.    <
-00000150: 696d 6720 7469 746c 653d 2262 7569 6c64  img title="build
-00000160: 2220 7372 633d 2768 7474 7073 3a2f 2f67  " src='https://g
-00000170: 6974 6875 622e 636f 6d2f 5369 6d6f 6e65  ithub.com/Simone
-00000180: 4761 7370 6572 696e 692f 7169 736b 6974  Gasperini/qiskit
-00000190: 2d73 796d 622f 6163 7469 6f6e 732f 776f  -symb/actions/wo
-000001a0: 726b 666c 6f77 732f 7079 7468 6f6e 2d70  rkflows/python-p
-000001b0: 6163 6b61 6765 2e79 6d6c 2f62 6164 6765  ackage.yml/badge
-000001c0: 2e73 7667 3f62 7261 6e63 683d 6d61 7374  .svg?branch=mast
-000001d0: 6572 273e 0a20 2020 203c 696d 6720 7469  er'>.    <img ti
-000001e0: 746c 653d 2263 6f76 6572 6167 6522 2073  tle="coverage" s
-000001f0: 7263 3d27 6874 7470 733a 2f2f 636f 7665  rc='https://cove
-00000200: 7261 6c6c 732e 696f 2f72 6570 6f73 2f67  ralls.io/repos/g
-00000210: 6974 6875 622f 5369 6d6f 6e65 4761 7370  ithub/SimoneGasp
-00000220: 6572 696e 692f 7169 736b 6974 2d73 796d  erini/qiskit-sym
-00000230: 622f 6261 6467 652e 7376 673f 6272 616e  b/badge.svg?bran
-00000240: 6368 3d6d 6173 7465 7227 3e0a 3c2f 703e  ch=master'>.</p>
-00000250: 0a0a 2a2a 2a0a 0a23 2054 6162 6c65 206f  ..***..# Table o
-00000260: 6620 636f 6e74 656e 7473 0a2d 205b 496e  f contents.- [In
-00000270: 7472 6f64 7563 7469 6f6e 5d28 2369 6e74  troduction](#int
-00000280: 726f 6475 6374 696f 6e29 0a2d 205b 496e  roduction).- [In
-00000290: 7374 616c 6c61 7469 6f6e 5d28 2369 6e73  stallation](#ins
-000002a0: 7461 6c6c 6174 696f 6e29 0a20 2020 202d  tallation).    -
-000002b0: 205b 5573 6572 2d6d 6f64 655d 2823 7573   [User-mode](#us
-000002c0: 6572 2d6d 6f64 6529 0a20 2020 202d 205b  er-mode).    - [
-000002d0: 4465 762d 6d6f 6465 5d28 2364 6576 2d6d  Dev-mode](#dev-m
-000002e0: 6f64 6529 0a2d 205b 5573 6167 6520 6578  ode).- [Usage ex
-000002f0: 616d 706c 6573 5d28 2375 7361 6765 2d65  amples](#usage-e
-00000300: 7861 6d70 6c65 7329 0a20 2020 202d 205b  xamples).    - [
-00000310: 5f53 796d 7069 6679 5f20 6120 5169 736b  _Sympify_ a Qisk
-00000320: 6974 2063 6972 6375 6974 5d28 2373 796d  it circuit](#sym
-00000330: 7069 6679 2d61 2d71 6973 6b69 742d 6369  pify-a-qiskit-ci
-00000340: 7263 7569 7429 0a20 2020 202d 205b 5f4c  rcuit).    - [_L
-00000350: 616d 6264 6966 795f 2061 2051 6973 6b69  ambdify_ a Qiski
-00000360: 7420 6369 7263 7569 745d 2823 6c61 6d62  t circuit](#lamb
-00000370: 6469 6679 2d61 2d71 6973 6b69 742d 6369  dify-a-qiskit-ci
-00000380: 7263 7569 7429 0a2d 205b 436f 6e74 7269  rcuit).- [Contri
-00000390: 6275 746f 7273 5d28 2363 6f6e 7472 6962  butors](#contrib
-000003a0: 7574 6f72 7329 0a0a 0a23 2049 6e74 726f  utors)...# Intro
-000003b0: 6475 6374 696f 6e0a 5468 6520 6071 6973  duction.The `qis
-000003c0: 6b69 742d 7379 6d62 6020 7061 636b 6167  kit-symb` packag
-000003d0: 6520 6973 206d 6561 6e74 2074 6f20 6265  e is meant to be
-000003e0: 2061 2050 7974 686f 6e20 746f 6f6c 2074   a Python tool t
-000003f0: 6f20 656e 6162 6c65 2074 6865 2073 796d  o enable the sym
-00000400: 626f 6c69 6320 6576 616c 7561 7469 6f6e  bolic evaluation
-00000410: 206f 6620 7061 7261 6d65 7472 6963 2071   of parametric q
-00000420: 7561 6e74 756d 2073 7461 7465 7320 616e  uantum states an
-00000430: 6420 6f70 6572 6174 6f72 7320 6465 6669  d operators defi
-00000440: 6e65 6420 696e 205b 5169 736b 6974 5d28  ned in [Qiskit](
-00000450: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000460: 6f6d 2f51 6973 6b69 742f 7169 736b 6974  om/Qiskit/qiskit
-00000470: 2d74 6572 7261 2920 6279 2070 6172 616d  -terra) by param
-00000480: 6574 6572 697a 6564 2071 7561 6e74 756d  eterized quantum
-00000490: 2063 6972 6375 6974 732e 0a0a 4120 5061   circuits...A Pa
-000004a0: 7261 6d65 7465 7269 7a65 6420 5175 616e  rameterized Quan
-000004b0: 7475 6d20 4369 7263 7569 7420 2850 5143  tum Circuit (PQC
-000004c0: 2920 6973 2061 2071 7561 6e74 756d 2063  ) is a quantum c
-000004d0: 6972 6375 6974 2077 6865 7265 2077 6520  ircuit where we 
-000004e0: 6861 7665 2061 7420 6c65 6173 7420 6f6e  have at least on
-000004f0: 6520 6672 6565 2070 6172 616d 6574 6572  e free parameter
-00000500: 2028 652e 672e 2061 2072 6f74 6174 696f   (e.g. a rotatio
-00000510: 6e20 616e 676c 6520 245c 7468 6574 6124  n angle $\theta$
-00000520: 292e 2050 5143 7320 6172 6520 7061 7274  ). PQCs are part
-00000530: 6963 756c 6172 6c79 2072 656c 6576 616e  icularly relevan
-00000540: 7420 696e 2051 7561 6e74 756d 204d 6163  t in Quantum Mac
-00000550: 6869 6e65 204c 6561 726e 696e 6720 2851  hine Learning (Q
-00000560: 4d4c 2920 6d6f 6465 6c73 2c20 7768 6572  ML) models, wher
-00000570: 6520 7468 6520 7661 6c75 6573 206f 6620  e the values of 
-00000580: 7468 6573 6520 7061 7261 6d65 7465 7273  these parameters
-00000590: 2063 616e 2062 6520 6c65 6172 6e65 6420   can be learned 
-000005a0: 6475 7269 6e67 2074 7261 696e 696e 6720  during training 
-000005b0: 746f 2072 6561 6368 2074 6865 2064 6573  to reach the des
-000005c0: 6972 6564 206f 7574 7075 742e 0a0a 496e  ired output...In
-000005d0: 2070 6172 7469 6375 6c61 722c 2060 7169   particular, `qi
-000005e0: 736b 6974 2d73 796d 6260 2063 616e 2062  skit-symb` can b
-000005f0: 6520 7573 6564 2074 6f20 6372 6561 7465  e used to create
-00000600: 2061 2073 796d 626f 6c69 6320 7265 7072   a symbolic repr
-00000610: 6573 656e 7461 7469 6f6e 206f 6620 6120  esentation of a 
-00000620: 7061 7261 6d65 7472 6963 2071 7561 6e74  parametric quant
-00000630: 756d 2073 7461 7465 7665 6374 6f72 2c20  um statevector, 
-00000640: 6465 6e73 6974 7920 6d61 7472 6978 2c20  density matrix, 
-00000650: 6f72 2075 6e69 7461 7279 206f 7065 7261  or unitary opera
-00000660: 746f 7220 6469 7265 6374 6c79 2066 726f  tor directly fro
-00000670: 6d20 7468 6520 5169 736b 6974 2071 7561  m the Qiskit qua
-00000680: 6e74 756d 2063 6972 6375 6974 2e20 5468  ntum circuit. Th
-00000690: 6973 2068 6173 2062 6565 6e20 6163 6869  is has been achi
-000006a0: 6576 6564 2074 6872 6f75 6768 2074 6865  eved through the
-000006b0: 2072 652d 696d 706c 656d 656e 7461 7469   re-implementati
-000006c0: 6f6e 206f 6620 736f 6d65 2062 6173 6963  on of some basic
-000006d0: 2063 6c61 7373 6573 2064 6566 696e 6564   classes defined
-000006e0: 2069 6e20 7468 6520 5b60 7169 736b 6974   in the [`qiskit
-000006f0: 2f71 7561 6e74 756d 5f69 6e66 6f2f 605d  /quantum_info/`]
-00000700: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000710: 636f 6d2f 5169 736b 6974 2f71 6973 6b69  com/Qiskit/qiski
-00000720: 742d 7465 7272 612f 7472 6565 2f6d 6169  t-terra/tree/mai
-00000730: 6e2f 7169 736b 6974 2f71 7561 6e74 756d  n/qiskit/quantum
-00000740: 5f69 6e66 6f29 206d 6f64 756c 6520 6279  _info) module by
-00000750: 2075 7369 6e67 205b 7379 6d70 795d 2868   using [sympy](h
-00000760: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000770: 6d2f 7379 6d70 792f 7379 6d70 7929 2061  m/sympy/sympy) a
-00000780: 7320 6120 6261 636b 656e 6420 666f 7220  s a backend for 
-00000790: 7379 6d62 6f6c 6963 2065 7870 7265 7373  symbolic express
-000007a0: 696f 6e73 206d 616e 6970 756c 6174 696f  ions manipulatio
-000007b0: 6e2e 0a0a 0a23 2049 6e73 7461 6c6c 6174  n....# Installat
-000007c0: 696f 6e0a 0a23 2320 5573 6572 2d6d 6f64  ion..## User-mod
-000007d0: 650a 6060 600a 7069 7020 696e 7374 616c  e.```.pip instal
-000007e0: 6c20 7169 736b 6974 2d73 796d 620a 6060  l qiskit-symb.``
-000007f0: 600a 0a23 2320 4465 762d 6d6f 6465 0a60  `..## Dev-mode.`
-00000800: 6060 0a67 6974 2063 6c6f 6e65 2068 7474  ``.git clone htt
-00000810: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000820: 5369 6d6f 6e65 4761 7370 6572 696e 692f  SimoneGasperini/
-00000830: 7169 736b 6974 2d73 796d 622e 6769 740a  qiskit-symb.git.
-00000840: 6364 2071 6973 6b69 742d 7379 6d62 0a70  cd qiskit-symb.p
-00000850: 6970 2069 6e73 7461 6c6c 202d 6520 2e0a  ip install -e ..
-00000860: 6060 600a 0a0a 2320 5573 6167 6520 6578  ```...# Usage ex
-00000870: 616d 706c 6573 0a0a 2323 2320 5f53 796d  amples..### _Sym
-00000880: 7069 6679 5f20 6120 5169 736b 6974 2063  pify_ a Qiskit c
-00000890: 6972 6375 6974 0a4c 6574 2773 2067 6574  ircuit.Let's get
-000008a0: 2073 7461 7274 6564 206f 6e20 686f 7720   started on how 
-000008b0: 746f 2075 7365 2060 7169 736b 6974 2d73  to use `qiskit-s
-000008c0: 796d 6260 2074 6f20 6765 7420 7468 6520  ymb` to get the 
-000008d0: 7379 6d62 6f6c 6963 2072 6570 7265 7365  symbolic represe
-000008e0: 6e74 6174 696f 6e20 6f66 2061 2067 6976  ntation of a giv
-000008f0: 656e 2051 6973 6b69 7420 6369 7263 7569  en Qiskit circui
-00000900: 742e 2049 6e20 7061 7274 6963 756c 6172  t. In particular
-00000910: 2c20 696e 2074 6869 7320 6669 7273 7420  , in this first 
-00000920: 6261 7369 6320 6578 616d 706c 652c 2077  basic example, w
-00000930: 6520 636f 6e73 6964 6572 2074 6865 2066  e consider the f
-00000940: 6f6c 6c6f 7769 6e67 2071 7561 6e74 756d  ollowing quantum
-00000950: 2063 6972 6375 6974 3a0a 6060 6070 7974   circuit:.```pyt
-00000960: 686f 6e0a 6672 6f6d 2071 6973 6b69 7420  hon.from qiskit 
-00000970: 696d 706f 7274 2051 7561 6e74 756d 4369  import QuantumCi
-00000980: 7263 7569 740a 6672 6f6d 2071 6973 6b69  rcuit.from qiski
-00000990: 742e 6369 7263 7569 7420 696d 706f 7274  t.circuit import
-000009a0: 2050 6172 616d 6574 6572 2c20 5061 7261   Parameter, Para
-000009b0: 6d65 7465 7256 6563 746f 720a 0a79 203d  meterVector..y =
-000009c0: 2050 6172 616d 6574 6572 2827 7927 290a   Parameter('y').
-000009d0: 7020 3d20 5061 7261 6d65 7465 7256 6563  p = ParameterVec
-000009e0: 746f 7228 2770 272c 206c 656e 6774 683d  tor('p', length=
-000009f0: 3229 0a0a 7071 6320 3d20 5175 616e 7475  2)..pqc = Quantu
-00000a00: 6d43 6972 6375 6974 2832 290a 7071 632e  mCircuit(2).pqc.
-00000a10: 7279 2879 2c20 3029 0a70 7163 2e63 7828  ry(y, 0).pqc.cx(
-00000a20: 302c 2031 290a 7071 632e 7528 302c 202a  0, 1).pqc.u(0, *
-00000a30: 702c 2031 290a 0a70 7163 2e64 7261 7728  p, 1)..pqc.draw(
-00000a40: 276d 706c 2729 0a60 6060 0a21 5b5d 282f  'mpl').```.![](/
-00000a50: 696d 672f 6578 616d 706c 655f 6369 7263  img/example_circ
-00000a60: 7569 742e 706e 6729 0a0a 546f 2067 6574  uit.png)..To get
-00000a70: 2074 6865 202a 7379 6d70 792a 2072 6570   the *sympy* rep
-00000a80: 7265 7365 6e74 6174 696f 6e20 6f66 2074  resentation of t
-00000a90: 6865 2075 6e69 7461 7279 206d 6174 7269  he unitary matri
-00000aa0: 7820 636f 7272 6573 706f 6e64 696e 6720  x corresponding 
-00000ab0: 746f 2074 6865 2070 6172 616d 6574 6572  to the parameter
-00000ac0: 697a 6564 2063 6972 6375 6974 2c20 7765  ized circuit, we
-00000ad0: 206a 7573 7420 6861 7665 2074 6f20 6372   just have to cr
-00000ae0: 6561 7465 2074 6865 2073 796d 626f 6c69  eate the symboli
-00000af0: 6320 604f 7065 7261 746f 7260 2069 6e73  c `Operator` ins
-00000b00: 7461 6e63 6520 616e 6420 6361 6c6c 2074  tance and call t
-00000b10: 6865 2060 746f 5f73 796d 7079 2829 6020  he `to_sympy()` 
-00000b20: 6d65 7468 6f64 3a0a 6060 6070 7974 686f  method:.```pytho
-00000b30: 6e0a 6672 6f6d 2071 6973 6b69 745f 7379  n.from qiskit_sy
-00000b40: 6d62 2e71 7561 6e74 756d 5f69 6e66 6f20  mb.quantum_info 
-00000b50: 696d 706f 7274 204f 7065 7261 746f 720a  import Operator.
-00000b60: 0a6f 7020 3d20 4f70 6572 6174 6f72 2870  .op = Operator(p
-00000b70: 7163 290a 6f70 2e74 6f5f 7379 6d70 7928  qc).op.to_sympy(
-00000b80: 290a 6060 600a 6060 606d 6174 680a 5c6c  ).```.```math.\l
-00000b90: 6566 745b 5c62 6567 696e 7b6d 6174 7269  eft[\begin{matri
-00000ba0: 787d 5c63 6f73 7b5c 6c65 6674 285c 6672  x}\cos{\left(\fr
-00000bb0: 6163 7b79 7d7b 327d 205c 7269 6768 7429  ac{y}{2} \right)
-00000bc0: 7d20 2620 2d20 5c73 696e 7b5c 6c65 6674  } & - \sin{\left
-00000bd0: 285c 6672 6163 7b79 7d7b 327d 205c 7269  (\frac{y}{2} \ri
-00000be0: 6768 7429 7d20 2620 3020 2620 305c 5c30  ght)} & 0 & 0\\0
-00000bf0: 2026 2030 2026 205c 7369 6e7b 5c6c 6566   & 0 & \sin{\lef
-00000c00: 7428 5c66 7261 637b 797d 7b32 7d20 5c72  t(\frac{y}{2} \r
-00000c10: 6967 6874 297d 2026 205c 636f 737b 5c6c  ight)} & \cos{\l
-00000c20: 6566 7428 5c66 7261 637b 797d 7b32 7d20  eft(\frac{y}{2} 
-00000c30: 5c72 6967 6874 297d 5c5c 3020 2620 3020  \right)}\\0 & 0 
-00000c40: 2620 655e 7b69 205c 6c65 6674 2870 5b30  & e^{i \left(p[0
-00000c50: 5d20 2b20 705b 315d 5c72 6967 6874 297d  ] + p[1]\right)}
-00000c60: 205c 636f 737b 5c6c 6566 7428 5c66 7261   \cos{\left(\fra
-00000c70: 637b 797d 7b32 7d20 5c72 6967 6874 297d  c{y}{2} \right)}
-00000c80: 2026 202d 2065 5e7b 6920 5c6c 6566 7428   & - e^{i \left(
-00000c90: 705b 305d 202b 2070 5b31 5d5c 7269 6768  p[0] + p[1]\righ
-00000ca0: 7429 7d20 5c73 696e 7b5c 6c65 6674 285c  t)} \sin{\left(\
-00000cb0: 6672 6163 7b79 7d7b 327d 205c 7269 6768  frac{y}{2} \righ
-00000cc0: 7429 7d5c 5c65 5e7b 6920 5c6c 6566 7428  t)}\\e^{i \left(
-00000cd0: 705b 305d 202b 2070 5b31 5d5c 7269 6768  p[0] + p[1]\righ
-00000ce0: 7429 7d20 5c73 696e 7b5c 6c65 6674 285c  t)} \sin{\left(\
-00000cf0: 6672 6163 7b79 7d7b 327d 205c 7269 6768  frac{y}{2} \righ
-00000d00: 7429 7d20 2620 655e 7b69 205c 6c65 6674  t)} & e^{i \left
-00000d10: 2870 5b30 5d20 2b20 705b 315d 5c72 6967  (p[0] + p[1]\rig
-00000d20: 6874 297d 205c 636f 737b 5c6c 6566 7428  ht)} \cos{\left(
-00000d30: 5c66 7261 637b 797d 7b32 7d20 5c72 6967  \frac{y}{2} \rig
-00000d40: 6874 297d 2026 2030 2026 2030 5c65 6e64  ht)} & 0 & 0\end
-00000d50: 7b6d 6174 7269 787d 5c72 6967 6874 5d0a  {matrix}\right].
-00000d60: 6060 600a 0a49 6620 796f 7520 7761 6e74  ```..If you want
-00000d70: 2074 6865 6e20 746f 2061 7373 6967 6e20   then to assign 
-00000d80: 6120 7661 6c75 6520 746f 2073 6f6d 6520  a value to some 
-00000d90: 7370 6563 6966 6963 2070 6172 616d 6574  specific paramet
-00000da0: 6572 2c20 796f 7520 6361 6e20 7573 6520  er, you can use 
-00000db0: 7468 6520 6073 7562 7328 3c64 6963 743e  the `subs(<dict>
-00000dc0: 2960 206d 6574 686f 6420 7061 7373 696e  )` method passin
-00000dd0: 6720 6120 6469 6374 696f 6e61 7279 2074  g a dictionary t
-00000de0: 6861 7420 6d61 7073 2065 6163 6820 7061  hat maps each pa
-00000df0: 7261 6d65 7465 7220 746f 2074 6865 2064  rameter to the d
-00000e00: 6573 6972 6564 2063 6f72 7265 7370 6f6e  esired correspon
-00000e10: 6469 6e67 2076 616c 7565 3a0a 6060 6070  ding value:.```p
-00000e20: 7974 686f 6e0a 7061 7261 6d73 3276 616c  ython.params2val
-00000e30: 7565 203d 207b 703a 205b 2d31 2c20 325d  ue = {p: [-1, 2]
-00000e40: 7d0a 6e65 775f 6f70 203d 206f 702e 7375  }.new_op = op.su
-00000e50: 6273 2870 6172 616d 7332 7661 6c75 6529  bs(params2value)
-00000e60: 0a6e 6577 5f6f 702e 746f 5f73 796d 7079  .new_op.to_sympy
-00000e70: 2829 0a60 6060 0a60 6060 6d61 7468 0a5c  ().```.```math.\
-00000e80: 6c65 6674 5b5c 6265 6769 6e7b 6d61 7472  left[\begin{matr
-00000e90: 6978 7d5c 636f 737b 5c6c 6566 7428 5c66  ix}\cos{\left(\f
-00000ea0: 7261 637b 797d 7b32 7d20 5c72 6967 6874  rac{y}{2} \right
-00000eb0: 297d 2026 202d 205c 7369 6e7b 5c6c 6566  )} & - \sin{\lef
-00000ec0: 7428 5c66 7261 637b 797d 7b32 7d20 5c72  t(\frac{y}{2} \r
-00000ed0: 6967 6874 297d 2026 2030 2026 2030 5c5c  ight)} & 0 & 0\\
-00000ee0: 3020 2620 3020 2620 5c73 696e 7b5c 6c65  0 & 0 & \sin{\le
-00000ef0: 6674 285c 6672 6163 7b79 7d7b 327d 205c  ft(\frac{y}{2} \
-00000f00: 7269 6768 7429 7d20 2620 5c63 6f73 7b5c  right)} & \cos{\
-00000f10: 6c65 6674 285c 6672 6163 7b79 7d7b 327d  left(\frac{y}{2}
-00000f20: 205c 7269 6768 7429 7d5c 5c30 2026 2030   \right)}\\0 & 0
-00000f30: 2026 2065 5e7b 697d 205c 636f 737b 5c6c   & e^{i} \cos{\l
-00000f40: 6566 7428 5c66 7261 637b 797d 7b32 7d20  eft(\frac{y}{2} 
-00000f50: 5c72 6967 6874 297d 2026 202d 2065 5e7b  \right)} & - e^{
-00000f60: 697d 205c 7369 6e7b 5c6c 6566 7428 5c66  i} \sin{\left(\f
-00000f70: 7261 637b 797d 7b32 7d20 5c72 6967 6874  rac{y}{2} \right
-00000f80: 297d 5c5c 655e 7b69 7d20 5c73 696e 7b5c  )}\\e^{i} \sin{\
-00000f90: 6c65 6674 285c 6672 6163 7b79 7d7b 327d  left(\frac{y}{2}
-00000fa0: 205c 7269 6768 7429 7d20 2620 655e 7b69   \right)} & e^{i
-00000fb0: 7d20 5c63 6f73 7b5c 6c65 6674 285c 6672  } \cos{\left(\fr
-00000fc0: 6163 7b79 7d7b 327d 205c 7269 6768 7429  ac{y}{2} \right)
-00000fd0: 7d20 2620 3020 2620 305c 656e 647b 6d61  } & 0 & 0\end{ma
-00000fe0: 7472 6978 7d5c 7269 6768 745d 0a60 6060  trix}\right].```
-00000ff0: 0a0a 2323 2320 5f4c 616d 6264 6966 795f  ..### _Lambdify_
-00001000: 2061 2051 6973 6b69 7420 6369 7263 7569   a Qiskit circui
-00001010: 740a 4769 7665 6e20 6120 5169 736b 6974  t.Given a Qiskit
-00001020: 2063 6972 6375 6974 2c20 6071 6973 6b69   circuit, `qiski
-00001030: 742d 7379 6d62 6020 616c 736f 2061 6c6c  t-symb` also all
-00001040: 6f77 7320 746f 2067 656e 6572 6174 6520  ows to generate 
-00001050: 6120 5079 7468 6f6e 206c 616d 6264 6120  a Python lambda 
-00001060: 6675 6e63 7469 6f6e 2077 6974 6820 6163  function with ac
-00001070: 7475 616c 2061 7267 756d 656e 7473 206d  tual arguments m
-00001080: 6174 6368 696e 6720 7468 6520 5169 736b  atching the Qisk
-00001090: 6974 2075 6e62 6f75 6e64 6564 2070 6172  it unbounded par
-000010a0: 616d 6574 6572 732e 0a4c 6574 2773 2063  ameters..Let's c
-000010b0: 6f6e 7369 6465 7220 7468 6520 666f 6c6c  onsider the foll
-000010c0: 6f77 696e 6720 6578 616d 706c 6520 7374  owing example st
-000010d0: 6172 7469 6e67 2066 726f 6d20 6120 605a  arting from a `Z
-000010e0: 5a46 6561 7475 7265 4d61 7060 2063 6972  ZFeatureMap` cir
-000010f0: 6375 6974 2c20 636f 6d6d 6f6e 6c79 2075  cuit, commonly u
-00001100: 7365 6420 6173 2061 2064 6174 6120 656d  sed as a data em
-00001110: 6265 6464 696e 6720 616e 7361 747a 2069  bedding ansatz i
-00001120: 6e20 514d 4c20 6170 706c 6963 6174 696f  n QML applicatio
-00001130: 6e73 3a0a 6060 6070 7974 686f 6e0a 6672  ns:.```python.fr
-00001140: 6f6d 2071 6973 6b69 742e 6369 7263 7569  om qiskit.circui
-00001150: 742e 6c69 6272 6172 7920 696d 706f 7274  t.library import
-00001160: 205a 5a46 6561 7475 7265 4d61 700a 0a70   ZZFeatureMap..p
-00001170: 7163 203d 205a 5a46 6561 7475 7265 4d61  qc = ZZFeatureMa
-00001180: 7028 6665 6174 7572 655f 6469 6d65 6e73  p(feature_dimens
-00001190: 696f 6e3d 332c 2072 6570 733d 3129 0a70  ion=3, reps=1).p
-000011a0: 7163 2e64 7261 7728 276d 706c 2729 0a60  qc.draw('mpl').`
-000011b0: 6060 0a21 5b5d 282f 696d 672f 7a7a 6665  ``.![](/img/zzfe
-000011c0: 6174 7572 656d 6170 5f63 6972 6375 6974  aturemap_circuit
-000011d0: 2e70 6e67 290a 0a54 6f20 6765 7420 7468  .png)..To get th
-000011e0: 6520 5079 7468 6f6e 206c 616d 6264 6120  e Python lambda 
-000011f0: 6675 6e63 7469 6f6e 2072 6570 7265 7365  function represe
-00001200: 6e74 696e 672c 2066 6f72 2069 6e73 7461  nting, for insta
-00001210: 6e63 652c 2074 6865 2066 696e 616c 2070  nce, the final p
-00001220: 6172 616d 6574 6572 697a 6564 2073 7461  arameterized sta
-00001230: 7465 7665 6374 6f72 2c20 7765 206a 7573  tevector, we jus
-00001240: 7420 6861 7665 2074 6f20 6372 6561 7465  t have to create
-00001250: 2074 6865 2073 796d 626f 6c69 6320 6053   the symbolic `S
-00001260: 7461 7465 7665 6374 6f72 6020 696e 7374  tatevector` inst
-00001270: 616e 6365 2061 6e64 2063 616c 6c20 7468  ance and call th
-00001280: 6520 6074 6f5f 6c61 6d62 6461 2829 6020  e `to_lambda()` 
-00001290: 6d65 7468 6f64 3a0a 6060 6070 7974 686f  method:.```pytho
-000012a0: 6e0a 6672 6f6d 2071 6973 6b69 745f 7379  n.from qiskit_sy
-000012b0: 6d62 2e71 7561 6e74 756d 5f69 6e66 6f20  mb.quantum_info 
-000012c0: 696d 706f 7274 2053 7461 7465 7665 6374  import Statevect
-000012d0: 6f72 0a0a 7376 203d 2053 7461 7465 7665  or..sv = Stateve
-000012e0: 6374 6f72 2870 7163 290a 7376 5f66 756e  ctor(pqc).sv_fun
-000012f0: 6320 3d20 7376 2e74 6f5f 6c61 6d62 6461  c = sv.to_lambda
-00001300: 2829 0a60 6060 0a0a 5765 2063 616e 206e  ().```..We can n
-00001310: 6f77 2063 616c 6c20 7468 6520 6765 6e65  ow call the gene
-00001320: 7261 7465 6420 6c61 6d62 6461 2066 756e  rated lambda fun
-00001330: 6374 696f 6e20 7061 7373 696e 6720 7468  ction passing th
-00001340: 6520 6163 7475 616c 2076 616c 7565 7320  e actual values 
-00001350: 7765 2077 616e 7420 746f 2061 7373 6967  we want to assig
-00001360: 6e20 746f 2065 6163 6820 6672 6565 2070  n to each free p
-00001370: 6172 616d 6574 6572 2028 696e 2061 6c70  arameter (in alp
-00001380: 6861 6265 7469 6361 6c20 6f72 6465 722c  habetical order,
-00001390: 2073 616d 6520 636f 6e76 656e 7469 6f6e   same convention
-000013a0: 2075 7365 6420 696e 2060 7169 736b 6974   used in `qiskit
-000013b0: 2d74 6572 7261 6029 2e20 5468 6520 7265  -terra`). The re
-000013c0: 7475 726e 6564 206f 626a 6563 7420 7769  turned object wi
-000013d0: 6c6c 2062 6520 6120 2a6e 756d 7079 2a20  ll be a *numpy* 
-000013e0: 3244 2d61 7272 6179 2028 7769 7468 2060  2D-array (with `
-000013f0: 7368 6170 653d 2838 2c31 2960 2069 6e20  shape=(8,1)` in 
-00001400: 7468 6973 2063 6173 6529 2072 6570 7265  this case) repre
-00001410: 7365 6e74 696e 6720 7468 6520 6669 6e61  senting the fina
-00001420: 6c20 6f75 7470 7574 2073 7461 7465 7665  l output stateve
-00001430: 6374 6f72 2e0a 6060 6070 7974 686f 6e0a  ctor..```python.
-00001440: 7661 6c75 6573 203d 205b 312e 3234 2c20  values = [1.24, 
-00001450: 322e 3237 2c20 302e 3239 5d0a 7374 6174  2.27, 0.29].stat
-00001460: 6576 6563 203d 2073 765f 6675 6e63 282a  evec = sv_func(*
-00001470: 7661 6c75 6573 290a 6060 600a 0a2a 2a5f  values).```..**_
-00001480: 5245 4d41 524b 5f2a 2a20 5c0a 2a57 6865  REMARK_** \.*Whe
-00001490: 6e20 7468 6520 5051 4320 6861 7320 746f  n the PQC has to
-000014a0: 2062 6520 6576 616c 7561 7465 6420 6f6e   be evaluated on
-000014b0: 2061 206c 6172 6765 206e 756d 6265 7220   a large number 
-000014c0: 6f66 2064 6966 6665 7265 6e74 2073 6574  of different set
-000014d0: 7320 6f66 2070 6172 616d 6574 6572 7320  s of parameters 
-000014e0: 7661 6c75 6573 2028 7479 7069 6361 6c20  values (typical 
-000014f0: 6361 7365 2069 6e20 514d 4c29 2c20 7468  case in QML), th
-00001500: 6973 2060 7169 736b 6974 2d73 796d 6260  is `qiskit-symb`
-00001510: 2066 6561 7475 7265 2063 616e 2068 656c   feature can hel
-00001520: 7020 746f 2073 6967 6e69 6669 6361 6e74  p to significant
-00001530: 6c79 2069 6d70 726f 7665 2074 6865 2028  ly improve the (
-00001540: 6675 6c6c 2d73 7461 7465 7665 6374 6f72  full-statevector
-00001550: 2920 7369 6d75 6c61 7469 6f6e 2070 6572  ) simulation per
-00001560: 666f 726d 6163 652e 2049 6e64 6565 642c  formace. Indeed,
-00001570: 2074 6865 2073 796d 626f 6c69 6320 6576   the symbolic ev
-00001580: 616c 7574 6174 696f 6e20 6f66 2074 6865  alutation of the
-00001590: 2063 6972 6375 6974 2061 6e64 2074 6865   circuit and the
-000015a0: 206c 616d 6264 6120 6765 6e65 7261 7469   lambda generati
-000015b0: 6f6e 2074 616b 6520 706c 6163 6520 6f6e  on take place on
-000015c0: 6c79 206f 6e63 653b 2074 6865 6e2c 2074  ly once; then, t
-000015d0: 6865 2073 696d 756c 6174 696f 6e20 6f6e  he simulation on
-000015e0: 6c79 2063 6f6e 7369 7374 7320 696e 2065  ly consists in e
-000015f0: 7865 6375 7469 6e67 206d 756c 7469 706c  xecuting multipl
-00001600: 6520 7469 6d65 7320 7468 6520 7265 7475  e times the retu
-00001610: 726e 6564 2066 756e 6374 696f 6e20 7061  rned function pa
-00001620: 7373 696e 6720 6120 6469 6666 6572 656e  ssing a differen
-00001630: 7420 7365 7420 6f66 2070 6172 616d 6574  t set of paramet
-00001640: 6572 7320 7661 6c75 6573 2066 6f72 2065  ers values for e
-00001650: 6163 6820 6974 6572 6174 696f 6e2e 2046  ach iteration. F
-00001660: 6f72 2072 656c 6174 6976 656c 7920 7368  or relatively sh
-00001670: 616c 6c6f 7720 5051 4373 2077 6974 6820  allow PQCs with 
-00001680: 6120 6c69 6d69 6c74 6564 206e 756d 6265  a limilted numbe
-00001690: 7220 6f66 2071 7562 6974 7320 2865 2e67  r of qubits (e.g
-000016a0: 2e20 5175 616e 7475 6d20 4b65 726e 656c  . Quantum Kernel
-000016b0: 7320 6576 616c 7561 7469 6f6e 292c 2074  s evaluation), t
-000016c0: 6869 7320 6361 6e20 7265 6475 6365 2074  his can reduce t
-000016d0: 6865 2065 7865 6375 7469 6f6e 2074 696d  he execution tim
-000016e0: 6520 7570 2074 6f20 7477 6f20 6f72 6465  e up to two orde
-000016f0: 7220 6f66 206d 6167 6e69 7475 6465 7320  r of magnitudes 
-00001700: 2864 6570 656e 6469 6e67 206f 6e20 7468  (depending on th
-00001710: 6520 6e75 6d62 6572 206f 6620 6974 6572  e number of iter
-00001720: 6174 696f 6e73 2920 636f 6d70 6172 6564  ations) compared
-00001730: 2074 6f20 7468 6520 7374 616e 6461 7264   to the standard
-00001740: 2051 6973 6b69 7420 7369 6d75 6c61 7469   Qiskit simulati
-00001750: 6f6e 2062 6173 6564 206f 6e20 7468 6520  on based on the 
-00001760: 5b41 6572 2053 696d 756c 6174 6f72 735d  [Aer Simulators]
-00001770: 2868 7474 7073 3a2f 2f71 6973 6b69 742e  (https://qiskit.
-00001780: 6f72 672f 646f 6375 6d65 6e74 6174 696f  org/documentatio
-00001790: 6e2f 7475 746f 7269 616c 732f 7369 6d75  n/tutorials/simu
-000017a0: 6c61 746f 7273 2f31 5f61 6572 5f70 726f  lators/1_aer_pro
-000017b0: 7669 6465 722e 6874 6d6c 2920 6f72 2074  vider.html) or t
-000017c0: 6865 205b 5361 6d70 6c65 725d 2868 7474  he [Sampler](htt
-000017d0: 7073 3a2f 2f71 6973 6b69 742e 6f72 672f  ps://qiskit.org/
-000017e0: 646f 6375 6d65 6e74 6174 696f 6e2f 7374  documentation/st
-000017f0: 7562 732f 7169 736b 6974 2e70 7269 6d69  ubs/qiskit.primi
-00001800: 7469 7665 732e 5361 6d70 6c65 722e 6874  tives.Sampler.ht
-00001810: 6d6c 2920 7072 696d 6974 6976 652e 2a0a  ml) primitive.*.
-00001820: 0a0a 2320 436f 6e74 7269 6275 746f 7273  ..# Contributors
-00001830: 0a0a 3c74 6162 6c65 3e0a 2020 3c74 723e  ..<table>.  <tr>
-00001840: 0a20 2020 203c 7464 2061 6c69 676e 3d22  .    <td align="
-00001850: 6365 6e74 6572 223e 3c61 2068 7265 663d  center"><a href=
-00001860: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001870: 636f 6d2f 5369 6d6f 6e65 4761 7370 6572  com/SimoneGasper
-00001880: 696e 6922 3e3c 696d 6720 7372 633d 2268  ini"><img src="h
-00001890: 7474 7073 3a2f 2f61 7661 7461 7273 322e  ttps://avatars2.
-000018a0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-000018b0: 742e 636f 6d2f 752f 3731 3038 3637 3538  t.com/u/71086758
-000018c0: 3f73 3d34 3030 2676 3d34 2220 7769 6474  ?s=400&v=4" widt
-000018d0: 683d 2231 3230 7078 3b22 2f3e 3c62 722f  h="120px;"/><br/
-000018e0: 3e3c 623e 5369 6d6f 6e65 2047 6173 7065  ><b>Simone Gaspe
-000018f0: 7269 6e69 3c2f 623e 3c2f 613e 3c2f 7464  rini</b></a></td
-00001900: 3e0a 2020 3c2f 7472 3e0a 3c2f 7461 626c  >.  </tr>.</tabl
-00001910: 653e                                     e>
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7169 736b  : 2.1.Name: qisk
+00000020: 6974 2d73 796d 620a 5665 7273 696f 6e3a  it-symb.Version:
+00000030: 2030 2e31 2e33 0a48 6f6d 652d 7061 6765   0.1.3.Home-page
+00000040: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000050: 2e63 6f6d 2f53 696d 6f6e 6547 6173 7065  .com/SimoneGaspe
+00000060: 7269 6e69 2f71 6973 6b69 742d 7379 6d62  rini/qiskit-symb
+00000070: 0a41 7574 686f 723a 2053 696d 6f6e 6547  .Author: SimoneG
+00000080: 6173 7065 7269 6e69 0a41 7574 686f 722d  asperini.Author-
+00000090: 656d 6169 6c3a 2073 696d 6f6e 652e 6761  email: simone.ga
+000000a0: 7370 6572 696e 6934 4075 6e69 626f 2e69  sperini4@unibo.i
+000000b0: 740a 4c69 6365 6e73 653a 2041 7061 6368  t.License: Apach
+000000c0: 6520 322e 300a 5265 7175 6972 6573 2d50  e 2.0.Requires-P
+000000d0: 7974 686f 6e3a 203e 3d33 2e38 0a44 6573  ython: >=3.8.Des
+000000e0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+000000f0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000100: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
+00000110: 7472 613a 2074 6573 7469 6e67 0a4c 6963  tra: testing.Lic
+00000120: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
+00000130: 5345 0a0a 215b 5d28 2f69 6d67 2f6c 6f67  SE..![](/img/log
+00000140: 6f2e 706e 6729 0a0a 3c70 2061 6c69 676e  o.png)..<p align
+00000150: 3d22 6365 6e74 6572 223e 0a20 2020 203c  ="center">.    <
+00000160: 696d 6720 7469 746c 653d 226c 6963 656e  img title="licen
+00000170: 7365 2220 7372 633d 2268 7474 7073 3a2f  se" src="https:/
+00000180: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000190: 6261 6467 652f 6c69 6365 6e73 652d 4170  badge/license-Ap
+000001a0: 6163 6865 5f32 2e30 2d62 6c75 652e 7376  ache_2.0-blue.sv
+000001b0: 6722 3e0a 2020 2020 3c69 6d67 2074 6974  g">.    <img tit
+000001c0: 6c65 3d22 7079 7468 6f6e 2220 7372 633d  le="python" src=
+000001d0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+000001e0: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
+000001f0: 7468 6f6e 2de2 89a5 332e 382d 626c 7565  thon-...3.8-blue
+00000200: 2e73 7667 223e 0a20 2020 203c 6120 6872  .svg">.    <a hr
+00000210: 6566 3d22 6874 7470 733a 2f2f 7169 736b  ef="https://qisk
+00000220: 6974 2e6f 7267 2f65 636f 7379 7374 656d  it.org/ecosystem
+00000230: 2f22 2061 6c74 3d22 4563 6f73 7973 7465  /" alt="Ecosyste
+00000240: 6d22 3e0a 2020 2020 2020 2020 3c69 6d67  m">.        <img
+00000250: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000260: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000270: 6765 2f51 6973 6b69 742d 4563 6f73 7973  ge/Qiskit-Ecosys
+00000280: 7465 6d2d 626c 7565 7669 6f6c 6574 2e73  tem-blueviolet.s
+00000290: 7667 2220 2f3e 3c2f 613e 0a3c 2f70 3e0a  vg" /></a>.</p>.
+000002a0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+000002b0: 7222 3e0a 2020 2020 3c69 6d67 2074 6974  r">.    <img tit
+000002c0: 6c65 3d22 6275 696c 6422 2073 7263 3d27  le="build" src='
+000002d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000002e0: 6f6d 2f53 696d 6f6e 6547 6173 7065 7269  om/SimoneGasperi
+000002f0: 6e69 2f71 6973 6b69 742d 7379 6d62 2f61  ni/qiskit-symb/a
+00000300: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000310: 2f70 7974 686f 6e2d 7061 636b 6167 652e  /python-package.
+00000320: 796d 6c2f 6261 6467 652e 7376 673f 6272  yml/badge.svg?br
+00000330: 616e 6368 3d6d 6173 7465 7227 3e0a 2020  anch=master'>.  
+00000340: 2020 3c69 6d67 2074 6974 6c65 3d22 636f    <img title="co
+00000350: 7665 7261 6765 2220 7372 633d 2768 7474  verage" src='htt
+00000360: 7073 3a2f 2f63 6f76 6572 616c 6c73 2e69  ps://coveralls.i
+00000370: 6f2f 7265 706f 732f 6769 7468 7562 2f53  o/repos/github/S
+00000380: 696d 6f6e 6547 6173 7065 7269 6e69 2f71  imoneGasperini/q
+00000390: 6973 6b69 742d 7379 6d62 2f62 6164 6765  iskit-symb/badge
+000003a0: 2e73 7667 3f62 7261 6e63 683d 6d61 7374  .svg?branch=mast
+000003b0: 6572 273e 0a3c 2f70 3e0a 0a2a 2a2a 0a54  er'>.</p>..***.T
+000003c0: 6869 7320 7061 636b 6167 6520 7761 7320  his package was 
+000003d0: 7072 6573 656e 7465 6420 6174 205b 5169  presented at [Qi
+000003e0: 736b 6974 2044 656d 6f44 6179 735d 2868  skit DemoDays](h
+000003f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000400: 6d2f 5169 736b 6974 2f66 6565 6462 6163  m/Qiskit/feedbac
+00000410: 6b2f 7769 6b69 2f51 6973 6b69 742d 4465  k/wiki/Qiskit-De
+00000420: 6d6f 4461 7973 2920 6f6e 204a 756e 6520  moDays) on June 
+00000430: 3135 7468 2032 3032 3320 245c 7269 6768  15th 2023 $\righ
+00000440: 7461 7272 6f77 2420 5b57 6562 6578 2072  tarrow$ [Webex r
+00000450: 6563 6f72 6469 6e67 5d28 6874 7470 733a  ecording](https:
+00000460: 2f2f 6962 6d2e 7765 6265 782e 636f 6d2f  //ibm.webex.com/
+00000470: 7265 636f 7264 696e 6773 6572 7669 6365  recordingservice
+00000480: 2f73 6974 6573 2f69 626d 2f72 6563 6f72  /sites/ibm/recor
+00000490: 6469 6e67 2f70 6c61 7962 6163 6b2f 6336  ding/playback/c6
+000004a0: 6439 3666 3235 6564 6261 3130 3362 6237  d96f25edba103bb7
+000004b0: 6436 3030 3530 3536 3831 3034 3464 2920  d600505681044d) 
+000004c0: 2870 6173 7377 6f72 643a 2060 4465 6d6f  (password: `Demo
+000004d0: 6461 7932 3032 3330 3631 3560 2920 2b20  day20230615`) + 
+000004e0: 5b4a 7570 7974 6572 206e 6f74 6562 6f6f  [Jupyter noteboo
+000004f0: 6b5d 2868 7474 7073 3a2f 2f67 6974 6875  k](https://githu
+00000500: 622e 636f 6d2f 5169 736b 6974 2f66 6565  b.com/Qiskit/fee
+00000510: 6462 6163 6b2f 626c 6f62 2f6d 6169 6e2f  dback/blob/main/
+00000520: 6465 6d6f 2d64 6179 2d6e 6f74 6562 6f6f  demo-day-noteboo
+00000530: 6b73 2f32 3032 332d 3036 2d31 352f 315f  ks/2023-06-15/1_
+00000540: 7169 736b 6974 5f73 796d 625f 6465 6d6f  qiskit_symb_demo
+00000550: 2e69 7079 6e62 290a 2a2a 2a0a 0a23 2054  .ipynb).***..# T
+00000560: 6162 6c65 206f 6620 636f 6e74 656e 7473  able of contents
+00000570: 0a2d 205b 496e 7472 6f64 7563 7469 6f6e  .- [Introduction
+00000580: 5d28 2369 6e74 726f 6475 6374 696f 6e29  ](#introduction)
+00000590: 0a2d 205b 496e 7374 616c 6c61 7469 6f6e  .- [Installation
+000005a0: 5d28 2369 6e73 7461 6c6c 6174 696f 6e29  ](#installation)
+000005b0: 0a20 2020 202d 205b 5573 6572 2d6d 6f64  .    - [User-mod
+000005c0: 655d 2823 7573 6572 2d6d 6f64 6529 0a20  e](#user-mode). 
+000005d0: 2020 202d 205b 4465 762d 6d6f 6465 5d28     - [Dev-mode](
+000005e0: 2364 6576 2d6d 6f64 6529 0a2d 205b 5573  #dev-mode).- [Us
+000005f0: 6167 6520 6578 616d 706c 6573 5d28 2375  age examples](#u
+00000600: 7361 6765 2d65 7861 6d70 6c65 7329 0a20  sage-examples). 
+00000610: 2020 202d 205b 5f53 796d 7069 6679 5f20     - [_Sympify_ 
+00000620: 6120 5169 736b 6974 2063 6972 6375 6974  a Qiskit circuit
+00000630: 5d28 2373 796d 7069 6679 2d61 2d71 6973  ](#sympify-a-qis
+00000640: 6b69 742d 6369 7263 7569 7429 0a20 2020  kit-circuit).   
+00000650: 202d 205b 5f4c 616d 6264 6966 795f 2061   - [_Lambdify_ a
+00000660: 2051 6973 6b69 7420 6369 7263 7569 745d   Qiskit circuit]
+00000670: 2823 6c61 6d62 6469 6679 2d61 2d71 6973  (#lambdify-a-qis
+00000680: 6b69 742d 6369 7263 7569 7429 0a2d 205b  kit-circuit).- [
+00000690: 436f 6e74 7269 6275 746f 7273 5d28 2363  Contributors](#c
+000006a0: 6f6e 7472 6962 7574 6f72 7329 0a0a 0a23  ontributors)...#
+000006b0: 2049 6e74 726f 6475 6374 696f 6e0a 5468   Introduction.Th
+000006c0: 6520 6071 6973 6b69 742d 7379 6d62 6020  e `qiskit-symb` 
+000006d0: 7061 636b 6167 6520 6973 206d 6561 6e74  package is meant
+000006e0: 2074 6f20 6265 2061 2050 7974 686f 6e20   to be a Python 
+000006f0: 746f 6f6c 2074 6f20 656e 6162 6c65 2074  tool to enable t
+00000700: 6865 2073 796d 626f 6c69 6320 6576 616c  he symbolic eval
+00000710: 7561 7469 6f6e 206f 6620 7061 7261 6d65  uation of parame
+00000720: 7472 6963 2071 7561 6e74 756d 2073 7461  tric quantum sta
+00000730: 7465 7320 616e 6420 6f70 6572 6174 6f72  tes and operator
+00000740: 7320 6465 6669 6e65 6420 696e 205b 5169  s defined in [Qi
+00000750: 736b 6974 5d28 6874 7470 733a 2f2f 6769  skit](https://gi
+00000760: 7468 7562 2e63 6f6d 2f51 6973 6b69 742f  thub.com/Qiskit/
+00000770: 7169 736b 6974 2d74 6572 7261 2920 6279  qiskit-terra) by
+00000780: 2070 6172 616d 6574 6572 697a 6564 2071   parameterized q
+00000790: 7561 6e74 756d 2063 6972 6375 6974 732e  uantum circuits.
+000007a0: 0a0a 4120 5061 7261 6d65 7465 7269 7a65  ..A Parameterize
+000007b0: 6420 5175 616e 7475 6d20 4369 7263 7569  d Quantum Circui
+000007c0: 7420 2850 5143 2920 6973 2061 2071 7561  t (PQC) is a qua
+000007d0: 6e74 756d 2063 6972 6375 6974 2077 6865  ntum circuit whe
+000007e0: 7265 2077 6520 6861 7665 2061 7420 6c65  re we have at le
+000007f0: 6173 7420 6f6e 6520 6672 6565 2070 6172  ast one free par
+00000800: 616d 6574 6572 2028 652e 672e 2061 2072  ameter (e.g. a r
+00000810: 6f74 6174 696f 6e20 616e 676c 6520 245c  otation angle $\
+00000820: 7468 6574 6124 292e 2050 5143 7320 6172  theta$). PQCs ar
+00000830: 6520 7061 7274 6963 756c 6172 6c79 2072  e particularly r
+00000840: 656c 6576 616e 7420 696e 2051 7561 6e74  elevant in Quant
+00000850: 756d 204d 6163 6869 6e65 204c 6561 726e  um Machine Learn
+00000860: 696e 6720 2851 4d4c 2920 6d6f 6465 6c73  ing (QML) models
+00000870: 2c20 7768 6572 6520 7468 6520 7661 6c75  , where the valu
+00000880: 6573 206f 6620 7468 6573 6520 7061 7261  es of these para
+00000890: 6d65 7465 7273 2063 616e 2062 6520 6c65  meters can be le
+000008a0: 6172 6e65 6420 6475 7269 6e67 2074 7261  arned during tra
+000008b0: 696e 696e 6720 746f 2072 6561 6368 2074  ining to reach t
+000008c0: 6865 2064 6573 6972 6564 206f 7574 7075  he desired outpu
+000008d0: 742e 0a0a 496e 2070 6172 7469 6375 6c61  t...In particula
+000008e0: 722c 2060 7169 736b 6974 2d73 796d 6260  r, `qiskit-symb`
+000008f0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+00000900: 6372 6561 7465 2061 2073 796d 626f 6c69  create a symboli
+00000910: 6320 7265 7072 6573 656e 7461 7469 6f6e  c representation
+00000920: 206f 6620 6120 7061 7261 6d65 7472 6963   of a parametric
+00000930: 2071 7561 6e74 756d 2073 7461 7465 7665   quantum stateve
+00000940: 6374 6f72 2c20 6465 6e73 6974 7920 6d61  ctor, density ma
+00000950: 7472 6978 2c20 6f72 2075 6e69 7461 7279  trix, or unitary
+00000960: 206f 7065 7261 746f 7220 6469 7265 6374   operator direct
+00000970: 6c79 2066 726f 6d20 7468 6520 5169 736b  ly from the Qisk
+00000980: 6974 2071 7561 6e74 756d 2063 6972 6375  it quantum circu
+00000990: 6974 2e20 5468 6973 2068 6173 2062 6565  it. This has bee
+000009a0: 6e20 6163 6869 6576 6564 2074 6872 6f75  n achieved throu
+000009b0: 6768 2074 6865 2072 652d 696d 706c 656d  gh the re-implem
+000009c0: 656e 7461 7469 6f6e 206f 6620 736f 6d65  entation of some
+000009d0: 2062 6173 6963 2063 6c61 7373 6573 2064   basic classes d
+000009e0: 6566 696e 6564 2069 6e20 7468 6520 5b60  efined in the [`
+000009f0: 7169 736b 6974 2f71 7561 6e74 756d 5f69  qiskit/quantum_i
+00000a00: 6e66 6f2f 605d 2868 7474 7073 3a2f 2f67  nfo/`](https://g
+00000a10: 6974 6875 622e 636f 6d2f 5169 736b 6974  ithub.com/Qiskit
+00000a20: 2f71 6973 6b69 742d 7465 7272 612f 7472  /qiskit-terra/tr
+00000a30: 6565 2f6d 6169 6e2f 7169 736b 6974 2f71  ee/main/qiskit/q
+00000a40: 7561 6e74 756d 5f69 6e66 6f29 206d 6f64  uantum_info) mod
+00000a50: 756c 6520 6279 2075 7369 6e67 205b 7379  ule by using [sy
+00000a60: 6d70 795d 2868 7474 7073 3a2f 2f67 6974  mpy](https://git
+00000a70: 6875 622e 636f 6d2f 7379 6d70 792f 7379  hub.com/sympy/sy
+00000a80: 6d70 7929 2061 7320 6120 6261 636b 656e  mpy) as a backen
+00000a90: 6420 666f 7220 7379 6d62 6f6c 6963 2065  d for symbolic e
+00000aa0: 7870 7265 7373 696f 6e73 206d 616e 6970  xpressions manip
+00000ab0: 756c 6174 696f 6e2e 0a0a 0a23 2049 6e73  ulation....# Ins
+00000ac0: 7461 6c6c 6174 696f 6e0a 0a23 2320 5573  tallation..## Us
+00000ad0: 6572 2d6d 6f64 650a 6060 600a 7069 7020  er-mode.```.pip 
+00000ae0: 696e 7374 616c 6c20 7169 736b 6974 2d73  install qiskit-s
+00000af0: 796d 620a 6060 600a 0a23 2320 4465 762d  ymb.```..## Dev-
+00000b00: 6d6f 6465 0a60 6060 0a67 6974 2063 6c6f  mode.```.git clo
+00000b10: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
+00000b20: 622e 636f 6d2f 5369 6d6f 6e65 4761 7370  b.com/SimoneGasp
+00000b30: 6572 696e 692f 7169 736b 6974 2d73 796d  erini/qiskit-sym
+00000b40: 622e 6769 740a 6364 2071 6973 6b69 742d  b.git.cd qiskit-
+00000b50: 7379 6d62 0a70 6970 2069 6e73 7461 6c6c  symb.pip install
+00000b60: 202d 6520 2e0a 6060 600a 0a0a 2320 5573   -e ..```...# Us
+00000b70: 6167 6520 6578 616d 706c 6573 0a0a 2323  age examples..##
+00000b80: 2320 5f53 796d 7069 6679 5f20 6120 5169  # _Sympify_ a Qi
+00000b90: 736b 6974 2063 6972 6375 6974 0a4c 6574  skit circuit.Let
+00000ba0: 2773 2067 6574 2073 7461 7274 6564 206f  's get started o
+00000bb0: 6e20 686f 7720 746f 2075 7365 2060 7169  n how to use `qi
+00000bc0: 736b 6974 2d73 796d 6260 2074 6f20 6765  skit-symb` to ge
+00000bd0: 7420 7468 6520 7379 6d62 6f6c 6963 2072  t the symbolic r
+00000be0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+00000bf0: 2061 2067 6976 656e 2051 6973 6b69 7420   a given Qiskit 
+00000c00: 6369 7263 7569 742e 2049 6e20 7061 7274  circuit. In part
+00000c10: 6963 756c 6172 2c20 696e 2074 6869 7320  icular, in this 
+00000c20: 6669 7273 7420 6261 7369 6320 6578 616d  first basic exam
+00000c30: 706c 652c 2077 6520 636f 6e73 6964 6572  ple, we consider
+00000c40: 2074 6865 2066 6f6c 6c6f 7769 6e67 2071   the following q
+00000c50: 7561 6e74 756d 2063 6972 6375 6974 3a0a  uantum circuit:.
+00000c60: 6060 6070 7974 686f 6e0a 6672 6f6d 2071  ```python.from q
+00000c70: 6973 6b69 7420 696d 706f 7274 2051 7561  iskit import Qua
+00000c80: 6e74 756d 4369 7263 7569 740a 6672 6f6d  ntumCircuit.from
+00000c90: 2071 6973 6b69 742e 6369 7263 7569 7420   qiskit.circuit 
+00000ca0: 696d 706f 7274 2050 6172 616d 6574 6572  import Parameter
+00000cb0: 2c20 5061 7261 6d65 7465 7256 6563 746f  , ParameterVecto
+00000cc0: 720a 0a79 203d 2050 6172 616d 6574 6572  r..y = Parameter
+00000cd0: 2827 7927 290a 7020 3d20 5061 7261 6d65  ('y').p = Parame
+00000ce0: 7465 7256 6563 746f 7228 2770 272c 206c  terVector('p', l
+00000cf0: 656e 6774 683d 3229 0a0a 7071 6320 3d20  ength=2)..pqc = 
+00000d00: 5175 616e 7475 6d43 6972 6375 6974 2832  QuantumCircuit(2
+00000d10: 290a 7071 632e 7279 2879 2c20 3029 0a70  ).pqc.ry(y, 0).p
+00000d20: 7163 2e63 7828 302c 2031 290a 7071 632e  qc.cx(0, 1).pqc.
+00000d30: 7528 302c 202a 702c 2031 290a 0a70 7163  u(0, *p, 1)..pqc
+00000d40: 2e64 7261 7728 276d 706c 2729 0a60 6060  .draw('mpl').```
+00000d50: 0a21 5b5d 282f 696d 672f 6578 616d 706c  .![](/img/exampl
+00000d60: 655f 6369 7263 7569 742e 706e 6729 0a0a  e_circuit.png)..
+00000d70: 546f 2067 6574 2074 6865 202a 7379 6d70  To get the *symp
+00000d80: 792a 2072 6570 7265 7365 6e74 6174 696f  y* representatio
+00000d90: 6e20 6f66 2074 6865 2075 6e69 7461 7279  n of the unitary
+00000da0: 206d 6174 7269 7820 636f 7272 6573 706f   matrix correspo
+00000db0: 6e64 696e 6720 746f 2074 6865 2070 6172  nding to the par
+00000dc0: 616d 6574 6572 697a 6564 2063 6972 6375  ameterized circu
+00000dd0: 6974 2c20 7765 206a 7573 7420 6861 7665  it, we just have
+00000de0: 2074 6f20 6372 6561 7465 2074 6865 2073   to create the s
+00000df0: 796d 626f 6c69 6320 604f 7065 7261 746f  ymbolic `Operato
+00000e00: 7260 2069 6e73 7461 6e63 6520 616e 6420  r` instance and 
+00000e10: 6361 6c6c 2074 6865 2060 746f 5f73 796d  call the `to_sym
+00000e20: 7079 2829 6020 6d65 7468 6f64 3a0a 6060  py()` method:.``
+00000e30: 6070 7974 686f 6e0a 6672 6f6d 2071 6973  `python.from qis
+00000e40: 6b69 745f 7379 6d62 2e71 7561 6e74 756d  kit_symb.quantum
+00000e50: 5f69 6e66 6f20 696d 706f 7274 204f 7065  _info import Ope
+00000e60: 7261 746f 720a 0a6f 7020 3d20 4f70 6572  rator..op = Oper
+00000e70: 6174 6f72 2870 7163 290a 6f70 2e74 6f5f  ator(pqc).op.to_
+00000e80: 7379 6d70 7928 290a 6060 600a 6060 606d  sympy().```.```m
+00000e90: 6174 680a 5c6c 6566 745b 5c62 6567 696e  ath.\left[\begin
+00000ea0: 7b6d 6174 7269 787d 5c63 6f73 7b5c 6c65  {matrix}\cos{\le
+00000eb0: 6674 285c 6672 6163 7b79 7d7b 327d 205c  ft(\frac{y}{2} \
+00000ec0: 7269 6768 7429 7d20 2620 2d20 5c73 696e  right)} & - \sin
+00000ed0: 7b5c 6c65 6674 285c 6672 6163 7b79 7d7b  {\left(\frac{y}{
+00000ee0: 327d 205c 7269 6768 7429 7d20 2620 3020  2} \right)} & 0 
+00000ef0: 2620 305c 5c30 2026 2030 2026 205c 7369  & 0\\0 & 0 & \si
+00000f00: 6e7b 5c6c 6566 7428 5c66 7261 637b 797d  n{\left(\frac{y}
+00000f10: 7b32 7d20 5c72 6967 6874 297d 2026 205c  {2} \right)} & \
+00000f20: 636f 737b 5c6c 6566 7428 5c66 7261 637b  cos{\left(\frac{
+00000f30: 797d 7b32 7d20 5c72 6967 6874 297d 5c5c  y}{2} \right)}\\
+00000f40: 3020 2620 3020 2620 655e 7b69 205c 6c65  0 & 0 & e^{i \le
+00000f50: 6674 2870 5b30 5d20 2b20 705b 315d 5c72  ft(p[0] + p[1]\r
+00000f60: 6967 6874 297d 205c 636f 737b 5c6c 6566  ight)} \cos{\lef
+00000f70: 7428 5c66 7261 637b 797d 7b32 7d20 5c72  t(\frac{y}{2} \r
+00000f80: 6967 6874 297d 2026 202d 2065 5e7b 6920  ight)} & - e^{i 
+00000f90: 5c6c 6566 7428 705b 305d 202b 2070 5b31  \left(p[0] + p[1
+00000fa0: 5d5c 7269 6768 7429 7d20 5c73 696e 7b5c  ]\right)} \sin{\
+00000fb0: 6c65 6674 285c 6672 6163 7b79 7d7b 327d  left(\frac{y}{2}
+00000fc0: 205c 7269 6768 7429 7d5c 5c65 5e7b 6920   \right)}\\e^{i 
+00000fd0: 5c6c 6566 7428 705b 305d 202b 2070 5b31  \left(p[0] + p[1
+00000fe0: 5d5c 7269 6768 7429 7d20 5c73 696e 7b5c  ]\right)} \sin{\
+00000ff0: 6c65 6674 285c 6672 6163 7b79 7d7b 327d  left(\frac{y}{2}
+00001000: 205c 7269 6768 7429 7d20 2620 655e 7b69   \right)} & e^{i
+00001010: 205c 6c65 6674 2870 5b30 5d20 2b20 705b   \left(p[0] + p[
+00001020: 315d 5c72 6967 6874 297d 205c 636f 737b  1]\right)} \cos{
+00001030: 5c6c 6566 7428 5c66 7261 637b 797d 7b32  \left(\frac{y}{2
+00001040: 7d20 5c72 6967 6874 297d 2026 2030 2026  } \right)} & 0 &
+00001050: 2030 5c65 6e64 7b6d 6174 7269 787d 5c72   0\end{matrix}\r
+00001060: 6967 6874 5d0a 6060 600a 0a49 6620 796f  ight].```..If yo
+00001070: 7520 7761 6e74 2074 6865 6e20 746f 2061  u want then to a
+00001080: 7373 6967 6e20 6120 7661 6c75 6520 746f  ssign a value to
+00001090: 2073 6f6d 6520 7370 6563 6966 6963 2070   some specific p
+000010a0: 6172 616d 6574 6572 2c20 796f 7520 6361  arameter, you ca
+000010b0: 6e20 7573 6520 7468 6520 6073 7562 7328  n use the `subs(
+000010c0: 3c64 6963 743e 2960 206d 6574 686f 6420  <dict>)` method 
+000010d0: 7061 7373 696e 6720 6120 6469 6374 696f  passing a dictio
+000010e0: 6e61 7279 2074 6861 7420 6d61 7073 2065  nary that maps e
+000010f0: 6163 6820 7061 7261 6d65 7465 7220 746f  ach parameter to
+00001100: 2074 6865 2064 6573 6972 6564 2063 6f72   the desired cor
+00001110: 7265 7370 6f6e 6469 6e67 2076 616c 7565  responding value
+00001120: 3a0a 6060 6070 7974 686f 6e0a 6e65 775f  :.```python.new_
+00001130: 6f70 203d 206f 702e 7375 6273 287b 703a  op = op.subs({p:
+00001140: 205b 2d31 2c20 325d 7d29 0a6e 6577 5f6f   [-1, 2]}).new_o
+00001150: 702e 746f 5f73 796d 7079 2829 0a60 6060  p.to_sympy().```
+00001160: 0a60 6060 6d61 7468 0a5c 6c65 6674 5b5c  .```math.\left[\
+00001170: 6265 6769 6e7b 6d61 7472 6978 7d5c 636f  begin{matrix}\co
+00001180: 737b 5c6c 6566 7428 5c66 7261 637b 797d  s{\left(\frac{y}
+00001190: 7b32 7d20 5c72 6967 6874 297d 2026 202d  {2} \right)} & -
+000011a0: 205c 7369 6e7b 5c6c 6566 7428 5c66 7261   \sin{\left(\fra
+000011b0: 637b 797d 7b32 7d20 5c72 6967 6874 297d  c{y}{2} \right)}
+000011c0: 2026 2030 2026 2030 5c5c 3020 2620 3020   & 0 & 0\\0 & 0 
+000011d0: 2620 5c73 696e 7b5c 6c65 6674 285c 6672  & \sin{\left(\fr
+000011e0: 6163 7b79 7d7b 327d 205c 7269 6768 7429  ac{y}{2} \right)
+000011f0: 7d20 2620 5c63 6f73 7b5c 6c65 6674 285c  } & \cos{\left(\
+00001200: 6672 6163 7b79 7d7b 327d 205c 7269 6768  frac{y}{2} \righ
+00001210: 7429 7d5c 5c30 2026 2030 2026 2065 5e7b  t)}\\0 & 0 & e^{
+00001220: 697d 205c 636f 737b 5c6c 6566 7428 5c66  i} \cos{\left(\f
+00001230: 7261 637b 797d 7b32 7d20 5c72 6967 6874  rac{y}{2} \right
+00001240: 297d 2026 202d 2065 5e7b 697d 205c 7369  )} & - e^{i} \si
+00001250: 6e7b 5c6c 6566 7428 5c66 7261 637b 797d  n{\left(\frac{y}
+00001260: 7b32 7d20 5c72 6967 6874 297d 5c5c 655e  {2} \right)}\\e^
+00001270: 7b69 7d20 5c73 696e 7b5c 6c65 6674 285c  {i} \sin{\left(\
+00001280: 6672 6163 7b79 7d7b 327d 205c 7269 6768  frac{y}{2} \righ
+00001290: 7429 7d20 2620 655e 7b69 7d20 5c63 6f73  t)} & e^{i} \cos
+000012a0: 7b5c 6c65 6674 285c 6672 6163 7b79 7d7b  {\left(\frac{y}{
+000012b0: 327d 205c 7269 6768 7429 7d20 2620 3020  2} \right)} & 0 
+000012c0: 2620 305c 656e 647b 6d61 7472 6978 7d5c  & 0\end{matrix}\
+000012d0: 7269 6768 745d 0a60 6060 0a0a 2323 2320  right].```..### 
+000012e0: 5f4c 616d 6264 6966 795f 2061 2051 6973  _Lambdify_ a Qis
+000012f0: 6b69 7420 6369 7263 7569 740a 4769 7665  kit circuit.Give
+00001300: 6e20 6120 5169 736b 6974 2063 6972 6375  n a Qiskit circu
+00001310: 6974 2c20 6071 6973 6b69 742d 7379 6d62  it, `qiskit-symb
+00001320: 6020 616c 736f 2061 6c6c 6f77 7320 746f  ` also allows to
+00001330: 2067 656e 6572 6174 6520 6120 5079 7468   generate a Pyth
+00001340: 6f6e 206c 616d 6264 6120 6675 6e63 7469  on lambda functi
+00001350: 6f6e 2077 6974 6820 6163 7475 616c 2061  on with actual a
+00001360: 7267 756d 656e 7473 206d 6174 6368 696e  rguments matchin
+00001370: 6720 7468 6520 5169 736b 6974 2075 6e62  g the Qiskit unb
+00001380: 6f75 6e64 2070 6172 616d 6574 6572 732e  ound parameters.
+00001390: 0a4c 6574 2773 2063 6f6e 7369 6465 7220  .Let's consider 
+000013a0: 7468 6520 666f 6c6c 6f77 696e 6720 6578  the following ex
+000013b0: 616d 706c 6520 7374 6172 7469 6e67 2066  ample starting f
+000013c0: 726f 6d20 6120 605a 5a46 6561 7475 7265  rom a `ZZFeature
+000013d0: 4d61 7060 2063 6972 6375 6974 2c20 636f  Map` circuit, co
+000013e0: 6d6d 6f6e 6c79 2075 7365 6420 6173 2061  mmonly used as a
+000013f0: 2064 6174 6120 656d 6265 6464 696e 6720   data embedding 
+00001400: 616e 7361 747a 2069 6e20 514d 4c20 6170  ansatz in QML ap
+00001410: 706c 6963 6174 696f 6e73 3a0a 6060 6070  plications:.```p
+00001420: 7974 686f 6e0a 6672 6f6d 2071 6973 6b69  ython.from qiski
+00001430: 742e 6369 7263 7569 742e 6c69 6272 6172  t.circuit.librar
+00001440: 7920 696d 706f 7274 205a 5a46 6561 7475  y import ZZFeatu
+00001450: 7265 4d61 700a 0a70 7163 203d 205a 5a46  reMap..pqc = ZZF
+00001460: 6561 7475 7265 4d61 7028 6665 6174 7572  eatureMap(featur
+00001470: 655f 6469 6d65 6e73 696f 6e3d 332c 2072  e_dimension=3, r
+00001480: 6570 733d 3129 0a70 7163 2e64 7261 7728  eps=1).pqc.draw(
+00001490: 276d 706c 2729 0a60 6060 0a21 5b5d 282f  'mpl').```.![](/
+000014a0: 696d 672f 7a7a 6665 6174 7572 656d 6170  img/zzfeaturemap
+000014b0: 5f63 6972 6375 6974 2e70 6e67 290a 0a54  _circuit.png)..T
+000014c0: 6f20 6765 7420 7468 6520 5079 7468 6f6e  o get the Python
+000014d0: 2066 756e 6374 696f 6e20 7265 7072 6573   function repres
+000014e0: 656e 7469 6e67 2074 6865 2066 696e 616c  enting the final
+000014f0: 2070 6172 616d 6574 6572 6963 2073 7461   parameteric sta
+00001500: 7465 7665 6374 6f72 2c20 7765 206a 7573  tevector, we jus
+00001510: 7420 6861 7665 2074 6f20 6372 6561 7465  t have to create
+00001520: 2074 6865 2073 796d 626f 6c69 6320 6053   the symbolic `S
+00001530: 7461 7465 7665 6374 6f72 6020 696e 7374  tatevector` inst
+00001540: 616e 6365 2061 6e64 2063 616c 6c20 7468  ance and call th
+00001550: 6520 6074 6f5f 6c61 6d62 6461 2829 6020  e `to_lambda()` 
+00001560: 6d65 7468 6f64 3a0a 6060 6070 7974 686f  method:.```pytho
+00001570: 6e0a 6672 6f6d 2071 6973 6b69 745f 7379  n.from qiskit_sy
+00001580: 6d62 2e71 7561 6e74 756d 5f69 6e66 6f20  mb.quantum_info 
+00001590: 696d 706f 7274 2053 7461 7465 7665 6374  import Statevect
+000015a0: 6f72 0a0a 7071 6320 3d20 7071 632e 6465  or..pqc = pqc.de
+000015b0: 636f 6d70 6f73 6528 290a 7374 6174 6576  compose().statev
+000015c0: 6563 203d 2053 7461 7465 7665 6374 6f72  ec = Statevector
+000015d0: 2870 7163 292e 746f 5f6c 616d 6264 6128  (pqc).to_lambda(
+000015e0: 290a 6060 600a 0a57 6520 6361 6e20 6e6f  ).```..We can no
+000015f0: 7720 6361 6c6c 2074 6865 206c 616d 6264  w call the lambd
+00001600: 612d 6765 6e65 7261 7465 6420 6675 6e63  a-generated func
+00001610: 7469 6f6e 2060 7374 6174 6576 6563 6020  tion `statevec` 
+00001620: 7061 7373 696e 6720 7468 6520 6078 6020  passing the `x` 
+00001630: 7661 6c75 6573 2077 6520 7761 6e74 2074  values we want t
+00001640: 6f20 6173 7369 676e 2074 6f20 6561 6368  o assign to each
+00001650: 2070 6172 616d 6574 6572 2e20 5468 6520   parameter. The 
+00001660: 7265 7475 726e 6564 206f 626a 6563 7420  returned object 
+00001670: 7769 6c6c 2062 6520 6120 2a6e 756d 7079  will be a *numpy
+00001680: 2a20 3244 2d61 7272 6179 2028 7769 7468  * 2D-array (with
+00001690: 2060 7368 6170 653d 2838 2c31 2960 2069   `shape=(8,1)` i
+000016a0: 6e20 7468 6973 2063 6173 6529 2072 6570  n this case) rep
+000016b0: 7265 7365 6e74 696e 6720 7468 6520 6669  resenting the fi
+000016c0: 6e61 6c20 6f75 7470 7574 2073 7461 7465  nal output state
+000016d0: 7665 6374 6f72 2060 7073 6960 2e0a 6060  vector `psi`..``
+000016e0: 6070 7974 686f 6e0a 7820 3d20 5b31 2e32  `python.x = [1.2
+000016f0: 342c 2032 2e32 372c 2030 2e32 395d 0a70  4, 2.27, 0.29].p
+00001700: 7369 203d 2073 7461 7465 7665 6328 2a78  si = statevec(*x
+00001710: 290a 6060 600a 0a54 6869 7320 6665 6174  ).```..This feat
+00001720: 7572 6520 6361 6e20 6265 2075 7365 6675  ure can be usefu
+00001730: 6c20 7768 656e 2c20 6769 7665 6e20 6120  l when, given a 
+00001740: 5169 736b 6974 2050 5143 2c20 7765 2077  Qiskit PQC, we w
+00001750: 616e 7420 746f 2072 756e 2069 7420 6d75  ant to run it mu
+00001760: 6c74 6970 6c65 2074 696d 6573 2077 6974  ltiple times wit
+00001770: 6820 6469 6666 6572 656e 7420 7061 7261  h different para
+00001780: 6d65 7465 7273 2076 616c 7565 732e 2049  meters values. I
+00001790: 6e64 6565 642c 2077 6520 6361 6e20 7065  ndeed, we can pe
+000017a0: 7266 6f72 6d20 6120 7369 6e67 6c65 2073  rform a single s
+000017b0: 796d 626f 6c69 6320 6576 616c 7574 6174  ymbolic evalutat
+000017c0: 696f 6e20 616e 6420 7468 656e 2063 616c  ion and then cal
+000017d0: 6c20 7468 6520 6c61 6d62 6461 2067 656e  l the lambda gen
+000017e0: 6572 6174 6564 2066 756e 6374 696f 6e20  erated function 
+000017f0: 6173 206d 616e 7920 7469 6d65 7320 6173  as many times as
+00001800: 206e 6565 6465 642c 2070 6173 7369 6e67   needed, passing
+00001810: 2064 6966 6665 7265 6e74 2076 616c 7565   different value
+00001820: 7320 6f66 2074 6865 2070 6172 616d 6574  s of the paramet
+00001830: 6572 7320 6174 2065 6163 6820 6974 6572  ers at each iter
+00001840: 6174 696f 6e2e 0a0a 2320 436f 6e74 7269  ation...# Contri
+00001850: 6275 746f 7273 0a0a 3c74 6162 6c65 3e0a  butors..<table>.
+00001860: 2020 3c74 723e 0a20 2020 203c 7464 2061    <tr>.    <td a
+00001870: 6c69 676e 3d22 6365 6e74 6572 223e 3c61  lign="center"><a
+00001880: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00001890: 6974 6875 622e 636f 6d2f 5369 6d6f 6e65  ithub.com/Simone
+000018a0: 4761 7370 6572 696e 6922 3e3c 696d 6720  Gasperini"><img 
+000018b0: 7372 633d 2268 7474 7073 3a2f 2f61 7661  src="https://ava
+000018c0: 7461 7273 322e 6769 7468 7562 7573 6572  tars2.githubuser
+000018d0: 636f 6e74 656e 742e 636f 6d2f 752f 3731  content.com/u/71
+000018e0: 3038 3637 3538 3f73 3d34 3030 2676 3d34  086758?s=400&v=4
+000018f0: 2220 7769 6474 683d 2231 3230 7078 3b22  " width="120px;"
+00001900: 2f3e 3c62 722f 3e3c 623e 5369 6d6f 6e65  /><br/><b>Simone
+00001910: 2047 6173 7065 7269 6e69 3c2f 623e 3c2f   Gasperini</b></
+00001920: 613e 3c2f 7464 3e0a 2020 3c2f 7472 3e0a  a></td>.  </tr>.
+00001930: 3c2f 7461 626c 653e 0a                   </table>.
```

### Comparing `qiskit-symb-0.1.2/setup.cfg` & `qiskit-symb-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qiskit-symb
-version = 0.1.2
+version = 0.1.3
 url = https://github.com/SimoneGasperini/qiskit-symb
 author = SimoneGasperini
 author_email = simone.gasperini4@unibo.it
 license = Apache 2.0
 license_files = LICENSE
 long_description_content_type = text/markdown
 long_description = file: README.md
```

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/controlledgate.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/controlledgate.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/gate.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/gate.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/__init__.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/p.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/p.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/r.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/r.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/rx.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/rx.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/rxx.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/rxx.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/ry.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/ry.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/ryy.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/ryy.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/rz.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/rz.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/rzx.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/rzx.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/rzz.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/rzz.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/parametric_gates/u.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/parametric_gates/u.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/ecr.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/ecr.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/h.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/h.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/iswap.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/iswap.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/s.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/s.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/swap.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/swap.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/sx.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/sx.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/t.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/t.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/x.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/x.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/y.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/y.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/library/standard_gates/z.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/library/standard_gates/z.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/circuit/random.py` & `qiskit-symb-0.1.3/src/qiskit_symb/circuit/random.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,34 +26,29 @@
         'ry': (standard_gates.RYGate, 1, 1),
         's': (standard_gates.SGate, 1, 0),
         'sdg': (standard_gates.SdgGate, 1, 0),
         'sxdg': (standard_gates.SXdgGate, 1, 0),
         't': (standard_gates.TGate, 1, 0),
         'tdg': (standard_gates.TdgGate, 1, 0),
         'u': (standard_gates.UGate, 1, 3),
-        # 'u1': (standard_gates.U1Gate, 1, 1), deprecated
-        # 'u2': (standard_gates.U2Gate, 1, 2), deprecated
-        # 'u3': (standard_gates.U3Gate, 1, 3), deprecated
         'y': (standard_gates.YGate, 1, 0),
         'z': (standard_gates.ZGate, 1, 0),
     }
     if num_qubits > 1:
         qiskit_gates.update({
             'cx': (standard_gates.CXGate, 2, 0),
             # 'dcx': (standard_gates.DCXGate, 2, 0), TODO
             'ch': (standard_gates.CHGate, 2, 0),
             'cp': (standard_gates.CPhaseGate, 2, 1),
             'crx': (standard_gates.CRXGate, 2, 1),
             'cry': (standard_gates.CRYGate, 2, 1),
             'crz': (standard_gates.CRZGate, 2, 1),
             'csx': (standard_gates.CSXGate, 2, 0),
-            # https://github.com/Qiskit/qiskit-terra/issues/9763
+            # https://github.com/Qiskit/qiskit-terra/issues/7326
             # 'cu': (standard_gates.CUGate, 2, 4),
-            # 'cu1': (standard_gates.CU1Gate, 2, 1), deprecated
-            # 'cu3': (standard_gates.CU3Gate, 2, 3), deprecated
             'cy': (standard_gates.CYGate, 2, 0),
             'cz': (standard_gates.CZGate, 2, 0),
             'rxx': (standard_gates.RXXGate, 2, 1),
             'ryy': (standard_gates.RYYGate, 2, 1),
             'rzz': (standard_gates.RZZGate, 2, 1),
             'rzx': (standard_gates.RZXGate, 2, 1),
             # 'xx_minus_yy': (standard_gates.XXMinusYYGate, 2, 2), TODO
```

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/quantum_info/densitymatrix.py` & `qiskit-symb-0.1.3/src/qiskit_symb/quantum_info/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/quantum_info/operator.py` & `qiskit-symb-0.1.3/src/qiskit_symb/quantum_info/operator.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/quantum_info/quantumbase.py` & `qiskit-symb-0.1.3/src/qiskit_symb/quantum_info/quantumbase.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/quantum_info/statevector.py` & `qiskit-symb-0.1.3/src/qiskit_symb/quantum_info/statevector.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb/utils.py` & `qiskit-symb-0.1.3/src/qiskit_symb/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb.egg-info/PKG-INFO` & `qiskit-symb-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,421 +1,385 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7169 736b  : 2.1.Name: qisk
-00000020: 6974 2d73 796d 620a 5665 7273 696f 6e3a  it-symb.Version:
-00000030: 2030 2e31 2e32 0a48 6f6d 652d 7061 6765   0.1.2.Home-page
-00000040: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00000050: 2e63 6f6d 2f53 696d 6f6e 6547 6173 7065  .com/SimoneGaspe
-00000060: 7269 6e69 2f71 6973 6b69 742d 7379 6d62  rini/qiskit-symb
-00000070: 0a41 7574 686f 723a 2053 696d 6f6e 6547  .Author: SimoneG
-00000080: 6173 7065 7269 6e69 0a41 7574 686f 722d  asperini.Author-
-00000090: 656d 6169 6c3a 2073 696d 6f6e 652e 6761  email: simone.ga
-000000a0: 7370 6572 696e 6934 4075 6e69 626f 2e69  sperini4@unibo.i
-000000b0: 740a 4c69 6365 6e73 653a 2041 7061 6368  t.License: Apach
-000000c0: 6520 322e 300a 5265 7175 6972 6573 2d50  e 2.0.Requires-P
-000000d0: 7974 686f 6e3a 203e 3d33 2e38 0a44 6573  ython: >=3.8.Des
-000000e0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-000000f0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000100: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
-00000110: 7472 613a 2074 6573 7469 6e67 0a4c 6963  tra: testing.Lic
-00000120: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
-00000130: 5345 0a0a 215b 5d28 2f69 6d67 2f6c 6f67  SE..![](/img/log
-00000140: 6f2e 706e 6729 0a0a 3c70 2061 6c69 676e  o.png)..<p align
-00000150: 3d22 6365 6e74 6572 223e 0a20 2020 203c  ="center">.    <
-00000160: 696d 6720 7469 746c 653d 226c 6963 656e  img title="licen
-00000170: 7365 2220 7372 633d 2268 7474 7073 3a2f  se" src="https:/
-00000180: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000190: 6261 6467 652f 6c69 6365 6e73 652d 4170  badge/license-Ap
-000001a0: 6163 6865 5f32 2e30 2d62 6c75 652e 7376  ache_2.0-blue.sv
-000001b0: 6722 3e0a 2020 2020 3c69 6d67 2074 6974  g">.    <img tit
-000001c0: 6c65 3d22 7079 7468 6f6e 2220 7372 633d  le="python" src=
-000001d0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-000001e0: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
-000001f0: 7468 6f6e 2de2 89a5 332e 382d 626c 7565  thon-...3.8-blue
-00000200: 2e73 7667 223e 0a20 2020 203c 696d 6720  .svg">.    <img 
-00000210: 7469 746c 653d 2245 636f 7379 7374 656d  title="Ecosystem
-00000220: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00000230: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000240: 6467 652f 5169 736b 6974 2d45 636f 7379  dge/Qiskit-Ecosy
-00000250: 7374 656d 2d62 6c75 6576 696f 6c65 742e  stem-blueviolet.
-00000260: 7376 6722 3e0a 3c2f 703e 0a0a 3c70 2061  svg">.</p>..<p a
-00000270: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
-00000280: 2020 203c 696d 6720 7469 746c 653d 2262     <img title="b
-00000290: 7569 6c64 2220 7372 633d 2768 7474 7073  uild" src='https
-000002a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5369  ://github.com/Si
-000002b0: 6d6f 6e65 4761 7370 6572 696e 692f 7169  moneGasperini/qi
-000002c0: 736b 6974 2d73 796d 622f 6163 7469 6f6e  skit-symb/action
-000002d0: 732f 776f 726b 666c 6f77 732f 7079 7468  s/workflows/pyth
-000002e0: 6f6e 2d70 6163 6b61 6765 2e79 6d6c 2f62  on-package.yml/b
-000002f0: 6164 6765 2e73 7667 3f62 7261 6e63 683d  adge.svg?branch=
-00000300: 6d61 7374 6572 273e 0a20 2020 203c 696d  master'>.    <im
-00000310: 6720 7469 746c 653d 2263 6f76 6572 6167  g title="coverag
-00000320: 6522 2073 7263 3d27 6874 7470 733a 2f2f  e" src='https://
-00000330: 636f 7665 7261 6c6c 732e 696f 2f72 6570  coveralls.io/rep
-00000340: 6f73 2f67 6974 6875 622f 5369 6d6f 6e65  os/github/Simone
-00000350: 4761 7370 6572 696e 692f 7169 736b 6974  Gasperini/qiskit
-00000360: 2d73 796d 622f 6261 6467 652e 7376 673f  -symb/badge.svg?
-00000370: 6272 616e 6368 3d6d 6173 7465 7227 3e0a  branch=master'>.
-00000380: 3c2f 703e 0a0a 2a2a 2a0a 0a23 2054 6162  </p>..***..# Tab
-00000390: 6c65 206f 6620 636f 6e74 656e 7473 0a2d  le of contents.-
-000003a0: 205b 496e 7472 6f64 7563 7469 6f6e 5d28   [Introduction](
-000003b0: 2369 6e74 726f 6475 6374 696f 6e29 0a2d  #introduction).-
-000003c0: 205b 496e 7374 616c 6c61 7469 6f6e 5d28   [Installation](
-000003d0: 2369 6e73 7461 6c6c 6174 696f 6e29 0a20  #installation). 
-000003e0: 2020 202d 205b 5573 6572 2d6d 6f64 655d     - [User-mode]
-000003f0: 2823 7573 6572 2d6d 6f64 6529 0a20 2020  (#user-mode).   
-00000400: 202d 205b 4465 762d 6d6f 6465 5d28 2364   - [Dev-mode](#d
-00000410: 6576 2d6d 6f64 6529 0a2d 205b 5573 6167  ev-mode).- [Usag
-00000420: 6520 6578 616d 706c 6573 5d28 2375 7361  e examples](#usa
-00000430: 6765 2d65 7861 6d70 6c65 7329 0a20 2020  ge-examples).   
-00000440: 202d 205b 5f53 796d 7069 6679 5f20 6120   - [_Sympify_ a 
-00000450: 5169 736b 6974 2063 6972 6375 6974 5d28  Qiskit circuit](
-00000460: 2373 796d 7069 6679 2d61 2d71 6973 6b69  #sympify-a-qiski
-00000470: 742d 6369 7263 7569 7429 0a20 2020 202d  t-circuit).    -
-00000480: 205b 5f4c 616d 6264 6966 795f 2061 2051   [_Lambdify_ a Q
-00000490: 6973 6b69 7420 6369 7263 7569 745d 2823  iskit circuit](#
-000004a0: 6c61 6d62 6469 6679 2d61 2d71 6973 6b69  lambdify-a-qiski
-000004b0: 742d 6369 7263 7569 7429 0a2d 205b 436f  t-circuit).- [Co
-000004c0: 6e74 7269 6275 746f 7273 5d28 2363 6f6e  ntributors](#con
-000004d0: 7472 6962 7574 6f72 7329 0a0a 0a23 2049  tributors)...# I
-000004e0: 6e74 726f 6475 6374 696f 6e0a 5468 6520  ntroduction.The 
-000004f0: 6071 6973 6b69 742d 7379 6d62 6020 7061  `qiskit-symb` pa
-00000500: 636b 6167 6520 6973 206d 6561 6e74 2074  ckage is meant t
-00000510: 6f20 6265 2061 2050 7974 686f 6e20 746f  o be a Python to
-00000520: 6f6c 2074 6f20 656e 6162 6c65 2074 6865  ol to enable the
-00000530: 2073 796d 626f 6c69 6320 6576 616c 7561   symbolic evalua
-00000540: 7469 6f6e 206f 6620 7061 7261 6d65 7472  tion of parametr
-00000550: 6963 2071 7561 6e74 756d 2073 7461 7465  ic quantum state
-00000560: 7320 616e 6420 6f70 6572 6174 6f72 7320  s and operators 
-00000570: 6465 6669 6e65 6420 696e 205b 5169 736b  defined in [Qisk
-00000580: 6974 5d28 6874 7470 733a 2f2f 6769 7468  it](https://gith
-00000590: 7562 2e63 6f6d 2f51 6973 6b69 742f 7169  ub.com/Qiskit/qi
-000005a0: 736b 6974 2d74 6572 7261 2920 6279 2070  skit-terra) by p
-000005b0: 6172 616d 6574 6572 697a 6564 2071 7561  arameterized qua
-000005c0: 6e74 756d 2063 6972 6375 6974 732e 0a0a  ntum circuits...
-000005d0: 4120 5061 7261 6d65 7465 7269 7a65 6420  A Parameterized 
-000005e0: 5175 616e 7475 6d20 4369 7263 7569 7420  Quantum Circuit 
-000005f0: 2850 5143 2920 6973 2061 2071 7561 6e74  (PQC) is a quant
-00000600: 756d 2063 6972 6375 6974 2077 6865 7265  um circuit where
-00000610: 2077 6520 6861 7665 2061 7420 6c65 6173   we have at leas
-00000620: 7420 6f6e 6520 6672 6565 2070 6172 616d  t one free param
-00000630: 6574 6572 2028 652e 672e 2061 2072 6f74  eter (e.g. a rot
-00000640: 6174 696f 6e20 616e 676c 6520 245c 7468  ation angle $\th
-00000650: 6574 6124 292e 2050 5143 7320 6172 6520  eta$). PQCs are 
-00000660: 7061 7274 6963 756c 6172 6c79 2072 656c  particularly rel
-00000670: 6576 616e 7420 696e 2051 7561 6e74 756d  evant in Quantum
-00000680: 204d 6163 6869 6e65 204c 6561 726e 696e   Machine Learnin
-00000690: 6720 2851 4d4c 2920 6d6f 6465 6c73 2c20  g (QML) models, 
-000006a0: 7768 6572 6520 7468 6520 7661 6c75 6573  where the values
-000006b0: 206f 6620 7468 6573 6520 7061 7261 6d65   of these parame
-000006c0: 7465 7273 2063 616e 2062 6520 6c65 6172  ters can be lear
-000006d0: 6e65 6420 6475 7269 6e67 2074 7261 696e  ned during train
-000006e0: 696e 6720 746f 2072 6561 6368 2074 6865  ing to reach the
-000006f0: 2064 6573 6972 6564 206f 7574 7075 742e   desired output.
-00000700: 0a0a 496e 2070 6172 7469 6375 6c61 722c  ..In particular,
-00000710: 2060 7169 736b 6974 2d73 796d 6260 2063   `qiskit-symb` c
-00000720: 616e 2062 6520 7573 6564 2074 6f20 6372  an be used to cr
-00000730: 6561 7465 2061 2073 796d 626f 6c69 6320  eate a symbolic 
-00000740: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-00000750: 6620 6120 7061 7261 6d65 7472 6963 2071  f a parametric q
-00000760: 7561 6e74 756d 2073 7461 7465 7665 6374  uantum statevect
-00000770: 6f72 2c20 6465 6e73 6974 7920 6d61 7472  or, density matr
-00000780: 6978 2c20 6f72 2075 6e69 7461 7279 206f  ix, or unitary o
-00000790: 7065 7261 746f 7220 6469 7265 6374 6c79  perator directly
-000007a0: 2066 726f 6d20 7468 6520 5169 736b 6974   from the Qiskit
-000007b0: 2071 7561 6e74 756d 2063 6972 6375 6974   quantum circuit
-000007c0: 2e20 5468 6973 2068 6173 2062 6565 6e20  . This has been 
-000007d0: 6163 6869 6576 6564 2074 6872 6f75 6768  achieved through
-000007e0: 2074 6865 2072 652d 696d 706c 656d 656e   the re-implemen
-000007f0: 7461 7469 6f6e 206f 6620 736f 6d65 2062  tation of some b
-00000800: 6173 6963 2063 6c61 7373 6573 2064 6566  asic classes def
-00000810: 696e 6564 2069 6e20 7468 6520 5b60 7169  ined in the [`qi
-00000820: 736b 6974 2f71 7561 6e74 756d 5f69 6e66  skit/quantum_inf
-00000830: 6f2f 605d 2868 7474 7073 3a2f 2f67 6974  o/`](https://git
-00000840: 6875 622e 636f 6d2f 5169 736b 6974 2f71  hub.com/Qiskit/q
-00000850: 6973 6b69 742d 7465 7272 612f 7472 6565  iskit-terra/tree
-00000860: 2f6d 6169 6e2f 7169 736b 6974 2f71 7561  /main/qiskit/qua
-00000870: 6e74 756d 5f69 6e66 6f29 206d 6f64 756c  ntum_info) modul
-00000880: 6520 6279 2075 7369 6e67 205b 7379 6d70  e by using [symp
-00000890: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-000008a0: 622e 636f 6d2f 7379 6d70 792f 7379 6d70  b.com/sympy/symp
-000008b0: 7929 2061 7320 6120 6261 636b 656e 6420  y) as a backend 
-000008c0: 666f 7220 7379 6d62 6f6c 6963 2065 7870  for symbolic exp
-000008d0: 7265 7373 696f 6e73 206d 616e 6970 756c  ressions manipul
-000008e0: 6174 696f 6e2e 0a0a 0a23 2049 6e73 7461  ation....# Insta
-000008f0: 6c6c 6174 696f 6e0a 0a23 2320 5573 6572  llation..## User
-00000900: 2d6d 6f64 650a 6060 600a 7069 7020 696e  -mode.```.pip in
-00000910: 7374 616c 6c20 7169 736b 6974 2d73 796d  stall qiskit-sym
-00000920: 620a 6060 600a 0a23 2320 4465 762d 6d6f  b.```..## Dev-mo
-00000930: 6465 0a60 6060 0a67 6974 2063 6c6f 6e65  de.```.git clone
-00000940: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000950: 636f 6d2f 5369 6d6f 6e65 4761 7370 6572  com/SimoneGasper
-00000960: 696e 692f 7169 736b 6974 2d73 796d 622e  ini/qiskit-symb.
-00000970: 6769 740a 6364 2071 6973 6b69 742d 7379  git.cd qiskit-sy
-00000980: 6d62 0a70 6970 2069 6e73 7461 6c6c 202d  mb.pip install -
-00000990: 6520 2e0a 6060 600a 0a0a 2320 5573 6167  e ..```...# Usag
-000009a0: 6520 6578 616d 706c 6573 0a0a 2323 2320  e examples..### 
-000009b0: 5f53 796d 7069 6679 5f20 6120 5169 736b  _Sympify_ a Qisk
-000009c0: 6974 2063 6972 6375 6974 0a4c 6574 2773  it circuit.Let's
-000009d0: 2067 6574 2073 7461 7274 6564 206f 6e20   get started on 
-000009e0: 686f 7720 746f 2075 7365 2060 7169 736b  how to use `qisk
-000009f0: 6974 2d73 796d 6260 2074 6f20 6765 7420  it-symb` to get 
-00000a00: 7468 6520 7379 6d62 6f6c 6963 2072 6570  the symbolic rep
-00000a10: 7265 7365 6e74 6174 696f 6e20 6f66 2061  resentation of a
-00000a20: 2067 6976 656e 2051 6973 6b69 7420 6369   given Qiskit ci
-00000a30: 7263 7569 742e 2049 6e20 7061 7274 6963  rcuit. In partic
-00000a40: 756c 6172 2c20 696e 2074 6869 7320 6669  ular, in this fi
-00000a50: 7273 7420 6261 7369 6320 6578 616d 706c  rst basic exampl
-00000a60: 652c 2077 6520 636f 6e73 6964 6572 2074  e, we consider t
-00000a70: 6865 2066 6f6c 6c6f 7769 6e67 2071 7561  he following qua
-00000a80: 6e74 756d 2063 6972 6375 6974 3a0a 6060  ntum circuit:.``
-00000a90: 6070 7974 686f 6e0a 6672 6f6d 2071 6973  `python.from qis
-00000aa0: 6b69 7420 696d 706f 7274 2051 7561 6e74  kit import Quant
-00000ab0: 756d 4369 7263 7569 740a 6672 6f6d 2071  umCircuit.from q
-00000ac0: 6973 6b69 742e 6369 7263 7569 7420 696d  iskit.circuit im
-00000ad0: 706f 7274 2050 6172 616d 6574 6572 2c20  port Parameter, 
-00000ae0: 5061 7261 6d65 7465 7256 6563 746f 720a  ParameterVector.
-00000af0: 0a79 203d 2050 6172 616d 6574 6572 2827  .y = Parameter('
-00000b00: 7927 290a 7020 3d20 5061 7261 6d65 7465  y').p = Paramete
-00000b10: 7256 6563 746f 7228 2770 272c 206c 656e  rVector('p', len
-00000b20: 6774 683d 3229 0a0a 7071 6320 3d20 5175  gth=2)..pqc = Qu
-00000b30: 616e 7475 6d43 6972 6375 6974 2832 290a  antumCircuit(2).
-00000b40: 7071 632e 7279 2879 2c20 3029 0a70 7163  pqc.ry(y, 0).pqc
-00000b50: 2e63 7828 302c 2031 290a 7071 632e 7528  .cx(0, 1).pqc.u(
-00000b60: 302c 202a 702c 2031 290a 0a70 7163 2e64  0, *p, 1)..pqc.d
-00000b70: 7261 7728 276d 706c 2729 0a60 6060 0a21  raw('mpl').```.!
-00000b80: 5b5d 282f 696d 672f 6578 616d 706c 655f  [](/img/example_
-00000b90: 6369 7263 7569 742e 706e 6729 0a0a 546f  circuit.png)..To
-00000ba0: 2067 6574 2074 6865 202a 7379 6d70 792a   get the *sympy*
-00000bb0: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-00000bc0: 6f66 2074 6865 2075 6e69 7461 7279 206d  of the unitary m
-00000bd0: 6174 7269 7820 636f 7272 6573 706f 6e64  atrix correspond
-00000be0: 696e 6720 746f 2074 6865 2070 6172 616d  ing to the param
-00000bf0: 6574 6572 697a 6564 2063 6972 6375 6974  eterized circuit
-00000c00: 2c20 7765 206a 7573 7420 6861 7665 2074  , we just have t
-00000c10: 6f20 6372 6561 7465 2074 6865 2073 796d  o create the sym
-00000c20: 626f 6c69 6320 604f 7065 7261 746f 7260  bolic `Operator`
-00000c30: 2069 6e73 7461 6e63 6520 616e 6420 6361   instance and ca
-00000c40: 6c6c 2074 6865 2060 746f 5f73 796d 7079  ll the `to_sympy
-00000c50: 2829 6020 6d65 7468 6f64 3a0a 6060 6070  ()` method:.```p
-00000c60: 7974 686f 6e0a 6672 6f6d 2071 6973 6b69  ython.from qiski
-00000c70: 745f 7379 6d62 2e71 7561 6e74 756d 5f69  t_symb.quantum_i
-00000c80: 6e66 6f20 696d 706f 7274 204f 7065 7261  nfo import Opera
-00000c90: 746f 720a 0a6f 7020 3d20 4f70 6572 6174  tor..op = Operat
-00000ca0: 6f72 2870 7163 290a 6f70 2e74 6f5f 7379  or(pqc).op.to_sy
-00000cb0: 6d70 7928 290a 6060 600a 6060 606d 6174  mpy().```.```mat
-00000cc0: 680a 5c6c 6566 745b 5c62 6567 696e 7b6d  h.\left[\begin{m
-00000cd0: 6174 7269 787d 5c63 6f73 7b5c 6c65 6674  atrix}\cos{\left
-00000ce0: 285c 6672 6163 7b79 7d7b 327d 205c 7269  (\frac{y}{2} \ri
-00000cf0: 6768 7429 7d20 2620 2d20 5c73 696e 7b5c  ght)} & - \sin{\
-00000d00: 6c65 6674 285c 6672 6163 7b79 7d7b 327d  left(\frac{y}{2}
-00000d10: 205c 7269 6768 7429 7d20 2620 3020 2620   \right)} & 0 & 
-00000d20: 305c 5c30 2026 2030 2026 205c 7369 6e7b  0\\0 & 0 & \sin{
-00000d30: 5c6c 6566 7428 5c66 7261 637b 797d 7b32  \left(\frac{y}{2
-00000d40: 7d20 5c72 6967 6874 297d 2026 205c 636f  } \right)} & \co
-00000d50: 737b 5c6c 6566 7428 5c66 7261 637b 797d  s{\left(\frac{y}
-00000d60: 7b32 7d20 5c72 6967 6874 297d 5c5c 3020  {2} \right)}\\0 
-00000d70: 2620 3020 2620 655e 7b69 205c 6c65 6674  & 0 & e^{i \left
-00000d80: 2870 5b30 5d20 2b20 705b 315d 5c72 6967  (p[0] + p[1]\rig
-00000d90: 6874 297d 205c 636f 737b 5c6c 6566 7428  ht)} \cos{\left(
-00000da0: 5c66 7261 637b 797d 7b32 7d20 5c72 6967  \frac{y}{2} \rig
-00000db0: 6874 297d 2026 202d 2065 5e7b 6920 5c6c  ht)} & - e^{i \l
-00000dc0: 6566 7428 705b 305d 202b 2070 5b31 5d5c  eft(p[0] + p[1]\
-00000dd0: 7269 6768 7429 7d20 5c73 696e 7b5c 6c65  right)} \sin{\le
-00000de0: 6674 285c 6672 6163 7b79 7d7b 327d 205c  ft(\frac{y}{2} \
-00000df0: 7269 6768 7429 7d5c 5c65 5e7b 6920 5c6c  right)}\\e^{i \l
-00000e00: 6566 7428 705b 305d 202b 2070 5b31 5d5c  eft(p[0] + p[1]\
-00000e10: 7269 6768 7429 7d20 5c73 696e 7b5c 6c65  right)} \sin{\le
-00000e20: 6674 285c 6672 6163 7b79 7d7b 327d 205c  ft(\frac{y}{2} \
-00000e30: 7269 6768 7429 7d20 2620 655e 7b69 205c  right)} & e^{i \
-00000e40: 6c65 6674 2870 5b30 5d20 2b20 705b 315d  left(p[0] + p[1]
-00000e50: 5c72 6967 6874 297d 205c 636f 737b 5c6c  \right)} \cos{\l
-00000e60: 6566 7428 5c66 7261 637b 797d 7b32 7d20  eft(\frac{y}{2} 
-00000e70: 5c72 6967 6874 297d 2026 2030 2026 2030  \right)} & 0 & 0
-00000e80: 5c65 6e64 7b6d 6174 7269 787d 5c72 6967  \end{matrix}\rig
-00000e90: 6874 5d0a 6060 600a 0a49 6620 796f 7520  ht].```..If you 
-00000ea0: 7761 6e74 2074 6865 6e20 746f 2061 7373  want then to ass
-00000eb0: 6967 6e20 6120 7661 6c75 6520 746f 2073  ign a value to s
-00000ec0: 6f6d 6520 7370 6563 6966 6963 2070 6172  ome specific par
-00000ed0: 616d 6574 6572 2c20 796f 7520 6361 6e20  ameter, you can 
-00000ee0: 7573 6520 7468 6520 6073 7562 7328 3c64  use the `subs(<d
-00000ef0: 6963 743e 2960 206d 6574 686f 6420 7061  ict>)` method pa
-00000f00: 7373 696e 6720 6120 6469 6374 696f 6e61  ssing a dictiona
-00000f10: 7279 2074 6861 7420 6d61 7073 2065 6163  ry that maps eac
-00000f20: 6820 7061 7261 6d65 7465 7220 746f 2074  h parameter to t
-00000f30: 6865 2064 6573 6972 6564 2063 6f72 7265  he desired corre
-00000f40: 7370 6f6e 6469 6e67 2076 616c 7565 3a0a  sponding value:.
-00000f50: 6060 6070 7974 686f 6e0a 7061 7261 6d73  ```python.params
-00000f60: 3276 616c 7565 203d 207b 703a 205b 2d31  2value = {p: [-1
-00000f70: 2c20 325d 7d0a 6e65 775f 6f70 203d 206f  , 2]}.new_op = o
-00000f80: 702e 7375 6273 2870 6172 616d 7332 7661  p.subs(params2va
-00000f90: 6c75 6529 0a6e 6577 5f6f 702e 746f 5f73  lue).new_op.to_s
-00000fa0: 796d 7079 2829 0a60 6060 0a60 6060 6d61  ympy().```.```ma
-00000fb0: 7468 0a5c 6c65 6674 5b5c 6265 6769 6e7b  th.\left[\begin{
-00000fc0: 6d61 7472 6978 7d5c 636f 737b 5c6c 6566  matrix}\cos{\lef
-00000fd0: 7428 5c66 7261 637b 797d 7b32 7d20 5c72  t(\frac{y}{2} \r
-00000fe0: 6967 6874 297d 2026 202d 205c 7369 6e7b  ight)} & - \sin{
-00000ff0: 5c6c 6566 7428 5c66 7261 637b 797d 7b32  \left(\frac{y}{2
-00001000: 7d20 5c72 6967 6874 297d 2026 2030 2026  } \right)} & 0 &
-00001010: 2030 5c5c 3020 2620 3020 2620 5c73 696e   0\\0 & 0 & \sin
-00001020: 7b5c 6c65 6674 285c 6672 6163 7b79 7d7b  {\left(\frac{y}{
-00001030: 327d 205c 7269 6768 7429 7d20 2620 5c63  2} \right)} & \c
-00001040: 6f73 7b5c 6c65 6674 285c 6672 6163 7b79  os{\left(\frac{y
-00001050: 7d7b 327d 205c 7269 6768 7429 7d5c 5c30  }{2} \right)}\\0
-00001060: 2026 2030 2026 2065 5e7b 697d 205c 636f   & 0 & e^{i} \co
-00001070: 737b 5c6c 6566 7428 5c66 7261 637b 797d  s{\left(\frac{y}
-00001080: 7b32 7d20 5c72 6967 6874 297d 2026 202d  {2} \right)} & -
-00001090: 2065 5e7b 697d 205c 7369 6e7b 5c6c 6566   e^{i} \sin{\lef
-000010a0: 7428 5c66 7261 637b 797d 7b32 7d20 5c72  t(\frac{y}{2} \r
-000010b0: 6967 6874 297d 5c5c 655e 7b69 7d20 5c73  ight)}\\e^{i} \s
-000010c0: 696e 7b5c 6c65 6674 285c 6672 6163 7b79  in{\left(\frac{y
-000010d0: 7d7b 327d 205c 7269 6768 7429 7d20 2620  }{2} \right)} & 
-000010e0: 655e 7b69 7d20 5c63 6f73 7b5c 6c65 6674  e^{i} \cos{\left
-000010f0: 285c 6672 6163 7b79 7d7b 327d 205c 7269  (\frac{y}{2} \ri
-00001100: 6768 7429 7d20 2620 3020 2620 305c 656e  ght)} & 0 & 0\en
-00001110: 647b 6d61 7472 6978 7d5c 7269 6768 745d  d{matrix}\right]
-00001120: 0a60 6060 0a0a 2323 2320 5f4c 616d 6264  .```..### _Lambd
-00001130: 6966 795f 2061 2051 6973 6b69 7420 6369  ify_ a Qiskit ci
-00001140: 7263 7569 740a 4769 7665 6e20 6120 5169  rcuit.Given a Qi
-00001150: 736b 6974 2063 6972 6375 6974 2c20 6071  skit circuit, `q
-00001160: 6973 6b69 742d 7379 6d62 6020 616c 736f  iskit-symb` also
-00001170: 2061 6c6c 6f77 7320 746f 2067 656e 6572   allows to gener
-00001180: 6174 6520 6120 5079 7468 6f6e 206c 616d  ate a Python lam
-00001190: 6264 6120 6675 6e63 7469 6f6e 2077 6974  bda function wit
-000011a0: 6820 6163 7475 616c 2061 7267 756d 656e  h actual argumen
-000011b0: 7473 206d 6174 6368 696e 6720 7468 6520  ts matching the 
-000011c0: 5169 736b 6974 2075 6e62 6f75 6e64 6564  Qiskit unbounded
-000011d0: 2070 6172 616d 6574 6572 732e 0a4c 6574   parameters..Let
-000011e0: 2773 2063 6f6e 7369 6465 7220 7468 6520  's consider the 
-000011f0: 666f 6c6c 6f77 696e 6720 6578 616d 706c  following exampl
-00001200: 6520 7374 6172 7469 6e67 2066 726f 6d20  e starting from 
-00001210: 6120 605a 5a46 6561 7475 7265 4d61 7060  a `ZZFeatureMap`
-00001220: 2063 6972 6375 6974 2c20 636f 6d6d 6f6e   circuit, common
-00001230: 6c79 2075 7365 6420 6173 2061 2064 6174  ly used as a dat
-00001240: 6120 656d 6265 6464 696e 6720 616e 7361  a embedding ansa
-00001250: 747a 2069 6e20 514d 4c20 6170 706c 6963  tz in QML applic
-00001260: 6174 696f 6e73 3a0a 6060 6070 7974 686f  ations:.```pytho
-00001270: 6e0a 6672 6f6d 2071 6973 6b69 742e 6369  n.from qiskit.ci
-00001280: 7263 7569 742e 6c69 6272 6172 7920 696d  rcuit.library im
-00001290: 706f 7274 205a 5a46 6561 7475 7265 4d61  port ZZFeatureMa
-000012a0: 700a 0a70 7163 203d 205a 5a46 6561 7475  p..pqc = ZZFeatu
-000012b0: 7265 4d61 7028 6665 6174 7572 655f 6469  reMap(feature_di
-000012c0: 6d65 6e73 696f 6e3d 332c 2072 6570 733d  mension=3, reps=
-000012d0: 3129 0a70 7163 2e64 7261 7728 276d 706c  1).pqc.draw('mpl
-000012e0: 2729 0a60 6060 0a21 5b5d 282f 696d 672f  ').```.![](/img/
-000012f0: 7a7a 6665 6174 7572 656d 6170 5f63 6972  zzfeaturemap_cir
-00001300: 6375 6974 2e70 6e67 290a 0a54 6f20 6765  cuit.png)..To ge
-00001310: 7420 7468 6520 5079 7468 6f6e 206c 616d  t the Python lam
-00001320: 6264 6120 6675 6e63 7469 6f6e 2072 6570  bda function rep
-00001330: 7265 7365 6e74 696e 672c 2066 6f72 2069  resenting, for i
-00001340: 6e73 7461 6e63 652c 2074 6865 2066 696e  nstance, the fin
-00001350: 616c 2070 6172 616d 6574 6572 697a 6564  al parameterized
-00001360: 2073 7461 7465 7665 6374 6f72 2c20 7765   statevector, we
-00001370: 206a 7573 7420 6861 7665 2074 6f20 6372   just have to cr
-00001380: 6561 7465 2074 6865 2073 796d 626f 6c69  eate the symboli
-00001390: 6320 6053 7461 7465 7665 6374 6f72 6020  c `Statevector` 
-000013a0: 696e 7374 616e 6365 2061 6e64 2063 616c  instance and cal
-000013b0: 6c20 7468 6520 6074 6f5f 6c61 6d62 6461  l the `to_lambda
-000013c0: 2829 6020 6d65 7468 6f64 3a0a 6060 6070  ()` method:.```p
-000013d0: 7974 686f 6e0a 6672 6f6d 2071 6973 6b69  ython.from qiski
-000013e0: 745f 7379 6d62 2e71 7561 6e74 756d 5f69  t_symb.quantum_i
-000013f0: 6e66 6f20 696d 706f 7274 2053 7461 7465  nfo import State
-00001400: 7665 6374 6f72 0a0a 7376 203d 2053 7461  vector..sv = Sta
-00001410: 7465 7665 6374 6f72 2870 7163 290a 7376  tevector(pqc).sv
-00001420: 5f66 756e 6320 3d20 7376 2e74 6f5f 6c61  _func = sv.to_la
-00001430: 6d62 6461 2829 0a60 6060 0a0a 5765 2063  mbda().```..We c
-00001440: 616e 206e 6f77 2063 616c 6c20 7468 6520  an now call the 
-00001450: 6765 6e65 7261 7465 6420 6c61 6d62 6461  generated lambda
-00001460: 2066 756e 6374 696f 6e20 7061 7373 696e   function passin
-00001470: 6720 7468 6520 6163 7475 616c 2076 616c  g the actual val
-00001480: 7565 7320 7765 2077 616e 7420 746f 2061  ues we want to a
-00001490: 7373 6967 6e20 746f 2065 6163 6820 6672  ssign to each fr
-000014a0: 6565 2070 6172 616d 6574 6572 2028 696e  ee parameter (in
-000014b0: 2061 6c70 6861 6265 7469 6361 6c20 6f72   alphabetical or
-000014c0: 6465 722c 2073 616d 6520 636f 6e76 656e  der, same conven
-000014d0: 7469 6f6e 2075 7365 6420 696e 2060 7169  tion used in `qi
-000014e0: 736b 6974 2d74 6572 7261 6029 2e20 5468  skit-terra`). Th
-000014f0: 6520 7265 7475 726e 6564 206f 626a 6563  e returned objec
-00001500: 7420 7769 6c6c 2062 6520 6120 2a6e 756d  t will be a *num
-00001510: 7079 2a20 3244 2d61 7272 6179 2028 7769  py* 2D-array (wi
-00001520: 7468 2060 7368 6170 653d 2838 2c31 2960  th `shape=(8,1)`
-00001530: 2069 6e20 7468 6973 2063 6173 6529 2072   in this case) r
-00001540: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
-00001550: 6669 6e61 6c20 6f75 7470 7574 2073 7461  final output sta
-00001560: 7465 7665 6374 6f72 2e0a 6060 6070 7974  tevector..```pyt
-00001570: 686f 6e0a 7661 6c75 6573 203d 205b 312e  hon.values = [1.
-00001580: 3234 2c20 322e 3237 2c20 302e 3239 5d0a  24, 2.27, 0.29].
-00001590: 7374 6174 6576 6563 203d 2073 765f 6675  statevec = sv_fu
-000015a0: 6e63 282a 7661 6c75 6573 290a 6060 600a  nc(*values).```.
-000015b0: 0a2a 2a5f 5245 4d41 524b 5f2a 2a20 5c0a  .**_REMARK_** \.
-000015c0: 2a57 6865 6e20 7468 6520 5051 4320 6861  *When the PQC ha
-000015d0: 7320 746f 2062 6520 6576 616c 7561 7465  s to be evaluate
-000015e0: 6420 6f6e 2061 206c 6172 6765 206e 756d  d on a large num
-000015f0: 6265 7220 6f66 2064 6966 6665 7265 6e74  ber of different
-00001600: 2073 6574 7320 6f66 2070 6172 616d 6574   sets of paramet
-00001610: 6572 7320 7661 6c75 6573 2028 7479 7069  ers values (typi
-00001620: 6361 6c20 6361 7365 2069 6e20 514d 4c29  cal case in QML)
-00001630: 2c20 7468 6973 2060 7169 736b 6974 2d73  , this `qiskit-s
-00001640: 796d 6260 2066 6561 7475 7265 2063 616e  ymb` feature can
-00001650: 2068 656c 7020 746f 2073 6967 6e69 6669   help to signifi
-00001660: 6361 6e74 6c79 2069 6d70 726f 7665 2074  cantly improve t
-00001670: 6865 2028 6675 6c6c 2d73 7461 7465 7665  he (full-stateve
-00001680: 6374 6f72 2920 7369 6d75 6c61 7469 6f6e  ctor) simulation
-00001690: 2070 6572 666f 726d 6163 652e 2049 6e64   performace. Ind
-000016a0: 6565 642c 2074 6865 2073 796d 626f 6c69  eed, the symboli
-000016b0: 6320 6576 616c 7574 6174 696f 6e20 6f66  c evalutation of
-000016c0: 2074 6865 2063 6972 6375 6974 2061 6e64   the circuit and
-000016d0: 2074 6865 206c 616d 6264 6120 6765 6e65   the lambda gene
-000016e0: 7261 7469 6f6e 2074 616b 6520 706c 6163  ration take plac
-000016f0: 6520 6f6e 6c79 206f 6e63 653b 2074 6865  e only once; the
-00001700: 6e2c 2074 6865 2073 696d 756c 6174 696f  n, the simulatio
-00001710: 6e20 6f6e 6c79 2063 6f6e 7369 7374 7320  n only consists 
-00001720: 696e 2065 7865 6375 7469 6e67 206d 756c  in executing mul
-00001730: 7469 706c 6520 7469 6d65 7320 7468 6520  tiple times the 
-00001740: 7265 7475 726e 6564 2066 756e 6374 696f  returned functio
-00001750: 6e20 7061 7373 696e 6720 6120 6469 6666  n passing a diff
-00001760: 6572 656e 7420 7365 7420 6f66 2070 6172  erent set of par
-00001770: 616d 6574 6572 7320 7661 6c75 6573 2066  ameters values f
-00001780: 6f72 2065 6163 6820 6974 6572 6174 696f  or each iteratio
-00001790: 6e2e 2046 6f72 2072 656c 6174 6976 656c  n. For relativel
-000017a0: 7920 7368 616c 6c6f 7720 5051 4373 2077  y shallow PQCs w
-000017b0: 6974 6820 6120 6c69 6d69 6c74 6564 206e  ith a limilted n
-000017c0: 756d 6265 7220 6f66 2071 7562 6974 7320  umber of qubits 
-000017d0: 2865 2e67 2e20 5175 616e 7475 6d20 4b65  (e.g. Quantum Ke
-000017e0: 726e 656c 7320 6576 616c 7561 7469 6f6e  rnels evaluation
-000017f0: 292c 2074 6869 7320 6361 6e20 7265 6475  ), this can redu
-00001800: 6365 2074 6865 2065 7865 6375 7469 6f6e  ce the execution
-00001810: 2074 696d 6520 7570 2074 6f20 7477 6f20   time up to two 
-00001820: 6f72 6465 7220 6f66 206d 6167 6e69 7475  order of magnitu
-00001830: 6465 7320 2864 6570 656e 6469 6e67 206f  des (depending o
-00001840: 6e20 7468 6520 6e75 6d62 6572 206f 6620  n the number of 
-00001850: 6974 6572 6174 696f 6e73 2920 636f 6d70  iterations) comp
-00001860: 6172 6564 2074 6f20 7468 6520 7374 616e  ared to the stan
-00001870: 6461 7264 2051 6973 6b69 7420 7369 6d75  dard Qiskit simu
-00001880: 6c61 7469 6f6e 2062 6173 6564 206f 6e20  lation based on 
-00001890: 7468 6520 5b41 6572 2053 696d 756c 6174  the [Aer Simulat
-000018a0: 6f72 735d 2868 7474 7073 3a2f 2f71 6973  ors](https://qis
-000018b0: 6b69 742e 6f72 672f 646f 6375 6d65 6e74  kit.org/document
-000018c0: 6174 696f 6e2f 7475 746f 7269 616c 732f  ation/tutorials/
-000018d0: 7369 6d75 6c61 746f 7273 2f31 5f61 6572  simulators/1_aer
-000018e0: 5f70 726f 7669 6465 722e 6874 6d6c 2920  _provider.html) 
-000018f0: 6f72 2074 6865 205b 5361 6d70 6c65 725d  or the [Sampler]
-00001900: 2868 7474 7073 3a2f 2f71 6973 6b69 742e  (https://qiskit.
-00001910: 6f72 672f 646f 6375 6d65 6e74 6174 696f  org/documentatio
-00001920: 6e2f 7374 7562 732f 7169 736b 6974 2e70  n/stubs/qiskit.p
-00001930: 7269 6d69 7469 7665 732e 5361 6d70 6c65  rimitives.Sample
-00001940: 722e 6874 6d6c 2920 7072 696d 6974 6976  r.html) primitiv
-00001950: 652e 2a0a 0a0a 2320 436f 6e74 7269 6275  e.*...# Contribu
-00001960: 746f 7273 0a0a 3c74 6162 6c65 3e0a 2020  tors..<table>.  
-00001970: 3c74 723e 0a20 2020 203c 7464 2061 6c69  <tr>.    <td ali
-00001980: 676e 3d22 6365 6e74 6572 223e 3c61 2068  gn="center"><a h
-00001990: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-000019a0: 6875 622e 636f 6d2f 5369 6d6f 6e65 4761  hub.com/SimoneGa
-000019b0: 7370 6572 696e 6922 3e3c 696d 6720 7372  sperini"><img sr
-000019c0: 633d 2268 7474 7073 3a2f 2f61 7661 7461  c="https://avata
-000019d0: 7273 322e 6769 7468 7562 7573 6572 636f  rs2.githubuserco
-000019e0: 6e74 656e 742e 636f 6d2f 752f 3731 3038  ntent.com/u/7108
-000019f0: 3637 3538 3f73 3d34 3030 2676 3d34 2220  6758?s=400&v=4" 
-00001a00: 7769 6474 683d 2231 3230 7078 3b22 2f3e  width="120px;"/>
-00001a10: 3c62 722f 3e3c 623e 5369 6d6f 6e65 2047  <br/><b>Simone G
-00001a20: 6173 7065 7269 6e69 3c2f 623e 3c2f 613e  asperini</b></a>
-00001a30: 3c2f 7464 3e0a 2020 3c2f 7472 3e0a 3c2f  </td>.  </tr>.</
-00001a40: 7461 626c 653e 0a                        table>.
+00000000: 215b 5d28 2f69 6d67 2f6c 6f67 6f2e 706e  ![](/img/logo.pn
+00000010: 6729 0a0a 3c70 2061 6c69 676e 3d22 6365  g)..<p align="ce
+00000020: 6e74 6572 223e 0a20 2020 203c 696d 6720  nter">.    <img 
+00000030: 7469 746c 653d 226c 6963 656e 7365 2220  title="license" 
+00000040: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000050: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000060: 652f 6c69 6365 6e73 652d 4170 6163 6865  e/license-Apache
+00000070: 5f32 2e30 2d62 6c75 652e 7376 6722 3e0a  _2.0-blue.svg">.
+00000080: 2020 2020 3c69 6d67 2074 6974 6c65 3d22      <img title="
+00000090: 7079 7468 6f6e 2220 7372 633d 2268 7474  python" src="htt
+000000a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000000b0: 2e69 6f2f 6261 6467 652f 7079 7468 6f6e  .io/badge/python
+000000c0: 2de2 89a5 332e 382d 626c 7565 2e73 7667  -...3.8-blue.svg
+000000d0: 223e 0a20 2020 203c 6120 6872 6566 3d22  ">.    <a href="
+000000e0: 6874 7470 733a 2f2f 7169 736b 6974 2e6f  https://qiskit.o
+000000f0: 7267 2f65 636f 7379 7374 656d 2f22 2061  rg/ecosystem/" a
+00000100: 6c74 3d22 4563 6f73 7973 7465 6d22 3e0a  lt="Ecosystem">.
+00000110: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000120: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000130: 6965 6c64 732e 696f 2f62 6164 6765 2f51  ields.io/badge/Q
+00000140: 6973 6b69 742d 4563 6f73 7973 7465 6d2d  iskit-Ecosystem-
+00000150: 626c 7565 7669 6f6c 6574 2e73 7667 2220  blueviolet.svg" 
+00000160: 2f3e 3c2f 613e 0a3c 2f70 3e0a 0a3c 7020  /></a>.</p>..<p 
+00000170: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000180: 2020 2020 3c69 6d67 2074 6974 6c65 3d22      <img title="
+00000190: 6275 696c 6422 2073 7263 3d27 6874 7470  build" src='http
+000001a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
+000001b0: 696d 6f6e 6547 6173 7065 7269 6e69 2f71  imoneGasperini/q
+000001c0: 6973 6b69 742d 7379 6d62 2f61 6374 696f  iskit-symb/actio
+000001d0: 6e73 2f77 6f72 6b66 6c6f 7773 2f70 7974  ns/workflows/pyt
+000001e0: 686f 6e2d 7061 636b 6167 652e 796d 6c2f  hon-package.yml/
+000001f0: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
+00000200: 3d6d 6173 7465 7227 3e0a 2020 2020 3c69  =master'>.    <i
+00000210: 6d67 2074 6974 6c65 3d22 636f 7665 7261  mg title="covera
+00000220: 6765 2220 7372 633d 2768 7474 7073 3a2f  ge" src='https:/
+00000230: 2f63 6f76 6572 616c 6c73 2e69 6f2f 7265  /coveralls.io/re
+00000240: 706f 732f 6769 7468 7562 2f53 696d 6f6e  pos/github/Simon
+00000250: 6547 6173 7065 7269 6e69 2f71 6973 6b69  eGasperini/qiski
+00000260: 742d 7379 6d62 2f62 6164 6765 2e73 7667  t-symb/badge.svg
+00000270: 3f62 7261 6e63 683d 6d61 7374 6572 273e  ?branch=master'>
+00000280: 0a3c 2f70 3e0a 0a2a 2a2a 0a54 6869 7320  .</p>..***.This 
+00000290: 7061 636b 6167 6520 7761 7320 7072 6573  package was pres
+000002a0: 656e 7465 6420 6174 205b 5169 736b 6974  ented at [Qiskit
+000002b0: 2044 656d 6f44 6179 735d 2868 7474 7073   DemoDays](https
+000002c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5169  ://github.com/Qi
+000002d0: 736b 6974 2f66 6565 6462 6163 6b2f 7769  skit/feedback/wi
+000002e0: 6b69 2f51 6973 6b69 742d 4465 6d6f 4461  ki/Qiskit-DemoDa
+000002f0: 7973 2920 6f6e 204a 756e 6520 3135 7468  ys) on June 15th
+00000300: 2032 3032 3320 245c 7269 6768 7461 7272   2023 $\rightarr
+00000310: 6f77 2420 5b57 6562 6578 2072 6563 6f72  ow$ [Webex recor
+00000320: 6469 6e67 5d28 6874 7470 733a 2f2f 6962  ding](https://ib
+00000330: 6d2e 7765 6265 782e 636f 6d2f 7265 636f  m.webex.com/reco
+00000340: 7264 696e 6773 6572 7669 6365 2f73 6974  rdingservice/sit
+00000350: 6573 2f69 626d 2f72 6563 6f72 6469 6e67  es/ibm/recording
+00000360: 2f70 6c61 7962 6163 6b2f 6336 6439 3666  /playback/c6d96f
+00000370: 3235 6564 6261 3130 3362 6237 6436 3030  25edba103bb7d600
+00000380: 3530 3536 3831 3034 3464 2920 2870 6173  505681044d) (pas
+00000390: 7377 6f72 643a 2060 4465 6d6f 6461 7932  sword: `Demoday2
+000003a0: 3032 3330 3631 3560 2920 2b20 5b4a 7570  0230615`) + [Jup
+000003b0: 7974 6572 206e 6f74 6562 6f6f 6b5d 2868  yter notebook](h
+000003c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000003d0: 6d2f 5169 736b 6974 2f66 6565 6462 6163  m/Qiskit/feedbac
+000003e0: 6b2f 626c 6f62 2f6d 6169 6e2f 6465 6d6f  k/blob/main/demo
+000003f0: 2d64 6179 2d6e 6f74 6562 6f6f 6b73 2f32  -day-notebooks/2
+00000400: 3032 332d 3036 2d31 352f 315f 7169 736b  023-06-15/1_qisk
+00000410: 6974 5f73 796d 625f 6465 6d6f 2e69 7079  it_symb_demo.ipy
+00000420: 6e62 290a 2a2a 2a0a 0a23 2054 6162 6c65  nb).***..# Table
+00000430: 206f 6620 636f 6e74 656e 7473 0a2d 205b   of contents.- [
+00000440: 496e 7472 6f64 7563 7469 6f6e 5d28 2369  Introduction](#i
+00000450: 6e74 726f 6475 6374 696f 6e29 0a2d 205b  ntroduction).- [
+00000460: 496e 7374 616c 6c61 7469 6f6e 5d28 2369  Installation](#i
+00000470: 6e73 7461 6c6c 6174 696f 6e29 0a20 2020  nstallation).   
+00000480: 202d 205b 5573 6572 2d6d 6f64 655d 2823   - [User-mode](#
+00000490: 7573 6572 2d6d 6f64 6529 0a20 2020 202d  user-mode).    -
+000004a0: 205b 4465 762d 6d6f 6465 5d28 2364 6576   [Dev-mode](#dev
+000004b0: 2d6d 6f64 6529 0a2d 205b 5573 6167 6520  -mode).- [Usage 
+000004c0: 6578 616d 706c 6573 5d28 2375 7361 6765  examples](#usage
+000004d0: 2d65 7861 6d70 6c65 7329 0a20 2020 202d  -examples).    -
+000004e0: 205b 5f53 796d 7069 6679 5f20 6120 5169   [_Sympify_ a Qi
+000004f0: 736b 6974 2063 6972 6375 6974 5d28 2373  skit circuit](#s
+00000500: 796d 7069 6679 2d61 2d71 6973 6b69 742d  ympify-a-qiskit-
+00000510: 6369 7263 7569 7429 0a20 2020 202d 205b  circuit).    - [
+00000520: 5f4c 616d 6264 6966 795f 2061 2051 6973  _Lambdify_ a Qis
+00000530: 6b69 7420 6369 7263 7569 745d 2823 6c61  kit circuit](#la
+00000540: 6d62 6469 6679 2d61 2d71 6973 6b69 742d  mbdify-a-qiskit-
+00000550: 6369 7263 7569 7429 0a2d 205b 436f 6e74  circuit).- [Cont
+00000560: 7269 6275 746f 7273 5d28 2363 6f6e 7472  ributors](#contr
+00000570: 6962 7574 6f72 7329 0a0a 0a23 2049 6e74  ibutors)...# Int
+00000580: 726f 6475 6374 696f 6e0a 5468 6520 6071  roduction.The `q
+00000590: 6973 6b69 742d 7379 6d62 6020 7061 636b  iskit-symb` pack
+000005a0: 6167 6520 6973 206d 6561 6e74 2074 6f20  age is meant to 
+000005b0: 6265 2061 2050 7974 686f 6e20 746f 6f6c  be a Python tool
+000005c0: 2074 6f20 656e 6162 6c65 2074 6865 2073   to enable the s
+000005d0: 796d 626f 6c69 6320 6576 616c 7561 7469  ymbolic evaluati
+000005e0: 6f6e 206f 6620 7061 7261 6d65 7472 6963  on of parametric
+000005f0: 2071 7561 6e74 756d 2073 7461 7465 7320   quantum states 
+00000600: 616e 6420 6f70 6572 6174 6f72 7320 6465  and operators de
+00000610: 6669 6e65 6420 696e 205b 5169 736b 6974  fined in [Qiskit
+00000620: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000630: 2e63 6f6d 2f51 6973 6b69 742f 7169 736b  .com/Qiskit/qisk
+00000640: 6974 2d74 6572 7261 2920 6279 2070 6172  it-terra) by par
+00000650: 616d 6574 6572 697a 6564 2071 7561 6e74  ameterized quant
+00000660: 756d 2063 6972 6375 6974 732e 0a0a 4120  um circuits...A 
+00000670: 5061 7261 6d65 7465 7269 7a65 6420 5175  Parameterized Qu
+00000680: 616e 7475 6d20 4369 7263 7569 7420 2850  antum Circuit (P
+00000690: 5143 2920 6973 2061 2071 7561 6e74 756d  QC) is a quantum
+000006a0: 2063 6972 6375 6974 2077 6865 7265 2077   circuit where w
+000006b0: 6520 6861 7665 2061 7420 6c65 6173 7420  e have at least 
+000006c0: 6f6e 6520 6672 6565 2070 6172 616d 6574  one free paramet
+000006d0: 6572 2028 652e 672e 2061 2072 6f74 6174  er (e.g. a rotat
+000006e0: 696f 6e20 616e 676c 6520 245c 7468 6574  ion angle $\thet
+000006f0: 6124 292e 2050 5143 7320 6172 6520 7061  a$). PQCs are pa
+00000700: 7274 6963 756c 6172 6c79 2072 656c 6576  rticularly relev
+00000710: 616e 7420 696e 2051 7561 6e74 756d 204d  ant in Quantum M
+00000720: 6163 6869 6e65 204c 6561 726e 696e 6720  achine Learning 
+00000730: 2851 4d4c 2920 6d6f 6465 6c73 2c20 7768  (QML) models, wh
+00000740: 6572 6520 7468 6520 7661 6c75 6573 206f  ere the values o
+00000750: 6620 7468 6573 6520 7061 7261 6d65 7465  f these paramete
+00000760: 7273 2063 616e 2062 6520 6c65 6172 6e65  rs can be learne
+00000770: 6420 6475 7269 6e67 2074 7261 696e 696e  d during trainin
+00000780: 6720 746f 2072 6561 6368 2074 6865 2064  g to reach the d
+00000790: 6573 6972 6564 206f 7574 7075 742e 0a0a  esired output...
+000007a0: 496e 2070 6172 7469 6375 6c61 722c 2060  In particular, `
+000007b0: 7169 736b 6974 2d73 796d 6260 2063 616e  qiskit-symb` can
+000007c0: 2062 6520 7573 6564 2074 6f20 6372 6561   be used to crea
+000007d0: 7465 2061 2073 796d 626f 6c69 6320 7265  te a symbolic re
+000007e0: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
+000007f0: 6120 7061 7261 6d65 7472 6963 2071 7561  a parametric qua
+00000800: 6e74 756d 2073 7461 7465 7665 6374 6f72  ntum statevector
+00000810: 2c20 6465 6e73 6974 7920 6d61 7472 6978  , density matrix
+00000820: 2c20 6f72 2075 6e69 7461 7279 206f 7065  , or unitary ope
+00000830: 7261 746f 7220 6469 7265 6374 6c79 2066  rator directly f
+00000840: 726f 6d20 7468 6520 5169 736b 6974 2071  rom the Qiskit q
+00000850: 7561 6e74 756d 2063 6972 6375 6974 2e20  uantum circuit. 
+00000860: 5468 6973 2068 6173 2062 6565 6e20 6163  This has been ac
+00000870: 6869 6576 6564 2074 6872 6f75 6768 2074  hieved through t
+00000880: 6865 2072 652d 696d 706c 656d 656e 7461  he re-implementa
+00000890: 7469 6f6e 206f 6620 736f 6d65 2062 6173  tion of some bas
+000008a0: 6963 2063 6c61 7373 6573 2064 6566 696e  ic classes defin
+000008b0: 6564 2069 6e20 7468 6520 5b60 7169 736b  ed in the [`qisk
+000008c0: 6974 2f71 7561 6e74 756d 5f69 6e66 6f2f  it/quantum_info/
+000008d0: 605d 2868 7474 7073 3a2f 2f67 6974 6875  `](https://githu
+000008e0: 622e 636f 6d2f 5169 736b 6974 2f71 6973  b.com/Qiskit/qis
+000008f0: 6b69 742d 7465 7272 612f 7472 6565 2f6d  kit-terra/tree/m
+00000900: 6169 6e2f 7169 736b 6974 2f71 7561 6e74  ain/qiskit/quant
+00000910: 756d 5f69 6e66 6f29 206d 6f64 756c 6520  um_info) module 
+00000920: 6279 2075 7369 6e67 205b 7379 6d70 795d  by using [sympy]
+00000930: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000940: 636f 6d2f 7379 6d70 792f 7379 6d70 7929  com/sympy/sympy)
+00000950: 2061 7320 6120 6261 636b 656e 6420 666f   as a backend fo
+00000960: 7220 7379 6d62 6f6c 6963 2065 7870 7265  r symbolic expre
+00000970: 7373 696f 6e73 206d 616e 6970 756c 6174  ssions manipulat
+00000980: 696f 6e2e 0a0a 0a23 2049 6e73 7461 6c6c  ion....# Install
+00000990: 6174 696f 6e0a 0a23 2320 5573 6572 2d6d  ation..## User-m
+000009a0: 6f64 650a 6060 600a 7069 7020 696e 7374  ode.```.pip inst
+000009b0: 616c 6c20 7169 736b 6974 2d73 796d 620a  all qiskit-symb.
+000009c0: 6060 600a 0a23 2320 4465 762d 6d6f 6465  ```..## Dev-mode
+000009d0: 0a60 6060 0a67 6974 2063 6c6f 6e65 2068  .```.git clone h
+000009e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000009f0: 6d2f 5369 6d6f 6e65 4761 7370 6572 696e  m/SimoneGasperin
+00000a00: 692f 7169 736b 6974 2d73 796d 622e 6769  i/qiskit-symb.gi
+00000a10: 740a 6364 2071 6973 6b69 742d 7379 6d62  t.cd qiskit-symb
+00000a20: 0a70 6970 2069 6e73 7461 6c6c 202d 6520  .pip install -e 
+00000a30: 2e0a 6060 600a 0a0a 2320 5573 6167 6520  ..```...# Usage 
+00000a40: 6578 616d 706c 6573 0a0a 2323 2320 5f53  examples..### _S
+00000a50: 796d 7069 6679 5f20 6120 5169 736b 6974  ympify_ a Qiskit
+00000a60: 2063 6972 6375 6974 0a4c 6574 2773 2067   circuit.Let's g
+00000a70: 6574 2073 7461 7274 6564 206f 6e20 686f  et started on ho
+00000a80: 7720 746f 2075 7365 2060 7169 736b 6974  w to use `qiskit
+00000a90: 2d73 796d 6260 2074 6f20 6765 7420 7468  -symb` to get th
+00000aa0: 6520 7379 6d62 6f6c 6963 2072 6570 7265  e symbolic repre
+00000ab0: 7365 6e74 6174 696f 6e20 6f66 2061 2067  sentation of a g
+00000ac0: 6976 656e 2051 6973 6b69 7420 6369 7263  iven Qiskit circ
+00000ad0: 7569 742e 2049 6e20 7061 7274 6963 756c  uit. In particul
+00000ae0: 6172 2c20 696e 2074 6869 7320 6669 7273  ar, in this firs
+00000af0: 7420 6261 7369 6320 6578 616d 706c 652c  t basic example,
+00000b00: 2077 6520 636f 6e73 6964 6572 2074 6865   we consider the
+00000b10: 2066 6f6c 6c6f 7769 6e67 2071 7561 6e74   following quant
+00000b20: 756d 2063 6972 6375 6974 3a0a 6060 6070  um circuit:.```p
+00000b30: 7974 686f 6e0a 6672 6f6d 2071 6973 6b69  ython.from qiski
+00000b40: 7420 696d 706f 7274 2051 7561 6e74 756d  t import Quantum
+00000b50: 4369 7263 7569 740a 6672 6f6d 2071 6973  Circuit.from qis
+00000b60: 6b69 742e 6369 7263 7569 7420 696d 706f  kit.circuit impo
+00000b70: 7274 2050 6172 616d 6574 6572 2c20 5061  rt Parameter, Pa
+00000b80: 7261 6d65 7465 7256 6563 746f 720a 0a79  rameterVector..y
+00000b90: 203d 2050 6172 616d 6574 6572 2827 7927   = Parameter('y'
+00000ba0: 290a 7020 3d20 5061 7261 6d65 7465 7256  ).p = ParameterV
+00000bb0: 6563 746f 7228 2770 272c 206c 656e 6774  ector('p', lengt
+00000bc0: 683d 3229 0a0a 7071 6320 3d20 5175 616e  h=2)..pqc = Quan
+00000bd0: 7475 6d43 6972 6375 6974 2832 290a 7071  tumCircuit(2).pq
+00000be0: 632e 7279 2879 2c20 3029 0a70 7163 2e63  c.ry(y, 0).pqc.c
+00000bf0: 7828 302c 2031 290a 7071 632e 7528 302c  x(0, 1).pqc.u(0,
+00000c00: 202a 702c 2031 290a 0a70 7163 2e64 7261   *p, 1)..pqc.dra
+00000c10: 7728 276d 706c 2729 0a60 6060 0a21 5b5d  w('mpl').```.![]
+00000c20: 282f 696d 672f 6578 616d 706c 655f 6369  (/img/example_ci
+00000c30: 7263 7569 742e 706e 6729 0a0a 546f 2067  rcuit.png)..To g
+00000c40: 6574 2074 6865 202a 7379 6d70 792a 2072  et the *sympy* r
+00000c50: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+00000c60: 2074 6865 2075 6e69 7461 7279 206d 6174   the unitary mat
+00000c70: 7269 7820 636f 7272 6573 706f 6e64 696e  rix correspondin
+00000c80: 6720 746f 2074 6865 2070 6172 616d 6574  g to the paramet
+00000c90: 6572 697a 6564 2063 6972 6375 6974 2c20  erized circuit, 
+00000ca0: 7765 206a 7573 7420 6861 7665 2074 6f20  we just have to 
+00000cb0: 6372 6561 7465 2074 6865 2073 796d 626f  create the symbo
+00000cc0: 6c69 6320 604f 7065 7261 746f 7260 2069  lic `Operator` i
+00000cd0: 6e73 7461 6e63 6520 616e 6420 6361 6c6c  nstance and call
+00000ce0: 2074 6865 2060 746f 5f73 796d 7079 2829   the `to_sympy()
+00000cf0: 6020 6d65 7468 6f64 3a0a 6060 6070 7974  ` method:.```pyt
+00000d00: 686f 6e0a 6672 6f6d 2071 6973 6b69 745f  hon.from qiskit_
+00000d10: 7379 6d62 2e71 7561 6e74 756d 5f69 6e66  symb.quantum_inf
+00000d20: 6f20 696d 706f 7274 204f 7065 7261 746f  o import Operato
+00000d30: 720a 0a6f 7020 3d20 4f70 6572 6174 6f72  r..op = Operator
+00000d40: 2870 7163 290a 6f70 2e74 6f5f 7379 6d70  (pqc).op.to_symp
+00000d50: 7928 290a 6060 600a 6060 606d 6174 680a  y().```.```math.
+00000d60: 5c6c 6566 745b 5c62 6567 696e 7b6d 6174  \left[\begin{mat
+00000d70: 7269 787d 5c63 6f73 7b5c 6c65 6674 285c  rix}\cos{\left(\
+00000d80: 6672 6163 7b79 7d7b 327d 205c 7269 6768  frac{y}{2} \righ
+00000d90: 7429 7d20 2620 2d20 5c73 696e 7b5c 6c65  t)} & - \sin{\le
+00000da0: 6674 285c 6672 6163 7b79 7d7b 327d 205c  ft(\frac{y}{2} \
+00000db0: 7269 6768 7429 7d20 2620 3020 2620 305c  right)} & 0 & 0\
+00000dc0: 5c30 2026 2030 2026 205c 7369 6e7b 5c6c  \0 & 0 & \sin{\l
+00000dd0: 6566 7428 5c66 7261 637b 797d 7b32 7d20  eft(\frac{y}{2} 
+00000de0: 5c72 6967 6874 297d 2026 205c 636f 737b  \right)} & \cos{
+00000df0: 5c6c 6566 7428 5c66 7261 637b 797d 7b32  \left(\frac{y}{2
+00000e00: 7d20 5c72 6967 6874 297d 5c5c 3020 2620  } \right)}\\0 & 
+00000e10: 3020 2620 655e 7b69 205c 6c65 6674 2870  0 & e^{i \left(p
+00000e20: 5b30 5d20 2b20 705b 315d 5c72 6967 6874  [0] + p[1]\right
+00000e30: 297d 205c 636f 737b 5c6c 6566 7428 5c66  )} \cos{\left(\f
+00000e40: 7261 637b 797d 7b32 7d20 5c72 6967 6874  rac{y}{2} \right
+00000e50: 297d 2026 202d 2065 5e7b 6920 5c6c 6566  )} & - e^{i \lef
+00000e60: 7428 705b 305d 202b 2070 5b31 5d5c 7269  t(p[0] + p[1]\ri
+00000e70: 6768 7429 7d20 5c73 696e 7b5c 6c65 6674  ght)} \sin{\left
+00000e80: 285c 6672 6163 7b79 7d7b 327d 205c 7269  (\frac{y}{2} \ri
+00000e90: 6768 7429 7d5c 5c65 5e7b 6920 5c6c 6566  ght)}\\e^{i \lef
+00000ea0: 7428 705b 305d 202b 2070 5b31 5d5c 7269  t(p[0] + p[1]\ri
+00000eb0: 6768 7429 7d20 5c73 696e 7b5c 6c65 6674  ght)} \sin{\left
+00000ec0: 285c 6672 6163 7b79 7d7b 327d 205c 7269  (\frac{y}{2} \ri
+00000ed0: 6768 7429 7d20 2620 655e 7b69 205c 6c65  ght)} & e^{i \le
+00000ee0: 6674 2870 5b30 5d20 2b20 705b 315d 5c72  ft(p[0] + p[1]\r
+00000ef0: 6967 6874 297d 205c 636f 737b 5c6c 6566  ight)} \cos{\lef
+00000f00: 7428 5c66 7261 637b 797d 7b32 7d20 5c72  t(\frac{y}{2} \r
+00000f10: 6967 6874 297d 2026 2030 2026 2030 5c65  ight)} & 0 & 0\e
+00000f20: 6e64 7b6d 6174 7269 787d 5c72 6967 6874  nd{matrix}\right
+00000f30: 5d0a 6060 600a 0a49 6620 796f 7520 7761  ].```..If you wa
+00000f40: 6e74 2074 6865 6e20 746f 2061 7373 6967  nt then to assig
+00000f50: 6e20 6120 7661 6c75 6520 746f 2073 6f6d  n a value to som
+00000f60: 6520 7370 6563 6966 6963 2070 6172 616d  e specific param
+00000f70: 6574 6572 2c20 796f 7520 6361 6e20 7573  eter, you can us
+00000f80: 6520 7468 6520 6073 7562 7328 3c64 6963  e the `subs(<dic
+00000f90: 743e 2960 206d 6574 686f 6420 7061 7373  t>)` method pass
+00000fa0: 696e 6720 6120 6469 6374 696f 6e61 7279  ing a dictionary
+00000fb0: 2074 6861 7420 6d61 7073 2065 6163 6820   that maps each 
+00000fc0: 7061 7261 6d65 7465 7220 746f 2074 6865  parameter to the
+00000fd0: 2064 6573 6972 6564 2063 6f72 7265 7370   desired corresp
+00000fe0: 6f6e 6469 6e67 2076 616c 7565 3a0a 6060  onding value:.``
+00000ff0: 6070 7974 686f 6e0a 6e65 775f 6f70 203d  `python.new_op =
+00001000: 206f 702e 7375 6273 287b 703a 205b 2d31   op.subs({p: [-1
+00001010: 2c20 325d 7d29 0a6e 6577 5f6f 702e 746f  , 2]}).new_op.to
+00001020: 5f73 796d 7079 2829 0a60 6060 0a60 6060  _sympy().```.```
+00001030: 6d61 7468 0a5c 6c65 6674 5b5c 6265 6769  math.\left[\begi
+00001040: 6e7b 6d61 7472 6978 7d5c 636f 737b 5c6c  n{matrix}\cos{\l
+00001050: 6566 7428 5c66 7261 637b 797d 7b32 7d20  eft(\frac{y}{2} 
+00001060: 5c72 6967 6874 297d 2026 202d 205c 7369  \right)} & - \si
+00001070: 6e7b 5c6c 6566 7428 5c66 7261 637b 797d  n{\left(\frac{y}
+00001080: 7b32 7d20 5c72 6967 6874 297d 2026 2030  {2} \right)} & 0
+00001090: 2026 2030 5c5c 3020 2620 3020 2620 5c73   & 0\\0 & 0 & \s
+000010a0: 696e 7b5c 6c65 6674 285c 6672 6163 7b79  in{\left(\frac{y
+000010b0: 7d7b 327d 205c 7269 6768 7429 7d20 2620  }{2} \right)} & 
+000010c0: 5c63 6f73 7b5c 6c65 6674 285c 6672 6163  \cos{\left(\frac
+000010d0: 7b79 7d7b 327d 205c 7269 6768 7429 7d5c  {y}{2} \right)}\
+000010e0: 5c30 2026 2030 2026 2065 5e7b 697d 205c  \0 & 0 & e^{i} \
+000010f0: 636f 737b 5c6c 6566 7428 5c66 7261 637b  cos{\left(\frac{
+00001100: 797d 7b32 7d20 5c72 6967 6874 297d 2026  y}{2} \right)} &
+00001110: 202d 2065 5e7b 697d 205c 7369 6e7b 5c6c   - e^{i} \sin{\l
+00001120: 6566 7428 5c66 7261 637b 797d 7b32 7d20  eft(\frac{y}{2} 
+00001130: 5c72 6967 6874 297d 5c5c 655e 7b69 7d20  \right)}\\e^{i} 
+00001140: 5c73 696e 7b5c 6c65 6674 285c 6672 6163  \sin{\left(\frac
+00001150: 7b79 7d7b 327d 205c 7269 6768 7429 7d20  {y}{2} \right)} 
+00001160: 2620 655e 7b69 7d20 5c63 6f73 7b5c 6c65  & e^{i} \cos{\le
+00001170: 6674 285c 6672 6163 7b79 7d7b 327d 205c  ft(\frac{y}{2} \
+00001180: 7269 6768 7429 7d20 2620 3020 2620 305c  right)} & 0 & 0\
+00001190: 656e 647b 6d61 7472 6978 7d5c 7269 6768  end{matrix}\righ
+000011a0: 745d 0a60 6060 0a0a 2323 2320 5f4c 616d  t].```..### _Lam
+000011b0: 6264 6966 795f 2061 2051 6973 6b69 7420  bdify_ a Qiskit 
+000011c0: 6369 7263 7569 740a 4769 7665 6e20 6120  circuit.Given a 
+000011d0: 5169 736b 6974 2063 6972 6375 6974 2c20  Qiskit circuit, 
+000011e0: 6071 6973 6b69 742d 7379 6d62 6020 616c  `qiskit-symb` al
+000011f0: 736f 2061 6c6c 6f77 7320 746f 2067 656e  so allows to gen
+00001200: 6572 6174 6520 6120 5079 7468 6f6e 206c  erate a Python l
+00001210: 616d 6264 6120 6675 6e63 7469 6f6e 2077  ambda function w
+00001220: 6974 6820 6163 7475 616c 2061 7267 756d  ith actual argum
+00001230: 656e 7473 206d 6174 6368 696e 6720 7468  ents matching th
+00001240: 6520 5169 736b 6974 2075 6e62 6f75 6e64  e Qiskit unbound
+00001250: 2070 6172 616d 6574 6572 732e 0a4c 6574   parameters..Let
+00001260: 2773 2063 6f6e 7369 6465 7220 7468 6520  's consider the 
+00001270: 666f 6c6c 6f77 696e 6720 6578 616d 706c  following exampl
+00001280: 6520 7374 6172 7469 6e67 2066 726f 6d20  e starting from 
+00001290: 6120 605a 5a46 6561 7475 7265 4d61 7060  a `ZZFeatureMap`
+000012a0: 2063 6972 6375 6974 2c20 636f 6d6d 6f6e   circuit, common
+000012b0: 6c79 2075 7365 6420 6173 2061 2064 6174  ly used as a dat
+000012c0: 6120 656d 6265 6464 696e 6720 616e 7361  a embedding ansa
+000012d0: 747a 2069 6e20 514d 4c20 6170 706c 6963  tz in QML applic
+000012e0: 6174 696f 6e73 3a0a 6060 6070 7974 686f  ations:.```pytho
+000012f0: 6e0a 6672 6f6d 2071 6973 6b69 742e 6369  n.from qiskit.ci
+00001300: 7263 7569 742e 6c69 6272 6172 7920 696d  rcuit.library im
+00001310: 706f 7274 205a 5a46 6561 7475 7265 4d61  port ZZFeatureMa
+00001320: 700a 0a70 7163 203d 205a 5a46 6561 7475  p..pqc = ZZFeatu
+00001330: 7265 4d61 7028 6665 6174 7572 655f 6469  reMap(feature_di
+00001340: 6d65 6e73 696f 6e3d 332c 2072 6570 733d  mension=3, reps=
+00001350: 3129 0a70 7163 2e64 7261 7728 276d 706c  1).pqc.draw('mpl
+00001360: 2729 0a60 6060 0a21 5b5d 282f 696d 672f  ').```.![](/img/
+00001370: 7a7a 6665 6174 7572 656d 6170 5f63 6972  zzfeaturemap_cir
+00001380: 6375 6974 2e70 6e67 290a 0a54 6f20 6765  cuit.png)..To ge
+00001390: 7420 7468 6520 5079 7468 6f6e 2066 756e  t the Python fun
+000013a0: 6374 696f 6e20 7265 7072 6573 656e 7469  ction representi
+000013b0: 6e67 2074 6865 2066 696e 616c 2070 6172  ng the final par
+000013c0: 616d 6574 6572 6963 2073 7461 7465 7665  ameteric stateve
+000013d0: 6374 6f72 2c20 7765 206a 7573 7420 6861  ctor, we just ha
+000013e0: 7665 2074 6f20 6372 6561 7465 2074 6865  ve to create the
+000013f0: 2073 796d 626f 6c69 6320 6053 7461 7465   symbolic `State
+00001400: 7665 6374 6f72 6020 696e 7374 616e 6365  vector` instance
+00001410: 2061 6e64 2063 616c 6c20 7468 6520 6074   and call the `t
+00001420: 6f5f 6c61 6d62 6461 2829 6020 6d65 7468  o_lambda()` meth
+00001430: 6f64 3a0a 6060 6070 7974 686f 6e0a 6672  od:.```python.fr
+00001440: 6f6d 2071 6973 6b69 745f 7379 6d62 2e71  om qiskit_symb.q
+00001450: 7561 6e74 756d 5f69 6e66 6f20 696d 706f  uantum_info impo
+00001460: 7274 2053 7461 7465 7665 6374 6f72 0a0a  rt Statevector..
+00001470: 7071 6320 3d20 7071 632e 6465 636f 6d70  pqc = pqc.decomp
+00001480: 6f73 6528 290a 7374 6174 6576 6563 203d  ose().statevec =
+00001490: 2053 7461 7465 7665 6374 6f72 2870 7163   Statevector(pqc
+000014a0: 292e 746f 5f6c 616d 6264 6128 290a 6060  ).to_lambda().``
+000014b0: 600a 0a57 6520 6361 6e20 6e6f 7720 6361  `..We can now ca
+000014c0: 6c6c 2074 6865 206c 616d 6264 612d 6765  ll the lambda-ge
+000014d0: 6e65 7261 7465 6420 6675 6e63 7469 6f6e  nerated function
+000014e0: 2060 7374 6174 6576 6563 6020 7061 7373   `statevec` pass
+000014f0: 696e 6720 7468 6520 6078 6020 7661 6c75  ing the `x` valu
+00001500: 6573 2077 6520 7761 6e74 2074 6f20 6173  es we want to as
+00001510: 7369 676e 2074 6f20 6561 6368 2070 6172  sign to each par
+00001520: 616d 6574 6572 2e20 5468 6520 7265 7475  ameter. The retu
+00001530: 726e 6564 206f 626a 6563 7420 7769 6c6c  rned object will
+00001540: 2062 6520 6120 2a6e 756d 7079 2a20 3244   be a *numpy* 2D
+00001550: 2d61 7272 6179 2028 7769 7468 2060 7368  -array (with `sh
+00001560: 6170 653d 2838 2c31 2960 2069 6e20 7468  ape=(8,1)` in th
+00001570: 6973 2063 6173 6529 2072 6570 7265 7365  is case) represe
+00001580: 6e74 696e 6720 7468 6520 6669 6e61 6c20  nting the final 
+00001590: 6f75 7470 7574 2073 7461 7465 7665 6374  output statevect
+000015a0: 6f72 2060 7073 6960 2e0a 6060 6070 7974  or `psi`..```pyt
+000015b0: 686f 6e0a 7820 3d20 5b31 2e32 342c 2032  hon.x = [1.24, 2
+000015c0: 2e32 372c 2030 2e32 395d 0a70 7369 203d  .27, 0.29].psi =
+000015d0: 2073 7461 7465 7665 6328 2a78 290a 6060   statevec(*x).``
+000015e0: 600a 0a54 6869 7320 6665 6174 7572 6520  `..This feature 
+000015f0: 6361 6e20 6265 2075 7365 6675 6c20 7768  can be useful wh
+00001600: 656e 2c20 6769 7665 6e20 6120 5169 736b  en, given a Qisk
+00001610: 6974 2050 5143 2c20 7765 2077 616e 7420  it PQC, we want 
+00001620: 746f 2072 756e 2069 7420 6d75 6c74 6970  to run it multip
+00001630: 6c65 2074 696d 6573 2077 6974 6820 6469  le times with di
+00001640: 6666 6572 656e 7420 7061 7261 6d65 7465  fferent paramete
+00001650: 7273 2076 616c 7565 732e 2049 6e64 6565  rs values. Indee
+00001660: 642c 2077 6520 6361 6e20 7065 7266 6f72  d, we can perfor
+00001670: 6d20 6120 7369 6e67 6c65 2073 796d 626f  m a single symbo
+00001680: 6c69 6320 6576 616c 7574 6174 696f 6e20  lic evalutation 
+00001690: 616e 6420 7468 656e 2063 616c 6c20 7468  and then call th
+000016a0: 6520 6c61 6d62 6461 2067 656e 6572 6174  e lambda generat
+000016b0: 6564 2066 756e 6374 696f 6e20 6173 206d  ed function as m
+000016c0: 616e 7920 7469 6d65 7320 6173 206e 6565  any times as nee
+000016d0: 6465 642c 2070 6173 7369 6e67 2064 6966  ded, passing dif
+000016e0: 6665 7265 6e74 2076 616c 7565 7320 6f66  ferent values of
+000016f0: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
+00001700: 6174 2065 6163 6820 6974 6572 6174 696f  at each iteratio
+00001710: 6e2e 0a0a 2320 436f 6e74 7269 6275 746f  n...# Contributo
+00001720: 7273 0a0a 3c74 6162 6c65 3e0a 2020 3c74  rs..<table>.  <t
+00001730: 723e 0a20 2020 203c 7464 2061 6c69 676e  r>.    <td align
+00001740: 3d22 6365 6e74 6572 223e 3c61 2068 7265  ="center"><a hre
+00001750: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00001760: 622e 636f 6d2f 5369 6d6f 6e65 4761 7370  b.com/SimoneGasp
+00001770: 6572 696e 6922 3e3c 696d 6720 7372 633d  erini"><img src=
+00001780: 2268 7474 7073 3a2f 2f61 7661 7461 7273  "https://avatars
+00001790: 322e 6769 7468 7562 7573 6572 636f 6e74  2.githubusercont
+000017a0: 656e 742e 636f 6d2f 752f 3731 3038 3637  ent.com/u/710867
+000017b0: 3538 3f73 3d34 3030 2676 3d34 2220 7769  58?s=400&v=4" wi
+000017c0: 6474 683d 2231 3230 7078 3b22 2f3e 3c62  dth="120px;"/><b
+000017d0: 722f 3e3c 623e 5369 6d6f 6e65 2047 6173  r/><b>Simone Gas
+000017e0: 7065 7269 6e69 3c2f 623e 3c2f 613e 3c2f  perini</b></a></
+000017f0: 7464 3e0a 2020 3c2f 7472 3e0a 3c2f 7461  td>.  </tr>.</ta
+00001800: 626c 653e 0a                             ble>.
```

### Comparing `qiskit-symb-0.1.2/src/qiskit_symb.egg-info/SOURCES.txt` & `qiskit-symb-0.1.3/src/qiskit_symb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/tests/test_ctrl_parametric_gates.py` & `qiskit-symb-0.1.3/tests/test_ctrl_parametric_gates.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,47 +105,63 @@
 
 @settings(deadline=None, max_examples=10)
 @given(theta=strategies.floats(**val_range),
        seed=strategies.integers(min_value=0))
 def test_crxx(theta, seed):
     """todo"""
     par = Parameter(name='par')
-    circuit = get_random_controlled(base_gate=RXXGate(par), seed=seed)
+    try:
+        circuit = get_random_controlled(base_gate=RXXGate(par), seed=seed)
+    except TypeError:
+        # https://github.com/Qiskit/qiskit-terra/issues/10311
+        return
     arr1 = Operator(circuit.assign_parameters([theta])).data
     arr2 = symb_Operator(circuit).subs({par: theta}).to_numpy()
     assert numpy.allclose(arr1, arr2)
 
 
 @settings(deadline=None, max_examples=10)
 @given(theta=strategies.floats(**val_range),
        seed=strategies.integers(min_value=0))
 def test_cryy(theta, seed):
     """todo"""
     par = Parameter(name='par')
-    circuit = get_random_controlled(base_gate=RYYGate(par), seed=seed)
+    try:
+        circuit = get_random_controlled(base_gate=RYYGate(par), seed=seed)
+    except TypeError:
+        # https://github.com/Qiskit/qiskit-terra/issues/10311
+        return
     arr1 = Operator(circuit.assign_parameters([theta])).data
     arr2 = symb_Operator(circuit).subs({par: theta}).to_numpy()
     assert numpy.allclose(arr1, arr2)
 
 
 @settings(deadline=None, max_examples=10)
 @given(theta=strategies.floats(**val_range),
        seed=strategies.integers(min_value=0))
 def test_crzz(theta, seed):
     """todo"""
     par = Parameter(name='par')
-    circuit = get_random_controlled(base_gate=RZZGate(par), seed=seed)
+    try:
+        circuit = get_random_controlled(base_gate=RZZGate(par), seed=seed)
+    except TypeError:
+        # https://github.com/Qiskit/qiskit-terra/issues/10311
+        return
     arr1 = Operator(circuit.assign_parameters([theta])).data
     arr2 = symb_Operator(circuit).subs({par: theta}).to_numpy()
     assert numpy.allclose(arr1, arr2)
 
 
 @settings(deadline=None, max_examples=10)
 @given(theta=strategies.floats(**val_range),
        seed=strategies.integers(min_value=0))
 def test_crzx(theta, seed):
     """todo"""
     par = Parameter(name='par')
-    circuit = get_random_controlled(base_gate=RZXGate(par), seed=seed)
+    try:
+        circuit = get_random_controlled(base_gate=RZXGate(par), seed=seed)
+    except TypeError:
+        # https://github.com/Qiskit/qiskit-terra/issues/10311
+        return
     arr1 = Operator(circuit.assign_parameters([theta])).data
     arr2 = symb_Operator(circuit).subs({par: theta}).to_numpy()
     assert numpy.allclose(arr1, arr2)
```

### Comparing `qiskit-symb-0.1.2/tests/test_ctrl_standard_gates.py` & `qiskit-symb-0.1.3/tests/test_ctrl_standard_gates.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/tests/test_densitymatrix.py` & `qiskit-symb-0.1.3/tests/test_densitymatrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/tests/test_operator.py` & `qiskit-symb-0.1.3/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/tests/test_parametric_gates.py` & `qiskit-symb-0.1.3/tests/test_parametric_gates.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/tests/test_standard_gates.py` & `qiskit-symb-0.1.3/tests/test_standard_gates.py`

 * *Files identical despite different names*

### Comparing `qiskit-symb-0.1.2/tests/test_statevector.py` & `qiskit-symb-0.1.3/tests/test_statevector.py`

 * *Files identical despite different names*

