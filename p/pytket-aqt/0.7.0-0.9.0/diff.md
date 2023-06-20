# Comparing `tmp/pytket-aqt-0.7.0.tar.gz` & `tmp/pytket-aqt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-aqt-0.7.0.tar", last modified: Wed Apr 28 13:27:57 2021, max compression
+gzip compressed data, was "pytket-aqt-0.9.0.tar", last modified: Tue May 25 17:41:07 2021, max compression
```

## Comparing `pytket-aqt-0.7.0.tar` & `pytket-aqt-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:27:57.356801 pytket-aqt-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-04-28 13:26:53.000000 pytket-aqt-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2021-04-28 13:27:57.356801 pytket-aqt-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      420 2021-04-28 13:26:53.000000 pytket-aqt-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-04-28 13:26:53.000000 pytket-aqt-0.7.0/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:27:57.352801 pytket-aqt-0.7.0/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:27:57.352801 pytket-aqt-0.7.0/pytket/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:27:57.352801 pytket-aqt-0.7.0/pytket/extensions/aqt/
--rw-r--r--   0 runner    (1001) docker     (121)      890 2021-04-28 13:26:53.000000 pytket-aqt-0.7.0/pytket/extensions/aqt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-04-28 13:27:56.000000 pytket-aqt-0.7.0/pytket/extensions/aqt/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:27:57.356801 pytket-aqt-0.7.0/pytket/extensions/aqt/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2021-04-28 13:26:53.000000 pytket-aqt-0.7.0/pytket/extensions/aqt/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11945 2021-04-28 13:26:53.000000 pytket-aqt-0.7.0/pytket/extensions/aqt/backends/aqt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2021-04-28 13:26:53.000000 pytket-aqt-0.7.0/pytket/extensions/aqt/backends/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:27:57.356801 pytket-aqt-0.7.0/pytket_aqt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2021-04-28 13:27:57.000000 pytket-aqt-0.7.0/pytket_aqt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      436 2021-04-28 13:27:57.000000 pytket-aqt-0.7.0/pytket_aqt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-28 13:27:57.000000 pytket-aqt-0.7.0/pytket_aqt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-28 13:27:57.000000 pytket-aqt-0.7.0/pytket_aqt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-04-28 13:27:57.000000 pytket-aqt-0.7.0/pytket_aqt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-28 13:27:57.000000 pytket-aqt-0.7.0/pytket_aqt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-28 13:27:57.356801 pytket-aqt-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2045 2021-04-28 13:26:53.000000 pytket-aqt-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 17:41:07.984005 pytket-aqt-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-05-25 17:40:14.000000 pytket-aqt-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1410 2021-05-25 17:41:07.984005 pytket-aqt-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2021-05-25 17:40:14.000000 pytket-aqt-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-05-25 17:40:14.000000 pytket-aqt-0.9.0/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 17:41:07.984005 pytket-aqt-0.9.0/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 17:41:07.984005 pytket-aqt-0.9.0/pytket/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 17:41:07.984005 pytket-aqt-0.9.0/pytket/extensions/aqt/
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2021-05-25 17:40:14.000000 pytket-aqt-0.9.0/pytket/extensions/aqt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-05-25 17:41:07.000000 pytket-aqt-0.9.0/pytket/extensions/aqt/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 17:41:07.984005 pytket-aqt-0.9.0/pytket/extensions/aqt/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2021-05-25 17:40:14.000000 pytket-aqt-0.9.0/pytket/extensions/aqt/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12936 2021-05-25 17:40:14.000000 pytket-aqt-0.9.0/pytket/extensions/aqt/backends/aqt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1385 2021-05-25 17:40:14.000000 pytket-aqt-0.9.0/pytket/extensions/aqt/backends/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 17:41:07.984005 pytket-aqt-0.9.0/pytket_aqt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1410 2021-05-25 17:41:07.000000 pytket-aqt-0.9.0/pytket_aqt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2021-05-25 17:41:07.000000 pytket-aqt-0.9.0/pytket_aqt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-25 17:41:07.000000 pytket-aqt-0.9.0/pytket_aqt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-25 17:41:07.000000 pytket-aqt-0.9.0/pytket_aqt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-05-25 17:41:07.000000 pytket-aqt-0.9.0/pytket_aqt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-05-25 17:41:07.000000 pytket-aqt-0.9.0/pytket_aqt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-25 17:41:07.984005 pytket-aqt-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2045 2021-05-25 17:40:14.000000 pytket-aqt-0.9.0/setup.py
```

### Comparing `pytket-aqt-0.7.0/PKG-INFO` & `pytket-aqt-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-aqt
-Version: 0.7.0
+Version: 0.9.0
 Summary: Extension for pytket, providing access to AQT backends
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Alec Edgington
 Author-email: alec.edgington@cambridgequantum.com
 License: Apache 2
 Description: # pytket-aqt
