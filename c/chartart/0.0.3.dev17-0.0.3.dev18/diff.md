# Comparing `tmp/chartart-0.0.3.dev17.tar.gz` & `tmp/chartart-0.0.3.dev18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartart-0.0.3.dev17.tar", last modified: Wed Jun 14 20:59:57 2023, max compression
+gzip compressed data, was "chartart-0.0.3.dev18.tar", last modified: Tue Jun 20 13:44:15 2023, max compression
```

## Comparing `chartart-0.0.3.dev17.tar` & `chartart-0.0.3.dev18.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-14 20:59:57.048427 chartart-0.0.3.dev17/
--rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/LICENSE
--rw-r--r--   0 dhananjay   (504) staff       (20)     2336 2023-06-14 20:59:57.048776 chartart-0.0.3.dev17/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)     1814 2023-05-31 13:18:32.000000 chartart-0.0.3.dev17/README.md
--rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/pyproject.toml
--rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-06-14 20:59:57.050186 chartart-0.0.3.dev17/setup.cfg
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-14 20:59:57.027644 chartart-0.0.3.dev17/src/
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-14 20:59:57.038546 chartart-0.0.3.dev17/src/chartart/
--rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/conftest.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/helpers.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    84149 2023-06-14 18:51:32.000000 chartart-0.0.3.dev17/src/chartart/plot.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/simple_eda_template.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/test_plot.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-14 20:59:57.045651 chartart-0.0.3.dev17/src/chartart/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/tests/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/src/chartart/tests/test_simple.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-14 20:59:57.043469 chartart-0.0.3.dev17/src/chartart.egg-info/
--rw-r--r--   0 dhananjay   (504) staff       (20)     2336 2023-06-14 20:59:57.000000 chartart-0.0.3.dev17/src/chartart.egg-info/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-06-14 20:59:57.000000 chartart-0.0.3.dev17/src/chartart.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-06-14 20:59:57.000000 chartart-0.0.3.dev17/src/chartart.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-06-14 20:59:57.000000 chartart-0.0.3.dev17/src/chartart.egg-info/requires.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-06-14 20:59:57.000000 chartart-0.0.3.dev17/src/chartart.egg-info/top_level.txt
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-14 20:59:57.046923 chartart-0.0.3.dev17/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev17/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-20 13:44:15.572776 chartart-0.0.3.dev18/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/LICENSE
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2443 2023-06-20 13:44:15.573065 chartart-0.0.3.dev18/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1921 2023-06-20 13:39:39.000000 chartart-0.0.3.dev18/README.md
+-rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/pyproject.toml
+-rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-06-20 13:44:15.574754 chartart-0.0.3.dev18/setup.cfg
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-20 13:44:15.533692 chartart-0.0.3.dev18/src/
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-20 13:44:15.562196 chartart-0.0.3.dev18/src/chartart/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/conftest.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/helpers.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    86312 2023-06-20 13:39:50.000000 chartart-0.0.3.dev18/src/chartart/plot.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/simple_eda_template.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/test_plot.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-20 13:44:15.569925 chartart-0.0.3.dev18/src/chartart/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/tests/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/src/chartart/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-20 13:44:15.567939 chartart-0.0.3.dev18/src/chartart.egg-info/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2443 2023-06-20 13:44:15.000000 chartart-0.0.3.dev18/src/chartart.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-06-20 13:44:15.000000 chartart-0.0.3.dev18/src/chartart.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-06-20 13:44:15.000000 chartart-0.0.3.dev18/src/chartart.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-06-20 13:44:15.000000 chartart-0.0.3.dev18/src/chartart.egg-info/requires.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-06-20 13:44:15.000000 chartart-0.0.3.dev18/src/chartart.egg-info/top_level.txt
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-06-20 13:44:15.571831 chartart-0.0.3.dev18/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev18/tests/test_simple.py
```

### Comparing `chartart-0.0.3.dev17/LICENSE` & `chartart-0.0.3.dev18/LICENSE`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev17/PKG-INFO` & `chartart-0.0.3.dev18/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev17
+Version: 0.0.3.dev18
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
@@ -69,7 +69,11 @@
 - bar type : bar,column,stackedBar,stackedColumn,stackedBar,stackedBar100,stackedColumn100  
 - scatter : bubble , if size is specified as list of float scatter chart will get ploted as bubble chart
 
 0.0.3.dev14 => 0.0.3.dev15
 - Tree Map : c (color) param is optional
 - Map : shapeDataField is new optional param (defaults to key 'Name'). primaryValueMapper and data is optional parameters now. This will be usefull for markers/bubbles where we dont need these inputs.
 - Map : added support fo sub layers. 
+
+0.0.3.dev18
+- Added startAngle, endAngle, radius, groupTo in circular chart
+- Added number format on axis
```

