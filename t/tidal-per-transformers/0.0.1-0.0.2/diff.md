# Comparing `tmp/tidal_per_transformers-0.0.1.tar.gz` & `tmp/tidal_per_transformers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidal_per_transformers-0.0.1.tar", max compression
+gzip compressed data, was "tidal_per_transformers-0.0.2.tar", max compression
```

## Comparing `tidal_per_transformers-0.0.1.tar` & `tidal_per_transformers-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11357 2023-05-26 12:16:06.160846 tidal_per_transformers-0.0.1/LICENSE
--rw-r--r--   0        0        0      736 2023-06-08 12:26:06.996682 tidal_per_transformers-0.0.1/README.md
--rw-r--r--   0        0        0     1365 2023-06-20 11:07:56.183399 tidal_per_transformers-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2623 2023-06-02 12:05:26.448641 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/__init__.py
--rw-r--r--   0        0        0     1575 2023-05-26 12:22:52.886433 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/aggregate_transformer.py
--rw-r--r--   0        0        0     1974 2023-05-26 13:07:28.329225 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/artist_compound_transformer.py
--rw-r--r--   0        0        0     3327 2023-05-26 12:45:25.059286 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/artist_filter_transformer.py
--rw-r--r--   0        0        0     2858 2023-05-26 12:45:25.225615 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/artists_struct_filter_transformer.py
--rw-r--r--   0        0        0      801 2023-05-26 12:45:25.244156 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/blazingtext_input_format_transformer.py
--rw-r--r--   0        0        0      972 2023-05-26 12:45:25.088885 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/broadcast_array_intersect_transformer.py
--rw-r--r--   0        0        0     1714 2023-05-26 12:45:25.103619 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/clean_text_transformer.py
--rw-r--r--   0        0        0     1148 2023-05-26 12:45:25.039032 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/collect_ranked_list_transformer.py
--rw-r--r--   0        0        0     1864 2023-05-26 12:45:25.032669 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/collect_ranked_map_transformer.py
--rw-r--r--   0        0        0      889 2023-05-26 12:45:25.281067 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/deduplicate_sequence_transformer.py
--rw-r--r--   0        0        0     1240 2023-05-26 12:45:25.156913 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/distinct_sequence_transformer.py
--rw-r--r--   0        0        0      323 2023-05-26 12:45:25.241453 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/distinct_transformer.py
--rw-r--r--   0        0        0      451 2023-03-03 13:05:06.766654 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/drop_columns_transformer.py
--rw-r--r--   0        0        0      479 2023-05-26 12:45:25.130504 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/drop_duplicates_transformer.py
--rw-r--r--   0        0        0     2264 2023-05-26 12:45:25.266270 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/filter_infrequent_seq_transformer.py
--rw-r--r--   0        0        0      790 2023-05-26 12:45:25.071771 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/filter_infrequent_transformer.py
--rw-r--r--   0        0        0      683 2023-05-26 12:45:25.187064 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/flatten_struct_transformer.py
--rw-r--r--   0        0        0      661 2023-05-26 12:45:25.124454 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/join_transformer.py
--rw-r--r--   0        0        0      830 2023-05-26 13:07:28.499861 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/loggable_transformer.py
--rw-r--r--   0        0        0     1496 2023-05-26 12:45:25.198693 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/main_artist_compound_mapping_transformer.py
--rw-r--r--   0        0        0     1361 2023-05-26 12:45:25.271528 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/minmax_scaling_transformer.py
--rw-r--r--   0        0        0     1657 2023-05-26 12:45:25.151976 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/multiple_compound_mapping.py
--rw-r--r--   0        0        0      342 2023-05-26 12:45:25.108404 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/order_by_transformer.py
--rw-r--r--   0        0        0      809 2023-05-26 12:45:25.047224 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/participating_artist_transformer.py
--rw-r--r--   0        0        0     1020 2023-05-26 12:45:25.134461 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/pivot_transformer.py
--rw-r--r--   0        0        0     1241 2023-05-26 12:45:25.119654 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/playlist_coherence_transformer.py
--rw-r--r--   0        0        0      430 2023-05-26 12:45:25.117516 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/replace_null_values_transformer.py
--rw-r--r--   0        0        0      321 2023-05-26 12:45:25.098192 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/select_transformer.py
--rw-r--r--   0        0        0     4773 2023-05-26 12:45:25.285047 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/sequence_content_filter_transformer.py
--rw-r--r--   0        0        0     2473 2023-05-26 12:45:25.101119 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/single_artist_filter_transformer.py
--rw-r--r--   0        0        0     2721 2023-05-26 13:07:28.527893 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/stack_transformer.py
--rw-r--r--   0        0        0     1175 2023-05-26 12:45:25.041733 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/top_items_dithering_transformer.py
--rw-r--r--   0        0        0     1307 2023-05-26 12:45:25.073969 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/top_items_transformer.py
--rw-r--r--   0        0        0     1488 2023-05-26 12:45:25.229498 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/track_group_availability_by_country_transformer.py
--rw-r--r--   0        0        0     1297 2023-05-26 13:07:28.409016 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/track_group_availability_transformer.py
--rw-r--r--   0        0        0     4399 2023-05-26 12:45:25.221232 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/track_group_filter_transformer.py
--rw-r--r--   0        0        0      355 2023-05-26 12:45:25.115358 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/union_transformer.py
--rw-r--r--   0        0        0     1635 2023-05-26 12:45:25.138086 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/voiceness_filter_transformer.py
--rw-r--r--   0        0        0      780 2023-05-26 12:45:25.091990 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/where_transformer.py
--rw-r--r--   0        0        0      544 2023-05-26 12:45:25.277219 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/with_column_renamed_transfomer.py
--rw-r--r--   0        0        0      516 2023-05-26 12:45:25.238213 tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/with_column_transfomer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:23:49.409343 tidal_per_transformers-0.0.1/tidal_per_transformers/utils/__init__.py
--rw-r--r--   0        0        0      545 2023-05-26 13:07:28.342392 tidal_per_transformers-0.0.1/tidal_per_transformers/utils/class_utils.py
--rw-r--r--   0        0        0     7789 2023-05-26 12:27:47.437361 tidal_per_transformers-0.0.1/tidal_per_transformers/utils/constants.py
--rw-r--r--   0        0        0     1917 2021-11-09 07:16:08.661545 tidal_per_transformers-0.0.1/tidal_per_transformers/utils/dither_utils.py
--rw-r--r--   0        0        0      881 2023-05-26 13:07:28.479609 tidal_per_transformers-0.0.1/tidal_per_transformers/utils/schemas.py
--rw-r--r--   0        0        0     1233 2023-02-22 15:09:27.044718 tidal_per_transformers-0.0.1/tidal_per_transformers/utils/spark_utils.py
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 tidal_per_transformers-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-26 12:16:06.160846 tidal_per_transformers-0.0.2/LICENSE
+-rw-r--r--   0        0        0      736 2023-06-08 12:26:06.996682 tidal_per_transformers-0.0.2/README.md
+-rw-r--r--   0        0        0     1125 2023-06-20 11:37:30.309624 tidal_per_transformers-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2623 2023-06-02 12:05:26.448641 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/__init__.py
+-rw-r--r--   0        0        0     1575 2023-05-26 12:22:52.886433 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/aggregate_transformer.py
+-rw-r--r--   0        0        0     1974 2023-05-26 13:07:28.329225 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/artist_compound_transformer.py
+-rw-r--r--   0        0        0     3327 2023-05-26 12:45:25.059286 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/artist_filter_transformer.py
+-rw-r--r--   0        0        0     2858 2023-05-26 12:45:25.225615 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/artists_struct_filter_transformer.py
+-rw-r--r--   0        0        0      801 2023-05-26 12:45:25.244156 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/blazingtext_input_format_transformer.py
+-rw-r--r--   0        0        0      972 2023-05-26 12:45:25.088885 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/broadcast_array_intersect_transformer.py
+-rw-r--r--   0        0        0     1714 2023-05-26 12:45:25.103619 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/clean_text_transformer.py
+-rw-r--r--   0        0        0     1148 2023-05-26 12:45:25.039032 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/collect_ranked_list_transformer.py
+-rw-r--r--   0        0        0     1864 2023-05-26 12:45:25.032669 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/collect_ranked_map_transformer.py
+-rw-r--r--   0        0        0      889 2023-05-26 12:45:25.281067 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/deduplicate_sequence_transformer.py
+-rw-r--r--   0        0        0     1240 2023-05-26 12:45:25.156913 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/distinct_sequence_transformer.py
+-rw-r--r--   0        0        0      323 2023-05-26 12:45:25.241453 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/distinct_transformer.py
+-rw-r--r--   0        0        0      451 2023-03-03 13:05:06.766654 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/drop_columns_transformer.py
+-rw-r--r--   0        0        0      479 2023-05-26 12:45:25.130504 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/drop_duplicates_transformer.py
+-rw-r--r--   0        0        0     2264 2023-05-26 12:45:25.266270 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/filter_infrequent_seq_transformer.py
+-rw-r--r--   0        0        0      790 2023-05-26 12:45:25.071771 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/filter_infrequent_transformer.py
+-rw-r--r--   0        0        0      683 2023-05-26 12:45:25.187064 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/flatten_struct_transformer.py
+-rw-r--r--   0        0        0      661 2023-05-26 12:45:25.124454 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/join_transformer.py
+-rw-r--r--   0        0        0      830 2023-05-26 13:07:28.499861 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/loggable_transformer.py
+-rw-r--r--   0        0        0     1496 2023-05-26 12:45:25.198693 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/main_artist_compound_mapping_transformer.py
+-rw-r--r--   0        0        0     1361 2023-05-26 12:45:25.271528 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/minmax_scaling_transformer.py
+-rw-r--r--   0        0        0     1657 2023-05-26 12:45:25.151976 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/multiple_compound_mapping.py
+-rw-r--r--   0        0        0      342 2023-05-26 12:45:25.108404 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/order_by_transformer.py
+-rw-r--r--   0        0        0      809 2023-05-26 12:45:25.047224 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/participating_artist_transformer.py
+-rw-r--r--   0        0        0     1020 2023-05-26 12:45:25.134461 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/pivot_transformer.py
+-rw-r--r--   0        0        0     1241 2023-05-26 12:45:25.119654 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/playlist_coherence_transformer.py
+-rw-r--r--   0        0        0      430 2023-05-26 12:45:25.117516 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/replace_null_values_transformer.py
+-rw-r--r--   0        0        0      321 2023-05-26 12:45:25.098192 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/select_transformer.py
+-rw-r--r--   0        0        0     4773 2023-05-26 12:45:25.285047 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/sequence_content_filter_transformer.py
+-rw-r--r--   0        0        0     2473 2023-05-26 12:45:25.101119 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/single_artist_filter_transformer.py
+-rw-r--r--   0        0        0     2721 2023-05-26 13:07:28.527893 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/stack_transformer.py
+-rw-r--r--   0        0        0     1175 2023-05-26 12:45:25.041733 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/top_items_dithering_transformer.py
+-rw-r--r--   0        0        0     1307 2023-05-26 12:45:25.073969 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/top_items_transformer.py
+-rw-r--r--   0        0        0     1488 2023-05-26 12:45:25.229498 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/track_group_availability_by_country_transformer.py
+-rw-r--r--   0        0        0     1297 2023-05-26 13:07:28.409016 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/track_group_availability_transformer.py
+-rw-r--r--   0        0        0     4399 2023-05-26 12:45:25.221232 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/track_group_filter_transformer.py
+-rw-r--r--   0        0        0      355 2023-05-26 12:45:25.115358 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/union_transformer.py
+-rw-r--r--   0        0        0     1635 2023-05-26 12:45:25.138086 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/voiceness_filter_transformer.py
+-rw-r--r--   0        0        0      780 2023-05-26 12:45:25.091990 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/where_transformer.py
+-rw-r--r--   0        0        0      544 2023-05-26 12:45:25.277219 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/with_column_renamed_transfomer.py
+-rw-r--r--   0        0        0      516 2023-05-26 12:45:25.238213 tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/with_column_transfomer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:23:49.409343 tidal_per_transformers-0.0.2/tidal_per_transformers/utils/__init__.py
+-rw-r--r--   0        0        0      545 2023-05-26 13:07:28.342392 tidal_per_transformers-0.0.2/tidal_per_transformers/utils/class_utils.py
+-rw-r--r--   0        0        0     7789 2023-05-26 12:27:47.437361 tidal_per_transformers-0.0.2/tidal_per_transformers/utils/constants.py
+-rw-r--r--   0        0        0     1917 2021-11-09 07:16:08.661545 tidal_per_transformers-0.0.2/tidal_per_transformers/utils/dither_utils.py
+-rw-r--r--   0        0        0      881 2023-05-26 13:07:28.479609 tidal_per_transformers-0.0.2/tidal_per_transformers/utils/schemas.py
+-rw-r--r--   0        0        0     1233 2023-02-22 15:09:27.044718 tidal_per_transformers-0.0.2/tidal_per_transformers/utils/spark_utils.py
+-rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 tidal_per_transformers-0.0.2/PKG-INFO
```

### Comparing `tidal_per_transformers-0.0.1/LICENSE` & `tidal_per_transformers-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/README.md` & `tidal_per_transformers-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/pyproject.toml` & `tidal_per_transformers-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 [project]
-name = "tidal_per_transformers"
-version = "0.0.1"
-authors = [
-  { name="Jing", email="jxie@squareup.com"},
-  { name="Loay", email="loay@squareup.com" },
-  { name="Tao", email="tma@squareup.com" },
-  { name="Thomas", email="talmenningen@squareup.com"},
-]
-description = "Common transformers used by the tidal personalization team."
-readme = "README.md"
-requires-python = "3.8.16"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Apache License V 2.0",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "GitHub" = "https://github.com/tidal-open-source/per-transformers"
 
 [tool.poetry]
 name = "tidal_per_transformers"
 package-dir = "tidal_per_transformer"
