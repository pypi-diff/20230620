# Comparing `tmp/pytket_pennylane-0.8.0-py3-none-any.whl.zip` & `tmp/pytket_pennylane-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10829 bytes, number of entries: 10
--rw-r--r--  2.0 unx      168 b- defN 23-May-10 14:28 pytket/extensions/pennylane/__init__.py
--rw-r--r--  2.0 unx       72 b- defN 23-May-10 14:28 pytket/extensions/pennylane/_metadata.py
--rw-r--r--  2.0 unx     3007 b- defN 23-May-10 14:28 pytket/extensions/pennylane/pennylane_convert.py
--rw-r--r--  2.0 unx     6052 b- defN 23-May-10 14:28 pytket/extensions/pennylane/pytket_device.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-10 14:28 pytket_pennylane-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3868 b- defN 23-May-10 14:28 pytket_pennylane-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-10 14:28 pytket_pennylane-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       83 b- defN 23-May-10 14:28 pytket_pennylane-0.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-May-10 14:28 pytket_pennylane-0.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      931 b- defN 23-May-10 14:28 pytket_pennylane-0.8.0.dist-info/RECORD
-10 files, 25637 bytes uncompressed, 9199 bytes compressed:  64.1%
+Zip file size: 10902 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      171 b- defN 23-Jun-20 16:56 pytket/extensions/pennylane/__init__.py
+-rw-rw-rw-  2.0 fat       74 b- defN 23-Jun-20 16:57 pytket/extensions/pennylane/_metadata.py
+-rw-rw-rw-  2.0 fat     3114 b- defN 23-Jun-20 16:56 pytket/extensions/pennylane/pennylane_convert.py
+-rw-rw-rw-  2.0 fat     6203 b- defN 23-Jun-20 16:56 pytket/extensions/pennylane/pytket_device.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-20 16:57 pytket_pennylane-0.9.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3977 b- defN 23-Jun-20 16:57 pytket_pennylane-0.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-20 16:57 pytket_pennylane-0.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       83 b- defN 23-Jun-20 16:57 pytket_pennylane-0.9.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-20 16:57 pytket_pennylane-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      931 b- defN 23-Jun-20 16:57 pytket_pennylane-0.9.0.dist-info/RECORD
+10 files, 26210 bytes uncompressed, 9272 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: pytket/extensions/pennylane/pennylane_convert.py
 Comment: 
 
 Filename: pytket/extensions/pennylane/pytket_device.py
 Comment: 
 
-Filename: pytket_pennylane-0.8.0.dist-info/LICENSE
+Filename: pytket_pennylane-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_pennylane-0.8.0.dist-info/METADATA
+Filename: pytket_pennylane-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: pytket_pennylane-0.8.0.dist-info/WHEEL
+Filename: pytket_pennylane-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_pennylane-0.8.0.dist-info/entry_points.txt
+Filename: pytket_pennylane-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytket_pennylane-0.8.0.dist-info/top_level.txt
+Filename: pytket_pennylane-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_pennylane-0.8.0.dist-info/RECORD
+Filename: pytket_pennylane-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/extensions/pennylane/__init__.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
-from ._metadata import __extension_version__, __extension_name__  # type: ignore
-from .pytket_device import PytketDevice
-from .pennylane_convert import pennylane_to_tk
+from ._metadata import __extension_version__, __extension_name__  # type: ignore
+from .pytket_device import PytketDevice
+from .pennylane_convert import pennylane_to_tk
```

## pytket/extensions/pennylane/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.8.0"
-__extension_name__ = "pytket-pennylane"
+__extension_version__ = "0.9.0"
+__extension_name__ = "pytket-pennylane"
```

## pytket/extensions/pennylane/pennylane_convert.py

 * *Ordering differences only*

