# Comparing `tmp/e360_charting-1.8.2-py3-none-any.whl.zip` & `tmp/e360_charting-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 24066 bytes, number of entries: 14
--rw-r--r--  2.0 unx      398 b- defN 22-Jan-18 09:24 e360_charting/__init__.py
--rw-r--r--  2.0 unx     4770 b- defN 22-Jan-18 09:24 e360_charting/_charts.py
--rw-r--r--  2.0 unx    51754 b- defN 22-Jan-18 09:24 e360_charting/builders.py
--rw-r--r--  2.0 unx      936 b- defN 22-Jan-18 09:24 e360_charting/common.py
--rw-r--r--  2.0 unx      297 b- defN 22-Jan-18 09:24 e360_charting/helpers.py
--rw-r--r--  2.0 unx    12882 b- defN 22-Jan-18 09:24 e360_charting/models.py
--rw-r--r--  2.0 unx     4603 b- defN 22-Jan-18 09:24 e360_charting/stylers.py
--rw-r--r--  2.0 unx     6445 b- defN 22-Jan-18 09:24 e360_charting/styles.py
--rw-r--r--  2.0 unx     2988 b- defN 22-Jan-18 09:24 e360_charting/utils.py
--rw-rw-r--  2.0 unx      575 b- defN 22-Jan-18 09:26 e360_charting-1.8.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3033 b- defN 22-Jan-18 09:26 e360_charting-1.8.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-18 09:26 e360_charting-1.8.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 22-Jan-18 09:26 e360_charting-1.8.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1144 b- defN 22-Jan-18 09:26 e360_charting-1.8.2.dist-info/RECORD
-14 files, 89931 bytes uncompressed, 22168 bytes compressed:  75.3%
+Zip file size: 24198 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      398 b- defN 22-Jan-21 16:34 e360_charting/__init__.py
+-rw-r--r--  2.0 unx     4861 b- defN 22-Jan-21 16:34 e360_charting/_charts.py
+-rw-r--r--  2.0 unx    52749 b- defN 22-Jan-21 16:34 e360_charting/builders.py
+-rw-r--r--  2.0 unx      936 b- defN 22-Jan-21 16:34 e360_charting/common.py
+-rw-r--r--  2.0 unx      297 b- defN 22-Jan-21 16:34 e360_charting/helpers.py
+-rw-r--r--  2.0 unx    12882 b- defN 22-Jan-21 16:34 e360_charting/models.py
+-rw-r--r--  2.0 unx     4603 b- defN 22-Jan-21 16:34 e360_charting/stylers.py
+-rw-r--r--  2.0 unx     6445 b- defN 22-Jan-21 16:34 e360_charting/styles.py
+-rw-r--r--  2.0 unx     2988 b- defN 22-Jan-21 16:34 e360_charting/utils.py
+-rw-rw-r--  2.0 unx      575 b- defN 22-Jan-21 16:36 e360_charting-1.9.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3033 b- defN 22-Jan-21 16:36 e360_charting-1.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Jan-21 16:36 e360_charting-1.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 22-Jan-21 16:36 e360_charting-1.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1144 b- defN 22-Jan-21 16:36 e360_charting-1.9.0.dist-info/RECORD
+14 files, 91017 bytes uncompressed, 22300 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: e360_charting/styles.py
 Comment: 
 
 Filename: e360_charting/utils.py
 Comment: 
 
-Filename: e360_charting-1.8.2.dist-info/LICENSE.txt
+Filename: e360_charting-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: e360_charting-1.8.2.dist-info/METADATA
+Filename: e360_charting-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: e360_charting-1.8.2.dist-info/WHEEL
+Filename: e360_charting-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: e360_charting-1.8.2.dist-info/top_level.txt
+Filename: e360_charting-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: e360_charting-1.8.2.dist-info/RECORD
+Filename: e360_charting-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## e360_charting/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.8.2'
+__version__ = '1.9.0'
 
 try:
     # Attempts to import the client class
     # Allowed to fail importing so the package metadata can be read for building
     from ._charts import *  # noqa: F403
     from .models import AnnotationModel  # noqa: F401
     from .builders import PlotlyVisualisation  # noqa: F401
```

## e360_charting/_charts.py

```diff
@@ -80,14 +80,17 @@
     pass
 
 
 class SubplotVisualisation(builders.BaseAxesVisualisation, styles.SubplotMixin):
     pass
 
 
+class PhewasPlotVisualisation(builders.PhewasVisualisation, styles.ForestMixin):
+    pass
+
 # --- STRATIFIED CHARTS -------------------------------------------------------
 
 
 class BarStratifiedVisualisation(builders.BaseStratifiedVisualisation, styles.BarMixin):
     """Bar Stratified Chart for VRS"""
     pass
```

## e360_charting/builders.py

```diff
@@ -384,29 +384,15 @@
             data_item.yaxis = "y" + trace_idx
         self.chart.data.append(data_item)
 
     def setup_chart(self, style_class=None):
         style_class = style_class or self
         self._validate_input()
         self.chart = ChartModel(**style_class.chart_dict(), id=f'chart{len(self.report.charts) + 1}')
