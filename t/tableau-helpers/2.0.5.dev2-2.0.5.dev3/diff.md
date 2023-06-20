# Comparing `tmp/tableau-helpers-2.0.5.dev2.tar.gz` & `tmp/tableau-helpers-2.0.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau-helpers-2.0.5.dev2.tar", last modified: Tue Jun 20 13:35:07 2023, max compression
+gzip compressed data, was "tableau-helpers-2.0.5.dev3.tar", last modified: Tue Jun 20 14:29:08 2023, max compression
```

## Comparing `tableau-helpers-2.0.5.dev2.tar` & `tableau-helpers-2.0.5.dev3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.930075 tableau-helpers-2.0.5.dev2/
--rw-rw-rw-   0        0        0      122 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev2/.env.sample
--rw-rw-rw-   0        0        0       54 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev2/.flake8
--rw-rw-rw-   0        0        0      376 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev2/.gitignore
--rw-rw-rw-   0        0        0      463 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev2/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1088 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev2/LICENSE
--rw-rw-rw-   0        0        0     1893 2023-06-20 13:35:06.930075 tableau-helpers-2.0.5.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     1617 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev2/README.md
--rw-rw-rw-   0        0        0     1053 2023-06-20 12:54:09.000000 tableau-helpers-2.0.5.dev2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 13:35:06.934938 tableau-helpers-2.0.5.dev2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.623025 tableau-helpers-2.0.5.dev2/tableau_helpers/
--rw-rw-rw-   0        0        0      191 2023-06-19 16:08:17.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.719275 tableau-helpers-2.0.5.dev2/tableau_helpers/cli/
--rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/cli/__init__.py
--rw-rw-rw-   0        0        0     2876 2023-06-19 15:59:19.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/cli/csv_to_hyper.py
--rw-rw-rw-   0        0        0     1141 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/cli/upload_hyper.py
--rw-rw-rw-   0        0        0     7726 2023-06-19 14:05:36.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/hyper.py
--rw-rw-rw-   0        0        0     8008 2023-06-06 16:49:39.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/server.py
--rw-rw-rw-   0        0        0      700 2023-06-19 16:00:21.000000 tableau-helpers-2.0.5.dev2/tableau_helpers/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.685529 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/
--rw-rw-rw-   0        0        0     1893 2023-06-20 13:35:05.000000 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1045 2023-06-20 13:35:06.000000 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 13:35:05.000000 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-06-20 13:35:05.000000 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      146 2023-06-20 13:35:05.000000 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-20 13:35:05.000000 tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.781778 tableau-helpers-2.0.5.dev2/tests/
--rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.813029 tableau-helpers-2.0.5.dev2/tests/cli/
--rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev2/tests/cli/__init__.py
--rw-rw-rw-   0        0        0      880 2023-06-06 16:03:33.000000 tableau-helpers-2.0.5.dev2/tests/cli/test_csv_to_hyper.py
--rw-rw-rw-   0        0        0      730 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev2/tests/cli/test_upload_hyper.py
--rw-rw-rw-   0        0        0     1836 2023-06-12 12:44:15.000000 tableau-helpers-2.0.5.dev2/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-06-20 13:35:06.914237 tableau-helpers-2.0.5.dev2/tests/resources/
--rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_default_format.csv
--rw-rw-rw-   0        0        0    65536 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_default_format.hyper
--rw-rw-rw-   0        0        0       34 2023-06-06 15:42:19.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_default_format.tab
--rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_default_format2.csv
--rw-rw-rw-   0        0        0      378 2023-06-09 15:46:22.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_default_format_table_def.json
--rw-rw-rw-   0        0        0      887 2023-06-12 12:33:02.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_join_table_def.json
--rw-rw-rw-   0        0        0       52 2023-06-12 10:42:48.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_left.csv
--rw-rw-rw-   0        0        0       56 2023-06-12 10:43:02.000000 tableau-helpers-2.0.5.dev2/tests/resources/good_right.csv
--rw-rw-rw-   0        0        0    65536 2023-06-12 12:41:14.000000 tableau-helpers-2.0.5.dev2/tests/resources/joined.hyper
--rw-rw-rw-   0        0        0     3886 2023-06-12 12:44:37.000000 tableau-helpers-2.0.5.dev2/tests/test_hyper.py
--rw-rw-rw-   0        0        0     1128 2023-06-12 12:43:43.000000 tableau-helpers-2.0.5.dev2/tests/test_server.py
--rw-rw-rw-   0        0        0      591 2023-06-12 09:09:36.000000 tableau-helpers-2.0.5.dev2/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.260014 tableau-helpers-2.0.5.dev3/
+-rw-rw-rw-   0        0        0      122 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev3/.env.sample
+-rw-rw-rw-   0        0        0       54 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev3/.flake8
+-rw-rw-rw-   0        0        0      376 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev3/.gitignore
+-rw-rw-rw-   0        0        0      463 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev3/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1088 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev3/LICENSE
+-rw-rw-rw-   0        0        0     1893 2023-06-20 14:29:08.260014 tableau-helpers-2.0.5.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0     1617 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev3/README.md
+-rw-rw-rw-   0        0        0     1053 2023-06-20 12:54:09.000000 tableau-helpers-2.0.5.dev3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:29:08.260014 tableau-helpers-2.0.5.dev3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.049145 tableau-helpers-2.0.5.dev3/tableau_helpers/
+-rw-rw-rw-   0        0        0      191 2023-06-20 14:25:15.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.117853 tableau-helpers-2.0.5.dev3/tableau_helpers/cli/
+-rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/cli/__init__.py
+-rw-rw-rw-   0        0        0     2559 2023-06-20 14:27:44.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/cli/csv_to_hyper.py
+-rw-rw-rw-   0        0        0     1141 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/cli/upload_hyper.py
+-rw-rw-rw-   0        0        0     7726 2023-06-19 14:05:36.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/hyper.py
+-rw-rw-rw-   0        0        0     8008 2023-06-06 16:49:39.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/server.py
+-rw-rw-rw-   0        0        0     1146 2023-06-20 14:25:19.000000 tableau-helpers-2.0.5.dev3/tableau_helpers/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.102228 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/
+-rw-rw-rw-   0        0        0     1893 2023-06-20 14:29:07.000000 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2023-06-20 14:29:07.000000 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:29:07.000000 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-06-20 14:29:07.000000 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      146 2023-06-20 14:29:07.000000 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-20 14:29:07.000000 tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.149105 tableau-helpers-2.0.5.dev3/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.180601 tableau-helpers-2.0.5.dev3/tests/cli/
+-rw-rw-rw-   0        0        0        0 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev3/tests/cli/__init__.py
+-rw-rw-rw-   0        0        0      880 2023-06-06 16:03:33.000000 tableau-helpers-2.0.5.dev3/tests/cli/test_csv_to_hyper.py
+-rw-rw-rw-   0        0        0      730 2023-06-05 17:29:26.000000 tableau-helpers-2.0.5.dev3/tests/cli/test_upload_hyper.py
+-rw-rw-rw-   0        0        0     1836 2023-06-12 12:44:15.000000 tableau-helpers-2.0.5.dev3/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:29:08.260014 tableau-helpers-2.0.5.dev3/tests/resources/
+-rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_default_format.csv
+-rw-rw-rw-   0        0        0    65536 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_default_format.hyper
+-rw-rw-rw-   0        0        0       34 2023-06-06 15:42:19.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_default_format.tab
+-rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_default_format2.csv
+-rw-rw-rw-   0        0        0      378 2023-06-09 15:46:22.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_default_format_table_def.json
+-rw-rw-rw-   0        0        0      887 2023-06-12 12:33:02.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_join_table_def.json
+-rw-rw-rw-   0        0        0       52 2023-06-12 10:42:48.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_left.csv
+-rw-rw-rw-   0        0        0       56 2023-06-12 10:43:02.000000 tableau-helpers-2.0.5.dev3/tests/resources/good_right.csv
+-rw-rw-rw-   0        0        0    65536 2023-06-12 12:41:14.000000 tableau-helpers-2.0.5.dev3/tests/resources/joined.hyper
+-rw-rw-rw-   0        0        0     3886 2023-06-12 12:44:37.000000 tableau-helpers-2.0.5.dev3/tests/test_hyper.py
+-rw-rw-rw-   0        0        0     1128 2023-06-12 12:43:43.000000 tableau-helpers-2.0.5.dev3/tests/test_server.py
+-rw-rw-rw-   0        0        0      591 2023-06-12 09:09:36.000000 tableau-helpers-2.0.5.dev3/tox.ini
```

### Comparing `tableau-helpers-2.0.5.dev2/LICENSE` & `tableau-helpers-2.0.5.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/PKG-INFO` & `tableau-helpers-2.0.5.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau-helpers
-Version: 2.0.5.dev2
+Version: 2.0.5.dev3
 Summary: A collection of helpers to reduce boilerplate with Tableau APIs.
 License: MIT License
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `tableau-helpers-2.0.5.dev2/README.md` & `tableau-helpers-2.0.5.dev3/README.md`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/pyproject.toml` & `tableau-helpers-2.0.5.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tableau_helpers/cli/csv_to_hyper.py` & `tableau-helpers-2.0.5.dev3/tableau_helpers/cli/csv_to_hyper.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,38 +9,23 @@
 tempdir = tempfile.TemporaryDirectory()
 
 
 def literal(value: str) -> str:
     return value.encode().decode("unicode_escape")
 
 
