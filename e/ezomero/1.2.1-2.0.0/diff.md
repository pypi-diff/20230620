# Comparing `tmp/ezomero-1.2.1.tar.gz` & `tmp/ezomero-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezomero-1.2.1.tar", last modified: Wed Dec 21 18:25:18 2022, max compression
+gzip compressed data, was "ezomero-2.0.0.tar", last modified: Tue Jun 20 13:45:43 2023, max compression
```

## Comparing `ezomero-1.2.1.tar` & `ezomero-2.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 18:25:18.385828 ezomero-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-21 18:25:10.000000 ezomero-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2022-12-21 18:25:18.385828 ezomero-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2022-12-21 18:25:10.000000 ezomero-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 18:25:18.385828 ezomero-1.2.1/ezomero/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2022-12-21 18:25:10.000000 ezomero-1.2.1/ezomero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2022-12-21 18:25:10.000000 ezomero-1.2.1/ezomero/_ezomero.py
--rw-r--r--   0 runner    (1001) docker     (123)    45558 2022-12-21 18:25:10.000000 ezomero-1.2.1/ezomero/_gets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18719 2022-12-21 18:25:10.000000 ezomero-1.2.1/ezomero/_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2022-12-21 18:25:10.000000 ezomero-1.2.1/ezomero/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27857 2022-12-21 18:25:10.000000 ezomero-1.2.1/ezomero/_posts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2022-12-21 18:25:10.000000 ezomero-1.2.1/ezomero/json_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2022-12-21 18:25:10.000000 ezomero-1.2.1/ezomero/rois.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 18:25:18.385828 ezomero-1.2.1/ezomero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2022-12-21 18:25:18.000000 ezomero-1.2.1/ezomero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2022-12-21 18:25:18.000000 ezomero-1.2.1/ezomero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 18:25:18.000000 ezomero-1.2.1/ezomero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-21 18:25:18.000000 ezomero-1.2.1/ezomero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-21 18:25:18.000000 ezomero-1.2.1/ezomero.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 18:25:18.385828 ezomero-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2022-12-21 18:25:10.000000 ezomero-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 18:25:18.385828 ezomero-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 18:25:10.000000 ezomero-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21075 2022-12-21 18:25:10.000000 ezomero-1.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2022-12-21 18:25:10.000000 ezomero-1.2.1/tests/test_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2022-12-21 18:25:10.000000 ezomero-1.2.1/tests/test_ezimport.py
--rw-r--r--   0 runner    (1001) docker     (123)    20938 2022-12-21 18:25:10.000000 ezomero-1.2.1/tests/test_gets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2022-12-21 18:25:10.000000 ezomero-1.2.1/tests/test_json_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2022-12-21 18:25:10.000000 ezomero-1.2.1/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    22248 2022-12-21 18:25:10.000000 ezomero-1.2.1/tests/test_posts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2022-12-21 18:25:10.000000 ezomero-1.2.1/tests/test_puts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2022-12-21 18:25:10.000000 ezomero-1.2.1/tests/test_rois.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2022-12-21 18:25:10.000000 ezomero-1.2.1/tests/test_users_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:45:43.080070 ezomero-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-06-20 13:45:31.000000 ezomero-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-20 13:45:43.080070 ezomero-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-20 13:45:31.000000 ezomero-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:45:43.076070 ezomero-2.0.0/ezomero/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-20 13:45:31.000000 ezomero-2.0.0/ezomero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-06-20 13:45:31.000000 ezomero-2.0.0/ezomero/_ezomero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46168 2023-06-20 13:45:31.000000 ezomero-2.0.0/ezomero/_gets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-06-20 13:45:31.000000 ezomero-2.0.0/ezomero/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-06-20 13:45:31.000000 ezomero-2.0.0/ezomero/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26626 2023-06-20 13:45:31.000000 ezomero-2.0.0/ezomero/_posts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-06-20 13:45:31.000000 ezomero-2.0.0/ezomero/json_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-06-20 13:45:31.000000 ezomero-2.0.0/ezomero/rois.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:45:43.076070 ezomero-2.0.0/ezomero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-20 13:45:42.000000 ezomero-2.0.0/ezomero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-20 13:45:43.000000 ezomero-2.0.0/ezomero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:45:42.000000 ezomero-2.0.0/ezomero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-20 13:45:42.000000 ezomero-2.0.0/ezomero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 13:45:42.000000 ezomero-2.0.0/ezomero.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:45:43.080070 ezomero-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-20 13:45:31.000000 ezomero-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:45:43.080070 ezomero-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:45:31.000000 ezomero-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-06-20 13:45:31.000000 ezomero-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-20 13:45:31.000000 ezomero-2.0.0/tests/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-20 13:45:31.000000 ezomero-2.0.0/tests/test_ezimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-06-20 13:45:31.000000 ezomero-2.0.0/tests/test_gets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-20 13:45:31.000000 ezomero-2.0.0/tests/test_json_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-20 13:45:31.000000 ezomero-2.0.0/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19138 2023-06-20 13:45:31.000000 ezomero-2.0.0/tests/test_posts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-20 13:45:31.000000 ezomero-2.0.0/tests/test_puts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-20 13:45:31.000000 ezomero-2.0.0/tests/test_rois.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-20 13:45:31.000000 ezomero-2.0.0/tests/test_users_group.py
```

### Comparing `ezomero-1.2.1/PKG-INFO` & `ezomero-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezomero
-Version: 1.2.1
+Version: 2.0.0
 Summary: A suite of convenience functions for working with OMERO. Written and maintained by the Research IT team at The Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/ezomero
 Maintainer: Dave Mellert
 Maintainer-email: Dave.Mellert@jax.org
 License: UNKNOWN
 Description: ![Run Tests](https://github.com/TheJacksonLaboratory/ezomero/workflows/Run%20Tests/badge.svg?event=push) ![](https://raw.githubusercontent.com/TheJacksonLaboratory/ezomero/main/coverage.svg)
```

### Comparing `ezomero-1.2.1/README.md` & `ezomero-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ezomero-1.2.1/ezomero/__init__.py` & `ezomero-2.0.0/ezomero/__init__.py`

 * *Files identical despite different names*

### Comparing `ezomero-1.2.1/ezomero/_ezomero.py` & `ezomero-2.0.0/ezomero/_ezomero.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,35 +254,43 @@
         if config_dict:
             host = config_dict.get("OMERO_HOST", host)
         host = os.environ.get("OMERO_HOST", host)
     if host is None:
         host = input('Enter host: ')
 
     # set port
+    port_str = None
     if port is None:
         if config_dict:
-            port = config_dict.getint("OMERO_PORT", port)
-        port = int(os.environ.get("OMERO_PORT", str(port)))
+            port_str = config_dict.get("OMERO_PORT", str(port))
+        port_str = os.environ.get("OMERO_PORT", port_str)
+        if port_str:
+            port = int(port_str)
     if port is None:
         port = int(input('Enter port: '))
 
     # set session security
+    secure_str = None
     if secure is None:
         if config_dict:
-            secure = config_dict.getboolean("OMERO_SECURE", secure)
-        secure = bool(os.environ.get("OMERO_SECURE", str(secure)))
+            secure_str = config_dict.get("OMERO_SECURE", str(secure))
+    secure_str = os.environ.get("OMERO_SECURE", secure_str)
+    if secure_str:
+        if secure_str.lower() in ["true", "t"]:
+            secure = True
+        elif secure_str.lower() in ["false", "f"]:
+            secure = False
     if secure is None:
         str_secure: str = input('Secure session (True or False): ')
         if str_secure.lower() in ["true", "t"]:
             secure = True
         elif str_secure.lower() in ["false", "f"]:
             secure = False
         else:
             raise ValueError('secure must be set to either True or False')
-
     # create connection
     conn = BlitzGateway(user, password, group=group, host=host, port=port,
                         secure=secure)
     if conn.connect():
         return conn
     else:
         logging.error('Could not connect, check your settings')
```

### Comparing `ezomero-1.2.1/ezomero/_gets.py` & `ezomero-2.0.0/ezomero/_gets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import logging
 import os
 import numpy as np
 from typing import Optional, List, Union, Tuple, Literal
+from typing import Any
 from ._ezomero import do_across_groups
 from omero.gateway import FileAnnotationWrapper, BlitzGateway, ImageWrapper
 from omero import ApiUsageException, InternalException
 from omero.model import MapAnnotationI, TagAnnotationI, Shape
 from omero.grid import Table
 from omero.rtypes import rint, rlong
 from omero.sys import Parameters
 from omero.model import enums as omero_enums
 from .rois import Point, Line, Rectangle
 from .rois import Ellipse, Polygon, Polyline, Label, ezShape
 import importlib.util
-# try importing pandas
+
 if (importlib.util.find_spec('pandas')):
     import pandas as pd
     has_pandas = True
 else:
     has_pandas = False
 
 
@@ -473,15 +474,15 @@
     Returns
     -------
     proj_ids : list of ints
         List of project IDs accessible by current user.
 
     Examples
     --------
-   # Return IDs of all projects accessible by current user:
+    # Return IDs of all projects accessible by current user:
 
     >>> proj_ids = get_project_ids(conn)
     """
     proj_ids = []
     for p in conn.listProjects():
         proj_ids.append(p.getId())
     return proj_ids
@@ -1110,24 +1111,18 @@
     pix.setPixelsId(pid, False)
     levels: List[Tuple[int, ...]]
     levels = [(r.sizeX, r.sizeY) for r in pix.getResolutionDescriptions()]
     pix.close()
     return levels
 
 
-if has_pandas:
-    TableType = pd.core.frame.DataFrame
-else:
-    TableType = List
-
-
 @do_across_groups
 def get_table(conn: BlitzGateway, file_ann_id: int,
               across_groups: Optional[bool] = True
-              ) -> TableType:
+              ) -> Any:
     """Get a table from its FileAnnotation object.
 
     Parameters
     ----------
     conn : ``omero.gateway.BlitzGateway`` object
         OMERO connection.
     file_ann_id : int
@@ -1165,15 +1160,15 @@
         logging.warning(f' FileAnnotation {file_ann_id} does not exist.')
     return table
 
 
 @do_across_groups
 def get_shape(conn: BlitzGateway, shape_id: int,
               across_groups: Optional[bool] = True
-              ) -> Tuple[ezShape, Tuple, Tuple, float]:
+              ) -> ezShape:
     """Get an ezomero shape object from an OMERO Shape id
 
     Parameters
     ----------
     conn : ``omero.gateway.BlitzGateway`` object
         OMERO connection.
     shape_id : int
@@ -1182,33 +1177,36 @@
         Defines cross-group behavior of function - set to
         ``False`` to disable it.
 
     Returns
     -------
     shape : obj
         An object of one of ezomero shape classes
-    fill_color: tuple
-        Tuple of format (r, g, b, a) containing the shape fill color.
-    stroke_color: tuple
-        Tuple of format (r, g, b, a) containing the shape stroke color.
-    stroke_width: float
-        Shape stroke width, in pixels
+
+    Notes
+    -------
+    ``fill_color`` for the Shape defaults to (0, 0, 0, 0) in case the original
+    Shape doesn't have one.
+    ``stroke_color`` for the Shape defaults to (255, 255, 0, 255) in case the
+    original Shape doesn't have one.
+    ``stroke_width`` for the Shape defaults to 1 in case the original Shape
+    doesn't have one.
     Examples
     --------
     >>> shape = get_shape(conn, 634443)
 
     """
     if not isinstance(shape_id, int):
         raise TypeError('Shape ID must be an integer')
     omero_shape = conn.getObject('Shape', shape_id)
     return _omero_shape_to_shape(omero_shape)
 
 
 def _create_table(table_obj: Table
-                  ) -> TableType:
+                  ) -> Any:
     if importlib.util.find_spec('pandas'):
         columns = []
         for col in table_obj.getHeaders():
             columns.append(col.name)
         table = pd.DataFrame(columns=columns)
         rowCount = table_obj.getNumberOfRows()
         data = table_obj.read(list(range(len(columns))), 0, rowCount)
