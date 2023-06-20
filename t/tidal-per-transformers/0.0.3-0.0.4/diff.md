# Comparing `tmp/tidal_per_transformers-0.0.3.tar.gz` & `tmp/tidal_per_transformers-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidal_per_transformers-0.0.3.tar", max compression
+gzip compressed data, was "tidal_per_transformers-0.0.4.tar", max compression
```

## Comparing `tidal_per_transformers-0.0.3.tar` & `tidal_per_transformers-0.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11357 2023-05-26 12:16:06.160846 tidal_per_transformers-0.0.3/LICENSE
--rw-r--r--   0        0        0      736 2023-06-08 12:26:06.996682 tidal_per_transformers-0.0.3/README.md
--rw-r--r--   0        0        0     1126 2023-06-20 12:55:37.796608 tidal_per_transformers-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2623 2023-06-20 12:52:35.160636 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/__init__.py
--rw-r--r--   0        0        0     1575 2023-06-20 12:52:35.160891 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/aggregate_transformer.py
--rw-r--r--   0        0        0     1987 2023-06-20 12:52:35.161146 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/artist_compound_transformer.py
--rw-r--r--   0        0        0     3340 2023-06-20 12:52:35.161443 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/artist_filter_transformer.py
--rw-r--r--   0        0        0     2871 2023-06-20 12:52:35.161697 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/artists_struct_filter_transformer.py
--rw-r--r--   0        0        0      801 2023-06-20 12:52:35.161936 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/blazingtext_input_format_transformer.py
--rw-r--r--   0        0        0      985 2023-06-20 12:52:35.162262 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/broadcast_array_intersect_transformer.py
--rw-r--r--   0        0        0     1727 2023-06-20 12:52:35.162584 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/clean_text_transformer.py
--rw-r--r--   0        0        0     1148 2023-06-20 12:52:35.162832 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/collect_ranked_list_transformer.py
--rw-r--r--   0        0        0     1864 2023-06-20 12:52:35.163102 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/collect_ranked_map_transformer.py
--rw-r--r--   0        0        0      889 2023-06-20 12:52:35.163346 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/deduplicate_sequence_transformer.py
--rw-r--r--   0        0        0     1253 2023-06-20 12:52:35.163596 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/distinct_sequence_transformer.py
--rw-r--r--   0        0        0      323 2023-06-20 12:52:35.163837 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/distinct_transformer.py
--rw-r--r--   0        0        0      451 2023-06-20 12:52:35.164084 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/drop_columns_transformer.py
--rw-r--r--   0        0        0      479 2023-06-20 12:52:35.164327 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/drop_duplicates_transformer.py
--rw-r--r--   0        0        0     2277 2023-06-20 12:52:35.164600 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/filter_infrequent_seq_transformer.py
--rw-r--r--   0        0        0      790 2023-06-20 12:52:35.164848 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/filter_infrequent_transformer.py
--rw-r--r--   0        0        0      683 2023-06-20 12:52:35.165079 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/flatten_struct_transformer.py
--rw-r--r--   0        0        0      661 2023-06-20 12:52:35.165315 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/join_transformer.py
--rw-r--r--   0        0        0      844 2023-06-20 12:52:35.165569 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/loggable_transformer.py
--rw-r--r--   0        0        0     1510 2023-06-20 12:52:35.165831 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/main_artist_compound_mapping_transformer.py
--rw-r--r--   0        0        0     1374 2023-06-20 12:52:35.166081 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/minmax_scaling_transformer.py
--rw-r--r--   0        0        0     1670 2023-06-20 12:52:35.166341 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/multiple_compound_mapping.py
--rw-r--r--   0        0        0      342 2023-06-20 12:52:35.166581 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/order_by_transformer.py
--rw-r--r--   0        0        0      822 2023-06-20 12:52:35.166835 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/participating_artist_transformer.py
--rw-r--r--   0        0        0     1020 2023-06-20 12:52:35.167086 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/pivot_transformer.py
--rw-r--r--   0        0        0     1254 2023-06-20 12:52:35.167349 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/playlist_coherence_transformer.py
--rw-r--r--   0        0        0      430 2023-06-20 12:52:35.167583 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/replace_null_values_transformer.py
--rw-r--r--   0        0        0      321 2023-06-20 12:52:35.167815 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/select_transformer.py
--rw-r--r--   0        0        0     4791 2023-06-20 12:52:35.168067 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/sequence_content_filter_transformer.py
--rw-r--r--   0        0        0     2486 2023-06-20 12:52:35.168328 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/single_artist_filter_transformer.py
--rw-r--r--   0        0        0     2721 2023-06-20 12:52:35.168570 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/stack_transformer.py
--rw-r--r--   0        0        0     1188 2023-06-20 12:52:35.168870 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/top_items_dithering_transformer.py
--rw-r--r--   0        0        0     1307 2023-06-20 12:52:35.169124 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/top_items_transformer.py
--rw-r--r--   0        0        0     1501 2023-06-20 12:52:35.169450 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/track_group_availability_by_country_transformer.py
--rw-r--r--   0        0        0     1310 2023-06-20 12:52:35.169855 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/track_group_availability_transformer.py
--rw-r--r--   0        0        0     4412 2023-06-20 12:52:35.170282 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/track_group_filter_transformer.py
--rw-r--r--   0        0        0      355 2023-06-20 12:52:35.170552 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/union_transformer.py
--rw-r--r--   0        0        0        0 2023-06-20 12:52:35.170729 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/utils/__init__.py
--rw-r--r--   0        0        0      545 2023-06-20 12:52:35.171119 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/utils/class_utils.py
--rw-r--r--   0        0        0     7789 2023-06-20 12:52:35.171415 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/utils/constants.py
--rw-r--r--   0        0        0     1917 2023-06-20 12:52:35.171814 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/utils/dither_utils.py
--rw-r--r--   0        0        0      894 2023-06-20 12:52:35.172207 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/utils/schemas.py
--rw-r--r--   0        0        0     1233 2023-06-20 12:52:35.172519 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/utils/spark_utils.py
--rw-r--r--   0        0        0     1648 2023-06-20 12:52:35.172935 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/voiceness_filter_transformer.py
--rw-r--r--   0        0        0      780 2023-06-20 12:52:35.173320 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/where_transformer.py
--rw-r--r--   0        0        0      544 2023-06-20 12:52:35.173716 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/with_column_renamed_transfomer.py
--rw-r--r--   0        0        0      516 2023-06-20 12:52:35.174103 tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/with_column_transfomer.py
--rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 tidal_per_transformers-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 14:31:43.020173 tidal_per_transformers-0.0.4/LICENSE
+-rw-r--r--   0        0        0      736 2023-06-20 14:31:43.020173 tidal_per_transformers-0.0.4/README.md
+-rw-r--r--   0        0        0     1088 2023-06-20 14:31:43.020173 tidal_per_transformers-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2625 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/__init__.py
+-rw-r--r--   0        0        0     1598 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/aggregate_transformer.py
+-rw-r--r--   0        0        0     2033 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/artist_compound_transformer.py
+-rw-r--r--   0        0        0     3409 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/artist_filter_transformer.py
+-rw-r--r--   0        0        0     2917 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/artists_struct_filter_transformer.py
+-rw-r--r--   0        0        0      824 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/blazingtext_input_format_transformer.py
+-rw-r--r--   0        0        0     1031 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/broadcast_array_intersect_transformer.py
+-rw-r--r--   0        0        0     1750 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/clean_text_transformer.py
+-rw-r--r--   0        0        0     1171 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/collect_ranked_list_transformer.py
+-rw-r--r--   0        0        0     1887 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/collect_ranked_map_transformer.py
+-rw-r--r--   0        0        0      912 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/deduplicate_sequence_transformer.py
+-rw-r--r--   0        0        0     1299 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/distinct_sequence_transformer.py
+-rw-r--r--   0        0        0      346 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/distinct_transformer.py
+-rw-r--r--   0        0        0      451 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/drop_columns_transformer.py
+-rw-r--r--   0        0        0      502 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/drop_duplicates_transformer.py
+-rw-r--r--   0        0        0     2323 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/filter_infrequent_seq_transformer.py
+-rw-r--r--   0        0        0      813 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/filter_infrequent_transformer.py
+-rw-r--r--   0        0        0      706 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/flatten_struct_transformer.py
+-rw-r--r--   0        0        0      684 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/join_transformer.py
+-rw-r--r--   0        0        0      902 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/loggable_transformer.py
+-rw-r--r--   0        0        0     1556 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/main_artist_compound_mapping_transformer.py
+-rw-r--r--   0        0        0     1420 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/minmax_scaling_transformer.py
+-rw-r--r--   0        0        0     1716 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/multiple_compound_mapping.py
+-rw-r--r--   0        0        0      365 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/order_by_transformer.py
+-rw-r--r--   0        0        0      868 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/participating_artist_transformer.py
+-rw-r--r--   0        0        0     1043 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/pivot_transformer.py
+-rw-r--r--   0        0        0     1300 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/playlist_coherence_transformer.py
+-rw-r--r--   0        0        0      453 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/replace_null_values_transformer.py
+-rw-r--r--   0        0        0      344 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/select_transformer.py
+-rw-r--r--   0        0        0     4914 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/sequence_content_filter_transformer.py
+-rw-r--r--   0        0        0     2532 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/single_artist_filter_transformer.py
+-rw-r--r--   0        0        0     2721 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/stack_transformer.py
+-rw-r--r--   0        0        0     1270 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/top_items_dithering_transformer.py
+-rw-r--r--   0        0        0     1330 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/top_items_transformer.py
+-rw-r--r--   0        0        0     1547 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/track_group_availability_by_country_transformer.py
+-rw-r--r--   0        0        0     1356 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/track_group_availability_transformer.py
+-rw-r--r--   0        0        0     4458 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/track_group_filter_transformer.py
+-rw-r--r--   0        0        0      378 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/union_transformer.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/utils/__init__.py
+-rw-r--r--   0        0        0      545 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/utils/class_utils.py
+-rw-r--r--   0        0        0     7789 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/utils/constants.py
+-rw-r--r--   0        0        0     1917 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/utils/dither_utils.py
+-rw-r--r--   0        0        0      917 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/utils/schemas.py
+-rw-r--r--   0        0        0     1233 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/utils/spark_utils.py
+-rw-r--r--   0        0        0     1671 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/voiceness_filter_transformer.py
+-rw-r--r--   0        0        0      803 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/where_transformer.py
+-rw-r--r--   0        0        0      567 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/with_column_renamed_transfomer.py
+-rw-r--r--   0        0        0      539 2023-06-20 14:31:43.024173 tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/with_column_transfomer.py
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 tidal_per_transformers-0.0.4/PKG-INFO
```

### Comparing `tidal_per_transformers-0.0.3/LICENSE` & `tidal_per_transformers-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.3/README.md` & `tidal_per_transformers-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.3/pyproject.toml` & `tidal_per_transformers-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 ]
 
 [project.urls]
 "GitHub" = "https://github.com/tidal-open-source/per-transformers"
 
 [tool.poetry]
 name = "tidal_per_transformers"