-def path_or_url(arg: Union[Path, str]) -> Path:
-    result = arg
-    if isinstance(arg, Path):
-        result = arg
-    if isinstance(arg, str):
-        if arg.startswith("https://"):
-            result = utils.download_file(Path(tempdir.name), arg)
-        else:
-            result = Path(arg)
-    else:
-        raise TypeError
-
-    return utils.try_unzip(result)
-
-
 def _parse_args(args):
     description = (
         "csv_to_hyper creates a hyperfile with Tableau's hyperapi given a csv and"
         " table-definition"
     )
     parser = argparse.ArgumentParser(description=description)
     parser.add_argument(
         "--csv",
-        type=path_or_url,
+        type=utils.path_or_url,
         required=True,
         nargs="+",
         help="Provide the CSV to be copied with the hyperapi.",
     )
     parser.add_argument(
         "--table-def",
         type=Path,
@@ -87,14 +72,15 @@
         help="Specify the encoding type of your csv.",
     )
     return parser.parse_args(args)
 
 
 def main(args):
     args = _parse_args(args)
+    args.csv = [utils.try_unzip(csv) for csv in args.csv]
     table_definition = hyper.load_table_defs(args.table_def)
     hyper.copy_csv_to_hyper(
         args.dest,
         args.csv,
         table_definition,
         delimiter=args.delimiter,
         header=args.header,
```

### Comparing `tableau-helpers-2.0.5.dev2/tableau_helpers/cli/upload_hyper.py` & `tableau-helpers-2.0.5.dev3/tableau_helpers/cli/upload_hyper.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tableau_helpers/hyper.py` & `tableau-helpers-2.0.5.dev3/tableau_helpers/hyper.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tableau_helpers/server.py` & `tableau-helpers-2.0.5.dev3/tableau_helpers/server.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/PKG-INFO` & `tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau-helpers
-Version: 2.0.5.dev2
+Version: 2.0.5.dev3
 Summary: A collection of helpers to reduce boilerplate with Tableau APIs.
 License: MIT License
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `tableau-helpers-2.0.5.dev2/tableau_helpers.egg-info/SOURCES.txt` & `tableau-helpers-2.0.5.dev3/tableau_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tests/cli/test_csv_to_hyper.py` & `tableau-helpers-2.0.5.dev3/tests/cli/test_csv_to_hyper.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tests/cli/test_upload_hyper.py` & `tableau-helpers-2.0.5.dev3/tests/cli/test_upload_hyper.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tests/conftest.py` & `tableau-helpers-2.0.5.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tests/resources/good_default_format.hyper` & `tableau-helpers-2.0.5.dev3/tests/resources/good_default_format.hyper`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tests/resources/good_join_table_def.json` & `tableau-helpers-2.0.5.dev3/tests/resources/good_join_table_def.json`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tests/resources/joined.hyper` & `tableau-helpers-2.0.5.dev3/tests/resources/joined.hyper`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tests/test_hyper.py` & `tableau-helpers-2.0.5.dev3/tests/test_hyper.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tests/test_server.py` & `tableau-helpers-2.0.5.dev3/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev2/tox.ini` & `tableau-helpers-2.0.5.dev3/tox.ini`

 * *Files identical despite different names*