@@ -1237,17 +1235,23 @@
         for row in data_lists:
             table.append(row)
 
     return table
 
 
 def _omero_shape_to_shape(omero_shape: Shape
-                          ) -> Tuple[ezShape, Tuple, Tuple, float]:
+                          ) -> ezShape:
     """ Helper function to convert ezomero shapes into omero shapes"""
     shape_type = omero_shape.ice_id().split("::omero::model::")[1]
+    fill_color = _int_to_rgba(omero_shape.getFillColor(), True)
+    stroke_color = _int_to_rgba(omero_shape.getStrokeColor(), False)
+    try:
+        stroke_width = omero_shape.getStrokeWidth().getValue()
+    except AttributeError:
+        stroke_width = 1
     try:
         z_val = omero_shape.theZ
     except AttributeError:
         z_val = None
     try:
         c_val = omero_shape.theC
     except AttributeError:
@@ -1268,66 +1272,74 @@
         mk_end = omero_shape.markerEnd
     except AttributeError:
         mk_end = None
     shape: Union[Point, Line, Rectangle, Ellipse, Polygon, Polyline, Label]
     if shape_type == "Point":
         x = omero_shape.x
         y = omero_shape.y
-        shape = Point(x, y, z_val, c_val, t_val, text)
+        shape = Point(x, y, z_val, c_val, t_val, text, fill_color,
+                      stroke_color, stroke_width)
     elif shape_type == "Line":
         x1 = omero_shape.x1
         x2 = omero_shape.x2
         y1 = omero_shape.y1
         y2 = omero_shape.y2
