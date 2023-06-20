# Comparing `tmp/pytket-qulacs-0.8.0.tar.gz` & `tmp/pytket-qulacs-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-qulacs-0.8.0.tar", last modified: Tue May 25 17:43:51 2021, max compression
+gzip compressed data, was "pytket-qulacs-0.9.0.tar", last modified: Thu Jun 24 14:41:23 2021, max compression
```

## Comparing `pytket-qulacs-0.8.0.tar` & `pytket-qulacs-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 17:43:51.840392 pytket-qulacs-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-05-25 17:40:14.000000 pytket-qulacs-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2021-05-25 17:43:51.840392 pytket-qulacs-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-05-25 17:40:14.000000 pytket-qulacs-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-05-25 17:40:14.000000 pytket-qulacs-0.8.0/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 17:43:51.836392 pytket-qulacs-0.8.0/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 17:43:51.836392 pytket-qulacs-0.8.0/pytket/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 17:43:51.840392 pytket-qulacs-0.8.0/pytket/extensions/qulacs/
--rw-r--r--   0 runner    (1001) docker     (121)      992 2021-05-25 17:40:14.000000 pytket-qulacs-0.8.0/pytket/extensions/qulacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-05-25 17:43:51.000000 pytket-qulacs-0.8.0/pytket/extensions/qulacs/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 17:43:51.840392 pytket-qulacs-0.8.0/pytket/extensions/qulacs/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-05-25 17:40:14.000000 pytket-qulacs-0.8.0/pytket/extensions/qulacs/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7752 2021-05-25 17:40:14.000000 pytket-qulacs-0.8.0/pytket/extensions/qulacs/backends/qulacs_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     3340 2021-05-25 17:40:14.000000 pytket-qulacs-0.8.0/pytket/extensions/qulacs/qulacs_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 17:43:51.840392 pytket-qulacs-0.8.0/pytket_qulacs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2021-05-25 17:43:51.000000 pytket-qulacs-0.8.0/pytket_qulacs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-05-25 17:43:51.000000 pytket-qulacs-0.8.0/pytket_qulacs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-25 17:43:51.000000 pytket-qulacs-0.8.0/pytket_qulacs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-25 17:43:51.000000 pytket-qulacs-0.8.0/pytket_qulacs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-05-25 17:43:51.000000 pytket-qulacs-0.8.0/pytket_qulacs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-05-25 17:43:51.000000 pytket-qulacs-0.8.0/pytket_qulacs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-25 17:43:51.840392 pytket-qulacs-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2045 2021-05-25 17:40:14.000000 pytket-qulacs-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 14:41:23.053958 pytket-qulacs-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-06-24 14:38:26.000000 pytket-qulacs-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1612 2021-06-24 14:41:23.053958 pytket-qulacs-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2021-06-24 14:38:26.000000 pytket-qulacs-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-06-24 14:38:26.000000 pytket-qulacs-0.9.0/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 14:41:23.049957 pytket-qulacs-0.9.0/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 14:41:23.049957 pytket-qulacs-0.9.0/pytket/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 14:41:23.053958 pytket-qulacs-0.9.0/pytket/extensions/qulacs/
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2021-06-24 14:38:26.000000 pytket-qulacs-0.9.0/pytket/extensions/qulacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-06-24 14:41:22.000000 pytket-qulacs-0.9.0/pytket/extensions/qulacs/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 14:41:23.053958 pytket-qulacs-0.9.0/pytket/extensions/qulacs/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-06-24 14:38:26.000000 pytket-qulacs-0.9.0/pytket/extensions/qulacs/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8453 2021-06-24 14:38:26.000000 pytket-qulacs-0.9.0/pytket/extensions/qulacs/backends/qulacs_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3338 2021-06-24 14:38:26.000000 pytket-qulacs-0.9.0/pytket/extensions/qulacs/qulacs_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 14:41:23.053958 pytket-qulacs-0.9.0/pytket_qulacs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1612 2021-06-24 14:41:23.000000 pytket-qulacs-0.9.0/pytket_qulacs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-06-24 14:41:23.000000 pytket-qulacs-0.9.0/pytket_qulacs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 14:41:23.000000 pytket-qulacs-0.9.0/pytket_qulacs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 14:41:23.000000 pytket-qulacs-0.9.0/pytket_qulacs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-06-24 14:41:23.000000 pytket-qulacs-0.9.0/pytket_qulacs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-24 14:41:23.000000 pytket-qulacs-0.9.0/pytket_qulacs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-24 14:41:23.053958 pytket-qulacs-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2045 2021-06-24 14:38:26.000000 pytket-qulacs-0.9.0/setup.py
```

### Comparing `pytket-qulacs-0.8.0/PKG-INFO` & `pytket-qulacs-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-qulacs
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing access to the Qulacs Simulator
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Irfan Khan
 Author-email: irfan.khan@cambridgequantum.com
 License: Apache 2
 Description: # pytket-qulacs
