# Comparing `tmp/geoformat-20230421.tar.gz` & `tmp/geoformat-20230620.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoformat-20230421.tar", last modified: Fri Apr 21 13:15:47 2023, max compression
+gzip compressed data, was "geoformat-20230620.tar", last modified: Tue Jun 20 15:18:04 2023, max compression
```

## Comparing `geoformat-20230421.tar` & `geoformat-20230620.tar`

### file list

```diff
@@ -1,240 +1,240 @@
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.504982 geoformat-20230421/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1305 2022-10-13 08:02:35.000000 geoformat-20230421/LICENSE
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20635 2023-04-21 13:15:47.500982 geoformat-20230421/PKG-INFO
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    19758 2023-04-21 13:10:35.000000 geoformat-20230421/README.md
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.356985 geoformat-20230421/geoformat/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    14558 2023-01-16 19:36:49.000000 geoformat-20230421/geoformat/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      280 2023-04-21 13:15:34.000000 geoformat-20230421/geoformat/_version.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.360985 geoformat-20230421/geoformat/conf/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conf/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2044 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conf/decorator.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      836 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/conf/driver_variable.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3625 2023-01-16 19:36:49.000000 geoformat-20230421/geoformat/conf/error_messages.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3832 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/conf/fields_variable.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1744 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conf/format_data.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)       35 2022-12-12 09:38:12.000000 geoformat-20230421/geoformat/conf/geoformat_var.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3990 2023-01-03 14:19:37.000000 geoformat-20230421/geoformat/conf/geometry_variable.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4897 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/conf/path.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      700 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/conf/proj_var.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10042 2023-01-03 14:29:45.000000 geoformat-20230421/geoformat/conf/timer.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.364985 geoformat-20230421/geoformat/constraints/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/constraints/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1810 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/constraints/primary_key.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.372985 geoformat-20230421/geoformat/conversion/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conversion/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1381 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conversion/bbox_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4858 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conversion/bytes_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     8010 2023-04-21 13:15:34.000000 geoformat-20230421/geoformat/conversion/coordinates_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      992 2023-01-03 14:29:45.000000 geoformat-20230421/geoformat/conversion/datetime_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    46110 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/conversion/feature_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    16223 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/conversion/fields_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6898 2023-01-16 19:36:49.000000 geoformat-20230421/geoformat/conversion/geolayer_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    50975 2023-01-03 14:29:45.000000 geoformat-20230421/geoformat/conversion/geometry_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7331 2023-01-16 19:36:49.000000 geoformat-20230421/geoformat/conversion/metadata_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      701 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conversion/precision_tolerance_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1732 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/conversion/segment_conversion.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.372985 geoformat-20230421/geoformat/db/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/db/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2070 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/db/db_request.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.376985 geoformat-20230421/geoformat/driver/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/driver/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2652 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/driver/common_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    13306 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/driver/csv_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    40428 2023-01-03 14:29:45.000000 geoformat-20230421/geoformat/driver/esri_shapefile_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    12370 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/driver/geojson_driver.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.376985 geoformat-20230421/geoformat/driver/ogr/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/driver/ogr/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    41141 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/driver/ogr/ogr_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     9889 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/driver/postgresql_driver.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.380985 geoformat-20230421/geoformat/explore_data/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/explore_data/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5345 2023-01-16 19:36:49.000000 geoformat-20230421/geoformat/explore_data/duplicate.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    16452 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/explore_data/print_data.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1403 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/explore_data/random_geometry.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.380985 geoformat-20230421/geoformat/geoprocessing/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1256 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/area.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.380985 geoformat-20230421/geoformat/geoprocessing/connectors/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/connectors/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2143 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/connectors/operations.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    12104 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/connectors/predicates.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.388985 geoformat-20230421/geoformat/geoprocessing/generalization/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/generalization/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2209 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/generalization/ramer_douglas_peucker.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4989 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/generalization/visvalingam_whyatt.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.392984 geoformat-20230421/geoformat/geoprocessing/geoparameters/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/geoparameters/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3396 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/geoparameters/bbox.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      877 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/geoparameters/boundaries.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5335 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/geoparameters/lines.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1362 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/length.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    11567 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/line_merge.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.392984 geoformat-20230421/geoformat/geoprocessing/matrix/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/matrix/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5464 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/matrix/adjacency.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.392984 geoformat-20230421/geoformat/geoprocessing/measure/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/measure/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1328 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/measure/area.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3560 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/measure/distance.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      560 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/measure/length.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7282 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/merge_geometries.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7441 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/point_on_linestring.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3824 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/simplify.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5237 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/geoprocessing/split.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2084 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/geoprocessing/union.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.392984 geoformat-20230421/geoformat/index/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/index/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.392984 geoformat-20230421/geoformat/index/attributes/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/index/attributes/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      670 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/index/attributes/hash.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.392984 geoformat-20230421/geoformat/index/geometry/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/index/geometry/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    14746 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/index/geometry/grid.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.396984 geoformat-20230421/geoformat/manipulation/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/manipulation/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2859 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/manipulation/feature_manipulation.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20815 2023-01-03 14:42:19.000000 geoformat-20230421/geoformat/manipulation/geolayer_manipulation.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10051 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/manipulation/metadata_manipulation.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.396984 geoformat-20230421/geoformat/obj/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/obj/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      774 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/obj/geometry.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.396984 geoformat-20230421/geoformat/processing/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/processing/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.396984 geoformat-20230421/geoformat/processing/data/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/geoformat/processing/data/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     9722 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/processing/data/clauses.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10536 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/processing/data/field_statistics.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.400984 geoformat-20230421/geoformat/processing/data/join/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/geoformat/processing/data/join/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    26996 2023-01-16 19:36:49.000000 geoformat-20230421/geoformat/processing/data/join/join.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    11975 2023-01-03 14:30:13.000000 geoformat-20230421/geoformat/processing/data/join/merge_objects.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5199 2022-11-24 15:49:21.000000 geoformat-20230421/geoformat/processing/data/union.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.356985 geoformat-20230421/geoformat.egg-info/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20635 2023-04-21 13:15:47.000000 geoformat-20230421/geoformat.egg-info/PKG-INFO
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7676 2023-04-21 13:15:47.000000 geoformat-20230421/geoformat.egg-info/SOURCES.txt
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        1 2023-04-21 13:15:47.000000 geoformat-20230421/geoformat.egg-info/dependency_links.txt
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)       16 2023-04-21 13:15:47.000000 geoformat-20230421/geoformat.egg-info/top_level.txt
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)       38 2023-04-21 13:15:47.504982 geoformat-20230421/setup.cfg
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1210 2023-04-21 13:10:35.000000 geoformat-20230421/setup.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.356985 geoformat-20230421/tests/
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.428984 geoformat-20230421/tests/data/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/data/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15423 2022-10-13 08:02:35.000000 geoformat-20230421/tests/data/coordinates.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    43859 2023-01-03 14:30:13.000000 geoformat-20230421/tests/data/features.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2394 2022-10-13 08:02:35.000000 geoformat-20230421/tests/data/fields_metadata.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)  9850700 2023-01-03 14:30:13.000000 geoformat-20230421/tests/data/geolayers.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    26450 2023-04-21 13:15:34.000000 geoformat-20230421/tests/data/geometries.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    58422 2022-09-13 14:34:13.000000 geoformat-20230421/tests/data/geometry_index.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1227 2022-10-13 08:02:35.000000 geoformat-20230421/tests/data/index.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      232 2022-09-13 14:34:13.000000 geoformat-20230421/tests/data/matrix.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5099 2023-01-03 14:30:13.000000 geoformat-20230421/tests/data/metadata.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      435 2022-09-13 14:34:13.000000 geoformat-20230421/tests/data/segments.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.428984 geoformat-20230421/tests/geoformat/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.432983 geoformat-20230421/tests/geoformat/conf/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/conf/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3617 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conf/test_format_data.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     8633 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/conf/test_path.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.432983 geoformat-20230421/tests/geoformat/constraints/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/constraints/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2987 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/constraints/test_primary_key.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.460983 geoformat-20230421/tests/geoformat/conversion/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/conversion/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2380 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conversion/test_bbox_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17731 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conversion/test_bytes_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17709 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conversion/test_coordinates_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      986 2023-01-03 14:29:45.000000 geoformat-20230421/tests/geoformat/conversion/test_datetime_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   205565 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/conversion/test_feature_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   161950 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/conversion/test_fields_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)  5602810 2022-11-24 15:49:21.000000 geoformat-20230421/tests/geoformat/conversion/test_geolayer_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    92781 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conversion/test_geometry_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    65479 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/conversion/test_metadata_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1238 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conversion/test_precision_tolerance_conversion.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3245 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/conversion/test_segment_conversion.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.460983 geoformat-20230421/tests/geoformat/db/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/db/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.472983 geoformat-20230421/tests/geoformat/driver/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/driver/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.472983 geoformat-20230421/tests/geoformat/driver/ogr/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/driver/ogr/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      369 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/driver/ogr/compare_ogr_files.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1251 2023-01-03 14:29:45.000000 geoformat-20230421/tests/geoformat/driver/ogr/geolayer_to_geojson.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1263 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/driver/ogr/geolayer_to_postgresql.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2155 2023-01-03 14:29:45.000000 geoformat-20230421/tests/geoformat/driver/ogr/geolayer_to_shapefile.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    16224 2023-01-03 14:29:45.000000 geoformat-20230421/tests/geoformat/driver/test_common_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    29687 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/driver/test_csv_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   321121 2023-01-03 14:29:45.000000 geoformat-20230421/tests/geoformat/driver/test_esri_shapefile_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)  1461478 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/driver/test_geojson_driver.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   114134 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/driver/test_postgresql_driver.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.476982 geoformat-20230421/tests/geoformat/explore_data/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/explore_data/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17339 2023-01-16 19:36:49.000000 geoformat-20230421/tests/geoformat/explore_data/test_duplicate.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    66158 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/explore_data/test_print_data.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.476982 geoformat-20230421/tests/geoformat/geoprocessing/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/geoprocessing/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.480982 geoformat-20230421/tests/geoformat/geoprocessing/connectors/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/geoprocessing/connectors/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4728 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/connectors/test_operations.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15761 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/connectors/test_predicates.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.480982 geoformat-20230421/tests/geoformat/geoprocessing/generalization/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/generalization/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2176 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/generalization/test_ramer_douglas_peucker.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1845 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/generalization/test_visvalingam_whyatt.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.480982 geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3562 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/test_bbox.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      901 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/test_boundaries.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     9425 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/test_lines.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.480982 geoformat-20230421/tests/geoformat/geoprocessing/matrix/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/geoprocessing/matrix/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1645 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/matrix/test_adjacency.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.484982 geoformat-20230421/tests/geoformat/geoprocessing/measure/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/geoprocessing/measure/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2234 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/measure/test_area.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3736 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/measure/test_distance.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1525 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/measure/test_length.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1758 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_area.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2337 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_length.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15898 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_line_merge.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4976 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_merge_geometries.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4575 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_point_on_linestring.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    14514 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_simplify.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    53164 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_split.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1387 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/geoprocessing/test_union.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.484982 geoformat-20230421/tests/geoformat/index/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/index/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.484982 geoformat-20230421/tests/geoformat/index/attributes/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/index/attributes/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1279 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/index/attributes/test_hash.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.488982 geoformat-20230421/tests/geoformat/index/geometry/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/index/geometry/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15928 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/index/geometry/test_grid.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.496982 geoformat-20230421/tests/geoformat/manipulation/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/manipulation/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    12109 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/manipulation/test_feature_manipulation.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   256166 2023-01-03 14:30:13.000000 geoformat-20230421/tests/geoformat/manipulation/test_geolayer_manipulation.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    38639 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/manipulation/test_metadata_manipulation.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.496982 geoformat-20230421/tests/geoformat/obj/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/obj/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1928 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/obj/test_geometry.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.496982 geoformat-20230421/tests/geoformat/processing/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/processing/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.496982 geoformat-20230421/tests/geoformat/processing/data/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/geoformat/processing/data/__init__.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.500982 geoformat-20230421/tests/geoformat/processing/data/join/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/processing/data/join/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   608012 2023-01-16 19:36:49.000000 geoformat-20230421/tests/geoformat/processing/data/join/test_join.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20394 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/processing/data/join/test_merge_objects.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6946 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/processing/data/test_clauses.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7537 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/processing/data/test_field_statistics.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6065 2022-10-13 08:02:35.000000 geoformat-20230421/tests/geoformat/processing/data/test_union.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.500982 geoformat-20230421/tests/inspector/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230421/tests/inspector/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17877 2023-01-03 14:30:13.000000 geoformat-20230421/tests/inspector/geoformat_inspector.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.500982 geoformat-20230421/tests/perf/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/tests/perf/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10403 2023-01-03 14:30:13.000000 geoformat-20230421/tests/perf/compare_func.py
-drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-04-21 13:15:47.500982 geoformat-20230421/tests/utils/
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230421/tests/utils/__init__.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1379 2023-01-03 14:29:45.000000 geoformat-20230421/tests/utils/compare.py
--rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6701 2023-01-03 14:30:13.000000 geoformat-20230421/tests/utils/tests_utils.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.955898 geoformat-20230620/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1305 2022-10-13 08:02:35.000000 geoformat-20230620/LICENSE
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20635 2023-06-20 15:18:04.955898 geoformat-20230620/PKG-INFO
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    19758 2023-06-20 11:56:04.000000 geoformat-20230620/README.md
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.719904 geoformat-20230620/geoformat/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    14558 2023-01-16 19:36:49.000000 geoformat-20230620/geoformat/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      280 2023-06-20 14:15:56.000000 geoformat-20230620/geoformat/_version.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.731904 geoformat-20230620/geoformat/conf/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/conf/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2044 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/conf/decorator.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      836 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/conf/driver_variable.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3699 2023-06-20 12:32:23.000000 geoformat-20230620/geoformat/conf/error_messages.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3832 2023-01-03 14:30:13.000000 geoformat-20230620/geoformat/conf/fields_variable.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1744 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/conf/format_data.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)       35 2022-12-12 09:38:12.000000 geoformat-20230620/geoformat/conf/geoformat_var.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3990 2023-01-03 14:19:37.000000 geoformat-20230620/geoformat/conf/geometry_variable.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4897 2023-01-03 14:30:13.000000 geoformat-20230620/geoformat/conf/path.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      700 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/conf/proj_var.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10042 2023-01-03 14:29:45.000000 geoformat-20230620/geoformat/conf/timer.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.731904 geoformat-20230620/geoformat/constraints/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/constraints/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1810 2022-11-24 15:49:21.000000 geoformat-20230620/geoformat/constraints/primary_key.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.739904 geoformat-20230620/geoformat/conversion/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/conversion/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1381 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/conversion/bbox_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4858 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/conversion/bytes_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     8010 2023-06-20 11:56:04.000000 geoformat-20230620/geoformat/conversion/coordinates_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      992 2023-01-03 14:29:45.000000 geoformat-20230620/geoformat/conversion/datetime_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    46110 2023-01-03 14:30:13.000000 geoformat-20230620/geoformat/conversion/feature_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    16223 2023-01-03 14:30:13.000000 geoformat-20230620/geoformat/conversion/fields_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6898 2023-01-16 19:36:49.000000 geoformat-20230620/geoformat/conversion/geolayer_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    50975 2023-01-03 14:29:45.000000 geoformat-20230620/geoformat/conversion/geometry_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7331 2023-01-16 19:36:49.000000 geoformat-20230620/geoformat/conversion/metadata_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      701 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/conversion/precision_tolerance_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1732 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/conversion/segment_conversion.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.739904 geoformat-20230620/geoformat/db/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/db/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2070 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/db/db_request.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.743903 geoformat-20230620/geoformat/driver/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/driver/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2695 2023-06-20 12:32:23.000000 geoformat-20230620/geoformat/driver/common_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    13306 2023-01-03 14:30:13.000000 geoformat-20230620/geoformat/driver/csv_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    40428 2023-01-03 14:29:45.000000 geoformat-20230620/geoformat/driver/esri_shapefile_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    12370 2023-01-03 14:30:13.000000 geoformat-20230620/geoformat/driver/geojson_driver.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.743903 geoformat-20230620/geoformat/driver/ogr/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/driver/ogr/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    41141 2022-11-24 15:49:21.000000 geoformat-20230620/geoformat/driver/ogr/ogr_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     9889 2022-11-24 15:49:21.000000 geoformat-20230620/geoformat/driver/postgresql_driver.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.743903 geoformat-20230620/geoformat/explore_data/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/explore_data/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5345 2023-01-16 19:36:49.000000 geoformat-20230620/geoformat/explore_data/duplicate.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    16452 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/explore_data/print_data.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1403 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/explore_data/random_geometry.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.747903 geoformat-20230620/geoformat/geoprocessing/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1256 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/area.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.751903 geoformat-20230620/geoformat/geoprocessing/connectors/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/connectors/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2143 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/geoprocessing/connectors/operations.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    12104 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/connectors/predicates.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.759903 geoformat-20230620/geoformat/geoprocessing/generalization/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/geoprocessing/generalization/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2209 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/geoprocessing/generalization/ramer_douglas_peucker.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4989 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/geoprocessing/generalization/visvalingam_whyatt.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.759903 geoformat-20230620/geoformat/geoprocessing/geoparameters/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/geoparameters/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3396 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/geoprocessing/geoparameters/bbox.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      877 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/geoparameters/boundaries.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5335 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/geoparameters/lines.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1362 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/length.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    11567 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/line_merge.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.759903 geoformat-20230620/geoformat/geoprocessing/matrix/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/matrix/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5464 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/matrix/adjacency.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.759903 geoformat-20230620/geoformat/geoprocessing/measure/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/measure/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1328 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/geoprocessing/measure/area.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3560 2023-06-20 11:56:04.000000 geoformat-20230620/geoformat/geoprocessing/measure/distance.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      560 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/measure/length.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7282 2023-06-20 11:56:04.000000 geoformat-20230620/geoformat/geoprocessing/merge_geometries.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7441 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/point_on_linestring.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3824 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/geoprocessing/simplify.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5237 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/geoprocessing/split.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2084 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/geoprocessing/union.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.759903 geoformat-20230620/geoformat/index/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/index/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.763903 geoformat-20230620/geoformat/index/attributes/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/index/attributes/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      670 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/index/attributes/hash.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.763903 geoformat-20230620/geoformat/index/geometry/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/index/geometry/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    14746 2022-11-24 15:49:21.000000 geoformat-20230620/geoformat/index/geometry/grid.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.767903 geoformat-20230620/geoformat/manipulation/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/manipulation/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2859 2022-11-24 15:49:21.000000 geoformat-20230620/geoformat/manipulation/feature_manipulation.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20815 2023-01-03 14:42:19.000000 geoformat-20230620/geoformat/manipulation/geolayer_manipulation.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10051 2023-01-03 14:30:13.000000 geoformat-20230620/geoformat/manipulation/metadata_manipulation.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.767903 geoformat-20230620/geoformat/obj/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/obj/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      774 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/obj/geometry.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.767903 geoformat-20230620/geoformat/processing/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/processing/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.771903 geoformat-20230620/geoformat/processing/data/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/geoformat/processing/data/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     9722 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/processing/data/clauses.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10536 2022-11-24 15:49:21.000000 geoformat-20230620/geoformat/processing/data/field_statistics.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.771903 geoformat-20230620/geoformat/processing/data/join/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230620/geoformat/processing/data/join/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    26996 2023-06-20 15:03:24.000000 geoformat-20230620/geoformat/processing/data/join/join.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    11975 2023-01-03 14:30:13.000000 geoformat-20230620/geoformat/processing/data/join/merge_objects.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5199 2022-11-24 15:49:21.000000 geoformat-20230620/geoformat/processing/data/union.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.723904 geoformat-20230620/geoformat.egg-info/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20635 2023-06-20 15:18:04.000000 geoformat-20230620/geoformat.egg-info/PKG-INFO
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7676 2023-06-20 15:18:04.000000 geoformat-20230620/geoformat.egg-info/SOURCES.txt
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        1 2023-06-20 15:18:04.000000 geoformat-20230620/geoformat.egg-info/dependency_links.txt
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)       16 2023-06-20 15:18:04.000000 geoformat-20230620/geoformat.egg-info/top_level.txt
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)       38 2023-06-20 15:18:04.955898 geoformat-20230620/setup.cfg
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1210 2023-06-20 11:56:04.000000 geoformat-20230620/setup.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.715904 geoformat-20230620/tests/
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.815902 geoformat-20230620/tests/data/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/data/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15423 2022-10-13 08:02:35.000000 geoformat-20230620/tests/data/coordinates.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    43859 2023-05-06 10:15:36.000000 geoformat-20230620/tests/data/features.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2394 2022-10-13 08:02:35.000000 geoformat-20230620/tests/data/fields_metadata.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)  9850700 2023-05-06 10:15:36.000000 geoformat-20230620/tests/data/geolayers.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    26450 2023-06-20 11:56:04.000000 geoformat-20230620/tests/data/geometries.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    58422 2022-09-13 14:34:13.000000 geoformat-20230620/tests/data/geometry_index.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1227 2022-10-13 08:02:35.000000 geoformat-20230620/tests/data/index.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      232 2022-09-13 14:34:13.000000 geoformat-20230620/tests/data/matrix.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     5099 2023-01-03 14:30:13.000000 geoformat-20230620/tests/data/metadata.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      435 2022-09-13 14:34:13.000000 geoformat-20230620/tests/data/segments.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.815902 geoformat-20230620/tests/geoformat/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.815902 geoformat-20230620/tests/geoformat/conf/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/conf/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3617 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/conf/test_format_data.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     8633 2023-01-03 14:30:13.000000 geoformat-20230620/tests/geoformat/conf/test_path.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.819902 geoformat-20230620/tests/geoformat/constraints/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/constraints/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2987 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/constraints/test_primary_key.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.859900 geoformat-20230620/tests/geoformat/conversion/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/conversion/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2380 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/conversion/test_bbox_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17731 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/conversion/test_bytes_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17709 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/conversion/test_coordinates_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      986 2023-01-03 14:29:45.000000 geoformat-20230620/tests/geoformat/conversion/test_datetime_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   205565 2023-01-03 14:30:13.000000 geoformat-20230620/tests/geoformat/conversion/test_feature_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   161950 2023-01-03 14:30:13.000000 geoformat-20230620/tests/geoformat/conversion/test_fields_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)  5602810 2022-11-24 15:49:21.000000 geoformat-20230620/tests/geoformat/conversion/test_geolayer_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    92781 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/conversion/test_geometry_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    65479 2023-01-03 14:30:13.000000 geoformat-20230620/tests/geoformat/conversion/test_metadata_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1238 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/conversion/test_precision_tolerance_conversion.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3245 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/conversion/test_segment_conversion.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.859900 geoformat-20230620/tests/geoformat/db/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/db/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.875900 geoformat-20230620/tests/geoformat/driver/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/driver/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.875900 geoformat-20230620/tests/geoformat/driver/ogr/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/driver/ogr/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      369 2023-01-03 14:30:13.000000 geoformat-20230620/tests/geoformat/driver/ogr/compare_ogr_files.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1251 2023-01-03 14:29:45.000000 geoformat-20230620/tests/geoformat/driver/ogr/geolayer_to_geojson.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1263 2023-01-03 14:30:13.000000 geoformat-20230620/tests/geoformat/driver/ogr/geolayer_to_postgresql.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2155 2023-01-03 14:29:45.000000 geoformat-20230620/tests/geoformat/driver/ogr/geolayer_to_shapefile.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    16408 2023-06-20 14:20:52.000000 geoformat-20230620/tests/geoformat/driver/test_common_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    29687 2023-01-03 14:30:13.000000 geoformat-20230620/tests/geoformat/driver/test_csv_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   321121 2023-01-03 14:29:45.000000 geoformat-20230620/tests/geoformat/driver/test_esri_shapefile_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)  1461478 2023-01-03 14:30:13.000000 geoformat-20230620/tests/geoformat/driver/test_geojson_driver.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   114134 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/driver/test_postgresql_driver.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.895900 geoformat-20230620/tests/geoformat/explore_data/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/explore_data/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17339 2023-01-16 19:36:49.000000 geoformat-20230620/tests/geoformat/explore_data/test_duplicate.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    66158 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/explore_data/test_print_data.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.907899 geoformat-20230620/tests/geoformat/geoprocessing/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/geoprocessing/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.907899 geoformat-20230620/tests/geoformat/geoprocessing/connectors/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/geoprocessing/connectors/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4728 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/connectors/test_operations.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15761 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/connectors/test_predicates.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.907899 geoformat-20230620/tests/geoformat/geoprocessing/generalization/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/generalization/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2176 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/generalization/test_ramer_douglas_peucker.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1845 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/generalization/test_visvalingam_whyatt.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.915899 geoformat-20230620/tests/geoformat/geoprocessing/geoparameters/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/geoprocessing/geoparameters/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3562 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/geoparameters/test_bbox.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)      901 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/geoparameters/test_boundaries.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     9425 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/geoparameters/test_lines.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.919899 geoformat-20230620/tests/geoformat/geoprocessing/matrix/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/geoprocessing/matrix/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1645 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/matrix/test_adjacency.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.919899 geoformat-20230620/tests/geoformat/geoprocessing/measure/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/geoprocessing/measure/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2234 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/measure/test_area.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     3736 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/measure/test_distance.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1525 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/measure/test_length.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1758 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/test_area.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     2337 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/test_length.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15898 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/test_line_merge.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4976 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/test_merge_geometries.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     4575 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/test_point_on_linestring.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    14514 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/test_simplify.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    53164 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/test_split.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1387 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/geoprocessing/test_union.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.923899 geoformat-20230620/tests/geoformat/index/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/index/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.935898 geoformat-20230620/tests/geoformat/index/attributes/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/index/attributes/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1279 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/index/attributes/test_hash.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.935898 geoformat-20230620/tests/geoformat/index/geometry/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/index/geometry/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    15928 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/index/geometry/test_grid.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.939898 geoformat-20230620/tests/geoformat/manipulation/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/manipulation/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    12109 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/manipulation/test_feature_manipulation.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   256166 2023-01-03 14:30:13.000000 geoformat-20230620/tests/geoformat/manipulation/test_geolayer_manipulation.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    38639 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/manipulation/test_metadata_manipulation.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.939898 geoformat-20230620/tests/geoformat/obj/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/obj/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1928 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/obj/test_geometry.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.939898 geoformat-20230620/tests/geoformat/processing/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/processing/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.939898 geoformat-20230620/tests/geoformat/processing/data/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/geoformat/processing/data/__init__.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.951898 geoformat-20230620/tests/geoformat/processing/data/join/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/processing/data/join/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)   614826 2023-06-20 15:15:59.000000 geoformat-20230620/tests/geoformat/processing/data/join/test_join.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    20394 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/processing/data/join/test_merge_objects.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6946 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/processing/data/test_clauses.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     7537 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/processing/data/test_field_statistics.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6065 2022-10-13 08:02:35.000000 geoformat-20230620/tests/geoformat/processing/data/test_union.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.951898 geoformat-20230620/tests/inspector/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-09-13 14:34:13.000000 geoformat-20230620/tests/inspector/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    17877 2023-01-03 14:30:13.000000 geoformat-20230620/tests/inspector/geoformat_inspector.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.951898 geoformat-20230620/tests/perf/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230620/tests/perf/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)    10403 2023-01-03 14:30:13.000000 geoformat-20230620/tests/perf/compare_func.py
+drwxrwxr-x   0 guilhain  (1000) guilhain  (1000)        0 2023-06-20 15:18:04.955898 geoformat-20230620/tests/utils/
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)        0 2022-10-13 08:02:35.000000 geoformat-20230620/tests/utils/__init__.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     1379 2023-01-03 14:29:45.000000 geoformat-20230620/tests/utils/compare.py
+-rw-rw-r--   0 guilhain  (1000) guilhain  (1000)     6701 2023-01-03 14:30:13.000000 geoformat-20230620/tests/utils/tests_utils.py
```

### Comparing `geoformat-20230421/LICENSE` & `geoformat-20230620/LICENSE`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/PKG-INFO` & `geoformat-20230620/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoformat
-Version: 20230421
+Version: 20230620
 Summary: Geoformat is a GDAL/OGR library overlayer
 Home-page: https://framagit.org/Guilhain/Geoformat
 Author: Guilhain Averlant
 Author-email: g.averlant@mailfence.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `geoformat-20230421/README.md` & `geoformat-20230620/README.md`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/__init__.py` & `geoformat-20230620/geoformat/__init__.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conf/decorator.py` & `geoformat-20230620/geoformat/conf/decorator.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conf/driver_variable.py` & `geoformat-20230620/geoformat/conf/driver_variable.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conf/error_messages.py` & `geoformat-20230620/geoformat/conf/error_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # path
 path_not_valid = "path : {path} is not valid"
 path_not_a_dir = f"{path_not_valid}, it must be a directory"
 path_not_a_file = f"{path_not_valid}, it must be a file"
 path_not_valid_file_exists_overwrite_is_false = "path : {path} exists."
 path_http_not_valid = "{path} not valid, code : {code}"
 path_not_http = "{path} is not http path"
+path_not_exists = "cannot load data file or http address does not exists"
 
 # fields
 field_missing = "field : {field_name} does not exists."
 field_exists = "{field_name} still exists"
 field_type_not_valid = "field type {field_type} not valid. You must use a type in this list : {field_type_list}"
 field_width_not_valid = "width value for field {field_name} must be specified"
 field_precision_not_valid = "precision value for field {field_name} must be specified"
```