-package-dir = "tidal_per_transformer"
-version = "0.0.3"
+version = "0.0.4"
 description = "common transformers used by the tidal personalization team."
 authors = [
     "Jing <jxie@squareup.com>",
     "Loay <loay@squareup.com>",
     "Tao <tma@squareup.com>",
     "Thomas <talmenningen@squareup.com>",
 ]
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/__init__.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .artist_filter_transformer import ArtistFilterTransformer
 from .artists_struct_filter_transformer import ArtistsStructFilterTransformer
 from .blazingtext_input_format_transformer import BlazingTextInputFormatTransformer
 from .clean_text_transformer import CleanTextTransformer
 from .collect_ranked_list_transformer import CollectRankedListTransformer
 from .deduplicate_sequence_transformer import DuplicateSequenceTransformer
 from .distinct_sequence_transformer import DistinctSequenceTransformer
-from .distinct_transformer import DistinctTransformer
+# from .distinct_transformer import DistinctTransformer
 from .drop_duplicates_transformer import DropDuplicatesTransformer
 from .filter_infrequent_seq_transformer import FilterInfrequentSeqItemsTransformer
 from .filter_infrequent_transformer import FilterInfrequentTransformer
 from .flatten_struct_transformer import FlattenStructTransformer
 from .join_transformer import JoinTransformer
 from .minmax_scaling_transformer import MinMaxScalingTransformer
 from .order_by_transformer import OrderByTransformer
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/aggregate_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/aggregate_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from transformers import LoggableTransformer
+from tidal_per_transformers.transformers import LoggableTransformer
 
 
 class AggregateTransformer(LoggableTransformer):
     """
     Group a column by the 'group_by' column and perform aggregation expressions defined in 'agg_exp'.
     This implementation does unfortunately not support multiple aggregations per column!
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/artist_compound_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/artist_compound_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pyspark.sql import functions as F, DataFrame
-from transformers import LoggableTransformer
+from tidal_per_transformers.transformers import LoggableTransformer
 
-import transformers.utils.constants as c
+import tidal_per_transformers.transformers.utils.constants as c
 
 
 class ArtistCompoundMappingTransformer(LoggableTransformer):
     """
     Map the artist compound id's (e.g. Miguel feat. Travis Scott -> Miguel, Travis Scott)
 
     TODO: Find a better way of picking the top n featuring artist per compound id
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/artist_filter_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/artist_filter_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import abstractmethod
 
 import pyspark.sql.functions as F
 from pyspark.sql.dataframe import DataFrame
 
