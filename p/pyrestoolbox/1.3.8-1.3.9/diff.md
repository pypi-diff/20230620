# Comparing `tmp/pyrestoolbox-1.3.8.tar.gz` & `tmp/pyrestoolbox-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrestoolbox-1.3.8.tar", last modified: Wed Jan  4 03:23:44 2023, max compression
+gzip compressed data, was "pyrestoolbox-1.3.9.tar", last modified: Tue Jun 20 05:19:10 2023, max compression
```

## Comparing `pyrestoolbox-1.3.8.tar` & `pyrestoolbox-1.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-01-04 03:23:44.190924 pyrestoolbox-1.3.8/
--rw-rw-rw-   0        0        0    33092 2021-12-19 10:23:37.000000 pyrestoolbox-1.3.8/LICENSE
--rw-rw-rw-   0        0        0       37 2022-01-30 04:13:11.000000 pyrestoolbox-1.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5222 2023-01-04 03:23:44.190924 pyrestoolbox-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    19628 2023-01-04 03:22:28.000000 pyrestoolbox-1.3.8/README.rst
--rw-rw-rw-   0        0        0      121 2022-01-07 02:09:05.000000 pyrestoolbox-1.3.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-01-04 03:23:44.174794 pyrestoolbox-1.3.8/pyrestoolbox/
--rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.3.8/pyrestoolbox/__init__.py
--rw-rw-rw-   0        0        0    41658 2022-01-30 01:52:14.000000 pyrestoolbox-1.3.8/pyrestoolbox/component_library.xlsx
--rw-rw-rw-   0        0        0   124852 2023-01-04 03:20:29.000000 pyrestoolbox-1.3.8/pyrestoolbox/pyrestoolbox.py
-drwxrwxrwx   0        0        0        0 2023-01-04 03:23:44.190924 pyrestoolbox-1.3.8/pyrestoolbox/simtools/
--rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.3.8/pyrestoolbox/simtools/__init__.py
--rw-rw-rw-   0        0        0    37326 2022-04-19 07:29:27.000000 pyrestoolbox-1.3.8/pyrestoolbox/simtools/simtools.py
-drwxrwxrwx   0        0        0        0 2023-01-04 03:23:44.174794 pyrestoolbox-1.3.8/pyrestoolbox.egg-info/
--rw-rw-rw-   0        0        0     5222 2023-01-04 03:23:44.000000 pyrestoolbox-1.3.8/pyrestoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-01-04 03:23:44.000000 pyrestoolbox-1.3.8/pyrestoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-04 03:23:44.000000 pyrestoolbox-1.3.8/pyrestoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-01-04 03:23:44.000000 pyrestoolbox-1.3.8/pyrestoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-01-04 03:23:44.000000 pyrestoolbox-1.3.8/pyrestoolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-01-04 03:23:44.190924 pyrestoolbox-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1218 2023-01-04 03:06:51.000000 pyrestoolbox-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:19:10.725211 pyrestoolbox-1.3.9/
+-rw-rw-rw-   0        0        0    33092 2021-12-19 10:23:37.000000 pyrestoolbox-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0       37 2022-01-30 04:13:11.000000 pyrestoolbox-1.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5313 2023-06-20 05:19:10.726212 pyrestoolbox-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    19717 2023-06-20 05:17:25.000000 pyrestoolbox-1.3.9/README.rst
+-rw-rw-rw-   0        0        0      121 2022-01-07 02:09:05.000000 pyrestoolbox-1.3.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-20 05:19:10.711213 pyrestoolbox-1.3.9/pyrestoolbox/
+-rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.3.9/pyrestoolbox/__init__.py
+-rw-rw-rw-   0        0        0    41658 2022-01-30 01:52:14.000000 pyrestoolbox-1.3.9/pyrestoolbox/component_library.xlsx
+-rw-rw-rw-   0        0        0   122791 2023-06-20 01:59:12.000000 pyrestoolbox-1.3.9/pyrestoolbox/pyrestoolbox.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:19:10.723243 pyrestoolbox-1.3.9/pyrestoolbox/simtools/
+-rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.3.9/pyrestoolbox/simtools/__init__.py
+-rw-rw-rw-   0        0        0    37326 2022-04-19 07:29:27.000000 pyrestoolbox-1.3.9/pyrestoolbox/simtools/simtools.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:19:10.719210 pyrestoolbox-1.3.9/pyrestoolbox.egg-info/
+-rw-rw-rw-   0        0        0     5313 2023-06-20 05:19:10.000000 pyrestoolbox-1.3.9/pyrestoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2023-06-20 05:19:10.000000 pyrestoolbox-1.3.9/pyrestoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 05:19:10.000000 pyrestoolbox-1.3.9/pyrestoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-20 05:19:10.000000 pyrestoolbox-1.3.9/pyrestoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 05:19:10.000000 pyrestoolbox-1.3.9/pyrestoolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-06-20 05:19:10.727213 pyrestoolbox-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2023-06-20 05:18:54.000000 pyrestoolbox-1.3.9/setup.py
```

### Comparing `pyrestoolbox-1.3.8/LICENSE` & `pyrestoolbox-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.3.8/PKG-INFO` & `pyrestoolbox-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestoolbox
-Version: 1.3.8
+Version: 1.3.9
 Summary: pyResToolbox - A collection of Reservoir Engineering Utilities
 Home-page: https://github.com/mwburgoyne/pyResToolbox
 Author: Mark W. Burgoyne
 Author-email: mark.w.burgoyne@gmail.com
 Keywords: restoolbox,petroleum,reservoir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -40,14 +40,17 @@
     ECLIPSE
 -   Creation of Corey and LET relative permeability tables in Eclipse
     format
 
 Apologies in advance that it is only in oilfield
 units with no current plans to add multi-unit support.
 
