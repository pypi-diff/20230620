# Comparing `tmp/econoplots-0.1.2.tar.gz` & `tmp/econoplots-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econoplots-0.1.2.tar", last modified: Wed May 31 13:28:56 2023, max compression
+gzip compressed data, was "econoplots-0.1.3.tar", last modified: Tue Jun 20 15:45:25 2023, max compression
```

## Comparing `econoplots-0.1.2.tar` & `econoplots-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-05-31 13:28:56.748229 econoplots-0.1.2/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1053 2023-05-19 14:19:37.000000 econoplots-0.1.2/LICENSE
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-05-31 13:28:56.748229 econoplots-0.1.2/PKG-INFO
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      799 2023-05-19 14:40:50.000000 econoplots-0.1.2/README.md
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-05-31 13:28:56.748229 econoplots-0.1.2/econoplots/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       22 2023-05-31 13:27:50.000000 econoplots-0.1.2/econoplots/__init__.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     4945 2023-05-10 21:36:54.000000 econoplots-0.1.2/econoplots/_standalone_plotters.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2029 2023-05-10 18:47:46.000000 econoplots-0.1.2/econoplots/color_map.json
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2392 2023-05-19 15:01:31.000000 econoplots-0.1.2/econoplots/colors.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1375 2023-05-23 14:35:40.000000 econoplots-0.1.2/econoplots/converter.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      878 2023-05-22 17:38:56.000000 econoplots-0.1.2/econoplots/params.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    11934 2023-05-31 13:26:26.000000 econoplots-0.1.2/econoplots/utils.py
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-05-31 13:28:56.748229 econoplots-0.1.2/econoplots.egg-info/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-05-31 13:28:56.000000 econoplots-0.1.2/econoplots.egg-info/PKG-INFO
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      457 2023-05-31 13:28:56.000000 econoplots-0.1.2/econoplots.egg-info/SOURCES.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-05-31 13:28:56.000000 econoplots-0.1.2/econoplots.egg-info/dependency_links.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-05-10 17:37:10.000000 econoplots-0.1.2/econoplots.egg-info/not-zip-safe
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       40 2023-05-31 13:28:56.000000 econoplots-0.1.2/econoplots.egg-info/requires.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       11 2023-05-31 13:28:56.000000 econoplots-0.1.2/econoplots.egg-info/top_level.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1336 2023-05-22 17:38:24.000000 econoplots-0.1.2/pyproject.toml
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       38 2023-05-31 13:28:56.748229 econoplots-0.1.2/setup.cfg
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       60 2023-05-10 17:07:57.000000 econoplots-0.1.2/setup.py
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-05-31 13:28:56.748229 econoplots-0.1.2/tests/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      681 2023-05-23 15:37:46.000000 econoplots-0.1.2/tests/test_converter.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      734 2023-05-18 20:49:32.000000 econoplots-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-06-20 15:45:25.624873 econoplots-0.1.3/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1053 2023-05-19 14:19:37.000000 econoplots-0.1.3/LICENSE
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-06-20 15:45:25.624873 econoplots-0.1.3/PKG-INFO
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      799 2023-05-19 14:40:50.000000 econoplots-0.1.3/README.md
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-06-20 15:45:25.624873 econoplots-0.1.3/econoplots/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       22 2023-06-20 15:42:45.000000 econoplots-0.1.3/econoplots/__init__.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     4957 2023-05-31 14:08:21.000000 econoplots-0.1.3/econoplots/_standalone_plotters.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3345 2023-06-01 18:36:30.000000 econoplots-0.1.3/econoplots/color_map.json
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3049 2023-06-01 18:36:24.000000 econoplots-0.1.3/econoplots/colors.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3752 2023-06-20 15:42:33.000000 econoplots-0.1.3/econoplots/converter.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      960 2023-06-20 15:25:38.000000 econoplots-0.1.3/econoplots/params.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    21758 2023-06-20 15:30:30.000000 econoplots-0.1.3/econoplots/utils.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-06-20 15:45:25.624873 econoplots-0.1.3/econoplots.egg-info/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-06-20 15:45:25.000000 econoplots-0.1.3/econoplots.egg-info/PKG-INFO
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      457 2023-06-20 15:45:25.000000 econoplots-0.1.3/econoplots.egg-info/SOURCES.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-06-20 15:45:25.000000 econoplots-0.1.3/econoplots.egg-info/dependency_links.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-05-10 17:37:10.000000 econoplots-0.1.3/econoplots.egg-info/not-zip-safe
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       40 2023-06-20 15:45:25.000000 econoplots-0.1.3/econoplots.egg-info/requires.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       11 2023-06-20 15:45:25.000000 econoplots-0.1.3/econoplots.egg-info/top_level.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1336 2023-05-31 20:11:16.000000 econoplots-0.1.3/pyproject.toml
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       38 2023-06-20 15:45:25.624873 econoplots-0.1.3/setup.cfg
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       60 2023-05-10 17:07:57.000000 econoplots-0.1.3/setup.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-06-20 15:45:25.624873 econoplots-0.1.3/tests/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1775 2023-06-20 15:00:16.000000 econoplots-0.1.3/tests/test_converter.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      734 2023-05-18 20:49:32.000000 econoplots-0.1.3/tests/test_utils.py
```

### Comparing `econoplots-0.1.2/LICENSE` & `econoplots-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `econoplots-0.1.2/PKG-INFO` & `econoplots-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econoplots
-Version: 0.1.2
+Version: 0.1.3
 Summary: Formats Matplotlib plots into the style of The Economist
 Author-email: Dylan Penn <dylan.penn@vt.edu>
 License: Copyright (c) 2022 Dylan Penn
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

### Comparing `econoplots-0.1.2/README.md` & `econoplots-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `econoplots-0.1.2/econoplots/_standalone_plotters.py` & `econoplots-0.1.3/econoplots/_standalone_plotters.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 # Third Party Imports
 import matplotlib as mpl
 from cycler import cycler
 from matplotlib import pyplot as plt
 from matplotlib.figure import Figure
 from numpy import absolute, linspace, ndarray
 
+# Econoplots Imports
 # econoplots Imports
 from econoplots.utils import (
     makePatchSpinesInvisible,
     padXAxis,
-    setDefaultYAxisParams,
+    setLineYAxisParams,
 )
 
 # %% Load color map
 with open("econoplots/color_map.json") as json_file:
     color_map = json.load(json_file)
 
 # %% MPL Params
@@ -87,15 +88,15 @@
             ax.fill_between(x, shaded[i][0], shaded[i][1], alpha=0.5)
 
     # set ax labels
     ax.set(xlabel=x_ax_label)
     ax.set(ylabel=y_ax_label)
 
     # set y-axis params
-    setDefaultYAxisParams(ax, "left")
+    setLineYAxisParams(ax, "left")
 
     # delete top, right, left spines
     makePatchSpinesInvisible(ax, ["top", "right", "left"])
 
     # pad left side of x-axis
     padXAxis(ax, "left")
 
@@ -149,15 +150,15 @@
     # set ax1 colors and labels
     ax1.yaxis.label.set_color(ax1.lines[0].get_color())  # tick label color
     ax1.yaxis.set_tick_params(
         labelcolor=ax1.lines[0].get_color()
     )  # set tick color
 
     # set ax2 colors and labels
-    setDefaultYAxisParams(ax2, "right")
+    setLineYAxisParams(ax2, "right")
     ax2.yaxis.label.set_color(ax2.lines[0].get_color())  # tick label color
     ax2.yaxis.set_tick_params(
         labelcolor=ax2.lines[0].get_color(), colors="#FFFFFF"
     )  # set tick color to transparent
 
     # scale ylimits to align yticks between ax2 and ax1
     pad1 = absolute(ax1.get_ylim()[0] - ax1.get_yticks()[1])
```