-import transformers.utils.constants as c
-from transformers.loggable_transformer import LoggableTransformer
-from transformers.track_group_filter_transformer import apply_category_filters
+import tidal_per_transformers.transformers.utils.constants as c
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
+from tidal_per_transformers.transformers.track_group_filter_transformer import apply_category_filters
 
 
 class ArtistFilterTransformer(LoggableTransformer):
     """
     Transformer for removing artists based on either category, popularity or a combination of the two. E.g. if you
     want the artist recommender feature to not recommend children music you can choose to filter all artists tagged
     with the children music tag. The popularity features are based on streaming data from the last 12 months
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/artists_struct_filter_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/artists_struct_filter_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pyspark.sql.functions as F
 import pyspark.sql.types as T
 from pyspark.sql.dataframe import DataFrame
 
-import transformers.utils.constants as c
-from transformers import ArtistFilterTransformer
+import tidal_per_transformers.transformers.utils.constants as c
+from tidal_per_transformers.transformers import ArtistFilterTransformer
 
 
 class ArtistsStructFilterTransformer(ArtistFilterTransformer):
     """
     :param artist_filters:          DataFrame containing the content filter information
     :param remove_ambient_music:    flag for toggling ambient music on/off
     :param remove_holiday_music:    flag for toggling holiday music on/off
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/blazingtext_input_format_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/blazingtext_input_format_transformer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 import pyspark.sql.functions as F
 