### Comparing `geoformat-20230421/geoformat/conf/fields_variable.py` & `geoformat-20230620/geoformat/conf/fields_variable.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conf/format_data.py` & `geoformat-20230620/geoformat/conf/format_data.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conf/geometry_variable.py` & `geoformat-20230620/geoformat/conf/geometry_variable.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conf/path.py` & `geoformat-20230620/geoformat/conf/path.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conf/proj_var.py` & `geoformat-20230620/geoformat/conf/proj_var.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conf/timer.py` & `geoformat-20230620/geoformat/conf/timer.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/constraints/primary_key.py` & `geoformat-20230620/geoformat/constraints/primary_key.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conversion/bbox_conversion.py` & `geoformat-20230620/geoformat/conversion/bbox_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conversion/bytes_conversion.py` & `geoformat-20230620/geoformat/conversion/bytes_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conversion/coordinates_conversion.py` & `geoformat-20230620/geoformat/conversion/coordinates_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conversion/datetime_conversion.py` & `geoformat-20230620/geoformat/conversion/datetime_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conversion/feature_conversion.py` & `geoformat-20230620/geoformat/conversion/feature_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conversion/fields_conversion.py` & `geoformat-20230620/geoformat/conversion/fields_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conversion/geolayer_conversion.py` & `geoformat-20230620/geoformat/conversion/geolayer_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conversion/geometry_conversion.py` & `geoformat-20230620/geoformat/conversion/geometry_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conversion/metadata_conversion.py` & `geoformat-20230620/geoformat/conversion/metadata_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conversion/precision_tolerance_conversion.py` & `geoformat-20230620/geoformat/conversion/precision_tolerance_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/conversion/segment_conversion.py` & `geoformat-20230620/geoformat/conversion/segment_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/db/db_request.py` & `geoformat-20230620/geoformat/db/db_request.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/driver/common_driver.py` & `geoformat-20230620/geoformat/driver/common_driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import tempfile
 from pathlib import Path
 
 from geoformat.conf.path import (
-    path_to_file_path,
     verify_input_path_is_file,
     verify_input_path_is_http,
     path_is_file,
     path_is_http,
     open_http_path,
 )