-        shape = Line(x1, y1, x2, y2, z_val, c_val, t_val,
-                     mk_start, mk_end, text)
+        shape = Line(x1, y1, x2, y2, z_val, c_val, t_val, mk_start, mk_end,
+                     text, fill_color, stroke_color, stroke_width)
     elif shape_type == "Rectangle":
         x = omero_shape.x
         y = omero_shape.y
         width = omero_shape.width
         height = omero_shape.height
-        shape = Rectangle(x, y, width, height, z_val, c_val, t_val, text)
+        shape = Rectangle(x, y, width, height, z_val, c_val, t_val, text,
+                          fill_color, stroke_color, stroke_width)
     elif shape_type == "Ellipse":
         x = omero_shape.x
         y = omero_shape.y
         radiusX = omero_shape.radiusX
         radiusY = omero_shape.radiusY
-        shape = Ellipse(x, y, radiusX, radiusY, z_val, c_val, t_val, text)
+        shape = Ellipse(x, y, radiusX, radiusY, z_val, c_val, t_val, text,
+                        fill_color, stroke_color, stroke_width)
     elif shape_type == "Polygon":
         omero_points = omero_shape.points.split()
         points = []
         for point in omero_points:
             coords = point.split(',')
             points.append((float(coords[0]), float(coords[1])))
-        shape = Polygon(points, z_val, c_val, t_val, text)
+        shape = Polygon(points, z_val, c_val, t_val, text, fill_color,
+                        stroke_color, stroke_width)
     elif shape_type == "Polyline":
         omero_points = omero_shape.points.split()
         points = []
         for point in omero_points:
             coords = point.split(',')
             points.append((float(coords[0]), float(coords[1])))
-        shape = Polyline(points, z_val, c_val, t_val, text)
+        shape = Polyline(points, z_val, c_val, t_val, text, fill_color,
+                         stroke_color, stroke_width)
     elif shape_type == "Label":
         x = omero_shape.x
         y = omero_shape.y
         fsize = omero_shape.getFontSize().getValue()