### Comparing `econoplots-0.1.2/econoplots/colors.py` & `econoplots-0.1.3/econoplots/colors.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,38 @@
     "cyan": "#3EBCD2",
     "green": "#379A8B",
     "yellow": "#EBB434",
     "olive": "#B4BA39",
     "purple": "#9A607F",
     "gold": "#D1B07C",
     "grey": "#758D99",
+    "red1": "#A81829",
+    "red2": "#C7303C",
+    "red3": "#E64E53",
+    "red4": "#FF6B6C",
+    "red5": "#FF8785",
+    "red6": "#FFA39F",
+    "blue1": "#00588D",
+    "blue2": "#1270A8",
+    "blue3": "#3D89C3",
+    "blue4": "#5DA4DF",
+    "blue5": "#7BBFFC",
+    "blue6": "#98DAFF",
+    "green1": "#005F52",
+    "green2": "#00786B",
+    "green3": "#2E9284",
+    "green4": "#4DAD9E",
+    "green5": "#69C9B9",
+    "green6": "#86E5D4",
+    "purple1": "#78405F",
+    "purple2": "#925977",
+    "purple3": "#AD7291",
+    "purple4": "#C98CAC",
+    "purple5": "#E6A6C7",
+    "purple6": "#FFC2E3",
     "grey1": "#758D99",
     "grey2": "#3F5661",
     "grey3": "#6F8793",
     "grey4": "#89A2AE",
     "grey5": "#A4BDC9",
     "grey6": "#BFD8E5",
 }