-from geoformat.conf.format_data import value_to_iterable_value
+
+from geoformat.conf.error_messages import path_not_exists
 
 def _get_recast_field_type_mapping(fields_metadata, geoformat_type_to_output_driver_type):
     """
     From geolayer field's metadata to output driver recast dict
 
     :param fields_metadata: geolayer field's metadata
     :param geoformat_type_to_output_driver_type: dict that make translation between geoformat type and output driver
@@ -45,29 +45,31 @@
     :param read_mode: data is open in 'r' mode (by default) but you can choose an other parameters ('rb', 'r+b')
     :param temp_mode: data is load in NamedTemporaryFile we can choose writing mode
     :return:
     """
     # create temporary file
     fp = tempfile.NamedTemporaryFile(mode=temp_mode)
 
-    if path_is_file(path=path):
+    if path_is_file(path=path) is True:
         p = verify_input_path_is_file(path=path)
         # open file
         with open(file=p, mode=read_mode, encoding=encoding) as file:
             fp.write(file.read())
 
-    elif path_is_http(path=path, headers=http_headers):
+    elif path_is_http(path=path, headers=http_headers)[0] is True:
         p = verify_input_path_is_http(path=path, headers=http_headers)
         http_req = open_http_path(path=p, headers=http_headers)
         http_req_str = http_req.read()
         if encoding is not None:
             http_req_str = http_req_str.decode(encoding)
         fp.write(http_req_str)
         file_name = http_req.info().get_filename()
         if file_name is None:
             file_name = path.split('/')[-1]
         p = Path(file_name)