-from transformers.loggable_transformer import LoggableTransformer
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
 
 
 class BlazingTextInputFormatTransformer(LoggableTransformer):
     """ Convert an array column to the input format required by BlazingText """
 
     def __init__(self, items_column: str, alias: Optional[str] = None):
         """
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/broadcast_array_intersect_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/broadcast_array_intersect_transformer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pyspark.sql.functions as F
-import transformers.utils.constants as c
+import tidal_per_transformers.transformers.utils.constants as c
 from pyspark.sql import DataFrame
 
-from transformers import LoggableTransformer
+from tidal_per_transformers.transformers import LoggableTransformer
 
 
 class BroadcastArrayIntersectTransformer(LoggableTransformer):
     def __init__(self, array_col: str, items_to_keep: DataFrame):
         """
         Transformer to filter out invalid items from an array column based on items_to_keep.
         :param array_col:       name of column containing an array of items
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/clean_text_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/clean_text_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pandas as pd
 import pyspark.sql.functions as F
 from alphabet_detector import AlphabetDetector
 from pyspark.ml.base import Transformer
 from pyspark.sql.types import StringType
 
-import transformers.utils.constants as c
+import tidal_per_transformers.transformers.utils.constants as c
 
 
 @F.pandas_udf(returnType=StringType())
 def strip_accents_udf(texts: pd.Series) -> pd.Series:
 
     def _strip_accents(text):
         if not AlphabetDetector().only_alphabet_chars(text, "LATIN"):
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/collect_ranked_list_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/collect_ranked_list_transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pyspark.sql import functions as F
 from pyspark.sql.window import Window
