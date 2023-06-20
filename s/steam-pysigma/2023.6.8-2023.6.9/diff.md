# Comparing `tmp/steam-pysigma-2023.6.8.tar.gz` & `tmp/steam-pysigma-2023.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.6.8.tar", last modified: Thu Jun 15 08:30:24 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.6.9.tar", last modified: Tue Jun 20 08:21:43 2023, max compression
```

## Comparing `steam-pysigma-2023.6.8.tar` & `steam-pysigma-2023.6.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.912745 steam-pysigma-2023.6.8/
--rw-rw-rw-   0        0        0     1030 2023-06-15 08:30:24.905743 steam-pysigma-2023.6.8/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 08:30:24.912745 steam-pysigma-2023.6.8/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-06-15 08:29:50.000000 steam-pysigma-2023.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.809744 steam-pysigma-2023.6.8/steam_pysigma/
--rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.8/steam_pysigma/MainSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.8/steam_pysigma/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.849743 steam-pysigma-2023.6.8/steam_pysigma/comsol/
--rw-rw-rw-   0        0        0    17523 2023-06-15 08:24:04.000000 steam-pysigma-2023.6.8/steam_pysigma/comsol/BuildComsolModel.py
--rw-rw-rw-   0        0        0    15418 2023-06-15 07:02:59.000000 steam-pysigma-2023.6.8/steam_pysigma/comsol/BuildGlobalVariables.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/comsol/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.862743 steam-pysigma-2023.6.8/steam_pysigma/data/
--rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.8/steam_pysigma/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.8/steam_pysigma/data/DataSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.867745 steam-pysigma-2023.6.8/steam_pysigma/domain_generator/
--rw-rw-rw-   0        0        0    17309 2023-06-14 13:36:18.000000 steam-pysigma-2023.6.8/steam_pysigma/domain_generator/GeometryMultipole.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/domain_generator/__init__.py
--rw-rw-rw-   0        0        0    12590 2023-06-15 08:15:06.000000 steam-pysigma-2023.6.8/steam_pysigma/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.870742 steam-pysigma-2023.6.8/steam_pysigma/parsers/
--rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.8/steam_pysigma/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.876743 steam-pysigma-2023.6.8/steam_pysigma/plotters/
--rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.6.8/steam_pysigma/plotters/PlotterPysigma.py
--rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.8/steam_pysigma/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.879743 steam-pysigma-2023.6.8/steam_pysigma/postprocessing/
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.8/steam_pysigma/postprocessing/postprocessing.py
--rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.8/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.901743 steam-pysigma-2023.6.8/steam_pysigma/utils/
--rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.8/steam_pysigma/utils/Util.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/utils/__init__.py
--rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.8/steam_pysigma/utils/make_folder_if_not_existing.py
-drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.831743 steam-pysigma-2023.6.8/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-06-15 08:30:19.000000 steam-pysigma-2023.6.8/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1005 2023-06-15 08:30:19.000000 steam-pysigma-2023.6.8/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 08:30:19.000000 steam-pysigma-2023.6.8/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      315 2023-06-15 08:30:19.000000 steam-pysigma-2023.6.8/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-15 08:30:19.000000 steam-pysigma-2023.6.8/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 08:21:43.911632 steam-pysigma-2023.6.9/
+-rw-rw-rw-   0        0        0     1030 2023-06-20 08:21:43.910631 steam-pysigma-2023.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:21:43.911632 steam-pysigma-2023.6.9/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-20 08:21:04.000000 steam-pysigma-2023.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:21:43.863631 steam-pysigma-2023.6.9/steam_pysigma/
+-rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.9/steam_pysigma/MainSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.9/steam_pysigma/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:21:43.880631 steam-pysigma-2023.6.9/steam_pysigma/comsol/
+-rw-rw-rw-   0        0        0    17582 2023-06-20 08:21:04.000000 steam-pysigma-2023.6.9/steam_pysigma/comsol/BuildComsolModel.py
+-rw-rw-rw-   0        0        0    15418 2023-06-15 07:02:59.000000 steam-pysigma-2023.6.9/steam_pysigma/comsol/BuildGlobalVariables.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.9/steam_pysigma/comsol/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:21:43.885631 steam-pysigma-2023.6.9/steam_pysigma/data/
+-rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.9/steam_pysigma/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.9/steam_pysigma/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.9/steam_pysigma/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:21:43.888631 steam-pysigma-2023.6.9/steam_pysigma/domain_generator/
+-rw-rw-rw-   0        0        0    17553 2023-06-20 08:18:52.000000 steam-pysigma-2023.6.9/steam_pysigma/domain_generator/GeometryMultipole.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.9/steam_pysigma/domain_generator/__init__.py
+-rw-rw-rw-   0        0        0    12590 2023-06-15 08:15:06.000000 steam-pysigma-2023.6.9/steam_pysigma/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:21:43.891631 steam-pysigma-2023.6.9/steam_pysigma/parsers/
+-rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.9/steam_pysigma/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.9/steam_pysigma/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:21:43.895630 steam-pysigma-2023.6.9/steam_pysigma/plotters/
+-rw-rw-rw-   0        0        0    18142 2023-06-15 15:18:36.000000 steam-pysigma-2023.6.9/steam_pysigma/plotters/PlotterPysigma.py
+-rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.9/steam_pysigma/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.9/steam_pysigma/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:21:43.898630 steam-pysigma-2023.6.9/steam_pysigma/postprocessing/
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.9/steam_pysigma/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.9/steam_pysigma/postprocessing/postprocessing.py
+-rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.9/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:21:43.906633 steam-pysigma-2023.6.9/steam_pysigma/utils/
+-rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.9/steam_pysigma/utils/Util.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.9/steam_pysigma/utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.9/steam_pysigma/utils/make_folder_if_not_existing.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:21:43.873633 steam-pysigma-2023.6.9/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-06-20 08:21:40.000000 steam-pysigma-2023.6.9/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1005 2023-06-20 08:21:40.000000 steam-pysigma-2023.6.9/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:21:40.000000 steam-pysigma-2023.6.9/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      315 2023-06-20 08:21:40.000000 steam-pysigma-2023.6.9/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-20 08:21:40.000000 steam-pysigma-2023.6.9/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.6.8/PKG-INFO` & `steam-pysigma-2023.6.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.6.8
+Version: 2023.6.9
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,SIGMA,STEAM
+Keywords: CERN,STEAM,SIGMA
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.6.8/README.md` & `steam-pysigma-2023.6.9/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.8/setup.py` & `steam-pysigma-2023.6.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.6.8",
+    version="2023.6.9",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
```

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/MainSIGMA.py` & `steam-pysigma-2023.6.9/steam_pysigma/MainSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/comsol/BuildComsolModel.py` & `steam-pysigma-2023.6.9/steam_pysigma/comsol/BuildComsolModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
 
         geom_multipole = GeometryMultipole(self.g, self.roxie_data, model_data, self.bh_curve_database, self.input_conductor_params,
                                            self.settings_dict, self.COMSOL_version)
 
         self.domains = geom_multipole.build_magnet()
         self.wedge_areas = geom_multipole.wedge_areas
+        self.iron_yoke_areas = geom_multipole.iron_yoke_areas
         #self.plot_magnet()
         self.connect_create_MPH_model(self.domains)
         self.save_files_java()
         self.save_compile_and_open_bat()
 
     def setup_config_sigma(self):
         cfg = self.g.ConfigSigma()
@@ -280,15 +281,15 @@
         fig = plt.figure(figsize=(10, 10))
         ax = plt.axes()
         ax.set_xlim(0., 0.2)
         ax.set_ylim(-.1, 0.1)
         self.show_halfTurns = True
         # p.plot_multiple_areas(ax, self.air_far_field_areas)  # air far field
         # p.plot_multiple_areas(ax, self.air_areas)  # air
-        # p.plot_multiple_areas(ax, self.iron_yoke_areas)  # iron yoke
+        plot_multiple_areas(ax, self.iron_yoke_areas)  # iron yoke
         plot_multiple_areas(ax, self.wedge_areas)  # wedges
         if self.show_halfTurns:
             for coil_nr, coil in self.roxie_data.coil.coils.items():
                 for pole_nr, pole in coil.poles.items():
                     for layer_nr, layer in pole.layers.items():
                         for winding_key, winding in layer.windings.items():
                             for block_key, block in winding.blocks.items():
```

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/comsol/BuildGlobalVariables.py` & `steam-pysigma-2023.6.9/steam_pysigma/comsol/BuildGlobalVariables.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/data/DataRoxieParser.py` & `steam-pysigma-2023.6.9/steam_pysigma/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/data/DataSIGMA.py` & `steam-pysigma-2023.6.9/steam_pysigma/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/domain_generator/GeometryMultipole.py` & `steam-pysigma-2023.6.9/steam_pysigma/domain_generator/GeometryMultipole.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
             self.cableParameters = {'cable': {}, 'strand': {}, 'Jc_fit': {}}  # dM.Conductor #self.cablesParameters
             # self.wedge_elements =
             # self.model =
             self.coil = []
             self.elements = {}
             self.coil_areas = []
             self.wedge_areas = []