+    else:
+        raise Exception(path_not_exists)
 
     fp.seek(0)
 
     file_name = p.stem
     return fp, file_name
```

### Comparing `geoformat-20230421/geoformat/driver/csv_driver.py` & `geoformat-20230620/geoformat/driver/csv_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/driver/esri_shapefile_driver.py` & `geoformat-20230620/geoformat/driver/esri_shapefile_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/driver/geojson_driver.py` & `geoformat-20230620/geoformat/driver/geojson_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/driver/ogr/ogr_driver.py` & `geoformat-20230620/geoformat/driver/ogr/ogr_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/driver/postgresql_driver.py` & `geoformat-20230620/geoformat/driver/postgresql_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/explore_data/duplicate.py` & `geoformat-20230620/geoformat/explore_data/duplicate.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/explore_data/print_data.py` & `geoformat-20230620/geoformat/explore_data/print_data.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/explore_data/random_geometry.py` & `geoformat-20230620/geoformat/explore_data/random_geometry.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/area.py` & `geoformat-20230620/geoformat/geoprocessing/area.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/connectors/operations.py` & `geoformat-20230620/geoformat/geoprocessing/connectors/operations.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/connectors/predicates.py` & `geoformat-20230620/geoformat/geoprocessing/connectors/predicates.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/generalization/ramer_douglas_peucker.py` & `geoformat-20230620/geoformat/geoprocessing/generalization/ramer_douglas_peucker.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/generalization/visvalingam_whyatt.py` & `geoformat-20230620/geoformat/geoprocessing/generalization/visvalingam_whyatt.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/geoparameters/bbox.py` & `geoformat-20230620/geoformat/geoprocessing/geoparameters/bbox.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/geoparameters/boundaries.py` & `geoformat-20230620/geoformat/geoprocessing/geoparameters/boundaries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/geoparameters/lines.py` & `geoformat-20230620/geoformat/geoprocessing/geoparameters/lines.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/length.py` & `geoformat-20230620/geoformat/geoprocessing/length.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/line_merge.py` & `geoformat-20230620/geoformat/geoprocessing/line_merge.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/matrix/adjacency.py` & `geoformat-20230620/geoformat/geoprocessing/matrix/adjacency.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/measure/area.py` & `geoformat-20230620/geoformat/geoprocessing/measure/area.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/measure/distance.py` & `geoformat-20230620/geoformat/geoprocessing/measure/distance.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/measure/length.py` & `geoformat-20230620/geoformat/geoprocessing/measure/length.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/merge_geometries.py` & `geoformat-20230620/geoformat/geoprocessing/merge_geometries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/point_on_linestring.py` & `geoformat-20230620/geoformat/geoprocessing/point_on_linestring.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/simplify.py` & `geoformat-20230620/geoformat/geoprocessing/simplify.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/split.py` & `geoformat-20230620/geoformat/geoprocessing/split.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/geoprocessing/union.py` & `geoformat-20230620/geoformat/geoprocessing/union.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/index/attributes/hash.py` & `geoformat-20230620/geoformat/index/attributes/hash.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/index/geometry/grid.py` & `geoformat-20230620/geoformat/index/geometry/grid.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/manipulation/feature_manipulation.py` & `geoformat-20230620/geoformat/manipulation/feature_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/manipulation/geolayer_manipulation.py` & `geoformat-20230620/geoformat/manipulation/geolayer_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/manipulation/metadata_manipulation.py` & `geoformat-20230620/geoformat/manipulation/metadata_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/obj/geometry.py` & `geoformat-20230620/geoformat/obj/geometry.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/processing/data/clauses.py` & `geoformat-20230620/geoformat/processing/data/clauses.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/processing/data/field_statistics.py` & `geoformat-20230620/geoformat/processing/data/field_statistics.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/processing/data/join/join.py` & `geoformat-20230620/geoformat/processing/data/join/join.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         raise Exception(
             geolayer_attributes_missing.format(
                 geolayer_name=geolayer_a["metadata"]["name"]
             )
         )
 
     if "fields" in geolayer_b["metadata"]:
-        if on_field_a not in geolayer_b["metadata"]["fields"]:
+        if on_field_b not in geolayer_b["metadata"]["fields"]:
             raise Exception(field_missing.format(field_name=on_field_b))
     else:
         raise Exception(
             geolayer_attributes_missing.format(
                 geolayer_name=geolayer_b["metadata"]["name"]
             )
         )
```

### Comparing `geoformat-20230421/geoformat/processing/data/join/merge_objects.py` & `geoformat-20230620/geoformat/processing/data/join/merge_objects.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat/processing/data/union.py` & `geoformat-20230620/geoformat/processing/data/union.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/geoformat.egg-info/PKG-INFO` & `geoformat-20230620/geoformat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoformat
-Version: 20230421
+Version: 20230620
 Summary: Geoformat is a GDAL/OGR library overlayer
 Home-page: https://framagit.org/Guilhain/Geoformat
 Author: Guilhain Averlant
 Author-email: g.averlant@mailfence.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `geoformat-20230421/geoformat.egg-info/SOURCES.txt` & `geoformat-20230620/geoformat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/setup.py` & `geoformat-20230620/setup.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/data/coordinates.py` & `geoformat-20230620/tests/data/coordinates.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/data/features.py` & `geoformat-20230620/tests/data/features.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/data/fields_metadata.py` & `geoformat-20230620/tests/data/fields_metadata.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/data/geolayers.py` & `geoformat-20230620/tests/data/geolayers.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/data/geometries.py` & `geoformat-20230620/tests/data/geometries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/data/geometry_index.py` & `geoformat-20230620/tests/data/geometry_index.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/data/index.py` & `geoformat-20230620/tests/data/index.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/data/metadata.py` & `geoformat-20230620/tests/data/metadata.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conf/test_format_data.py` & `geoformat-20230620/tests/geoformat/conf/test_format_data.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conf/test_path.py` & `geoformat-20230620/tests/geoformat/conf/test_path.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/constraints/test_primary_key.py` & `geoformat-20230620/tests/geoformat/constraints/test_primary_key.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conversion/test_bbox_conversion.py` & `geoformat-20230620/tests/geoformat/conversion/test_bbox_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conversion/test_bytes_conversion.py` & `geoformat-20230620/tests/geoformat/conversion/test_bytes_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conversion/test_coordinates_conversion.py` & `geoformat-20230620/tests/geoformat/conversion/test_coordinates_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conversion/test_datetime_conversion.py` & `geoformat-20230620/tests/geoformat/conversion/test_datetime_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conversion/test_feature_conversion.py` & `geoformat-20230620/tests/geoformat/conversion/test_feature_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conversion/test_fields_conversion.py` & `geoformat-20230620/tests/geoformat/conversion/test_fields_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conversion/test_geolayer_conversion.py` & `geoformat-20230620/tests/geoformat/conversion/test_geolayer_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conversion/test_geometry_conversion.py` & `geoformat-20230620/tests/geoformat/conversion/test_geometry_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conversion/test_metadata_conversion.py` & `geoformat-20230620/tests/geoformat/conversion/test_metadata_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conversion/test_precision_tolerance_conversion.py` & `geoformat-20230620/tests/geoformat/conversion/test_precision_tolerance_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/conversion/test_segment_conversion.py` & `geoformat-20230620/tests/geoformat/conversion/test_segment_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/driver/ogr/geolayer_to_geojson.py` & `geoformat-20230620/tests/geoformat/driver/ogr/geolayer_to_geojson.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/driver/ogr/geolayer_to_postgresql.py` & `geoformat-20230620/tests/geoformat/driver/ogr/geolayer_to_postgresql.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/driver/ogr/geolayer_to_shapefile.py` & `geoformat-20230620/tests/geoformat/driver/ogr/geolayer_to_shapefile.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/driver/test_common_driver.py` & `geoformat-20230620/tests/geoformat/driver/test_common_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,14 +595,20 @@
     }
   ]
 }
 """,
             "loire",
         ),
     },
+    5: {
+        "path": 'foo/bar.csv',
+        "encoding": 'utf8',
+        "http_headers": None,
+        "return_value": 'cannot load data file or http address does not exists'
+    }
 }
 
 
 def test_all():
 
     # load_data
     print(test_function(load_data, load_data_parameters))
```

### Comparing `geoformat-20230421/tests/geoformat/driver/test_csv_driver.py` & `geoformat-20230620/tests/geoformat/driver/test_csv_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/driver/test_esri_shapefile_driver.py` & `geoformat-20230620/tests/geoformat/driver/test_esri_shapefile_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/driver/test_geojson_driver.py` & `geoformat-20230620/tests/geoformat/driver/test_geojson_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/driver/test_postgresql_driver.py` & `geoformat-20230620/tests/geoformat/driver/test_postgresql_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/explore_data/test_duplicate.py` & `geoformat-20230620/tests/geoformat/explore_data/test_duplicate.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/explore_data/test_print_data.py` & `geoformat-20230620/tests/geoformat/explore_data/test_print_data.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/connectors/test_operations.py` & `geoformat-20230620/tests/geoformat/geoprocessing/connectors/test_operations.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/connectors/test_predicates.py` & `geoformat-20230620/tests/geoformat/geoprocessing/connectors/test_predicates.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/generalization/test_ramer_douglas_peucker.py` & `geoformat-20230620/tests/geoformat/geoprocessing/generalization/test_ramer_douglas_peucker.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/generalization/test_visvalingam_whyatt.py` & `geoformat-20230620/tests/geoformat/geoprocessing/generalization/test_visvalingam_whyatt.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/test_bbox.py` & `geoformat-20230620/tests/geoformat/geoprocessing/geoparameters/test_bbox.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/test_boundaries.py` & `geoformat-20230620/tests/geoformat/geoprocessing/geoparameters/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/geoparameters/test_lines.py` & `geoformat-20230620/tests/geoformat/geoprocessing/geoparameters/test_lines.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/matrix/test_adjacency.py` & `geoformat-20230620/tests/geoformat/geoprocessing/matrix/test_adjacency.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/measure/test_area.py` & `geoformat-20230620/tests/geoformat/geoprocessing/measure/test_area.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/measure/test_distance.py` & `geoformat-20230620/tests/geoformat/geoprocessing/measure/test_distance.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/measure/test_length.py` & `geoformat-20230620/tests/geoformat/geoprocessing/measure/test_length.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/test_area.py` & `geoformat-20230620/tests/geoformat/geoprocessing/test_area.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/test_length.py` & `geoformat-20230620/tests/geoformat/geoprocessing/test_length.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/test_line_merge.py` & `geoformat-20230620/tests/geoformat/geoprocessing/test_line_merge.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/test_merge_geometries.py` & `geoformat-20230620/tests/geoformat/geoprocessing/test_merge_geometries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/test_point_on_linestring.py` & `geoformat-20230620/tests/geoformat/geoprocessing/test_point_on_linestring.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/test_simplify.py` & `geoformat-20230620/tests/geoformat/geoprocessing/test_simplify.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/test_split.py` & `geoformat-20230620/tests/geoformat/geoprocessing/test_split.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/geoprocessing/test_union.py` & `geoformat-20230620/tests/geoformat/geoprocessing/test_union.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/index/attributes/test_hash.py` & `geoformat-20230620/tests/geoformat/index/attributes/test_hash.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/index/geometry/test_grid.py` & `geoformat-20230620/tests/geoformat/index/geometry/test_grid.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/manipulation/test_feature_manipulation.py` & `geoformat-20230620/tests/geoformat/manipulation/test_feature_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/manipulation/test_geolayer_manipulation.py` & `geoformat-20230620/tests/geoformat/manipulation/test_geolayer_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/manipulation/test_metadata_manipulation.py` & `geoformat-20230620/tests/geoformat/manipulation/test_metadata_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/obj/test_geometry.py` & `geoformat-20230620/tests/geoformat/obj/test_geometry.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/processing/data/join/test_join.py` & `geoformat-20230620/tests/geoformat/processing/data/join/test_join.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,20 @@
 geolayer_dpt_2_with_geom = feature_list_to_geolayer(
     feature_list=copy.deepcopy(
         [feature_dpt_data_and_geometry_b, feature_dpt_data_and_geometry_c]
     ),
     geolayer_name="geolayer_dpt_2_with_geom",
 )
 
