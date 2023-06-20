# Comparing `tmp/thunder-ase-0.3.1.tar.gz` & `tmp/thunder-ase-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunder-ase-0.3.1.tar", last modified: Mon Jun  5 05:04:06 2023, max compression
+gzip compressed data, was "thunder-ase-0.4.tar", last modified: Tue Jun 20 09:43:19 2023, max compression
```

## Comparing `thunder-ase-0.3.1.tar` & `thunder-ase-0.4.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:04:06.462797 thunder-ase-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-05 05:04:06.462797 thunder-ase-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-05 05:03:56.000000 thunder-ase-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-05 05:03:56.000000 thunder-ase-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 05:04:06.462797 thunder-ase-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 05:03:56.000000 thunder-ase-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:04:06.462797 thunder-ase-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-05 05:03:56.000000 thunder-ase-0.3.1/tests/test_Si_lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:04:06.462797 thunder-ase-0.3.1/thunder_ase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 05:03:56.000000 thunder-ase-0.3.1/thunder_ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30732 2023-06-05 05:03:56.000000 thunder-ase-0.3.1/thunder_ase/fireball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 05:04:06.462797 thunder-ase-0.3.1/thunder_ase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-05 05:04:06.000000 thunder-ase-0.3.1/thunder_ase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-05 05:04:06.000000 thunder-ase-0.3.1/thunder_ase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 05:04:06.000000 thunder-ase-0.3.1/thunder_ase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 05:04:06.000000 thunder-ase-0.3.1/thunder_ase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 05:04:06.000000 thunder-ase-0.3.1/thunder_ase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:43:19.731167 thunder-ase-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-20 09:43:19.731167 thunder-ase-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-20 09:43:07.000000 thunder-ase-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-20 09:43:07.000000 thunder-ase-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:43:19.731167 thunder-ase-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:43:07.000000 thunder-ase-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:43:19.731167 thunder-ase-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-20 09:43:07.000000 thunder-ase-0.4/tests/test_Si_lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:43:19.731167 thunder-ase-0.4/thunder_ase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:43:07.000000 thunder-ase-0.4/thunder_ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32039 2023-06-20 09:43:07.000000 thunder-ase-0.4/thunder_ase/fireball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:43:19.731167 thunder-ase-0.4/thunder_ase/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-20 09:43:07.000000 thunder-ase-0.4/thunder_ase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-06-20 09:43:07.000000 thunder-ase-0.4/thunder_ase/utils/basis_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-20 09:43:07.000000 thunder-ase-0.4/thunder_ase/utils/mwfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-20 09:43:07.000000 thunder-ase-0.4/thunder_ase/utils/shell_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:43:19.731167 thunder-ase-0.4/thunder_ase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-20 09:43:19.000000 thunder-ase-0.4/thunder_ase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-20 09:43:19.000000 thunder-ase-0.4/thunder_ase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:43:19.000000 thunder-ase-0.4/thunder_ase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 09:43:19.000000 thunder-ase-0.4/thunder_ase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 09:43:19.000000 thunder-ase-0.4/thunder_ase.egg-info/top_level.txt
```

### Comparing `thunder-ase-0.3.1/PKG-INFO` & `thunder-ase-0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.3.1
+Version: 0.4
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,10 +36,11 @@
   * v0.1.1: jupyter-notebook for examples
   * v0.1.2: multiple atoms for one calculator
   * v0.1.3: read fireball input to construct calculator
 * v0.2: band structure calculation.
   * v0.2.1: DOS calculation.
 * v0.3.1: fit basis to gaussian, write orbitals to mwfn.
   * v0.3.2: interface to multiwfn.
