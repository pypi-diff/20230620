# Comparing `tmp/vector2dggs-0.5.0.tar.gz` & `tmp/vector2dggs-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector2dggs-0.5.0.tar", max compression
+gzip compressed data, was "vector2dggs-0.5.1.tar", max compression
```

## Comparing `vector2dggs-0.5.0.tar` & `vector2dggs-0.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8360 2023-06-09 00:47:52.784100 vector2dggs-0.5.0/README.md
--rw-r--r--   0        0        0     1092 2023-06-09 00:47:52.792101 vector2dggs-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       27 2023-06-09 00:47:52.792101 vector2dggs-0.5.0/vector2dggs/__init__.py
--rw-r--r--   0        0        0      599 2023-05-29 05:44:55.043652 vector2dggs-0.5.0/vector2dggs/cli.py
--rw-r--r--   0        0        0    12629 2023-06-09 00:47:52.792101 vector2dggs-0.5.0/vector2dggs/h3.py
--rw-r--r--   0        0        0     3173 2023-05-29 05:44:55.043652 vector2dggs-0.5.0/vector2dggs/katana.py
--rw-r--r--   0        0        0     9794 1970-01-01 00:00:00.000000 vector2dggs-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     8360 2023-06-20 08:17:49.493916 vector2dggs-0.5.1/README.md
+-rw-r--r--   0        0        0     1092 2023-06-20 08:17:39.335792 vector2dggs-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-06-20 08:17:23.697601 vector2dggs-0.5.1/vector2dggs/__init__.py
+-rw-r--r--   0        0        0      599 2023-06-20 07:50:37.408069 vector2dggs-0.5.1/vector2dggs/cli.py
+-rw-r--r--   0        0        0    12726 2023-06-20 08:17:11.953457 vector2dggs-0.5.1/vector2dggs/h3.py
+-rw-r--r--   0        0        0     3173 2023-06-20 07:50:37.408069 vector2dggs-0.5.1/vector2dggs/katana.py
+-rw-r--r--   0        0        0     9794 1970-01-01 00:00:00.000000 vector2dggs-0.5.1/PKG-INFO
```

### Comparing `vector2dggs-0.5.0/README.md` & `vector2dggs-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -153,17 +153,17 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.5.0},
+  version={0.5.1},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.5.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.5.1) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `vector2dggs-0.5.0/pyproject.toml` & `vector2dggs-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vector2dggs"
-version = "0.5.0"
+version = "0.5.1"
 description = "CLI DGGS indexer for vector geospatial data"
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/vector2dggs"
 keywords = ["dggs", "vector", "h3", "cli"]
```

### Comparing `vector2dggs-0.5.0/vector2dggs/cli.py` & `vector2dggs-0.5.1/vector2dggs/cli.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.5.0/vector2dggs/h3.py` & `vector2dggs-0.5.1/vector2dggs/h3.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,20 +183,23 @@
     with tqdm(total=df.shape[0]) as pbar:
         for index, row in df.iterrows():
             df.loc[index, "geometry"] = GeometryCollection(
                 katana.katana(row.geometry, cut_threshold)
             )
             pbar.update(1)
 
-    LOGGER.info("Preparing for spatial partitioning...")
+    LOGGER.info("Exploding geometry collections and multipolygons")
     df = (
         df.to_crs(4326)
         .explode(index_parts=False)  # Explode from GeometryCollection
         .explode(index_parts=False)  # Explode multipolygons to polygons
-        .drop(df[(df.geometry.is_empty|df.geometry.isna())].index)
+    ).reset_index()
+    LOGGER.info("Dropping empty or null geometries")
+    df = (
+        df.drop(df[(df.geometry.is_empty|df.geometry.isna())].index)
         .reset_index()
     )
 
     ddf = dgpd.from_geopandas(df, chunksize=max(1, chunksize), sort=True)
 
     LOGGER.info("Spatially sorting and partitioning (%s)", spatial_sorting)
     ddf = ddf.spatial_shuffle(by=spatial_sorting)
```

### Comparing `vector2dggs-0.5.0/vector2dggs/katana.py` & `vector2dggs-0.5.1/vector2dggs/katana.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.5.0/PKG-INFO` & `vector2dggs-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector2dggs
-Version: 0.5.0
+Version: 0.5.1
 Summary: CLI DGGS indexer for vector geospatial data
 Home-page: https://github.com/manaakiwhenua/vector2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,vector,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -188,18 +188,18 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.5.0},
+  version={0.5.1},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.5.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.5.1) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