+geolayer_dpt_2_update_field_name_code = feature_list_to_geolayer(
+    feature_list=copy.deepcopy([feature_dpt_data_only_b, feature_dpt_data_only_c]),
+    geolayer_name="geolayer_dpt_2",
+)
+geolayer_dpt_2_update_field_name_code = geoformat.rename_field(geolayer=geolayer_dpt_2_update_field_name_code, old_field_name='CODE_DEPT', new_field_name='code')
+
 geolayer_dpt_pop_full = feature_list_to_geolayer(
     feature_list=copy.deepcopy(
         [
             feature_dpt_population_a,
             feature_dpt_population_b,
             feature_dpt_population_c,
             feature_dpt_population_d,
@@ -3197,14 +3203,54 @@
                         "DENSITY": 979.62,
                     }
                 },
             },
         },
     },
     7: {
+        "geolayer_a": geolayer_dpt_2_update_field_name_code,
+        "geolayer_b": geolayer_dpt_pop_full,
+        "on_field_a": "code",
+        "on_field_b": "CODE_DEPT",
+        "output_geolayer_name": "FRANCE_DPT_2_LEFT_JOIN_POP_FULL",
+        "field_name_filter_a": ["code", "NOM_DEPT"],
+        "field_name_filter_b": ["POPULATION", "DENSITY"],
+        "rename_output_field_from_geolayer_a": {"code": "CODE_DEPT"},
+        "rename_output_field_from_geolayer_b": "auto",
+        "return_value": {
+            "metadata": {
+                "name": "FRANCE_DPT_2_LEFT_JOIN_POP_FULL",
+                "fields": {
+                    "CODE_DEPT": {"type": "String", "width": 2, "index": 0},
+                    "NOM_DEPT": {"type": "String", "width": 10, "index": 1},
+                    "POPULATION": {"type": "Integer", "index": 2},
+                    "DENSITY": {"type": "Real", "width": 5, "precision": 2, "index": 3},
+                },
+            },
+            "features": {
+                0: {
+                    "attributes": {
+                        "CODE_DEPT": "02",
+                        "NOM_DEPT": "AISNE",
+                        "POPULATION": 534490,
+                        "DENSITY": 72.04,
+                    }
+                },
+                1: {
+                    "attributes": {
+                        "CODE_DEPT": "95",
+                        "NOM_DEPT": "VAL-D'OISE",
+                        "POPULATION": 1228618,
+                        "DENSITY": 979.62,
+                    }
+                },
+            },
+        },
+    },
+    8: {
         "geolayer_a": geolayer_dpt_2,
         "geolayer_b": geolayer_dpt_pop_full_with_duplicate,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_LEFT_JOIN_POP_FULL_WITH_DUPLICATE",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -3244,15 +3290,15 @@
                         "POPULATION": 1228618,
                         "DENSITY": 979.62,
                     }
                 },
             },
         },
     },
-    8: {
+    9: {
         "geolayer_a": geolayer_dpt_2,
         "geolayer_b": geolayer_dpt_pop_2,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_JOIN_POP_2",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -3267,15 +3313,15 @@
                     "POPULATION": {"type": "Integer", "index": 2},
                     "DENSITY": {"type": "Real", "width": 5, "precision": 2, "index": 3},
                 },
             },
             "features": {},
         },
     },
-    9: {
+    10: {
         "geolayer_a": geolayer_dpt_2_with_geom,
         "geolayer_b": geolayer_dpt_pop_full,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_JOIN_POP_FULL",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -3410,15 +3456,15 @@
                         ],
                         "bbox": (598361.0, 6867928.0, 670084.0, 6904387.0),
                     },
                 },
             },
         },
     },
-    10: {
+    11: {
         "geolayer_a": geolayer_dpt_2_with_geom,
         "geolayer_b": geolayer_dpt_pop_full,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_JOIN_POP_FULL",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -3451,15 +3497,15 @@
                         "POPULATION": 1228618,
                         "DENSITY": 979.62,
                     }
                 },
             },
         },
     },
-    11: {
+    12: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2_with_geom,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_JOIN_POP_FULL",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -3594,15 +3640,15 @@
                         ],
                         "bbox": (598361.0, 6867928.0, 670084.0, 6904387.0),
                     },
                 },
             },
         },
     },
-    12: {
+    13: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2_with_geom,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_JOIN_POP_FULL",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -3737,15 +3783,15 @@
                         ],
                         "bbox": (598361.0, 6867928.0, 670084.0, 6904387.0),
                     },
                 },
             },
         },
     },
-    13: {
+    14: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2_with_geom,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_JOIN_POP_FULL",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -3753,15 +3799,15 @@
             "CODE_DEPT": "code",
             "POPULATION": "pop",
         },
         "rename_output_field_from_geolayer_b": "auto",
         "geometry_ref": "geolayer_b",
         "return_value": field_missing.format(field_name="CODE_DEPT"),
     },
-    14: {
+    15: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "key_id": {"type": "Integer", "index": 0},
                     "price": {"type": "Integer", "index": 1},
                     "count": {"type": "Integer", "index": 2},
@@ -3867,15 +3913,15 @@
                         "count_b": 1,
                         "probability_b": 0.1,
                     }
                 }
             },
         },
     },
-    15: {
+    16: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "id": {"type": "Integer", "index": 0},
                     "name": {"type": "String", "width": 7, "index": 1},
                 },
@@ -3920,15 +3966,15 @@
             },
             "features": {
                 0: {"attributes": {"id": 0, "name": "Alice", "id1": 0, "age": 28}},
                 1: {"attributes": {"id": 1, "name": "Jane", "id1": 1, "age": 2}},
             },
         },
     },
-    16: {
+    17: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "id": {"type": "Integer", "index": 0},
                     "name": {"type": "String", "width": 5, "index": 1},
                 },
@@ -3973,15 +4019,15 @@
             },
             "features": {
                 0: {"attributes": {"id": 0, "name": "Alice", "id1": 0, "age": 28}},
                 1: {"attributes": {"id": 1, "name": "Jane", "id1": 1, "age": 2}},
             },
         },
     },
-    17: {
+    18: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "id": {"type": "Integer", "index": 0},
                     "name": {"type": "String", "width": 7, "index": 1},
                 },
@@ -7135,14 +7181,54 @@
                         "DENSITY": 979.62,
                     }
                 },
             },
         },
     },
     7: {
+        "geolayer_a": geolayer_dpt_2_update_field_name_code,
+        "geolayer_b": geolayer_dpt_pop_full,
+        "on_field_a": "code",
+        "on_field_b": "CODE_DEPT",
+        "output_geolayer_name": "FRANCE_DPT_2_LEFT_JOIN_POP_FULL",
+        "field_name_filter_a": ["code", "NOM_DEPT"],
+        "field_name_filter_b": ["POPULATION", "DENSITY"],
+        "rename_output_field_from_geolayer_a": {"code": "CODE_DEPT"},
+        "rename_output_field_from_geolayer_b": "auto",
+        "return_value": {
+            "metadata": {
+                "name": "FRANCE_DPT_2_LEFT_JOIN_POP_FULL",
+                "fields": {
+                    "CODE_DEPT": {"type": "String", "width": 2, "index": 0},
+                    "NOM_DEPT": {"type": "String", "width": 10, "index": 1},
+                    "POPULATION": {"type": "Integer", "index": 2},
+                    "DENSITY": {"type": "Real", "width": 5, "precision": 2, "index": 3},
+                },
+            },
+            "features": {
+                0: {
+                    "attributes": {
+                        "CODE_DEPT": "02",
+                        "NOM_DEPT": "AISNE",
+                        "POPULATION": 534490,
+                        "DENSITY": 72.04,
+                    }
+                },
+                1: {
+                    "attributes": {
+                        "CODE_DEPT": "95",
+                        "NOM_DEPT": "VAL-D'OISE",
+                        "POPULATION": 1228618,
+                        "DENSITY": 979.62,
+                    }
+                },
+            },
+        },
+    },
+    8: {
         "geolayer_a": geolayer_dpt_2,
         "geolayer_b": geolayer_dpt_pop_full_with_duplicate,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_LEFT_JOIN_POP_FULL_WITH_DUPLICATE",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -7182,15 +7268,15 @@
                         "POPULATION": 1228618,
                         "DENSITY": 979.62,
                     }
                 },
             },
         },
     },
