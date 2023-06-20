# Comparing `tmp/pygus-2.0.3.tar.gz` & `tmp/pygus-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygus-2.0.3.tar", max compression
+gzip compressed data, was "pygus-2.0.4.tar", max compression
```

## Comparing `pygus-2.0.3.tar` & `pygus-2.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2022-10-24 14:24:35.788368 pygus-2.0.3/LICENSE
--rw-r--r--   0        0        0     1541 2023-04-19 16:37:11.282155 pygus-2.0.3/README-pypi.md
--rw-r--r--   0        0        0      161 2023-06-14 13:00:54.096939 pygus-2.0.3/pygus/__init__.py
--rw-r--r--   0        0        0      183 2023-06-14 13:00:54.097675 pygus-2.0.3/pygus/gus/__init__.py
--rw-r--r--   0        0        0    27311 2023-06-07 17:14:01.717670 pygus-2.0.3/pygus/gus/agents.py
--rw-r--r--   0        0        0     7484 2023-06-07 17:14:01.718672 pygus-2.0.3/pygus/gus/allometrics.py
--rw-r--r--   0        0        0     3069 2023-04-26 08:20:10.279558 pygus-2.0.3/pygus/gus/inputs/allometrics.json
--rw-r--r--   0        0        0  9874219 2023-05-23 13:42:14.779205 pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees.csv
--rw-r--r--   0        0        0    39187 2023-05-23 14:51:09.274748 pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_1000.csv
--rw-r--r--   0        0        0  9874219 2023-05-30 13:48:12.428717 pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_100000.csv
--rw-r--r--   0        0        0     7679 2023-05-29 16:04:17.254756 pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_200.csv
--rw-r--r--   0        0        0   793770 2023-05-30 13:23:28.448382 pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_20000.csv
--rw-r--r--   0        0        0       95 2023-05-22 14:31:01.986378 pygus-2.0.3/pygus/gus/inputs/scenario.json
--rw-r--r--   0        0        0      264 2023-04-26 08:20:10.279976 pygus-2.0.3/pygus/gus/inputs/site.json
--rw-r--r--   0        0        0     5932 2023-04-26 08:20:10.280228 pygus-2.0.3/pygus/gus/inputs/trees.csv
--rw-r--r--   0        0        0    16148 2023-06-14 13:17:00.376677 pygus-2.0.3/pygus/gus/models.py
--rw-r--r--   0        0        0  1566870 2023-04-26 08:20:10.288567 pygus-2.0.3/pygus/gus/outputs/trees_yearly.json
--rw-r--r--   0        0        0     4210 2023-06-14 13:00:54.098664 pygus-2.0.3/pygus/gus/utilities.py
--rw-r--r--   0        0        0     1701 2023-04-26 08:20:10.289503 pygus-2.0.3/pygus/gus/weather.py
--rw-r--r--   0        0        0       58 2023-04-26 08:20:10.290114 pygus-2.0.3/pygus/impacts/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-26 08:20:10.290632 pygus-2.0.3/pygus/impacts/carbon.py
--rw-r--r--   0        0        0    32960 2023-04-26 08:20:10.291410 pygus-2.0.3/pygus/impacts/water.py
--rw-r--r--   0        0        0     1501 2023-06-14 13:40:01.257695 pygus-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 pygus-2.0.3/setup.py
--rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 pygus-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-24 14:24:35.788368 pygus-2.0.4/LICENSE
+-rw-r--r--   0        0        0     1541 2023-04-19 16:37:11.282155 pygus-2.0.4/README-pypi.md
+-rw-r--r--   0        0        0      185 2023-06-20 14:39:46.120957 pygus-2.0.4/pygus/__init__.py
+-rw-r--r--   0        0        0      217 2023-06-20 14:39:46.121591 pygus-2.0.4/pygus/gus/__init__.py
+-rw-r--r--   0        0        0    27333 2023-06-20 14:39:46.122395 pygus-2.0.4/pygus/gus/agents.py
+-rw-r--r--   0        0        0     7484 2023-06-07 17:14:01.718672 pygus-2.0.4/pygus/gus/allometrics.py
+-rw-r--r--   0        0        0     3069 2023-04-26 08:20:10.279558 pygus-2.0.4/pygus/gus/inputs/allometrics.json
+-rw-r--r--   0        0        0  9874219 2023-05-23 13:42:14.779205 pygus-2.0.4/pygus/gus/inputs/amsterdam_all_trees.csv
+-rw-r--r--   0        0        0    39187 2023-05-23 14:51:09.274748 pygus-2.0.4/pygus/gus/inputs/amsterdam_all_trees_1000.csv
+-rw-r--r--   0        0        0  9874219 2023-05-30 13:48:12.428717 pygus-2.0.4/pygus/gus/inputs/amsterdam_all_trees_100000.csv
+-rw-r--r--   0        0        0     7679 2023-05-29 16:04:17.254756 pygus-2.0.4/pygus/gus/inputs/amsterdam_all_trees_200.csv
+-rw-r--r--   0        0        0   793770 2023-05-30 13:23:28.448382 pygus-2.0.4/pygus/gus/inputs/amsterdam_all_trees_20000.csv
+-rw-r--r--   0        0        0       95 2023-05-22 14:31:01.986378 pygus-2.0.4/pygus/gus/inputs/scenario.json
+-rw-r--r--   0        0        0      264 2023-04-26 08:20:10.279976 pygus-2.0.4/pygus/gus/inputs/site.json
+-rw-r--r--   0        0        0     5932 2023-04-26 08:20:10.280228 pygus-2.0.4/pygus/gus/inputs/trees.csv
+-rw-r--r--   0        0        0    16153 2023-06-20 14:39:46.124037 pygus-2.0.4/pygus/gus/models.py
+-rw-r--r--   0        0        0  1566870 2023-04-26 08:20:10.288567 pygus-2.0.4/pygus/gus/outputs/trees_yearly.json
+-rw-r--r--   0        0        0     4959 2023-06-20 14:39:46.124655 pygus-2.0.4/pygus/gus/utilities.py
+-rw-r--r--   0        0        0     1701 2023-04-26 08:20:10.289503 pygus-2.0.4/pygus/gus/weather.py
+-rw-r--r--   0        0        0       58 2023-04-26 08:20:10.290114 pygus-2.0.4/pygus/impacts/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-26 08:20:10.290632 pygus-2.0.4/pygus/impacts/carbon.py
+-rw-r--r--   0        0        0    32960 2023-04-26 08:20:10.291410 pygus-2.0.4/pygus/impacts/water.py
+-rw-r--r--   0        0        0     1523 2023-06-20 14:40:08.301261 pygus-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 pygus-2.0.4/setup.py
+-rw-r--r--   0        0        0     3264 1970-01-01 00:00:00.000000 pygus-2.0.4/PKG-INFO
```

### Comparing `pygus-2.0.3/LICENSE` & `pygus-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/README-pypi.md` & `pygus-2.0.4/README-pypi.md`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pygus/gus/agents.py` & `pygus-2.0.4/pygus/gus/agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,28 +124,28 @@
         elif condition:
             self.condition = condition
             self.dieback = self._estimate_dieback(condition)
         else:
             self.dieback = np.random.uniform(0, 0.1)
             self.condition = self._get_condition_class(self.dieback)
 
-        self.diameter_growth = model.species.get_diameter_growth(species)
+        self.diameter_growth = self.model.species.get_diameter_growth(species)
         # Slow, moderate and fast growing species respectively.
         # c(0.23, 0.33, 0.43) in inch/yr Source: https://database.itreetools.org/#/splash
         # Converted into cm.
 
         # Default crown light exposure based on site types.
         self.cle = Tree.sun_exposure_rates[self.model.site_type]
         # Crown light exposure to sunlight (CLE).
         # CLE <- c(0.44, 0.56, 1)
         # (1) Forest conditions with a closed, or nearly closed canopy,
         # (2) Park conditions
         # (3) Open-grown conditions.
 
-        self.average_height_at_maturity = model.species.get_height_at_maturity(
+        self.average_height_at_maturity = self.model.species.get_height_at_maturity(
             self.species
         )
         # Avg height at maturity for the given species.
 
         self.biomass = self.compute_biomass()  # In Kg
         self.carbon_storage = Tree.carbon_coeff * self.biomass  # In Kg
 
@@ -157,18 +157,18 @@
 
         self.mulched = 0
         self.decomposing_root = 0
         self.decomposing_trunk = 0
         self.immediate_release = 0
         self.death_acc = False
 
-        if model.maintenance_scope == 0:
+        if self.model.maintenance_scope == 0:
             self.expected_care = 0
-        elif model.maintenance_scope == 1:
-            self.expected_care = 0.3
+        elif self.model.maintenance_scope == 1:
+            self.expected_care = 0.5
         else:
             self.expected_care = 1.0
 
     def step(self):
         """State transitions of a given Tree agent.
 
         Args:
@@ -447,20 +447,20 @@
         #  1.96% for good-excellent and DBH < 3inches
         #  1.46% for good-excellent and DBH > 3inches
         #  3.32% for fair condition
         #  8.86% for poor condition
         #  13.08% for critical condition
         #  50% for dying condition
         risk = np.random.uniform(0, 1)
-        if self.model.maintenance_scope < 1:
+        if self.model.maintenance_scope == 0:
             dr = 5
-        elif self.model.maintenance_scope > 1:
-            dr = 1
-        else:
+        elif self.model.maintenance_scope == 1:
             dr = 4
+        else:
+            dr = 1
 
         if self.dieback >= 1:
             register_death()
         elif self.condition == "dead":
             register_death()
         elif (
             self.condition in ("good", "excellent")
```

