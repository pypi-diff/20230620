# Comparing `tmp/qiskit-qrack-provider-0.6.0.tar.gz` & `tmp/qiskit-qrack-provider-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-qrack-provider-0.6.0.tar", last modified: Tue Jun 20 14:37:55 2023, max compression
+gzip compressed data, was "qiskit-qrack-provider-0.7.0.tar", last modified: Tue Jun 20 19:11:52 2023, max compression
```

## Comparing `qiskit-qrack-provider-0.6.0.tar` & `qiskit-qrack-provider-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2021-05-14 12:44:18.000000 qiskit-qrack-provider-0.6.0/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2691 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1671 2021-12-03 23:15:01.000000 qiskit-qrack-provider-0.6.0/README.md
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/qiskit/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/qiskit/providers/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1135 2021-10-08 01:17:38.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/__init__.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/backends/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      548 2023-06-20 14:23:28.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/backends/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    36810 2023-06-20 14:36:16.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/backends/qasm_simulator.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      914 2021-05-14 12:44:18.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/qrackerror.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1903 2021-10-09 18:55:08.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/qrackjob.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1449 2023-06-20 14:23:28.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/qrackprovider.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      506 2023-06-03 15:42:26.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/version.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2691 2023-06-20 14:37:55.000000 qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      525 2023-06-20 14:37:55.000000 qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-06-20 14:37:55.000000 qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       29 2023-06-20 14:37:55.000000 qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/requires.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        7 2023-06-20 14:37:55.000000 qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1642 2023-06-20 14:37:15.000000 qiskit-qrack-provider-0.6.0/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 19:11:52.508524 qiskit-qrack-provider-0.7.0/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2021-05-14 12:44:18.000000 qiskit-qrack-provider-0.7.0/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2691 2023-06-20 19:11:52.508524 qiskit-qrack-provider-0.7.0/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1671 2021-12-03 23:15:01.000000 qiskit-qrack-provider-0.7.0/README.md
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 19:11:52.508524 qiskit-qrack-provider-0.7.0/qiskit/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 19:11:52.508524 qiskit-qrack-provider-0.7.0/qiskit/providers/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 19:11:52.508524 qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1135 2021-10-08 01:17:38.000000 qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/__init__.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 19:11:52.508524 qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/backends/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      548 2023-06-20 14:23:28.000000 qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/backends/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    37498 2023-06-20 19:01:21.000000 qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/backends/qasm_simulator.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      914 2021-05-14 12:44:18.000000 qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/qrackerror.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1903 2021-10-09 18:55:08.000000 qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/qrackjob.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1449 2023-06-20 14:23:28.000000 qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/qrackprovider.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      506 2023-06-03 15:42:26.000000 qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/version.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 19:11:52.508524 qiskit-qrack-provider-0.7.0/qiskit_qrack_provider.egg-info/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2691 2023-06-20 19:11:52.000000 qiskit-qrack-provider-0.7.0/qiskit_qrack_provider.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      525 2023-06-20 19:11:52.000000 qiskit-qrack-provider-0.7.0/qiskit_qrack_provider.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-06-20 19:11:52.000000 qiskit-qrack-provider-0.7.0/qiskit_qrack_provider.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       29 2023-06-20 19:11:52.000000 qiskit-qrack-provider-0.7.0/qiskit_qrack_provider.egg-info/requires.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        7 2023-06-20 19:11:52.000000 qiskit-qrack-provider-0.7.0/qiskit_qrack_provider.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-06-20 19:11:52.508524 qiskit-qrack-provider-0.7.0/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1642 2023-06-20 19:01:58.000000 qiskit-qrack-provider-0.7.0/setup.py
```

### Comparing `qiskit-qrack-provider-0.6.0/LICENSE` & `qiskit-qrack-provider-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.6.0/PKG-INFO` & `qiskit-qrack-provider-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-qrack-provider
-Version: 0.6.0
+Version: 0.7.0
 Summary: Qiskit Qrack Provider - Qrack High-Performance GPU simulation for Qiskit
 Home-page: https://github.com/vm6502q/qiskit-qrack-provider
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: Apache 2.0
 Keywords: qiskit qrack pyqrack simulator quantum addon backend
 Classifier: Environment :: Console
```

### Comparing `qiskit-qrack-provider-0.6.0/README.md` & `qiskit-qrack-provider-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/__init__.py` & `qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/backends/__init__.py` & `qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/backends/qasm_simulator.py` & `qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/backends/qasm_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,16 @@
         'is_schmidt_decompose_multi': True,
         'is_schmidt_decompose': True,
         'is_stabilizer_hybrid': True,
         'is_binary_decision_tree': False,
         'is_paged': True,
         'is_cpu_gpu_hybrid': True,
         'is_host_pointer': False,