-        shape = Label(x, y, text, fsize, z_val, c_val, t_val)
+        shape = Label(x, y, text, fsize, z_val, c_val, t_val, fill_color,
+                      stroke_color, stroke_width)
     else:
         err = 'The shape passed for the roi is not a valid shape type'
         raise TypeError(err)
+    return shape
 
-    fill_color = _int_to_rgba(omero_shape.getFillColor())
-    stroke_color = _int_to_rgba(omero_shape.getStrokeColor())
-    stroke_width = omero_shape.getStrokeWidth().getValue()
-
-    return shape, fill_color, stroke_color, stroke_width
 
-
-def _int_to_rgba(omero_val: int) -> Tuple[int, ...]:
+def _int_to_rgba(omero_val: Union[int, None], is_fill: bool) -> \
+        Tuple[int, int, int, int]:
     """ Helper function returning the color as an Integer in RGBA encoding """
-    if omero_val < 0:
-        omero_val = omero_val + (2**32)
-    r = omero_val >> 24
-    g = omero_val - (r << 24) >> 16
-    b = omero_val - (r << 24) - (g << 16) >> 8
-    a = omero_val - (r << 24) - (g << 16) - (b << 8)
-    return (r, g, b, a)
+    if omero_val:
+        if omero_val < 0:
+            omero_val = omero_val + (2**32)
+        r = omero_val >> 24
+        g = omero_val - (r << 24) >> 16
+        b = omero_val - (r << 24) - (g << 16) >> 8
+        a = omero_val - (r << 24) - (g << 16) - (b << 8)
+        return (r, g, b, a)
+    else:
+        if is_fill:
+            return (0, 0, 0, 0)
+        else:
+            return (255, 255, 0, 255)
```

### Comparing `ezomero-1.2.1/ezomero/_importer.py` & `ezomero-2.0.0/ezomero/_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,29 +44,31 @@
 
     Returns
     -------
     plate_ids or image_ids : list of ints
         The ids of the Images/Plates that were generated by importing the
         specified target.
 
-    NOTE: this function is EXPERIMENTAL and has seen minimal testing. Use at
+    Notes
+    -------
+    This function is EXPERIMENTAL and has seen minimal testing. Use at
     your own risk! We do not recommend using this in production.
     """
 
     imp_ctl = Importer(conn, target, project, dataset, screen,
                        ln_s, ann, ns)
     imp_ctl.ezimport()
     if imp_ctl.screen:
         imp_ctl.get_plate_ids()
         imp_ctl.organize_plates()
         imp_ctl.annotate_plates()
         return imp_ctl.plate_ids
 
     else:
-        imp_ctl.get_image_ids()
+        imp_ctl.get_my_image_ids()
         imp_ctl.organize_images()
         imp_ctl.annotate_images()
         return imp_ctl.image_ids
 
 
 def set_or_create_project(conn: BlitzGateway, project: Union[str, int],
                           across_groups: Optional[bool] = True) -> int:
@@ -275,15 +277,15 @@
         self.imported = False
         self.image_ids: Union[List[int], None] = None
         self.plate_ids: Union[List[int], None] = None
         self.ln_s = ln_s
         self.ann = ann
         self.ns = ns
 
-    def get_image_ids(self) -> Union[List[int], None]:
+    def get_my_image_ids(self) -> Union[List[int], None]:
         """Get the Ids of imported images.
 
         Note that this will not find images if they have not been imported.
         Also, while image_ids are returned, this method also sets
         ``self.image_ids``.
         Returns
         -------
```

### Comparing `ezomero-1.2.1/ezomero/_misc.py` & `ezomero-2.0.0/ezomero/_misc.py`

 * *Files identical despite different names*

### Comparing `ezomero-1.2.1/ezomero/_posts.py` & `ezomero-2.0.0/ezomero/_posts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import mimetypes
-from typing import Optional, List, Union, Tuple
+from typing import Optional, List, Union, Tuple, Any
 import numpy as np
 from uuid import uuid4
 from ._ezomero import do_across_groups, set_group
 from ._misc import link_datasets_to_project
 from omero.gateway import BlitzGateway
 from omero.model import RoiI, PointI, LineI, RectangleI, EllipseI
 from omero.model import PolygonI, PolylineI, LabelI, LengthI, enums
@@ -12,17 +12,17 @@
 from omero.grid import BoolColumn, LongColumn
 from omero.grid import StringColumn, DoubleColumn, Column
 from omero.gateway import ProjectWrapper, DatasetWrapper
 from omero.gateway import ScreenWrapper, FileAnnotationWrapper
 from omero.gateway import MapAnnotationWrapper, OriginalFileWrapper
 from omero.rtypes import rstring, rint, rdouble
 from .rois import Point, Line, Rectangle, Ellipse
-from .rois import Polygon, Polyline, Label, ezShape
+from .rois import Polygon, Polyline, Label
 import importlib.util
-# try importing pandas
+
 if (importlib.util.find_spec('pandas')):
     import pandas as pd
     has_pandas = True
 else:
     has_pandas = False
 
 
