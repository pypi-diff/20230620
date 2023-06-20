# Comparing `tmp/rtc-tools-diagnostics-0.1.3.tar.gz` & `tmp/rtc-tools-diagnostics-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc-tools-diagnostics-0.1.3.tar", last modified: Wed Jun 14 12:45:54 2023, max compression
+gzip compressed data, was "rtc-tools-diagnostics-0.2.0.tar", last modified: Tue Jun 20 13:01:08 2023, max compression
```

## Comparing `rtc-tools-diagnostics-0.1.3.tar` & `rtc-tools-diagnostics-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:45:54.721439 rtc-tools-diagnostics-0.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-14 12:45:53.000000 rtc-tools-diagnostics-0.1.3/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)      406 2023-06-14 12:45:54.721439 rtc-tools-diagnostics-0.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-06-14 12:45:53.000000 rtc-tools-diagnostics-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:45:54.720439 rtc-tools-diagnostics-0.1.3/rtc_tools_diagnostics.egg-info/
--rw-r--r--   0 root         (0) root         (0)      406 2023-06-14 12:45:54.000000 rtc-tools-diagnostics-0.1.3/rtc_tools_diagnostics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      511 2023-06-14 12:45:54.000000 rtc-tools-diagnostics-0.1.3/rtc_tools_diagnostics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 12:45:54.000000 rtc-tools-diagnostics-0.1.3/rtc_tools_diagnostics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-14 12:45:54.000000 rtc-tools-diagnostics-0.1.3/rtc_tools_diagnostics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-14 12:45:54.000000 rtc-tools-diagnostics-0.1.3/rtc_tools_diagnostics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:45:54.722439 rtc-tools-diagnostics-0.1.3/rtctools_diagnostics/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-14 12:45:53.000000 rtc-tools-diagnostics-0.1.3/rtctools_diagnostics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-14 12:45:54.722439 rtc-tools-diagnostics-0.1.3/rtctools_diagnostics/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2039 2023-06-14 12:45:53.000000 rtc-tools-diagnostics-0.1.3/rtctools_diagnostics/export_results.py
--rw-rw-rw-   0 root         (0) root         (0)    14125 2023-06-14 12:45:53.000000 rtc-tools-diagnostics-0.1.3/rtctools_diagnostics/get_linear_problem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:45:54.721439 rtc-tools-diagnostics-0.1.3/rtctools_diagnostics/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 12:45:53.000000 rtc-tools-diagnostics-0.1.3/rtctools_diagnostics/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5447 2023-06-14 12:45:53.000000 rtc-tools-diagnostics-0.1.3/rtctools_diagnostics/utils/casadi_to_lp.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-06-14 12:45:54.721439 rtc-tools-diagnostics-0.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-06-14 12:45:53.000000 rtc-tools-diagnostics-0.1.3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2023-06-14 12:45:53.000000 rtc-tools-diagnostics-0.1.3/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:01:08.254689 rtc-tools-diagnostics-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-20 13:01:07.000000 rtc-tools-diagnostics-0.2.0/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)      406 2023-06-20 13:01:08.254689 rtc-tools-diagnostics-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2023-06-20 13:01:07.000000 rtc-tools-diagnostics-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:01:08.252689 rtc-tools-diagnostics-0.2.0/rtc_tools_diagnostics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-06-20 13:01:08.000000 rtc-tools-diagnostics-0.2.0/rtc_tools_diagnostics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      511 2023-06-20 13:01:08.000000 rtc-tools-diagnostics-0.2.0/rtc_tools_diagnostics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 13:01:08.000000 rtc-tools-diagnostics-0.2.0/rtc_tools_diagnostics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-20 13:01:08.000000 rtc-tools-diagnostics-0.2.0/rtc_tools_diagnostics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 13:01:08.000000 rtc-tools-diagnostics-0.2.0/rtc_tools_diagnostics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:01:08.254689 rtc-tools-diagnostics-0.2.0/rtctools_diagnostics/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-20 13:01:07.000000 rtc-tools-diagnostics-0.2.0/rtctools_diagnostics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-20 13:01:08.254689 rtc-tools-diagnostics-0.2.0/rtctools_diagnostics/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2039 2023-06-20 13:01:07.000000 rtc-tools-diagnostics-0.2.0/rtctools_diagnostics/export_results.py
+-rw-rw-rw-   0 root         (0) root         (0)    14243 2023-06-20 13:01:07.000000 rtc-tools-diagnostics-0.2.0/rtctools_diagnostics/get_linear_problem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 13:01:08.254689 rtc-tools-diagnostics-0.2.0/rtctools_diagnostics/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 13:01:07.000000 rtc-tools-diagnostics-0.2.0/rtctools_diagnostics/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5447 2023-06-20 13:01:07.000000 rtc-tools-diagnostics-0.2.0/rtctools_diagnostics/utils/casadi_to_lp.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-06-20 13:01:08.254689 rtc-tools-diagnostics-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-06-20 13:01:07.000000 rtc-tools-diagnostics-0.2.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2023-06-20 13:01:07.000000 rtc-tools-diagnostics-0.2.0/versioneer.py
```

### Comparing `rtc-tools-diagnostics-0.1.3/COPYING.LESSER` & `rtc-tools-diagnostics-0.2.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-diagnostics-0.1.3/rtctools_diagnostics/export_results.py` & `rtc-tools-diagnostics-0.2.0/rtctools_diagnostics/export_results.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-diagnostics-0.1.3/rtctools_diagnostics/get_linear_problem.py` & `rtc-tools-diagnostics-0.2.0/rtctools_diagnostics/get_linear_problem.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 def get_constraints(casadi_equations):
     """ Get constraints in human-readable format"""
     return casadi_to_lp(casadi_equations)
 
 
 def evaluate_constraints(results, nlp):
     """ Evaluate the constraints wrt to the optimized solution """
