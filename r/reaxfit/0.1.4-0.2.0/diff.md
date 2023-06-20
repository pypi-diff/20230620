# Comparing `tmp/reaxfit-0.1.4.tar.gz` & `tmp/reaxfit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxfit-0.1.4.tar", last modified: Fri Jun  9 08:33:45 2023, max compression
+gzip compressed data, was "reaxfit-0.2.0.tar", last modified: Tue Jun 20 03:09:27 2023, max compression
```

## Comparing `reaxfit-0.1.4.tar` & `reaxfit-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.765588 reaxfit-0.1.4/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.761588 reaxfit-0.1.4/.github/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       48 2023-03-03 06:38:54.000000 reaxfit-0.1.4/.github/release.yml
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.761588 reaxfit-0.1.4/.github/workflows/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      251 2023-03-03 06:38:54.000000 reaxfit-0.1.4/.github/workflows/tagpr.yml
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      111 2023-04-12 04:40:21.000000 reaxfit-0.1.4/.gitignore
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     1794 2023-03-03 06:38:54.000000 reaxfit-0.1.4/.tagpr
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     1067 2023-03-01 01:38:22.000000 reaxfit-0.1.4/LICENSE
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-06-09 08:33:45.765588 reaxfit-0.1.4/PKG-INFO
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      732 2023-06-09 06:14:50.000000 reaxfit-0.1.4/README.md
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.761588 reaxfit-0.1.4/example/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.761588 reaxfit-0.1.4/example/CoCO/
--rw-r--r--   0 ykane     (1000) ykane     (1000)     1892 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/0.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2151 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/1.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/2.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/3.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/4.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/5.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/6.xyz
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      189 2023-02-28 13:43:09.000000 reaxfit-0.1.4/example/CoCO/batch.sh
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      374 2023-02-28 13:52:46.000000 reaxfit-0.1.4/example/CoCO/chk.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      260 2023-03-03 02:56:27.000000 reaxfit-0.1.4/example/CoCO/config.json
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2310 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/data0
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    22606 2023-06-09 06:14:50.000000 reaxfit-0.1.4/example/CoCO/ffield.reax
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    22677 2023-03-02 14:08:20.000000 reaxfit-0.1.4/example/CoCO/ffield.temp
--rw-r--r--   0 ykane     (1000) ykane     (1000)       58 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/refE
--rw-r--r--   0 ykane     (1000) ykane     (1000)       56 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/refF
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      127 2023-02-28 13:40:22.000000 reaxfit-0.1.4/example/CoCO/run.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      235 2023-03-01 02:14:34.000000 reaxfit-0.1.4/example/README.md
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    61858 2023-06-09 06:14:50.000000 reaxfit-0.1.4/reaxfit_sample.ipynb
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       38 2023-06-09 08:33:45.765588 reaxfit-0.1.4/setup.cfg
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      723 2023-06-09 06:14:50.000000 reaxfit-0.1.4/setup.py
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.757588 reaxfit-0.1.4/src/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.761588 reaxfit-0.1.4/src/reaxfit/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       30 2023-02-22 05:23:36.000000 reaxfit-0.1.4/src/reaxfit/__init__.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      160 2023-03-03 07:37:02.000000 reaxfit-0.1.4/src/reaxfit/_version.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     8849 2023-06-09 08:31:23.000000 reaxfit-0.1.4/src/reaxfit/reaxfit.py
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.765588 reaxfit-0.1.4/src/reaxfit.egg-info/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-06-09 08:33:45.000000 reaxfit-0.1.4/src/reaxfit.egg-info/PKG-INFO
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      667 2023-06-09 08:33:45.000000 reaxfit-0.1.4/src/reaxfit.egg-info/SOURCES.txt
--rw-rw-r--   0 ykane     (1000) ykane     (1000)        1 2023-06-09 08:33:45.000000 reaxfit-0.1.4/src/reaxfit.egg-info/dependency_links.txt
--rw-rw-r--   0 ykane     (1000) ykane     (1000)        8 2023-06-09 08:33:45.000000 reaxfit-0.1.4/src/reaxfit.egg-info/top_level.txt
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.239962 reaxfit-0.2.0/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.235962 reaxfit-0.2.0/.github/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       48 2023-03-03 06:38:54.000000 reaxfit-0.2.0/.github/release.yml
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.235962 reaxfit-0.2.0/.github/workflows/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      251 2023-03-03 06:38:54.000000 reaxfit-0.2.0/.github/workflows/tagpr.yml
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      111 2023-04-12 04:40:21.000000 reaxfit-0.2.0/.gitignore
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     1794 2023-03-03 06:38:54.000000 reaxfit-0.2.0/.tagpr
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     1067 2023-03-01 01:38:22.000000 reaxfit-0.2.0/LICENSE
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-06-20 03:09:27.239962 reaxfit-0.2.0/PKG-INFO
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      732 2023-06-09 06:14:50.000000 reaxfit-0.2.0/README.md
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.235962 reaxfit-0.2.0/example/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.235962 reaxfit-0.2.0/example/CoCO/
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     1892 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/0.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2151 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/1.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/2.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/3.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/4.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/5.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/6.xyz
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      189 2023-02-28 13:43:09.000000 reaxfit-0.2.0/example/CoCO/batch.sh
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      374 2023-02-28 13:52:46.000000 reaxfit-0.2.0/example/CoCO/chk.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      260 2023-03-03 02:56:27.000000 reaxfit-0.2.0/example/CoCO/config.json
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2310 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/data0
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    22606 2023-06-09 06:14:50.000000 reaxfit-0.2.0/example/CoCO/ffield.reax
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    22677 2023-03-02 14:08:20.000000 reaxfit-0.2.0/example/CoCO/ffield.temp
+-rw-r--r--   0 ykane     (1000) ykane     (1000)       58 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/refE
+-rw-r--r--   0 ykane     (1000) ykane     (1000)       56 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/refF
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      127 2023-02-28 13:40:22.000000 reaxfit-0.2.0/example/CoCO/run.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      235 2023-03-01 02:14:34.000000 reaxfit-0.2.0/example/README.md
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    61858 2023-06-09 06:14:50.000000 reaxfit-0.2.0/reaxfit_sample.ipynb
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       38 2023-06-20 03:09:27.239962 reaxfit-0.2.0/setup.cfg
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      723 2023-06-09 06:14:50.000000 reaxfit-0.2.0/setup.py
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.231962 reaxfit-0.2.0/src/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.235962 reaxfit-0.2.0/src/reaxfit/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       30 2023-02-22 05:23:36.000000 reaxfit-0.2.0/src/reaxfit/__init__.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     2185 2023-06-20 03:09:07.000000 reaxfit-0.2.0/src/reaxfit/__main__.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      160 2023-03-03 07:37:02.000000 reaxfit-0.2.0/src/reaxfit/_version.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    10238 2023-06-20 03:09:07.000000 reaxfit-0.2.0/src/reaxfit/reaxfit.py
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.239962 reaxfit-0.2.0/src/reaxfit.egg-info/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-06-20 03:09:27.000000 reaxfit-0.2.0/src/reaxfit.egg-info/PKG-INFO
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      691 2023-06-20 03:09:27.000000 reaxfit-0.2.0/src/reaxfit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)        1 2023-06-20 03:09:27.000000 reaxfit-0.2.0/src/reaxfit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)        8 2023-06-20 03:09:27.000000 reaxfit-0.2.0/src/reaxfit.egg-info/top_level.txt
```

### Comparing `reaxfit-0.1.4/.tagpr` & `reaxfit-0.2.0/.tagpr`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/LICENSE` & `reaxfit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/PKG-INFO` & `reaxfit-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: reaxfit
-Version: 0.1.4
-Summary: parameter fitting for ReaxFF
-Home-page: https://github.com/ykanematsu/reaxfit
-Author: ykanematsu
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ReaxFit
 Parameter-fitting module for lammps-reaxff with differential_evolution of scipy.
 ## Requirements
 - lammps (library)
 - numpy
 - scipy
 ## Install
```