@@ -459,45 +459,30 @@
     screen.save()
     return screen.getId()
 
 
 def post_roi(conn: BlitzGateway, image_id: int,
              shapes: List[Union[Point, Line, Rectangle, Ellipse,
                                 Polygon, Polyline, Label]],
-             name: Optional[str] = None, description: Optional[str] = None,
-             fill_color: Optional[Union[Tuple[int, int, int, int], int]] =
-             (10, 10, 10, 10),
-             stroke_color: Optional[Union[Tuple[int, int, int, int], int]] =
-             (255, 255, 255, 255),
-             stroke_width: Optional[int] = 1) -> int:
+             name: Optional[str] = None, description: Optional[str] = None)\
+                -> int:
     """Create new ROI from a list of shapes and link to an image.
 
     Parameters
     ----------
     conn : ``omero.gateway.BlitzGateway`` object
         OMERO connection.
     image_id : int
         IDs of the image to which the new ROI will be linked.
     shapes : list of shapes
         List of shape objects associated with the new ROI.
     name : str, optional
         Name for the new ROI.
     description : str, optional
         Description of the new ROI.
-    fill_color: tuple of int, optional
-        The color fill of the shape. Color is specified as a a tuple containing
-        4 integers from 0 to 255, representing red, green, blue and alpha
-        levels. Default is (10, 10, 10, 10).
-    stroke_color: tuple of int, optional
-        The color of the shape edge. Color is specified as a a tuple containing
-        4 integers from 0 to 255, representing red, green, blue and alpha
-        levels. Default is (255, 255, 255, 255).
-    stroke_width: int, optional
-        The width of the shape stroke in pixels. Default is 1.
-
 
     Returns
     -------
     ROI_id : int
         ID of newly created ROI
 
     Examples
@@ -506,64 +491,44 @@
     >>> point = Point(x=30.6, y=80.4)
     >>> shapes.append(point)
     >>> rectangle = Rectangle(x=50.0,
                               y=51.3,
                               width=90,
                               height=40,
                               z=3,
-                              label='The place')
+                              label='The place',
+                              fill_color=(255, 10, 10, 150),
+                              stroke_color=(255, 0, 0, 0),
+                              stroke_width=2)
     >>> shapes.append(rectangle)
     >>> post_roi(conn, 23, shapes, name='My Cell',
-                 description='Very important',
-                 fill_color=(255, 10, 10, 150),
-                 stroke_color=(255, 0, 0, 0),
-                 stroke_width=2)
+                 description='Very important')
     234
     """
 
     if type(image_id) is not int:
         raise TypeError('Image ID must be an integer')
 
     if not isinstance(shapes, list):
         raise TypeError('Shapes must be a list')
 
-    if not isinstance(fill_color, tuple):
-        raise TypeError('Fill color must be a tuple')
-    if len(fill_color) != 4:
-        raise ValueError('Fill color must contain 4 integers')
-
-    if not isinstance(stroke_color, tuple):
-        raise TypeError('Stroke color must be a tuple')
-    if len(stroke_color) != 4:
-        raise ValueError('Stroke color must contain 4 integers')
-
-    if type(stroke_width) is not int:
-        raise TypeError('Stroke width must be an integer')
-
     roi = RoiI()
     if name is not None:
         roi.setName(rstring(name))
     if description is not None:
         roi.setDescription(rstring(description))
     for shape in shapes:
-        roi.addShape(_shape_to_omero_shape(shape, fill_color, stroke_color,
-                                           stroke_width))
+        roi.addShape(_shape_to_omero_shape(shape))
     image = conn.getObject('Image', image_id)
     roi.setImage(image._obj)
     roi = conn.getUpdateService().saveAndReturnObject(roi)
     return roi.getId().getValue()
 
 