```

### Comparing `pytket-aqt-0.7.0/pytket/extensions/aqt/__init__.py` & `pytket-aqt-0.9.0/pytket/extensions/aqt/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-aqt-0.7.0/pytket/extensions/aqt/backends/__init__.py` & `pytket-aqt-0.9.0/pytket/extensions/aqt/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-aqt-0.7.0/pytket/extensions/aqt/backends/aqt.py` & `pytket-aqt-0.9.0/pytket/extensions/aqt/backends/aqt.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,28 +31,29 @@
     BasePass,
     SequencePass,
     SynthesiseIBM,
     FullPeepholeOptimise,
     FlattenRegisters,
     RebaseCustom,
     EulerAngleReduction,
-    RemoveRedundancies,
     DecomposeBoxes,
     RenameQubitsPass,
+    SimplifyInitial,
 )
 from pytket.predicates import (  # type: ignore
     GateSetPredicate,
     MaxNQubitsPredicate,
     NoClassicalControlPredicate,
     NoFastFeedforwardPredicate,
     NoMidMeasurePredicate,
     NoSymbolsPredicate,
     Predicate,
 )
 from pytket.routing import FullyConnected  # type: ignore
+from pytket.utils import prepare_circuit
 from pytket.utils.outcomearray import OutcomeArray
 from .config import AQTConfig
 
 AQT_URL_PREFIX = "https://gateway.aqt.eu/marmot/"
 
 AQT_DEVICE_QC = "lint"
 AQT_DEVICE_SIM = "sim"
@@ -89,14 +90,15 @@
 class AQTBackend(Backend):
     """
     Interface to an AQT device or simulator.
     """
 
     _supports_shots = True
     _supports_counts = True