+            self.iron_yoke_areas = []
 
 
     def build_magnet(self):
         """
         This function builds a magnet and creates the different domains.
 
         :return: None
@@ -117,14 +118,16 @@
         i = 0
         # while conductor != self.input_conductor_params.Model_Data_GS.conductors[conductor]:
         # i += 1
         for entry in self.input_conductor_params.Model_Data_GS.conductors[conductor]:
             if entry[0] == 'cable' or entry[0] == 'strand' or entry[0] == 'Jc_fit':
                 for key in entry[1]:
                     self.cableParameters[entry[0]][key[0]] = key[1] if key[1] else 0.
+        if self.cableParameters['cable']['type'] == "Ribbon":
+            raise ValueError("SIGMA does not support Ribbon cables, please enter another magnet.")
         self.g.cable.setwInsulNarrow(self.cableParameters['cable']['th_insulation_along_height'])
         self.g.cable.setwInsulWide(self.cableParameters['cable']['th_insulation_along_width'])
         self.g.cable.setRc(self.cableParameters['cable']['Rc'])
         self.g.cable.setRa(self.cableParameters['cable']['Ra'])
         self.g.cable.setwBare(self.cableParameters['cable']['bare_cable_width'])
         self.g.cable.sethInBare(self.cableParameters['cable']['bare_cable_height_low'])
         self.g.cable.sethOutBare(self.cableParameters['cable']['bare_cable_height_high'])
@@ -287,14 +290,15 @@
         for i in hyperAreasCOMSOL:
             arg = []  # elements
             for j, ar in enumerate(hyperAreasCOMSOL[i]):
                 arg.append(self.g.Element(f"IY{iron.hyper_areas[i].material[2:]}_{i}_El{j}", ar))
 
             self.elements[i] = self.a.create_element_array(self.g.gateway, tuple(arg))
 
+            self.iron_yoke_areas += [ar]
     def get_all_domains(self):
         """
         This function saves a Java file to be used in COMSOL simulation software.
 
         :return: None
         """
         domains = [self.g.AirFarFieldDomain("AFF", self.g.MatDatabase.MAT_AIR, self.air_far_field)]
```

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/helpers.py` & `steam-pysigma-2023.6.9/steam_pysigma/helpers.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/parsers/ParserRoxie.py` & `steam-pysigma-2023.6.9/steam_pysigma/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/plotters/PlotterPysigma.py` & `steam-pysigma-2023.6.9/steam_pysigma/plotters/PlotterPysigma.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,29 +40,44 @@
     for hl in hls:
         last_dot_index = hl.toString().rfind('.')
         at_index = hl.toString().find('@')
         class_name = hl.toString()[last_dot_index + 1:at_index]
         if class_name == 'Line':
             points.append([hl.getKp1().getX(), hl.getKp1().getY()])
             points.append([hl.getKp2().getX(), hl.getKp2().getY()])
+            ax.add_line(lines.Line2D([hl.getKp1().getX(), hl.getKp2().getX()], [hl.getKp1().getY(), hl.getKp2().getY()], color=color))
         elif class_name == 'Arc':
             start_angle = np.arctan2(hl.getKp1().getY() - hl.getKpc().getY(),
                                      hl.getKp1().getX() - hl.getKpc().getX()) * 180 / np.pi
             end_angle = start_angle + hl.getDTheta() * 180 / np.pi
             r = np.sqrt((hl.getKp1().getY() - hl.getKpc().getY()) ** 2 + (hl.getKp1().getX() - hl.getKpc().getX()) ** 2)
             ax.add_patch(patches.Arc([hl.getKpc().getX(), hl.getKpc().getY()], 2 * r, 2 * r, 0,
                                      min(start_angle, end_angle), max(start_angle, end_angle), color=color))
         elif class_name == 'Circumference':
             r = hl.getRadius()
             ax.add_patch(patches.Arc([hl.getCenter().getX(), hl.getCenter().getY()], 2 * r, 2 * r, 0, 0, 360))
+
+        elif class_name == 'EllipticArc':
+            pt1 = (hl.getKp1().getX(), hl.getKp1().getY())
+            ptc = (hl.getKpc().getX(), hl.getKpc().getY())
+            dTheta = hl.getDTheta()*180/np.pi
+            a, b = hl.getA(), hl.getB()
+
+            start_angle = float(np.degrees(np.arctan2(pt1[1] - ptc[1], pt1[0] - ptc[0])))
+
+            arc = patches.Arc(ptc, 2 * a, 2 * b, angle=0, theta1=start_angle, theta2=start_angle + dTheta,color=color )
+
+            ax.add_patch(arc)
         else:
             raise ValueError('Not supported Hyperline object!')
+    # try:
+    #     ax.add_line(lines.Line2D([points[0][0], points[3][0]], [points[0][1], points[3][1]], color=color))
+    #     ax.add_line(lines.Line2D([points[1][0], points[2][0]], [points[1][1], points[2][1]], color=color))
+    # except: print("couldn't plot line")
 
-    ax.add_line(lines.Line2D([points[0][0], points[3][0]], [points[0][1], points[3][1]], color=color))
-    ax.add_line(lines.Line2D([points[1][0], points[2][0]], [points[1][1], points[2][1]], color=color))
 
 def write_result_summary(df, n1, n2):
     with open("error_summary.txt", "a") as myfile:
         mean_Bmod_error = (df["Bmod_error"]).mean() * 1000
         abs_mean_Bmod_error = abs(df["Bmod_error"]).mean() * 1000
         std_Bmod_error = (df["Bmod_error"]).std() * 1000
         max_Bmod_error = abs(df["Bmod_error"]).max() * 1000
```

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/plotters/PlotterRoxie.py` & `steam-pysigma-2023.6.9/steam_pysigma/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/postprocessing/postprocessing.py` & `steam-pysigma-2023.6.9/steam_pysigma/postprocessing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/pysigma.py` & `steam-pysigma-2023.6.9/steam_pysigma/pysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.8/steam_pysigma/utils/Util.py` & `steam-pysigma-2023.6.9/steam_pysigma/utils/Util.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.8/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.6.9/steam_pysigma.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.6.8
+Version: 2023.6.9
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,SIGMA,STEAM
+Keywords: CERN,STEAM,SIGMA
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.6.8/steam_pysigma.egg-info/SOURCES.txt` & `steam-pysigma-2023.6.9/steam_pysigma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