```diff
@@ -1,107 +1,107 @@
-from typing import List, OrderedDict, cast
-from numpy import pi as PI
-from pennylane.operation import Operation  # type: ignore
-from pytket.circuit import OpType, QubitRegister, BitRegister, Circuit  # type: ignore
-
-# TODO add all pennylane operations
-# https://pennylane.readthedocs.io/en/stable/introduction/operations.html
-PYTKET_OPERATION_MAP = {
-    "Hadamard": OpType.H,
-    "PauliX": OpType.X,
-    "PauliY": OpType.Y,
-    "PauliZ": OpType.Z,
-    "S": OpType.S,
-    "T": OpType.T,
-    "RX": OpType.Rx,
-    "RY": OpType.Ry,
-    "RZ": OpType.Rz,
-    "CNOT": OpType.CX,
-    "CY": OpType.CY,
-    "CZ": OpType.CZ,
-    "SWAP": OpType.SWAP,
-    "U1": OpType.U1,
-    "U2": OpType.U2,
-    "U3": OpType.U3,
-    "CRZ": OpType.CRz,
-    "Toffoli": OpType.CCX,
-    "CSWAP": OpType.CSWAP,
-}
-
-PYTKET_OPERATION_INVERSES_MAP = {k + ".inv": v for k, v in PYTKET_OPERATION_MAP.items()}
-OPERATION_MAP = {**PYTKET_OPERATION_MAP, **PYTKET_OPERATION_INVERSES_MAP}
-
-
-def apply_operations(
-    operations: List[Operation], wire_map: OrderedDict, qreg: QubitRegister
-) -> List[Circuit]:
-    """Apply the circuit operations.
-
-    This method serves as an auxiliary method to :meth:`~.PytketDevice.apply`.
-
-    Args:
-        operations (List[pennylane.Operation]): operations to be applied
-
-    Returns:
-        list[Circuit]: a list of tket circuit objects that
-            specify the corresponding operations
-    """
-    circuits = []
-
-    for operation in operations:
-        # Apply the circuit operations
-        device_wires = operation.wires.map(wire_map)
-        par = cast(List[float], operation.parameters)
-        operation = operation.name
-
-        mapped_operation = OPERATION_MAP[operation]
-
-        # self.qubit_unitary_check(operation, par, device_wires)
-
-        qregs = [qreg[i] for i in device_wires.labels]
-
-        invert = operation.endswith(".inv")
-
-        new_c = Circuit()
-        for q in qreg:
-            new_c.add_qubit(q)
-
-        new_c.add_gate(mapped_operation, [p / PI for p in par], qregs)
-        if invert:
-            new_c = new_c.dagger()
-
-        circuits.append(new_c)
-
-    return circuits
-
-
-def pennylane_to_tk(
-    operations: List[Operation],
-    wire_map: OrderedDict,
-    qreg: QubitRegister,
-    creg: BitRegister,
-    measure: bool = False,
-) -> Circuit:
-    """
-    Convert a PennyLane circuit to a pytket circuit
-
-    :param      operations: list of operations
-    :param      wire_map:   mapping of qubits
-    :param      qreg:       target qubit register
-    :param      creg:       target bit register
-    :param      measure:    whether to add measurements
-
-    :returns:   pytket circuit
-    """
-    applied_operations = apply_operations(operations, wire_map, qreg)
-    circ = Circuit("temp")
-    circ.add_q_register(qreg)
-    circ.add_c_register(creg)
-    for circuit in applied_operations:
-        circ.append(circuit)
-
-    if measure:
-        # Add measurements if they are needed
-        for qr, cr in zip(qreg, creg):
-            circ.Measure(qr, cr)
-
-    return circ
+from typing import List, OrderedDict, cast
+from numpy import pi as PI
+from pennylane.operation import Operation  # type: ignore
+from pytket.circuit import OpType, QubitRegister, BitRegister, Circuit  # type: ignore
+
+# TODO add all pennylane operations
+# https://pennylane.readthedocs.io/en/stable/introduction/operations.html
+PYTKET_OPERATION_MAP = {
+    "Hadamard": OpType.H,
+    "PauliX": OpType.X,
+    "PauliY": OpType.Y,
+    "PauliZ": OpType.Z,
+    "S": OpType.S,
+    "T": OpType.T,
+    "RX": OpType.Rx,
+    "RY": OpType.Ry,
+    "RZ": OpType.Rz,
+    "CNOT": OpType.CX,
+    "CY": OpType.CY,
+    "CZ": OpType.CZ,
+    "SWAP": OpType.SWAP,
+    "U1": OpType.U1,
+    "U2": OpType.U2,
+    "U3": OpType.U3,
+    "CRZ": OpType.CRz,
+    "Toffoli": OpType.CCX,
+    "CSWAP": OpType.CSWAP,
+}
+
+PYTKET_OPERATION_INVERSES_MAP = {k + ".inv": v for k, v in PYTKET_OPERATION_MAP.items()}
+OPERATION_MAP = {**PYTKET_OPERATION_MAP, **PYTKET_OPERATION_INVERSES_MAP}
+
+
+def apply_operations(
+    operations: List[Operation], wire_map: OrderedDict, qreg: QubitRegister
+) -> List[Circuit]:
+    """Apply the circuit operations.
+
+    This method serves as an auxiliary method to :meth:`~.PytketDevice.apply`.
+
+    Args:
+        operations (List[pennylane.Operation]): operations to be applied
+
+    Returns:
+        list[Circuit]: a list of tket circuit objects that
+            specify the corresponding operations
+    """
+    circuits = []
+
+    for operation in operations:
+        # Apply the circuit operations
+        device_wires = operation.wires.map(wire_map)
+        par = cast(List[float], operation.parameters)
+        operation = operation.name
+
+        mapped_operation = OPERATION_MAP[operation]
+
+        # self.qubit_unitary_check(operation, par, device_wires)
+
+        qregs = [qreg[i] for i in device_wires.labels]
+
+        invert = operation.endswith(".inv")
+
+        new_c = Circuit()
+        for q in qreg:
+            new_c.add_qubit(q)
+
+        new_c.add_gate(mapped_operation, [p / PI for p in par], qregs)
+        if invert:
+            new_c = new_c.dagger()
+
+        circuits.append(new_c)
+
+    return circuits
+
+
+def pennylane_to_tk(
+    operations: List[Operation],
+    wire_map: OrderedDict,
+    qreg: QubitRegister,
+    creg: BitRegister,
+    measure: bool = False,
+) -> Circuit:
+    """
+    Convert a PennyLane circuit to a pytket circuit
+
+    :param      operations: list of operations
+    :param      wire_map:   mapping of qubits
+    :param      qreg:       target qubit register
+    :param      creg:       target bit register
+    :param      measure:    whether to add measurements
+
+    :returns:   pytket circuit
+    """
+    applied_operations = apply_operations(operations, wire_map, qreg)
+    circ = Circuit("temp")
+    circ.add_q_register(qreg)
+    circ.add_c_register(creg)
+    for circuit in applied_operations:
+        circ.append(circuit)
+
+    if measure:
+        # Add measurements if they are needed
+        for qr, cr in zip(qreg, creg):
+            circ.Measure(qr, cr)
+
+    return circ
```