-from transformers import LoggableTransformer
+from tidal_per_transformers.transformers import LoggableTransformer
 
 
 class CollectRankedListTransformer(LoggableTransformer):
     """
     Group a column by the 'group_by' column and collect the sorted values in the 'list_col' as a list
 
     :param group_by:   Columns to group the DataFrame by
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/collect_ranked_map_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/collect_ranked_map_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pyspark.sql import functions as F
 from pyspark.sql.types import MapType, ArrayType, StringType
 from pyspark.sql.window import Window
-from transformers import LoggableTransformer
+from tidal_per_transformers.transformers import LoggableTransformer
 
 
 class CollectRankedMapTransformer(LoggableTransformer):
     """
     Group a column by the 'group_by' column and collect the sorted values in the 'map_col' as a map
 
     :param group_by:        Columns to group the DataFrame by
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/deduplicate_sequence_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/deduplicate_sequence_transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from transformers.loggable_transformer import LoggableTransformer
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
 import pyspark.sql.types as T
 import pyspark.sql.functions as F
 
 
 class DuplicateSequenceTransformer(LoggableTransformer):
     """ Remove duplicate items from a sequence """
     def __init__(self, column: str, id_field: str, schema: T.ArrayType):
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/distinct_sequence_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/distinct_sequence_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pyspark.sql.types as T
 from pyspark.sql import Window
 from pyspark.sql import functions as F
 
-import transformers.utils.constants as c
-from transformers.loggable_transformer import LoggableTransformer
+import tidal_per_transformers.transformers.utils.constants as c
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
 
 SEQUENCE_HASH = "sequenceHash"
 
 
 class DistinctSequenceTransformer(LoggableTransformer):
     """
     Deduplicate a dataframe by a column containing a collection. This can e.g. be used to remove duplicate
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/filter_infrequent_seq_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/filter_infrequent_seq_transformer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 import pyspark.sql.functions as F
-from transformers.loggable_transformer import LoggableTransformer
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
 from pyspark.sql.types import DataType
 
-import transformers.utils.constants as c
+import tidal_per_transformers.transformers.utils.constants as c
 
 
 class FilterInfrequentSeqItemsTransformer(LoggableTransformer):
 
     def __init__(self,
                  min_item_frequency: int,
                  sequence_column: str,
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/filter_infrequent_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/filter_infrequent_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pyspark.sql.window import Window
-from transformers.loggable_transformer import LoggableTransformer
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
 import pyspark.sql.functions as F
 
 
 class FilterInfrequentTransformer(LoggableTransformer):
     """
     Remove the items with a count smaller than cutoff
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/flatten_struct_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/flatten_struct_transformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict
 import pyspark.sql.functions as F
 
 from pyspark.sql import DataFrame
-from transformers import LoggableTransformer
+from tidal_per_transformers.transformers import LoggableTransformer
 
 
 class FlattenStructTransformer(LoggableTransformer):
     """Flatten each struct field into a new column
 
     :param struct_fields: Dictionary containing new column names and their corresponding struct field names
     """
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/loggable_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/loggable_transformer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC
 from typing import Dict
 from pyspark.ml.base import Transformer
-import transformers.utils.constants as c
-from transformers.utils import as_dict
+import tidal_per_transformers.transformers.utils.constants as c
+from tidal_per_transformers.transformers.utils.class_utils import as_dict
 
 
 class LoggableTransformer(Transformer, ABC):
     """
     Collect list on "item_column" and ordered by order_by_column
     """
     def __init__(self):
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/main_artist_compound_mapping_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/main_artist_compound_mapping_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pyspark.ml.base import Transformer
 from pyspark.sql import functions as F, DataFrame
 
-import transformers.utils.constants as c
-from transformers.utils import get_top_items
+import tidal_per_transformers.transformers.utils.constants as c
+from tidal_per_transformers.transformers.utils import get_top_items
 
 
 class MainArtistCompoundMappingTransformer(Transformer):
     """
     Map the artist compound id's to a single main artist (e.g. Miguel feat. Travis Scott -> Miguel)
 
     :returns    DataFrame where the compound id's have been mapped to their constituent parts
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/minmax_scaling_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/minmax_scaling_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pyspark.sql.functions as F
-from transformers.loggable_transformer import LoggableTransformer
-import transformers.utils.constants as c
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
+import tidal_per_transformers.transformers.utils.constants as c
 
 
 class MinMaxScalingTransformer(LoggableTransformer):
     """
     Min max transformation
     """
     def __init__(self, input_score_range=None, target_score_range=(1, 5), rounding=True):
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/multiple_compound_mapping.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/multiple_compound_mapping.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pyspark.sql import DataFrame
 from pyspark.sql.window import Window
 import pyspark.sql.functions as F
-import transformers.utils.constants as c
-from transformers import LoggableTransformer
+import tidal_per_transformers.transformers.utils.constants as c
+from tidal_per_transformers.transformers import LoggableTransformer
 
 
 class MultipleCompoundTransformer(LoggableTransformer):
     """
     Custom compound mapping transformer mapping compoundIds to all main artists on a track
     For tracks with > 1 main artists they are all assigned a weight equal to count/num_artists
     E.g. for each stream on a track featuring both Jay-Z and Kanye they each receive 0.5 streams each
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/participating_artist_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/participating_artist_transformer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pyspark.sql.functions as F
-import transformers.utils.constants as c
+import tidal_per_transformers.transformers.utils.constants as c
 
 from pyspark.sql import DataFrame