-
-        common_attr = self.trace_names, self.colors, self.hovertext
-        if self.horizontal and not self.vertical:
-            self.layout.set_data_points(len(self.x_values))
-            for x, trace_name, color, hovertext in zip(self.x_values, *common_attr):
-                self._setup_chart_data(style_class, color, x=x, name=trace_name, hovertext=hovertext)
-        elif self.vertical and not self.horizontal:
-            self.layout.set_data_points(len(self.y_values), horizontal=False)
-            for y, trace_name, color, hovertext in zip(self.y_values, *common_attr):
-                self._setup_chart_data(style_class, color, y=y, name=trace_name, hovertext=hovertext)
-        else:
-            self.layout.set_data_points(len(self.x_values))
-            for x, y, trace_name, color, hovertext in zip(self.x_values, self.y_values, *common_attr):
-                self._setup_chart_data(style_class, color, x=x, y=y, name=trace_name, hovertext=hovertext)
-
+        self.setup_typed_chart(style_class)
         self.report.charts.append(self.chart)
 
     def setup_extra_charts(self):
         for StyleClass in self.extra_charts:
             self.setup_chart(style_class=StyleClass)
 
     def _setup_subplots(self):
@@ -438,14 +424,29 @@
                 if len(z[y_idx]) != len(x):
                     raise ValueError('Number of z_values columns needs to match x_value number of elements')
                 annot = AnnotationModel(x=x_val, y=y_val, text=str(z[y_idx][x_idx]),
                  xref='x1', yref='y1', font={'color': annot_color})
                 annots.append(annot)
         return annots
 
+    def setup_typed_chart(self, style_class):
+        common_attr = self.trace_names, self.colors, self.hovertext
+        if self.horizontal and not self.vertical:
+            self.layout.set_data_points(len(self.x_values))
+            for x, trace_name, color, hovertext in zip(self.x_values, *common_attr):
+                self._setup_chart_data(style_class, color, x=x, name=trace_name, hovertext=hovertext)
+        elif self.vertical and not self.horizontal:
+            self.layout.set_data_points(len(self.y_values), horizontal=False)
+            for y, trace_name, color, hovertext in zip(self.y_values, *common_attr):
+                self._setup_chart_data(style_class, color, y=y, name=trace_name, hovertext=hovertext)
+        else:
+            self.layout.set_data_points(len(self.x_values))
+            for x, y, trace_name, color, hovertext in zip(self.x_values, self.y_values, *common_attr):
+                self._setup_chart_data(style_class, color, x=x, y=y, name=trace_name, hovertext=hovertext)
+
 
 @dataclass
 class BaseAxesArrayVisualisation(BaseAxesVisualisation):
 
     array_x: Optional[List[List[Any]]] = field(default_factory=list)
     arrayminus_x: Optional[List[List[Any]]] = field(default_factory=list)
     array_y: Optional[List[List[Any]]] = field(default_factory=list)
@@ -461,28 +462,44 @@
 
         if not self.array_y:
             self.array_y = [[] for _ in range(len(self.y_values))]
 
         if not self.arrayminus_y:
             self.arrayminus_y = [[] for _ in range(len(self.y_values))]
 
-    def setup_chart(self, style_class=None):
-        style_class = style_class or self
-        self._validate_input()
-        self.chart = ChartModel(**style_class.chart_dict(), id=f'chart{len(self.report.charts) + 1}')
+    def setup_typed_chart(self, style_class):
         self.layout.set_data_points(len(self.x_values))
-
         for x, array_x, arrayminus_x, y, array_y, arrayminus_y, trace_name, color, hovertext in zip(self.x_values, self.array_x, self.arrayminus_x, self.y_values, self.array_y, self.arrayminus_y, self.trace_names, self.colors, self.hovertext):
             marker = MarkerModel(**style_class.marker_dict(), color=color)
-            error_x_model = ErrorAxisModel(array=array_x, arrayminus=arrayminus_x)
-            error_y_model = ErrorAxisModel(array=array_y, arrayminus=arrayminus_y)
-            data_item = ChartDataModel(**style_class.chartdata_dict(), x=x, error_x=error_x_model, y=y, error_y=error_y_model, name=trace_name, marker=marker, hovertext=hovertext)
+            data_item = self.setup_data_item(style_class, marker, x, array_x, arrayminus_x, y, array_y, arrayminus_y, trace_name, color, hovertext)
             self.chart.data.append(data_item)
 