+        'is_t_injected': True,
+        'is_reactively_separated': True
     }
 
     DEFAULT_CONFIGURATION = {
         'backend_name': 'statevector_simulator',
         'backend_version': __version__,
         'n_qubits': 64,
         'conditional': True,
@@ -516,14 +518,16 @@
             'isPaged': options.is_paged if hasattr(options, 'is_paged') else self._options.get('is_paged'),
             'isCpuGpuHybrid': options.is_cpu_gpu_hybrid if hasattr(options, 'is_cpu_gpu_hybrid') else self._options.get('is_cpu_gpu_hybrid'),
             'isHostPointer': options.is_host_pointer if hasattr(options, 'is_host_pointer') else self._options.get('is_host_pointer'),
         }
 
         data = run_input.config.memory if hasattr(run_input, 'config') else []
         self._shots = options['shots'] if 'shots' in options else (run_input.config.shots if hasattr(run_input, 'config') else self._options.get('shots'))
+        self.is_t = options.is_t_injected if hasattr(options, 'is_t_injected') else self._options.get('is_t_injected')
+        self.is_reactive = options.is_reactively_separated if hasattr(options, 'is_reactively_separated') else self._options.get('is_reactively_separated')
         qobj_id = options['qobj_id'] if 'qobj_id' in options else (run_input.qobj_id if hasattr(run_input, 'config') else '')
         qobj_header = options['qobj_header'] if 'qobj_header' in options else (run_input.header if hasattr(run_input, 'config') else {})
         job_id = str(uuid.uuid4())
 
         job = QrackJob(self, job_id, self._run_job(job_id, run_input, data, qobj_id, qobj_header, **qrack_options), run_input)
         return job
 
@@ -658,31 +662,37 @@
             self._sample_measure = True
             shotsPerLoop = self._shots
             shotLoopMax = 1
         else:
             boundary_start -= 1
             if boundary_start > 0:
                 self._sim = QrackSimulator(qubitCount = self._number_of_qubits, **options)
+                self._sim.set_t_injection(is_t)
+                self._sim.set_reactive_separate(self.is_reactive)
                 self._classical_memory = 0
                 self._classical_register = 0
 
                 for operation in instructions[:boundary_start]:
                     self._apply_op(operation)
 
                 preamble_memory = self._classical_memory
                 preamble_register = self._classical_register
                 preamble_sim = self._sim
 
         for shot in range(shotLoopMax):
             if preamble_sim is None:
                 self._sim = QrackSimulator(qubitCount = self._number_of_qubits, **options)
+                self._sim.set_t_injection(is_t)
+                self._sim.set_reactive_separate(self.is_reactive)
                 self._classical_memory = 0
                 self._classical_register = 0
             else:
                 self._sim = QrackSimulator(cloneSid = preamble_sim.sid)
+                self._sim.set_t_injection(is_t)
+                self._sim.set_reactive_separate(self.is_reactive)
                 self._classical_memory = preamble_memory
                 self._classical_register = preamble_register
 
             for operation in instructions[boundary_start:]:
                 self._apply_op(operation)
 
             if not self._sample_measure and (len(self._sample_qubits) > 0):
```

### Comparing `qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/qrackerror.py` & `qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/qrackerror.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/qrackjob.py` & `qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/qrackjob.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/qrackprovider.py` & `qiskit-qrack-provider-0.7.0/qiskit/providers/qrack/qrackprovider.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/PKG-INFO` & `qiskit-qrack-provider-0.7.0/qiskit_qrack_provider.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-qrack-provider
-Version: 0.6.0
+Version: 0.7.0
 Summary: Qiskit Qrack Provider - Qrack High-Performance GPU simulation for Qiskit
 Home-page: https://github.com/vm6502q/qiskit-qrack-provider
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: Apache 2.0
 Keywords: qiskit qrack pyqrack simulator quantum addon backend
 Classifier: Environment :: Console
```

### Comparing `qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/SOURCES.txt` & `qiskit-qrack-provider-0.7.0/qiskit_qrack_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.6.0/setup.py` & `qiskit-qrack-provider-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = [
     'numpy>=1.16.3',
     'pyqrack>=0.8.0'
 ]
 
 # Handle version.
-VERSION = "0.6.0"
+VERSION = "0.7.0"
 
 # Read long description from README.
 README_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)),
                            'README.md')
 with open(README_PATH) as readme_file:
     README = readme_file.read()
```