-if has_pandas:
-    TableType = pd.core.frame.DataFrame
-else:
-    TableType = List
-
-
-def post_table(conn: BlitzGateway, table: TableType,
+def post_table(conn: BlitzGateway, table: Any,
                object_type: str, object_id: int,
                title: Optional[str] = "",
                headers: bool = True) -> Union[int, None]:
     """Create new table and link it to an OMERO object.
 
     Parameters
     ----------
@@ -639,15 +604,15 @@
     file_obj = OriginalFileWrapper(conn, orig_file)
     file_obj.save()
     file_ann.setFile(file_obj)
     file_ann = obj.linkAnnotation(file_ann)
     return file_ann.id
 
 
-def create_columns(table: TableType,
+def create_columns(table: Any,
                    headers: bool) -> List[Column]:
     """Helper function to create the correct column types from a table"""
     cols = []
     if type(table) == list:
         if headers:
             titles = table[0]
             data = table[1:]
@@ -689,18 +654,15 @@
     else:
         raise TypeError("Table must be a list of row lists or "
                         "pandas Dataframe")
     return cols
 
 
 def _shape_to_omero_shape(shape: Union[Point, Line, Rectangle, Ellipse,
-                                       Polygon, Polyline, Label],
-                          fill_color: Tuple[int, int, int, int],
-                          stroke_color: Tuple[int, int, int, int],
-                          stroke_width: int) -> Shape:
+                                       Polygon, Polyline, Label]) -> Shape:
     """ Helper function to convert ezomero shapes into omero shapes"""
     if isinstance(shape, Point):
         omero_shape = PointI()
         omero_shape.x = rdouble(shape.x)
         omero_shape.y = rdouble(shape.y)
     elif isinstance(shape, Line):
         omero_shape = LineI()
@@ -748,22 +710,31 @@
         omero_shape.theZ = rint(shape.z)
     if shape.c is not None:
         omero_shape.theC = rint(shape.c)
     if shape.t is not None:
         omero_shape.theT = rint(shape.t)
     if shape.label is not None:
         omero_shape.setTextValue(rstring(shape.label))
-    omero_shape.setFillColor(rint(_rgba_to_int(fill_color)))
-    omero_shape.setStrokeColor(rint(_rgba_to_int(stroke_color)))
-    omero_shape.setStrokeWidth(LengthI(stroke_width, enums.UnitsLength.PIXEL))
-
+    if shape.fill_color is not None:
+        omero_shape.setFillColor(rint(_rgba_to_int(shape.fill_color)))
+    else:
+        omero_shape.setFillColor(rint(_rgba_to_int((0, 0, 0, 0))))
+    if shape.stroke_color is not None:
+        omero_shape.setStrokeColor(rint(_rgba_to_int(shape.stroke_color)))
+    else:
+        omero_shape.setFillColor(rint(_rgba_to_int((255, 255, 0, 255))))
+    if shape.stroke_width is not None:
+        omero_shape.setStrokeWidth(LengthI(shape.stroke_width,
+                                           enums.UnitsLength.PIXEL))
+    else:
+        omero_shape.setStrokeWidth(LengthI(1.0, enums.UnitsLength.PIXEL))
     return omero_shape
 
 
-def _rgba_to_int(color: Tuple[int, int, int, int]) -> int:
+def _rgba_to_int(color: Tuple[int, ...]) -> int:
     """ Helper function returning the color as an Integer in RGBA encoding """
     try:
         r, g, b, a = color
     except ValueError:
         print('The format for the shape color is not addequate')
     r = r << 24
     g = g << 16
```

### Comparing `ezomero-1.2.1/ezomero/json_api.py` & `ezomero-2.0.0/ezomero/json_api.py`

 * *Files identical despite different names*

### Comparing `ezomero-1.2.1/ezomero.egg-info/PKG-INFO` & `ezomero-2.0.0/ezomero.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezomero
-Version: 1.2.1
+Version: 2.0.0
 Summary: A suite of convenience functions for working with OMERO. Written and maintained by the Research IT team at The Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/ezomero
 Maintainer: Dave Mellert
 Maintainer-email: Dave.Mellert@jax.org
 License: UNKNOWN
 Description: ![Run Tests](https://github.com/TheJacksonLaboratory/ezomero/workflows/Run%20Tests/badge.svg?event=push) ![](https://raw.githubusercontent.com/TheJacksonLaboratory/ezomero/main/coverage.svg)
```

### Comparing `ezomero-1.2.1/ezomero.egg-info/SOURCES.txt` & `ezomero-2.0.0/ezomero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezomero-1.2.1/setup.py` & `ezomero-2.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,16 +13,15 @@
                  " with OMERO. Written and maintained by the "
                  "Research IT team at The Jackson Laboratory."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheJacksonLaboratory/ezomero",
     packages=setuptools.find_packages(),
     install_requires=[
-        'omero-py==5.11.2',
-        'numpy>=1.22',
-        'dataclasses;python_version<"3.7"'
+        'omero-py==5.13.1',
+        'numpy>=1.22'
     ],
     extras_require={
         "tables": ["pandas"],
     },
     python_requires='>=3.8'
 )
```

### Comparing `ezomero-1.2.1/tests/conftest.py` & `ezomero-2.0.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -194,42 +194,57 @@
                                stdout=subprocess.PIPE,
                                stderr=subprocess.PIPE)
     stdoutval, stderrval = process.communicate()
 
 
 @pytest.fixture(scope='session')
 def roi_fixture():
-    point = rois.Point(x=100.0, y=100.0, z=0, c=0, t=0, label='test_point')
+    point = rois.Point(x=100.0, y=100.0, z=0, c=0, t=0, label='test_point',
+                       fill_color=(0, 1, 2, 3), stroke_color=(4, 5, 6, 100),
+                       stroke_width=1.0)
     line = rois.Line(x1=100.0, y1=100.0, x2=150.0, y2=150.0, z=0, c=0, t=0,
-                     label='test_line')
+                     label='test_line', fill_color=(7, 8, 9, 10),
+                     stroke_color=(11, 12, 13, 106), stroke_width=2.0)
     arrow = rois.Line(x1=100.0, y1=100.0, x2=150.0, y2=150.0, z=0, c=0, t=0,
                       label='test_arrow', markerEnd="Arrow",
                       markerStart="Arrow")
     rectangle = rois.Rectangle(x=100.0, y=100.0, width=50.0, height=40.0, z=0,
-                               c=0, t=0, label='test_rectangle')
+                               c=0, t=0, label='test_rectangle',
+                               fill_color=(14, 15, 16, 17),
+                               stroke_color=(18, 19, 20, 101),
+                               stroke_width=3.0)
     ellipse = rois.Ellipse(x=80, y=60, x_rad=20.0, y_rad=40.0, z=0, c=0, t=0,
-                           label='test_ellipse')
+                           label='test_ellipse',
+                           fill_color=(21, 22, 23, 24),
+                           stroke_color=(25, 26, 27, 102),
+                           stroke_width=4.0)
     polygon = rois.Polygon(points=[(100.0, 100.0),
                                    (110.0, 150.0),
                                    (100.0, 150.0)],
-                           z=0, c=0, t=0, label='test_polygon')
+                           z=0, c=0, t=0, label='test_polygon',
+                           fill_color=(28, 29, 30, 31),
+                           stroke_color=(32, 33, 34, 103),
+                           stroke_width=5.0)
     polyline = rois.Polyline(points=[(100.0, 100.0),
                                      (110.0, 150.0),
                                      (100.0, 150.0)],
-                             z=0, c=0, t=0, label='test_polyline')
+                             z=0, c=0, t=0, label='test_polyline',
+                             fill_color=(35, 36, 37, 38),
+                             stroke_color=(39, 40, 41, 104),
+                             stroke_width=6.0)
     label = rois.Label(x=100.0, y=100.0, z=0, c=0, t=0,
-                       label='test_label', fontSize=60)
+                       label='test_label', fontSize=60,
+                       fill_color=(42, 43, 44, 45),
+                       stroke_color=(46, 47, 48, 105),
+                       stroke_width=7.0)
 
     return {'shapes': [point, line, rectangle, ellipse,
                        polygon, polyline, arrow, label],
             'name': 'ROI_name',
-            'desc': 'A description for the ROI',
-            'fill_color': (255, 0, 0, 200),
-            'stroke_color': (255, 0, 0, 0),
-            'stroke_width': 2
+            'desc': 'A description for the ROI'
             }
 
 
 @pytest.fixture(scope='session')
 def timestamp():
     return f'{datetime.now():%Y%m%d%H%M%S}'
```

### Comparing `ezomero-1.2.1/tests/test_connect.py` & `ezomero-2.0.0/tests/test_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
                 "omero_user = fail\n"
                 "omero_group = fail\n"
                 "omero_host = fail\n"
                 "omero_port = 9999\n"
                 "omero_secure = True\n")
     conf_path = tmp_path / '.ezomero'
     conf_path.write_text(conf_txt)
-
     conn = ezomero.connect(user, password, host=host, group='', port=port,
                            secure=True, config_path=str(tmp_path))
     assert conn.getUser().getName() == user
     conn.close()
 
 
 def test_connect_env(omero_params, tmp_path, monkeypatch):
```

### Comparing `ezomero-1.2.1/tests/test_ezimport.py` & `ezomero-2.0.0/tests/test_ezimport.py`

 * *Files identical despite different names*

### Comparing `ezomero-1.2.1/tests/test_gets.py` & `ezomero-2.0.0/tests/test_gets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from attr import dataclass
 import pytest
 import numpy as np
 import ezomero
 from omero.gateway import TagAnnotationWrapper
 
 # Test gets
 ###########
@@ -448,18 +447,15 @@
 
     # test normal usage
     image_info = project_structure[2]
     im_id = image_info[0][1]
     roi_id = ezomero.post_roi(conn, im_id,
                               shapes=roi_fixture['shapes'],
                               name=roi_fixture['name'],
-                              description=roi_fixture['desc'],
-                              fill_color=roi_fixture['fill_color'],
-                              stroke_color=roi_fixture['stroke_color'],
-                              stroke_width=roi_fixture['stroke_width'])
+                              description=roi_fixture['desc'])
     return_ids = ezomero.get_roi_ids(conn, im_id)
     assert roi_id in return_ids
 
     # Test getting from an invalid cross-group
     username = users_groups[1][2][0]  # test_user3
     groupname = users_groups[0][1][0]  # test_group_2
     current_conn = conn.suConn(username, groupname)
@@ -482,30 +478,38 @@
         _ = ezomero.get_shape_ids(conn, '9999')
     with pytest.raises(TypeError):
         _ = ezomero.get_shape(conn, '9999')
 
     # test normal usage
     image_info = project_structure[2]
     im_id = image_info[0][1]
+    shapes = roi_fixture['shapes']
+    arrow = shapes.pop(6)
     roi_id = ezomero.post_roi(conn, im_id,
-                              shapes=roi_fixture['shapes'],
+                              shapes=shapes,
                               name=roi_fixture['name'],
-                              description=roi_fixture['desc'],
-                              fill_color=roi_fixture['fill_color'],
-                              stroke_color=roi_fixture['stroke_color'],
-                              stroke_width=roi_fixture['stroke_width'])
+                              description=roi_fixture['desc'])
     shape_ids = ezomero.get_shape_ids(conn, roi_id)
     assert len(shape_ids) == len(roi_fixture['shapes'])
     for i in range(len(shape_ids)):
-        shape, fill, stroke, width = ezomero.get_shape(conn, shape_ids[i])
+        shape = ezomero.get_shape(conn, shape_ids[i])
         assert hasattr(shape, 'label')
-        assert fill == roi_fixture['fill_color']
-        assert stroke == roi_fixture['stroke_color']
-        assert width == roi_fixture['stroke_width']
-
+        for pre_shape in shapes:
+            if type(shape) == type(pre_shape):
+                assert shape.fill_color == pre_shape.fill_color
+                assert shape.stroke_color == pre_shape.stroke_color
+                assert shape.stroke_width == pre_shape.stroke_width
+    roi_id2 = ezomero.post_roi(conn, im_id,
+                               shapes=[arrow],
+                               name=roi_fixture['name'],
+                               description=roi_fixture['desc'])
+    shape_ids2 = ezomero.get_shape_ids(conn, roi_id2)
+    assert len(shape_ids2) == 1
+    shape = ezomero.get_shape(conn, shape_ids2[0])
+    assert shape.markerStart == "Arrow"
     # Test getting from an invalid cross-group
     username = users_groups[1][2][0]  # test_user3
     groupname = users_groups[0][1][0]  # test_group_2
     current_conn = conn.suConn(username, groupname)
     empty_ret = ezomero.get_shape_ids(current_conn, roi_id)
     assert empty_ret is None
     current_conn.close()
```

### Comparing `ezomero-1.2.1/tests/test_json_api.py` & `ezomero-2.0.0/tests/test_json_api.py`

 * *Files identical despite different names*

### Comparing `ezomero-1.2.1/tests/test_misc.py` & `ezomero-2.0.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `ezomero-1.2.1/tests/test_posts.py` & `ezomero-2.0.0/tests/test_posts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from attr import dataclass
 import pytest
 import numpy as np
 import ezomero
 import filecmp
 import os
 import sys
 from unittest import mock
@@ -312,82 +311,30 @@
     im_id = image_info[0][1]
 
     # test sanitized input on post
     with pytest.raises(TypeError):
         _ = ezomero.post_roi(conn, '10',
                              shapes=roi_fixture['shapes'],
                              name=roi_fixture['name'],
-                             description=roi_fixture['desc'],
-                             fill_color=roi_fixture['fill_color'],
-                             stroke_color=roi_fixture['stroke_color'],
-                             stroke_width=roi_fixture['stroke_width'])
+                             description=roi_fixture['desc'])
     with pytest.raises(TypeError):
         _ = ezomero.post_roi(conn, im_id,
                              shapes='10',
                              name=roi_fixture['name'],
-                             description=roi_fixture['desc'],
-                             fill_color=roi_fixture['fill_color'],
-                             stroke_color=roi_fixture['stroke_color'],
-                             stroke_width=roi_fixture['stroke_width'])
+                             description=roi_fixture['desc'])
     with pytest.raises(TypeError):
         _ = ezomero.post_roi(conn, im_id,
                              shapes=['10'],
                              name=roi_fixture['name'],
-                             description=roi_fixture['desc'],
-                             fill_color=roi_fixture['fill_color'],
-                             stroke_color=roi_fixture['stroke_color'],
-                             stroke_width=roi_fixture['stroke_width'])
-    with pytest.raises(TypeError):
-        _ = ezomero.post_roi(conn, im_id,
-                             shapes=roi_fixture['shapes'],
-                             name=roi_fixture['name'],
-                             description=roi_fixture['desc'],
-                             fill_color=[10, 10, 10, 10],
-                             stroke_color=roi_fixture['stroke_color'],
-                             stroke_width=roi_fixture['stroke_width'])
-    with pytest.raises(ValueError):
-        _ = ezomero.post_roi(conn, im_id,
-                             shapes=roi_fixture['shapes'],
-                             name=roi_fixture['name'],
-                             description=roi_fixture['desc'],
-                             fill_color=(10, 10, 10),
-                             stroke_color=roi_fixture['stroke_color'],
-                             stroke_width=roi_fixture['stroke_width'])
-    with pytest.raises(TypeError):
-        _ = ezomero.post_roi(conn, im_id,
-                             shapes=roi_fixture['shapes'],
-                             name=roi_fixture['name'],
-                             description=roi_fixture['desc'],
-                             fill_color=roi_fixture['fill_color'],
-                             stroke_color=[10, 10, 10, 10],
-                             stroke_width=roi_fixture['stroke_width'])
-    with pytest.raises(ValueError):
-        _ = ezomero.post_roi(conn, im_id,
-                             shapes=roi_fixture['shapes'],
-                             name=roi_fixture['name'],
-                             description=roi_fixture['desc'],
-                             fill_color=roi_fixture['fill_color'],
-                             stroke_color=(10, 10, 10),
-                             stroke_width=roi_fixture['stroke_width'])
-    with pytest.raises(TypeError):
-        _ = ezomero.post_roi(conn, im_id,
-                             shapes=roi_fixture['shapes'],
-                             name=roi_fixture['name'],
-                             description=roi_fixture['desc'],
-                             fill_color=roi_fixture['fill_color'],
-                             stroke_color=roi_fixture['stroke_color'],
-                             stroke_width='width')
+                             description=roi_fixture['desc'])
 # "regular" test
     roi_id = ezomero.post_roi(conn, im_id,
                               shapes=roi_fixture['shapes'],
                               name=roi_fixture['name'],
-                              description=roi_fixture['desc'],
-                              fill_color=roi_fixture['fill_color'],
-                              stroke_color=roi_fixture['stroke_color'],
-                              stroke_width=roi_fixture['stroke_width'])
+                              description=roi_fixture['desc'])
     roi_in_omero = conn.getObject('Roi', roi_id)
     assert roi_in_omero.getName() == roi_fixture['name']
     assert roi_in_omero.getDescription() == roi_fixture['desc']
 
     # Test posting to a non-existing image
     im_id2 = 999999999
     with pytest.raises(Exception):  # TODO: verify which exception type
```

### Comparing `ezomero-1.2.1/tests/test_puts.py` & `ezomero-2.0.0/tests/test_puts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from attr import dataclass
 import pytest
 import ezomero
 
 # Test puts
 ###########
```