-    8: {
+    9: {
         "geolayer_a": geolayer_dpt_2,
         "geolayer_b": geolayer_dpt_pop_2,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_LEFT_JOIN_POP_2",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -7208,15 +7294,15 @@
             },
             "features": {
                 0: {"attributes": {"CODE_DEPT": "02", "NOM_DEPT": "AISNE"}},
                 1: {"attributes": {"CODE_DEPT": "95", "NOM_DEPT": "VAL-D'OISE"}},
             },
         },
     },
-    9: {
+    10: {
         "geolayer_a": geolayer_dpt_2_with_geom,
         "geolayer_b": geolayer_dpt_pop_full,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_LEFT_JOIN_POP_FULL",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -7351,15 +7437,15 @@
                         ],
                         "bbox": (598361.0, 6867928.0, 670084.0, 6904387.0),
                     },
                 },
             },
         },
     },
-    10: {
+    11: {
         "geolayer_a": geolayer_dpt_2_with_geom,
         "geolayer_b": geolayer_dpt_pop_full,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_LEFT_JOIN_POP_FULL",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -7392,15 +7478,15 @@
                         "POPULATION": 1228618,
                         "DENSITY": 979.62,
                     }
                 },
             },
         },
     },
-    11: {
+    12: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2_with_geom,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_LEFT_JOIN_POP_FULL",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -7537,15 +7623,15 @@
                         "bbox": (598361.0, 6867928.0, 670084.0, 6904387.0),
                     },
                 },
                 3: {"attributes": {"POPULATION": 750863, "DENSITY": 109.39}},
             },
         },
     },
-    12: {
+    13: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2_with_geom,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_LEFT_JOIN_POP_FULL",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -7682,15 +7768,15 @@
                         "bbox": (598361.0, 6867928.0, 670084.0, 6904387.0),
                     },
                 },
                 3: {"attributes": {"DENSITY": 109.39, "pop": 750863}},
             },
         },
     },
-    13: {
+    14: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2_with_geom,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_LEFT_JOIN_POP_FULL",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -7698,15 +7784,15 @@
             "CODE_DEPT": "code",
             "POPULATION": "pop",
         },
         "rename_output_field_from_geolayer_b": "auto",
         "geometry_ref": "geolayer_b",
         "return_value": field_missing.format(field_name="CODE_DEPT"),
     },
-    14: {
+    15: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "key_id": {"type": "Integer", "index": 0},
                     "price": {"type": "Integer", "index": 1},
                     "count": {"type": "Integer", "index": 2},
@@ -7812,15 +7898,15 @@
                         "count_b": 1,
                         "probability_b": 0.1,
                     }
                 }
             },
         },
     },
-    15: {
+    16: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "id": {"type": "Integer", "index": 0},
                     "name": {"type": "String", "width": 7, "index": 1},
                 },
@@ -7867,15 +7953,15 @@
                 0: {"attributes": {"id": 0, "name": "Alice", "id1": 0, "age": 28}},
                 1: {"attributes": {"id": None, "name": "Bob"}},
                 2: {"attributes": {"id": None, "name": "Patrick"}},
                 3: {"attributes": {"id": 1, "name": "Jane", "id1": 1, "age": 2}},
             },
         },
     },
-    16: {
+    17: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "id": {"type": "Integer", "index": 0},
                     "name": {"type": "String", "width": 5, "index": 1},
                 },
@@ -7920,15 +8006,15 @@
             },
             "features": {
                 0: {"attributes": {"id": 0, "name": "Alice", "id1": 0, "age": 28}},
                 1: {"attributes": {"id": 1, "name": "Jane", "id1": 1, "age": 2}},
             },
         },
     },
-    17: {
+    18: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "id": {"type": "Integer", "index": 0},
                     "name": {"type": "String", "width": 7, "index": 1},
                 },
@@ -11050,16 +11136,16 @@
                 },
             },
         },
     },
     6: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2,
-        "on_field_b": "CODE_DEPT",
         "on_field_a": "CODE_DEPT",
+        "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "dpt_pop_ful_right_join_dpt_2",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
         "rename_output_field_from_geolayer_a": "auto",
         "rename_output_field_from_geolayer_b": "auto",
         "return_value": {
             "metadata": {
@@ -11088,14 +11174,54 @@
                         "DENSITY": 979.62,
                     }
                 },
             },
         },
     },
     7: {
+        "geolayer_a": geolayer_dpt_pop_full,
+        "geolayer_b": geolayer_dpt_2_update_field_name_code,
+        "on_field_a": "CODE_DEPT",
+        "on_field_b": "code",
+        "output_geolayer_name": "dpt_pop_ful_right_join_dpt_2",
+        "field_name_filter_a": ["CODE_DEPT", "POPULATION", "DENSITY"],
+        "field_name_filter_b": ["NOM_DEPT"],
+        "rename_output_field_from_geolayer_a": "auto",
+        "rename_output_field_from_geolayer_b": "auto",
+        "return_value": {
+            "metadata": {
+                "name": "dpt_pop_ful_right_join_dpt_2",
+                "fields": {
+                    "CODE_DEPT": {"type": "String", "width": 2, "index": 0},
+                    "POPULATION": {"type": "Integer", "index": 1},
+                    "DENSITY": {"type": "Real", "width": 5, "precision": 2, "index": 2},
+                    "NOM_DEPT": {"type": "String", "width": 10, "index": 3},
+                },
+            },
+            "features": {
+                0: {
+                    "attributes": {
+                        "CODE_DEPT": "02",
+                        "NOM_DEPT": "AISNE",
+                        "POPULATION": 534490,
+                        "DENSITY": 72.04,
+                    }
+                },
+                1: {
+                    "attributes": {
+                        "CODE_DEPT": "95",
+                        "NOM_DEPT": "VAL-D'OISE",
+                        "POPULATION": 1228618,
+                        "DENSITY": 979.62,
+                    }
+                },
+            },
+        },
+    },
+    8: {
         "geolayer_a": geolayer_dpt_pop_full_with_duplicate,
         "geolayer_b": geolayer_dpt_2,
         "on_field_b": "CODE_DEPT",
         "on_field_a": "CODE_DEPT",
         "output_geolayer_name": "dpt_pop_full_with_duplicate_right_join_dpt_2",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -11135,15 +11261,15 @@
                         "POPULATION": 1228618,
                         "DENSITY": 979.62,
                     }
                 },
             },
         },
     },
-    8: {
+    9: {
         "geolayer_a": geolayer_dpt_pop_2,
         "geolayer_b": geolayer_dpt_2,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_RIGHT_JOIN_POP_2",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -11161,15 +11287,15 @@
             },
             "features": {
                 0: {"attributes": {"CODE_DEPT": "02", "NOM_DEPT": "AISNE"}},
                 1: {"attributes": {"CODE_DEPT": "95", "NOM_DEPT": "VAL-D'OISE"}},
             },
         },
     },
-    9: {
+    10: {
         "geolayer_a": geolayer_dpt_2_with_geom,
         "geolayer_b": geolayer_dpt_pop_full,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_RIGHT_JOIN_POP_FULL",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -11306,15 +11432,15 @@
                         "bbox": (598361.0, 6867928.0, 670084.0, 6904387.0),
                     },
                 },
                 3: {"attributes": {"POPULATION": 750863, "DENSITY": 109.39}},
             },
         },
     },
-    10: {
+    11: {
         "geolayer_a": geolayer_dpt_2_with_geom,
         "geolayer_b": geolayer_dpt_pop_full,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_RIGHT_JOIN_POP_FULL",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -11349,15 +11475,15 @@
                         "DENSITY": 979.62,
                     },
                 },
                 3: {"attributes": {"POPULATION": 750863, "DENSITY": 109.39}},
             },
         },
     },
-    11: {
+    12: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2_with_geom,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_RIGHT_JOIN_POP_FULL",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -11492,15 +11618,15 @@
                         ],
                         "bbox": (598361.0, 6867928.0, 670084.0, 6904387.0),
                     },
                 },
             },
         },
     },
-    12: {
+    13: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2_with_geom,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_RIGHT_JOIN_POP_FULL",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -11635,15 +11761,15 @@
                         ],
                         "bbox": (598361.0, 6867928.0, 670084.0, 6904387.0),
                     },
                 },
             },
         },
     },
-    13: {
+    14: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2_with_geom,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_RIGHT_JOIN_POP_FULL",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -11651,15 +11777,15 @@
             "CODE_DEPT": "code",
             "POPULATION": "pop",
         },
         "rename_output_field_from_geolayer_b": "auto",
         "geometry_ref": "geolayer_b",
         "return_value": field_missing.format(field_name="CODE_DEPT"),
     },
-    14: {
+    15: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "key_id": {"type": "Integer", "index": 0},
                     "price": {"type": "Integer", "index": 1},
                     "count": {"type": "Integer", "index": 2},
@@ -11773,15 +11899,15 @@
                         "count_b": 1,
                         "probability_b": 0.1,
                     }
                 },
             },
         },
     },
-    15: {
+    16: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "id": {"type": "Integer", "index": 0},
                     "name": {"type": "String", "width": 7, "index": 1},
                 },
@@ -11826,15 +11952,15 @@
             },
             "features": {
                 0: {"attributes": {"id": 0, "name": "Alice", "id1": 0, "age": 28}},
                 1: {"attributes": {"id": 1, "name": "Jane", "id1": 1, "age": 2}},
             },
         },
     },