```

### Comparing `pytket-qulacs-0.8.0/README.md` & `pytket-qulacs-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pytket-qulacs-0.8.0/pytket/extensions/qulacs/__init__.py` & `pytket-qulacs-0.9.0/pytket/extensions/qulacs/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-qulacs-0.8.0/pytket/extensions/qulacs/backends/__init__.py` & `pytket-qulacs-0.9.0/pytket/extensions/qulacs/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-qulacs-0.8.0/pytket/extensions/qulacs/backends/qulacs_backend.py` & `pytket-qulacs-0.9.0/pytket/extensions/qulacs/backends/qulacs_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,31 +11,33 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Methods to allow tket circuits to be ran on the Qulacs simulator
 """
 
-from typing import TYPE_CHECKING, Iterable, List, Optional
+from typing import TYPE_CHECKING, List, Optional, Sequence, Union, cast
 from logging import warning
 from uuid import uuid4
 import numpy as np
 from qulacs import Observable, QuantumState  # type: ignore
 from qulacs.observable import create_observable_from_openfermion_text  # type: ignore
 from pytket.backends import (
     Backend,
     CircuitNotRunError,
     CircuitStatus,
     ResultHandle,
     StatusEnum,
 )
 from pytket.backends.backend import KwargTypes
+from pytket.backends.backendinfo import BackendInfo
 from pytket.backends.backendresult import BackendResult
 from pytket.backends.resulthandle import _ResultIdTuple
 from pytket.circuit import Circuit, OpType  # type: ignore
+from pytket.extensions.qulacs._metadata import __extension_version__
 from pytket.passes import (  # type: ignore
     BasePass,
     SynthesiseIBM,
     SequencePass,
     DecomposeBoxes,
     RebaseIBM,
     FullPeepholeOptimise,
@@ -46,14 +48,15 @@
     NoClassicalControlPredicate,
     NoFastFeedforwardPredicate,
     NoMidMeasurePredicate,
     NoSymbolsPredicate,
     DefaultRegisterPredicate,
     Predicate,
 )
+from pytket.routing import Architecture  # type: ignore
 from pytket.utils.operators import QubitPauliOperator
 from pytket.utils.outcomearray import OutcomeArray
 from pytket.extensions.qulacs.qulacs_convert import tk_to_qulacs
 
 _GPU_ENABLED = True
 try:
     from qulacs import QuantumStateGpu
@@ -70,58 +73,66 @@
     Backend for running simulations on the Qulacs simulator
     """
 
     _supports_shots = True
     _supports_counts = True
     _supports_state = True
     _supports_expectation = True
+    _expectation_allows_nonhermitian = False
     _persistent_handles = False
+    _GATE_SET = {
+        OpType.X,
+        OpType.Y,
+        OpType.Z,
+        OpType.H,
+        OpType.S,
+        OpType.Sdg,
+        OpType.T,
+        OpType.Tdg,
+        OpType.Rx,
+        OpType.Ry,
+        OpType.Rz,
+        OpType.CX,
+        OpType.CZ,
+        OpType.SWAP,
+        OpType.U1,
+        OpType.U2,
+        OpType.U3,
+        OpType.Measure,
+        OpType.Barrier,
+    }
 
     def __init__(self) -> None:
         super().__init__()
+        self._backend_info = BackendInfo(
+            type(self).__name__,
+            None,
+            __extension_version__,
+            Architecture([]),
+            self._GATE_SET,
+        )
+
         self._sim = QuantumState
 
     @property
     def _result_id_type(self) -> _ResultIdTuple:
         return (str,)
 
     @property
-    def device(self) -> Optional["Device"]:
+    def backend_info(self) -> Optional["Device"]:
         return None
 
     @property
     def required_predicates(self) -> List[Predicate]:
         return [
             NoClassicalControlPredicate(),
             NoFastFeedforwardPredicate(),
             NoMidMeasurePredicate(),
             NoSymbolsPredicate(),
-            GateSetPredicate(
-                {
-                    OpType.X,
-                    OpType.Y,
-                    OpType.Z,
-                    OpType.H,
-                    OpType.S,
-                    OpType.Sdg,
-                    OpType.T,
-                    OpType.Tdg,
-                    OpType.Rx,
-                    OpType.Ry,
-                    OpType.Rz,
-                    OpType.CX,
-                    OpType.CZ,
-                    OpType.SWAP,
-                    OpType.U1,
-                    OpType.U2,
-                    OpType.U3,
-                    OpType.Measure,
-                    OpType.Barrier,
-                }
-            ),
+            GateSetPredicate(self._GATE_SET),
             DefaultRegisterPredicate(),
         ]
 
     def default_compilation_pass(self, optimisation_level: int = 1) -> BasePass:
         assert optimisation_level in range(3)
         if optimisation_level == 0:
             return SequencePass([DecomposeBoxes(), FlattenRegisters(), RebaseIBM()])
