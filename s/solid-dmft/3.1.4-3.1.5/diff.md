# Comparing `tmp/solid_dmft-3.1.4.tar.gz` & `tmp/solid_dmft-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solid_dmft-3.1.4.tar", last modified: Thu Feb 23 20:26:23 2023, max compression
+gzip compressed data, was "solid_dmft-3.1.5.tar", last modified: Tue Jun 20 16:28:48 2023, max compression
```

## Comparing `solid_dmft-3.1.4.tar` & `solid_dmft-3.1.5.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-02-23 20:26:23.009229 solid_dmft-3.1.4/
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)      885 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/LICENSE.txt
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)      227 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/MANIFEST.in
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     3445 2023-02-23 20:26:23.009229 solid_dmft-3.1.4/PKG-INFO
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     2796 2023-01-17 19:52:54.000000 solid_dmft-3.1.4/README.md
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)      909 2023-02-23 20:04:35.000000 solid_dmft-3.1.4/pyproject.toml
-drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-02-23 20:26:22.999229 solid_dmft-3.1.4/python/
-drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-02-23 20:26:22.999229 solid_dmft-3.1.4/python/solid_dmft/
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1126 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/__init__.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)    16286 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/csc_flow.py
-drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-02-23 20:26:23.009229 solid_dmft-3.1.4/python/solid_dmft/dft_managers/
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1146 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/dft_managers/__init__.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     9673 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/dft_managers/qe_manager.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     8850 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/dft_managers/vasp_manager.py
--rwxr-xr-x   0 ahampel   (1000) ahampel   (1000)    39764 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_cycle.py
-drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-02-23 20:26:23.009229 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1179 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/__init__.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     6014 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/afm_mapping.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)    12268 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/convergence.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     8953 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/formatter.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     9925 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/greens_functions_mixer.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)    22040 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/initial_self_energies.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)    23470 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/interaction_hamiltonian.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     2068 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/legendre_filter.py
--rwxr-xr-x   0 ahampel   (1000) ahampel   (1000)    18641 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/manipulate_chemical_potential.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)    24704 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/observables.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     7133 2023-02-10 17:37:34.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/results_to_archive.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)    48946 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/dmft_tools/solver.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     6792 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/main.py
-drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-02-23 20:26:23.009229 solid_dmft-3.1.4/python/solid_dmft/postprocessing/
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1143 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/postprocessing/__init__.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)    11274 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)    10289 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/postprocessing/maxent_gf_imp.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)    12826 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/postprocessing/maxent_gf_latt.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)    17254 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/postprocessing/maxent_sigma.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)    37525 2023-02-23 19:59:04.000000 solid_dmft-3.1.4/python/solid_dmft/postprocessing/plot_correlated_bands.py
--rwxr-xr-x   0 ahampel   (1000) ahampel   (1000)    64113 2023-02-23 19:58:58.000000 solid_dmft-3.1.4/python/solid_dmft/read_config.py
-drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-02-23 20:26:23.009229 solid_dmft-3.1.4/python/solid_dmft/util/
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1178 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/util/__init__.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     6808 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/util/symmetrize_gamma_file.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     4940 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/util/update_dmft_config.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     3814 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/util/update_results_h5.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     4727 2023-01-17 19:52:25.000000 solid_dmft-3.1.4/python/solid_dmft/util/write_kslice_to_h5.py
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1472 2023-02-23 20:22:32.000000 solid_dmft-3.1.4/python/solid_dmft/version.py
-drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-02-23 20:26:23.009229 solid_dmft-3.1.4/python/solid_dmft.egg-info/
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     3445 2023-02-23 20:26:22.000000 solid_dmft-3.1.4/python/solid_dmft.egg-info/PKG-INFO
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1714 2023-02-23 20:26:22.000000 solid_dmft-3.1.4/python/solid_dmft.egg-info/SOURCES.txt
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)        1 2023-02-23 20:26:22.000000 solid_dmft-3.1.4/python/solid_dmft.egg-info/dependency_links.txt
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)       52 2023-02-23 20:26:22.000000 solid_dmft-3.1.4/python/solid_dmft.egg-info/entry_points.txt
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)       32 2023-02-23 20:26:22.000000 solid_dmft-3.1.4/python/solid_dmft.egg-info/requires.txt
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)       11 2023-02-23 20:26:22.000000 solid_dmft-3.1.4/python/solid_dmft.egg-info/top_level.txt
--rw-r--r--   0 ahampel   (1000) ahampel   (1000)       38 2023-02-23 20:26:23.009229 solid_dmft-3.1.4/setup.cfg
+drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-06-20 16:28:48.555077 solid_dmft-3.1.5/
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    35147 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/COPYING.txt
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)      885 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/LICENSE.txt
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)      227 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/MANIFEST.in
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     3471 2023-06-20 16:28:48.555077 solid_dmft-3.1.5/PKG-INFO
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     2796 2023-01-17 19:52:54.000000 solid_dmft-3.1.5/README.md
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)      909 2023-06-20 16:22:43.000000 solid_dmft-3.1.5/pyproject.toml
+drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-06-20 16:28:48.545077 solid_dmft-3.1.5/python/
+drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-06-20 16:28:48.555077 solid_dmft-3.1.5/python/solid_dmft/
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1126 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/python/solid_dmft/__init__.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    15143 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/csc_flow.py
+drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-06-20 16:28:48.555077 solid_dmft-3.1.5/python/solid_dmft/dft_managers/
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1146 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/python/solid_dmft/dft_managers/__init__.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    11661 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/dft_managers/qe_manager.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    11845 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/dft_managers/vasp_manager.py
+-rwxr-xr-x   0 ahampel   (1000) ahampel   (1000)    38965 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_cycle.py
+drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-06-20 16:28:48.555077 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1179 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/__init__.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     6014 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/afm_mapping.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    12268 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/convergence.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     8953 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/formatter.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     9925 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/greens_functions_mixer.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    22040 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/initial_self_energies.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    23470 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/interaction_hamiltonian.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     2068 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/legendre_filter.py
+-rwxr-xr-x   0 ahampel   (1000) ahampel   (1000)    18641 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/manipulate_chemical_potential.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    24878 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/observables.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     7133 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/results_to_archive.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    48946 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/dmft_tools/solver.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     6792 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/main.py
+drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-06-20 16:28:48.555077 solid_dmft-3.1.5/python/solid_dmft/postprocessing/
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1143 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/python/solid_dmft/postprocessing/__init__.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    11274 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    10289 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/postprocessing/maxent_gf_imp.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    12826 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/postprocessing/maxent_gf_latt.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    17254 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/postprocessing/maxent_sigma.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)    37525 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/postprocessing/plot_correlated_bands.py
+-rwxr-xr-x   0 ahampel   (1000) ahampel   (1000)    65450 2023-06-20 16:22:31.000000 solid_dmft-3.1.5/python/solid_dmft/read_config.py
+drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-06-20 16:28:48.555077 solid_dmft-3.1.5/python/solid_dmft/util/
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1178 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/python/solid_dmft/util/__init__.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     6808 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/python/solid_dmft/util/symmetrize_gamma_file.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     4940 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/python/solid_dmft/util/update_dmft_config.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     3814 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/python/solid_dmft/util/update_results_h5.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     4727 2023-01-17 19:52:25.000000 solid_dmft-3.1.5/python/solid_dmft/util/write_kslice_to_h5.py
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1472 2023-06-20 16:27:36.000000 solid_dmft-3.1.5/python/solid_dmft/version.py
+drwxr-xr-x   0 ahampel   (1000) ahampel   (1000)        0 2023-06-20 16:28:48.555077 solid_dmft-3.1.5/python/solid_dmft.egg-info/
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     3471 2023-06-20 16:28:48.000000 solid_dmft-3.1.5/python/solid_dmft.egg-info/PKG-INFO
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)     1726 2023-06-20 16:28:48.000000 solid_dmft-3.1.5/python/solid_dmft.egg-info/SOURCES.txt
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)        1 2023-06-20 16:28:48.000000 solid_dmft-3.1.5/python/solid_dmft.egg-info/dependency_links.txt
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)       52 2023-06-20 16:28:48.000000 solid_dmft-3.1.5/python/solid_dmft.egg-info/entry_points.txt
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)       32 2023-06-20 16:28:48.000000 solid_dmft-3.1.5/python/solid_dmft.egg-info/requires.txt
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)       11 2023-06-20 16:28:48.000000 solid_dmft-3.1.5/python/solid_dmft.egg-info/top_level.txt
+-rw-r--r--   0 ahampel   (1000) ahampel   (1000)       38 2023-06-20 16:28:48.555077 solid_dmft-3.1.5/setup.cfg
```

### Comparing `solid_dmft-3.1.4/LICENSE.txt` & `solid_dmft-3.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/PKG-INFO` & `solid_dmft-3.1.5/python/solid_dmft.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
-Name: solid_dmft
-Version: 3.1.4
+Name: solid-dmft
+Version: 3.1.5
 Summary: solid_dmft: a versatile python wrapper to perform DFT+DMFT calculations utilizing the TRIQS software library
 Author-email: Alexander Hampel <ahampel@flatironinstitute.org>
 Project-URL: Homepage, https://triqs.github.io/solid_dmft
 Project-URL: Bug Tracker, https://github.com/triqs/solid_dmft/issues
 Keywords: DMFT,DFT,triqs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+License-File: COPYING.txt
 
 ![logo_soliDMFT](https://raw.githubusercontent.com/triqs/solid_dmft/unstable/doc/logos/logo_solid_dmft.png)
 
 ![CI](https://github.com/triqs/solid_dmft/actions/workflows/build.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/solid_dmft.svg)](https://badge.fury.io/py/solid_dmft)
 [![status](https://joss.theoj.org/papers/48eb529b08c6bb464b235ba919d78922/status.svg)](https://joss.theoj.org/papers/48eb529b08c6bb464b235ba919d78922)
```

### Comparing `solid_dmft-3.1.4/README.md` & `solid_dmft-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/pyproject.toml` & `solid_dmft-3.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["python"]
 
 [project]
 name = "solid_dmft"
-version = "3.1.4"
+version = "3.1.5"
 authors = [
   { name="Alexander Hampel", email="ahampel@flatironinstitute.org" }
 ]
 description = "solid_dmft: a versatile python wrapper to perform DFT+DMFT calculations utilizing the TRIQS software library"
 readme = "README.md"
 keywords = ["DMFT", "DFT", "triqs"]
 requires-python = ">=3.7"
```

### Comparing `solid_dmft-3.1.4/python/solid_dmft/__init__.py` & `solid_dmft-3.1.5/python/solid_dmft/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/csc_flow.py` & `solid_dmft-3.1.5/python/solid_dmft/csc_flow.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,31 +21,28 @@
 # <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
 contains the charge self-consistency flow control functions
 """
 
-import time
 from timeit import default_timer as timer
 import subprocess
 import shlex
 import os
 import numpy as np
 
 # triqs
 from h5 import HDFArchive
 import triqs.utility.mpi as mpi
+
 from triqs_dft_tools.converters.wannier90 import Wannier90Converter
-try:
-    from triqs_dft_tools.converters.vasp import VaspConverter
-    from triqs_dft_tools.converters.plovasp.vaspio import VaspData
-    import triqs_dft_tools.converters.plovasp.converter as plo_converter
-except ImportError:
-    pass
+from triqs_dft_tools.converters.vasp import VaspConverter
+from triqs_dft_tools.converters.plovasp.vaspio import VaspData
+import triqs_dft_tools.converters.plovasp.converter as plo_converter
 
 from solid_dmft.dmft_cycle import dmft_cycle
 from solid_dmft.dft_managers import vasp_manager as vasp
 from solid_dmft.dft_managers import qe_manager as qe
 
 def _run_plo_converter(general_params):
     if not mpi.is_master_node():
@@ -92,148 +89,42 @@
 
     # Checks if creating of rot_mat succeeded
     if mpi.is_master_node():
         with HDFArchive(seedname+'.h5', 'r') as archive:
             assert archive['dft_input']['use_rotations'], 'Creation of rot_mat failed in W90 converter'
     mpi.barrier()
 
-def _run_qe(general_params, dft_params, iter_dmft, iteration_offset):
+def _full_qe_run(seedname, dft_params, mode):
+    assert mode in ('initial', 'restart', 'update')
+
     # runs a full iteration of DFT
-    start_qe = lambda n_cores, calc_type: qe.start(n_cores, calc_type, dft_params['dft_exec'],
-                                                   dft_params['mpi_env'], general_params['seedname'])
+    qe_wrapper = lambda calc_type: qe.run(dft_params['n_cores'], calc_type, dft_params['dft_exec'],
+                                          dft_params['mpi_env'], seedname)
 
-    if iter_dmft == 1: # scf
-        qe_scf = start_qe(dft_params['n_cores'], 'scf')
-    else: # use modified scf
-
-        # if calculation is restarted, need to check in first iteration if DFT step needs to be skipped
-        iter_one_shot = (iter_dmft - 1 - general_params['n_iter_dmft_first'])%general_params['n_iter_dmft_per']
-        if iteration_offset > 0 and iter_dmft == iteration_offset + 1 and iter_one_shot > 0:
-            mpi.report('  solid_dmft: ...skipping DFT step')
-            return
+    # Initially run an scf calculation
+    if mode == 'initial':
+        qe_wrapper('scf')
+    # For charge update, use mode scf
+    elif mode == 'update':
+        qe_wrapper('mod_scf')
 
-        qe_scf = start_qe(dft_params['n_cores'], 'mod_scf')
-    # optionally do bnd, bands, proj if files are present
+    # Rest is executed regardless of mode
+    # Optionally does bnd, bands, proj if files are present
     for nscf in ['bnd', 'bands', 'proj']:
-        if os.path.isfile(f'{general_params["seedname"]}.{nscf}.in'):
-            qe_nscf = start_qe(dft_params['n_cores'], nscf)
+        if os.path.isfile(f'{seedname}.{nscf}.in'):
+            qe_wrapper(nscf)
+
     # nscf
-    qe_nscf = start_qe(dft_params['n_cores'], 'nscf')
+    qe_wrapper('nscf')
     # w90 parts
-    qe_w90 = start_qe(dft_params['n_cores'], 'win_pp')
-    qe_pw2wan = start_qe(dft_params['n_cores'], 'pw2wan')
-    qe_w90 = start_qe(dft_params['n_cores'], 'win')
-
-    # launch Wannier90Converter
-    _run_w90converter(general_params['seedname'], dft_params['w90_tolerance'])
-
-def read_dft_energy_vasp():
-    """
-    Reads DFT energy from the last line of Vasp's OSZICAR.
-    """
-    try:
-        with open('OSZICAR', 'r') as file:
-            nextline = file.readline()
-            while nextline.strip():
-                line = nextline
-                nextline = file.readline()
-        dft_energy = float(line.split()[2])
-    except FileNotFoundError:
-        print('OSZICAR not found, cannot read DFT energy')
-        return None
-    except ValueError:
-        print('Failed to read DFT energy from OSZICAR')
-        return None
-
-    print('DFT energy read from OSZICAR')
-    return dft_energy
-
-def read_dft_energy_qe(seedname):
-    """
-    Reads DFT energy from quantum espresso's seedname.scf.out.
-    """
-    RYDBERG = 13.605698066 # eV
-
-    for mode in ['mod_scf', 'scf']:
-        try:
-            with open(f'{seedname}.{mode}.out', 'r') as file:
-                dft_output = file.readlines()
-            for line in dft_output:
-                if 'total energy' in line:
-                    dft_energy = float(line.split()[-2]) * RYDBERG
-            break
-        except FileNotFoundError:
-            if mode == 'scf':
-                print(f'{seedname}.{mode}.out not found, cannot read DFT energy.')
-        except ValueError:
-            pass
-
-    print(f'DFT energy read from {seedname}.{mode}.out')
-    return dft_energy
-
-
-def _set_projections_suppressed(suppressed):
-    if mpi.is_master_node():
-        if suppressed:
-            print('  solid_dmft: Writing suppress projectors file', flush=True)
-            open('./vasp.suppress_projs', 'w').close()
-        elif os.path.isfile('./vasp.suppress_projs'):
-            print('  solid_dmft: Removing suppress projectors file', flush=True)
-            os.remove('./vasp.suppress_projs')
-    mpi.barrier()
+    qe_wrapper('win_pp')
+    qe_wrapper('pw2wan')
+    qe_wrapper('win')
+    _run_w90converter(seedname, dft_params['w90_tolerance'])
 
-def _read_irred_kpoints_from_vasp(general_params):
-    irred_indices = None
-    if mpi.is_master_node():
-        with HDFArchive(general_params['seedname'] + '.h5', 'r') as archive:
-            kpts = archive['dft_input/kpts']
-
-        def read_outcar(file):
-            has_started_reading = False
-            for line in file:
-                if 'IBZKPT_HF' in line:
-                    has_started_reading = True
-                    continue
-
-                if not has_started_reading:
-                    continue
-
-                if 't-inv' in line:
-                    yield line
-                    continue
-
-                if '-'*10 in line:
-                    break
-
-        with open('OUTCAR', 'r') as file:
-            outcar_data_raw = np.loadtxt(read_outcar(file), usecols=[0, 1, 2, 4])
-        outcar_kpoints = outcar_data_raw[:, :3]
-        outcar_indices = (outcar_data_raw[:, 3]-.5).astype(int)
-
-        symmetry_mapping = np.full(outcar_kpoints.shape[0], -1, dtype=int)
-
-        for i, (kpt_outcar, outcar_index) in enumerate(zip(outcar_kpoints, outcar_indices)):
-            for j, kpt in enumerate(kpts):
-                if np.allclose(kpt_outcar, kpt):
-                    # Symmetry-irreducible k points
-                    if i == outcar_index:
-                        symmetry_mapping[j] = outcar_index
-                    # Symmetry-reducible
-                    else:
-                        symmetry_mapping[j] = outcar_index
-                    break
-
-            # Asserts that loop left through break, i.e. a pair was found
-            assert np.allclose(kpt_outcar, kpt)
-
-        irreds, irred_indices = np.unique(symmetry_mapping, return_index=True)
-        assert np.all(np.diff(irreds) == 1)
-        assert np.all(symmetry_mapping >= 0)
-
-    return mpi.bcast(irred_indices)
 
 def _store_dft_eigvals(path_to_h5, iteration, projector_type):
     """
     save the eigenvalues from LOCPROJ/wannier90 file to h5 archive
     """
     with HDFArchive(path_to_h5, 'a') as archive:
         if 'dft_eigvals' not in archive:
@@ -248,161 +139,230 @@
             n_k = archive['dft_input']['n_k']
             num_ks_bands = archive['dft_input']['n_orbitals'][0, 0]
             eigenvals = np.loadtxt('wannier90.eig', usecols=2)
             eigenvals = eigenvals.reshape((n_k, num_ks_bands)) - fermi_energy
 
         archive['dft_eigvals']['it_'+str(iteration)] = eigenvals
 
+def _full_vasp_run(general_params, dft_params, initial_run, n_iter_dft=1, sum_k=None):
+    """
+    Performs a complete DFT cycle in Vasp and the correct converter. If
+    initial_run, Vasp is starting and performing a normal scf calculation
+    followed by a converter run. Otherwise, it performs n_iter_dft runs of DFT,
+    generating the projectors with the converter, and recalculating the charge
+    density correction with the new projectors.
+
+    Parameters
+    ----------
+    general_params : dict
+        general parameters as a dict
+    dft_params : dict
+        dft parameters as a dict
+    initial_run : bool
+        True when VASP is called for the first time. initial_run = True requires
+        n_iter_dft = 1.
+    n_iter_dft : int, optional
+        Number of DFT iterations to perform. The default is 1.
+    sum_k : SumkDFT, optional
+        The SumkDFT object required to recalculate the charge-density correction
+        if n_iter_dft > 1. The default is None.
+
+    Returns
+    -------
+    vasp_process_id : int
+        The process ID of the forked VASP process.
+    irred_indices : np.array
+        Integer indices of kpts in the irreducible Brillouin zone. Only needed
+        for Wannier projectors, which are normally run with symmetries.
+    """
+
+
+    if initial_run:
+        assert n_iter_dft == 1
+    else:
+        assert n_iter_dft == 1 or sum_k is not None, 'Sumk object needed to run multiple DFT iterations'
+
+    for i in range(n_iter_dft):
+        if initial_run:
+            vasp_process_id = vasp.run_initial_scf(dft_params['n_cores'], dft_params['dft_exec'],
+                                                   dft_params['mpi_env'])
+        else:
+            vasp_process_id = None
+            vasp.run_charge_update()
+
+        if dft_params['projector_type'] == 'plo':
+            _run_plo_converter(general_params)
+            irred_indices = None
+        elif dft_params['projector_type'] == 'w90':
+            _run_wannier90(general_params, dft_params)
+            mpi.barrier()
+            _run_w90converter(general_params['seedname'], dft_params['w90_tolerance'])
+            mpi.barrier()
+            kpts = None
+            if mpi.is_master_node():
+                with HDFArchive(general_params['seedname']+'.h5', 'r') as archive:
+                    kpts = archive['dft_input/kpts']
+            irred_indices = vasp.read_irred_kpoints(kpts)
+
+        # No need for recalculation of density correction if we run DMFT next
+        if i == n_iter_dft - 1:
+            break
+
+        # Recalculates the density correction
+        # Reads in new projectors and hopping and updates chemical potential
+        # rot_mat is not updated since it's more closely related to the local problem than DFT
+        # New fermi weights are directly read in calc_density_correction
+        mpi.barrier()
+        if mpi.is_master_node():
+            with HDFArchive(general_params['seedname']+'.h5', 'r') as archive:
+                sum_k.proj_mat = archive['dft_input/proj_mat']
+                sum_k.hopping = archive['dft_input/hopping']
+        sum_k.proj_mat = mpi.bcast(sum_k.proj_mat)
+        sum_k.hopping = mpi.bcast(sum_k.hopping)
+        sum_k.calc_mu(precision=general_params['prec_mu'])
+
+        # Writes out GAMMA file
+        sum_k.calc_density_correction(dm_type='vasp',  kpts_to_write=irred_indices)
+
+    return vasp_process_id, irred_indices
+
+
 # Main CSC flow method
 def csc_flow_control(general_params, solver_params, dft_params, advanced_params):
     """
-    function to run the csc cycle. It writes and removes the vasp.lock file to
+    Function to run the csc cycle. It writes and removes the vasp.lock file to
     start and stop Vasp, run the converter, run the dmft cycle and abort the job
     if all iterations are finished.
 
     Parameters
     ----------
     general_params : dict
         general parameters as a dict
     solver_params : dict
         solver parameters as a dict
     dft_params : dict
         dft parameters as a dict
     advanced_params : dict
         advanced parameters as a dict
-
-    Returns
-    -------
-    nothing
-
     """
 
-    iter_dft = 0
-    irred_indices = None
-    if dft_params['dft_code'] == 'vasp':
-        # if GAMMA file already exists, load it by doing extra DFT iterations
-        if os.path.exists('GAMMA'):
-            iter_dft = -dft_params['n_iter']
-            mpi.barrier()
+    # Removes legacy file vasp.suppress_projs if present
+    vasp.remove_legacy_projections_suppressed()
 
-        vasp_process_id = vasp.start(dft_params['n_cores'], dft_params['dft_exec'],
-                                     dft_params['mpi_env'])
-        # Removes projection suppression file if present
-        _set_projections_suppressed(False)
-        mpi.report('  solid_dmft: Waiting for VASP to start (lock appears)...')
-        while not vasp.is_lock_file_present():
-            time.sleep(1)
+    # if GAMMA file already exists, load it by doing extra DFT iterations
+    if dft_params['dft_code'] == 'vasp' and os.path.exists('GAMMA'):
+        # TODO: implement
+        raise NotImplementedError('GAMMA file found but restarting from updated '
+                                  + 'charge density not yet implemented for Vasp.')
 
     # Reads in iteration offset if restarting
     iteration_offset = 0
     if mpi.is_master_node() and os.path.isfile(general_params['seedname']+'.h5'):
         with HDFArchive(general_params['seedname']+'.h5', 'r') as archive:
             if 'DMFT_results' in archive and 'iteration_count' in archive['DMFT_results']:
                 iteration_offset = archive['DMFT_results']['iteration_count']
     iteration_offset = mpi.bcast(iteration_offset)
 
     iter_dmft = iteration_offset+1
-    start_time_dft = timer()
-    while iter_dmft <= general_params['n_iter_dmft'] + iteration_offset:
-        mpi.report('  solid_dmft: Running {}...'.format(dft_params['dft_code'].upper()))
-        mpi.barrier()
 
-        # vasp dft run
-        if dft_params['dft_code'] == 'vasp':
-            while vasp.is_lock_file_present():
-                time.sleep(1)
-        # qe dft run
-        elif dft_params['dft_code'] == 'qe':
-            _run_qe(general_params, dft_params, iter_dmft, iteration_offset)
-
-        # check if we should do another DFT iteration or go on with DMFT
-        iter_dft += 1
-        if dft_params['dft_code'] == 'vasp' and ((iter_dft-1) % dft_params['n_iter'] != 0 or iter_dft < 0):
-            suppressed = iter_dft%dft_params['n_iter'] != 0 or iter_dft+1 < 0
-            _set_projections_suppressed(suppressed)
-            vasp.reactivate()
-            continue
+    # Runs DFT once and converter
+    mpi.barrier()
+    irred_indices = None
+    start_time_dft = timer()
+    mpi.report('  solid_dmft: Running {}...'.format(dft_params['dft_code'].upper()))
 
-        end_time_dft = timer()
-        mpi.report('  solid_dmft: DFT cycle took {:10.4f} seconds'.format(end_time_dft-start_time_dft))
+    if dft_params['dft_code'] == 'qe':
+        if iteration_offset == 0:
+            _full_qe_run(general_params['seedname'], dft_params, 'initial')
+        else:
+            _full_qe_run(general_params['seedname'], dft_params, 'restart')
+    elif dft_params['dft_code'] == 'vasp':
+        vasp_process_id, irred_indices = _full_vasp_run(general_params, dft_params, True)
 
-        if dft_params['dft_code'] == 'vasp':
-            # Runs the converter
-            if dft_params['projector_type'] == 'plo':
-                _run_plo_converter(general_params)
-            elif dft_params['projector_type'] == 'w90':
-                _run_wannier90(general_params, dft_params)
-                mpi.barrier()
-                _run_w90converter(general_params['seedname'], dft_params['w90_tolerance'])
-                mpi.barrier()
-                irred_indices = _read_irred_kpoints_from_vasp(general_params)
-                mpi.barrier()
+    mpi.barrier()
+    end_time_dft = timer()
+    mpi.report('  solid_dmft: DFT cycle took {:10.3f} seconds'.format(end_time_dft-start_time_dft))
 
-        # Writes eigenvals to archive if requested
+    # Now that everything is ready, starts DFT+DMFT loop
+    while True:
         dft_energy = None
         if mpi.is_master_node():
-            # TODO: not yet compatible with dft_code = qe
+            # Writes eigenvals to archive if requested
             if dft_params['store_eigenvals']:
+                if dft_params['dft_code'] == 'qe':
+                    # TODO: implement
+                    raise NotImplementedError('store_eigenvals not yet compatible with dft_code = qe')
                 _store_dft_eigvals(path_to_h5=general_params['seedname']+'.h5',
                                    iteration=iter_dmft,
                                    projector_type=dft_params['projector_type'])
 
+            # Reads the DFT energy
             if dft_params['dft_code'] == 'vasp':
-                dft_energy = read_dft_energy_vasp()
+                dft_energy = vasp.read_dft_energy()
             elif dft_params['dft_code'] == 'qe':
-                dft_energy = read_dft_energy_qe(general_params['seedname'])
+                dft_energy = qe.read_dft_energy(general_params['seedname'], iter_dmft)
         dft_energy = mpi.bcast(dft_energy)
 
         if mpi.is_master_node():
             print('\n' + '='*80)
             print('Calling dmft_cycle')
             print('DMFT iteration {} / {}'.format(iter_dmft,
                                                   general_params['n_iter_dmft']+iteration_offset))
             print('='*80 + '\n')
 
         if mpi.is_master_node():
             start_time_dmft = timer()
 
-        # Determines number of steps
+        # Determines number of DMFT steps
         if iter_dmft == 1:
             iter_one_shot = general_params['n_iter_dmft_first']
         elif iteration_offset > 0 and iter_dmft == iteration_offset + 1:
             iter_one_shot = general_params['n_iter_dmft_per'] - (iter_dmft - 1
                             - general_params['n_iter_dmft_first'])%general_params['n_iter_dmft_per']
         else:
             iter_one_shot = general_params['n_iter_dmft_per']
         # Maximum total number of iterations is n_iter_dmft+iteration_offset
         iter_one_shot = min(iter_one_shot,
                             general_params['n_iter_dmft'] + iteration_offset - iter_dmft + 1)
 
         ############################################################
         # run the dmft_cycle
-        is_converged = dmft_cycle(general_params, solver_params, advanced_params,
-                                  dft_params, iter_one_shot, irred_indices, dft_energy)
+        is_converged, sum_k = dmft_cycle(general_params, solver_params, advanced_params,
+                                         dft_params, iter_one_shot, irred_indices, dft_energy)
         ############################################################
 
         iter_dmft += iter_one_shot
 
         if mpi.is_master_node():
             end_time_dmft = timer()
             print('\n' + '='*80)
-            print('DMFT cycle took {:10.4f} seconds'.format(end_time_dmft-start_time_dmft))
+            print('DMFT cycle took {:10.3f} seconds'.format(end_time_dmft-start_time_dmft))
             print('='*80 + '\n')
 
-        if is_converged:
+        # If all steps are executed or calculation is converged, finish DFT+DMFT loop
+        if is_converged or iter_dmft > general_params['n_iter_dmft'] + iteration_offset:
             break
 
-        # Reactivates Vasp if we do another run
-        if iter_dmft <= general_params['n_iter_dmft'] + iteration_offset:
-            mpi.barrier()
+        # Restarts DFT
+        mpi.barrier()
+        start_time_dft = timer()
+        mpi.report('  solid_dmft: Running {}...'.format(dft_params['dft_code'].upper()))
 
-            start_time_dft = timer()
-            if dft_params['dft_code'] == 'vasp':
-                _set_projections_suppressed(dft_params['n_iter'] > 1)
-                mpi.report('  solid_dmft: Reactivating VASP')
-                vasp.reactivate()
+        # Runs DFT and converter
+        if dft_params['dft_code'] == 'qe':
+            _full_qe_run(general_params['seedname'], dft_params, 'update')
+        elif dft_params['dft_code'] == 'vasp':
+            # Determines number of DFT steps
+            if iter_dmft == general_params['n_iter_dmft_first'] + 1:
+                n_iter_dft = dft_params['n_iter_first']
+            else:
+                n_iter_dft = dft_params['n_iter']
+            _, irred_indices = _full_vasp_run(general_params, dft_params, False, n_iter_dft, sum_k)
 
-    # Stops after maximum number of dmft iterations or convergence
-    if mpi.is_master_node():
-        print('  solid_dmft: Stopping {}\n'.format(dft_params['dft_code'].upper()), flush=True)
-        if dft_params['dft_code'] == 'vasp':
-            vasp.kill(vasp_process_id)
+        mpi.barrier()
+        end_time_dft = timer()
+        mpi.report('  solid_dmft: DFT cycle took {:10.3f} seconds'.format(end_time_dft-start_time_dft))
+
+    # Kills background VASP process for clean end
+    if mpi.is_master_node() and dft_params['dft_code'] == 'vasp':
+        print('  solid_dmft: Stopping VASP\n', flush=True)
+        vasp.kill(vasp_process_id)
```

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dft_managers/__init__.py` & `solid_dmft-3.1.5/python/solid_dmft/dft_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dft_managers/qe_manager.py` & `solid_dmft-3.1.5/python/solid_dmft/dft_managers/qe_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 # You should have received a copy of the GNU General Public License along with
 # solid_dmft (in the file COPYING.txt in this directory). If not, see
 # <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 
 """
-Contains the handling of the QE process. It can start QE, reactivate it,
-check if the lock file is there and finally kill QE. Needed for CSC calculations.
+Contains the function to run a QuantumEspresso iteration. Needed for CSC calculations.
 """
 
 import os
 import socket
 from collections import defaultdict
 import subprocess
 import shlex
@@ -145,83 +144,89 @@
 
     if cluster_name == 'daint':
         return [mpi_exe, '-launcher', 'ssh', '-hostfile', hostfile,
                 '-np', str(number_cores), '-envlist', 'PATH'] + shlex.split(qe_exec)
 
     return None
 
-def _fork_and_start_qe(mpi_exe, arguments, env_vars, seedname):
+def _poll_barrier(comm, poll_interval = 0.1):
+    """
+    Use asynchronous synchronization, otherwise mpi.barrier uses up all the CPU time during
+    the run of subprocess.
+
+    Parameters
+    ----------
+    comm: MPI communicator
+    poll_interval: float, time step for pinging the status of the sleeping ranks
     """
-    Forks a process from the master process that then calls mpi to start vasp.
-    The child process running VASP never leaves this function whereas the main
-    process returns the child's process id and continues.
+
+    req = comm.Ibarrier()
+    while not req.Test():
+        time.sleep(poll_interval)
+
+def _start_with_piping(mpi_exe, mpi_arguments, qe_file_ext, env_vars, seedname):
+    """
+    Handles the piping of the output when starting QE.
 
     Parameters
     ----------
     mpi_exe: string, mpi command
-    arguments: list of string, arguments to start mpi with
+    mpi_arguments: list of string, arguments to start mpi with
+    qe_file_ext : string, file name for QE
     env_vars: dict of string, environment variables containing PATH
     seedname: string, QE input file
 
     Returns
     -------
     int: id of the VASP child process
     """
 
-    mpi_arguments, qe_file_ext = arguments[0], arguments[1]
-
     if qe_file_ext in ['scf', 'nscf', 'pw2wan', 'mod_scf', 'bnd', 'bands', 'proj']:
 
         inp = open(f'{seedname}.{qe_file_ext}.in', 'r')
         out = open(f'{seedname}.{qe_file_ext}.out','w')
         err = open(f'{seedname}.{qe_file_ext}.err','w')
 
         print('  solid_dmft: Starting {} calculation...'.format(qe_file_ext))
 
         # start subprocess
-        qe_process_id = subprocess.run(mpi_arguments, stdin=inp, env=env_vars, capture_output=True,
-                                       text=True, shell=False)
+        qe_result = subprocess.run(mpi_arguments, stdin=inp, env=env_vars, capture_output=True,
+                                   text=True, shell=False)
 
         # write output and error file
-        output = qe_process_id.stdout
-        error = qe_process_id.stderr
+        output = qe_result.stdout
+        error = qe_result.stderr
         out.writelines(output)
         err.writelines(error)
 
-        if qe_process_id.returncode != 0:
+        if qe_result.returncode != 0:
             mpi.report('QE calculation failed. Exiting programm.')
             sys.exit(1)
 
     elif 'win' in qe_file_ext:
-
         print('  solid_dmft: Starting Wannier90 {}...'.format(qe_file_ext))
-
         # don't need any piping for Wannier90
-        qe_process_id = subprocess.check_call(mpi_arguments + [seedname], env=env_vars, shell=False)
-
-    return qe_process_id
+        subprocess.check_call(mpi_arguments + [seedname], env=env_vars, shell=False)
 
 
-def start(number_cores, qe_file_ext, qe_exec, cluster_name, seedname):
+def run(number_cores, qe_file_ext, qe_exec, mpi_profile, seedname):
     """
     Starts the VASP child process. Takes care of initializing a clean
     environment for the child process. This is needed so that VASP does not
     get confused with all the standard slurm environment variables.
 
     Parameters
     ----------
     number_cores: int, the number of cores that vasp runs on
     vasp_command: string, the command to start vasp
     cluster_name: string, name of the cluster so that settings can be tailored to it
     """
 
     # get MPI env
-    qe_process_id = 0
-
-    hostfile = _create_hostfile(number_cores, cluster_name)
+    hostfile = _create_hostfile(number_cores, mpi_profile)
     qe_exec_path = qe_exec.strip(qe_exec.rsplit('/')[-1])
     qe_exec = qe_exec_path
 
     if mpi.is_master_node():
         # clean environment
         env_vars = {}
         for var_name in ['PATH', 'LD_LIBRARY_PATH', 'SHELL', 'PWD', 'HOME',
@@ -242,30 +247,65 @@
         elif qe_file_ext in ['proj']:
             qe_exec += f'projwfc.x -nk {number_cores}'
         elif qe_file_ext in ['win_pp']:
             qe_exec += 'wannier90.x -pp'
         elif qe_file_ext in ['win']:
             qe_exec += 'wannier90.x'
 
-        arguments = _get_mpi_arguments(cluster_name, mpi_exe, number_cores, qe_exec, hostfile)
-        qe_process_id = _fork_and_start_qe(mpi_exe, (arguments, qe_file_ext), env_vars, seedname)
-
-    poll_barrier(mpi.MPI.COMM_WORLD)
-    qe_process_id = mpi.bcast(qe_process_id)
+        arguments = _get_mpi_arguments(mpi_profile, mpi_exe, number_cores, qe_exec, hostfile)
+        _start_with_piping(mpi_exe, arguments, qe_file_ext, env_vars, seedname)
 
-    return qe_process_id
-
-
-def poll_barrier(comm, poll_interval = 0.1):
-    """
-    Use asynchronous synchronization, otherwise mpi.barrier uses up all the CPU time during
-    the run of subprocess.
+    _poll_barrier(mpi.MPI.COMM_WORLD)
 
-    Parameters
-    ----------
-    comm: MPI communicator
-    poll_interval: float, time step for pinging the status of the sleeping ranks
+def read_dft_energy(seedname, iter_dmft):
     """
+    Reads DFT energy from quantum espresso's out files
 
-    req = comm.Ibarrier()
-    while not req.Test():
-        time.sleep(poll_interval)
+    1. At the first iteration, the DFT energy is read from the scf file.
+
+    2. After the first iteration the band energy computed in the mod_scf calculation is wrong,
+       and needs to be subtracted from the reported total energy. The correct band energy
+       is computed in the nscf calculation.
+
+    """
+    dft_energy = 0.0
+    RYDBERG = 13.605693123 # eV
+
+    if iter_dmft == 1:
+        with open(f'{seedname}.scf.out', 'r') as file:
+            dft_output = file.readlines()
+        for line in dft_output:
+            if '!' in line:
+                print("\nReading total energy from the scf calculation \n")
+                dft_energy = float(line.split()[-2]) * RYDBERG
+                print(f"The DFT energy is: {dft_energy} eV")
+                break
+            if  line =="":
+                raise EOFError("Did not find scf total energy")
+    else:
+        with open(f'{seedname}.mod_scf.out', 'r') as file:
+            dft_output = file.readlines()
+        for line in dft_output:
+            #if 'eband, Ef (eV)' in line:
+            if "(sum(wg*et))" in line:
+                print("\nReading band energy from the mod_scf calculation \n")
+                #band_energy = float(line.split())
+                band_energy_modscf = float(line.split()[-2])*RYDBERG
+                print(f"The mod_scf band energy is: {band_energy_modscf} eV")
+            if 'total energy' in line:
+                print("\nReading total energy from the mod_scf calculation \n")
+                dft_energy = float(line.split()[-2]) * RYDBERG
+                print(f"The uncorrected DFT energy is: {dft_energy} eV")
+        dft_energy -= band_energy_modscf
+        print(f"The DFT energy without kinetic part is: {dft_energy} eV")
+
+        with open(f'{seedname}.nscf.out', 'r') as file:
+            dft_output = file.readlines()
+        for line in dft_output:
+            if 'The nscf band energy' in line:
+                print("\nReading band energy from the nscf calculation\n")
+                band_energy_nscf = float(line.split()[-2]) * RYDBERG
+                dft_energy += band_energy_nscf
+                print(f"The nscf band energy is: {band_energy_nscf} eV")
+                print(f"The corrected DFT energy is: {dft_energy} eV")
+                break
+    return dft_energy
```

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dft_managers/vasp_manager.py` & `solid_dmft-3.1.5/python/solid_dmft/dft_managers/vasp_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,20 +23,23 @@
 # <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 
 """
 Contains the handling of the VASP process. It can start VASP, reactivate it,
 check if the lock file is there and finally kill VASP. Needed for CSC calculations.
+
+This functionality is contained in the simpler public functions.
 """
 
 import os
 import socket
 import signal
-from collections import defaultdict
+import time
+import numpy as np
 
 import triqs.utility.mpi as mpi
 
 
 def _create_hostfile(number_cores, cluster_name):
     """
     Writes a host file for the mpirun. This tells mpi which nodes to ssh into
@@ -179,30 +182,53 @@
         os.execve(mpi_exe, arguments, env_vars)
         print('\n VASP exec failed\n')
         os._exit(127)
 
     return vasp_process_id
 
 
-def start(number_cores, vasp_command, cluster_name):
+def _is_lock_file_present():
+    """
+    Checks if the lock file 'vasp.lock' is there, i.e. if VASP is still working.
+    """
+
+    res_bool = False
+    if mpi.is_master_node():
+        res_bool = os.path.isfile('./vasp.lock')
+    res_bool = mpi.bcast(res_bool)
+    return res_bool
+
+
+def remove_legacy_projections_suppressed():
+    """ Removes legacy file vasp.suppress_projs if present. """
+    if mpi.is_master_node():
+        if os.path.isfile('./vasp.suppress_projs'):
+            print('  solid_dmft: Removing legacy file vasp.suppress_projs', flush=True)
+            os.remove('./vasp.suppress_projs')
+    mpi.barrier()
+
+
+def run_initial_scf(number_cores, vasp_command, cluster_name):
     """
     Starts the VASP child process. Takes care of initializing a clean
     environment for the child process. This is needed so that VASP does not
-    get confused with all the standard slurm environment variables.
+    get confused with all the standard slurm environment variables. Returns when
+    VASP has completed its initial scf cycle.
 
     Parameters
     ----------
     number_cores: int, the number of cores that vasp runs on
     vasp_command: string, the command to start vasp
     cluster_name: string, name of the cluster so that settings can be tailored to it
     """
 
     # Removes STOPCAR
     if mpi.is_master_node() and os.path.isfile('STOPCAR'):
         os.remove('STOPCAR')
+    mpi.barrier()
 
     # get MPI env
     vasp_process_id = 0
 
     hostfile = _create_hostfile(number_cores, cluster_name)
 
     if mpi.is_master_node():
@@ -220,35 +246,105 @@
         arguments = _get_mpi_arguments(cluster_name, mpi_exe, number_cores, vasp_command, hostfile)
         vasp_process_id = _fork_and_start_vasp(mpi_exe, arguments, env_vars)
 
 
     mpi.barrier()
     vasp_process_id = mpi.bcast(vasp_process_id)
 
+    # Waits for VASP to start
+    while not _is_lock_file_present():
+        time.sleep(1)
+    mpi.barrier()
+
+    # Waits for VASP to finish
+    while _is_lock_file_present():
+        time.sleep(1)
+    mpi.barrier()
+
     return vasp_process_id
 
 
-def reactivate():
-    """ Reactivates VASP by creating the vasp.lock file. """
+def run_charge_update():
+    """
+    Performs one step of the charge update with VASP by creating the vasp.lock
+    file and then waiting until it gets delete by VASP when it has finished.
+    """
     if mpi.is_master_node():
         open('./vasp.lock', 'a').close()
     mpi.barrier()
 
+    # Waits for VASP to finish
+    while _is_lock_file_present():
+        time.sleep(1)
+    mpi.barrier()
+
 
-def is_lock_file_present():
+def read_dft_energy():
     """
-    Checks if the lock file 'vasp.lock' is there, i.e. if VASP is still working.
+    Reads DFT energy from the last line of Vasp's OSZICAR.
     """
+    with open('OSZICAR', 'r') as file:
+        nextline = file.readline()
+        while nextline.strip():
+            line = nextline
+            nextline = file.readline()
+    dft_energy = float(line.split()[2])
 
-    res_bool = False
+    return dft_energy
+
+
+def read_irred_kpoints(kpts):
+    """ Reads the indices of the irreducible k-points from the OUTCAR. """
+
+    def read_outcar(file):
+        has_started_reading = False
+        for line in file:
+            if 'IBZKPT_HF' in line:
+                has_started_reading = True
+                continue
+
+            if not has_started_reading:
+                continue
+
+            if 't-inv' in line:
+                yield line
+                continue
+
+            if '-'*10 in line:
+                break
+
+    irred_indices = None
     if mpi.is_master_node():
-        res_bool = os.path.isfile('./vasp.lock')
-    mpi.barrier()
-    res_bool = mpi.bcast(res_bool)
-    return res_bool
+        with open('OUTCAR', 'r') as file:
+            outcar_data_raw = np.loadtxt(read_outcar(file), usecols=[0, 1, 2, 4])
+        outcar_kpoints = outcar_data_raw[:, :3]
+        outcar_indices = (outcar_data_raw[:, 3]-.5).astype(int)
+        assert np.allclose(outcar_kpoints, kpts)
+
+        symmetry_mapping = np.full(outcar_kpoints.shape[0], -1, dtype=int)
+
+        for i, (kpt_outcar, outcar_index) in enumerate(zip(outcar_kpoints, outcar_indices)):
+            for j, kpt in enumerate(kpts):
+                if np.allclose(kpt_outcar, kpt):
+                    # Symmetry-irreducible k points
+                    if i == outcar_index:
+                        symmetry_mapping[j] = outcar_index
+                    # Symmetry-reducible
+                    else:
+                        symmetry_mapping[j] = outcar_index
+                    break
+
+            # Asserts that loop left through break, i.e. a pair was found
+            assert np.allclose(kpt_outcar, kpt)
+
+        irreds, irred_indices = np.unique(symmetry_mapping, return_index=True)
+        assert np.all(np.diff(irreds) == 1)
+        assert np.all(symmetry_mapping >= 0)
+
+    return mpi.bcast(irred_indices)
 
 
 def kill(vasp_process_id):
     """ Kills the VASP process. """
     # TODO: if we kill the process in the next step, does it make a difference if we write the STOPCAR
     with open('STOPCAR', 'wt') as f_stop:
         f_stop.write('LABORT = .TRUE.\n')
```

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_cycle.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_cycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -577,26 +577,21 @@
                                                         h_int, archive, shell_multiplicity, E_kin_dft,
                                                         observables, conv_obs, Op_list, dft_irred_kpt_indices, dft_energy,
                                                         is_converged=True, is_sampling=True)
 
         mpi.report('** Sampling finished ***')
         mpi.report('#'*80)
 
-    # for one-shot calculations, we can use the updated GAMMA file for postprocessing
-    if not general_params['csc'] and general_params['oneshot_postproc_gamma_file']:
-        # Write the density correction to file after the one-shot calculation
-        sum_k.calc_density_correction(filename=os.path.join(general_params['jobname'], 'GAMMA'), dm_type='vasp')
-
     mpi.barrier()
 
     # close the h5 archive
     if mpi.is_master_node():
         del archive
 
-    return is_converged
+    return is_converged, sum_k
 
 
 def _dmft_step(sum_k, solvers, it, general_params,
                solver_params, advanced_params, dft_params,
                h_int, archive, shell_multiplicity, E_kin_dft,
                observables, conv_obs, Op_list, dft_irred_kpt_indices, dft_energy,
                is_converged, is_sampling):
@@ -730,25 +725,19 @@
     previous_mu = sum_k.chemical_potential
     sum_k = manipulate_mu.update_mu(general_params, sum_k, it, archive)
 
     # if we do a CSC calculation we need always an updated GAMMA file
     E_bandcorr = 0.0
     if general_params['csc']:
         # handling the density correction for fcsc calculations
-        # TODO: keep only code in "else", the rest is redundant with handling inside
-        #     sum_k.calc_density_correction. Code in "if" only implemented for
-        #     compatibility with last official dft_tools release
         if dft_params['dft_code'] == 'vasp':
-            if dft_irred_kpt_indices is None:
-                deltaN, dens, E_bandcorr = sum_k.calc_density_correction(filename='GAMMA', dm_type='vasp')
-            else:
-                deltaN, dens, E_bandcorr = sum_k.calc_density_correction(filename='GAMMA', dm_type='vasp',
-                                                                         kpts_to_write=dft_irred_kpt_indices)
+            deltaN, dens, E_bandcorr = sum_k.calc_density_correction(dm_type='vasp',
+                                                                     kpts_to_write=dft_irred_kpt_indices)
         elif dft_params['dft_code'] == 'qe':
-            deltaN, dens, E_bandcorr = sum_k.calc_density_correction(dm_type=dft_params['dft_code'])
+            deltaN, dens, E_bandcorr = sum_k.calc_density_correction(dm_type='qe')
 
     # for a one shot calculation we are using our own method
     if not general_params['csc'] and general_params['calc_energies']:
         E_bandcorr = calc_bandcorr_man(general_params, sum_k, E_kin_dft)
 
     if general_params['csc']:
         results_to_archive.write(archive, sum_k, general_params, solver_params, solvers, it,
```

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_tools/__init__.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_tools/afm_mapping.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_tools/afm_mapping.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_tools/convergence.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_tools/convergence.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_tools/formatter.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_tools/formatter.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_tools/greens_functions_mixer.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_tools/greens_functions_mixer.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_tools/initial_self_energies.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_tools/initial_self_energies.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_tools/interaction_hamiltonian.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_tools/interaction_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_tools/legendre_filter.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_tools/legendre_filter.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_tools/manipulate_chemical_potential.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_tools/manipulate_chemical_potential.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_tools/observables.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_tools/observables.py`

 * *Files 1% similar despite different names*

```diff
@@ -594,21 +594,21 @@
     E_bandcorr = E_kin_dmft - E_kin_dft
 
     return E_bandcorr
 
 def calc_Z(Sigma):
     """
     calculates the inverse mass enhancement from the impurity
-    self-energy by a simple estimate:
-    [ 1 - (Im S_iw[n_iw0]/iw[n_iw0]) ]^-1
+    self-energy by a simple linear fit estimate:
+    [ 1 - ((Im S_iw[n_iw0+1]-S_iw[n_iw0])/(iw[n_iw0+1]-iw[n_iw0])) ]^-1
 
     Parameters
     ----------
-    dft_mu: Gf_Im_Freq
-        self-energy in Matsubara
+    Sigma: Gf on MeshImFreq
+        self-energy on Matsubara mesh
 
 
     Returns
     -------
     orb_Z: 1d numpy array
         list of Z values per orbital in Sigma
 
@@ -617,12 +617,13 @@
 
     iw = [np.imag(n) for n in Sigma.mesh]
     # find smallest iw_n
     n_iw0 = int(0.5*len(iw))
 
     for orb in range(0,Sigma.target_shape[0]):
         Im_S_iw = Sigma[orb,orb].data.imag
-        # simple extraction from S_iw_0
-        Z = 1/(1 - (Im_S_iw[n_iw0]/iw[n_iw0]) )
+        # simple extraction from linear fit to first two Matsubara freq of Sigma
+        # assuming Fermi liquid like self energy
+        Z = 1/(1 - (Im_S_iw[n_iw0+1]-Im_S_iw[n_iw0]) / (iw[n_iw0+1]-iw[n_iw0]) )
         orb_Z.append(abs(Z))
 
     return np.array(orb_Z)
```

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_tools/results_to_archive.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_tools/results_to_archive.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/dmft_tools/solver.py` & `solid_dmft-3.1.5/python/solid_dmft/dmft_tools/solver.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/main.py` & `solid_dmft-3.1.5/python/solid_dmft/main.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/postprocessing/__init__.py` & `solid_dmft-3.1.5/python/solid_dmft/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py` & `solid_dmft-3.1.5/python/solid_dmft/postprocessing/eval_U_cRPA_Vasp.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/postprocessing/maxent_gf_imp.py` & `solid_dmft-3.1.5/python/solid_dmft/postprocessing/maxent_gf_imp.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/postprocessing/maxent_gf_latt.py` & `solid_dmft-3.1.5/python/solid_dmft/postprocessing/maxent_gf_latt.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/postprocessing/maxent_sigma.py` & `solid_dmft-3.1.5/python/solid_dmft/postprocessing/maxent_sigma.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/postprocessing/plot_correlated_bands.py` & `solid_dmft-3.1.5/python/solid_dmft/postprocessing/plot_correlated_bands.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/read_config.py` & `solid_dmft-3.1.5/python/solid_dmft/read_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,16 +194,14 @@
             The program ensures that 0 <= factor <= 1.
             mu_mix_const = 1.0 and mu_mix_per_occupation_offset = 0.0 means no mixing.
 afm_order : bool, optional, default=False
             copy self energies instead of solving explicitly for afm order
 set_rot : string, optional, default='none'
             use density_mat_dft to diagonalize occupations = 'den'
             use hloc_dft to diagonalize occupations = 'hloc'
-oneshot_postproc_gamma_file : bool, optional, default=False
-            write the GAMMA file for vasp after completed one-shot calculations
 measure_chi_SzSz : bool, optional, default=False
             measure the dynamic spin suszeptibility chi(sz,sz(tau))
             triqs.github.io/cthyb/unstable/guide/dynamic_susceptibility_notebook.html
 measure_chi_insertions : int, optional, default=100
             number of insertation for measurement of chi
 mu_gap_gb2_threshold : float, optional, default=none
             Threshold of the absolute of the lattice GF at tau=beta/2 for use
@@ -265,14 +263,18 @@
 fit_max_w : float, optional
             highest matsubara frequency to fit
 random_seed : int, optional default by triqs
             if specified the int will be used for random seeds! Careful, this will give the same random
             numbers on all mpi ranks
 legendre_fit : bool, optional default= False
             filter noise of G(tau) with G_l, cutoff is taken from n_l
+loc_n_min : int, optional
+            Restrict local Hilbert space to states with at least this number of particles
+loc_n_max : int, optional
+            Restrict local Hilbert space to states with at most this number of particles
 
 ftps parameters
 ===============
 n_bath :     int
             number of bath sites
 bath_fit :   bool, default=False
             DiscretizeBath vs BathFitter
@@ -329,25 +331,31 @@
             Possible values:
 
             * 'vasp'
             * 'qe'
 n_cores : int
             number of cores for the DFT code (VASP)
 n_iter : int, optional, default= 6
-            number of dft iterations per cycle
+            only needed for VASP. Number of DFT iterations to feed the DMFT
+            charge density into DFT, which generally takes multiple Davidson steps.
+            For every DFT iterations, the charge-density correction is recalculated
+            using newly generated projectors and hoppings from the previous DFT run
+n_iter_first : int, optional, default= dft/n_iter
+            number of DFT iterations in the first charge correction because this
+            first charge correction usually changes the DFT wave functions the most.
 dft_exec :  string, default= 'vasp_std'
-            command for the DFT / VASP executable
+            command for the DFT executable
 store_eigenvals : bool, optional, default= False
             stores the dft eigenvals from LOCPROJ (projector_type=plo) or
             wannier90.eig (projector_type=w90) file in h5 archive
 mpi_env : string, default= 'local'
             selection for mpi env for DFT / VASP in default this will only call VASP as mpirun -np n_cores_dft dft_exec
 projector_type : string, optional, default= 'plo'
             plo: uses VASP's PLO formalism, requires LOCPROJ in the INCAR
-            w90: uses Wannier90, requires LWANNIER90 in the INCAR
+            w90: uses Wannier90 (for VASP and QuantumEspresso)
 w90_exec :  string, default='wannier90.x'
             the command to start a single-core wannier run
 w90_tolerance :  float, default=1e-6
             threshold for mapping of shells and checks of the Hamiltonian
 
 [  advanced  ]
 --------------
@@ -559,17 +567,14 @@
                                                                   'valid for': lambda x, _: x > 0 or np.isclose(x, 0),
                                                                   'used': lambda params: params['general']['fixed_mu_value'] == 'none',
                                                                   'default': 0.},
 
                                  'set_rot': {'valid for': lambda x, _: x in ('none', 'den', 'hloc'),
                                              'used': True, 'default': 'none'},
 
-                                 'oneshot_postproc_gamma_file': {'converter': BOOL_PARSER,
-                                                                 'used': lambda params: not params['general']['csc'], 'default': False},
-
                                  'measure_chi': {'valid for': lambda x, _: x in ('SzSz', 'NN', 'none'), 'used': True, 'default': 'none'},
 
                                  'measure_chi_insertions': {'converter': int, 'used': True, 'default': 100},
 
                                  # TODO: used for which solvers? Generalize to real freq. solvers without maxent?
                                  'mu_gap_gb2_threshold': {'converter': float,
                                                           'valid for': lambda x, _: x == 'none' or x > 0 or np.isclose(x, 0),
@@ -586,35 +591,39 @@
                      'dft': {'dft_code': {'used': lambda params: params['general']['csc'],
                                           'valid for': lambda x, _: x in ('vasp', 'qe')},
 
                              'n_cores': {'converter': int, 'valid for': lambda x, _: x > 0,
                                          'used': lambda params: params['general']['csc']},
 
                              'n_iter': {'converter': int, 'valid for': lambda x, _: x > 0,
-                                        'used': lambda params: params['general']['csc'], 'default': 6},
+                                        'used': lambda params: params['general']['csc'] and params['dft']['dft_code'] == 'vasp',
+                                        'default': 4},
+
+                             'n_iter_first': {'converter': int, 'valid for': lambda x, _: x > 0,
+                                              'used': lambda params: params['general']['csc'] and params['dft']['dft_code'] == 'vasp',
+                                              'default': lambda params: params['dft']['n_iter']},
 
                              'dft_exec': {'used': lambda params: params['general']['csc'], 'default': 'vasp_std'},
 
                              'store_eigenvals': {'converter': BOOL_PARSER,
                                                  'used': lambda params: params['general']['csc'],
                                                  'default': False},
 
                              'mpi_env': {'valid for': lambda x, _: x in ('local', 'rusty', 'rusty-intra', 'rusty-ompi2', 'daint'),
                                          'used': lambda params: params['general']['csc'], 'default': 'local'},
 
-                             'projector_type': {'valid for': lambda x, _: x in ('plo', 'w90'),
+                             'projector_type': {'valid for': lambda x, params: x == 'w90' or x == 'plo' and params['dft']['dft_code'] == 'vasp',
                                                 'used': lambda params: params['general']['csc'], 'default': 'plo'},
 
                              'w90_exec': {'used': lambda params: (params['general']['csc']
-                                                                  and params['dft']['projector_type'] == 'w90'),
+                                                                  and params['dft']['dft_code'] == 'vasp' and params['dft']['projector_type'] == 'w90'),
                                                 'default': 'wannier90.x'},
 
                              'w90_tolerance': {'converter': lambda s: float(s),
-                                                'used': lambda params: (params['general']['csc']
-                                                                      and params['dft']['projector_type'] == 'w90'),
+                                                'used': lambda params: params['general']['csc'] and params['dft']['projector_type'] == 'w90',
                                                 'default': 1e-6},
                             },
                      'solver': {
                                 #
                                 'store_solver': {'converter': BOOL_PARSER, 'used': True, 'default': False},
                                 #
                                 # cthyb parameters
@@ -702,14 +711,23 @@
                                                       and params['general']['solver_type'] in ['cthyb'],
                                               'default': None},
 
                                 'legendre_fit': {'converter': BOOL_PARSER,
                                                  'used': lambda params: params['general']['solver_type'] in ['cthyb','ctseg'],
                                                  'default': False},
 
+                                'loc_n_min': {'converter': int, 'valid for': lambda x, _: x >= 0,
+                                              'used': lambda params: params['general']['solver_type'] in ['cthyb'],
+                                              'default': None},
+
+                                'loc_n_max': {'converter': int, 'valid for': lambda x, _: x >= 0,
+                                              'used': lambda params: params['general']['solver_type'] in ['cthyb'],
+                                              'default': None},
+
+
                                 #
                                 # extra ctseg params
                                 #
                                 'improved_estimator': {'converter': BOOL_PARSER,
                                                  'used': lambda params: params['general']['solver_type'] in ['ctseg'],
                                                  'default': False},
```

### Comparing `solid_dmft-3.1.4/python/solid_dmft/util/__init__.py` & `solid_dmft-3.1.5/python/solid_dmft/util/__init__.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/util/symmetrize_gamma_file.py` & `solid_dmft-3.1.5/python/solid_dmft/util/symmetrize_gamma_file.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/util/update_dmft_config.py` & `solid_dmft-3.1.5/python/solid_dmft/util/update_dmft_config.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/util/update_results_h5.py` & `solid_dmft-3.1.5/python/solid_dmft/util/update_results_h5.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/util/write_kslice_to_h5.py` & `solid_dmft-3.1.5/python/solid_dmft/util/write_kslice_to_h5.py`

 * *Files identical despite different names*

### Comparing `solid_dmft-3.1.4/python/solid_dmft/version.py` & `solid_dmft-3.1.5/python/solid_dmft/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 # You should have received a copy of the GNU General Public License along with
 # solid_dmft (in the file COPYING.txt in this directory). If not, see
 # <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 
-version = "3.1.4"
+version = "3.1.5"
 triqs_hash = "41574c923131900ddfab7c25a3ad4b5da93dcfdd"
 solid_dmft_hash = "707c012359758d3aca1ce46e3446312df86ca5d6"
 
 def show_version():
   print("\nYou are using solid_dmft version %s\n"%version)
 
 def show_git_hash():
```

### Comparing `solid_dmft-3.1.4/python/solid_dmft.egg-info/PKG-INFO` & `solid_dmft-3.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
-Name: solid-dmft
-Version: 3.1.4
+Name: solid_dmft
+Version: 3.1.5
 Summary: solid_dmft: a versatile python wrapper to perform DFT+DMFT calculations utilizing the TRIQS software library
 Author-email: Alexander Hampel <ahampel@flatironinstitute.org>
 Project-URL: Homepage, https://triqs.github.io/solid_dmft
 Project-URL: Bug Tracker, https://github.com/triqs/solid_dmft/issues
 Keywords: DMFT,DFT,triqs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+License-File: COPYING.txt
 
 ![logo_soliDMFT](https://raw.githubusercontent.com/triqs/solid_dmft/unstable/doc/logos/logo_solid_dmft.png)
 
 ![CI](https://github.com/triqs/solid_dmft/actions/workflows/build.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/solid_dmft.svg)](https://badge.fury.io/py/solid_dmft)
 [![status](https://joss.theoj.org/papers/48eb529b08c6bb464b235ba919d78922/status.svg)](https://joss.theoj.org/papers/48eb529b08c6bb464b235ba919d78922)
```

### Comparing `solid_dmft-3.1.4/python/solid_dmft.egg-info/SOURCES.txt` & `solid_dmft-3.1.5/python/solid_dmft.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+COPYING.txt
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 python/solid_dmft/__init__.py
 python/solid_dmft/csc_flow.py
 python/solid_dmft/dmft_cycle.py
```

