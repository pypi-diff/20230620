# Comparing `tmp/reaxfit-0.2.0.tar.gz` & `tmp/reaxfit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxfit-0.2.0.tar", last modified: Tue Jun 20 03:09:27 2023, max compression
+gzip compressed data, was "reaxfit-0.2.1.tar", last modified: Tue Jun 20 03:31:19 2023, max compression
```

## Comparing `reaxfit-0.2.0.tar` & `reaxfit-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.239962 reaxfit-0.2.0/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.235962 reaxfit-0.2.0/.github/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       48 2023-03-03 06:38:54.000000 reaxfit-0.2.0/.github/release.yml
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.235962 reaxfit-0.2.0/.github/workflows/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      251 2023-03-03 06:38:54.000000 reaxfit-0.2.0/.github/workflows/tagpr.yml
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      111 2023-04-12 04:40:21.000000 reaxfit-0.2.0/.gitignore
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     1794 2023-03-03 06:38:54.000000 reaxfit-0.2.0/.tagpr
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     1067 2023-03-01 01:38:22.000000 reaxfit-0.2.0/LICENSE
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-06-20 03:09:27.239962 reaxfit-0.2.0/PKG-INFO
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      732 2023-06-09 06:14:50.000000 reaxfit-0.2.0/README.md
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.235962 reaxfit-0.2.0/example/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.235962 reaxfit-0.2.0/example/CoCO/
--rw-r--r--   0 ykane     (1000) ykane     (1000)     1892 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/0.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2151 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/1.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/2.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/3.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/4.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/5.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/6.xyz
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      189 2023-02-28 13:43:09.000000 reaxfit-0.2.0/example/CoCO/batch.sh
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      374 2023-02-28 13:52:46.000000 reaxfit-0.2.0/example/CoCO/chk.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      260 2023-03-03 02:56:27.000000 reaxfit-0.2.0/example/CoCO/config.json
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2310 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/data0
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    22606 2023-06-09 06:14:50.000000 reaxfit-0.2.0/example/CoCO/ffield.reax
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    22677 2023-03-02 14:08:20.000000 reaxfit-0.2.0/example/CoCO/ffield.temp
--rw-r--r--   0 ykane     (1000) ykane     (1000)       58 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/refE
--rw-r--r--   0 ykane     (1000) ykane     (1000)       56 2023-02-22 04:48:36.000000 reaxfit-0.2.0/example/CoCO/refF
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      127 2023-02-28 13:40:22.000000 reaxfit-0.2.0/example/CoCO/run.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      235 2023-03-01 02:14:34.000000 reaxfit-0.2.0/example/README.md
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    61858 2023-06-09 06:14:50.000000 reaxfit-0.2.0/reaxfit_sample.ipynb
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       38 2023-06-20 03:09:27.239962 reaxfit-0.2.0/setup.cfg
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      723 2023-06-09 06:14:50.000000 reaxfit-0.2.0/setup.py
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.231962 reaxfit-0.2.0/src/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.235962 reaxfit-0.2.0/src/reaxfit/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       30 2023-02-22 05:23:36.000000 reaxfit-0.2.0/src/reaxfit/__init__.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     2185 2023-06-20 03:09:07.000000 reaxfit-0.2.0/src/reaxfit/__main__.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      160 2023-03-03 07:37:02.000000 reaxfit-0.2.0/src/reaxfit/_version.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    10238 2023-06-20 03:09:07.000000 reaxfit-0.2.0/src/reaxfit/reaxfit.py
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:09:27.239962 reaxfit-0.2.0/src/reaxfit.egg-info/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-06-20 03:09:27.000000 reaxfit-0.2.0/src/reaxfit.egg-info/PKG-INFO
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      691 2023-06-20 03:09:27.000000 reaxfit-0.2.0/src/reaxfit.egg-info/SOURCES.txt
--rw-rw-r--   0 ykane     (1000) ykane     (1000)        1 2023-06-20 03:09:27.000000 reaxfit-0.2.0/src/reaxfit.egg-info/dependency_links.txt
--rw-rw-r--   0 ykane     (1000) ykane     (1000)        8 2023-06-20 03:09:27.000000 reaxfit-0.2.0/src/reaxfit.egg-info/top_level.txt
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:31:19.407519 reaxfit-0.2.1/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:31:19.403519 reaxfit-0.2.1/.github/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       48 2023-03-03 06:38:54.000000 reaxfit-0.2.1/.github/release.yml
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:31:19.403519 reaxfit-0.2.1/.github/workflows/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      251 2023-03-03 06:38:54.000000 reaxfit-0.2.1/.github/workflows/tagpr.yml
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      111 2023-04-12 04:40:21.000000 reaxfit-0.2.1/.gitignore
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     1794 2023-03-03 06:38:54.000000 reaxfit-0.2.1/.tagpr
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     1067 2023-03-01 01:38:22.000000 reaxfit-0.2.1/LICENSE
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-06-20 03:31:19.407519 reaxfit-0.2.1/PKG-INFO
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      732 2023-06-09 06:14:50.000000 reaxfit-0.2.1/README.md
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:31:19.403519 reaxfit-0.2.1/example/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:31:19.407519 reaxfit-0.2.1/example/CoCO/
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     1892 2023-02-22 04:48:36.000000 reaxfit-0.2.1/example/CoCO/0.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2151 2023-02-22 04:48:36.000000 reaxfit-0.2.1/example/CoCO/1.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.1/example/CoCO/2.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.1/example/CoCO/3.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.2.1/example/CoCO/4.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.2.1/example/CoCO/5.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.2.1/example/CoCO/6.xyz
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      189 2023-02-28 13:43:09.000000 reaxfit-0.2.1/example/CoCO/batch.sh
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      374 2023-02-28 13:52:46.000000 reaxfit-0.2.1/example/CoCO/chk.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      260 2023-03-03 02:56:27.000000 reaxfit-0.2.1/example/CoCO/config.json
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2310 2023-02-22 04:48:36.000000 reaxfit-0.2.1/example/CoCO/data0
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    22606 2023-06-09 06:14:50.000000 reaxfit-0.2.1/example/CoCO/ffield.reax
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    22677 2023-03-02 14:08:20.000000 reaxfit-0.2.1/example/CoCO/ffield.temp
+-rw-r--r--   0 ykane     (1000) ykane     (1000)       58 2023-02-22 04:48:36.000000 reaxfit-0.2.1/example/CoCO/refE
+-rw-r--r--   0 ykane     (1000) ykane     (1000)       56 2023-02-22 04:48:36.000000 reaxfit-0.2.1/example/CoCO/refF
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      127 2023-02-28 13:40:22.000000 reaxfit-0.2.1/example/CoCO/run.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      235 2023-03-01 02:14:34.000000 reaxfit-0.2.1/example/README.md
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    61858 2023-06-09 06:14:50.000000 reaxfit-0.2.1/reaxfit_sample.ipynb
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       38 2023-06-20 03:31:19.407519 reaxfit-0.2.1/setup.cfg
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      723 2023-06-09 06:14:50.000000 reaxfit-0.2.1/setup.py
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:31:19.403519 reaxfit-0.2.1/src/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:31:19.407519 reaxfit-0.2.1/src/reaxfit/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       30 2023-02-22 05:23:36.000000 reaxfit-0.2.1/src/reaxfit/__init__.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     2185 2023-06-20 03:09:07.000000 reaxfit-0.2.1/src/reaxfit/__main__.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      160 2023-03-03 07:37:02.000000 reaxfit-0.2.1/src/reaxfit/_version.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    10238 2023-06-20 03:28:39.000000 reaxfit-0.2.1/src/reaxfit/reaxfit.py
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-20 03:31:19.407519 reaxfit-0.2.1/src/reaxfit.egg-info/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-06-20 03:31:19.000000 reaxfit-0.2.1/src/reaxfit.egg-info/PKG-INFO
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      691 2023-06-20 03:31:19.000000 reaxfit-0.2.1/src/reaxfit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)        1 2023-06-20 03:31:19.000000 reaxfit-0.2.1/src/reaxfit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)        8 2023-06-20 03:31:19.000000 reaxfit-0.2.1/src/reaxfit.egg-info/top_level.txt
```

### Comparing `reaxfit-0.2.0/.tagpr` & `reaxfit-0.2.1/.tagpr`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/LICENSE` & `reaxfit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/PKG-INFO` & `reaxfit-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxfit
-Version: 0.2.0
+Version: 0.2.1
 Summary: parameter fitting for ReaxFF
 Home-page: https://github.com/ykanematsu/reaxfit
 Author: ykanematsu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `reaxfit-0.2.0/README.md` & `reaxfit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/example/CoCO/0.xyz` & `reaxfit-0.2.1/example/CoCO/0.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/example/CoCO/1.xyz` & `reaxfit-0.2.1/example/CoCO/1.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/example/CoCO/2.xyz` & `reaxfit-0.2.1/example/CoCO/2.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/example/CoCO/3.xyz` & `reaxfit-0.2.1/example/CoCO/3.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/example/CoCO/4.xyz` & `reaxfit-0.2.1/example/CoCO/4.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/example/CoCO/5.xyz` & `reaxfit-0.2.1/example/CoCO/5.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/example/CoCO/6.xyz` & `reaxfit-0.2.1/example/CoCO/6.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/example/CoCO/data0` & `reaxfit-0.2.1/example/CoCO/data0`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/example/CoCO/ffield.reax` & `reaxfit-0.2.1/example/CoCO/ffield.reax`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/example/CoCO/ffield.temp` & `reaxfit-0.2.1/example/CoCO/ffield.temp`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/reaxfit_sample.ipynb` & `reaxfit-0.2.1/reaxfit_sample.ipynb`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/setup.py` & `reaxfit-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/src/reaxfit/__main__.py` & `reaxfit-0.2.1/src/reaxfit/__main__.py`

 * *Files identical despite different names*

### Comparing `reaxfit-0.2.0/src/reaxfit/reaxfit.py` & `reaxfit-0.2.1/src/reaxfit/reaxfit.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,16 +263,16 @@
             pes0=pes[0]
             pes-=pes[self.baseIdx] # initial structure is reference by default
             pes-=refE
             if self.relative_force: fns-=fns[self.baseIdx]
             fns-=refF
             fns*=self.force_weight
             fmax=np.abs(fns).max()
