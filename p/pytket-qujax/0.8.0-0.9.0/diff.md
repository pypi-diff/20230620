# Comparing `tmp/pytket_qujax-0.8.0-py3-none-any.whl.zip` & `tmp/pytket_qujax-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12166 bytes, number of entries: 9
--rw-r--r--  2.0 unx      938 b- defN 22-Nov-01 15:26 pytket/extensions/qujax/__init__.py
--rw-r--r--  2.0 unx       68 b- defN 22-Nov-01 15:27 pytket/extensions/qujax/_metadata.py
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-01 15:26 pytket/extensions/qujax/py.typed
--rw-r--r--  2.0 unx    14515 b- defN 22-Nov-01 15:26 pytket/extensions/qujax/qujax_convert.py
--rw-r--r--  2.0 unx    11357 b- defN 22-Nov-01 15:27 pytket_qujax-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4592 b- defN 22-Nov-01 15:27 pytket_qujax-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-01 15:27 pytket_qujax-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 22-Nov-01 15:27 pytket_qujax-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      777 b- defN 22-Nov-01 15:27 pytket_qujax-0.8.0.dist-info/RECORD
-9 files, 32346 bytes uncompressed, 10806 bytes compressed:  66.6%
+Zip file size: 12370 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      938 b- defN 22-Nov-11 15:02 pytket/extensions/qujax/__init__.py
+-rw-r--r--  2.0 unx       68 b- defN 22-Nov-11 15:03 pytket/extensions/qujax/_metadata.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Nov-11 15:02 pytket/extensions/qujax/py.typed
+-rw-r--r--  2.0 unx    15134 b- defN 22-Nov-11 15:02 pytket/extensions/qujax/qujax_convert.py
+-rw-r--r--  2.0 unx    11357 b- defN 22-Nov-11 15:03 pytket_qujax-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4723 b- defN 22-Nov-11 15:03 pytket_qujax-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Nov-11 15:03 pytket_qujax-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 22-Nov-11 15:03 pytket_qujax-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      777 b- defN 22-Nov-11 15:03 pytket_qujax-0.9.0.dist-info/RECORD
+9 files, 33096 bytes uncompressed, 11010 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: pytket/extensions/qujax/py.typed
 Comment: 
 
 Filename: pytket/extensions/qujax/qujax_convert.py
 Comment: 
 
-Filename: pytket_qujax-0.8.0.dist-info/LICENSE
+Filename: pytket_qujax-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_qujax-0.8.0.dist-info/METADATA
+Filename: pytket_qujax-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: pytket_qujax-0.8.0.dist-info/WHEEL
+Filename: pytket_qujax-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_qujax-0.8.0.dist-info/top_level.txt
+Filename: pytket_qujax-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_qujax-0.8.0.dist-info/RECORD
+Filename: pytket_qujax-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/extensions/qujax/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.8.0"
+__extension_version__ = "0.9.0"
 __extension_name__ = "pytket-qujax"
```

## pytket/extensions/qujax/qujax_convert.py

```diff
@@ -192,21 +192,21 @@
         qubit_inds_seq.append(_tk_qubits_to_inds(c.qubits))
         param_inds_seq.append(param_inds)
 
     return gate_name_seq, qubit_inds_seq, param_inds_seq, circuit.n_qubits
 
 
 def tk_to_qujax(
-    circuit: Circuit, symbol_map: Optional[dict] = None
+    circuit: Circuit, symbol_map: Optional[dict] = None, simulator: str = "statetensor"
 ) -> qujax.UnionCallableOptionalArray:
     """
     Converts a pytket circuit into a function that maps circuit parameters
-    to a statetensor. Assumes all circuit gates can be found in ``qujax.gates``
-    The ``symbol_map`` argument controls the interpretation of any symbolic parameters
-    found in ``circuit.free_symbols()``.
+    to a statetensor (or densitytensor). Assumes all circuit gates can be found in
+    ``qujax.gates``. The ``symbol_map`` argument controls the interpretation of any
+    symbolic parameters found in ``circuit.free_symbols()``.
 
     - If ``symbol_map`` is ``None``, circuit.free_symbols() will be ignored.
       Parameterised gates will be determined based on whether they are stored as
       functions (parameterised) or arrays (non-parameterised) in qujax.gates. The order
       of qujax circuit parameters is the same as in circuit.get_commands().
     - If ``symbol_map`` is provided as a ``dict``, assign qujax circuit parameters to
       symbolic parameters in ``circuit.free_symbols()``; the order of qujax circuit
@@ -219,24 +219,37 @@
 
     :param circuit: Circuit to be converted (without any measurement commands).
     :type circuit: pytket.Circuit
     :param symbol_map:
         If ``None``, parameterised gates determined by ``qujax.gates``. \n
         If ``dict``, maps symbolic pytket parameters following the order in this dict.
     :type symbol_map: Optional[dict]
+    :param simulator: string in ('statetensor', 'densitytensor') corresponding to
+        qujax simulator type. Defaults to statetensor.
+    :type simulator: str
     :return: Function which maps parameters (and optional statetensor_in)
         to a statetensor.
         If the circuit has no parameters, the resulting function
         will only take the optional ``statetensor_in`` as an argument.
     :rtype: Callable[[jnp.ndarray, jnp.ndarray = None], jnp.ndarray]
         or Callable[[jnp.ndarray = None], jnp.ndarray]
         if no parameters found in circuit
     """