### Comparing `chartart-0.0.3.dev17/README.md` & `chartart-0.0.3.dev18/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,8 +52,12 @@
 - line type : line, area, spline, stepLine, splineArea, stepArea, stackedLine, stackedArea, stackedArea100, stackedLine100
 - bar type : bar,column,stackedBar,stackedColumn,stackedBar,stackedBar100,stackedColumn100  
 - scatter : bubble , if size is specified as list of float scatter chart will get ploted as bubble chart
 
 0.0.3.dev14 => 0.0.3.dev15
 - Tree Map : c (color) param is optional
 - Map : shapeDataField is new optional param (defaults to key 'Name'). primaryValueMapper and data is optional parameters now. This will be usefull for markers/bubbles where we dont need these inputs.
-- Map : added support fo sub layers. 
+- Map : added support fo sub layers. 
+
+0.0.3.dev18
+- Added startAngle, endAngle, radius, groupTo in circular chart
+- Added number format on axis
```

### Comparing `chartart-0.0.3.dev17/setup.cfg` & `chartart-0.0.3.dev18/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chartart
-version = 0.0.3.dev17
+version = 0.0.3.dev18
 author = BR-Advisers
 author_email = info@br-advisers.com
 description = ChartArt python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `chartart-0.0.3.dev17/src/chartart/__init__.py` & `chartart-0.0.3.dev18/src/chartart/__init__.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev17/src/chartart/conftest.py` & `chartart-0.0.3.dev18/src/chartart/conftest.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev17/src/chartart/helpers.py` & `chartart-0.0.3.dev18/src/chartart/helpers.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev17/src/chartart/plot.py` & `chartart-0.0.3.dev18/src/chartart/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,15 +331,15 @@
          self.xAxisProperties['labelRotation'] = xAxisLabelRotation
 
     def set_xAxisIsVisible(self, xAxisIsVisible: bool):
          self.xAxisProperties['isVisible'] = xAxisIsVisible
 
     def set_xAxisDateFormat(self, xAxisDateFormat: str):
          self.xAxisProperties['dateFormat'] = xAxisDateFormat
-    
+
     def set_xAxisNumberFormat(self, xAxisNumberFormat: str):
          self.xAxisProperties['numberFormat'] = xAxisNumberFormat
 
     def set_xAxisNumberFormat(self, xAxisNumberFormat: str):
          self.xAxisProperties['numberFormat'] = xAxisNumberFormat
 
     def set_xAxisRangePadding(self, xAxisRangePadding: str):
@@ -1083,32 +1083,37 @@
             if sortOn is not None:
                 hist_info['sortOn'] = sortOn
             self.data.insert(hist_info)
 
             i += 1
 
     def pie(self, x: Union[list, np.ndarray, pd.Series], label: Union[list, np.ndarray, pd.Series, pd.Index],
-            c: Union[list,str] = None, animationDelay: Optional[float] = None, animationDuration: Optional[float] = None, animationType: Optional[str]='parallel'):
+            c: Union[list,str] = None, radius: Optional[str] = None, startAngle: Optional[int] = None, endAngle: Optional[int] = None, groupTo: Optional[int] = None, 
+            animationDelay: Optional[float] = None, animationDuration: Optional[float] = None, animationType: Optional[str]='parallel'):
         """
         Constructs a pie chart.
 
         :param x: A list, NumPy array, or Pandas series denoting the size of each pie.
         :param label: A list, NumPy array, Pandas series, or Pandas index denoting the label of each pie.
         :param c: A hex code or string specifying pie colour.
+        :param radius: Size of chart with respect plot area in % e.g  50%. Default is 80%
+        :param startAngle: render all the data points or segments in semi-pie, quarter-pie, or in any sector using the startAngle and endAngle properties.
+        :param endAngle: render all the data points or segments in semi-pie, quarter-pie, or in any sector using the startAngle and endAngle properties.
+        :param groupTo: The small segments in the pie chart can be grouped into others category using the groupTo. Specify max number of slice, all remaining slice will get rendeed under Others. 
         :param animationDelay: wait before starting animation. applicable if animationType == parallel
         :param animationDuration: total time to animate entire series
         :param animationType: parallel or sequential, dapapoints will get printed accordingly.
         :return:
         """
-        self._construct_circular_chart(x, label, c, 'pie',animationDelay,animationDuration,animationType)
+        self._construct_circular_chart(x, label, c, 'pie', radius, startAngle, endAngle, groupTo, animationDelay,animationDuration,animationType)
 
     def _construct_circular_chart(self, x: Union[list, np.ndarray, pd.Series],
                                   label: Union[list, np.ndarray, pd.Series, pd.Index],
-                                  c: Union[list,str] = None, kind: str = 'pie',animationDelay: Optional[float] = None, 
-                                  animationDuration: Optional[float] = None, animationType: Optional[str]='parallel'):
+                                  c: Union[list,str] = None, kind: str = 'pie', radius: Optional[str] = None, startAngle: Optional[int] = None, endAngle: Optional[int] = None, groupTo: Optional[int] = None,
+                                  animationDelay: Optional[float] = None, animationDuration: Optional[float] = None, animationType: Optional[str]='parallel'):
         self.check_not_datetime(x[0])
         self.check_input_data_validity(x, label)
         if animationType == 'sequential':
             current_fig_type: str = 'circularRace'
         else:   
             current_fig_type: str = 'circular'
         if self.check_multi_axes_consistency(current_fig_type):
@@ -1140,47 +1145,61 @@
             }
 
             if animationDelay is not None:
                 pie_info['animationDelay'] = animationDelay
 
             if animationDuration is not None:
                 pie_info['animationDuration'] = animationDuration
+            if radius is not None:
+                pie_info['radius'] = radius
+            if startAngle is not None:
+                pie_info['startAngle'] = startAngle
+            if endAngle is not None:
+                pie_info['endAngle'] = endAngle
+            if groupTo is not None:
+                pie_info['groupTo'] = groupTo
 
             self.data.insert(pie_info)
 
             i += 1
     def doughnut(self, x: Union[list, np.ndarray, pd.Series], label: Union[list, np.ndarray, pd.Series, pd.Index],
-                 c: Union[list,str] = None,animationDelay: Optional[float] = None, animationDuration: Optional[float] = None, animationType: Optional[str]='parallel'):
+                 c: Union[list,str] = None, radius: Optional[str] = None, startAngle: Optional[int] = None, endAngle: Optional[int] = None, groupTo: Optional[int] = None, 
+                 animationDelay: Optional[float] = None, animationDuration: Optional[float] = None, animationType: Optional[str]='parallel'):
         """
         Constructs a doughnut chart.
 
         :param x: A list, NumPy array, or Pandas series denoting the size of each doughnut piece.
         :param label: A list, NumPy array, Pandas series, or Pandas index denoting the label of each doughnut piece.
         :param c: A hex code or string specifying each doughnut colour.
+        :param radius: Size of chart with respect plot area in % e.g  50%. Default is 80%
+        :param startAngle: render all the data points or segments in semi-pie, quarter-pie, or in any sector using the startAngle and endAngle properties.
+        :param endAngle: render all the data points or segments in semi-pie, quarter-pie, or in any sector using the startAngle and endAngle properties.
+        :param groupTo: The small segments in the pie chart can be grouped into others category using the groupTo. Specify max number of slice, all remaining slice will get rendeed under Others. 
         :param animationDelay: wait before starting animation. applicable if animationType == parallel
         :param animationDuration: total time to animate entire series
         :param animationType: parallel or sequential, dapapoints will get printed accordingly.
         :return:
         """
-        self._construct_circular_chart(x, label, c, 'doughnut',animationDelay,animationDuration,animationType)
+        self._construct_circular_chart(x, label, c, 'doughnut', radius, startAngle, endAngle, groupTo, animationDelay,animationDuration,animationType)
 
     def radialbar(self, x: Union[list, np.ndarray, pd.Series], label: Union[list, np.ndarray, pd.Series, pd.Index],
-                  c: Union[list,str] = None,animationDelay: Optional[float] = None, animationDuration: Optional[float] = None, animationType: Optional[str]='parallel'):
+                  c: Union[list,str] = None,  radius: Optional[str] = None, animationDelay: Optional[float] = None, animationDuration: Optional[float] = None, animationType: Optional[str]='parallel'):
         """
         Constructs a radial bar chart.
 
         :param x: A list, NumPy array, or Pandas series denoting the size of each radial bar.
         :param label: A list, NumPy array, Pandas series, or Pandas index denoting the label of each radial bar.
         :param c: A hex code or string specifying radial bar colour.
         :param animationDelay: wait before starting animation. applicable if animationType == parallel
+        :param radius: Size of chart with respect plot area in % e.g  50%. Default is 80%
         :param animationDuration: total time to animate entire series
         :param animationType: parallel or sequential, dapapoints will get printed accordingly.
         :return:
         """
-        self._construct_circular_chart(x, label, c, 'radialbar',animationDelay,animationDuration,animationType)
+        self._construct_circular_chart(x, label, c, 'radialbar', radius, None, None, None, animationDelay,animationDuration,animationType)
 
     @staticmethod
     def get_pie_value_type(x: list) -> str:
         if sum(x) == 100.:
             return 'percent'
         else:
             return 'absolute'
```

### Comparing `chartart-0.0.3.dev17/src/chartart/simple_eda_template.py` & `chartart-0.0.3.dev18/src/chartart/simple_eda_template.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev17/src/chartart/test_plot.py` & `chartart-0.0.3.dev18/src/chartart/test_plot.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev17/src/chartart.egg-info/PKG-INFO` & `chartart-0.0.3.dev18/src/chartart.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev17
+Version: 0.0.3.dev18
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
@@ -69,7 +69,11 @@
 - bar type : bar,column,stackedBar,stackedColumn,stackedBar,stackedBar100,stackedColumn100  
 - scatter : bubble , if size is specified as list of float scatter chart will get ploted as bubble chart
 
 0.0.3.dev14 => 0.0.3.dev15
 - Tree Map : c (color) param is optional
 - Map : shapeDataField is new optional param (defaults to key 'Name'). primaryValueMapper and data is optional parameters now. This will be usefull for markers/bubbles where we dont need these inputs.
 - Map : added support fo sub layers. 
+
+0.0.3.dev18
+- Added startAngle, endAngle, radius, groupTo in circular chart
+- Added number format on axis
```