### Comparing `pygus-2.0.3/pygus/gus/allometrics.py` & `pygus-2.0.4/pygus/gus/allometrics.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pygus/gus/inputs/allometrics.json` & `pygus-2.0.4/pygus/gus/inputs/allometrics.json`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees.csv` & `pygus-2.0.4/pygus/gus/inputs/amsterdam_all_trees.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_1000.csv` & `pygus-2.0.4/pygus/gus/inputs/amsterdam_all_trees_1000.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_100000.csv` & `pygus-2.0.4/pygus/gus/inputs/amsterdam_all_trees_100000.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_200.csv` & `pygus-2.0.4/pygus/gus/inputs/amsterdam_all_trees_200.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pygus/gus/inputs/amsterdam_all_trees_20000.csv` & `pygus-2.0.4/pygus/gus/inputs/amsterdam_all_trees_20000.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pygus/gus/inputs/trees.csv` & `pygus-2.0.4/pygus/gus/inputs/trees.csv`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pygus/gus/models.py` & `pygus-2.0.4/pygus/gus/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 # Importing needed GUS objects
 from .agents import Tree
 from .allometrics import Species
 from .weather import WeatherSim
 
        
 class WeatherConfig:
-    def __init__(self, mean_growth_rate: int = 153, growth_rate_var: int = 7):
-        self.mean_growth_rate = mean_growth_rate
+    
+    def __init__(self, mean_growth_days: int = 153, growth_rate_var: int = 7):
+        self.mean_growth_rate = mean_growth_days
         self.growth_rate_var = growth_rate_var
 
 class SiteConfig:
     """A class to hold site configuration parameters."""
 
     def __init__(self, total_m2: int, impervious_m2: int, pervious_m2: int, weather: Union[Dict, WeatherConfig], tree_density_per_ha: int = None, site_type: str = "park"):
         self.total_m2 = total_m2
