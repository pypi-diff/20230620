# Comparing `tmp/tdasha-0.1.0.tar.gz` & `tmp/tdasha-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdasha-0.1.0.tar", last modified: Thu May  4 12:42:44 2023, max compression
+gzip compressed data, was "tdasha-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tdasha-0.1.0.tar` & `tdasha-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-05-04 12:42:34.755796 tdasha-0.1.0/LICENSE
--rw-r--r--   0        0        0        8 2023-05-04 12:42:34.755796 tdasha-0.1.0/README.md
--rw-r--r--   0        0        0      971 2023-05-04 12:42:34.755796 tdasha-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      234 2023-05-04 12:42:34.755796 tdasha-0.1.0/tdasha/__init__.py
--rw-r--r--   0        0        0     6177 2023-05-04 12:42:34.755796 tdasha-0.1.0/tdasha/compute.py
--rw-r--r--   0        0        0     2649 2023-05-04 12:42:34.755796 tdasha-0.1.0/tdasha/io.py
--rw-r--r--   0        0        0     6549 2023-05-04 12:42:34.755796 tdasha-0.1.0/tdasha/window.py
--rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 tdasha-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-20 13:36:15.673513 tdasha-0.2.0/LICENSE
+-rw-r--r--   0        0        0        8 2023-06-20 13:36:15.673513 tdasha-0.2.0/README.md
+-rw-r--r--   0        0        0      971 2023-06-20 13:36:15.673513 tdasha-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      234 2023-06-20 13:36:15.673513 tdasha-0.2.0/tdasha/__init__.py
+-rw-r--r--   0        0        0    13900 2023-06-20 13:36:15.673513 tdasha-0.2.0/tdasha/compute.py
+-rw-r--r--   0        0        0     2723 2023-06-20 13:36:15.673513 tdasha-0.2.0/tdasha/io.py
+-rw-r--r--   0        0        0     8662 2023-06-20 13:36:15.673513 tdasha-0.2.0/tdasha/window.py
+-rw-r--r--   0        0        0      858 1970-01-01 00:00:00.000000 tdasha-0.2.0/PKG-INFO
```

### Comparing `tdasha-0.1.0/LICENSE` & `tdasha-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tdasha-0.1.0/pyproject.toml` & `tdasha-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 authors = [
   {name = "Stanisław Lasocki"},
   {name = "Francis Tong"},
 ]
 description = "Time-dependent Anthropogenic Seismic Hazard Assessment"
 name = "tdasha"
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
```

### Comparing `tdasha-0.1.0/tdasha/io.py` & `tdasha-0.2.0/tdasha/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from obspy import UTCDateTime
 from obspy.clients.fdsn import Client
 from obspy import read_events
 import numpy as np
 
 def read_csv(csv_file,  datenum= True, **kwargs):
     
-    df = pd.read_csv(csv_file, engine="pyarrow", **kwargs)
+    # df = pd.read_csv(csv_file, engine="pyarrow", **kwargs) #use pyarrow for faster input
+    df = pd.read_csv(csv_file, **kwargs)
     
     df.columns= df.columns.str.lower() # convert header to all lowercase letters
     header = df.columns
     
     # replace with common column names if present
     if 'time' in header:
         t_label = 'time'