### Comparing `reaxfit-0.1.4/example/CoCO/0.xyz` & `reaxfit-0.2.0/example/CoCO/0.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/example/CoCO/1.xyz` & `reaxfit-0.2.0/example/CoCO/1.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/example/CoCO/2.xyz` & `reaxfit-0.2.0/example/CoCO/2.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/example/CoCO/3.xyz` & `reaxfit-0.2.0/example/CoCO/3.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/example/CoCO/4.xyz` & `reaxfit-0.2.0/example/CoCO/4.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/example/CoCO/5.xyz` & `reaxfit-0.2.0/example/CoCO/5.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/example/CoCO/6.xyz` & `reaxfit-0.2.0/example/CoCO/6.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/example/CoCO/data0` & `reaxfit-0.2.0/example/CoCO/data0`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/example/CoCO/ffield.reax` & `reaxfit-0.2.0/example/CoCO/ffield.reax`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/example/CoCO/ffield.temp` & `reaxfit-0.2.0/example/CoCO/ffield.temp`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/reaxfit_sample.ipynb` & `reaxfit-0.2.0/reaxfit_sample.ipynb`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/setup.py` & `reaxfit-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.4/src/reaxfit/reaxfit.py` & `reaxfit-0.2.0/src/reaxfit/reaxfit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 from lammps import lammps
 import json,os,sys,re
 import numpy as np
