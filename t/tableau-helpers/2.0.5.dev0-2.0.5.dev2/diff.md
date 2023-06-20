# Comparing `tmp/tableau-helpers-2.0.5.dev0.tar.gz` & `tmp/tableau-helpers-2.0.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau-helpers-2.0.5.dev0.tar", last modified: Tue Jun  6 14:31:49 2023, max compression
+gzip compressed data, was "tableau-helpers-2.0.5.dev2.tar", last modified: Tue Jun 20 13:35:07 2023, max compression
```

## Comparing `tableau-helpers-2.0.5.dev0.tar` & `tableau-helpers-2.0.5.dev2.tar`

### file list

```diff
@@ -1,40 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.864135 tableau-helpers-2.0.5.dev0/
--rw-rw-rw-   0        0        0      122 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev0/.env.sample
--rw-rw-rw-   0        0        0       54 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev0/.flake8
--rw-rw-rw-   0        0        0      376 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev0/.gitignore
--rw-rw-rw-   0        0        0      463 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1088 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev0/LICENSE
--rw-rw-rw-   0        0        0     1920 2023-06-06 14:31:49.862130 tableau-helpers-2.0.5.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     1617 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev0/README.md
--rw-rw-rw-   0        0        0     1023 2023-06-06 14:31:27.000000 tableau-helpers-2.0.5.dev0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 14:31:49.864135 tableau-helpers-2.0.5.dev0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.780126 tableau-helpers-2.0.5.dev0/tableau_helpers/
--rw-rw-rw-   0        0        0      182 2023-06-06 14:09:21.000000 tableau-helpers-2.0.5.dev0/tableau_helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.813125 tableau-helpers-2.0.5.dev0/tableau_helpers/cli/
--rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tableau_helpers/cli/__init__.py
--rw-rw-rw-   0        0        0     2280 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tableau_helpers/cli/csv_to_hyper.py
--rw-rw-rw-   0        0        0     1141 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tableau_helpers/cli/upload_hyper.py
--rw-rw-rw-   0        0        0     7149 2023-06-05 17:29:10.000000 tableau-helpers-2.0.5.dev0/tableau_helpers/hyper.py
--rw-rw-rw-   0        0        0     8008 2023-06-05 17:29:18.000000 tableau-helpers-2.0.5.dev0/tableau_helpers/server.py
-drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.801123 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/
--rw-rw-rw-   0        0        0     1920 2023-06-06 14:31:49.000000 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2023-06-06 14:31:49.000000 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 14:31:49.000000 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-06-06 14:31:49.000000 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      126 2023-06-06 14:31:49.000000 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 14:31:49.000000 tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.827124 tableau-helpers-2.0.5.dev0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.838122 tableau-helpers-2.0.5.dev0/tests/cli/
--rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tests/cli/__init__.py
--rw-rw-rw-   0        0        0      483 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tests/cli/test_csv_to_hyper.py
--rw-rw-rw-   0        0        0      730 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev0/tests/cli/test_upload_hyper.py
--rw-rw-rw-   0        0        0     1365 2023-06-05 17:29:10.000000 tableau-helpers-2.0.5.dev0/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-06-06 14:31:49.858125 tableau-helpers-2.0.5.dev0/tests/resources/
--rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev0/tests/resources/good_default_format.csv
--rw-rw-rw-   0        0        0    65536 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev0/tests/resources/good_default_format.hyper
--rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev0/tests/resources/good_default_format2.csv
--rw-rw-rw-   0        0        0      332 2023-06-05 17:28:41.000000 tableau-helpers-2.0.5.dev0/tests/resources/good_default_format_table_def.json
--rw-rw-rw-   0        0        0     3181 2023-06-05 17:29:10.000000 tableau-helpers-2.0.5.dev0/tests/test_hyper.py
--rw-rw-rw-   0        0        0      905 2023-06-05 17:29:10.000000 tableau-helpers-2.0.5.dev0/tests/test_server.py
--rw-rw-rw-   0        0        0      503 2023-06-05 17:29:22.000000 tableau-helpers-2.0.5.dev0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.930075 tableau-helpers-2.0.5.dev2/
+-rw-rw-rw-   0        0        0      122 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev2/.env.sample
+-rw-rw-rw-   0        0        0       54 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev2/.flake8
+-rw-rw-rw-   0        0        0      376 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev2/.gitignore
+-rw-rw-rw-   0        0        0      463 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev2/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1088 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev2/LICENSE
+-rw-rw-rw-   0        0        0     1893 2023-06-20 13:35:06.930075 tableau-helpers-2.0.5.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0     1617 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev2/README.md
+-rw-rw-rw-   0        0        0     1053 2023-06-20 12:54:09.000000 tableau-helpers-2.0.5.dev2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 13:35:06.934938 tableau-helpers-2.0.5.dev2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.623025 tableau-helpers-2.0.5.dev2/tableau_helpers/
+-rw-rw-rw-   0        0        0      191 2023-06-19 16:08:17.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.719275 tableau-helpers-2.0.5.dev2/tableau_helpers/cli/
+-rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/cli/__init__.py
+-rw-rw-rw-   0        0        0     2876 2023-06-19 15:59:19.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/cli/csv_to_hyper.py
+-rw-rw-rw-   0        0        0     1141 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/cli/upload_hyper.py
+-rw-rw-rw-   0        0        0     7726 2023-06-19 14:05:36.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/hyper.py
+-rw-rw-rw-   0        0        0     8008 2023-06-06 16:49:39.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/server.py
+-rw-rw-rw-   0        0        0      700 2023-06-19 16:00:21.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.685529 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/
+-rw-rw-rw-   0        0        0     1893 2023-06-20 13:35:05.000000 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2023-06-20 13:35:06.000000 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:35:05.000000 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-06-20 13:35:05.000000 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      146 2023-06-20 13:35:05.000000 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-20 13:35:05.000000 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.781778 tableau-helpers-2.0.5.dev2/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.813029 tableau-helpers-2.0.5.dev2/tests/cli/
+-rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev2/tests/cli/__init__.py
+-rw-rw-rw-   0        0        0      880 2023-06-06 16:03:33.000000 tableau-helpers-2.0.5.dev2/tests/cli/test_csv_to_hyper.py
+-rw-rw-rw-   0        0        0      730 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev2/tests/cli/test_upload_hyper.py
+-rw-rw-rw-   0        0        0     1836 2023-06-12 12:44:15.000000 tableau-helpers-2.0.5.dev2/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.914237 tableau-helpers-2.0.5.dev2/tests/resources/
+-rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_default_format.csv
+-rw-rw-rw-   0        0        0    65536 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_default_format.hyper
+-rw-rw-rw-   0        0        0       34 2023-06-06 15:42:19.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_default_format.tab
+-rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_default_format2.csv
+-rw-rw-rw-   0        0        0      378 2023-06-09 15:46:22.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_default_format_table_def.json
+-rw-rw-rw-   0        0        0      887 2023-06-12 12:33:02.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_join_table_def.json
+-rw-rw-rw-   0        0        0       52 2023-06-12 10:42:48.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_left.csv
+-rw-rw-rw-   0        0        0       56 2023-06-12 10:43:02.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_right.csv
+-rw-rw-rw-   0        0        0    65536 2023-06-12 12:41:14.000000 tableau-helpers-2.0.5.dev2/tests/resources/joined.hyper
+-rw-rw-rw-   0        0        0     3886 2023-06-12 12:44:37.000000 tableau-helpers-2.0.5.dev2/tests/test_hyper.py
+-rw-rw-rw-   0        0        0     1128 2023-06-12 12:43:43.000000 tableau-helpers-2.0.5.dev2/tests/test_server.py
+-rw-rw-rw-   0        0        0      591 2023-06-12 09:09:36.000000 tableau-helpers-2.0.5.dev2/tox.ini
```

### Comparing `tableau-helpers-2.0.5.dev0/LICENSE` & `tableau-helpers-2.0.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev0/PKG-INFO` & `tableau-helpers-2.0.5.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tableau-helpers
-Version: 2.0.5.dev0
+Version: 2.0.5.dev2
 Summary: A collection of helpers to reduce boilerplate with Tableau APIs.
 License: MIT License
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: sys-certs
 License-File: LICENSE
 
 # tableau_helpers
 
 A wrapper for the tableau-server-client and hyper-api which abstracts away
 boilerplate and in some cases provides a CLI which works without admin privileges.
