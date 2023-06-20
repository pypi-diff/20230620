# Comparing `tmp/jupyter-utility-widgets-0.0.1a1.tar.gz` & `tmp/jupyter-utility-widgets-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-utility-widgets-0.0.1a1.tar", last modified: Sat Jun 17 22:34:41 2023, max compression
+gzip compressed data, was "jupyter-utility-widgets-0.0.1a2.tar", last modified: Tue Jun 20 17:05:29 2023, max compression
```

## Comparing `jupyter-utility-widgets-0.0.1a1.tar` & `jupyter-utility-widgets-0.0.1a2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.644863 jupyter-utility-widgets-0.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/file_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/filter_design.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/specgram.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/specgram_examiner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/selector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/selector/index_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/utility/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/utility/numpy_parameter_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:34:41.640863 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-17 22:34:41.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-17 22:34:41.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:34:41.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-17 22:34:41.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-17 22:34:41.000000 jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-17 22:34:29.000000 jupyter-utility-widgets-0.0.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 22:34:41.644863 jupyter-utility-widgets-0.0.1a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.227021 jupyter-utility-widgets-0.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-20 17:05:29.227021 jupyter-utility-widgets-0.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.223021 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/file_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/filter_design.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.223021 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.227021 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/specgram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/specgram_examiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.227021 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/selector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/selector/index_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.227021 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/utility/numpy_parameter_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:05:29.223021 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-20 17:05:29.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-20 17:05:29.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:05:29.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 17:05:29.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 17:05:29.000000 jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-20 17:05:19.000000 jupyter-utility-widgets-0.0.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:05:29.227021 jupyter-utility-widgets-0.0.1a2/setup.cfg
```

### Comparing `jupyter-utility-widgets-0.0.1a1/LICENSE` & `jupyter-utility-widgets-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a1/PKG-INFO` & `jupyter-utility-widgets-0.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.1a1
+Version: 0.0.1a2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-utility
 
 Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
```

### Comparing `jupyter-utility-widgets-0.0.1a1/README.md` & `jupyter-utility-widgets-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/file_explorer.py` & `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/file_explorer.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/filter_design.py` & `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/filter_design.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from jupyter_utility_widgets.plot.filter import Filter
-from jupyter_utility_widgets.utility.numpy_parameter_converter import NumpyFunctionUIFactory
+from jupyter_utility_widgets.utility.numpy_parameter_converter import NumpyFunctionUIFactory, SKIP_PARAMETER
 from ipywidgets import HBox, VBox, Dropdown, BoundedIntText, BoundedFloatText
 from traitlets import Any, Unicode
 from scipy.signal import windows, firwin
 available_windows = list(filter(lambda s: not (s.startswith("_") or s in ["get_window"]), dir(windows))) + ["manual"]
 class WindowSelect(VBox):
     manual = Any()
     value = Any()
@@ -11,24 +11,25 @@
     def __init__(self, **kwargs):
         self.window_func_selector = Dropdown(options=available_windows, **kwargs)
         self.extras = VBox([])
 
         super().__init__(children=[self.window_func_selector, self.extras])
 
         self.window_func_selector.observe(lambda evt: self._handle_window_change(evt.new), names=["value"])
+        self._handle_window_change(self.window_func_selector.value)
 
     def _handle_window_change(self, window_name):
         self.set_extras(window_name)
         self.update_value()
     
     def set_extras(self, window_name):
         func = getattr(windows, window_name)
         parameters, parameters_types = NumpyFunctionUIFactory.get_parameter_types(func)
-        parameters_types.pop('M')
-        parameters_types.pop('sym')
+        parameters_types['M'] = SKIP_PARAMETER
+        parameters_types["sym"] = SKIP_PARAMETER
 
         for child in self.extras.children:
             child.unobserve_all()
 
         self.extras.children = NumpyFunctionUIFactory.construct_widgets(parameters, parameters_types)
         
         for child in self.extras.children:
@@ -56,14 +57,16 @@
             self.cutoff_input,
             self.window_selector,
         ]
         super().__init__(children, **kwargs)
 
         for child in children:
             child.observe(lambda evt: self.calc_filt(),names=["value"])
+        
+        self.calc_filt()
     
     def calc_filt(self, ):
         self.value = firwin(
             self.window_length.value,
             self.cutoff_input.value,
             window=self.window_selector.value
         )
@@ -71,8 +74,9 @@
 class FilterDesign(HBox):
     def __init__(self, **kwargs):
         self.filter_plot = Filter()
         self.design_controls = FilterDesignControls()
         children = [self.filter_plot, self.design_controls]
         super().__init__(children, **kwargs)
 
-        self.design_controls.observe(lambda evt: self.filter_plot.update(evt.new))
+        self.design_controls.observe(lambda evt: self.filter_plot.update(evt.new), names=["value"])
+        self.filter_plot.update(self.design_controls.value)
```

### Comparing `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/base.py` & `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,16 @@
             self.axes = [axes]
         else:
             self.axes = list(axes.reshape(-1,))
         children = [self.fig.canvas]
 
         super().__init__(children, **kwargs)
 
-    @abstractmethod
-    def update(self, data):
-        raise NotImplementedError()
+    def update(self, data=None):
+        self.fig.canvas.draw()
+        self.fig.canvas.flush_events()
     
     @abstractmethod
     def select(self, x=None, y=None, z=None):
         raise NotImplementedError()
```

### Comparing `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/lines.py` & `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/lines.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,16 @@
             x, y = data[name]
             line = self.lines[name]
             line.set_xdata(x)
             line.set_ydata(y)
 
         if self.autoscale:
              self._autoscale()
+        
+        super().update()
     
     def _autoscale(self,):
         xmin = None
         xmax = None
         ymin = None
         ymax = None
         for line in self.lines.values():
@@ -34,8 +36,9 @@
             if ymin is None or (ydata.min()) < xmin:
                 ymin = ydata.min()
             
             if ymax is None or (ydata.max()) < ymax:
                 ymax = ydata.max()
         self.ax.set_xlim([xmin, xmax])
         self.ax.set_ylim([ymin, ymax])
+
```

### Comparing `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/figures/specgram.py` & `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/figures/specgram.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,8 +18,9 @@
     def update(self, data):
         self.ax.cla()
 
         if data is None:
             return
 
         _, freqs,_,_ = self.ax.specgram(data, *self.spec_args, **self.spec_kwargs)
-        self.sample_rate = freqs[-1]*2
+        self.sample_rate = freqs[-1]*2
+        super().update()
```

### Comparing `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/filter.py` & `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/filter.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/plot/specgram_examiner.py` & `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/plot/specgram_examiner.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/selector/index_selector.py` & `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/selector/index_selector.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets/utility/numpy_parameter_converter.py` & `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets/utility/numpy_parameter_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     @staticmethod
     def construct_widgets(parameters: List[Parameter], parameter_types=None):
         if parameter_types is None:
             parameter_types = NumpyFunctionUIFactory.get_parameter_types(parameters)
 
         widgets = []
         for parameter in parameters:
-            current_type = parameter_types.get(parameter.name, SKIP_PARAMETER)
+            current_type = parameter_types.get(parameter.name)
             
             if current_type is None:
                 if "optional" not in parameter.type:
                     warn("Missing type '%s' for non-optional parameter %s" % (parameter.type, parameter.name))
                 continue
             
             if current_type == SKIP_PARAMETER:
```

### Comparing `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/PKG-INFO` & `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.1a1
+Version: 0.0.1a2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-utility
 
 Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
```

### Comparing `jupyter-utility-widgets-0.0.1a1/jupyter_utility_widgets.egg-info/SOURCES.txt` & `jupyter-utility-widgets-0.0.1a2/jupyter_utility_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

