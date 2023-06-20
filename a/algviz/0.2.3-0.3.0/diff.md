# Comparing `tmp/algviz-0.2.3.tar.gz` & `tmp/algviz-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algviz-0.2.3.tar", last modified: Sun Jun  4 17:07:59 2023, max compression
+gzip compressed data, was "algviz-0.3.0.tar", last modified: Tue Jun 20 12:51:07 2023, max compression
```

## Comparing `algviz-0.2.3.tar` & `algviz-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 17:07:59.656408 algviz-0.2.3/
--rw-rw-rw-   0        0        0    35149 2022-05-22 10:50:14.000000 algviz-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     4360 2023-06-04 17:07:59.655912 algviz-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3446 2023-05-05 10:41:17.000000 algviz-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 17:07:59.642998 algviz-0.2.3/algviz/
--rw-rw-rw-   0        0        0     2964 2023-06-04 13:51:17.000000 algviz-0.2.3/algviz/__init__.py
--rw-rw-rw-   0        0        0    15093 2022-12-23 04:24:34.000000 algviz-0.2.3/algviz/cursor.py
--rw-rw-rw-   0        0        0    11159 2023-06-04 16:53:31.000000 algviz-0.2.3/algviz/graph.py
--rw-rw-rw-   0        0        0     3658 2022-12-23 04:29:05.000000 algviz-0.2.3/algviz/graph_node_base.py
--rw-rw-rw-   0        0        0     5211 2022-12-23 04:29:24.000000 algviz-0.2.3/algviz/linked_list.py
--rw-rw-rw-   0        0        0     3408 2022-12-23 04:29:32.000000 algviz-0.2.3/algviz/logger.py
--rw-rw-rw-   0        0        0     6088 2022-12-23 09:41:37.000000 algviz-0.2.3/algviz/map.py
--rw-rw-rw-   0        0        0    35861 2022-12-23 09:09:51.000000 algviz-0.2.3/algviz/svg_graph.py
--rw-rw-rw-   0        0        0    20308 2022-12-23 04:33:10.000000 algviz-0.2.3/algviz/svg_table.py
--rw-rw-rw-   0        0        0    19828 2023-05-24 12:25:12.000000 algviz-0.2.3/algviz/table.py
--rw-rw-rw-   0        0        0    12028 2022-12-23 04:34:15.000000 algviz-0.2.3/algviz/tree.py
--rw-rw-rw-   0        0        0    13626 2023-06-04 16:42:18.000000 algviz-0.2.3/algviz/utility.py
--rw-rw-rw-   0        0        0    21393 2022-12-23 04:35:13.000000 algviz-0.2.3/algviz/vector.py
--rw-rw-rw-   0        0        0     9785 2023-05-24 13:11:24.000000 algviz-0.2.3/algviz/visual.py
-drwxrwxrwx   0        0        0        0 2023-06-04 17:07:59.649952 algviz-0.2.3/algviz.egg-info/
--rw-rw-rw-   0        0        0     4360 2023-06-04 17:07:59.000000 algviz-0.2.3/algviz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-06-04 17:07:59.000000 algviz-0.2.3/algviz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 17:07:59.000000 algviz-0.2.3/algviz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-04 17:07:59.000000 algviz-0.2.3/algviz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       82 2023-06-04 17:07:59.000000 algviz-0.2.3/algviz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-04 17:07:59.000000 algviz-0.2.3/algviz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 17:07:59.656408 algviz-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1486 2023-06-04 16:41:58.000000 algviz-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 17:07:59.655415 algviz-0.2.3/tests/
--rw-rw-rw-   0        0        0    11071 2023-06-04 14:03:48.000000 algviz-0.2.3/tests/test_graph.py
--rw-rw-rw-   0        0        0    10959 2022-12-23 04:06:37.000000 algviz-0.2.3/tests/test_linked_list.py
--rw-rw-rw-   0        0        0     1972 2022-12-23 04:03:34.000000 algviz-0.2.3/tests/test_logger.py
--rw-rw-rw-   0        0        0     4097 2022-12-23 10:32:23.000000 algviz-0.2.3/tests/test_map.py
--rw-rw-rw-   0        0        0      921 2023-05-24 12:50:29.000000 algviz-0.2.3/tests/test_regression.py
--rw-rw-rw-   0        0        0    11905 2022-12-23 04:06:44.000000 algviz-0.2.3/tests/test_table.py
--rw-rw-rw-   0        0        0    10612 2022-12-23 04:42:51.000000 algviz-0.2.3/tests/test_tree.py
--rw-rw-rw-   0        0        0    10670 2022-12-23 04:07:06.000000 algviz-0.2.3/tests/test_vector.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:51:07.301268 algviz-0.3.0/
+-rw-rw-rw-   0        0        0    35149 2022-05-22 10:50:14.000000 algviz-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-06-19 15:08:36.000000 algviz-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4454 2023-06-20 12:51:07.300271 algviz-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3533 2023-06-19 16:43:36.000000 algviz-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 12:51:07.291301 algviz-0.3.0/algviz/
+-rw-rw-rw-   0        0        0     2964 2023-06-18 04:07:49.000000 algviz-0.3.0/algviz/__init__.py
+-rw-rw-rw-   0        0        0    15093 2022-12-23 04:24:34.000000 algviz-0.3.0/algviz/cursor.py
+-rw-rw-rw-   0        0        0    11159 2023-06-04 16:53:31.000000 algviz-0.3.0/algviz/graph.py
+-rw-rw-rw-   0        0        0     3658 2022-12-23 04:29:05.000000 algviz-0.3.0/algviz/graph_node_base.py
+-rw-rw-rw-   0        0        0    12293 2023-06-19 16:27:25.000000 algviz-0.3.0/algviz/layouter.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:51:07.296288 algviz-0.3.0/algviz/lib/
+-rw-rw-rw-   0        0        0    73488 2023-06-18 14:31:12.000000 algviz-0.3.0/algviz/lib/packing_solver_linux_amd64.so
+-rw-rw-rw-   0        0        0    52224 2023-06-18 14:48:49.000000 algviz-0.3.0/algviz/lib/packing_solver_win_amd64.dll
+-rw-rw-rw-   0        0        0     5211 2022-12-23 04:29:24.000000 algviz-0.3.0/algviz/linked_list.py
+-rw-rw-rw-   0        0        0     3408 2022-12-23 04:29:32.000000 algviz-0.3.0/algviz/logger.py
+-rw-rw-rw-   0        0        0    10963 2023-06-19 16:27:56.000000 algviz-0.3.0/algviz/logo.py
+-rw-rw-rw-   0        0        0     6088 2022-12-23 09:41:37.000000 algviz-0.3.0/algviz/map.py
+-rw-rw-rw-   0        0        0    10880 2023-06-19 16:29:23.000000 algviz-0.3.0/algviz/sequencer.py
+-rw-rw-rw-   0        0        0    35861 2022-12-23 09:09:51.000000 algviz-0.3.0/algviz/svg_graph.py
+-rw-rw-rw-   0        0        0    20460 2023-06-20 10:36:01.000000 algviz-0.3.0/algviz/svg_table.py
+-rw-rw-rw-   0        0        0    19828 2023-05-24 12:25:12.000000 algviz-0.3.0/algviz/table.py
+-rw-rw-rw-   0        0        0    12028 2022-12-23 04:34:15.000000 algviz-0.3.0/algviz/tree.py
+-rw-rw-rw-   0        0        0    13626 2023-06-20 12:01:04.000000 algviz-0.3.0/algviz/utility.py
+-rw-rw-rw-   0        0        0    21393 2022-12-23 04:35:13.000000 algviz-0.3.0/algviz/vector.py
+-rw-rw-rw-   0        0        0    11254 2023-06-20 10:01:27.000000 algviz-0.3.0/algviz/visual.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:51:07.295287 algviz-0.3.0/algviz.egg-info/
+-rw-rw-rw-   0        0        0     4454 2023-06-20 12:51:07.000000 algviz-0.3.0/algviz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      816 2023-06-20 12:51:07.000000 algviz-0.3.0/algviz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 12:51:07.000000 algviz-0.3.0/algviz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-20 12:51:07.000000 algviz-0.3.0/algviz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       82 2023-06-20 12:51:07.000000 algviz-0.3.0/algviz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-20 12:51:07.000000 algviz-0.3.0/algviz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 12:51:07.301268 algviz-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1554 2023-06-20 12:00:39.000000 algviz-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:51:07.300271 algviz-0.3.0/tests/
+-rw-rw-rw-   0        0        0    11071 2023-06-04 14:03:48.000000 algviz-0.3.0/tests/test_graph.py
+-rw-rw-rw-   0        0        0    10959 2022-12-23 04:06:37.000000 algviz-0.3.0/tests/test_linked_list.py
+-rw-rw-rw-   0        0        0     1972 2023-06-18 06:55:42.000000 algviz-0.3.0/tests/test_logger.py
+-rw-rw-rw-   0        0        0     4097 2022-12-23 10:32:23.000000 algviz-0.3.0/tests/test_map.py
+-rw-rw-rw-   0        0        0      921 2023-05-24 12:50:29.000000 algviz-0.3.0/tests/test_regression.py
+-rw-rw-rw-   0        0        0    11905 2022-12-23 04:06:44.000000 algviz-0.3.0/tests/test_table.py
+-rw-rw-rw-   0        0        0    10612 2022-12-23 04:42:51.000000 algviz-0.3.0/tests/test_tree.py
+-rw-rw-rw-   0        0        0    10670 2022-12-23 04:07:06.000000 algviz-0.3.0/tests/test_vector.py
```

### Comparing `algviz-0.2.3/LICENSE` & `algviz-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/PKG-INFO` & `algviz-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algviz
-Version: 0.2.3
+Version: 0.3.0
 Summary: An algorithm visualization tool for jupyter notebook to show animation for vector, table, linked list, tree and graph data structures.
 Home-page: https://algviz.com/
 Author: zjl9959
 Author-email: zjl9959@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://algviz.readthedocs.io/en/latest/index.html
 Project-URL: Issue Tracker, https://github.com/zjl9959/algviz/issues