```

### Comparing `tableau-helpers-2.0.5.dev0/README.md` & `tableau-helpers-2.0.5.dev2/README.md`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev0/pyproject.toml` & `tableau-helpers-2.0.5.dev2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -5,39 +5,38 @@
 [project]
 name="tableau-helpers"
 description="A collection of helpers to reduce boilerplate with Tableau APIs."
 readme="README.md"
 requires-python = ">=3.4"
 license={text="MIT License"}
 dependencies = [
-    "tableauhyperapi>=0.0.14109",
-    "tableauserverclient>=0.17.0",
+    "tableauhyperapi>=0.0.17002",
+    "tableauserverclient>=0.25.0",
     "python-dotenv",
+    "pip-system-certs>=4.0; platform_system=='Windows'"
 ]
 dynamic = ["version"]
 
 [project.scripts]
 csv-to-hyper = "tableau_helpers.cli.csv_to_hyper:entry_point"
 upload-hyper = "tableau_helpers.cli.upload_hyper:entry_point"
 
 [tool.setuptools.dynamic]
 version ={attr = "tableau_helpers.__version__"}
 
 [tool.setuptools.packages.find]
 include = ["tableau_helpers*"]
-exclude = ["tests*"]
+exclude = ["tableau_helpers.tests*"]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pylint"
 ]
 
-sys-certs = [ "pip-system-certs>=4.0" ]
-
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 markers = [
     "integration: integration tests which require a tableau-server",
 ]
```