-    16: {
+    17: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "id": {"type": "Integer", "index": 0},
                     "name": {"type": "String", "width": 5, "index": 1},
                 },
@@ -11881,15 +12007,15 @@
                 0: {"attributes": {"id": 0, "name": "Alice", "id1": 0, "age": 28}},
                 1: {"attributes": {"id1": None, "age": 67}},
                 2: {"attributes": {"id1": None, "age": 15}},
                 3: {"attributes": {"id": 1, "name": "Jane", "id1": 1, "age": 2}},
             },
         },
     },
-    17: {
+    18: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "id": {"type": "Integer", "index": 0},
                     "name": {"type": "String", "width": 7, "index": 1},
                 },
@@ -15047,14 +15173,56 @@
                     }
                 },
                 3: {"attributes": {"POPULATION": 750863, "DENSITY": 109.39}},
             },
         },
     },
     7: {
+        "geolayer_a": geolayer_dpt_2_update_field_name_code,
+        "geolayer_b": geolayer_dpt_pop_full,
+        "on_field_a": "code",
+        "on_field_b": "CODE_DEPT",
+        "output_geolayer_name": "FRANCE_DPT_2_FULL_JOIN_POP_FULL",
+        "field_name_filter_a": ["code", "NOM_DEPT"],
+        "field_name_filter_b": ["POPULATION", "DENSITY"],
+        "rename_output_field_from_geolayer_a": {"code": "CODE_DEPT"},
+        "rename_output_field_from_geolayer_b": "auto",
+        "return_value": {
+            "metadata": {
+                "name": "FRANCE_DPT_2_FULL_JOIN_POP_FULL",
+                "fields": {
+                    "CODE_DEPT": {"type": "String", "width": 2, "index": 0},
+                    "NOM_DEPT": {"type": "String", "width": 10, "index": 1},
+                    "POPULATION": {"type": "Integer", "index": 2},
+                    "DENSITY": {"type": "Real", "width": 5, "precision": 2, "index": 3},
+                },
+            },
+            "features": {
+                0: {"attributes": {"POPULATION": 307445, "DENSITY": 59.03}},
+                1: {
+                    "attributes": {
+                        "CODE_DEPT": "02",
+                        "NOM_DEPT": "AISNE",
+                        "POPULATION": 534490,
+                        "DENSITY": 72.04,
+                    }
+                },
+                2: {
+                    "attributes": {
+                        "CODE_DEPT": "95",
+                        "NOM_DEPT": "VAL-D'OISE",
+                        "POPULATION": 1228618,
+                        "DENSITY": 979.62,
+                    }
+                },
+                3: {"attributes": {"POPULATION": 750863, "DENSITY": 109.39}},
+            },
+        },
+    },
+    8: {
         "geolayer_a": geolayer_dpt_2,
         "geolayer_b": geolayer_dpt_pop_full_with_duplicate,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_FULL_JOIN_POP_FULL_WITH_DUPLICATE",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -15097,15 +15265,15 @@
                     }
                 },
                 4: {"attributes": {"POPULATION": 750863, "DENSITY": 109.39}},
                 5: {"attributes": {"POPULATION": 750863, "DENSITY": 109.39}},
             },
         },
     },
-    8: {
+    9: {
         "geolayer_a": geolayer_dpt_2,
         "geolayer_b": geolayer_dpt_pop_2,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_FULL_JOIN_POP_2",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -15125,15 +15293,15 @@
                 0: {"attributes": {"CODE_DEPT": "02", "NOM_DEPT": "AISNE"}},
                 1: {"attributes": {"CODE_DEPT": "95", "NOM_DEPT": "VAL-D'OISE"}},
                 2: {"attributes": {"POPULATION": 307445, "DENSITY": 59.03}},
                 3: {"attributes": {"POPULATION": 750863, "DENSITY": 109.39}},
             },
         },
     },
-    9: {
+    10: {
         "geolayer_a": geolayer_dpt_2_with_geom,
         "geolayer_b": geolayer_dpt_pop_full,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_FULL_JOIN_POP_FULL",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -15270,15 +15438,15 @@
                         "bbox": (598361.0, 6867928.0, 670084.0, 6904387.0),
                     },
                 },
                 3: {"attributes": {"POPULATION": 750863, "DENSITY": 109.39}},
             },
         },
     },
-    10: {
+    11: {
         "geolayer_a": geolayer_dpt_2_with_geom,
         "geolayer_b": geolayer_dpt_pop_full,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_FULL_JOIN_POP_FULL",
         "field_name_filter_a": ["CODE_DEPT", "NOM_DEPT"],
         "field_name_filter_b": ["POPULATION", "DENSITY"],
@@ -15313,15 +15481,15 @@
                         "DENSITY": 979.62,
                     },
                 },
                 3: {"attributes": {"POPULATION": 750863, "DENSITY": 109.39}},
             },
         },
     },
-    11: {
+    12: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2_with_geom,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_FULL_JOIN_POP_FULL",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -15458,15 +15626,15 @@
                         "bbox": (598361.0, 6867928.0, 670084.0, 6904387.0),
                     },
                 },
                 3: {"attributes": {"POPULATION": 750863, "DENSITY": 109.39}},
             },
         },
     },
-    12: {
+    13: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2_with_geom,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_FULL_JOIN_POP_FULL",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -15603,15 +15771,15 @@
                         "bbox": (598361.0, 6867928.0, 670084.0, 6904387.0),
                     },
                 },
                 3: {"attributes": {"DENSITY": 109.39, "pop": 750863}},
             },
         },
     },
-    13: {
+    14: {
         "geolayer_a": geolayer_dpt_pop_full,
         "geolayer_b": geolayer_dpt_2_with_geom,
         "on_field_a": "CODE_DEPT",
         "on_field_b": "CODE_DEPT",
         "output_geolayer_name": "FRANCE_DPT_2_WITH_GEOM_FULL_JOIN_POP_FULL",
         "field_name_filter_a": ["POPULATION", "DENSITY"],
         "field_name_filter_b": ["CODE_DEPT", "NOM_DEPT"],
@@ -15619,15 +15787,15 @@
             "CODE_DEPT": "code",
             "POPULATION": "pop",
         },
         "rename_output_field_from_geolayer_b": "auto",
         "geometry_ref": "geolayer_b",
         "return_value": field_missing.format(field_name="CODE_DEPT"),
     },
-    14: {
+    15: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "key_id": {"type": "Integer", "index": 0},
                     "price": {"type": "Integer", "index": 1},
                     "count": {"type": "Integer", "index": 2},
@@ -15741,15 +15909,15 @@
                         "count_b": 1,
                         "probability_b": 0.1,
                     }
                 },
             },
         },
     },
-    15: {
+    16: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "id": {"type": "Integer", "index": 0},
                     "name": {"type": "String", "width": 7, "index": 1},
                 },
@@ -15796,15 +15964,15 @@
                 0: {"attributes": {"id": 0, "name": "Alice", "id1": 0, "age": 28}},
                 1: {"attributes": {"id": None, "name": "Bob"}},
                 2: {"attributes": {"id": None, "name": "Patrick"}},
                 3: {"attributes": {"id": 1, "name": "Jane", "id1": 1, "age": 2}},
             },
         },
     },
-    16: {
+    17: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "id": {"type": "Integer", "index": 0},
                     "name": {"type": "String", "width": 5, "index": 1},
                 },
@@ -15851,15 +16019,15 @@
                 0: {"attributes": {"id": 0, "name": "Alice", "id1": 0, "age": 28}},
                 1: {"attributes": {"id1": None, "age": 67}},
                 2: {"attributes": {"id1": None, "age": 15}},
                 3: {"attributes": {"id": 1, "name": "Jane", "id1": 1, "age": 2}},
             },
         },
     },
-    17: {
+    18: {
         "geolayer_a": {
             "metadata": {
                 "name": "geolayer_a",
                 "fields": {
                     "id": {"type": "Integer", "index": 0},
                     "name": {"type": "String", "width": 7, "index": 1},
                 },
```

### Comparing `geoformat-20230421/tests/geoformat/processing/data/join/test_merge_objects.py` & `geoformat-20230620/tests/geoformat/processing/data/join/test_merge_objects.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/processing/data/test_clauses.py` & `geoformat-20230620/tests/geoformat/processing/data/test_clauses.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/processing/data/test_field_statistics.py` & `geoformat-20230620/tests/geoformat/processing/data/test_field_statistics.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/geoformat/processing/data/test_union.py` & `geoformat-20230620/tests/geoformat/processing/data/test_union.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/inspector/geoformat_inspector.py` & `geoformat-20230620/tests/inspector/geoformat_inspector.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/perf/compare_func.py` & `geoformat-20230620/tests/perf/compare_func.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/utils/compare.py` & `geoformat-20230620/tests/utils/compare.py`

 * *Files identical despite different names*

### Comparing `geoformat-20230421/tests/utils/tests_utils.py` & `geoformat-20230620/tests/utils/tests_utils.py`

 * *Files identical despite different names*