+Changelist in 1.3.9:
+- Tweaks to speed DAK and Hall & Yarborough Z-Factor calculations
+
 Changelist in 1.3.8:
 - Fix bug in Hall & Yarborough Z-Factor calculation
 
 Changelist in 1.3.5:
 - Fix bug in ECL deck zip/check recursion
 
 Changelist in 1.3.4:
```

### Comparing `pyrestoolbox-1.3.8/README.rst` & `pyrestoolbox-1.3.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 - Return critical parameters for typical components
 - Creation of Black Oil Table information
 - Creation of layered permeability distribution consistent with a Lorenze heterogeneity factor
 - Extract problem cells information from Intesect (IX) print files
 - Generation of AQUTAB include file influence functions for use in ECLIPSE
 - Creation of Corey and LET relative permeability tables in Eclipse format
 
+Changelist in 1.3.9:
+
+- Tweaks to speed DAK and Hall & Yarborough Z-Factor calculations
+
 Changelist in 1.3.8:
 
 - Fix bug in Hall & Yarborough Z-Factor algorithm
 
 Changelist in 1.3.5:
 
 - Fix bug in ECL deck zip/check recursion
```

### Comparing `pyrestoolbox-1.3.8/pyrestoolbox/component_library.xlsx` & `pyrestoolbox-1.3.9/pyrestoolbox/component_library.xlsx`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.3.8/pyrestoolbox/pyrestoolbox.py` & `pyrestoolbox-1.3.9/pyrestoolbox/pyrestoolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -551,19 +551,19 @@
     cmethod: c_method = c_method.PMC,
     n2: float = 0,
     co2: float = 0,
     h2s: float = 0,
     tc: float = 0,
     pc: float = 0,
 ) -> np.ndarray:
-    """ Returns real-gas deviation factor (Z)
-        p: Gas pressure (psia)
-        sg: Gas SG relative to air. Defaults to False if undefined
-        pwf: BHFP (psia)
-        degf: Gas Temperature (deg F)
+    """ Returns real-gas deviation factor (Z). Returning either single float, or numpy array depending upon 
+        whether single pressure of list/array or pressures has been specified.
+        p: Gas pressure (psia). Takes a single float, 1D list or 1D Numpy array
+        sg: Gas SG relative to air. Single float only
+        degf: Gas Temperature (deg F). Single float only
         zmethod: Method for calculating Z-Factor
                  'DAK' Dranchuk & Abou-Kassem (1975) using from Equations 2.7-2.8 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
                  'HY' Hall & Yarborough (1973)
                  'WYW' Wang, Ye & Wu (2021)
                  defaults to 'DAK' if not specified
         cmethod: Method for calculting critical properties
                'SUT' for Sutton with Wichert & Aziz non-hydrocarbon corrections, or
@@ -577,235 +577,112 @@
     """
     p = np.asarray(p)
     zmethod, cmethod = validate_methods(
         ["zmethod", "cmethod"], [zmethod, cmethod]
     )
 
     tc, pc = gas_tc_pc(sg, n2, co2, h2s, cmethod.name, tc, pc)
-
-    def zdak(p, degf, sg, tc, pc):
+    tr = (degf + f2r) / tc
+    
+    single_p = False
+    if p.size == 1:
+        single_p = True
+        pprs = np.array([p/pc])
+    else:
+        pprs = np.array(p/pc)
+    
+    def zdak(pprs, tr):
         # DAK from Equations 2.7-2.8 from 'Petroleum Reservoir Fluid Property Correlations' by W. McCain et al.
         # sg relative to air, t in deg F, p in psia, n2, co2 and h2s in fractions (0-1)
+        
+        tr2, tr3 = tr**2, tr**3
+        a = np.array([0,0.3265,-1.07,-0.5339,0.01569,-0.05165,0.5475,-0.7361,0.1844,0.1056,0.6134,0.7210])
+        c1 = a[1]+(a[2]/tr) + (a[3]/tr3) + (a[4]/tr**4) + (a[5]/tr**5)
+        c2 = a[6] + (a[7]/tr) + (a[8]/tr2)
+        c3 = a[9] * ((a[7]/tr) + (a[8]/tr2))
+    
+        def new_dak_z(z, pr, tr):
+            rhor = 0.27 * pr / (tr * z)  # 2.8
+            c4 = a[10] * (1 + a[11] * rhor**2) * (rhor**2/tr3) * np.exp(-a[11] * rhor**2)
+            err = fz(z, rhor, c4)
+            return z - err/fz_prime(z, rhor, c4), err # Returns updated guess for Z, as well as the error
+        
+        def fz(z, rhor, c4):                          # The DAK Error function
+            return z - (1 + c1*rhor + c2*rhor**2 - c3 * rhor**5 + c4)
+    
+        def fz_prime(z, rhor, c4):                    # Derivative of the DAK Error function
+            return 1 + c1*rhor/z + (2*c2*rhor**2/z) - (5*c3*rhor**5/z) + 2*a[10]*rhor**2/(z*tr3)*(1+a[11]*rhor**2 - (a[11]*rhor**2)**2)*np.exp(-a[11]*rhor**2)
+    
+        def z_dak_calc(pr, tr, tol = 1e-6):
+            niter = 0
+            midz = min(max(0.1, z_wyw(pr, tr)),3) # First guess using explict calculation method
+            mid_err = 1
+            while abs(mid_err) > tol and niter < 100:
+                midz, mid_err = new_dak_z(midz, pr, tr)
+                niter += 1
+            return midz
 
-        def Eq2p7(pr, tr, rhor, a):
-            z_calc = (
-                1
-                + (
-                    a[1]
-                    + (a[2] / tr)
-                    + (a[3] / (tr * tr * tr))
-                    + (a[4] / (tr * tr * tr * tr))
-                    + (a[5] / np.power(tr, 5))
-                )
-                * rhor
-                + ((a[6] + (a[7] / tr) + (a[8] / (tr * tr))) * rhor * rhor)
-                - (
-                    a[9]
-                    * ((a[7] / tr) + (a[8] / (tr * tr)))
-                    * np.power(rhor, 5)
-                )
-                + (
-                    a[10]
-                    * (1 + (a[11] * rhor * rhor))
-                    * (rhor * rhor / np.power(tr, 3))
-                    * np.exp(-a[11] * rhor * rhor)
-                )
-            )
-            return z_calc
-
-        zout = []
-        single_p = False
-        if p.size == 1:
-            single_p = True
-            ps = [p]
-        else:
-            ps = p.tolist()
-
-        a = np.array(
-            [
-                0,
-                0.3265,
-                -1.07,
-                -0.5339,
-                0.01569,
-                -0.05165,
-                0.5475,
-                -0.7361,
-                0.1844,
-                0.1056,
-                0.6134,
-                0.7210,
-            ]
-        )
-        tr = (degf + f2r) / tc
-
-        for p in ps:
-            pr = p / pc
-
-            def z_err(z):
-                rhor = 0.27 * pr / (tr * z)  # 2.8
-                z2 = Eq2p7(pr, tr, rhor, a)
-                return z2 - z
-
-            if sg < 1.725:  # Gas, cutoff MW used = 50 lb/lb-mol
-                low_z = 0.106196302 * pr - 0.024351977
-                low_z = max(0.15, low_z)
-                if pr > 9.74:
-                    low_z = 0.029121 * pr + 0.726357
-                if pr < 8.79:
-                    hi_z = 0.021745 * pr + 1.144863
-                else:
-                    hi_z = 0.103725 * pr + 0.42426
-
-                z = brentq(z_err, low_z, hi_z)
-            else:  # Oil
-                mwo = sg * mw_air
-                zhigh = (
-                    p * mwo / (0.4 * 62.42) / (R * (degf + f2r))
-                )  # Z-Factor consistent with liquid SG = 0.4
-                zlow = (
-                    p * mwo / (1.1 * 62.42) / (R * (degf + f2r))
-                )  # Z-Factor consistent with liquid SG = 1.1
-                z = brentq(z_err, zlow, zhigh)  # For Oil
-            zout.append(z)
+        zout = [z_dak_calc(pr, tr) for pr in pprs]
+            
         if single_p:
             return zout[0]
         else:
             return np.array(zout)
 
     # Hall & Yarborough
-    def z_hy(p, degf, sg, tc, pc):
-        # Using implemention in "Petroleum Production Engineering, A computer assisted approach"
-        single_p = False
-        if p.size == 1:
-            single_p = True
-            ps = [p]
-        else:
-            ps = p.tolist()
-
+    def z_hy(pprs, tr):
+        tr = 1/tr
+        t2 = tr ** 2
+        a = 0.06125 * tr * np.exp(-1.2 * (1 - tr) ** 2)
+        b = tr * (14.76 - 9.76 * tr + 4.58 * t2)
+        c = tr * (90.7 - 242.2 * tr + 42.4 * t2)
+        D = 2.18 + 2.82 * tr
+         
+        # f(y)
+        def f(y, a, b, c, D, pr):   
+            return ((y + y ** 2 + y ** 3 - y ** 4) / ((1 - y) ** 3)) - a * pr - b * y ** 2 + c * y ** D
+    
+        # derivative of f(y)
+        def df(y, a, b, c, D):
+            return ((1 + 4 * y + 4 * y ** 2 - 4 * y ** 3 + y ** 4) / ((1 - y) ** 4)) - 2 * b * y + c * D * y ** (D - 1)     
+         
         zout = []
-
-        tpr = (degf + f2r) / tc
-        t = 1 / tpr
-        t2 = t ** 2
-        A = 0.06125 * t * np.exp(-1.2 * (1 - t) ** 2)
-        B = t * (14.76 - 9.76 * t + 4.58 * t2)
-        C = t * (90.7 - 242.2 * t + 42.4 * t2)
-        D = 2.18 + 2.82 * t
-
-        for p in ps:
-            pr = p / pc
-            low_z = 0.106196302 * pr - 0.024351977
-            low_z = max(0.15, low_z)
-            if pr > 9.74:
-                low_z = 0.029121 * pr + 0.726357
-            if pr < 8.79:
-                hi_z = 0.021745 * pr + 1.144863
-            else:
-                hi_z = 0.103725 * pr + 0.42426
-            low_y, high_y = (
-                A * pr / hi_z,
-                A * pr / low_z,
-            )  # Establish limits on y consistent with reasonable Z range
-
-            def fy(y):  # Eq 3.43
-                x = (
-                    (y + y ** 2 + y ** 3 - y ** 4) / (1 - y) ** 3
-                    - A * pr
-                    - B * y ** 2
-                    + C * y ** D
-                )
-                return x
-
-            y = brentq(fy, low_y, high_y)
-
-            zout.append(A * pr / y)
+        for pr in pprs:
+            yi = a*pr / z_wyw(pr, 1/tr) # First guess
+            niter, y = 0, 0.01
+            while (abs(y-yi)/y) > 0.0005 and niter < 100: 
+                # Newton Raphson
+                y = yi - (f(yi, a, b, c, D, pr) / df(yi, a, b, c, D))
+                niter += 1
+                yi = y
+            zout.append(a * pr / y)
+                
         if single_p:
             return zout[0]
         else:
             return np.array(zout)
 
-    # Gas Z-Factor from Wang, Ye & Wu (2021)
-    def z_wyw(p, degf, sg, tc, pc):
-        a = [
-            0,
-            256.41675,
-            7.18202,
-            -178.5725,
-            182.98704,
-            -40.74427,
-            2.24427,
-            47.44825,
-            5.2852,
-            -0.14914,
-            271.50446,
-            16.2694,
-            -121.51728,
-            167.71477,
-            -81.73093,
-            20.36191,
-            -2.1177,
-            124.64444,
-            -6.74331,
-            0.20897,
-            -0.00314
-        ]
-        single_p = False
-        if p.size == 1:
-            single_p = True
-            ps = [p]
-        else:
-            ps = p.tolist()
+    # Wang, Ye & Wu, 2021, 0.2 < Ppr < 30, 1.05 < tpr < 3.0
+    # "An accurate correlation for calculating natural gas compressibility factors under a wide range of pressure conditions"
+    # https://doi.org/10.1016/j.egyr.2021.11.029
+    def z_wyw(pprs, tr):
+        a = [0, 256.41675, 7.18202, -178.5725, 182.98704, -40.74427, 2.24427, 47.44825, 5.2852, -0.14914, 271.50446, 16.2694, -121.51728, 167.71477, -81.73093, 20.36191, -2.1177, 124.64444, -6.74331, 0.20897, -0.00314]
+        numerators = a[1] + a[2] * (1 + a[3] * tr + a[4] * tr ** 2 + a[5] * tr ** 3 + a[6] * tr ** 4) * pprs + a[7] * pprs ** 2 + a[8] * pprs ** 3 + a[9] * pprs ** 4
+        denominators = a[10] + a[11] * (1 + a[12] * tr + a[13] * tr ** 2 + a[14] * tr ** 3 + a[15] * tr ** 4 + a[16] * tr ** 5) * pprs + a[17] * pprs ** 2 + a[18] * pprs ** 3 + a[19] * pprs ** 4 + a[20] * pprs ** 5
+        zs = numerators/denominators
 
-        zout = []
-        tr = (degf + f2r) / tc
-
-        for p in ps:
-            pr = p / pc
-            numerator = (
-                a[1]
-                + a[2]
-                * (
-                    1
-                    + a[3] * tr
-                    + a[4] * tr ** 2
-                    + a[5] * tr ** 3
-                    + a[6] * tr ** 4
-                )
-                * pr
-                + a[7] * pr ** 2
-                + a[8] * pr ** 3
-                + a[9] * pr ** 4
-            )
-            denominator = (
-                a[10]
-                + a[11]
-                * (
-                    1
-                    + a[12] * tr
-                    + a[13] * tr ** 2
-                    + a[14] * tr ** 3
-                    + a[15] * tr ** 4
-                    + a[16] * tr ** 5
-                )
-                * pr
-                + a[17] * pr ** 2
-                + a[18] * pr ** 3
-                + a[19] * pr ** 4
-                + a[20] * pr ** 5
-            )
-            zout.append(numerator / denominator)
         if single_p:
-            return zout[0]
+            return float(zs)
         else:
-            return np.array(zout)
+            return zs
+
 
     zfuncs = {"DAK": zdak, "HY": z_hy, "WYW": z_wyw}
 
-    return zfuncs[zmethod.name](p, degf, sg, tc, pc)
+    return zfuncs[zmethod.name](pprs, tr)
 
 
 def gas_ug(
     p: npt.ArrayLike,
     sg: float,
     degf: float,
     zmethod: z_method = z_method.DAK,
```

