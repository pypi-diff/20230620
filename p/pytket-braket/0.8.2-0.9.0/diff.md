# Comparing `tmp/pytket-braket-0.8.2.tar.gz` & `tmp/pytket-braket-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-braket-0.8.2.tar", last modified: Thu Jun 10 12:06:36 2021, max compression
+gzip compressed data, was "pytket-braket-0.9.0.tar", last modified: Thu Jun 24 14:39:35 2021, max compression
```

## Comparing `pytket-braket-0.8.2.tar` & `pytket-braket-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 12:06:36.398331 pytket-braket-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-06-10 12:06:28.000000 pytket-braket-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-06-10 12:06:36.398331 pytket-braket-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      457 2021-06-10 12:06:28.000000 pytket-braket-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-06-10 12:06:28.000000 pytket-braket-0.8.2/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 12:06:36.394331 pytket-braket-0.8.2/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 12:06:36.394331 pytket-braket-0.8.2/pytket/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 12:06:36.394331 pytket-braket-0.8.2/pytket/extensions/braket/
--rw-r--r--   0 runner    (1001) docker     (121)      939 2021-06-10 12:06:28.000000 pytket-braket-0.8.2/pytket/extensions/braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-06-10 12:06:36.000000 pytket-braket-0.8.2/pytket/extensions/braket/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 12:06:36.394331 pytket-braket-0.8.2/pytket/extensions/braket/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      697 2021-06-10 12:06:28.000000 pytket-braket-0.8.2/pytket/extensions/braket/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32994 2021-06-10 12:06:28.000000 pytket-braket-0.8.2/pytket/extensions/braket/backends/braket.py
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2021-06-10 12:06:28.000000 pytket-braket-0.8.2/pytket/extensions/braket/backends/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7575 2021-06-10 12:06:28.000000 pytket-braket-0.8.2/pytket/extensions/braket/braket_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-10 12:06:36.398331 pytket-braket-0.8.2/pytket_braket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-06-10 12:06:36.000000 pytket-braket-0.8.2/pytket_braket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      515 2021-06-10 12:06:36.000000 pytket-braket-0.8.2/pytket_braket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-10 12:06:36.000000 pytket-braket-0.8.2/pytket_braket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-10 12:06:36.000000 pytket-braket-0.8.2/pytket_braket.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-10 12:06:36.000000 pytket-braket-0.8.2/pytket_braket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-10 12:06:36.000000 pytket-braket-0.8.2/pytket_braket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-10 12:06:36.398331 pytket-braket-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2021-06-10 12:06:28.000000 pytket-braket-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 14:39:35.857294 pytket-braket-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-06-24 14:38:26.000000 pytket-braket-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-06-24 14:39:35.857294 pytket-braket-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2021-06-24 14:38:26.000000 pytket-braket-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-06-24 14:38:26.000000 pytket-braket-0.9.0/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 14:39:35.857294 pytket-braket-0.9.0/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 14:39:35.857294 pytket-braket-0.9.0/pytket/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 14:39:35.857294 pytket-braket-0.9.0/pytket/extensions/braket/
+-rw-r--r--   0 runner    (1001) docker     (121)      939 2021-06-24 14:38:26.000000 pytket-braket-0.9.0/pytket/extensions/braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-06-24 14:39:35.000000 pytket-braket-0.9.0/pytket/extensions/braket/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 14:39:35.857294 pytket-braket-0.9.0/pytket/extensions/braket/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2021-06-24 14:38:26.000000 pytket-braket-0.9.0/pytket/extensions/braket/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34467 2021-06-24 14:38:26.000000 pytket-braket-0.9.0/pytket/extensions/braket/backends/braket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2029 2021-06-24 14:38:26.000000 pytket-braket-0.9.0/pytket/extensions/braket/backends/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9135 2021-06-24 14:38:26.000000 pytket-braket-0.9.0/pytket/extensions/braket/braket_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-24 14:39:35.857294 pytket-braket-0.9.0/pytket_braket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-06-24 14:39:35.000000 pytket-braket-0.9.0/pytket_braket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2021-06-24 14:39:35.000000 pytket-braket-0.9.0/pytket_braket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 14:39:35.000000 pytket-braket-0.9.0/pytket_braket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-24 14:39:35.000000 pytket-braket-0.9.0/pytket_braket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-24 14:39:35.000000 pytket-braket-0.9.0/pytket_braket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-06-24 14:39:35.000000 pytket-braket-0.9.0/pytket_braket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-24 14:39:35.857294 pytket-braket-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2066 2021-06-24 14:38:26.000000 pytket-braket-0.9.0/setup.py
```

### Comparing `pytket-braket-0.8.2/PKG-INFO` & `pytket-braket-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-braket
-Version: 0.8.2
+Version: 0.9.0
 Summary: Extension for pytket, providing access to Amazon Braket backends
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Alec Edgington
 Author-email: alec.edgington@cambridgequantum.com
 License: Apache 2
 Description: # pytket-braket
