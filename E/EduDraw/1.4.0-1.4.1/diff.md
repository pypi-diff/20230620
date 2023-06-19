# Comparing `tmp/edudraw-1.4.0.tar.gz` & `tmp/edudraw-1.4.1.tar.gz`

## Comparing `edudraw-1.4.0.tar` & `edudraw-1.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edudraw-1.4.0/src/EduDraw/__init__.py
--rw-r--r--   0        0        0    66011 2020-02-02 00:00:00.000000 edudraw-1.4.0/src/EduDraw/edudraw.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 edudraw-1.4.0/src/EduDraw/requirements.txt
--rw-r--r--   0        0        0    17985 2020-02-02 00:00:00.000000 edudraw-1.4.0/tests/edudraw_tests.py
--rw-r--r--   0        0        0    27030 2020-02-02 00:00:00.000000 edudraw-1.4.0/LICENSE
--rw-r--r--   0        0        0    39773 2020-02-02 00:00:00.000000 edudraw-1.4.0/README.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 edudraw-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    38938 2020-02-02 00:00:00.000000 edudraw-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edudraw-1.4.1/src/EduDraw/__init__.py
+-rw-r--r--   0        0        0    66576 2020-02-02 00:00:00.000000 edudraw-1.4.1/src/EduDraw/edudraw.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 edudraw-1.4.1/src/EduDraw/requirements.txt
+-rw-r--r--   0        0        0    18246 2020-02-02 00:00:00.000000 edudraw-1.4.1/tests/edudraw_tests.py
+-rw-r--r--   0        0        0    27030 2020-02-02 00:00:00.000000 edudraw-1.4.1/LICENSE
+-rw-r--r--   0        0        0    44932 2020-02-02 00:00:00.000000 edudraw-1.4.1/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 edudraw-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    43965 2020-02-02 00:00:00.000000 edudraw-1.4.1/PKG-INFO
```

### Comparing `edudraw-1.4.0/src/EduDraw/edudraw.py` & `edudraw-1.4.1/src/EduDraw/edudraw.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,17 @@
 
             if self.interval != 0:
                 time.sleep(self.interval)
 
     def quit(self):
         self.flag = True
 
+    def change_interval(self, new_deltatime: int):
+        self.interval = new_deltatime / 1000
+
 
 class _SimulationData:
     """
     Helper class to hold simulation data
     """
     def __init__(self):
         self.draw_mode = {'TOP_LEFT': 0, 'CENTER': 1}
@@ -137,15 +140,15 @@
 
 class EduDraw:
     def __init__(self, width: int, height: int, null_mode: bool = False):
         global _instance_handler
         self.width = width
         self.height = height
 
-        self.timeloop = None
+        self.timeloop: None | _RepeatTimer = None
         self.deltatime = 1
 
         self.null_mode = null_mode
 
         if null_mode:
             _instance_handler.add(self)
 
@@ -1792,16 +1795,33 @@
             pygame.mouse.set_visible(visible)
 
     def frame_rate(self, fps: int):
         """
         Sets the desired frame rate. Note that EduDraw using python is slower than it's C# counterpart.
         :param fps: The desired FPS rate.
         """
+
+        if fps == 0:
+            return
+
         self.deltatime = 1000 / fps
 
+        if self.timeloop is not None:
+            self.timeloop.change_interval(int(self.deltatime))
+
+    def use_max_frame_rate(self):
+        """
+        Changes the inner time between frames to zero, the frame rate is determined by computation speed and may vary
+        """
+
+        self.deltatime = 0
+
+        if self.timeloop is not None:
+            self.timeloop.interval = 0
+
     def save(self, filename: str):
         """
         Saves a picture of the current frame
 
         :param filename: The name to give the resulting file (Ex: 'MyPhoto.png')
         """
         if filename == '':
```

### Comparing `edudraw-1.4.0/tests/edudraw_tests.py` & `edudraw-1.4.1/tests/edudraw_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,40 +15,44 @@
 start = time.time()
 
 antialias = False
 
 # Note: This is just a test picture, nothing special
 img = pygame.image.load(r"Image\path\goes\here")
 