### Comparing `tableau-helpers-2.0.5.dev0/tableau_helpers/cli/upload_hyper.py` & `tableau-helpers-2.0.5.dev2/tableau_helpers/cli/upload_hyper.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev0/tableau_helpers/hyper.py` & `tableau-helpers-2.0.5.dev2/tableau_helpers/hyper.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,18 +45,18 @@
         sql_with += f", FORCE_NOT_NULL ({','.join(force_not_null)})"
     if force_null is not None:
         sql_with += f", FORCE_NULL ({','.join(force_null)})"
     sql_with += ")"
     return sql_with
 
 
-def load_table_def(table_conf_file: Path) -> TableDefinition:
+def load_table_defs(table_conf_file: Path) -> list[TableDefinition]:
     with open(table_conf_file) as file:
-        table_conf = json.load(file)
-    return parse_table_definition(table_conf)
+        table_confs = json.load(file)
+    return [parse_table_definition(table_conf) for table_conf in table_confs]
 
 
 def parse_columns(columns: dict) -> Iterable[TableDefinition.Column]:
     for col in columns:
         name = col.get("name", None)
         if not name:
             raise ValueError("No name was provided for a column.")
@@ -80,21 +80,26 @@
 
 
 def parse_table_definition(tableconf: dict) -> TableDefinition:
     table_name = tableconf.get("table_name", None)
     columns = tableconf.get("columns", [])
     columns = parse_columns(columns)
     table_def = TableDefinition(TableName(table_name), columns)