-        self.report.charts.append(self.chart)
+    def setup_data_item(self, style_class, marker, x, array_x, arrayminus_x, y, array_y, arrayminus_y, trace_name, color, hovertext):
+        error_x_model = ErrorAxisModel(array=array_x, arrayminus=arrayminus_x)
+        error_y_model = ErrorAxisModel(array=array_y, arrayminus=arrayminus_y)
+        return ChartDataModel(**style_class.chartdata_dict(), x=x, error_x=error_x_model, y=y, error_y=error_y_model, name=trace_name, marker=marker, hovertext=hovertext)
+
+
+@dataclass
+class PhewasVisualisation(BaseAxesArrayVisualisation):
+
+    def __post_init__(self):
+        super().__post_init__()
+        self.is_subplot = True
+        self.subplot_dimensions = [2, 2]
+
+    def setup_data_item(self, style_class, marker, x, array_x, arrayminus_x, y, array_y, arrayminus_y, trace_name, color, hovertext):
+        if self.trace_names.index(trace_name) == 1:
+            data_item = ChartDataModel(**style_class.chartdata_dict(), x=x, y=y, name=trace_name, marker=marker, hovertext=hovertext)
+            trace_idx = str(self.colors.index(color) + 1)
+            data_item.xaxis = "x" + trace_idx
+            data_item.yaxis = "y" + trace_idx
+            return data_item
+        else:
+            return super().setup_data_item(style_class, marker, x, array_x, arrayminus_x, y, array_y, arrayminus_y, trace_name, color, hovertext)
 
 
 @dataclass
 class BaseMeasureVisualisation(BaseBuilder, BaseVisualisation):
     """
     Base for waterfall charts.
```

## Comparing `e360_charting-1.8.2.dist-info/LICENSE.txt` & `e360_charting-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `e360_charting-1.8.2.dist-info/METADATA` & `e360_charting-1.9.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e360-charting
-Version: 1.8.2
+Version: 1.9.0
 Summary: Create charts for E360 Plotly Visualisations.
 Home-page: UNKNOWN
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `e360_charting-1.8.2.dist-info/RECORD` & `e360_charting-1.9.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-e360_charting/__init__.py,sha256=VWVlHj4qrsAj9YbsITbXkoFA266hWN6kOdXwRQnnV3s,398
-e360_charting/_charts.py,sha256=ETFxRFGtBXsvxQQuaxkY33Q7i2rJrB9b5DMzpDf9XyA,4770
-e360_charting/builders.py,sha256=fYt4YwqNbXpGi9yhi63m6X6C3Z6AT3K9djTRCJTuf5g,51754
+e360_charting/__init__.py,sha256=7mv1GMwLQEokb1A0wnX8KJtPTeuo959uSuSrf_n5nlI,398
+e360_charting/_charts.py,sha256=LUBtScDqOVCZgjtidhS1-VEdQizdLPpdvE6_x8ffiPM,4861
+e360_charting/builders.py,sha256=VraE8Ud1-GoQl4EgDCdA45md55WhQM-Ni7OVVo-mOV4,52749
 e360_charting/common.py,sha256=FOKnqSwjixQ3k1eTgRjM3GsS8c8gTIC-91i-DYBr8oQ,936
 e360_charting/helpers.py,sha256=VmubqRoSWdeZa_1oaa8_8v1QdcIubd1LvesXggYLENY,297
 e360_charting/models.py,sha256=ZXanQg8-nMdK3RFt4A3yvRqmkgVobXMi-XyOxxV28wc,12882
 e360_charting/stylers.py,sha256=0ziwXglqgcc2nIT3cy__tzKxZn9zsAjWhwPIn83bmO0,4603
 e360_charting/styles.py,sha256=QmRiWkVRbb-nKf0DF12YQLGGX3xIyHd8HmYSBeH9218,6445
 e360_charting/utils.py,sha256=DWnBq6oZvNfzJaV7fYf8zRTlwdBVLMhZpzDmDiO8S5E,2988
-e360_charting-1.8.2.dist-info/LICENSE.txt,sha256=TpqXYcSsLjtOgJqhfMJFO9rHZudUyck-GdOuUvqcggc,575
-e360_charting-1.8.2.dist-info/METADATA,sha256=hhXWWHejqUFZRarYdARNPe8UqpUTzbWO-skpOOHBYnM,3033
-e360_charting-1.8.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-e360_charting-1.8.2.dist-info/top_level.txt,sha256=leF6vutzZgX852QeQVeZDhdXmaz_N2bLupbQWWqX8g8,14
-e360_charting-1.8.2.dist-info/RECORD,,
+e360_charting-1.9.0.dist-info/LICENSE.txt,sha256=TpqXYcSsLjtOgJqhfMJFO9rHZudUyck-GdOuUvqcggc,575
+e360_charting-1.9.0.dist-info/METADATA,sha256=Y_zwMD_Ppv7NJ5cJcxJq4dYnCk6gZ3xZVvAaNTQRkNs,3033
+e360_charting-1.9.0.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+e360_charting-1.9.0.dist-info/top_level.txt,sha256=leF6vutzZgX852QeQVeZDhdXmaz_N2bLupbQWWqX8g8,14
+e360_charting-1.9.0.dist-info/RECORD,,
```