-from transformers import LoggableTransformer
+from tidal_per_transformers.transformers import LoggableTransformer
 
 
 class ParticipatingArtistsTransformer(LoggableTransformer):
     """Transforms artists field into main and featuring artist transformer
 
     """
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/pivot_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/pivot_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, List, Union
 
-from transformers.loggable_transformer import LoggableTransformer
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
 
 
 class PivotTransformer(LoggableTransformer):
 
     def __init__(self,
                  group_by: Union[str, List],
                  pivot_col: str,
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/playlist_coherence_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/playlist_coherence_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pyspark.sql import Window, DataFrame, functions as F
-from transformers.loggable_transformer import LoggableTransformer
-import transformers.utils.constants as c
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
+import tidal_per_transformers.transformers.utils.constants as c
 
 
 class PlaylistCoherenceTransformer(LoggableTransformer):
     """
     Filter playlists based on how coherence according to the playlist_coherence model
 
     threshold: minimum coherence value to keep the playlist
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/sequence_content_filter_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/sequence_content_filter_transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pyspark.sql.functions as F
 from pyspark.sql.dataframe import DataFrame
 
-import transformers.utils.constants as c
-from transformers.artist_filter_transformer import ArtistFilterTransformer
-from transformers.loggable_transformer import LoggableTransformer
-from transformers.track_group_filter_transformer import TrackGroupFilterTransformer
-from transformers.utils import PLAYLIST_TRACKS_SCHEMA
+import tidal_per_transformers.transformers.utils.constants as c
+from tidal_per_transformers.transformers.artist_filter_transformer import ArtistFilterTransformer
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
+from tidal_per_transformers.transformers.track_group_filter_transformer import TrackGroupFilterTransformer
+from tidal_per_transformers.transformers.utils.schemas import PLAYLIST_TRACKS_SCHEMA
 
 MATCHES = "matches"
 
 
 class SequenceContentFilterTransformer(LoggableTransformer):
     """
     Transformer for applying content filters to columns with lists of tracks. This can e.g. be applied to the
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/single_artist_filter_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/single_artist_filter_transformer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pyspark.sql.dataframe import DataFrame
 
-import transformers.utils.constants as c
-from transformers import ArtistFilterTransformer
+import tidal_per_transformers.transformers.utils.constants as c
+from tidal_per_transformers.transformers import ArtistFilterTransformer
 
 
 class SingleArtistFilterTransformer(ArtistFilterTransformer):
     """
         :param artist_filters:          DataFrame containing the content filter information
         :param remove_ambient_music:    flag for toggling ambient music on/off
         :param remove_holiday_music:    flag for toggling holiday music on/off
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/stack_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/stack_transformer.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/top_items_dithering_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/top_items_dithering_transformer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pyspark.sql.functions as F
-import transformers.utils.constants as c
+import tidal_per_transformers.transformers.utils.constants as c
 
 from pyspark.sql.window import Window
-from transformers.loggable_transformer import LoggableTransformer
-from transformers.utils import dither
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
+from tidal_per_transformers.transformers.utils.dither_utils import dither
 
 
 class TopItemsDitheringTransformer(LoggableTransformer):
     """
     Take the top 'n' records from a partition ordered by 'order_by' after applying dithering on the original
     relevance ordering.
     """
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/top_items_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/top_items_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pyspark.sql.functions as F
 from pyspark.sql.window import Window
-from transformers.loggable_transformer import LoggableTransformer
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
 
 
 class TopItemsTransformer(LoggableTransformer):
     """
     Take the top 'n' records from a partition ordered by 'order_by'
     :param partition:   The columns used to partition the DataFrame
     :param order_by:    The column(s) used to sort the partitions
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/track_group_availability_by_country_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/track_group_availability_by_country_transformer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pyspark.sql.functions as F
-import transformers.utils.constants as c
+import tidal_per_transformers.transformers.utils.constants as c
 
 from pyspark.sql import DataFrame
-from transformers import LoggableTransformer
+from tidal_per_transformers.transformers import LoggableTransformer
 
 
 class TrackGroupAvailabilityByCountryTransformer(LoggableTransformer):
 
     def __init__(self,
                  track_group_availability: DataFrame,
                  country_col: str = c.COUNTRY_CODE,
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/track_group_availability_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/track_group_availability_transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pyspark.sql.functions as F
 from pyspark.sql import DataFrame
 
-import transformers.utils.constants as c
-from transformers import LoggableTransformer
+import tidal_per_transformers.transformers.utils.constants as c
+from tidal_per_transformers.transformers import LoggableTransformer
 
 
 class TrackGroupAvailabilityTransformer(LoggableTransformer):
 
     def __init__(self, track_group_availability: DataFrame):
         """
         Filter any track group from the input dataset that is not available for streaming. This transformer is for
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/track_group_filter_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/track_group_filter_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pyspark.sql.functions as F
 from pyspark.sql.dataframe import DataFrame
 
-import transformers.utils.constants as c
-from transformers.loggable_transformer import LoggableTransformer
+import tidal_per_transformers.transformers.utils.constants as c
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
 
 
 class TrackGroupFilterTransformer(LoggableTransformer):
     """
     Transformer for removing track groups based on either category, popularity or a combination of the two. E.g. if you
     want to remove Christmas and children music from a track based model or mix you can use this transformer to easily
     exclude those content types. The popularity features are based on streaming data from the last 12 months
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/utils/class_utils.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/utils/class_utils.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/utils/constants.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/utils/constants.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/utils/dither_utils.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/utils/dither_utils.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/utils/schemas.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/utils/schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pyspark.sql.types as T
-import transformers.utils.constants as c
+import tidal_per_transformers.transformers.utils.constants as c
 
 
 ARTISTS_SCHEMA = T.ArrayType(T.StructType([
     T.StructField(c.ALIASES, T.ArrayType(T.StringType())),
     T.StructField(c.ID, T.IntegerType()),
     T.StructField(c.NAME, T.StringType()),
     T.StructField(c.MAIN, T.BooleanType()),
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/utils/spark_utils.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/utils/spark_utils.py`

 * *Files identical despite different names*

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/voiceness_filter_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/voiceness_filter_transformer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 import pyspark.sql.functions as F
 from pandas import DataFrame
 from pyspark.ml import Transformer
 
-import transformers.utils.constants as c
+import tidal_per_transformers.transformers.utils.constants as c
 
 
 class VoicenessFilterTransformer(Transformer):
 
     def __init__(self, voiceness_scores: DataFrame, track_index: DataFrame, score_threshold: Optional[float] = None):
         """
         Transformer used to remove tracks containing voice (non music) content
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/where_transformer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/where_transformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict
-from transformers.loggable_transformer import LoggableTransformer
+from tidal_per_transformers.transformers.loggable_transformer import LoggableTransformer
 
 
 class WhereTransformer(LoggableTransformer):
     def __init__(self, where_filter):
         super().__init__()
         self.where_filter = where_filter
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/with_column_renamed_transfomer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/with_column_renamed_transfomer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pyspark.sql import DataFrame
-from transformers import LoggableTransformer
+from tidal_per_transformers.transformers import LoggableTransformer
 
 
 class WithColumnRenamedTransformer(LoggableTransformer):
     """Transformer to rename a column
 
     """
```

### Comparing `tidal_per_transformers-0.0.3/tidal_per_transformers/transformers/with_column_transfomer.py` & `tidal_per_transformers-0.0.4/tidal_per_transformers/transformers/with_column_transfomer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any
 
 from pyspark.sql import DataFrame
-from transformers import LoggableTransformer
+from tidal_per_transformers.transformers import LoggableTransformer
 
 
 class WithColumnTransformer(LoggableTransformer):
     """Create a new column with a given pyspark expression.
 
     """
```

### Comparing `tidal_per_transformers-0.0.3/PKG-INFO` & `tidal_per_transformers-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal-per-transformers
-Version: 0.0.3
+Version: 0.0.4
 Summary: common transformers used by the tidal personalization team.
 License: Apache License V 2.0
 Author: Jing
 Author-email: jxie@squareup.com
 Requires-Python: >=3.8.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