-from scipy.optimize import differential_evolution
+from scipy.optimize import differential_evolution, minimize
 
 # global parameters are required for multiprocessing
 def wrap_eval(): pass
 def dump_best(): pass
-
-class reaxfit():
-  def __init__(self,cfile="config.json",dump_config=False):
-    self.cfile=cfile
-    self.option={
-            "refE_file":"refE", # reference energy
-            "refF_file":"refF", # reference force norm
+default_option={
+            "refE_file":"refE", # reference energy file
+            "refF_file":"refF", # reference force norm file
+            "ref_eV":True, # units for reference energy is in eV
+            "relative_force":True, # force norms are relative as refE
+            "force_weight":1e-6, # penalty weight for force norms
+            "harmonic":0, # harmonic constraint on initial parameters
             "datafile":"data0", # data file with initial structure
             "initfile":"ffield.temp", # initial template file
             "midfile":"ffield.currentbest", # intermediate file
             "endfile":"ffield.end", # final file
-            "bound":0.1, # define range of parameters 
-            "bound2":0.1, # define range of parameters 
+            "bound":0.1, # define range of parameters with "{"
+            "bound2":0.1, # define range of parameters  with "["
             "stopfile":"STOP", # file for early stopping
-            "seed":None, # file for early stopping
+            "seed":None, # seed for random number
             "tol":0.01, # tolerance for convergence
-            "workers":4, # file for early stopping
+            "workers":4, # number of cpus
             "maxiter":1000, # maximum number of iteration
+            "optimizer":"differential_evolution", # maximum number of iteration
             "scrdir":"scr" # scratch directory
-    }
-    isconfig=os.path.isfile(cfile)
-    if dump_config:
-        if isconfig: os.rename(cfile,cfile+".bk")
-        with open(cfile,"w") as f:
-            json.dump(self.option,f,indent=1)
-        sys.exit()
+}
+
+class reaxfit():
+  def __init__(self,cfile="config.json"):
+    self.cfile=cfile
+    self.option=default_option
     return