```

### Comparing `tdasha-0.1.0/tdasha/window.py` & `tdasha-0.2.0/tdasha/window.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 """
 
 import numpy as np
 from KDEpy import FFTKDE
 from scipy.stats import norm
 from inspect import signature
 from resample.bootstrap import confidence_interval, resample
+from scipy.optimize import root_scalar
+from adaptivekde import sskernel, ssvkernel
+
+import dask
 
 class Window:
     
     
     def __init__(self, mc, rum, m, t, t_unit, t_step, t_period, **kwargs):
         
         self.mc = mc
@@ -78,22 +82,32 @@
         # if type(bandwidth)==str: #need to estimate bandwidth
         #     kde = sm.nonparametric.KDEUnivariate(xx)
         #     kde.fit(bw=bandwidth)
         #     h = kde.bw
         # else:
         #     h = bandwidth
                 
-        # use KDEpy to estimate bandwidth                
-        if type(bw)==str: 
+        # use KDEpy to estimate bandwidth
+        if bw == 'ls':
+            args = self.filter_args(kwargs, self.h_plat) #filter kwargs
+            h = self.h_plat(x, **args)
+        elif bw == 'ss':
+            args = self.filter_args(kwargs, sskernel) #filter kwargs
+            kde = sskernel(x, **args)
+            h = kde[2]
+        # elif bw == 'ssv': #don't know how to use multiple bandwidth values in a window yet.
+        
+        elif type(bw)==str: 
             args = self.filter_args(kwargs, FFTKDE) #filter kwargs
             h = FFTKDE(bw=bw, **args).fit(x).bw            
-        else:
+        elif type(bw)==float:
             h = bw # use user-provided value for bandwidth
         
-        print(h)        
+
+        
         return h
     
     def bootstrap_ci(self, size=2000, **kwargs):
         
         # use pingouin for bootstrap
         # from pingouin import compute_bootci
         # CDF_CI = compute_bootci(M_sel, func=cdf_nonpar_ci, n_boot=2000, paired=False, method='cper', confidence=0.98)
@@ -173,8 +187,57 @@
         ci_upper = 1 - np.exp(np.multiply(- act_rate * (1 - cdf_ci[0]),t_period))
         ci_lower = 1 - np.exp(np.multiply(- act_rate * (1 - cdf_ci[1]),t_period))
         return [ci_lower, ci_upper]
     
     def filter_args(self, args, function): #filter arguments dictionary by list of arguments that the function actually accepts 
         key_list = signature(function).parameters
         filtered_args = {key: value for key, value in args.items() if key in key_list}      
-        return filtered_args
+        return filtered_args
+    
+    def funct(self, t, x):
+        p2 = 1.41421356
+        n = len(x)
+        yy = np.zeros(n)
+        for i in range(n):
+            xij = (x - x[i])**2 / t**2
+            y = np.exp(-xij / 4) * ((xij / 2 - 1) / p2) - 2 * np.exp(-xij / 2) * (xij - 1)
+            yy[i] = np.sum(y)
+        fct = np.sum(yy) - 2 * n
+        return fct
+    
+    def h_plat(self, x, solver='brenth'):
+
+        n = len(x)
+        x = np.sort(x)
+        sig = np.std(x, ddof=1)
+        interval = np.array([0.1 * sig / n**0.2, 2 * sig / n**0.2])
+        x1 = self.funct(interval[0], x)
+        x2 = self.funct(interval[1], x)
+
+        if x1 * x2 < 0:
+            fun = lambda t: self.funct(t, x)
+            sol = root_scalar(fun, method=solver, bracket=interval)
+            h = sol.root
+        else:
+            y1 = 10 ** (np.floor(np.log10(interval[0]))) / 10
+            x1 = self.funct(y1, x)
+            x2 = self.funct(interval[0], x)
+            if x1 * x2 < 0:
+                interval[1] = interval[0]
+                interval[0] = y1
+                fun = lambda t: self.funct(t, x)
+                sol = root_scalar(fun, method=solver, bracket=interval)
+                h = sol.root
+            else:
+                y1 = 10 ** (np.floor(np.log10(interval[0]))) / 10
+                dy = 0.05 * y1
+                k = 0
+                hh = []
+                for i in np.arange(y1, interval[0], dy):
+                    k += 1
+                    hh.append(self.funct(i, x))
+                k = np.argmin(np.abs(hh))
+                h = y1 + (k - 1) * dy
+
+        return h
+
+
```

### Comparing `tdasha-0.1.0/PKG-INFO` & `tdasha-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdasha
-Version: 0.1.0
+Version: 0.2.0
 Summary: Time-dependent Anthropogenic Seismic Hazard Assessment
 Author: Stanisław Lasocki, Francis Tong
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

