# Comparing `tmp/mindstorm-0.8.1.tar.gz` & `tmp/mindstorm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindstorm-0.8.1.tar", last modified: Wed May 19 18:59:45 2021, max compression
+gzip compressed data, was "mindstorm-0.9.0.tar", last modified: Wed Jul 20 22:27:24 2022, max compression
```

## Comparing `mindstorm-0.8.1.tar` & `mindstorm-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 18:59:45.568743 mindstorm-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-05-19 18:59:35.000000 mindstorm-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      829 2021-05-19 18:59:45.568743 mindstorm-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      263 2021-05-19 18:59:35.000000 mindstorm-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-05-19 18:59:35.000000 mindstorm-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 18:59:45.568743 mindstorm-0.8.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3625 2021-05-19 18:59:35.000000 mindstorm-0.8.1/scripts/apply_clustsim_svc.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1208 2021-05-19 18:59:35.000000 mindstorm-0.8.1/scripts/lsvol
--rwxr-xr-x   0 runner    (1001) docker     (121)     3707 2021-05-19 18:59:35.000000 mindstorm-0.8.1/scripts/transform_func2mni.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     3007 2021-05-19 18:59:35.000000 mindstorm-0.8.1/scripts/transform_mni2func.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     4825 2021-05-19 18:59:35.000000 mindstorm-0.8.1/scripts/zstat_randomise.sh
--rw-r--r--   0 runner    (1001) docker     (121)      691 2021-05-19 18:59:45.568743 mindstorm-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-05-19 18:59:35.000000 mindstorm-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 18:59:45.564743 mindstorm-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 18:59:45.568743 mindstorm-0.8.1/src/mindstorm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-19 18:59:35.000000 mindstorm-0.8.1/src/mindstorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6229 2021-05-19 18:59:35.000000 mindstorm-0.8.1/src/mindstorm/dsmplot.py
--rw-r--r--   0 runner    (1001) docker     (121)     7670 2021-05-19 18:59:35.000000 mindstorm-0.8.1/src/mindstorm/prsa.py
--rw-r--r--   0 runner    (1001) docker     (121)     4800 2021-05-19 18:59:35.000000 mindstorm-0.8.1/src/mindstorm/statplot.py
--rw-r--r--   0 runner    (1001) docker     (121)     7835 2021-05-19 18:59:35.000000 mindstorm-0.8.1/src/mindstorm/subjutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-19 18:59:45.568743 mindstorm-0.8.1/src/mindstorm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      829 2021-05-19 18:59:45.000000 mindstorm-0.8.1/src/mindstorm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      491 2021-05-19 18:59:45.000000 mindstorm-0.8.1/src/mindstorm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-19 18:59:45.000000 mindstorm-0.8.1/src/mindstorm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-05-19 18:59:45.000000 mindstorm-0.8.1/src/mindstorm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-05-19 18:59:45.000000 mindstorm-0.8.1/src/mindstorm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 22:27:24.143875 mindstorm-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-07-20 22:27:15.000000 mindstorm-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      780 2022-07-20 22:27:24.143875 mindstorm-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-07-20 22:27:15.000000 mindstorm-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-07-20 22:27:15.000000 mindstorm-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 22:27:24.143875 mindstorm-0.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3625 2022-07-20 22:27:15.000000 mindstorm-0.9.0/scripts/apply_clustsim_svc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1208 2022-07-20 22:27:15.000000 mindstorm-0.9.0/scripts/lsvol
+-rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-07-20 22:27:15.000000 mindstorm-0.9.0/scripts/remove_short_runs.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2452 2022-07-20 22:27:15.000000 mindstorm-0.9.0/scripts/run_freesurfer.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-07-20 22:27:15.000000 mindstorm-0.9.0/scripts/smooth_susan
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3707 2022-07-20 22:27:15.000000 mindstorm-0.9.0/scripts/transform_func2mni.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3007 2022-07-20 22:27:15.000000 mindstorm-0.9.0/scripts/transform_mni2func.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4825 2022-07-20 22:27:15.000000 mindstorm-0.9.0/scripts/zstat_randomise.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2022-07-20 22:27:24.143875 mindstorm-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-07-20 22:27:15.000000 mindstorm-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 22:27:24.139874 mindstorm-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 22:27:24.143875 mindstorm-0.9.0/src/mindstorm/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 22:27:15.000000 mindstorm-0.9.0/src/mindstorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6229 2022-07-20 22:27:15.000000 mindstorm-0.9.0/src/mindstorm/dsmplot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7670 2022-07-20 22:27:15.000000 mindstorm-0.9.0/src/mindstorm/prsa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5929 2022-07-20 22:27:15.000000 mindstorm-0.9.0/src/mindstorm/statplot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7835 2022-07-20 22:27:15.000000 mindstorm-0.9.0/src/mindstorm/subjutil.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 22:27:24.143875 mindstorm-0.9.0/src/mindstorm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      780 2022-07-20 22:27:24.000000 mindstorm-0.9.0/src/mindstorm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2022-07-20 22:27:24.000000 mindstorm-0.9.0/src/mindstorm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-20 22:27:24.000000 mindstorm-0.9.0/src/mindstorm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-07-20 22:27:24.000000 mindstorm-0.9.0/src/mindstorm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-07-20 22:27:24.000000 mindstorm-0.9.0/src/mindstorm.egg-info/top_level.txt
```

### Comparing `mindstorm-0.8.1/LICENSE` & `mindstorm-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mindstorm-0.8.1/PKG-INFO` & `mindstorm-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mindstorm
-Version: 0.8.1
+Version: 0.9.0
 Summary: Mindstorm: Advanced analysis of neuroimaging data
 Home-page: https://github.com/mortonne/mindstorm
 Author: Neal Morton
 Author-email: mortonne@gmail.com
 License: GPL-3.0-or-later