### Comparing `pyrestoolbox-1.3.8/pyrestoolbox/simtools/simtools.py` & `pyrestoolbox-1.3.9/pyrestoolbox/simtools/simtools.py`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.3.8/pyrestoolbox.egg-info/PKG-INFO` & `pyrestoolbox-1.3.9/pyrestoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestoolbox
-Version: 1.3.8
+Version: 1.3.9
 Summary: pyResToolbox - A collection of Reservoir Engineering Utilities
 Home-page: https://github.com/mwburgoyne/pyResToolbox
 Author: Mark W. Burgoyne
 Author-email: mark.w.burgoyne@gmail.com
 Keywords: restoolbox,petroleum,reservoir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -40,14 +40,17 @@
     ECLIPSE
 -   Creation of Corey and LET relative permeability tables in Eclipse
     format
 
 Apologies in advance that it is only in oilfield
 units with no current plans to add multi-unit support.
 
+Changelist in 1.3.9:
+- Tweaks to speed DAK and Hall & Yarborough Z-Factor calculations
+
 Changelist in 1.3.8:
 - Fix bug in Hall & Yarborough Z-Factor calculation
 
 Changelist in 1.3.5:
 - Fix bug in ECL deck zip/check recursion
 
 Changelist in 1.3.4:
```

### Comparing `pyrestoolbox-1.3.8/setup.cfg` & `pyrestoolbox-1.3.9/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6465 7363  [metadata]..desc
 00000010: 7269 7074 696f 6e5f 6669 6c65 203d 2052  ription_file = R
 00000020: 4541 444d 452e 6d64 0d0a 6e61 6d65 203d  EADME.md..name =
 00000030: 2070 7972 6573 746f 6f6c 626f 780d 0a76   pyrestoolbox..v