@@ -72,24 +96,26 @@
 
 
 if __name__ == "__main__":
     # Run to save color map JSON file.
     colors_print_dict = _normalizeRGBdict(colors_print_dict)
 
     cm_web_main = [colors_web_dict.get(key) for key in main_keys]
+    cm_web_all = colors_web_dict
 
     line_chart_keys = ["blue1", "blue2", "gold", "burgundy", "dark_teal", "tan"]
     cm_line_chart = [colors_print_dict.get(key) for key in line_chart_keys]
 
     grey_keys = ["grey" + str(x) for x in range(1, 7)]
     colors_greys = [colors_web_dict.get(key) for key in grey_keys]
 
     color_map_master = {
         "print": colors_print_dict,
-        "web": cm_web_main,
+        "web_main": cm_web_main,
+        "web_all": cm_web_all,
         "line_chart": cm_line_chart,
         "greys": colors_greys,
         "grid": grid_color,
     }
 
     json_obj = json.dumps(color_map_master)
     with open("econoplots/color_map.json", "w") as outfile:
```

### Comparing `econoplots-0.1.2/econoplots/params.py` & `econoplots-0.1.3/econoplots/params.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,7 +27,9 @@
     mpl.rcParams["lines.linestyle"] = "-"
     mpl.rcParams["lines.linewidth"] = 3
     mpl.rcParams["axes.prop_cycle"] = cycler(color=color_map["line_chart"])
     mpl.rcParams["figure.facecolor"] = "w"
     mpl.rcParams["axes.facecolor"] = "w"
     mpl.rcParams["xtick.major.size"] = 6  # length of tick marks
     mpl.rcParams["xtick.minor.size"] = 3
+    mpl.rcParams["ytick.major.size"] = 0
+    mpl.rcParams["ytick.minor.size"] = 0
```

### Comparing `econoplots-0.1.2/econoplots.egg-info/PKG-INFO` & `econoplots-0.1.3/econoplots.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econoplots
-Version: 0.1.2
+Version: 0.1.3
 Summary: Formats Matplotlib plots into the style of The Economist
 Author-email: Dylan Penn <dylan.penn@vt.edu>
 License: Copyright (c) 2022 Dylan Penn
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

### Comparing `econoplots-0.1.2/pyproject.toml` & `econoplots-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `econoplots-0.1.2/tests/test_utils.py` & `econoplots-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