-* v0.4: MD calculation.
-* v0.5: Fdata management.
-* v0.6: interactive running.
+* v0.4: Read charge and population.
+* v0.5: MD calculation.
+* v0.6: Fdata management.
+* v0.7: interactive running.
```

### Comparing `thunder-ase-0.3.1/README.md` & `thunder-ase-0.4/thunder_ase.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,46 @@
-[![Upload Python Package](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml)
-
-# Thunder ASE
-
-### Description
-The interface of ASE for FIREBALL.  
-
-[FIREBALL](https://sites.google.com/site/fireballofficialsite/) is a local-orbital ab-initio tight binding implementation of  molecular dynamics. The method allows for the simulation and calculation of very large supercells of thousands of atoms or very long MD  simulations with ease.
-
-[ASE](https://wiki.fysik.dtu.dk/ase/index.html) is a popular python package for atomic structure modeling. ASE provide interfaces with many QM and MM software. This package is the interface for FIREBALL. 
-
-### Installation
-
-`pip install thunder-ase`
-
-#### Requirements
-
-* ase
-
-## Roadmap
-
-* v0.1: run basic fireball calculation and read basic result from it.
-  * v0.1.1: jupyter-notebook for examples
-  * v0.1.2: multiple atoms for one calculator
-  * v0.1.3: read fireball input to construct calculator
-* v0.2: band structure calculation.
-  * v0.2.1: DOS calculation.
-* v0.3.1: fit basis to gaussian, write orbitals to mwfn.
-  * v0.3.2: interface to multiwfn.
-* v0.4: MD calculation.
-* v0.5: Fdata management.
-* v0.6: interactive running.
+Metadata-Version: 2.1
+Name: thunder-ase
+Version: 0.4
+Summary: ASE calculator interface for FIREBALL code
+Author-email: PJ Ren <openrpj@gmail.com>
+Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
+Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+[![Upload Python Package](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml)
+
+# Thunder ASE
+
+### Description
+The interface of ASE for FIREBALL.  
+
+[FIREBALL](https://sites.google.com/site/fireballofficialsite/) is a local-orbital ab-initio tight binding implementation of  molecular dynamics. The method allows for the simulation and calculation of very large supercells of thousands of atoms or very long MD  simulations with ease.
+
+[ASE](https://wiki.fysik.dtu.dk/ase/index.html) is a popular python package for atomic structure modeling. ASE provide interfaces with many QM and MM software. This package is the interface for FIREBALL. 
+
+### Installation
+
+`pip install thunder-ase`
+
+#### Requirements
+
+* ase
+
+## Roadmap
+
+* v0.1: run basic fireball calculation and read basic result from it.
+  * v0.1.1: jupyter-notebook for examples
+  * v0.1.2: multiple atoms for one calculator
+  * v0.1.3: read fireball input to construct calculator
+* v0.2: band structure calculation.
+  * v0.2.1: DOS calculation.
+* v0.3.1: fit basis to gaussian, write orbitals to mwfn.
+  * v0.3.2: interface to multiwfn.
+* v0.4: Read charge and population.
+* v0.5: MD calculation.
+* v0.6: Fdata management.
+* v0.7: interactive running.
```

### Comparing `thunder-ase-0.3.1/pyproject.toml` & `thunder-ase-0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "thunder-ase"
-version = "0.3.1"
+version = "0.4"
 authors = [
   { name="PJ Ren", email="openrpj@gmail.com" },
 ]
 description = "ASE calculator interface for FIREBALL code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -17,12 +17,12 @@
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
 fit-gaussians = "thunder_ase.utils:fit_gaussian"
 
 [tool.setuptools]
-packages=['thunder_ase']
+packages=['thunder_ase', 'thunder_ase.utils']
 
 [project.urls]
 "Homepage" = "https://github.com/thunder-dft/thunder-ase"
 "Bug Tracker" = "https://github.com/thunder-dft/thunder-ase/issues"
```

### Comparing `thunder-ase-0.3.1/tests/test_Si_lightning.py` & `thunder-ase-0.4/tests/test_Si_lightning.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.3.1/thunder_ase/fireball.py` & `thunder-ase-0.4/thunder_ase/fireball.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from ase.geometry import get_distances
 import ase.spacegroup
 from ase.io import jsonio
 from ase.dft.kpoints import BandPath
 from thunder_ase.utils.mwfn import MWFN_FORMAT, MWFN_DEFAULT, MWFN_TEMPLATE, \
     CELL_TEMPLATE, format_data, read_cdcoeffs, reorder_cdcoeffs
 from thunder_ase.utils.basis_set import read_info, read_gaussian
-from thunder_ase.utils.shell_dict import SHELL_NUM, SHELL_NAME, SHELL_PRIMARY_NUMS, SHELL_PRIMITIVE
+from thunder_ase.utils.shell_dict import SHELL_PRIMARY_NUMS, SHELL_PRIMITIVE
 
 
 def get_kpts(atoms, size=None, offset=None, reduced=False, **kwargs):
     """
     Get reduced kpoints.
     Reference:
     * https://wiki.fysik.dtu.dk/ase/ase/dft/kpoints.html
@@ -38,34 +38,26 @@
     TODO: compare with vasp in several systems
     """
     # generate MP kpoints
     kpoints = monkhorst_pack(size) + np.asarray(offset)
     kpoints = kpoint_convert(cell_cv=atoms.cell, skpts_kc=kpoints)  # convert from scaled and cartesian coordinates
     nkpt = len(kpoints)
     if not reduced or nkpt <= 1:
-        kpoints_weight = []
-        for k in kpoints:
-            kx, ky, kz = k
-            kpoints_weight.append([kx, ky, kz, 1.0 / nkpt])
-        return kpoints_weight
+        return [[kx, ky, kz, 1.0 / nkpt] for kx, ky, kz in kpoints]
 
     if 'symprec' in kwargs:
         symprec = kwargs['symprec']
     else:
         symprec = 1e-05  # for Cartesian coordinate in real space
     try:
         # get spacegroup from atoms ase.spacegroup.get_spacegroup
         sg = ase.spacegroup.get_spacegroup(atoms, symprec=symprec)
     except RuntimeError:
         print("Didn't find symmetry. No reducing is needed.")
-        kpoints_weight = []
-        for k in kpoints:
-            kx, ky, kz = k
-            kpoints_weight.append([kx, ky, kz, 1.0 / nkpt])
-        return kpoints_weight
+        return [[kx, ky, kz, 1.0 / nkpt] for kx, ky, kz in kpoints]
 
     kpts_extend = []  # all the symmetry points for each kpts
     for kpt in kpoints:
         sites, kinds = sg.equivalent_sites([kpt])
         kpts_extend.append(sites)
 
     irreducible_dct = dict()
@@ -90,32 +82,33 @@
     kpoints_weight = [[k[0], k[1], k[2], len(v) / nkpt] for k, v in irreducible_dct.items()]
     return kpoints_weight
 
 
 options_params = {
     'nstepi': {'type': (int,), 'name': 'nstepi', 'default': 1},
     'nstepf': {'type': (int,), 'name': 'nstepf', 'default': 1},
+    'qstate': {'type': (int,), 'name': 'qstate', 'default': 0},  # Extra electron. +1 mean adding 1 electron.
     'iquench': {'type': (int,), 'name': 'iquench', 'default': 0},
     't_initial': {'type': (int, float), 'name': 'T_initial', 'default': 300.0},
     't_final': {'type': (int, float), 'name': 'T_final', 'default': 0.0},
     't_want': {'type': (int, float), 'name': 'T_want', 'default': 300.0},
     'taurelax': {'type': (int, float), 'name': 'taurelax', 'default': 5.0},
     'efermi_t': {'type': (int, float), 'name': 'efermi_T', 'default': 100.0},
     'dt': {'type': (int, float), 'name': 'dt', 'default': 0.25},  # fs
     'iensemble': {'type': (int,), 'name': 'iensemble', 'default': 0},
-    'iconstraint_rcm': {'type': (int,), 'name': 'iconstraint_rcm', 'default': 1},
-    'iconstraint_vcm': {'type': (int,), 'name': 'iconstraint_vcm', 'default': 1},
+    'iconstraint_rcm': {'type': (int,), 'name': 'iconstraint_rcm', 'default': 1},  # shift molecule to COM or not
+    'iconstraint_vcm': {'type': (int,), 'name': 'iconstraint_vcm', 'default': 1},  # whether keep COM fixed during md
     'iconstraint_l': {'type': (int,), 'name': 'iconstraint_L', 'default': 0},
     'iconstraint_ke': {'type': (int,), 'name': 'iconstraint_KE', 'default': 1},
     'ifix_neighbors': {'type': (int,), 'name': 'ifix_neighbors', 'default': 0},
     'ifix_charges': {'type': (int,), 'name': 'ifix_CHARGES', 'default': 1},
     'max_scf_iterations_set': {'type': (int,), 'name': 'max_scf_iterations_set', 'default': 50},
     'scf_tolerance_set': {'type': (int, float), 'name': 'scf_tolerance_set', 'default': 0.00000001},
-    'beta_set': {'type': (int, float), 'name': 'beta_set', 'default': 0.08},
-    'ecut_set': {'type': (int, float), 'name': 'Ecut_set', 'default': 200.0},
+    'beta_set': {'type': (int, float), 'name': 'beta_set', 'default': 0.08},  # mix factor
+    'ecut_set': {'type': (int, float), 'name': 'Ecut_set', 'default': 200.0},  # control mesh grid number
 }
 
 output_params = {
     'iwriteout_me_sandh': {'type': (int,), 'name': 'iwriteout_ME_SandH', 'default': 0},
     'iwriteout_density': {'type': (int,), 'name': 'iwriteout_density', 'default': 0},
     'iwriteout_cdcoeffs': {'type': (int,), 'name': 'iwriteout_cdcoeffs', 'default': 0},
     'iwriteout_charges': {'type': (int,), 'name': 'iwriteout_charges', 'default': 0},
@@ -130,20 +123,20 @@
 
 xsfoptions_params = {
     'rho_surface_min': {'type': (int, float), 'name': 'rho_surface_min', 'default': 0.0005},
     'rho_surface_max': {'type': (int, float), 'name': 'rho_surface_max', 'default': 0.1},
 }
 
 calc_params = {
-    'kpt_size': {'type': (list, np.array), 'name': 'kpt_size', 'default': [1, 1, 1]},
-    'kpt_offset': {'type': (list, np.array), 'name': 'kpt_offset', 'default': [0., 0., 0.]},
+    'kpt_size': {'type': (list, np.array), 'name': 'kpt_size', 'default': None},
+    'kpt_offset': {'type': (list, np.array), 'name': 'kpt_offset', 'default': None},
     'kpt_interval': {'type': (list, np.array, float, int), 'name': 'kpt_interval', 'default': None},
     'kpt_path': {'type': (BandPath, str, list, np.array), 'name': 'kpt_path', 'default': None},
-    'nkpt': {'type': (int,), 'name': 'nkpt', 'default': None},
-    # number of kpoints on path, use it if kpt_path is string
+    'nkpt': {'type': (int,), 'name': 'nkpt', 'default': None},  # n kpoints on path. Used if kpt_path is string.
+    'kpt_reduced': {'type': (bool,), 'name': 'kpt_reduced', 'default': False},
 }
 
 fireball_params = options_params | output_params | xsfoptions_params | calc_params
 
 
 def get_params_from_string(s):
     k, v = s.split('=')
@@ -172,19 +165,20 @@
         else:
             self._atoms = None
         self.sname = '001'
         self.output_params = {}
         self.options_params = {}
         self.xsfoptions_params = {}
 
-        self.kpt_size = None
-        self.kpt_interval = None
-        self.kpt_offset = None
-        self.kpt_path = None
-        self.nkpt = None
+        self.kpt_size = fireball_params['kpt_size']['default']
+        self.kpt_interval = fireball_params['kpt_interval']['default']
+        self.kpt_offset = fireball_params['kpt_offset']['default']
+        self.kpt_path = fireball_params['kpt_path']['default']
+        self.nkpt = fireball_params['nkpt']['default']
+        self.kpt_reduced = fireball_params['kpt_reduced']['default']
         self._kpoints = None
 
         self.check_kwargs(kwargs)
 
     @property
     def atoms(self):
         return self._atoms
@@ -275,14 +269,16 @@
                 self.kpt_offset = v
             elif k == 'kpt_interval':
                 self.kpt_interval = v
             elif k == 'kpt_path':
                 self.kpt_path = v
             elif k == 'nkpt':
                 self.nkpt = v
+            elif k == 'kpt_reduced':
+                self.kpt_reduced = v
         return
 
     def write_options(self):
         with open('structures.inp', 'w') as f:
             f.write("1\n")
             f.write("{}.inp\n".format(self.sname))
 
@@ -297,14 +293,20 @@
             f.write("&END\n")
 
             f.write("&XSFOPTIONS\n")
             write_params(self.xsfoptions_params, f)
             f.write("&END\n")
 
     def write_atoms(self, atoms=None, pbc=None):
+        """
+        TODO: for non-PBC system, set cell to [0.000] * 9
+        :param atoms:
+        :param pbc:
+        :return:
+        """
         if atoms is not None:
             self.atoms = atoms.copy()
 
         with open(self.sname + ".inp", 'w') as f:
             if pbc is None:
                 ipbc = 0 if np.any(self.atoms.pbc) else 1
             else:
@@ -334,15 +336,15 @@
     def write_input(self, atoms=None, Fdata_path=None):
         if atoms is not None:
             self.atoms = atoms.copy()
         self.write_Fdata_inp(atoms=self.atoms, Fdata_path=Fdata_path)
         self.write_options()
         self.write_atoms(pbc=self.atoms.pbc)
         if np.any(self.atoms.pbc):
-            self.write_kpts()
+            self.write_kpts(reduced=self.kpt_reduced)
 
     def read_options(self, input_file='structures.inp', read_atoms=False):
         # read structures.inp, get names for atoms and kpoints
         with open(input_file, 'r') as f:
             lines = f.readlines()
 
         natoms_list = int(lines[0].strip())
@@ -480,18 +482,36 @@
             directory = self.directory
         errorcode = subprocess.call(command,
                                     shell=True,
                                     cwd=directory)
         return errorcode
 
     def read_results(self):
-        output = self.sname + ".log.json"
+        output = self.sname + ".json"
         result = jsonio.read_json(output)
+        if 'charges' in result['fireball'][-1]:
+            shell_charges = result['fireball'][-1]['charges']
+            result['fireball'][-1]['shell_charges'] = shell_charges
         self.results = result['fireball'][-1]
 
+    def get_charges(self, atoms=None):
+        if self.results is None:
+            try:
+                self.read_results()
+            except AttributeError:
+                return None
+        shell_charges = self.results['fireball'][-1]['shell_charges']
+        sum_charges = [sum(isc) for isc in shell_charges]
+        if atoms is None:
+            atoms = self.atoms
+        ref_charges = [sum(self.shell_info[s]['occupation']) for s in atoms.symbols]
+        charges = [ref-sc for sc, ref in zip(sum_charges, ref_charges)]
+        self.results['charges'] = charges
+        return charges
+
     def get_forces(self, atoms=None):
         forces = self.get_property('forces', atoms)
         return np.asarray(forces)
 
     def get_fermi_level(self):
         return self.get_property('fermi')
 
@@ -612,15 +632,15 @@
         # Initialize default data format
         for k, v in mwfn_dict.items():
             if v is not None:
                 mwfn_dict[k] = MWFN_FORMAT[k].format(v)
 
         # atom information
         mwfn_dict['ncenter'] = MWFN_FORMAT['ncenter'].format(len(self.atoms))
-        atoms_coord = [MWFN_FORMAT['atoms_coord'].format(idx+1,
+        atoms_coord = [MWFN_FORMAT['atoms_coord'].format(idx + 1,
                                                          iatom.symbol,
                                                          iatom.number,
                                                          self.get_valence_charge(idx),
                                                          *iatom.position)
                        for idx, iatom in enumerate(self.atoms)]
         mwfn_dict['atoms_coord'] = '\n'.join(atoms_coord)
 
@@ -648,26 +668,26 @@
         shell_types = []
         shell_centers = []
         shell_contraction_degress = []
         primitive_exponents = []
         contraction_coefficients = []
         for idx, symbol in enumerate(self.atoms.symbols):
             ishells = self.shell_info[symbol]['shells']
-            shell_centers += [idx+1] * len(ishells)
+            shell_centers += [idx + 1] * len(ishells)
             shell_types += ishells
             excited_label = self.shell_info[symbol]['excited']
             for shell, is_excited in zip(ishells, excited_label):
                 gbs = read_gaussian(self.shell_info[symbol]['number'], shell, is_excited, Fdata_path=self.Fdata_path)
                 shell_contraction_degress.append(gbs['degree'])
                 primitive_exponents += gbs['alpha'].tolist()
                 contraction_coefficients += gbs['coefficient'].tolist()
-        nbasis = sum([shell*2+1 for shell in shell_types])
+        nbasis = sum([shell * 2 + 1 for shell in shell_types])
         nshell = len(shell_types)
         nprimshell = len(primitive_exponents)
-        nprims = sum([SHELL_PRIMITIVE[st]*degree
+        nprims = sum([SHELL_PRIMITIVE[st] * degree
                       for st, degree in zip(shell_types, shell_contraction_degress)])
         shell_types = [((i < 2) * 2 - 1) * i for i in shell_types]  # if i >= 2, use negative value
 
         mwfn_dict['nbasis'] = MWFN_FORMAT['nbasis'].format(nbasis)
         mwfn_dict['nindbasis'] = MWFN_FORMAT['nindbasis'].format(nbasis)
         mwfn_dict['nprims'] = MWFN_FORMAT['nprims'].format(nprims)
         mwfn_dict['nshell'] = MWFN_FORMAT['nshell'].format(nshell)
@@ -675,15 +695,15 @@
 
         mwfn_dict['shell_types'] = format_data('shell_types', shell_types)
         mwfn_dict['shell_centers'] = format_data('shell_centers', shell_centers)
         mwfn_dict['shell_contraction_degress'] = format_data('shell_contraction_degress', shell_contraction_degress)
         mwfn_dict['primitive_exponents'] = format_data('primitive_exponents', primitive_exponents)
         mwfn_dict['contraction_coefficients'] = format_data('contraction_coefficients', contraction_coefficients)
 
-        cdcoeffs = read_cdcoeffs(self.sname+'.cdcoeffs-mwfn')[kpoint]
+        cdcoeffs = read_cdcoeffs(self.sname + '.cdcoeffs-mwfn')[kpoint]
         orbital_coeffs = []
         for orbital in cdcoeffs:
             info = ''.join(orbital['info'])
             coeff = orbital['coeff']
             coeff = reorder_cdcoeffs(coeff, shell_types)
             orbital_coeffs += [info + format_data('MO_coefficients', coeff)]
         mwfn_dict['orbital_coeffs'] = '\n\n'.join(orbital_coeffs)
```

### Comparing `thunder-ase-0.3.1/thunder_ase.egg-info/PKG-INFO` & `thunder-ase-0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,33 @@
-Metadata-Version: 2.1
-Name: thunder-ase
-Version: 0.3.1
-Summary: ASE calculator interface for FIREBALL code
-Author-email: PJ Ren <openrpj@gmail.com>
-Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
-Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-[![Upload Python Package](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml)
-
-# Thunder ASE
-
-### Description
-The interface of ASE for FIREBALL.  
-
-[FIREBALL](https://sites.google.com/site/fireballofficialsite/) is a local-orbital ab-initio tight binding implementation of  molecular dynamics. The method allows for the simulation and calculation of very large supercells of thousands of atoms or very long MD  simulations with ease.
-
-[ASE](https://wiki.fysik.dtu.dk/ase/index.html) is a popular python package for atomic structure modeling. ASE provide interfaces with many QM and MM software. This package is the interface for FIREBALL. 
-
-### Installation
-
-`pip install thunder-ase`
-
-#### Requirements
-
-* ase
-
-## Roadmap
-
-* v0.1: run basic fireball calculation and read basic result from it.
-  * v0.1.1: jupyter-notebook for examples
-  * v0.1.2: multiple atoms for one calculator
-  * v0.1.3: read fireball input to construct calculator
-* v0.2: band structure calculation.
-  * v0.2.1: DOS calculation.
-* v0.3.1: fit basis to gaussian, write orbitals to mwfn.
-  * v0.3.2: interface to multiwfn.
-* v0.4: MD calculation.
-* v0.5: Fdata management.
-* v0.6: interactive running.
+[![Upload Python Package](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml)
+
+# Thunder ASE
+
+### Description
+The interface of ASE for FIREBALL.  
+
+[FIREBALL](https://sites.google.com/site/fireballofficialsite/) is a local-orbital ab-initio tight binding implementation of  molecular dynamics. The method allows for the simulation and calculation of very large supercells of thousands of atoms or very long MD  simulations with ease.
+
+[ASE](https://wiki.fysik.dtu.dk/ase/index.html) is a popular python package for atomic structure modeling. ASE provide interfaces with many QM and MM software. This package is the interface for FIREBALL. 
+
+### Installation
+
+`pip install thunder-ase`
+
+#### Requirements
+
+* ase
+
+## Roadmap
+
+* v0.1: run basic fireball calculation and read basic result from it.
+  * v0.1.1: jupyter-notebook for examples
+  * v0.1.2: multiple atoms for one calculator
+  * v0.1.3: read fireball input to construct calculator
+* v0.2: band structure calculation.
+  * v0.2.1: DOS calculation.
+* v0.3.1: fit basis to gaussian, write orbitals to mwfn.
+  * v0.3.2: interface to multiwfn.
+* v0.4: Read charge and population.
+* v0.5: MD calculation.
+* v0.6: Fdata management.
+* v0.7: interactive running.
```