@@ -130,47 +141,54 @@
         else:
             return SequencePass(
                 [DecomposeBoxes(), FlattenRegisters(), FullPeepholeOptimise()]
             )
 
     def process_circuits(
         self,
-        circuits: Iterable[Circuit],
-        n_shots: Optional[int] = None,
+        circuits: Sequence[Circuit],
+        n_shots: Optional[Union[int, Sequence[int]]] = None,
         valid_check: bool = True,
         **kwargs: KwargTypes,
     ) -> List[ResultHandle]:
-        circuit_list = list(circuits)
+        circuits = list(circuits)
+        if hasattr(n_shots, "__iter__"):
+            n_shots_list = list(cast(Sequence[Optional[int]], n_shots))
+            if len(n_shots_list) != len(circuits):
+                raise ValueError("The length of n_shots and circuits must match")
+        else:
+            # convert n_shots to a list
+            n_shots_list = [cast(Optional[int], n_shots)] * len(circuits)
+
         if valid_check:
-            self._check_all_circuits(circuit_list, nomeasure_warn=False)
+            self._check_all_circuits(circuits, nomeasure_warn=False)
 
         handle_list = []
-        for circuit in circuit_list:
+        for circuit, n_shots_circ in zip(circuits, n_shots_list):
             qulacs_state = self._sim(circuit.n_qubits)
             qulacs_state.set_zero_state()
             qulacs_circ = tk_to_qulacs(circuit)
             qulacs_circ.update_quantum_state(qulacs_state)
             state = qulacs_state.get_vector()
             qubits = sorted(circuit.qubits, reverse=True)
             shots = None
             bits = None
-            if n_shots:
-
+            if n_shots_circ is not None:
                 bits2index = list(
                     (com.bits[0], qubits.index(com.qubits[0]))
                     for com in circuit
                     if com.op.type == OpType.Measure
                 )
                 if len(bits2index) == 0:
                     bits = circuit.bits
-                    shots = OutcomeArray.from_ints([0] * n_shots, len(bits))
+                    shots = OutcomeArray.from_ints([0] * n_shots_circ, len(bits))
                 else:
                     bits, choose_indices = zip(*bits2index)
 
-                    samples = qulacs_state.sampling(n_shots)
+                    samples = qulacs_state.sampling(n_shots_circ)
                     shots = OutcomeArray.from_ints(samples, circuit.n_qubits)
                     shots = shots.choose_indices(choose_indices)
             try:
                 phase = float(circuit.phase)
                 coeff = np.exp(phase * np.pi * 1j)
                 state *= coeff
             except TypeError:
@@ -229,8 +247,9 @@
     class QulacsGPUBackend(QulacsBackend):
         """
         Backend for running simulations on the Qulacs GPU simulator
         """
 
         def __init__(self) -> None:
             super().__init__()
+            self._backend_info.name = type(self).__name__
             self._sim = QuantumStateGpu
```

### Comparing `pytket-qulacs-0.8.0/pytket/extensions/qulacs/qulacs_convert.py` & `pytket-qulacs-0.9.0/pytket/extensions/qulacs/qulacs_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 _TWO_QUBIT_GATES = {OpType.CX: gate.CNOT, OpType.CZ: gate.CZ, OpType.SWAP: gate.SWAP}
 
 _IBM_GATES = {OpType.U1: gate.U1, OpType.U2: gate.U2, OpType.U3: gate.U3}
 
 
 def tk_to_qulacs(circuit: Circuit) -> QuantumCircuit:
-    """ Convert a pytket circuit to a qulacs circuit object. """
+    """Convert a pytket circuit to a qulacs circuit object."""
     qulacs_circ = QuantumCircuit(circuit.n_qubits)
     for com in circuit:
         optype = com.op.type
         if optype in _IBM_GATES:
             qulacs_gate = _IBM_GATES[optype]
             index = com.qubits[0].index[0]
```

### Comparing `pytket-qulacs-0.8.0/pytket_qulacs.egg-info/PKG-INFO` & `pytket-qulacs-0.9.0/pytket_qulacs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-qulacs
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing access to the Qulacs Simulator
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Irfan Khan
 Author-email: irfan.khan@cambridgequantum.com
 License: Apache 2
 Description: # pytket-qulacs
```

### Comparing `pytket-qulacs-0.8.0/setup.py` & `pytket-qulacs-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     url="https://github.com/CQCL/pytket-extensions",
     description="Extension for pytket, providing access to the Qulacs Simulator",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="Apache 2",
     packages=find_namespace_packages(include=["pytket.*"]),
     include_package_data=True,
-    install_requires=["pytket ~= 0.11.0", "Qulacs ~= 0.2"],
+    install_requires=["pytket ~= 0.12.0", "Qulacs ~= 0.2"],
     classifiers=[
         "Environment :: Console",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: Other/Proprietary License",
         "Operating System :: MacOS :: MacOS X",
```