+
 def pressed(data):
     global antialias
     antialias = not antialias
 
 
 def setup():
     # s.frame_rate(50)
     s.deltatime = 0
     s.set_controls(key_down=pressed)
 
+
 flag_has_null = False
 
+
 def draw():
     global flag_done, start, end, flag_has_null
 
     # print(s._get_data_object().custom_font_object)
 
     if antialias:
         s.toggle_antialiasing()
 
     if len(tests) == 0:
         # d.quit()
         if flag_done:
             s.quit()
             end = time.time()
-            print(f"Test done: {str(test_null_mode)}, Elapsed time: {end - start}, Avg. FPS: {s.frame_count / (end - start)}")
+            print(f"Test done: {str(test_null_mode)}, Elapsed time: {end - start}, "
+                  f"Avg. FPS: {s.frame_count / (end - start)}")
             print(f"Avg. fps for inner instance: {d.frame_count / (end - start)}")
             print("All tests done.")
             return
         else:
             if not flag_has_null:
                 start = time.time()
                 d.start(dummy, inner_drawing, "This should not appear")
@@ -66,16 +70,19 @@
             gc.collect()
             # d.frame_count = 0
 
 
 def dummy():
     pass
 
+
 position = [d.width/2, d.height//2]
 velocity = [3, 4]
+
+
 def inner_drawing():
     global position, velocity
     if position[0] < 0 or position[0] > d.width:
         velocity[0] *= -1
 
     if position[1] < 0 or position[1] > d.height:
         velocity[1] *= -1
@@ -683,16 +690,14 @@
 
     if s.frame_count > 40:
         flag_done = True
 
 
 tests.append(test_polygon)
 
-# Note: This is just a test picture, nothing special
-img = pygame.image.load(r"File\path\goes\here")
 
 def test_image():
     global flag_done
 
     s.scale(0.75, 1.25)
     s.background((200, 200, 200))
     s.image(img, 50, 50, 200, 200)
@@ -848,9 +853,25 @@
     if s.frame_count > 160:
         flag_done = True
 
 
 tests.append(test_lerp)
 
 
-s.start(setup, draw, "Running tests")
+def test_framerate():
+    global flag_done
+    s.background((255, 255, 255))
+    s.fill((255, 0, 0))
+
+    s.frame_rate(s.frame_count % 100)
+
+    s.circle(s.frame_count % s.width, s.height//2, 25)
+
+    if s.frame_count > 100:
+        s.use_max_frame_rate()
+        flag_done = True
 
+
+tests.append(test_framerate)
+
+
+s.start(setup, draw, "Running tests")
```

### Comparing `edudraw-1.4.0/LICENSE` & `edudraw-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edudraw-1.4.0/README.md` & `edudraw-1.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,142 @@
 
 This project is aimed to provide an interface that allows for a simplified experience when using basic 2D graphics in the Python language. 
 
 The general design of the interface is heavily (if not all) inspired by the [P5.js](https://p5js.org/) library and the Processing library, and is intended to make simple graphical programs easy to do in the .NET environment in the shape of a Windows Forms app and/or in the Python language.
 
 The details of installation and documentation of the respective versions are below. 
 
+## Summary
+
+* 1.0. [Installation](#installation)
+
+* 2.0. [Setting up](#setting-up) 
+
+* 3.0. [Documentation](#documentation)
+
+  * 3.1. [State methods](#state-methods)  
+    
+    * 3.1.1. [EduDraw()](#edudrawwidth-int-height-int-null_mode-bool--false---edudraw)
+    
+    * 3.1.2. [EduDraw.start()](#edudrawstartsetup-draw-window_title-str)
+
+    * 3.1.3. [EduDraw.rect_mode()](#edudrawrect_modemode-str)
+  
+    * 3.1.4. [EduDraw.circle_mode()](#edudrawcircle_modemode-str)
+
+    * 3.1.5. [EduDraw.fill()](#edudrawfillcolor-tuple)
+
+    * 3.1.6. [EduDraw.no_fill()](#edudrawno_fill)
+
+    * 3.1.7. [EduDraw.font()](#edudrawfontnew_font-str-font_size-int--12-boldfalse-italicfalse-underlinefalse)
+
+    * 3.1.8. [EduDraw.font_from_instance()](#edudrawfont_from_instancenew_font-pygamefontfont)
+
+    * 3.1.9. [EduDraw.change_default_font()](#edudrawchange_default_fontnew_font-str-font_size-int--12-boldfalse-italicfalse-underlinefalse)
+
+    * 3.1.10. [EduDraw.reset_font()](#edudrawreset_font)
+
+    * 3.1.11. [EduDraw.stroke()](#edudrawstrokecolor-tuple)
+
+    * 3.1.12. [EduDraw.no_stroke()](#edudrawno_stroke)
+
+    * 3.1.13. [EduDraw.stroke_weight()](#edudrawstroke_weightnew_weight-int)
+
+    * 3.1.14. [EduDraw.push()](#edudrawpush)
+
+    * 3.1.15. [EduDraw.pop()](#edudrawpop)
+
+    * 3.1.16. [EduDraw.mouse_pos()](#edudrawmouse_pos--tuple)
+
+    * 3.1.17. [EduDraw.rotate()](#edudrawrotateangle-int)
+
+    * 3.1.18. [EduDraw.scale()](#edudrawscalescale_x-float-scale_y-float)
+
+    * 3.1.19. [EduDraw.translate()](#edudrawtranslatetranslate_x-int-translate_y-int)
+
+    * 3.1.20. [EduDraw.reset_transformations()](#edudrawreset_transformations)
+
+    * 3.1.21. [EduDraw.reset_scaling()](#edudrawreset_scaling)
+
+    * 3.1.22. [EduDraw.reset_translation()](#edudrawreset_translation)
+
+    * 3.1.23. [EduDraw.reset_rotation()](#edudrawreset_rotation)
+
+    * 3.1.24. [EduDraw.set_account_for_transformations()](#edudrawset_account_for_transformationsstate-bool)
+
+    * 3.1.25. [EduDraw.set_controls()](#edudrawset_controlskey_downnone-key_upnone-mouse_motionnone-mouse_button_upnone-mouse_button_downnone-mouse_wheelnone)
+
+    * 3.1.26. [EduDraw.toggle_antialiasing()](#edudrawtoggle_antialiasing)
+
+    * 3.1.27. [EduDraw.erase()](#edudrawerase)
+
+    * 3.1.28. [EduDraw.no_erase()](#edudrawno_erase)
+
+  * 3.2. [Drawing methods](#drawing-methods)
+
+     * 3.2.1. [EduDraw.point()](#edudrawpointx-int-y-int)
+
+     * 3.2.2. [EduDraw.text()](#edudrawtextstring-str-x-int-y-int)
+
+     * 3.2.3. [EduDraw.background()](#edudrawbackgroundcolor-tuple)
+
+     * 3.2.4. [EduDraw.circle()](#edudrawcirclex-int-y-int-radius-int)
+    
+     * 3.2.5. [EduDraw.ellipse()](#edudrawellipsex-int-y-int-width-int-height-int)
+
+     * 3.2.6. [EduDraw.line()](#edudrawlinex1-int-y1-int-x2-int-y2-int)
+
+     * 3.2.7. [EduDraw.rect()](#edudrawrectx-int-y-int-width-int-height-int)
+
+     * 3.2.8. [EduDraw.square()](#edudrawsquarex-int-y-int-side_size-int)
+
+     * 3.2.9. [EduDraw.triangle()](#edudrawtrianglex1-int-y1-int-x2-int-y2-int-x3-int-y3-int)
+
+     * 3.2.10. [EduDraw.polygon()](#edudrawpolygonpoints-list)
+
+     * 3.2.11. [EduDraw.image()](#edudrawimageimg-pygamesurfacesurface-x-int-y-int-width-int--none-height-int--none-force_transparency-bool--false)
+
+     * 3.2.12. [EduDraw.bezier_curve()](#edudrawbezier_curveself-control_points-list-num_points-int--none--none)
+
+     * 3.2.13. [EduDraw.arc_open()](#edudrawarc_openself-start_angle-int-stop_angle-int-x-int-y-int-width-int-height-int)
+
+     * 3.2.14. [EduDraw.arc_pie()](#edudrawarc_piestart_angle-int-stop_angle-int-x-int-y-int-width-int-height-int-close_edges-bool--true)
+
+     * 3.2.15. [EduDraw.arc_closed()](#edudrawarc_closedstart_angle-int-stop_angle-int-x-int-y-int-width-int-height-int-close_edges-bool--true)
+
+   * 3.3. [Other methods](#other-methods)
+
+     * 3.3.1. [EduDraw.frame_rate()](#edudrawframe_ratefps-int)
+
+     * 3.3.2. [EduDraw.use_max_frame_rate()](#edudrawuse_max_frame_rate)
+
+     * 3.3.3. [EduDraw.save()](#edudrawsavefilename-str)
+
+     * 3.3.4. [EduDraw.quit()](#edudrawquit)
+
+     * 3.3.5. [EduDraw.load_sound()](#edudrawload_soundfile-str---pygamemixersound)
+
+     * 3.3.6. [EduDraw.play_sound()](#edudrawplay_soundsound-pygamemixersound-loops-int--0-max_time-int--0-fade_time-int--0)
+
+     * 3.3.7. [EduDraw.remove_icon()](#edudrawremove_icon)
+
+     * 3.3.8. [EduDraw.change_icon()](#edudrawchange_iconself-image-pygamesurfacesurface)
+
+     * 3.3.9. [EduDraw.retrieve_frame()](#edudrawretrieve_frame---pygamesurfacesurface)
+
+     * 3.3.10. [EduDraw.lerp_color()](#edudrawlerp_colorcolor_1-tuple-color_2-tuple-amount-float--05---tuple)
+
+     * 3.3.11. [EduDraw.get_color_from_pos()](#edudrawget_color_from_posx-int-y-int---tuple)
+
+     * 3.3.12. [EduDraw.is_focused()](#edudrawis_focused---bool)
+
+     * 3.3.13. [EduDraw.set_mouse_visibility()](#edudrawset_mouse_visibilityvisible-bool)
+
+     3.4. [Null mode](#null-mode)
+  
 ## Installation
 
 You can install the package using PIP by typing the following command: `pip install edudraw`, and import it in your code like any other library.
 You'll need the pygame library as well, in case it doesn't get automatically installed.
 
 ## Setting up
 
@@ -795,15 +923,15 @@
     else:
         my_word += data['unicode']
 ```
 
 ![keyexample](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/ddb1a44e-77a0-46f3-bf10-fff2d76989ec)
 
 
-### EduDraw.toggle_antialising()
+### EduDraw.toggle_antialiasing()
 
 Toggles antialiasing on or off. It's off by default.
 
 Note: Antialiasing needs more processing, especially when the number of shapes and their complexity is higher. Also, antialised shapes do not take
 into account the stroke weight of the lines, and all lines are drawn with the weight of 1px.
 
 
@@ -1115,14 +1243,16 @@
     s.bezier_curve(control_points, 70)
 
     # Drawing the control points for visibility
     for point in control_points:
         s.circle(point[0], point[1], 5)
 ```
 
+![bezier_image](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/0d1d01dd-17f1-45cc-bdaa-15f9a9fa0293)
+
 
 ### EduDraw.arc_open(self, start_angle: int, stop_angle: int, x: int, y: int, width: int, height: int)
 
 Draws an open arc onto the canvas.
 
 Parameters:
 
@@ -1236,21 +1366,23 @@
 ![arcs_closed](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/4d096234-b456-454e-a1a7-5c692b561555)
 
 
 ## Other methods
 
 ### EduDraw.frame_rate(fps: int)
 
-Changes the framerate of the simulation. Must be called in ```setup()```.
-Note that in the Python version the simulation does not run as fast as the C# one, to run the simulation as fast as possible set the EduDraw.deltatime to zero.
+Changes the framerate of the simulation. To run the simulation as fast as possible use `use_max_frame_rate()` instead.
 
 Parameters:
 
 int frames: The number of FPS to set the simulation to.
 
+### EduDraw.use_max_frame_rate()
+
+Makes the simulation run as fast as possible, with the maximum frame rate being determined by computation speed.
 
 ### EduDraw.save(filename: str)
 
 Saves the current frame as an image file.
 If filename is empty, the name will be the frame count of when the photo was saved.
```

### Comparing `edudraw-1.4.0/pyproject.toml` & `edudraw-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EduDraw"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name="Murilo Luis Calvo Neves", email="muriloluiscalvoneves2004@hotmail.com" },
 ]
 description = "A simple interface for using 2D graphics in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/MuriloLCN/Edu-Draw-Python"
-"Bug Tracker" = "https://github.com/MuriloLCN/Edu-Draw-Python/issues"
+"Bug Tracker" = "https://github.com/MuriloLCN/Edu-Draw-Python/issues"
```

### Comparing `edudraw-1.4.0/PKG-INFO` & `edudraw-1.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EduDraw
-Version: 1.4.0
+Version: 1.4.1
 Summary: A simple interface for using 2D graphics in python
 Project-URL: Homepage, https://github.com/MuriloLCN/Edu-Draw-Python
 Project-URL: Bug Tracker, https://github.com/MuriloLCN/Edu-Draw-Python/issues
 Author-email: Murilo Luis Calvo Neves <muriloluiscalvoneves2004@hotmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,142 @@
 
 This project is aimed to provide an interface that allows for a simplified experience when using basic 2D graphics in the Python language. 
 
 The general design of the interface is heavily (if not all) inspired by the [P5.js](https://p5js.org/) library and the Processing library, and is intended to make simple graphical programs easy to do in the .NET environment in the shape of a Windows Forms app and/or in the Python language.
 
 The details of installation and documentation of the respective versions are below. 
 
+## Summary
+
+* 1.0. [Installation](#installation)
+
+* 2.0. [Setting up](#setting-up) 
+
+* 3.0. [Documentation](#documentation)
+
+  * 3.1. [State methods](#state-methods)  
+    
+    * 3.1.1. [EduDraw()](#edudrawwidth-int-height-int-null_mode-bool--false---edudraw)
+    
+    * 3.1.2. [EduDraw.start()](#edudrawstartsetup-draw-window_title-str)
+
+    * 3.1.3. [EduDraw.rect_mode()](#edudrawrect_modemode-str)
+  
+    * 3.1.4. [EduDraw.circle_mode()](#edudrawcircle_modemode-str)
+
+    * 3.1.5. [EduDraw.fill()](#edudrawfillcolor-tuple)
+
+    * 3.1.6. [EduDraw.no_fill()](#edudrawno_fill)
+
+    * 3.1.7. [EduDraw.font()](#edudrawfontnew_font-str-font_size-int--12-boldfalse-italicfalse-underlinefalse)
+
+    * 3.1.8. [EduDraw.font_from_instance()](#edudrawfont_from_instancenew_font-pygamefontfont)
+
+    * 3.1.9. [EduDraw.change_default_font()](#edudrawchange_default_fontnew_font-str-font_size-int--12-boldfalse-italicfalse-underlinefalse)
+
+    * 3.1.10. [EduDraw.reset_font()](#edudrawreset_font)
+
+    * 3.1.11. [EduDraw.stroke()](#edudrawstrokecolor-tuple)
+
+    * 3.1.12. [EduDraw.no_stroke()](#edudrawno_stroke)
+
+    * 3.1.13. [EduDraw.stroke_weight()](#edudrawstroke_weightnew_weight-int)
+
+    * 3.1.14. [EduDraw.push()](#edudrawpush)
+
+    * 3.1.15. [EduDraw.pop()](#edudrawpop)
+
+    * 3.1.16. [EduDraw.mouse_pos()](#edudrawmouse_pos--tuple)
+
+    * 3.1.17. [EduDraw.rotate()](#edudrawrotateangle-int)
+
+    * 3.1.18. [EduDraw.scale()](#edudrawscalescale_x-float-scale_y-float)
+
+    * 3.1.19. [EduDraw.translate()](#edudrawtranslatetranslate_x-int-translate_y-int)
+
+    * 3.1.20. [EduDraw.reset_transformations()](#edudrawreset_transformations)
+
+    * 3.1.21. [EduDraw.reset_scaling()](#edudrawreset_scaling)
+
+    * 3.1.22. [EduDraw.reset_translation()](#edudrawreset_translation)
+
+    * 3.1.23. [EduDraw.reset_rotation()](#edudrawreset_rotation)
+
+    * 3.1.24. [EduDraw.set_account_for_transformations()](#edudrawset_account_for_transformationsstate-bool)
+
+    * 3.1.25. [EduDraw.set_controls()](#edudrawset_controlskey_downnone-key_upnone-mouse_motionnone-mouse_button_upnone-mouse_button_downnone-mouse_wheelnone)
+
+    * 3.1.26. [EduDraw.toggle_antialiasing()](#edudrawtoggle_antialiasing)
+
+    * 3.1.27. [EduDraw.erase()](#edudrawerase)
+
+    * 3.1.28. [EduDraw.no_erase()](#edudrawno_erase)
+
+  * 3.2. [Drawing methods](#drawing-methods)
+
+     * 3.2.1. [EduDraw.point()](#edudrawpointx-int-y-int)
+
+     * 3.2.2. [EduDraw.text()](#edudrawtextstring-str-x-int-y-int)
+
+     * 3.2.3. [EduDraw.background()](#edudrawbackgroundcolor-tuple)
+
+     * 3.2.4. [EduDraw.circle()](#edudrawcirclex-int-y-int-radius-int)
+    
+     * 3.2.5. [EduDraw.ellipse()](#edudrawellipsex-int-y-int-width-int-height-int)
+
+     * 3.2.6. [EduDraw.line()](#edudrawlinex1-int-y1-int-x2-int-y2-int)
+
+     * 3.2.7. [EduDraw.rect()](#edudrawrectx-int-y-int-width-int-height-int)
+
+     * 3.2.8. [EduDraw.square()](#edudrawsquarex-int-y-int-side_size-int)
+
+     * 3.2.9. [EduDraw.triangle()](#edudrawtrianglex1-int-y1-int-x2-int-y2-int-x3-int-y3-int)
+
+     * 3.2.10. [EduDraw.polygon()](#edudrawpolygonpoints-list)
+
+     * 3.2.11. [EduDraw.image()](#edudrawimageimg-pygamesurfacesurface-x-int-y-int-width-int--none-height-int--none-force_transparency-bool--false)
+
+     * 3.2.12. [EduDraw.bezier_curve()](#edudrawbezier_curveself-control_points-list-num_points-int--none--none)
+
+     * 3.2.13. [EduDraw.arc_open()](#edudrawarc_openself-start_angle-int-stop_angle-int-x-int-y-int-width-int-height-int)
+
+     * 3.2.14. [EduDraw.arc_pie()](#edudrawarc_piestart_angle-int-stop_angle-int-x-int-y-int-width-int-height-int-close_edges-bool--true)
+
+     * 3.2.15. [EduDraw.arc_closed()](#edudrawarc_closedstart_angle-int-stop_angle-int-x-int-y-int-width-int-height-int-close_edges-bool--true)
+
+   * 3.3. [Other methods](#other-methods)
+
+     * 3.3.1. [EduDraw.frame_rate()](#edudrawframe_ratefps-int)
+
+     * 3.3.2. [EduDraw.use_max_frame_rate()](#edudrawuse_max_frame_rate)
+
+     * 3.3.3. [EduDraw.save()](#edudrawsavefilename-str)
+
+     * 3.3.4. [EduDraw.quit()](#edudrawquit)
+
+     * 3.3.5. [EduDraw.load_sound()](#edudrawload_soundfile-str---pygamemixersound)
+
+     * 3.3.6. [EduDraw.play_sound()](#edudrawplay_soundsound-pygamemixersound-loops-int--0-max_time-int--0-fade_time-int--0)
+
+     * 3.3.7. [EduDraw.remove_icon()](#edudrawremove_icon)
+
+     * 3.3.8. [EduDraw.change_icon()](#edudrawchange_iconself-image-pygamesurfacesurface)
+
+     * 3.3.9. [EduDraw.retrieve_frame()](#edudrawretrieve_frame---pygamesurfacesurface)
+
+     * 3.3.10. [EduDraw.lerp_color()](#edudrawlerp_colorcolor_1-tuple-color_2-tuple-amount-float--05---tuple)
+
+     * 3.3.11. [EduDraw.get_color_from_pos()](#edudrawget_color_from_posx-int-y-int---tuple)
+
+     * 3.3.12. [EduDraw.is_focused()](#edudrawis_focused---bool)
+
+     * 3.3.13. [EduDraw.set_mouse_visibility()](#edudrawset_mouse_visibilityvisible-bool)
+
+     3.4. [Null mode](#null-mode)
+  
 ## Installation
 
 You can install the package using PIP by typing the following command: `pip install edudraw`, and import it in your code like any other library.
 You'll need the pygame library as well, in case it doesn't get automatically installed.
 
 ## Setting up
 
@@ -809,15 +937,15 @@
     else:
         my_word += data['unicode']
 ```
 
 ![keyexample](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/ddb1a44e-77a0-46f3-bf10-fff2d76989ec)
 
 
-### EduDraw.toggle_antialising()
+### EduDraw.toggle_antialiasing()
 
 Toggles antialiasing on or off. It's off by default.
 
 Note: Antialiasing needs more processing, especially when the number of shapes and their complexity is higher. Also, antialised shapes do not take
 into account the stroke weight of the lines, and all lines are drawn with the weight of 1px.
 
 
@@ -1129,14 +1257,16 @@
     s.bezier_curve(control_points, 70)
 
     # Drawing the control points for visibility
     for point in control_points:
         s.circle(point[0], point[1], 5)
 ```
 
+![bezier_image](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/0d1d01dd-17f1-45cc-bdaa-15f9a9fa0293)
+
 
 ### EduDraw.arc_open(self, start_angle: int, stop_angle: int, x: int, y: int, width: int, height: int)
 
 Draws an open arc onto the canvas.
 
 Parameters:
 
@@ -1250,21 +1380,23 @@
 ![arcs_closed](https://github.com/MuriloLCN/Edu-Draw-Python/assets/88753590/4d096234-b456-454e-a1a7-5c692b561555)
 
 
 ## Other methods
 
 ### EduDraw.frame_rate(fps: int)
 
-Changes the framerate of the simulation. Must be called in ```setup()```.
-Note that in the Python version the simulation does not run as fast as the C# one, to run the simulation as fast as possible set the EduDraw.deltatime to zero.
+Changes the framerate of the simulation. To run the simulation as fast as possible use `use_max_frame_rate()` instead.
 
 Parameters:
 
 int frames: The number of FPS to set the simulation to.
 
+### EduDraw.use_max_frame_rate()
+
+Makes the simulation run as fast as possible, with the maximum frame rate being determined by computation speed.
 
 ### EduDraw.save(filename: str)
 
 Saves the current frame as an image file.
 If filename is empty, the name will be the frame count of when the photo was saved.
```