```

### Comparing `pytket-braket-0.8.2/pytket/extensions/braket/__init__.py` & `pytket-braket-0.9.0/pytket/extensions/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-braket-0.8.2/pytket/extensions/braket/backends/__init__.py` & `pytket-braket-0.9.0/pytket/extensions/braket/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-braket-0.8.2/pytket/extensions/braket/backends/braket.py` & `pytket-braket-0.9.0/pytket/extensions/braket/backends/braket.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,30 +13,38 @@
 # limitations under the License.
 
 import json
 from enum import Enum
 import time
 from typing import (
     cast,
+    Any,
+    Callable,
     Dict,
     Iterable,
     List,
     Optional,
+    Sequence,
     Union,
     Tuple,
+    TYPE_CHECKING,
 )
 from uuid import uuid4
 from pytket.backends import Backend, CircuitStatus, ResultHandle, StatusEnum
 from pytket.backends.backend import KwargTypes
+from pytket.backends.backendinfo import BackendInfo
 from pytket.backends.backend_exceptions import CircuitNotRunError
 from pytket.backends.backendresult import BackendResult
 from pytket.backends.resulthandle import _ResultIdTuple
-from pytket.extensions.braket.braket_convert import tk_to_braket
+from pytket.extensions.braket.braket_convert import (
+    tk_to_braket,
+    get_avg_characterisation,
+)
+from pytket.extensions.braket._metadata import __extension_version__
 from pytket.circuit import Circuit, OpType  # type: ignore
