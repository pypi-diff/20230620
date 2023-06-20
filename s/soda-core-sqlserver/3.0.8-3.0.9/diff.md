# Comparing `tmp/soda-core-sqlserver-3.0.8.tar.gz` & `tmp/soda-core-sqlserver-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-sqlserver-3.0.8.tar", last modified: Wed Sep 21 19:42:04 2022, max compression
+gzip compressed data, was "soda-core-sqlserver-3.0.9.tar", last modified: Tue Sep 27 20:20:14 2022, max compression
```

## Comparing `soda-core-sqlserver-3.0.8.tar` & `soda-core-sqlserver-3.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:42:04.983366 soda-core-sqlserver-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-21 19:42:04.983366 soda-core-sqlserver-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:42:04.983366 soda-core-sqlserver-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-09-21 19:41:14.000000 soda-core-sqlserver-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:42:04.983366 soda-core-sqlserver-3.0.8/soda/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:42:04.983366 soda-core-sqlserver-3.0.8/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (121)    11887 2022-09-21 19:41:14.000000 soda-core-sqlserver-3.0.8/soda/data_sources/sqlserver_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:42:04.983366 soda-core-sqlserver-3.0.8/soda_core_sqlserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-21 19:42:04.000000 soda-core-sqlserver-3.0.8/soda_core_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-09-21 19:42:04.000000 soda-core-sqlserver-3.0.8/soda_core_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:42:04.000000 soda-core-sqlserver-3.0.8/soda_core_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-09-21 19:42:04.000000 soda-core-sqlserver-3.0.8/soda_core_sqlserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-21 19:42:04.000000 soda-core-sqlserver-3.0.8/soda_core_sqlserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:14.676273 soda-core-sqlserver-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-27 20:20:14.676273 soda-core-sqlserver-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:20:14.676273 soda-core-sqlserver-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-09-27 20:19:27.000000 soda-core-sqlserver-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:14.676273 soda-core-sqlserver-3.0.9/soda/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:14.676273 soda-core-sqlserver-3.0.9/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)    12018 2022-09-27 20:19:27.000000 soda-core-sqlserver-3.0.9/soda/data_sources/sqlserver_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:14.676273 soda-core-sqlserver-3.0.9/soda_core_sqlserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-27 20:20:14.000000 soda-core-sqlserver-3.0.9/soda_core_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-09-27 20:20:14.000000 soda-core-sqlserver-3.0.9/soda_core_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:20:14.000000 soda-core-sqlserver-3.0.9/soda_core_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-09-27 20:20:14.000000 soda-core-sqlserver-3.0.9/soda_core_sqlserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-27 20:20:14.000000 soda-core-sqlserver-3.0.9/soda_core_sqlserver.egg-info/top_level.txt
```

### Comparing `soda-core-sqlserver-3.0.8/setup.py` & `soda-core-sqlserver-3.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda SQL requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-sqlserver"
-package_version = "3.0.8"
+package_version = "3.0.9"
 description = "Soda Core SQL Server Package"
 
 requires = [
     f"soda-core=={package_version}",
     "pyodbc",
 ]
 # TODO Fix the params
```

### Comparing `soda-core-sqlserver-3.0.8/soda/data_sources/sqlserver_data_source.py` & `soda-core-sqlserver-3.0.9/soda/data_sources/sqlserver_data_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -262,20 +262,25 @@
             FROM {qualified_table_name}
             """
         )
 
     def expr_regexp_like(self, expr: str, regex_pattern: str):
         return f"PATINDEX ('%{regex_pattern}%' ,{expr} ) = 0"
 
-    def sql_select_all(self, table_name: str, limit: int | None = None) -> str:
+    def sql_select_all(self, table_name: str, limit: int | None = None, filter: str | None = None) -> str:
         qualified_table_name = self.qualified_table_name(table_name)
+
+        filter_sql = ""
+        if filter:
+            filter_sql = f" \n WHERE {filter}"
+
         limit_sql = ""
         if limit is not None:
             limit_sql = f" \n TOP {limit} \n"
-        sql = f"SELECT {limit_sql} * FROM {qualified_table_name}"
+        sql = f"SELECT {limit_sql} * FROM {qualified_table_name}{filter_sql}"
         return sql
 
     def sql_select_column_with_filter_and_limit(
         self, column_name: str, table_name: str, filter_clause: str, limit: int | None = None
     ) -> str:
 
         sql = f"SELECT TOP {limit} \n" f" {column_name} \n" f"FROM {table_name}{filter_clause}"
```