+
   def changes(self,para,file_name,atm1,atm2,numbers):
     with open(file_name) as f:
         text=f.read().splitlines()
     general =text[1].split()
     generals = int(general[0]) + 1
     atom=text[generals+1].split()
     atoms = int(atom[0])*4 +1 +3
@@ -95,14 +96,15 @@
         i+=1
     with open(file_name) as f:
         l = f.readlines()
     del l[gyou]
     l.insert(gyou,f"{result}\n")
     with open(file_name,mode="w")as f:
         f.writelines(l)
+
   def config(self,**kwargs):
     global dump_best
     if hasattr(kwargs,"cfile"): self.cfile=kwargs["cfile"]
     opt=self.option
     isconfig=os.path.isfile(self.cfile)
     if isconfig:
         print(f"read {self.cfile}")
@@ -114,26 +116,42 @@
                 print("unrecognized options: ",*(jwargs.keys()-optk))
     # overwrite options if given
     if kwargs:
         optk=opt.keys()&kwargs.keys()
         opt.update(**{k:kwargs[k] for k in optk})
         if(optk != kwargs.keys()): 
             print("unrecognized options: ",*(kwargs.keys()-optk))
+    self.option=opt
     midfile=opt["midfile"]
     stopfile=opt["stopfile"]
     for k in opt:
         setattr(self,k,opt[k])
     # create scratch directory
     os.makedirs(self.scrdir,exist_ok=True)
-    with open(self.refE_file) as f:
-      refE=f.read().split()
-    with open(self.refF_file) as f:
-      refF=f.read().split()
-    refE=np.array(refE,dtype=float)
-    refF=np.array(refF,dtype=float)
+    # conver eV to kcal/mol if refE is in eV
+    _coeff = 1.0/0.043364124 if self.ref_eV else 1.0
+    if os.path.isfile(self.refE_file):
+      with open(self.refE_file) as f:
+        refE=f.read().split()
+        _idx=[ i for i,v in enumerate(refE) if "*" in v ]+[len(refE)]
+        if _idx[0] != 0: _idx = [0] + _idx # initial snapshot must be reference
+        self.baseIdx=np.hstack([[_idx[i]]*(_idx[i+1]-_idx[i]) for i in range(len(_idx)-1)])
+        refE=[en.replace("*","") for en in refE]
+    else:
+      self.baseIdx=np.array([0])
+      refE=[0.0]
+    if os.path.isfile(self.refF_file):
+      with open(self.refF_file) as f:
+        refF=f.read().split()
+    else:
+      refF=[0.0]
+    refE=np.array(refE,dtype=float)*_coeff # relative energy
+    refE-=refE[self.baseIdx]
+    refF=np.array(refF,dtype=float)*_coeff
+    if self.relative_force: refF-=refF[self.baseIdx]
     # read template and x0
     with open(self.initfile) as f:
       _template=f.read()
     regex=re.compile("[\{\[][\d.-]+")
     x0=regex.findall(_template)
     isBound1=[]
     x1 = 0
@@ -181,25 +199,30 @@
       sys.stdout.flush()
       if fout: fname=fout
       with open(fname,"w") as f:
           _x=np.round(xk,5)
           y=[f"{{{xx}" for xx in _x]
           f.write(template.format(*y))
       if os.path.isfile(stopfile):
-          print("optimization will be stopped")
+          print("optimization will be stopped by the stop file")
           os.remove(stopfile)
           return True
     dump_best=callbackF
     return
   def set_eval(self,func):
     global wrap_eval
+    _x0=np.array(self.x0)
     def wrap_eval(*args,**kwargs):
       pid=os.getpid()
       pes,fns=self.reax(*args,pid=pid)
-      return func(pes,fns,self.refE,self.refF)
+      output = func(pes,fns,self.refE,self.refF) 
+      if self.harmonic > 0:
+        deltax=(np.array(args[0])-_x0)/(_x0+0.01)
+        output+=deltax@deltax*self.harmonic
+      return output
     return wrap_eval
   def reax(self,xk=None,pid=0):
       x=xk if xk is not None else self.x0
       ffname=f"{self.scrdir}/ffield.reax.{pid}"
       elements=self.elements
       pes,fns=[],[]
       with open(ffname,"w") as f:
@@ -225,35 +248,39 @@
       pes=np.array(pes)
       fns=np.array(fns)
       return pes,fns
 
   def fit(self,func=None):
       global dump_best
       if not hasattr(self,"x0"): self.config()
+      print("config parameters for fitting")
+      json.dump(self.option,sys.stdout)
+      print("")
       #refE,refF=self.refE,self.refF
       print(f"initial {len(self.x0)} parameters : {self.x0}")
       if not func:
-          _idx0=np.where(self.refE==0.0)[0]
-          idx0=_idx0[0] if _idx0 else 0
           @self.set_eval
           def default_eval(pes,fns,refE,refF):
-            fns*=0.043364124 # kcal/mol to ev
-            pes-=pes[idx0] # initial structure is reference by default
-            pes*=0.043364124 # kcal/mol to ev
-            pes+=refE[idx0]
+            pes0=pes[0]
+            pes-=pes[self.baseIdx] # initial structure is reference by default
             pes-=refE
+            if self.relative_force: fns-=fns[self.baseIdx]
             fns-=refF
-            return pes@pes + np.linalg.norm(fns)/len(fns)/10+fns[idx0]*fns[idx0]/10
+            fns*=self.force_weight
+            fmax=np.abs(fns).max()
+            return np.sign(pes0)*np.log10(np.abs(pes0)+1) + np.log10(fns@fns+1)
+            #return pes@pes + np.linalg.norm(fns)+np.abs(pes).max()*np.abs(fns).max()+fmax**2
+            #return pes@pes + np.linalg.norm(fns)/len(fns)/10+fns[0]*fns[0]/10
           func=default_eval
-      result = differential_evolution(func, self.bounds,workers=self.workers,x0=self.x0,updating='deferred',
+      if self.optimizer == "differential_evolution":
+        result = differential_evolution(func, self.bounds,workers=self.workers,x0=self.x0,updating='deferred',
                                   disp=True,maxiter=self.maxiter,tol=self.tol,callback=dump_best,popsize=16,seed=self.seed)
-      #print(result)
+      else:
+        result = minimize(func,x0=self.x0,method=self.optimizer,tol=self.tol,callback=dump_best,jac='3-point') 
+      print(result)
       dump_best(result.x,fout=self.endfile)
       self.result=result
       self.E,self.F=self.reax(result.x)
       return result
 
 if __name__ =='__main__':
-    reax=reaxfit()
-    result=reax.fit()
-    pes,fns=reax.reax(result.x)
-    print(pes,fns)
+    pass
```

### Comparing `reaxfit-0.1.4/src/reaxfit.egg-info/PKG-INFO` & `reaxfit-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxfit
-Version: 0.1.4
+Version: 0.2.0
 Summary: parameter fitting for ReaxFF
 Home-page: https://github.com/ykanematsu/reaxfit
 Author: ykanematsu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `reaxfit-0.1.4/src/reaxfit.egg-info/SOURCES.txt` & `reaxfit-0.2.0/src/reaxfit.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,13 +20,14 @@
 example/CoCO/data0
 example/CoCO/ffield.reax
 example/CoCO/ffield.temp
 example/CoCO/refE
 example/CoCO/refF
 example/CoCO/run.py
 src/reaxfit/__init__.py
+src/reaxfit/__main__.py
 src/reaxfit/_version.py
 src/reaxfit/reaxfit.py
 src/reaxfit.egg-info/PKG-INFO
 src/reaxfit.egg-info/SOURCES.txt
 src/reaxfit.egg-info/dependency_links.txt
 src/reaxfit.egg-info/top_level.txt
```