-version = "0.0.1"
+version = "0.0.2"
 description = "common transformers used by the tidal personalization team."
-authors = ["loay <loay@squareup.com>"]
+authors = [
+    "Jing <jxie@squareup.com>",
+    "Loay <loay@squareup.com>",
+    "Tao <tma@squareup.com>",
+    "Thomas <talmenningen@squareup.com>",
+]
+
 license = "Apache License V 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.8.16"
 pyspark = "3.4.0"
 numpy = ">=1.16.4"
```

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/__init__.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/aggregate_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/aggregate_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/artist_compound_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/artist_compound_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/artist_filter_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/artist_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/artists_struct_filter_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/artists_struct_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/blazingtext_input_format_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/blazingtext_input_format_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/broadcast_array_intersect_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/broadcast_array_intersect_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/clean_text_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/clean_text_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/collect_ranked_list_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/collect_ranked_list_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/collect_ranked_map_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/collect_ranked_map_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/deduplicate_sequence_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/deduplicate_sequence_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/distinct_sequence_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/distinct_sequence_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/filter_infrequent_seq_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/filter_infrequent_seq_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/filter_infrequent_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/filter_infrequent_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/flatten_struct_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/flatten_struct_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/join_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/join_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/loggable_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/loggable_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/main_artist_compound_mapping_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/main_artist_compound_mapping_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/minmax_scaling_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/minmax_scaling_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/multiple_compound_mapping.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/multiple_compound_mapping.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/participating_artist_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/participating_artist_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/pivot_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/pivot_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/playlist_coherence_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/playlist_coherence_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/sequence_content_filter_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/sequence_content_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/single_artist_filter_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/single_artist_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/stack_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/stack_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/top_items_dithering_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/top_items_dithering_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/top_items_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/top_items_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/track_group_availability_by_country_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/track_group_availability_by_country_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/track_group_availability_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/track_group_availability_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/track_group_filter_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/track_group_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/voiceness_filter_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/voiceness_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/where_transformer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/where_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/with_column_renamed_transfomer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/with_column_renamed_transfomer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/transformers/with_column_transfomer.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/transformers/with_column_transfomer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/utils/class_utils.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/utils/class_utils.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/utils/constants.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/utils/constants.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/utils/dither_utils.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/utils/dither_utils.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/utils/schemas.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/tidal_per_transformers/utils/spark_utils.py` & `tidal_per_transformers-0.0.2/tidal_per_transformers/utils/spark_utils.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.1/PKG-INFO` & `tidal_per_transformers-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tidal-per-transformers
-Version: 0.0.1
+Version: 0.0.2
 Summary: common transformers used by the tidal personalization team.
 License: Apache License V 2.0
-Author: loay
-Author-email: loay@squareup.com
+Author: Jing
+Author-email: jxie@squareup.com
 Requires-Python: ==3.8.16
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: alphabet-detector (==0.0.7)
 Requires-Dist: boto3 (==1.24.59)
 Requires-Dist: great-expectations (==0.16.15)
 Requires-Dist: numpy (>=1.16.4)
```