-Description: # mindstorm
-        [![PyPI version](https://badge.fury.io/py/mindstorm.svg)](https://badge.fury.io/py/mindstorm)
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4248135.svg)](https://doi.org/10.5281/zenodo.4248135)
-        
-        Package for advanced neuroimaging analysis tools.
-        
 Keywords: fMRI,neuroimaging,RSA
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mindstorm
+[![PyPI version](https://badge.fury.io/py/mindstorm.svg)](https://badge.fury.io/py/mindstorm)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4248135.svg)](https://doi.org/10.5281/zenodo.4248135)
+
+Package for advanced neuroimaging analysis tools.
```

### Comparing `mindstorm-0.8.1/scripts/apply_clustsim_svc.sh` & `mindstorm-0.9.0/scripts/apply_clustsim_svc.sh`

 * *Files identical despite different names*

### Comparing `mindstorm-0.8.1/scripts/lsvol` & `mindstorm-0.9.0/scripts/lsvol`

 * *Files identical despite different names*

### Comparing `mindstorm-0.8.1/scripts/transform_func2mni.sh` & `mindstorm-0.9.0/scripts/transform_func2mni.sh`

 * *Files identical despite different names*

### Comparing `mindstorm-0.8.1/scripts/transform_mni2func.sh` & `mindstorm-0.9.0/scripts/transform_mni2func.sh`

 * *Files identical despite different names*

### Comparing `mindstorm-0.8.1/scripts/zstat_randomise.sh` & `mindstorm-0.9.0/scripts/zstat_randomise.sh`

 * *Files identical despite different names*

### Comparing `mindstorm-0.8.1/src/mindstorm/dsmplot.py` & `mindstorm-0.9.0/src/mindstorm/dsmplot.py`

 * *Files identical despite different names*

### Comparing `mindstorm-0.8.1/src/mindstorm/prsa.py` & `mindstorm-0.9.0/src/mindstorm/prsa.py`

 * *Files identical despite different names*

### Comparing `mindstorm-0.8.1/src/mindstorm/statplot.py` & `mindstorm-0.9.0/src/mindstorm/statplot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,53 @@
 """Plot statistics using Seaborn."""
 
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 
+def add_swarm_bar_sig(ax, sig_ind, y_offset=None):
+    """Add significance stats to swarm bar plot."""
+    # center of each bar in left/right order
+    bx = np.array(sorted([p.get_x() + (p.get_width() / 2) for p in ax.patches]))
+
+    # highest point in each point plot in left/right order
+    collections = [c for c in ax.collections if c.get_offsets().shape[0] > 1]
+    cy = np.array([np.max(c.get_offsets()[:, 1]) for c in collections])
+    cx = np.array([np.mean(c.get_offsets()[:, 0]) for c in collections])
+    cy = cy[np.argsort(cx)]
+
+    # define y point relative to the highest point
+    if y_offset is None:
+        y_lim = ax.get_ylim()
+        y_offset = (y_lim[1] - y_lim[0]) * .15
+
+    # plot significance markers
+    ax.plot(
+        bx[sig_ind],
+        cy[sig_ind] + y_offset,
+        markersize=8,
+        color='k',
+        linestyle='',
+        marker=(5, 2, 0),
+    )
+
+
 def plot_swarm_bar(
     data=None,
     x=None,
     y=None,
     hue=None,
     dark=None,
     light=None,
     dodge=False,
     point_kind='swarm',
     legend=True,
     width=None,
+    sig_ind=None,
     ax=None,
     point_kws={},
     bar_kws={},
 ):
     """
     Make a bar plot with individual points and error bars.
 
@@ -52,14 +80,17 @@
 
     legend : bool, optional
         If true, and the hue input is set, include a legend on the plot.
 
     width : float, optional
         Width of the bars.
 
+    sig_ind : list of int, optional
+        Indices of bars (from left to right) to label as significant.
+
     ax : matplotlib.axes.Axes, optional
         Axes object to draw the plot onto; if not specified, will use
         the current Axes.
 
     point_kws : dict, optional
         Options when plotting points using seaborn.swarmplot or
         seaborn.stripplot.
@@ -115,15 +146,15 @@
     sns.barplot(data=data, x=x, y=y, hue=hue, ax=ax, **bar_prop)
 
     # remove overall xlabel and increase size of x-tick labels
     ax.set_xlabel('')
     ax.tick_params(axis='x', labelsize='large')
 
     # fix ordering of plot elements
-    plt.setp(ax.lines, zorder=100, linewidth=1.25, label=None)
+    plt.setp(ax.lines, zorder=100, linewidth=1.25, label=None, clip_on=False)
     plt.setp(ax.collections, zorder=100, label=None)
 
     # modify the width of the bar plot
     if width is not None:
         bar_x = []
         for patch in ax.patches:
             # set width
@@ -143,14 +174,18 @@
     # delete legend (redundant with the x-tick labels)
     lg = ax.get_legend()
     if lg is not None:
         lg.remove()
         if hue is not None and legend:
             # refresh the legend to remove the swarm points
             ax.legend()
+
+    # add significance markers
+    if sig_ind is not None:
+        add_swarm_bar_sig(ax, sig_ind)
     return ax
 
 
 def plot_sig(x, y, spacing, line_kws={}, marker_kws={}, ax=None):
     """Plot brackets with a significance indicator."""
     if ax is None:
         ax = plt.gca()
```

### Comparing `mindstorm-0.8.1/src/mindstorm/subjutil.py` & `mindstorm-0.9.0/src/mindstorm/subjutil.py`

 * *Files identical despite different names*

### Comparing `mindstorm-0.8.1/src/mindstorm.egg-info/PKG-INFO` & `mindstorm-0.9.0/src/mindstorm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mindstorm
-Version: 0.8.1
+Version: 0.9.0
 Summary: Mindstorm: Advanced analysis of neuroimaging data
 Home-page: https://github.com/mortonne/mindstorm
 Author: Neal Morton
 Author-email: mortonne@gmail.com
 License: GPL-3.0-or-later
-Description: # mindstorm
-        [![PyPI version](https://badge.fury.io/py/mindstorm.svg)](https://badge.fury.io/py/mindstorm)
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4248135.svg)](https://doi.org/10.5281/zenodo.4248135)
-        
-        Package for advanced neuroimaging analysis tools.
-        
 Keywords: fMRI,neuroimaging,RSA
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mindstorm
+[![PyPI version](https://badge.fury.io/py/mindstorm.svg)](https://badge.fury.io/py/mindstorm)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4248135.svg)](https://doi.org/10.5281/zenodo.4248135)
+
+Package for advanced neuroimaging analysis tools.
```