-    x_optimized = np.array(results["x"]).ravel()
+    x_optimized = results["x_ravel"]
     X_sx = ca.SX.sym("X", *nlp["x"].shape)
     expand_fg = ca.Function("f_g", [nlp["x"]], [nlp["f"], nlp["g"]]).expand()
     _f_sx, g_sx = expand_fg(X_sx)
     eval_g = ca.Function("g_eval", [X_sx], [g_sx]).expand()
     evaluated_g = [x[0] for x in np.array(eval_g(x_optimized))]
     return evaluated_g
 
@@ -127,23 +127,23 @@
         lam_x, lam_tol
     )
     upper_bound_variable_hits = find_variable_hits(
         lam_x_larger_than_zero,
         lbx,
         ubx,
         variable_names,
-        np.array(results["x"]).ravel(),
+        results["x_ravel"],
         lam_x,
     )
     lower_bound_variable_hits = find_variable_hits(
         lam_x_smaller_than_zero,
         lbx,
         ubx,
         variable_names,
-        np.array(results["x"]).ravel(),
+        results["x_ravel"],
         lam_x,
     )
     upper_bound_dict = convert_to_dict_per_var(upper_bound_variable_hits)
     lower_bound_dict = convert_to_dict_per_var(lower_bound_variable_hits)
 
     # Upper and lower constraints
     lam_g_larger_than_zero, lam_g_smaller_than_zero = get_tol_exceedance(
@@ -333,23 +333,27 @@
     lam_tol = 0.1
     manual_expansion = True
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.problem_and_results_list = []
 
-    def solver_finished(self, results, nlp, lbx, ubx, lbg, ubg, x0, priority=None):
-        super().solver_finished(nlp, results, lbx, ubx, lbg, ubg, x0, priority)
+    def priority_completed(self, priority):
+        super().priority_completed(priority)
+        lbx, ubx, lbg, ubg, x0, nlp = self.transcribed_problem.values()
         expand_f_g = ca.Function("f_g", [nlp["x"]], [nlp["f"], nlp["g"]]).expand()
         casadi_equations = {}
         casadi_equations[
             "indices"
         ] = self._CollocatedIntegratedOptimizationProblem__indices
         casadi_equations["func"] = expand_f_g
         casadi_equations["other"] = (lbx, ubx, lbg, ubg, x0)
+        lam_g, lam_x = self.lagrange_multipliers
+        x_ravel = self.solver_output
+        results = {"lam_g": lam_g, "lam_x": lam_x, "x_ravel": x_ravel}
         self.problem_and_results_list.append((priority, results, nlp, casadi_equations))
 
     def post(self):
         super().post()
 
         result_text = ""
         if len(self.problem_and_results_list) == 0:
```

### Comparing `rtc-tools-diagnostics-0.1.3/rtctools_diagnostics/utils/casadi_to_lp.py` & `rtc-tools-diagnostics-0.2.0/rtctools_diagnostics/utils/casadi_to_lp.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-diagnostics-0.1.3/setup.py` & `rtc-tools-diagnostics-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-diagnostics-0.1.3/versioneer.py` & `rtc-tools-diagnostics-0.2.0/versioneer.py`

 * *Files identical despite different names*