+    constraints = tableconf.get("constraints")
+    if constraints is not None:
+        if isinstance(constraints, str):
+            constraints = [constraints]
+        table_def.th_alterations = [f"ALTER TABLE \"{table_name}\" ADD {x}" for x in constraints]
     return table_def
 
 
 def copy_csv_to_hyper(
     save_path: Path,
     csv: Union[Path, list[Path]],
-    schema: TableDefinition,
+    schema: Union[TableDefinition, list[TableDefinition]],
     delimiter: str = ",",
     null: str = "",
     encoding: str = "utf-8",
     on_cast_failure: str = "error",
     header: bool = False,
     quote: str = '"',
     escape: Optional[str] = None,
@@ -127,45 +132,47 @@
         against the null string, even if it has been quoted,
         and if a match is found set the value to NULL.
         In the default case where the null string is empty,
         this converts a quoted empty string into NULL.
     :return: the count of rows written to the hyper file,
         otherwise None
     """  # noqa
-    sql_from: str = f"COPY {schema.table_name} "
+    sql_commands: list[str] = []
+    alterations: list[str] = []
 
+    if isinstance(csv, str):
+        raise TypeError("str instead of Path object passed as csv")
     if isinstance(csv, Path):
-        if not csv.exists():
-            raise FileNotFoundError(str(csv))
-        sql_from += f"FROM {escape_string_literal(str(csv))}"
-    elif isinstance(csv, list):
-        if len(csv) < 1:
-            raise ValueError
-        for x in csv:
-            if not isinstance(x, Path):
-                raise TypeError
-            if not x.exists():
-                raise FileNotFoundError(str(x))
-        escaped_paths = [escape_string_literal(str(x)) for x in csv]
-        sql_from += f"FROM ARRAY[{','.join(escaped_paths)}]"
-    else:
-        raise TypeError
-
-    sql_with = _gen_sql_for_with_csv(
-        delimiter=delimiter,
-        null=null,
-        encoding=encoding,
-        on_cast_failure=on_cast_failure,
-        header=header,
-        quote=quote,
-        escape=escape,
-        force_not_null=force_not_null,
-        force_null=force_null,
-    )
-    sql_command = f"{sql_from} {sql_with}"
+        csv = [csv]
+    if isinstance(schema, TableDefinition):
+        schema = [schema]
+    for c, s in zip(csv, schema):
+        if not c.exists():
+            raise FileNotFoundError(str(c))
+        sql_from = f"COPY {s.table_name} "
+        sql_from += f"FROM {escape_string_literal(str(c))}"
+
+        sql_with = _gen_sql_for_with_csv(
+            delimiter=delimiter,
+            null=null,
+            encoding=encoding,
+            on_cast_failure=on_cast_failure,
+            header=header,
+            quote=quote,
+            escape=escape,
+            force_not_null=force_not_null,
+            force_null=force_null,
+        )
+        sql_commands.append(f"{sql_from} {sql_with}")
+        try:
+            if s.th_alterations is not None:
+                [alterations.append(x) for x in s.th_alterations]
+        except:
+            pass
+
 
     process_parameters = {}
     log_file_max_count = os.getenv("TABLEAU_HYPERAPI_LOG_FILE_MAX_COUNT", "3")
     process_parameters["log_file_max_count"] = log_file_max_count
     log_file_size_limit = os.getenv("TABLEAU_HYPERAPI_LOG_FILE_SIZE_LIMIT", "100M")
     process_parameters["log_file_size_limit"] = log_file_size_limit
     log_dir = os.getenv("TABLEAU_HYPERAPI_LOG_DIR", None)
@@ -177,10 +184,14 @@
         parameters=process_parameters,
     ) as hyper_process:
         with Connection(
             endpoint=hyper_process.endpoint,
             database=save_path,
             create_mode=CreateMode.CREATE_AND_REPLACE,
         ) as connection:
-            connection.catalog.create_table(table_definition=schema)
-            rowcount = connection.execute_command(sql_command)
+            rowcount = 0
+            for s, command in zip(schema, sql_commands):
+                connection.catalog.create_table(table_definition=s)
+                rowcount += connection.execute_command(command)
+            for command in alterations:
+                connection.execute_command(command)
             return rowcount
```

### Comparing `tableau-helpers-2.0.5.dev0/tableau_helpers/server.py` & `tableau-helpers-2.0.5.dev2/tableau_helpers/server.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/PKG-INFO` & `tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tableau-helpers
-Version: 2.0.5.dev0
+Version: 2.0.5.dev2
 Summary: A collection of helpers to reduce boilerplate with Tableau APIs.
 License: MIT License
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: sys-certs
 License-File: LICENSE
 
 # tableau_helpers
 
 A wrapper for the tableau-server-client and hyper-api which abstracts away
 boilerplate and in some cases provides a CLI which works without admin privileges.
```

### Comparing `tableau-helpers-2.0.5.dev0/tableau_helpers.egg-info/SOURCES.txt` & `tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 LICENSE
 README.md
 pyproject.toml
 tox.ini
 tableau_helpers/__init__.py
 tableau_helpers/hyper.py
 tableau_helpers/server.py
+tableau_helpers/utils.py
 tableau_helpers.egg-info/PKG-INFO
 tableau_helpers.egg-info/SOURCES.txt
 tableau_helpers.egg-info/dependency_links.txt
 tableau_helpers.egg-info/entry_points.txt
 tableau_helpers.egg-info/requires.txt
 tableau_helpers.egg-info/top_level.txt
 tableau_helpers/cli/__init__.py
@@ -23,9 +24,14 @@
 tests/test_hyper.py
 tests/test_server.py
 tests/cli/__init__.py
 tests/cli/test_csv_to_hyper.py
 tests/cli/test_upload_hyper.py
 tests/resources/good_default_format.csv
 tests/resources/good_default_format.hyper
+tests/resources/good_default_format.tab
 tests/resources/good_default_format2.csv
-tests/resources/good_default_format_table_def.json
+tests/resources/good_default_format_table_def.json
+tests/resources/good_join_table_def.json
+tests/resources/good_left.csv
+tests/resources/good_right.csv
+tests/resources/joined.hyper
```

### Comparing `tableau-helpers-2.0.5.dev0/tests/cli/test_upload_hyper.py` & `tableau-helpers-2.0.5.dev2/tests/cli/test_upload_hyper.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev0/tests/resources/good_default_format.hyper` & `tableau-helpers-2.0.5.dev2/tests/resources/good_default_format.hyper`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev0/tests/test_server.py` & `tableau-helpers-2.0.5.dev2/tests/test_server.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,11 +24,17 @@
 @pytest.mark.integration
 def test_create_or_replace_hyperfile(good_hyper_path=Path(ct.good_hyper_path())):
     helper = ServerHelper()
     helper.create_or_replace_hyper_file(good_hyper_path, "ApiTest", "test-data")
 
 
 @pytest.mark.integration
+def test_create_or_replace_joined_hyperfile(hyper_path=Path(ct.joined_hyper_path())):
+    helper = ServerHelper()
+    helper.create_or_replace_hyper_file(hyper_path, "ApiTest", "test-data")
+
+
+@pytest.mark.integration
 def test_get_flow_by_name():
     helper = ServerHelper()
     flow: FlowItem = helper.get_flow("ApiTest", "New Flow")
     assert flow is not None
```