## pytket/extensions/pennylane/pytket_device.py

 * *Ordering differences only*

```diff
@@ -1,151 +1,151 @@
-from typing import cast, Any, Dict, Iterable, List, Optional, Union
-
-import numpy as np
-from pennylane import QubitDevice  # type: ignore
-from pennylane.operation import Operation  # type: ignore
-from pytket.backends.backend import Backend
-from pytket.backends.backendresult import BackendResult
-from pytket.passes import BasePass  # type: ignore
-
-from pytket.extensions.qiskit import AerStateBackend
-from pytket.extensions.pennylane import __extension_version__
-from pytket.circuit import OpType, Circuit  # type: ignore
-
-from .pennylane_convert import (
-    OPERATION_MAP,
-    pennylane_to_tk,
-)
-
-
-class PytketDevice(QubitDevice):
-    """PytketDevice allows pytket backends and compilation to be used as Pennylane
-    devices."""
-
-    name = "pytket-pennylane plugin"
-    short_name = "pytket.pytketdevice"
-    pennylane_requires = ">=0.14.0"
-    version = "0.14.0"
-    plugin_version = __extension_version__
-    author = "KN"
-
-    _operation_map = OPERATION_MAP
-    operations = set(_operation_map.keys())
-    observables = {"PauliX", "PauliY", "PauliZ", "Identity", "Hadamard"}
-
-    def __init__(
-        self,
-        wires: int,
-        shots: Optional[int] = None,
-        pytket_backend: Backend = AerStateBackend(),
-        optimisation_level: Optional[int] = None,
-        compilation_pass: Optional[BasePass] = None,
-    ):
-        """Construct a device that use a Pytket Backend and compilation to
-        execute circuits.
-
-        :param wires: Number of wires
-        :type wires: int
-        :param shots: Number of shots to use (only relevant for sampling backends),
-            defaults to None
-        :type shots: Optional[int], optional
-        :param pytket_backend: Pytket Backend class to use, defaults to
-            AerStateBackend() to facilitate automated pennylane testing of this backend
-        :type pytket_backend: Backend, optional
-        :param optimisation_level: Backend default compilation optimisation level,
-            ignored if `compilation_pass` is set, defaults to None
-        :type optimisation_level: int, optional
-        :param compilation_pass: Pytket compiler pass with which to compile circuits,
-            defaults to None
-        :type compilation_pass: Optional[BasePass], optional
-        :raises ValueError: If the Backend does not support shots or state results
-        """
-
-        if not (pytket_backend.supports_shots or pytket_backend.supports_state):
-            raise ValueError("pytket Backend must support shots or state.")
-        self.pytket_backend = pytket_backend
-        if compilation_pass is None:
-            if optimisation_level is None:
-                self.compilation_pass = self.pytket_backend.default_compilation_pass()
-            else:
-                self.compilation_pass = self.pytket_backend.default_compilation_pass(
-                    optimisation_level
-                )
-        else:
-            self.compilation_pass = compilation_pass
-        super().__init__(wires=wires, shots=shots)
-
-    def capabilities(self) -> Dict[str, Any]:
-        cap_dic: Dict[str, Any] = super().capabilities().copy()
-        cap_dic.update(
-            {
-                "supports_finite_shots": self.pytket_backend.supports_shots,
-                "returns_state": self.pytket_backend.supports_state,
-                "supports_inverse_operations": True,
-            }
-        )
-        return cap_dic
-
-    def reset(self) -> None:
-        # Reset only internal data, not the options that are determined on
-        # device creation
-        self._circuit = Circuit(name="temp")
-        self._reg = self._circuit.add_q_register("q", self.num_wires)
-        self._creg = self._circuit.add_c_register("c", self.num_wires)
-        self._backres: Optional[BackendResult] = None
-        self._state: Optional[np.ndarray] = None  # statevector of a simulator backend
-        self._samples: Optional[np.ndarray] = None
-        super().reset()
-
-    def apply(
-        self, operations: List[Operation], rotations: Optional[List[Operation]] = None
-    ) -> None:
-        self._circuit = pennylane_to_tk(
-            operations if rotations is None else operations + rotations,
-            self._wire_map,
-            self._reg,
-            self._creg,
-            measure=(not self.pytket_backend.supports_state),
-        )
-        # These operations need to run for all devices
-        compiled_c = self.compile(self._circuit)
-        self.run(compiled_c)
-
-    def compile(self, circuit: Circuit) -> Circuit:
-        compile_c = circuit.copy()
-        self.compilation_pass.apply(compile_c)
-        return compile_c
-
-    def run(self, compiled_c: Circuit) -> None:
-        """Run the compiled circuit, and query the result."""
-        shots = None
-        if self.pytket_backend.supports_shots:
-            shots = self.shots
-            if compiled_c.n_gates_of_type(OpType.Measure) == 0:
-                compiled_c.measure_all()
-        handle = self.pytket_backend.process_circuit(compiled_c, n_shots=shots)
-        self._backres = self.pytket_backend.get_result(handle)
-
-    def analytic_probability(
-        self, wires: Optional[Union[int, Iterable[int]]] = None
-    ) -> np.ndarray:
-        prob = self.marginal_prob(np.abs(self.state) ** 2, wires)
-        return cast(np.ndarray, prob)
-
-    def generate_samples(self) -> np.ndarray:
-        if self.pytket_backend.supports_shots:
-            if self._backres is None:
-                raise RuntimeError("Result does not exist.")
-            self._samples = np.asarray(self._backres.get_shots(self._creg), dtype=int)
-            return self._samples
-        else:
-            return cast(np.ndarray, super().generate_samples())
-
-    @property
-    def state(self) -> np.ndarray:
-        if self.pytket_backend.supports_state:
-            if self._state is None:
-                if self._backres is None:
-                    raise RuntimeError("Result does not exist.")
-                self._state = self._backres.get_state(self._reg)
-            return self._state
-        raise AttributeError("Device does not support state.")
+from typing import cast, Any, Dict, Iterable, List, Optional, Union
+
+import numpy as np
+from pennylane import QubitDevice  # type: ignore
+from pennylane.operation import Operation  # type: ignore
+from pytket.backends.backend import Backend
+from pytket.backends.backendresult import BackendResult
+from pytket.passes import BasePass  # type: ignore
+
+from pytket.extensions.qiskit import AerStateBackend
+from pytket.extensions.pennylane import __extension_version__
+from pytket.circuit import OpType, Circuit  # type: ignore
+
+from .pennylane_convert import (
+    OPERATION_MAP,
+    pennylane_to_tk,
+)
+
+
+class PytketDevice(QubitDevice):
+    """PytketDevice allows pytket backends and compilation to be used as Pennylane
+    devices."""
+
+    name = "pytket-pennylane plugin"
+    short_name = "pytket.pytketdevice"
+    pennylane_requires = ">=0.14.0"
+    version = "0.14.0"
+    plugin_version = __extension_version__
+    author = "KN"
+
+    _operation_map = OPERATION_MAP
+    operations = set(_operation_map.keys())
+    observables = {"PauliX", "PauliY", "PauliZ", "Identity", "Hadamard"}
+
+    def __init__(
+        self,
+        wires: int,
+        shots: Optional[int] = None,
+        pytket_backend: Backend = AerStateBackend(),
+        optimisation_level: Optional[int] = None,
+        compilation_pass: Optional[BasePass] = None,
+    ):
+        """Construct a device that use a Pytket Backend and compilation to
+        execute circuits.
+
+        :param wires: Number of wires
+        :type wires: int
+        :param shots: Number of shots to use (only relevant for sampling backends),
+            defaults to None
+        :type shots: Optional[int], optional
+        :param pytket_backend: Pytket Backend class to use, defaults to
+            AerStateBackend() to facilitate automated pennylane testing of this backend
+        :type pytket_backend: Backend, optional
+        :param optimisation_level: Backend default compilation optimisation level,
+            ignored if `compilation_pass` is set, defaults to None
+        :type optimisation_level: int, optional
+        :param compilation_pass: Pytket compiler pass with which to compile circuits,
+            defaults to None
+        :type compilation_pass: Optional[BasePass], optional
+        :raises ValueError: If the Backend does not support shots or state results
+        """
+
+        if not (pytket_backend.supports_shots or pytket_backend.supports_state):
+            raise ValueError("pytket Backend must support shots or state.")
+        self.pytket_backend = pytket_backend
+        if compilation_pass is None:
+            if optimisation_level is None:
+                self.compilation_pass = self.pytket_backend.default_compilation_pass()
+            else:
+                self.compilation_pass = self.pytket_backend.default_compilation_pass(
+                    optimisation_level
+                )
+        else:
+            self.compilation_pass = compilation_pass
+        super().__init__(wires=wires, shots=shots)
+
+    def capabilities(self) -> Dict[str, Any]:
+        cap_dic: Dict[str, Any] = super().capabilities().copy()
+        cap_dic.update(
+            {
+                "supports_finite_shots": self.pytket_backend.supports_shots,
+                "returns_state": self.pytket_backend.supports_state,
+                "supports_inverse_operations": True,
+            }
+        )
+        return cap_dic
+
+    def reset(self) -> None:
+        # Reset only internal data, not the options that are determined on
+        # device creation
+        self._circuit = Circuit(name="temp")
+        self._reg = self._circuit.add_q_register("q", self.num_wires)
+        self._creg = self._circuit.add_c_register("c", self.num_wires)
+        self._backres: Optional[BackendResult] = None
+        self._state: Optional[np.ndarray] = None  # statevector of a simulator backend
+        self._samples: Optional[np.ndarray] = None
+        super().reset()
+
+    def apply(
+        self, operations: List[Operation], rotations: Optional[List[Operation]] = None
+    ) -> None:
+        self._circuit = pennylane_to_tk(
+            operations if rotations is None else operations + rotations,
+            self._wire_map,
+            self._reg,
+            self._creg,
+            measure=(not self.pytket_backend.supports_state),
+        )
+        # These operations need to run for all devices
+        compiled_c = self.compile(self._circuit)
+        self.run(compiled_c)
+
+    def compile(self, circuit: Circuit) -> Circuit:
+        compile_c = circuit.copy()
+        self.compilation_pass.apply(compile_c)
+        return compile_c
+
+    def run(self, compiled_c: Circuit) -> None:
+        """Run the compiled circuit, and query the result."""
+        shots = None
+        if self.pytket_backend.supports_shots:
+            shots = self.shots
+            if compiled_c.n_gates_of_type(OpType.Measure) == 0:
+                compiled_c.measure_all()
+        handle = self.pytket_backend.process_circuit(compiled_c, n_shots=shots)
+        self._backres = self.pytket_backend.get_result(handle)
+
+    def analytic_probability(
+        self, wires: Optional[Union[int, Iterable[int]]] = None
+    ) -> np.ndarray:
+        prob = self.marginal_prob(np.abs(self.state) ** 2, wires)
+        return cast(np.ndarray, prob)
+
+    def generate_samples(self) -> np.ndarray:
+        if self.pytket_backend.supports_shots:
+            if self._backres is None:
+                raise RuntimeError("Result does not exist.")
+            self._samples = np.asarray(self._backres.get_shots(self._creg), dtype=int)
+            return self._samples
+        else:
+            return cast(np.ndarray, super().generate_samples())
+
+    @property
+    def state(self) -> np.ndarray:
+        if self.pytket_backend.supports_state:
+            if self._state is None:
+                if self._backres is None:
+                    raise RuntimeError("Result does not exist.")
+                self._state = self._backres.get_state(self._reg)
+            return self._state
+        raise AttributeError("Device does not support state.")
```