-            return np.sign(pes0)*np.log10(np.abs(pes0)+1) + np.log10(fns@fns+1)
-            #return pes@pes + np.linalg.norm(fns)+np.abs(pes).max()*np.abs(fns).max()+fmax**2
+            #return np.sign(pes0)*np.log10(np.abs(pes0)+1) + np.log10(fns@fns+1)
+            return pes@pes + np.linalg.norm(fns)+np.abs(pes).max()*np.abs(fns).max()+fmax**2
             #return pes@pes + np.linalg.norm(fns)/len(fns)/10+fns[0]*fns[0]/10
           func=default_eval
       if self.optimizer == "differential_evolution":
         result = differential_evolution(func, self.bounds,workers=self.workers,x0=self.x0,updating='deferred',
                                   disp=True,maxiter=self.maxiter,tol=self.tol,callback=dump_best,popsize=16,seed=self.seed)
       else:
         result = minimize(func,x0=self.x0,method=self.optimizer,tol=self.tol,callback=dump_best,jac='3-point')
```

### Comparing `reaxfit-0.2.0/src/reaxfit.egg-info/PKG-INFO` & `reaxfit-0.2.1/src/reaxfit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxfit
-Version: 0.2.0
+Version: 0.2.1
 Summary: parameter fitting for ReaxFF
 Home-page: https://github.com/ykanematsu/reaxfit
 Author: ykanematsu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `reaxfit-0.2.0/src/reaxfit.egg-info/SOURCES.txt` & `reaxfit-0.2.1/src/reaxfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