+    _supports_contextual_optimisation = True
     _persistent_handles = True
 
     def __init__(
         self,
         device_name: str = AQT_DEVICE_SIM,
         access_token: Optional[str] = None,
         label: str = "",
@@ -170,34 +172,38 @@
             return SequencePass(
                 [
                     DecomposeBoxes(),
                     SynthesiseIBM(),
                     FlattenRegisters(),
                     RenameQubitsPass(self._qm),
                     _aqt_rebase(),
-                    RemoveRedundancies(),
+                    SimplifyInitial(
+                        allow_classical=False, create_all_qubits=True, xcirc=_xcirc
+                    ),
                     EulerAngleReduction(OpType.Ry, OpType.Rx),
                 ]
             )
         else:
             return SequencePass(
                 [
                     DecomposeBoxes(),
                     FullPeepholeOptimise(),
                     FlattenRegisters(),
                     RenameQubitsPass(self._qm),
                     _aqt_rebase(),
-                    RemoveRedundancies(),
+                    SimplifyInitial(
+                        allow_classical=False, create_all_qubits=True, xcirc=_xcirc
+                    ),
                     EulerAngleReduction(OpType.Ry, OpType.Rx),
                 ]
             )
 
     @property
     def _result_id_type(self) -> _ResultIdTuple:
-        return (str, str)
+        return (str, str, str)
 
     def process_circuits(
         self,
         circuits: Iterable[Circuit],
         n_shots: Optional[int] = None,
         valid_check: bool = True,
         **kwargs: KwargTypes,
@@ -207,21 +213,31 @@
         Supported kwargs: none.
         """
         if n_shots is None or n_shots < 1:
             raise ValueError("Parameter n_shots is required for this backend")
 
         if valid_check:
             self._check_all_circuits(circuits)
+
+        postprocess = kwargs.get("postprocess", False)
+
         handles = []
         for i, c in enumerate(circuits):
-            (aqt_circ, measures) = _translate_aqt(c)
+            if postprocess:
+                c0, ppcirc = prepare_circuit(c, allow_classical=False, xcirc=_xcirc)
+                ppcirc_rep = ppcirc.to_dict()
+            else:
+                c0, ppcirc_rep = c, None
+            (aqt_circ, measures) = _translate_aqt(c0)
             if self._MACHINE_DEBUG:
                 handles.append(
                     ResultHandle(
-                        _DEBUG_HANDLE_PREFIX + str((c.n_qubits, n_shots)), measures
+                        _DEBUG_HANDLE_PREFIX + str((c.n_qubits, n_shots)),
+                        measures,
+                        json.dumps(ppcirc_rep),
                     )
                 )
             else:
                 resp = put(
                     self._url,
                     data={
                         "data": json.dumps(aqt_circ),
@@ -231,41 +247,49 @@
                     },
                     headers=self._header,
                 ).json()
                 if "status" not in resp:
                     raise RuntimeError(resp["message"])
                 if resp["status"] == "error":
                     raise RuntimeError(resp["ERROR"])
-                handles.append(ResultHandle(resp["id"], measures))
+                handles.append(
+                    ResultHandle(resp["id"], measures, json.dumps(ppcirc_rep))
+                )
         for handle in handles:
             self._cache[handle] = dict()
         return handles
 
     def circuit_status(self, handle: ResultHandle) -> CircuitStatus:
         self._check_handle_type(handle)
         jobid = handle[0]
         message = ""
         measure_permutations = json.loads(handle[1])  # type: ignore
+        ppcirc_rep = json.loads(cast(str, handle[2]))
+        ppcirc = Circuit.from_dict(ppcirc_rep) if ppcirc_rep is not None else None
         if self._MACHINE_DEBUG:
             n_qubits, n_shots = literal_eval(jobid[len(_DEBUG_HANDLE_PREFIX) :])  # type: ignore
             empty_ar = OutcomeArray.from_ints([0] * n_shots, n_qubits, big_endian=True)
-            self._cache[handle].update({"result": BackendResult(shots=empty_ar)})
+            self._cache[handle].update(
+                {"result": BackendResult(shots=empty_ar, ppcirc=ppcirc)}
+            )
             statenum = StatusEnum.COMPLETED
         else:
             data = put(self._url, data={"id": jobid}, headers=self._header).json()
             status = data["status"]
             if "ERROR" in data:
                 message = data["ERROR"]
             statenum = _STATUS_MAP.get(status, StatusEnum.ERROR)
             if statenum is StatusEnum.COMPLETED:
                 shots = OutcomeArray.from_ints(
                     data["samples"], data["no_qubits"], big_endian=True
                 )
                 shots = shots.choose_indices(measure_permutations)
-                self._cache[handle].update({"result": BackendResult(shots=shots)})
+                self._cache[handle].update(
+                    {"result": BackendResult(shots=shots, ppcirc=ppcirc)}
+                )
         return CircuitStatus(statenum, message)
 
     def get_result(self, handle: ResultHandle, **kwargs: KwargTypes) -> BackendResult:
         """
         See :py:meth:`pytket.backends.Backend.get_result`.
         Supported kwargs: `timeout`, `wait`.
         """
@@ -325,7 +349,11 @@
     c_cx.Ry(0.5, 0).Rx(-1, 0)
     c_cx.add_phase(-0.25)
 
     # TK1 replacement
     c_tk1 = lambda a, b, c: Circuit(1).Rx(-0.5, 0).Ry(c, 0).Rx(b, 0).Ry(a, 0).Rx(0.5, 0)
 
     return RebaseCustom({OpType.XXPhase}, c_cx, {OpType.Rx, OpType.Ry}, c_tk1)
+
+
+_xcirc = Circuit(1).Rx(1, 0)
+_xcirc.add_phase(0.5)
```

### Comparing `pytket-aqt-0.7.0/pytket/extensions/aqt/backends/config.py` & `pytket-aqt-0.9.0/pytket/extensions/aqt/backends/config.py`

 * *Files identical despite different names*

### Comparing `pytket-aqt-0.7.0/pytket_aqt.egg-info/PKG-INFO` & `pytket-aqt-0.9.0/pytket_aqt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-aqt
-Version: 0.7.0
+Version: 0.9.0
 Summary: Extension for pytket, providing access to AQT backends
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Alec Edgington
 Author-email: alec.edgington@cambridgequantum.com
 License: Apache 2
 Description: # pytket-aqt
```

### Comparing `pytket-aqt-0.7.0/setup.py` & `pytket-aqt-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     url="https://github.com/CQCL/pytket-extensions",
     description="Extension for pytket, providing access to AQT backends",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="Apache 2",
     packages=find_namespace_packages(include=["pytket.*"]),
     include_package_data=True,
-    install_requires=["pytket ~= 0.10.0", "requests ~= 2.22"],
+    install_requires=["pytket ~= 0.11.0", "requests ~= 2.22"],
     classifiers=[
         "Environment :: Console",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: Other/Proprietary License",
         "Operating System :: MacOS :: MacOS X",
```