## Comparing `pytket_pennylane-0.8.0.dist-info/LICENSE` & `pytket_pennylane-0.9.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `pytket_pennylane-0.8.0.dist-info/METADATA` & `pytket_pennylane-0.9.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-Metadata-Version: 2.1
-Name: pytket-pennylane
-Version: 0.8.0
-Summary: Pytket extension and Pennylane plugin.
-Author: KN
-Author-email: seyon.sivarajah@cambridgequantum.com
-License: Apache 2
-Project-URL: Documentation, https://cqcl.github.io/pytket-pennylane/api/index.html
-Project-URL: Source, https://github.com/CQCL/pytket-pennylane
-Project-URL: Tracker, https://github.com/CQCL/pytket-pennylane/issues
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pytket (~=1.15)
-Requires-Dist: pennylane (~=0.30.0)
-Requires-Dist: pytket-qiskit (~=0.32.0)
-
-# pytket-pennylane
-[Pytket](https://cqcl.github.io/pytket) extension and [PennyLane](https://github.com/PennyLaneAI/pennylane) plugin which allows pytket backends and compilation to be used as a PennyLane device.
-
-
-Pytket is a quantum SDK python package which provides state of the art compilation for quantum
-circuits and a unified interface for execution on a number of "backends" (devices and simulators).
-PennyLane is a package for differentiable programming of quantum computer, which also provides a way
-to execute circuits on a variety of "devices". This package allows users to easily leverage the 
-differentiablecircuits of PennyLane combined with the compilation available in Pytket.
-
-The package is available for python 3.9, 3.10 and 3.11, and can be installed by
-cloning and installing from source, or via pip:
-
-```bash
-pip install pytket-pennylane
-```
-
-API documentation is [here](https://cqcl.github.io/pytket-pennylane/api/).
-
-See the PennyLane [documentation](https://pennylane.readthedocs.io) and Pytket [documentation](https://cqcl.github.io/tket/pytket/api/) to get an intro to PennyLane and Pytket.
-
-To use the integration once installed, initialise your pytket backend (in this example, an `AerBackend` which uses Qiskit Aer), and construct a PennyLane `PytketDevice` using this backend:
-
-```python
-import pennylane as qml
-from pytket.extensions.qiskit import AerBackend
-
-# initialise pytket backend
-pytket_backend = AerBackend()
-
-# construct PennyLane device
-dev = qml.device(
-    "pytket.pytketdevice",
-    wires=2,
-    pytket_backend=pytket_backend,
-    shots=1000
-)
-
-# define a PennyLane Qnode with this device
-@qml.qnode(dev)
-def my_quantum_function(x, y):
-    qml.RZ(x, wires=0)
-    qml.RX(y, wires=1)
-    return qml.expval(qml.PauliZ(0) @ qml.PauliZ(1))
-
-# call the node
-print(my_quantum_function(0.1, 0.2))
-
-```
-
-The example above uses the Pytket default compilation pass for the backend, you can change the optimisation
-level of the default backend pass (0, 1 or 2) by setting the `optimisation_level` parameter:
-
-```python
-dev = qml.device(
-    "pytket.pytketdevice",
-    wires=2,
-    pytket_backend=pytket_backend,
-    optimisation_level=2,
-    shots=1000
-)
-```
-
-You can also use any Pytket [compilation pass](https://cqcl.github.io/pytket/manual/manual_compiler.html) using the `compilation_pass` parameter, which is used instead of the default pass:
-
-```python
-from pytket.passes import PauliSimp, SequencePass
-
-# use a Chemistry optimised pass before the backend's default pass
-
-custom_pass = SequencePass([PauliSimp(), pytket_backend.default_compilation_pass()])
-
-dev = qml.device(
-    "pytket.pytketdevice",
-    wires=2,
-    pytket_backend=pytket_backend,
-    compilation_pass=custom_pass,
-    shots=1000
-)
-
-```
+Metadata-Version: 2.1
+Name: pytket-pennylane
+Version: 0.9.0
+Summary: Pytket extension and Pennylane plugin.
+Author: KN
+Author-email: seyon.sivarajah@cambridgequantum.com
+License: Apache 2
+Project-URL: Documentation, https://cqcl.github.io/pytket-pennylane/api/index.html
+Project-URL: Source, https://github.com/CQCL/pytket-pennylane
+Project-URL: Tracker, https://github.com/CQCL/pytket-pennylane/issues
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pytket (~=1.16)
+Requires-Dist: pennylane (~=0.30.0)
+Requires-Dist: pytket-qiskit (~=0.32.0)
+
+# pytket-pennylane
+[Pytket](https://cqcl.github.io/pytket) extension and [PennyLane](https://github.com/PennyLaneAI/pennylane) plugin which allows pytket backends and compilation to be used as a PennyLane device.
+
+
+Pytket is a quantum SDK python package which provides state of the art compilation for quantum
+circuits and a unified interface for execution on a number of "backends" (devices and simulators).
+PennyLane is a package for differentiable programming of quantum computer, which also provides a way
+to execute circuits on a variety of "devices". This package allows users to easily leverage the 
+differentiablecircuits of PennyLane combined with the compilation available in Pytket.
+
+The package is available for python 3.9, 3.10 and 3.11, and can be installed by
+cloning and installing from source, or via pip:
+
+```bash
+pip install pytket-pennylane
+```
+
+API documentation is [here](https://cqcl.github.io/pytket-pennylane/api/).
+
+See the PennyLane [documentation](https://pennylane.readthedocs.io) and Pytket [documentation](https://cqcl.github.io/tket/pytket/api/) to get an intro to PennyLane and Pytket.
+
+To use the integration once installed, initialise your pytket backend (in this example, an `AerBackend` which uses Qiskit Aer), and construct a PennyLane `PytketDevice` using this backend:
+
+```python
+import pennylane as qml
+from pytket.extensions.qiskit import AerBackend
+
+# initialise pytket backend
+pytket_backend = AerBackend()
+
+# construct PennyLane device
+dev = qml.device(
+    "pytket.pytketdevice",
+    wires=2,
+    pytket_backend=pytket_backend,
+    shots=1000
+)
+
+# define a PennyLane Qnode with this device
+@qml.qnode(dev)
+def my_quantum_function(x, y):
+    qml.RZ(x, wires=0)
+    qml.RX(y, wires=1)
+    return qml.expval(qml.PauliZ(0) @ qml.PauliZ(1))
+
+# call the node
+print(my_quantum_function(0.1, 0.2))
+
+```
+
+The example above uses the Pytket default compilation pass for the backend, you can change the optimisation
+level of the default backend pass (0, 1 or 2) by setting the `optimisation_level` parameter:
+
+```python
+dev = qml.device(
+    "pytket.pytketdevice",
+    wires=2,
+    pytket_backend=pytket_backend,
+    optimisation_level=2,
+    shots=1000
+)
+```
+
+You can also use any Pytket [compilation pass](https://cqcl.github.io/pytket/manual/manual_compiler.html) using the `compilation_pass` parameter, which is used instead of the default pass:
+
+```python
+from pytket.passes import PauliSimp, SequencePass
+
+# use a Chemistry optimised pass before the backend's default pass
+
+custom_pass = SequencePass([PauliSimp(), pytket_backend.default_compilation_pass()])
+
+dev = qml.device(
+    "pytket.pytketdevice",
+    wires=2,
+    pytket_backend=pytket_backend,
+    compilation_pass=custom_pass,
+    shots=1000
+)
+
+```
```

## Comparing `pytket_pennylane-0.8.0.dist-info/RECORD` & `pytket_pennylane-0.9.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-pytket/extensions/pennylane/__init__.py,sha256=4cIexBGR7m8_2U2KXWkJT4zTtfc9bPLt62MksSAvWME,168
-pytket/extensions/pennylane/_metadata.py,sha256=Xr8uC51LDvEFVXfaEH-pm6Dz1VqnXmNzSNUWqKPT6OU,72
-pytket/extensions/pennylane/pennylane_convert.py,sha256=3wwmtxMGiWdJ0VzDgQeIelD4lLDfd0mZmwOP0IUybXw,3007
-pytket/extensions/pennylane/pytket_device.py,sha256=ie8DhpxYKRKswj0Mq7Eos0MqfqzrRmedBjligxy6l-g,6052
-pytket_pennylane-0.8.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytket_pennylane-0.8.0.dist-info/METADATA,sha256=oS0ou9FcSF-O7CxcKWWqbXvUdk8FvN2imIxRhr72p30,3868
-pytket_pennylane-0.8.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pytket_pennylane-0.8.0.dist-info/entry_points.txt,sha256=QMxmLaiyW0CkB11ix3y_UssMos9bA3y6PmfwVLFvZM8,83
-pytket_pennylane-0.8.0.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
-pytket_pennylane-0.8.0.dist-info/RECORD,,
+pytket/extensions/pennylane/__init__.py,sha256=hWP8AbLG2q-r_ihFq5KOA_vdg4xlSRC94n13bWdUxRo,171
+pytket/extensions/pennylane/_metadata.py,sha256=K9dluJ3wBf6zjtBTVOcHwLgxC4JGIxdEtysAu8rCrDI,74
+pytket/extensions/pennylane/pennylane_convert.py,sha256=ratJZIdo34lBJMePLJ9apY6h0Ber_XjlAOiMVoZ0jew,3114
+pytket/extensions/pennylane/pytket_device.py,sha256=OmqrdiTj5KzCLvrlEk0CNh-kXMw2k_q6PsayTW1WTX8,6203
+pytket_pennylane-0.9.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+pytket_pennylane-0.9.0.dist-info/METADATA,sha256=L6WGxHrvvEHXYm4F1uQnMWYGgjETnGRLDC4fUUzmV28,3977
+pytket_pennylane-0.9.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pytket_pennylane-0.9.0.dist-info/entry_points.txt,sha256=QMxmLaiyW0CkB11ix3y_UssMos9bA3y6PmfwVLFvZM8,83
+pytket_pennylane-0.9.0.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
+pytket_pennylane-0.9.0.dist-info/RECORD,,
```