-from pytket.device import Device, QubitErrorContainer  # type: ignore
 from pytket.passes import (  # type: ignore
     BasePass,
     CXMappingPass,
     RebaseCustom,
     RemoveRedundancies,
     SequencePass,
     SynthesiseIBM,
@@ -72,14 +80,17 @@
 from braket.device_schema import DeviceActionType  # type: ignore
 from braket.devices import LocalSimulator  # type: ignore
 from braket.tasks.local_quantum_task import LocalQuantumTask  # type: ignore
 import numpy as np
 
 from .config import BraketConfig
 
+if TYPE_CHECKING:
+    from pytket.circuit import Node  # type: ignore
+
 # Known schemas for noise characteristics
 IONQ_SCHEMA = {
     "name": "braket.device_schema.ionq.ionq_provider_properties",
     "version": "1",
 }
 RIGETTI_SCHEMA = {
     "name": "braket.device_schema.rigetti.rigetti_provider_properties",
@@ -181,15 +192,15 @@
 class _DeviceType(str, Enum):
     LOCAL = "LOCAL"
     SIMULATOR = "SIMULATOR"
     QPU = "QPU"
 
 
 class BraketBackend(Backend):
-    """ Interface to Amazon Braket service """
+    """Interface to Amazon Braket service"""
 
     _persistent_handles = True
 
     def __init__(
         self,
         local: bool = False,
         device: Optional[str] = None,
@@ -357,55 +368,81 @@
 
         if connectivity_graph is None:
             arch = FullyConnected(n_qubits)
         else:
             arch = Architecture(
                 [(k, v) for k, l in connectivity_graph.items() for v in l]
             )
+            self._req_preds.append(ConnectivityPredicate(arch))
         if self._device_type == _DeviceType.QPU:
             assert self._characteristics is not None
-            node_errs = {}
-            edge_errs = {}
             schema = self._characteristics["braketSchemaHeader"]
             if schema == IONQ_SCHEMA:
                 fid = self._characteristics["fidelity"]
-                mean_1q_err = 1 - fid["1Q"]["mean"]
-                mean_2q_err = 1 - fid["2Q"]["mean"]
-                err_1q_cont = QubitErrorContainer(self._singleqs)
-                for optype in self._singleqs:
-                    err_1q_cont.add_error((optype, mean_1q_err))
-                err_2q_cont = QubitErrorContainer(self._multiqs)
-                for optype in self._multiqs:
-                    err_2q_cont.add_error((optype, mean_2q_err))
-                for node in arch.nodes:
-                    node_errs[node] = err_1q_cont
-                for coupling in arch.coupling:
-                    edge_errs[coupling] = err_2q_cont
+                get_node_error: Callable[["Node"], float] = lambda n: 1.0 - cast(
+                    float, fid["1Q"]["mean"]
+                )
+                get_readout_error: Callable[["Node"], float] = lambda n: 0.0
+                get_link_error: Callable[
+                    ["Node", "Node"], float
+                ] = lambda n0, n1: 1.0 - cast(float, fid["2Q"]["mean"])
             elif schema == RIGETTI_SCHEMA:
                 specs = self._characteristics["specs"]
                 specs1q, specs2q = specs["1Q"], specs["2Q"]
-                for node in arch.nodes:
-                    nodespecs = specs1q[f"{node.index[0]}"]
-                    err_1q_cont = QubitErrorContainer(self._singleqs)
-                    for optype in self._singleqs:
-                        err_1q_cont.add_error((optype, 1 - nodespecs.get("f1QRB", 1)))
-                    err_1q_cont.add_readout(nodespecs.get("fRO", 1))
-                    node_errs[node] = err_1q_cont
-                for coupling in arch.coupling:
-                    node0, node1 = coupling
-                    n0, n1 = node0.index[0], node1.index[0]
-                    couplingspecs = specs2q[f"{min(n0,n1)}-{max(n0,n1)}"]
-                    err_2q_cont = QubitErrorContainer({OpType.CZ})
-                    err_2q_cont.add_error((OpType.CZ, 1 - couplingspecs.get("fCZ", 1)))
-                    edge_errs[coupling] = err_2q_cont
-            self._tket_device = Device(node_errs, edge_errs, arch)
-            if connectivity_graph is not None:
-                self._req_preds.append(ConnectivityPredicate(self._tket_device))
+                get_node_error = lambda n: 1.0 - cast(
+                    float, specs1q[f"{n.index[0]}"].get("f1QRB", 1.0)
+                )
+                get_readout_error = lambda n: cast(
+                    float, specs1q[f"{n.index[0]}"].get("fRO", 1.0)
+                )
+                get_link_error = lambda n0, n1: 1.0 - cast(
+                    float,
+                    specs2q[
+                        f"{min(n0.index[0],n1.index[0])}-{max(n0.index[0],n1.index[0])}"
+                    ].get("fCZ", 1.0),
+                )
+            # readout error as symmetric 2x2 matrix
+            to_sym_mat: Callable[[float], List[List[float]]] = lambda x: [
+                [1.0 - x, x],
+                [x, 1.0 - x],
+            ]
+            node_errors = {
+                node: {optype: get_node_error(node) for optype in self._singleqs}
+                for node in arch.nodes
+            }
+            readout_errors = {
+                node: to_sym_mat(get_readout_error(node)) for node in arch.nodes
+            }
+            link_errors = {
+                (n0, n1): {optype: get_link_error(n0, n1) for optype in self._multiqs}
+                for n0, n1 in arch.coupling
+            }
+
+            self._backend_info = BackendInfo(
+                type(self).__name__,
+                device,
+                __extension_version__,
+                arch,
+                self._singleqs.union(self._multiqs),
+                misc={
+                    "characterisation": {
+                        "NodeErrors": node_errors,
+                        "EdgeErrors": link_errors,
+                        "ReadoutErrors": readout_errors,
+                    }
+                },
+            )
         else:
-            self._tket_device = None
+            self._backend_info = BackendInfo(
+                type(self).__name__,
+                device,
+                __extension_version__,
+                arch,
+                self._singleqs.union(self._multiqs),
+            )
 
         self._rebase_pass = RebaseCustom(
             self._multiqs,
             Circuit(),
             self._singleqs,
             lambda a, b, c: Circuit(1).Rz(c, 0).Rx(b, 0).Rz(a, 0),
         )
@@ -422,19 +459,22 @@
         assert optimisation_level in range(3)
         passes = [DecomposeBoxes()]
         if optimisation_level == 1:
             passes.append(SynthesiseIBM())
         elif optimisation_level == 2:
             passes.append(FullPeepholeOptimise())
         passes.append(self._rebase_pass)
-        if self._device_type == _DeviceType.QPU:
+        if self._device_type == _DeviceType.QPU and self.characterisation is not None:
+            arch = self.backend_info.architecture
             passes.append(
                 CXMappingPass(
-                    self._tket_device,
-                    NoiseAwarePlacement(self._tket_device),
+                    arch,
+                    NoiseAwarePlacement(
+                        arch, **get_avg_characterisation(self.characterisation)
+                    ),
                     directed_cx=False,
                     delay_measures=True,
                 )
             )
             # If CX weren't supported by the device then we'd need to do another
             # rebase_pass here. But we checked above that it is.
         if optimisation_level == 1:
@@ -471,42 +511,54 @@
         if self._device_type == _DeviceType.QPU:
             return tk_to_braket(circuit, self._all_qubits)
         else:
             return tk_to_braket(circuit)
 
     def process_circuits(
         self,
-        circuits: Iterable[Circuit],
-        n_shots: Optional[int] = None,
+        circuits: Sequence[Circuit],
+        n_shots: Optional[Union[int, Sequence[int]]] = None,
         valid_check: bool = True,
         **kwargs: KwargTypes,
     ) -> List[ResultHandle]:
         """
         Supported `kwargs`: none
         """
+        circuits = list(circuits)
+        n_shots_list: List[int] = []
+        if hasattr(n_shots, "__iter__"):
+            n_shots_list = [n or 0 for n in cast(Sequence[Optional[int]], n_shots)]
+        else:
+            # convert n_shots to a list
+            n_shots_list = [cast(Optional[int], n_shots) or 0] * len(circuits)
+
         if not self.supports_shots and not self.supports_state:
             raise RuntimeError("Backend does not support shots or state")
-        if n_shots is None:
-            n_shots = 0
-        want_state = n_shots == 0
-        if (not want_state) and (
-            n_shots < self._sample_min_shots or n_shots > self._sample_max_shots
+
+        if any(
+            map(
+                lambda n: n > 0
+                and (n < self._sample_min_shots or n > self._sample_max_shots),
+                n_shots_list,
+            )
         ):
             raise ValueError(
                 "For sampling, n_shots must be between "
                 f"{self._sample_min_shots} and {self._sample_max_shots}. "
                 "For statevector simulation, omit this parameter."
             )
+
         if valid_check:
             self._check_all_circuits(circuits, nomeasure_warn=False)
 
         postprocess = kwargs.get("postprocess", False)
 
         handles = []
-        for circ in circuits:
+        for circ, n_shots in zip(circuits, n_shots_list):
+            want_state = n_shots == 0
             if postprocess:
                 circ_measured = circ.copy()
                 circ_measured.measure_all()
                 c0, ppcirc = prepare_circuit(circ_measured, allow_classical=False)
                 ppcirc_rep = ppcirc.to_dict()
             else:
                 c0, ppcirc, ppcirc_rep = circ, None, None
@@ -563,20 +615,21 @@
             return CircuitStatus(StatusEnum.QUEUED)
         elif state == "RUNNING":
             return CircuitStatus(StatusEnum.RUNNING)
         else:
             return CircuitStatus(StatusEnum.ERROR, f"Unrecognized state '{state}'")
 
     @property
-    def characterisation(self) -> Optional[Dict]:
-        return self._characteristics
+    def characterisation(self) -> Optional[Dict[str, Any]]:
+        char = self._backend_info.get_misc("characterisation")
+        return cast(Dict[str, Any], char) if char else None
 
     @property
-    def device(self) -> Optional[Device]:
-        return self._tket_device
+    def backend_info(self) -> BackendInfo:
+        return self._backend_info
 
     def get_result(self, handle: ResultHandle, **kwargs: KwargTypes) -> BackendResult:
         """
         See :py:meth:`pytket.backends.Backend.get_result`.
         Supported kwargs: `timeout` (default none), `wait` (default 1s).
         """
         try:
```

### Comparing `pytket-braket-0.8.2/pytket/extensions/braket/backends/config.py` & `pytket-braket-0.9.0/pytket/extensions/braket/backends/config.py`

 * *Files identical despite different names*

### Comparing `pytket-braket-0.8.2/pytket/extensions/braket/braket_convert.py` & `pytket-braket-0.9.0/pytket/extensions/braket/braket_convert.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,19 +11,33 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Conversion from tket to AQT
 """
 
-from typing import Iterable, Optional
+from typing import (
+    cast,
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+    TYPE_CHECKING,
+)
 from pytket.circuit import Circuit, OpType  # type: ignore
 from braket.circuits import Circuit as BK_Circuit  # type: ignore
 from numpy import pi
 
+if TYPE_CHECKING:
+    from pytket.circuit import Node  # type: ignore
+
 
 def tk_to_braket(tkcirc: Circuit, allqbs: Optional[Iterable[int]] = None) -> BK_Circuit:
     """
     Convert a tket :py:class:`Circuit` to a braket circuit.
 
     `tkcirc` must be a circuit having a single one-dimensional register of qubits.
     If `allqbs` is not provided then it is taken to be the qubit set of `tkcirc`.
@@ -193,7 +207,48 @@
             # (2,1), and zeros elsewhere.
             # They could be decomposed into pytket gates, but it would be better to add
             # the gate types to tket.
             # The "Unitary" type could be represented as a box in the 1q and 2q cases,
             # but not in general.
             raise NotImplementedError(f"Cannot convert {opname} to tket")
     return tkcirc
+
+
+def get_avg_characterisation(
+    characterisation: Dict[str, Any]
+) -> Dict[str, Dict["Node", float]]:
+    """
+    Convert gate-specific characterisation into readout, one- and two-qubit errors
+
+    Used to convert the stored full `characterisation` into an input
+    noise characterisation for NoiseAwarePlacement
+    """
+
+    K = TypeVar("K")
+    V1 = TypeVar("V1")
+    V2 = TypeVar("V2")
+    map_values_t = Callable[[Callable[[V1], V2], Dict[K, V1]], Dict[K, V2]]
+    map_values: map_values_t = lambda f, d: {k: f(v) for k, v in d.items()}
+
+    node_errors = cast(
+        Dict["Node", Dict[OpType, float]], characterisation["NodeErrors"]
+    )
+    link_errors = cast(
+        Dict[Tuple["Node", "Node"], Dict[OpType, float]], characterisation["EdgeErrors"]
+    )
+    readout_errors = cast(
+        Dict["Node", List[List[float]]], characterisation["ReadoutErrors"]
+    )
+
+    avg: Callable[[Dict[Any, float]], float] = lambda xs: sum(xs.values()) / len(xs)
+    avg_mat: Callable[[List[List[float]]], float] = (
+        lambda xs: (xs[0][1] + xs[1][0]) / 2.0
+    )
+    avg_readout_errors = map_values(avg_mat, readout_errors)
+    avg_node_errors = map_values(avg, node_errors)
+    avg_link_errors = map_values(avg, link_errors)
+
+    return {
+        "node_errors": avg_node_errors,
+        "link_errors": avg_link_errors,
+        "readout_errors": avg_readout_errors,
+    }
```

### Comparing `pytket-braket-0.8.2/pytket_braket.egg-info/PKG-INFO` & `pytket-braket-0.9.0/pytket_braket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-braket
-Version: 0.8.2
+Version: 0.9.0
 Summary: Extension for pytket, providing access to Amazon Braket backends
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Alec Edgington
 Author-email: alec.edgington@cambridgequantum.com
 License: Apache 2
 Description: # pytket-braket
```

### Comparing `pytket-braket-0.8.2/pytket_braket.egg-info/SOURCES.txt` & `pytket-braket-0.9.0/pytket_braket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytket-braket-0.8.2/setup.py` & `pytket-braket-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     url="https://github.com/CQCL/pytket-extensions",
     description="Extension for pytket, providing access to Amazon Braket backends",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="Apache 2",
     packages=find_namespace_packages(include=["pytket.*"]),
     include_package_data=True,
-    install_requires=["pytket ~= 0.11.0", "amazon-braket-sdk ~= 1.0"],
+    install_requires=["pytket ~= 0.12.0", "amazon-braket-sdk ~= 1.0"],
     classifiers=[
         "Environment :: Console",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: Other/Proprietary License",
         "Operating System :: MacOS :: MacOS X",
```