+    qujax_args = tk_to_qujax_args(circuit, symbol_map)
+    simulator = simulator.lower()
 
-    return qujax.get_params_to_statetensor_func(*tk_to_qujax_args(circuit, symbol_map))
+    if simulator in ("statetensor", "state", "st"):
+        return qujax.get_params_to_statetensor_func(*qujax_args)
+    elif simulator in ("densitytensor", "density", "dt"):
+        return qujax.get_params_to_densitytensor_func(*qujax_args)
+    else:
+        raise TypeError(
+            f"simulator argument '{simulator}' not recognised, try 'statetensor' "
+            f"or 'densitytensor'"
+        )
 
 
 def tk_to_param(circuit: Circuit) -> jnp.ndarray:
     """
     Extract the parameter vector for non-symbolic circuits.
     i.e. an array where each element corresponds to the parameter
     of a parameterised gate found in the circuit
```

## Comparing `pytket_qujax-0.8.0.dist-info/LICENSE` & `pytket_qujax-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytket_qujax-0.8.0.dist-info/METADATA` & `pytket_qujax-0.9.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-qujax
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing access to qujax functions
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://cqcl.github.io/pytket-qujax/api/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-qujax
 Project-URL: Tracker, https://github.com/CQCL/pytket-qujax/issues
@@ -19,15 +19,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytket (~=1.8)
-Requires-Dist: qujax (~=0.2.8)
+Requires-Dist: qujax (~=0.3.0)
 
 # pytket-qujax
 
 This repository contains the pytket-qujax extension, using CQC's
 [pytket](https://cqcl.github.io/tket/pytket/api/index.html) quantum SDK.
 The other pytket extensions can be found [here](https://github.com/CQCL/pytket-extensions)
 
@@ -35,21 +35,21 @@
 with CQC tket, a set of quantum programming tools.
 
 [qujax](https://github.com/CQCL/qujax) is a pure [JAX](https://github.com/google/jax)
 quantum simulator. pytket-qujax is an extension to [pytket](https://cqcl.github.io/tket/pytket/api/index.html)
 that allows [pytket](https://cqcl.github.io/tket/pytket/api/index.html) circuits to
 be converted to [qujax](https://github.com/CQCL/qujax) for fast (classical) simulation and automatic differentiation.
 
-
 Some useful links:
 - [Documentation](https://cqcl.github.io/pytket-qujax/api/index.html)
 - [PyPI](https://pypi.org/project/pytket-qujax/)
 - [qujax](https://github.com/CQCL/qujax)
 - [pytket-qujax example notebook (VQE)](https://github.com/CQCL/pytket/blob/main/examples/pytket-qujax_heisenberg_vqe.ipynb)
 - [pytket-qujax example notebook (QAOA with `symbol_map`)](https://github.com/CQCL/pytket/blob/main/examples/pytket-qujax_qaoa.ipynb)
+- [pytket-qujax example notebook (classifier)](https://github.com/CQCL/pytket/blob/main/examples/pytket-qujax-classification.ipynb)
 - [qujax example notebooks](https://github.com/CQCL/qujax/tree/main/examples)
 
 
 ## Getting started
 
 `pytket-qujax` is available for Python 3.8, 3.9 and 3.10, on Linux, MacOS
 and Windows. To install, run:
```