```

### Comparing `pygus-2.0.3/pygus/gus/outputs/trees_yearly.json` & `pygus-2.0.4/pygus/gus/outputs/trees_yearly.json`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pygus/gus/utilities.py` & `pygus-2.0.4/pygus/gus/utilities.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,37 @@
             lambda x: x.condition not in ["dead", "replaced"], cell_content
         )
         filtered = filter(predicate, [eval("a.{}".format(var)) for a in cell_content])
         raster[x][y] = reduce(probe, filtered, init)
     return raster
 
 
+def latlng_array_to_xy(population_df, lat_column = "lat", lng_column = "lng"):
+    """A general purpose function that translates lat, lng data to x,y pos.
+
+    Args:
+            lat_array: (:obj:`numpy.ndarray`): array of latitudes.
+            lng_array: (:obj:`numpy.ndarray`): array of longitudes.
+
+    Returns:
+            (:obj:numpy.ndarray`): array of x,y positions.
+        Note:
+            None
+    """
+    lat = population_df[lat_column].to_numpy()
+    lng = population_df[lng_column].to_numpy()
+    xpos, ypos = utm.from_latlon(lat, lng)
+    population_df['xpos'] = xpos
+    population_df['ypos'] = ypos
+
+    #remove lat and lng
+    population_df = population_df.drop([lat_column, lng_column], axis=1)
+    return population_df
+    
+    
 def latlng_to_xy(row):
     """A general purpose function that translates lat, lng data to x,y pos.
 
     Args:
             row: (pandas.DataFrame.row): a Pandas DataFrame row.
 
     Returns:
```

### Comparing `pygus-2.0.3/pygus/gus/weather.py` & `pygus-2.0.4/pygus/gus/weather.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pygus/impacts/carbon.py` & `pygus-2.0.4/pygus/impacts/carbon.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pygus/impacts/water.py` & `pygus-2.0.4/pygus/impacts/water.py`

 * *Files identical despite different names*

### Comparing `pygus-2.0.3/pyproject.toml` & `pygus-2.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyGUS"
-version = "2.0.3"
+version = "2.0.4"
 description = "Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis."
 authors = ["Bulent Ozel <bulent@lucidminds.ai>"] 
 maintainers = [
     "Oguzhan Yayla <oguzhan@lucidminds.ai>", 
     "Marko Petrovic <marko@lucidminds.ai>", 
     "Axel Nilsson <axel@darkmatterlabs.org>"
 ]
@@ -40,14 +40,15 @@
 seaborn = "^0.11.2"
 portray = "^1.7.0"
 termcolor = "^2.1.1"
 utm = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
+ipykernel = "^6.23.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.portray]
 modules = ["pygus"]
```

### Comparing `pygus-2.0.3/setup.py` & `pygus-2.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'pytest>=7.1.2,<8.0.0',
  'seaborn>=0.11.2,<0.12.0',
  'termcolor>=2.1.1,<3.0.0',
  'utm>=0.7.0,<0.8.0']
 
 setup_kwargs = {
     'name': 'pygus',
-    'version': '2.0.3',
+    'version': '2.0.4',
     'description': 'Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.',
     'long_description': '[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Versions](https://img.shields.io/pypi/pyversions/pygus)]()\n\n\n\n# gus\n![GUS-IMAGE](https://miro.medium.com/max/1400/1*fMM7rnq1RJCh-nFBGLUvyA.png)\n\nGreen Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.\n\n## Getting Started\nVisit the GUS [website documentation](https://lucidmindsai.github.io/gus/) for help with installing GUS, code documentation, and a [basic tutorial](https://github.com/lucidmindsai/gus/blob/main/notebooks/Tutorial.ipynb) to get you started. \n\n## Install from PyPi\nWe publish GUS as `pyGus` package in PyPi. Dependencies can be found in the .toml file on the GUS GitHub page. Even though installation with Poetry is possible, the most stable installation can be done via pip.\n\n```\n$ pip install pygus\n```\n\nFor further instructions and code documentation, visit [GUS Code Documentation](https://lucidmindsai.github.io/gus/)\n\n### Who maintains GUS?\nThe GUS is currently developed and maintained by [Lucidminds](https://lucidminds.ai/) and [Dark Matter Labs](https://darkmatterlabs.org/) members as part of their joint project [TreesAI](https://treesasinfrastructure.com/#/).\n\n### Notes\n* The GUS is open for PRs.\n* PRs will be reviewed by the current maintainers of the project.\n* Extensive development guidelines will be provided soon.\n* To report bugs, fixes, and questions, please use the [GitHub issues](https://github.com/lucidmindsai/gus/issues).',
     'author': 'Bulent Ozel',
     'author_email': 'bulent@lucidminds.ai',
     'maintainer': 'Oguzhan Yayla',
     'maintainer_email': 'oguzhan@lucidminds.ai',
     'url': 'https://github.com/lucidmindsai/gus',
```

### Comparing `pygus-2.0.3/PKG-INFO` & `pygus-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygus
-Version: 2.0.3
+Version: 2.0.4
 Summary: Green Urban Scenarios - A digital twin representation, simulation of urban forests and their impact analysis.
 Home-page: https://github.com/lucidmindsai/gus
 License: Apache-2.0
 Author: Bulent Ozel
 Author-email: bulent@lucidminds.ai
 Maintainer: Oguzhan Yayla
 Maintainer-email: oguzhan@lucidminds.ai
```

