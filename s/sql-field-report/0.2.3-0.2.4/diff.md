# Comparing `tmp/sql_field_report-0.2.3.tar.gz` & `tmp/sql_field_report-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_field_report-0.2.3.tar", max compression
+gzip compressed data, was "sql_field_report-0.2.4.tar", max compression
```

## Comparing `sql_field_report-0.2.3.tar` & `sql_field_report-0.2.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      737 2023-06-12 10:03:03.243946 sql_field_report-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.2.3/README.md
--rw-r--r--   0        0        0      116 2023-06-12 09:54:08.238167 sql_field_report-0.2.3/sql_field_report/__init__.py
--rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-0.2.3/sql_field_report/__main__.py
--rw-r--r--   0        0        0     4069 2023-06-12 10:03:44.017730 sql_field_report-0.2.3/sql_field_report/sql_field_report.py
--rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-0.2.3/sql_field_report/utils/__init__.py
--rw-r--r--   0        0        0     6919 2023-06-12 09:54:08.250421 sql_field_report-0.2.3/sql_field_report/utils/analysis.py
--rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-0.2.3/sql_field_report/utils/databases.py
--rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-0.2.3/sql_field_report/utils/excel.py
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 sql_field_report-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      717 2023-06-20 16:59:24.080891 sql_field_report-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.2.4/README.md
+-rw-r--r--   0        0        0      116 2023-06-12 09:54:08.238167 sql_field_report-0.2.4/sql_field_report/__init__.py
+-rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-0.2.4/sql_field_report/__main__.py
+-rw-r--r--   0        0        0     4069 2023-06-12 10:03:44.017730 sql_field_report-0.2.4/sql_field_report/sql_field_report.py
+-rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-0.2.4/sql_field_report/utils/__init__.py
+-rw-r--r--   0        0        0     6919 2023-06-12 09:54:08.250421 sql_field_report-0.2.4/sql_field_report/utils/analysis.py
+-rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-0.2.4/sql_field_report/utils/databases.py
+-rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-0.2.4/sql_field_report/utils/excel.py
+-rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 sql_field_report-0.2.4/PKG-INFO
```

### Comparing `sql_field_report-0.2.3/pyproject.toml` & `sql_field_report-0.2.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [tool.poetry]
 name = "sql-field-report"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["Will James <willj@dealcloud.com>"]
 readme = "README.md"
 packages = [{include = "sql_field_report"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.8"
 pandas = "^1.5.3"
 openpyxl = "^3.1.2"
 sqlalchemy = "^2.0.11"
 python-dotenv = "^1.0.0"
 regex = "^2023.3.23"
 pyodbc = "^4.0.39"
 typer = {extras = ["all"], version = "^0.7.0"}
 coloredlogs = "^15.0.1"
 mysql-connector-python = "^8.0.33"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
-isort = "^5.12.0"
 
 [tool.poetry.scripts]
 sql-field-report = "sql_field_report.sql_field_report:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sql_field_report-0.2.3/README.md` & `sql_field_report-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.2.3/sql_field_report/sql_field_report.py` & `sql_field_report-0.2.4/sql_field_report/sql_field_report.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.2.3/sql_field_report/utils/analysis.py` & `sql_field_report-0.2.4/sql_field_report/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.2.3/sql_field_report/utils/databases.py` & `sql_field_report-0.2.4/sql_field_report/utils/databases.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.2.3/sql_field_report/utils/excel.py` & `sql_field_report-0.2.4/sql_field_report/utils/excel.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.2.3/PKG-INFO` & `sql_field_report-0.2.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: sql-field-report
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: Will James
 Author-email: willj@dealcloud.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: mysql-connector-python (>=8.0.33,<9.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pyodbc (>=4.0.39,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
```