-00000040: 6572 7369 6f6e 203d 2031 2e33 2e38 0d0a  ersion = 1.3.8..
+00000040: 6572 7369 6f6e 203d 2031 2e33 2e39 0d0a  ersion = 1.3.9..
 00000050: 6175 7468 6f72 203d 204d 6172 6b20 572e  author = Mark W.
 00000060: 2042 7572 676f 796e 650d 0a61 7574 686f   Burgoyne..autho
 00000070: 725f 656d 6169 6c20 3d20 6d61 726b 2e77  r_email = mark.w
 00000080: 2e62 7572 676f 796e 6540 676d 6169 6c2e  .burgoyne@gmail.
 00000090: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 000000a0: 203d 2070 7952 6573 546f 6f6c 626f 7820   = pyResToolbox 
 000000b0: 2d20 4120 636f 6c6c 6563 7469 6f6e 206f  - A collection o
```

### Comparing `pyrestoolbox-1.3.8/setup.py` & `pyrestoolbox-1.3.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 #import markdown
 import importlib
 import collections
 import os
 import pkg_resources
 
 ROOT = os.path.abspath(os.path.dirname(__file__))
-f = open('C:\\Users\\vinom\OneDrive - Santos\\Work in progress\\ML Learning tidbits\\0-ResEng\\pyResToolbox\\source_dir\\README.md', 'r').read()
+f = open('C:\\Users\\vinom\OneDrive - Santos\\Work in progress\\Python\\0-ResEng\\pyResToolbox\\source_dir\\README.md', 'r').read()
 long_description= f #markdown.markdown( f.read() )
 
 setup(
     name = 'pyrestoolbox',
     packages = find_packages(),
     include_package_data=True,
-    version = '1.3.8',  # Ideally should be same as your GitHub release tag varsion
+    version = '1.3.9',  # Ideally should be same as your GitHub release tag varsion
     description = 'pyResToolbox - A collection of Reservoir Engineering Utilities',
     long_description= long_description,
     long_description_content_type = 'text/markdown',
     author = 'Mark W. Burgoyne',
     author_email = 'mark.w.burgoyne@gmail.com',
     url = 'https://github.com/mwburgoyne/pyResToolbox',
     keywords = ['restoolbox', 'petroleum', 'reservoir'],
```

