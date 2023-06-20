# Comparing `tmp/qiskit-qrack-provider-0.5.2.tar.gz` & `tmp/qiskit-qrack-provider-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-qrack-provider-0.5.2.tar", last modified: Sat Jun  3 15:46:52 2023, max compression
+gzip compressed data, was "qiskit-qrack-provider-0.6.0.tar", last modified: Tue Jun 20 14:37:55 2023, max compression
```

## Comparing `qiskit-qrack-provider-0.5.2.tar` & `qiskit-qrack-provider-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-03 15:46:52.521543 qiskit-qrack-provider-0.5.2/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2021-05-14 12:44:18.000000 qiskit-qrack-provider-0.5.2/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2691 2023-06-03 15:46:52.517543 qiskit-qrack-provider-0.5.2/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1671 2021-12-03 23:15:01.000000 qiskit-qrack-provider-0.5.2/README.md
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-03 15:46:52.517543 qiskit-qrack-provider-0.5.2/qiskit/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-03 15:46:52.517543 qiskit-qrack-provider-0.5.2/qiskit/providers/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-03 15:46:52.517543 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1135 2021-10-08 01:17:38.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/__init__.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-03 15:46:52.517543 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/backends/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      548 2023-06-03 15:41:45.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/backends/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    36664 2023-06-03 15:45:18.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/backends/qasm_simulator.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      914 2021-05-14 12:44:18.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/qrackerror.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1903 2021-10-09 18:55:08.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/qrackjob.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1449 2023-06-03 15:42:03.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/qrackprovider.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      506 2023-06-03 15:42:26.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/version.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-03 15:46:52.517543 qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2691 2023-06-03 15:46:52.000000 qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      525 2023-06-03 15:46:52.000000 qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-06-03 15:46:52.000000 qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       29 2023-06-03 15:46:52.000000 qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/requires.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        7 2023-06-03 15:46:52.000000 qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-06-03 15:46:52.521543 qiskit-qrack-provider-0.5.2/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1642 2023-06-03 15:41:06.000000 qiskit-qrack-provider-0.5.2/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2021-05-14 12:44:18.000000 qiskit-qrack-provider-0.6.0/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2691 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1671 2021-12-03 23:15:01.000000 qiskit-qrack-provider-0.6.0/README.md
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/qiskit/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/qiskit/providers/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1135 2021-10-08 01:17:38.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/__init__.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/backends/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      548 2023-06-20 14:23:28.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/backends/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    36810 2023-06-20 14:36:16.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/backends/qasm_simulator.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      914 2021-05-14 12:44:18.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/qrackerror.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1903 2021-10-09 18:55:08.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/qrackjob.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1449 2023-06-20 14:23:28.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/qrackprovider.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      506 2023-06-03 15:42:26.000000 qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/version.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2691 2023-06-20 14:37:55.000000 qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      525 2023-06-20 14:37:55.000000 qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-06-20 14:37:55.000000 qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       29 2023-06-20 14:37:55.000000 qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/requires.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        7 2023-06-20 14:37:55.000000 qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-06-20 14:37:55.695530 qiskit-qrack-provider-0.6.0/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1642 2023-06-20 14:37:15.000000 qiskit-qrack-provider-0.6.0/setup.py
```

### Comparing `qiskit-qrack-provider-0.5.2/LICENSE` & `qiskit-qrack-provider-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.2/PKG-INFO` & `qiskit-qrack-provider-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-qrack-provider
-Version: 0.5.2
+Version: 0.6.0
 Summary: Qiskit Qrack Provider - Qrack High-Performance GPU simulation for Qiskit
 Home-page: https://github.com/vm6502q/qiskit-qrack-provider
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: Apache 2.0
 Keywords: qiskit qrack pyqrack simulator quantum addon backend
 Classifier: Environment :: Console
```

### Comparing `qiskit-qrack-provider-0.5.2/README.md` & `qiskit-qrack-provider-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/__init__.py` & `qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/backends/__init__.py` & `qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/backends/qasm_simulator.py` & `qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/backends/qasm_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -742,14 +742,16 @@
             self._sim.u(operation.qubits[0], 0, 0, float(operation.params[0]))
         elif name == 'u2':
             self._sim.u(operation.qubits[0], np.pi / 2, float(operation.params[0]), float(operation.params[1]))
         elif (name == 'u3') or (name == 'u'):
             self._sim.u(operation.qubits[0], float(operation.params[0]), float(operation.params[1]), float(operation.params[2]))
         elif name == 'r':
             self._sim.u(operation.qubits[0], float(operation.params[0]), float(operation.params[1]) - np.pi/2, (-1 * float(operation.params[1])) + np.pi/2)
+        elif (name == 'unitary') and (len(operation.qubits) == 1):
+            self._sim.mtrx(operation.params[0].flatten(), operation.qubits[0])
         elif name == 'rx':
             self._sim.r(Pauli.PauliX, float(operation.params[0]), operation.qubits[0])
         elif name == 'ry':
             self._sim.r(Pauli.PauliY, float(operation.params[0]), operation.qubits[0])
         elif name == 'rz':
             self._sim.r(Pauli.PauliZ, float(operation.params[0]), operation.qubits[0])
         elif name == 'h':
```

### Comparing `qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/qrackerror.py` & `qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/qrackerror.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/qrackjob.py` & `qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/qrackjob.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/qrackprovider.py` & `qiskit-qrack-provider-0.6.0/qiskit/providers/qrack/qrackprovider.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/PKG-INFO` & `qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-qrack-provider
-Version: 0.5.2
+Version: 0.6.0
 Summary: Qiskit Qrack Provider - Qrack High-Performance GPU simulation for Qiskit
 Home-page: https://github.com/vm6502q/qiskit-qrack-provider
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: Apache 2.0
 Keywords: qiskit qrack pyqrack simulator quantum addon backend
 Classifier: Environment :: Console
```

### Comparing `qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/SOURCES.txt` & `qiskit-qrack-provider-0.6.0/qiskit_qrack_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.2/setup.py` & `qiskit-qrack-provider-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = [
     'numpy>=1.16.3',
     'pyqrack>=0.8.0'
 ]
 
 # Handle version.
-VERSION = "0.5.2"
+VERSION = "0.6.0"
 
 # Read long description from README.
 README_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)),
                            'README.md')
 with open(README_PATH) as readme_file:
     README = readme_file.read()
```