@@ -93,7 +93,14 @@
 If you want to share your algorithm animation notebooks using algviz, you can create a [PR](https://github.com/zjl9959/algviz-launch/pulls) from this repo: 👉 [algviz-launch](https://github.com/zjl9959/algviz-launch).
 
 [bubble sort algorithm]: https://en.wikipedia.org/wiki/Bubble_sort
 [vector.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_vector.svg
 [table.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_table.svg
 [tree.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_tree.svg
 [graph.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_graph.svg
+
+
+## Discussion
+
+**QQ group**: 334605370
+
+**Telegram**: https://t.me/+mvF8Sivxr3thZWY1
```

### Comparing `algviz-0.2.3/README.md` & `algviz-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -74,7 +74,14 @@
 If you want to share your algorithm animation notebooks using algviz, you can create a [PR](https://github.com/zjl9959/algviz-launch/pulls) from this repo: 👉 [algviz-launch](https://github.com/zjl9959/algviz-launch).
 
 [bubble sort algorithm]: https://en.wikipedia.org/wiki/Bubble_sort
 [vector.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_vector.svg
 [table.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_table.svg
 [tree.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_tree.svg
 [graph.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_graph.svg
+
+
+## Discussion
+
+**QQ group**: 334605370
+
+**Telegram**: https://t.me/+mvF8Sivxr3thZWY1
```

### Comparing `algviz-0.2.3/algviz/__init__.py` & `algviz-0.3.0/algviz/__init__.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/algviz/cursor.py` & `algviz-0.3.0/algviz/cursor.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/algviz/graph.py` & `algviz-0.3.0/algviz/graph.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/algviz/graph_node_base.py` & `algviz-0.3.0/algviz/graph_node_base.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/algviz/linked_list.py` & `algviz-0.3.0/algviz/linked_list.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/algviz/logger.py` & `algviz-0.3.0/algviz/logger.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/algviz/map.py` & `algviz-0.3.0/algviz/map.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/algviz/svg_graph.py` & `algviz-0.3.0/algviz/svg_graph.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/algviz/svg_table.py` & `algviz-0.3.0/algviz/svg_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         g.appendChild(r)
         if text is not None:
             t = self._dom.createElement('text')
             t.setAttribute('class', 'txt')
             t.setAttribute('x', '{:.2f}'.format(rect[0] + rect[2] * 0.5))
             t.setAttribute('y', '{:.2f}'.format(rect[1] + rect[3] * 0.5))
             txt_font_size = min(rect[3] - 1, text_font_size(rect[2], '{}'.format(text)))
+            txt_font_size = max(txt_font_size, 4)
             t.setAttribute('font-size', '{:.2f}'.format(txt_font_size))
             t.setAttribute('fill', auto_text_color(fill))
             tt = self._dom.createTextNode('{}'.format(text))
             t.appendChild(tt)
             g.appendChild(t)
         return int(gid)
 
@@ -191,15 +192,16 @@
                 t.setAttribute('x', '{:.2f}'.format(rect[0] + rect[2] * 0.5))
                 t.setAttribute('y', '{:.2f}'.format(rect[1] + rect[3] * 0.5))
                 if t.getAttribute('font-size') == '0':
                     continue
                 for child in t.childNodes:
                     if child.nodeType == Node.TEXT_NODE:
                         new_font = text_font_size(rect[2], '{}'.format(child.data))
-                        t.setAttribute('font-size', '{:.2f}'.format(min(new_font, rect[3] - 1)))
+                        new_font = max(4, min(new_font, rect[3] - 1))
+                        t.setAttribute('font-size', '{:.2f}'.format(new_font))
                         break
         if text is not None:
             rx = float(r.getAttribute('x'))
             ry = float(r.getAttribute('y'))
             width = float(r.getAttribute('width'))
             height = float(r.getAttribute('height'))
             fc = str2rgbcolor(r.getAttribute('fill'))
@@ -212,14 +214,15 @@
             t1 = self._dom.createElement('text')
             g.appendChild(t1)
             t1.setAttribute('class', 'txt')
             t1.setAttribute('x', '{:.2f}'.format(rx + width * 0.5))
             t1.setAttribute('y', '{:.2f}'.format(ry + height * 0.5))
             txt_font_size = text_font_size(width, '{}'.format(text))
             txt_font_size = min(height - 1, txt_font_size)
+            txt_font_size = max(txt_font_size, 4)
             t1.setAttribute('font-size', '0')
             t1.setAttribute('fill', auto_text_color(fc))
             tt = self._dom.createTextNode('{}'.format(text))
             t1.appendChild(tt)
             animate1 = self._dom.createElement('animate')
             add_animate_scale_into_text(t1, animate1, time1, txt_font_size, True)
         if stroke is not None:
```

### Comparing `algviz-0.2.3/algviz/table.py` & `algviz-0.3.0/algviz/table.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/algviz/tree.py` & `algviz-0.3.0/algviz/tree.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/algviz/utility.py` & `algviz-0.3.0/algviz/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Author: zjl9959@gmail.com
 
 License: GPLv3
 
 """
 
-_version = '0.2.3'                  # algviz version
+_version = '0.3.0'                  # algviz version
 _url = 'https://algviz.com'         # The homepage for algviz
 RANDOM_SEED = None
 KFATAL_HELP_INFO = """You can report this bug from link: https://github.com/zjl9959/algviz/issues"""
 
 
 # Define exceptions for algviz runtime.
 class AlgvizParamError(Exception):
```

### Comparing `algviz-0.2.3/algviz/vector.py` & `algviz-0.3.0/algviz/vector.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/algviz/visual.py` & `algviz-0.3.0/algviz/visual.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from algviz.table import Table
 from algviz.vector import Vector
 from algviz.svg_graph import SvgGraph
 from algviz.svg_table import SvgTable
 from algviz.logger import Logger
 from algviz.cursor import Cursor, _CursorRange
 from algviz.map import Map
-from algviz.utility import AlgvizParamError, AlgvizTypeError, kMaxNameChars
+from algviz.utility import AlgvizParamError, AlgvizTypeError, AlgvizRuntimeError, kMaxNameChars
+from algviz.layouter import Layouter, is_layout_supported
 
 
 class _NoDisplay():
     def _repr_svg_(self):
         return ''
 
 
@@ -38,20 +39,21 @@
 
 
 _next_display_id = 0
 
 
 class Visualizer():
 
-    def __init__(self, delay=2.0, wait=0.5):
+    def __init__(self, delay=2.0, wait=0.5, layout=False):
         """
         Args:
             delay (float): Animation delay time (in seconds).
             wait (True/float/int): (True) wait for the key input to continue execute the code.
                                    (float/int) the wait time before start the next frame of animation.
+            layout (boolean): wheather to layout different display objects or not.
         """
         self._delay = 2.0               # Set default delay time for animation as 3.0 seconds.
         if delay > 0:
             self._delay = delay
         self._wait = wait
         if type(self._wait) != bool and type(self._wait) != float and type(self._wait) != int:
             self._wait = 0.5
@@ -64,14 +66,19 @@
         self._element2display = WeakKeyDictionary()
         # Record the displayed id. If object is not displayed, call the display interface, otherwise call the update interface.
         self._displayed = set()
         # The mapping relationship between the display object and the object's name.
         self._displayid2name = dict()
         # The next unique cursor id created by this visualizer.
         self._next_cursor_id = -1
+        # Init display engine.
+        if layout is True and is_layout_supported():
+            self._layouter = Layouter()
+        else:
+            self._layouter = None
 
     def display(self, delay=None):
         """Refresh all created display objects.
 
         Args:
             delay (float): Specific the delay time for this animation frame (in seconds).
         """
@@ -79,46 +86,51 @@
             delay = self._delay
         if type(self._wait) == float or type(self._wait) == int:
             for elem in self._element2display.keyrefs():
                 did = self._element2display[elem()]
                 if did not in self._displayed:
                     if did in self._displayid2name:
                         svg_title = _NameDisplay(self._displayid2name[did])
-                        display.display(svg_title, display_id='algviz_{}'.format(did))
+                        self._display(svg_title, 'algviz_{}'.format(did))
                     elem()._delay = delay
-                    display.display(elem(), display_id='algviz{}'.format(did))
+                    self._display(elem(), 'algviz{}'.format(did))
                     self._displayed.add(did)
                 else:
                     if did in self._displayid2name:
                         svg_title = _NameDisplay(self._displayid2name[did])
-                        display.update_display(svg_title, display_id='algviz_{}'.format(did))
+                        self._update_display(svg_title, 'algviz_{}'.format(did))
                     elem()._delay = delay
-                    display.update_display(elem(), display_id='algviz{}'.format(did))
+                    self._update_display(elem(), 'algviz{}'.format(did))
             temp_displayed = list(self._displayed)
             for did in temp_displayed:
                 if did not in self._element2display.values():
                     if did in self._displayid2name:
-                        display.update_display(_NoDisplay(), display_id='algviz_{}'.format(did))
-                    display.update_display(_NoDisplay(), display_id='algviz{}'.format(did))
+                        self._update_display(_NoDisplay(), 'algviz_{}'.format(did))
+                    self._update_display(_NoDisplay(), 'algviz{}'.format(did))
                     self._displayed.remove(did)
-            sleep(delay + self._wait)
+            if self._layouter is not None:
+                self._layouter.next_frame(delay + self._wait)
+            else:
+                sleep(delay + self._wait)
             return None
-        else:
+        elif self._wait is True and self._layouter is None:
             display.clear_output(wait=True)
             for elem in self._element2display.keyrefs():
                 did = self._element2display[elem()]
                 if did in self._displayid2name:
                     svg_title = SvgTable(400, 17)
                     title_name = '{}:'.format(self._displayid2name[did])
                     svg_title.add_text_element((4, 14), title_name, font_size=14, fill=(0, 0, 0))
                     display.display(svg_title, display_id='algviz_{}'.format(did))
                 elem()._delay = delay
                 display.display(elem(), display_id='algviz{}'.format(did))
                 self._displayed.add(did)
             return input('Input `Enter` to continue:')
+        else:
+            raise AlgvizRuntimeError('Invalid wait:{} parameter'.format(self._wait))
 
     def createTable(self, row, col, data=None, name=None, cell_size=(40, 40), show_index=True):
         """
         Args:
             row, col (int): The number of rows, columns for this table.
             data (list(list(printable))): The initial data for table cells.
             name (str): The name of this table object.
@@ -247,7 +259,34 @@
         """
         if type(st) is Cursor:
             st = st.index()
         if type(ed) is Cursor:
             ed = ed.index()
         self._next_cursor_id += 1
         return _CursorRange(self._next_cursor_id, name, st, ed, step)
+
+    def layout(self, max_width=800):
+        """Layout all the svg animation pictures.
+        Args:
+            max_width (int): The maximum strip width limit to layouter.
+
+        Returns:
+            str: The final svg string to display.
+        """
+        if self._layouter is None:
+            return
+        global _next_display_id
+        self._layouter._max_width = max_width
+        display.display(self._layouter, display_id='algviz_{}'.format(_next_display_id))
+        _next_display_id += 1
+
+    def _display(self, content, did):
+        if self._layouter is None:
+            display.display(content, display_id=did)
+        else:
+            self._layouter.display(content, display_id=did)
+
+    def _update_display(self, content, did):
+        if self._layouter is None:
+            display.update_display(content, display_id=did)
+        else:
+            self._layouter.update_display(content, display_id=did)
```

### Comparing `algviz-0.2.3/algviz.egg-info/PKG-INFO` & `algviz-0.3.0/algviz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algviz
-Version: 0.2.3
+Version: 0.3.0
 Summary: An algorithm visualization tool for jupyter notebook to show animation for vector, table, linked list, tree and graph data structures.
 Home-page: https://algviz.com/
 Author: zjl9959
 Author-email: zjl9959@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://algviz.readthedocs.io/en/latest/index.html
 Project-URL: Issue Tracker, https://github.com/zjl9959/algviz/issues
@@ -93,7 +93,14 @@
 If you want to share your algorithm animation notebooks using algviz, you can create a [PR](https://github.com/zjl9959/algviz-launch/pulls) from this repo: 👉 [algviz-launch](https://github.com/zjl9959/algviz-launch).
 
 [bubble sort algorithm]: https://en.wikipedia.org/wiki/Bubble_sort
 [vector.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_vector.svg
 [table.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_table.svg
 [tree.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_tree.svg
 [graph.svg]: https://cdn.jsdelivr.net/gh/zjl9959/algviz.com@master/assets/img/data_graph.svg
+
+
+## Discussion
+
+**QQ group**: 334605370
+
+**Telegram**: https://t.me/+mvF8Sivxr3thZWY1
```

### Comparing `algviz-0.2.3/setup.py` & `algviz-0.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,28 +15,31 @@
 readme_filepath = path.join(script_path, 'README.md')
 long_description_data = ''
 with open(readme_filepath, encoding='utf-8') as f:
     long_description_data = f.read()
 
 setup(
     name="algviz",
-    version="0.2.3",
+    version="0.3.0",
     author="zjl9959",
     author_email="zjl9959@gmail.com",
     description=("An algorithm visualization tool for jupyter notebook to show animation for vector, table, linked list, tree and graph data structures."),
     long_description=long_description_data,
     long_description_content_type="text/markdown",
     license="GPLv3",
     keywords="Algorithm Visualizer Animation Jupyter-notebook Graph",
     url="https://algviz.com/",
     project_urls={
         "Documentation": "https://algviz.readthedocs.io/en/latest/index.html",
         "Issue Tracker": "https://github.com/zjl9959/algviz/issues",
     },
     packages=['algviz'],
+    package_data={
+        'algviz': ['lib/packing_solver*']
+    },
     install_requires=[
         'graphviz >= 0.8.4, != 0.18, <= 0.20.1',
         'ipykernel >= 6.4.0, <= 6.23.1',
         'ipython >= 8.0.0, <= 8.12.0'
     ],
     python_requires='>=3.8',
     classifiers=[
```

### Comparing `algviz-0.2.3/tests/test_graph.py` & `algviz-0.3.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/tests/test_linked_list.py` & `algviz-0.3.0/tests/test_linked_list.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/tests/test_logger.py` & `algviz-0.3.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/tests/test_map.py` & `algviz-0.3.0/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/tests/test_regression.py` & `algviz-0.3.0/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/tests/test_table.py` & `algviz-0.3.0/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/tests/test_tree.py` & `algviz-0.3.0/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `algviz-0.2.3/tests/test_vector.py` & `algviz-0.3.0/tests/test_vector.py`

 * *Files identical despite different names*

