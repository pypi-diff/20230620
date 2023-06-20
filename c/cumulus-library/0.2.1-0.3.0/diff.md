# Comparing `tmp/cumulus_library-0.2.1.tar.gz` & `tmp/cumulus_library-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-0.2.1.tar` & `cumulus_library-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,51 @@
-lrwxr-xr-x   0        0        0        0 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/.sqlfluff -> cumulus_library/.sqlfluff
--rw-r--r--   0        0        0      421 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/README.md
--rw-r--r--   0        0        0      822 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0        0 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/__init__.py
--rw-r--r--   0        0        0      628 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/base_runner.py
--rwxr-xr-x   0        0        0    12415 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/cli.py
--rw-r--r--   0        0        0      190 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/errors.py
--rw-r--r--   0        0        0     1502 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/helper.py
--rw-r--r--   0        0        0      205 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/module_allowlist.json
--rw-r--r--   0        0        0        0 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4843 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     3322 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/schema/counts.py
--rw-r--r--   0        0        0     3364 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     5868 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0     2982 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/condition.sql
--rw-r--r--   0        0        0     2867 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/documentreference.sql
--rw-r--r--   0        0        0     3402 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/encounter.sql
--rw-r--r--   0        0        0     4146 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/fhir_define.sql
--rw-r--r--   0        0        0      615 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     1241 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/medication_request.sql
--rw-r--r--   0        0        0     2884 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/observation_lab.sql
--rw-r--r--   0        0        0     1701 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/patient.sql
--rw-r--r--   0        0        0     2241 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/patient_extensions.py
--rw-r--r--   0        0        0     1436 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     1472 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0      834 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     1562 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1152 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0 26867633 2023-06-01 19:47:52.284538 cumulus_library-0.2.1/cumulus_library/studies/vocab/ICD10.bsv
--rw-r--r--   0        0        0  2988766 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/studies/vocab/ICD9.bsv
--rw-r--r--   0        0        0      404 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      138 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0     4834 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    16000 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/study_parser.py
--rw-r--r--   0        0        0      610 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0       61 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0     1800 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/extension_denormalize.sql.jinja
--rw-r--r--   0        0        0      370 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0       52 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0       54 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0     5866 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/templates.py
--rw-r--r--   0        0        0     1566 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 cumulus_library-0.2.1/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      421 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/README.md
+-rw-r--r--   0        0        0      866 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0        0 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/base_runner.py
+-rwxr-xr-x   0        0        0    10545 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/cli.py
+-rw-r--r--   0        0        0     5129 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/cli_parser.py
+-rw-r--r--   0        0        0      190 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/errors.py
+-rw-r--r--   0        0        0     1889 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/helper.py
+-rw-r--r--   0        0        0      205 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0     2343 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/parsers/fhir_valueset.py
+-rw-r--r--   0        0        0        0 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4848 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3346 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/schema/counts.py
+-rw-r--r--   0        0        0     3364 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     5876 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0     2982 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/condition.sql
+-rw-r--r--   0        0        0     2867 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/documentreference.sql
+-rw-r--r--   0        0        0     3402 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/encounter.sql
+-rw-r--r--   0        0        0     4146 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/fhir_define.sql
+-rw-r--r--   0        0        0      673 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1241 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/medication_request.sql
+-rw-r--r--   0        0        0     1208 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/observation.sql
+-rw-r--r--   0        0        0     2884 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/observation_lab.sql
+-rw-r--r--   0        0        0     1272 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/observation_vital_signs.sql
+-rw-r--r--   0        0        0     1701 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/patient.sql
+-rw-r--r--   0        0        0     2241 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/patient_extensions.py
+-rw-r--r--   0        0        0     1436 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     1472 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0      834 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     1562 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1152 2023-06-20 19:33:36.969362 cumulus_library-0.3.0/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0 26867633 2023-06-20 19:33:37.045363 cumulus_library-0.3.0/cumulus_library/studies/vocab/ICD10.bsv
+-rw-r--r--   0        0        0  2988766 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/studies/vocab/ICD9.bsv
+-rw-r--r--   0        0        0      404 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      138 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0     4834 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    16090 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0      577 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/create_view_as.sql.jinja
+-rw-r--r--   0        0        0      610 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0       61 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     1800 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      370 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0       52 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0       54 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0     6517 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/template_sql/templates.py
+-rw-r--r--   0        0        0     2618 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/cumulus_library/upload.py
+-rw-r--r--   0        0        0     1586 2023-06-20 19:33:37.057363 cumulus_library-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 cumulus_library-0.3.0/PKG-INFO
```

### Comparing `cumulus_library-0.2.1/cumulus_library/.sqlfluff` & `cumulus_library-0.3.0/cumulus_library/.sqlfluff`

 * *Files 11% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 
 [sqlfluff:rules:capitalisation.keywords]
 capitalisation_policy = upper
 
 [sqlfluff:templater:jinja:context]
 schema_name = test_schema
 table_name = test_table
+view_name = test_view
 view_or_table_name = test_view_or_table
 view_or_table = TABLE
 prefix = Test
 dataset = [["foo","foo"],["bar","bar"]]
 table_cols = ["a","b"]
+view_cols = ["c","d"]
 col_type_list = ["a string","b string"]
 source_table = source_table
 source_id = source_id
 target_table = target_table
 target_col_prefix = prefix
 fhir_extension = fhir_extension
 code_systems = ["omb", "text"]
```

### Comparing `cumulus_library-0.2.1/cumulus_library/base_runner.py` & `cumulus_library-0.3.0/cumulus_library/base_runner.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/cli.py` & `cumulus_library-0.3.0/cumulus_library/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python3
 """Utility for building/retrieving data views in AWS Athena"""
 
-import argparse
 import json
 import os
 import sys
 import sysconfig
 
 from pathlib import Path, PosixPath
 from typing import Dict, List, Optional
 
 import pyathena
 
 from pyathena.pandas.cursor import PandasCursor
 
+from cumulus_library.cli_parser import get_parser
 from cumulus_library.study_parser import StudyManifestParser
+from cumulus_library.upload import upload_files
 
 
 # ** Don't delete! **
 # This class isn't used in the rest of the code,
 # but it is used manually as a quick & dirty alternative to the CLI.
 class CumulusEnv:  # pylint: disable=too-few-public-methods
     """
@@ -57,29 +58,48 @@
             work_group=workgroup,
             profile_name=profile,
             schema_name=schema,
             cursor_class=PandasCursor,
         ).cursor()
         self.schema_name = schema
 
-    def reset_export_dir(self, study: PosixPath) -> None:
+    def reset_data_path(self, study: PosixPath) -> None:
         """
         Removes existing exports from a study's local data dir
         """
         project_path = Path(__file__).resolve().parents[1]
         path = Path(f"{str(project_path)}/data_export/{study}/")
         if path.exists():
             for file in path.glob("*"):
                 file.unlink()
 
     ### Creating studies
+
+    def clean_study(self, targets: List[str]) -> None:
+        """Removes study table/views from Athena.
+
+        While this is usually not required, since it it done as part of a build,
+        this can be useful for cleaning up tables if a study prefix is changed
+        for some reason.
+
+        :param target: The study prefix to use for IDing tables to remove"""
+        if targets is None or targets == ["all"]:
+            sys.exit(
+                "Explicit targets for cleaning not provided. "
+                "Provide one or more explicit study prefixes to remove."
+            )
+        for study in targets:
+            StudyManifestParser.clean_study(
+                self.cursor, self.schema_name, self.verbose, prefix=f"{study}__"
+            )
+
     def clean_and_build_study(self, target: PosixPath) -> None:
-        """Exports aggregates defined in a manifesty
+        """Recreates study views/tables
 
-        :param taget: A PosixPath to the study directory
+        :param target: A PosixPath to the study directory
         """
         studyparser = StudyManifestParser(target)
         studyparser.clean_study(self.cursor, self.schema_name, self.verbose)
         studyparser.run_python_builder(self.cursor, self.schema_name, self.verbose)
         studyparser.build_study(self.cursor, self.verbose)
 
     def clean_and_build_all(self, study_dict: Dict) -> None:
@@ -95,30 +115,32 @@
         for precursor_study in ["vocab", "core"]:
             self.clean_and_build_study(study_dict[precursor_study])
             study_dict.pop(precursor_study)
         for key in study_dict:
             self.clean_and_build_study(study_dict[key])
 
     ### Data exporters
-    def export_study(self, target: PosixPath) -> None:
-        """Exports aggregates defined in a manifesty
+    def export_study(self, target: PosixPath, data_path: PosixPath) -> None:
+        """Exports aggregates defined in a manifest
 
-        :param taget: A PosixPath to the study directory
+        :param target: A PosixPath to the study directory
         """
+        if data_path is None:
+            sys.exit("Missing destination - please provide a path argument.")
         studyparser = StudyManifestParser(target)
-        studyparser.export_study(self.pandas_cursor)
+        studyparser.export_study(self.pandas_cursor, data_path)
 
-    def export_all(self, study_dict: Dict):
+    def export_all(self, study_dict: Dict, data_path: PosixPath):
         """Exports all defined count tables to disk"""
         for key in study_dict.keys():
-            self.export_study(study_dict[key])
+            self.export_study(study_dict[key], data_path)
 
 
 def get_abs_posix_path(path: str) -> PosixPath:
-    """Conveince method for hanlding abs vs rel paths"""
+    """Convenience method for handling abs vs rel paths"""
     if path[0] == "/":
         return Path(path)
     else:
         return Path(Path.cwd(), path)
 
 
 def create_template(path: str) -> None:
@@ -170,193 +192,102 @@
             elif child_path.name == "manifest.toml":
                 manifest_studies[parent_path.name] = parent_path
     return manifest_studies
 
 
 def run_cli(args: Dict):
     """Controls which library tasks are run based on CLI arguments"""
-    if not args["build"] and not args["export"] and not args["create"]:
-        sys.exit(
-            (
-                "Expecting at least one of build, export or create as arguments. "
-                "See `cumulus-library --help` for more information"
-            )
-        )
+    if args["action"] == "create":
+        create_template(args["create_dir"])
 
-    if args["create"]:
-        create_template(args["path"])
+    elif args["action"] == "upload":
+        upload_files(args)
 
-    elif args["build"] or args["export"]:
+    # all other actions require connecting to AWS
+    else:
         builder = StudyBuilder(
             args["region"],
             args["workgroup"],
             args["profile"],
             args["schema_name"],
         )
         if args["verbose"]:
             builder.verbose = True
-
-        study_dict = get_study_dict(args["study_dir"])
-        if args["target"]:
-            for target in args["target"]:
-                if target not in study_dict:
-                    sys.exit(
-                        f"{target} was not found in available studies: "
-                        f"{list(study_dict.keys())}.\n\n"
-                        "If you are trying to run a custom study, make sure "
-                        "you include `-s path/to/study/dir` as an arugment."
-                    )
-        # here we invoke the cursor once to confirm valid connections
+        print("Testing connection to athena...")
         builder.cursor.execute("show tables")
 
-        if args["build"]:
-            if "all" in args["target"]:
-                builder.clean_and_build_all(study_dict)
-            else:
-                for target in args["target"]:
-                    builder.clean_and_build_study(study_dict[target])
+        if args["action"] == "clean":
+            builder.clean_study(args["target"])
 
-        if args["export"]:
-            if "all" in args["target"]:
-                builder.export_all(study_dict)
-            else:
+        else:
+            study_dict = get_study_dict(args["study_dir"])
+            if args["target"]:
                 for target in args["target"]:
-                    builder.export_study(study_dict[target])
+                    if target not in study_dict:
+                        sys.exit(
+                            f"{target} was not found in available studies: "
+                            f"{list(study_dict.keys())}.\n\n"
+                            "If you are trying to run a custom study, make sure "
+                            "you include `-s path/to/study/dir` as an arugment."
+                        )
+
+            if args["action"] == "build":
+                if "all" in args["target"]:
+                    builder.clean_and_build_all(study_dict)
+                else:
+                    for target in args["target"]:
+                        builder.clean_and_build_study(study_dict[target])
+
+            elif args["action"] == "export":
+                if "all" in args["target"]:
+                    builder.export_all(study_dict, args["data_path"])
+                else:
+                    for target in args["target"]:
+                        builder.export_study(study_dict[target], args["data_path"])
 
         # returning the builder for ease of unit testing
         return builder
 
 
-def get_parser():
-    """Provides parser for handling CLI arguments"""
-    parser = argparse.ArgumentParser(
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-        description="""Generates study tables and views from post-Cumulus ETL data.
-
-cumulus_library will attempt to create a connection to AWS athena. The
-following order of preference is used to select credentials:
-  - explict command line arguments
-  - cumulus environment variables (CUMULUS_LIBRARY_PROFILE, 
-    CUMULUS_LIBRARY_DATABASE, CUMULUS_LIBRARY_REGION)
-  - Normal boto profile order (AWS env vars, ~/.aws/credentials, ~/.aws/config)""",
-    )
-
-    studygen = parser.add_argument_group("Creating study templates")
-    studygen.add_argument(
-        "-c",
-        "--create",
-        action="store_true",
-        default=False,
-        help=("Create a study instance from a template"),
-    )
-    studygen.add_argument(
-        "-p",
-        "--path",
-        default="./",
-        help=(
-            "The the directory the study will be created in. Default is "
-            "the current directory."
-        ),
-    )
-
-    db = parser.add_argument_group("SQL database modifications")
-    db.add_argument(
-        "-t",
-        "--target",
-        action="append",
-        help=(
-            "Specify one or more studies to create views form. Default is to "
-            "build all studies."
-        ),
-    )
-    db.add_argument(
-        "-s",
-        "--study-dir",
-        action="append",
-        help=(
-            "Optionally add one or more directories to look for study definitions in. "
-            "Default is in project directory and CUMULUS_LIBRARY_PATH, if present, "
-            "followed by any supplied paths. Target, and all its subdirectories, "
-            "are checked for manifests. Overriding studies with the same namespace "
-            "supersede earlier ones."
-        ),
-    )
-    db.add_argument(
-        "-b",
-        "--build",
-        default=False,
-        action="store_true",
-        help=("Removes and recreates Athena tables & views for the specified studies"),
-    )
-    db.add_argument(
-        "-e",
-        "--export",
-        default=False,
-        action="store_true",
-        help=("Generates files on disk from Athena views for the specified studies"),
-    )
-    db.add_argument(
-        "-v",
-        "--verbose",
-        default=False,
-        action="store_true",
-        help=("Prints detailed SQL query info"),
-    )
-
-    aws = parser.add_argument_group("AWS config")
-    aws.add_argument("--profile", help="AWS profile", default="default")
-    aws.add_argument(
-        "--database",
-        # internally, we use PyAthena's terminology for this but the UX term is "database"
-        dest="schema_name",
-        help="Cumulus Athena database name",
-    )
-    aws.add_argument(
-        "--workgroup",
-        default="cumulus",
-        help="Cumulus Athena workgroup (default: cumulus)",
-    )
-    aws.add_argument(
-        "--region",
-        help="AWS region data of Athena instance (default: us-east-1)",
-        default="us-east-1",
-    )
-
-    return parser
-
-
 def main(cli_args=None):
     """Reads CLI input/environment variables and invokes library calls"""
     parser = get_parser()
     args = vars(parser.parse_args(cli_args))
-
-    if args["target"] is not None:
+    if args["action"] is None:
+        parser.print_usage()
+        sys.exit(1)
+    if args.get("target"):
         for target in args["target"]:
             if target == "all":
                 args["target"] = ["all"]
                 break
-    else:
-        args["target"] = ["all"]
 
-    if args["study_dir"] is not None:
+    arg_env_pairs = (
+        ("profile", "CUMULUS_LIBRARY_PROFILE"),
+        ("schema_name", "CUMULUS_LIBRARY_DATABASE"),
+        ("workgroup", "CUMULUS_LIBRARY_WORKGROUP"),
+        ("region", "CUMULUS_LIBRARY_REGION"),
+        ("study_dir", "CUMULUS_LIBRARY_STUDY_DIR"),
+        ("data_path", "CUMULUS_LIBRARY_DATA_PATH"),
+        ("user", "CUMULUS_AGGREGATOR_USER"),
+        ("id", "CUMULUS_AGGREGATOR_ID"),
+        ("url", "CUMULUS_AGGREGATOR_URL"),
+    )
+    for pair in arg_env_pairs:
+        if env_val := os.environ.get(pair[1]):
+            args[pair[0]] = env_val
+
+    if args.get("study_dir"):
         posix_paths = []
         for path in args["study_dir"]:
             posix_paths.append(get_abs_posix_path(path))
         args["study_dir"] = posix_paths
 
-    if profile_env := os.environ.get("CUMULUS_LIBRARY_PROFILE"):
-        args["profile"] = profile_env
-    if database_env := os.environ.get("CUMULUS_LIBRARY_DATABASE"):
-        args["schema_name"] = database_env
-    if workgroup_env := os.environ.get("CUMULUS_LIBRARY_WORKGROUP"):
-        args["workgroup"] = workgroup_env
-    if region_env := os.environ.get("CUMULUS_LIBRARY_REGION"):
-        args["region"] = region_env
-    if path_dir := os.environ.get("CUMULUS_LIBRARY_PATH"):
-        args["path"] = [path_dir] + args["path"]
+    if args.get("data_path"):
+        args["data_path"] = get_abs_posix_path(args["data_path"])
 
     return run_cli(args)
 
 
 def main_cli():  # called by the generated wrapper scripts
     main()
```

### Comparing `cumulus_library-0.2.1/cumulus_library/helper.py` & `cumulus_library-0.3.0/cumulus_library/helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,7 +51,18 @@
 ):
     """Convenience function for determining output type"""
     if verbose:
         print()
         print(query)
     else:
         progress_bar.advance(task)
+
+
+def get_progress_bar(**kwargs) -> progress.Progress:
+    # The default columns don't change to elapsed time when finished.
+    return progress.Progress(
+        progress.TextColumn("[progress.description]{task.description}"),
+        progress.BarColumn(),
+        progress.TaskProgressColumn(),
+        progress.TimeRemainingColumn(elapsed_when_finished=True),
+        **kwargs,
+    )
```

### Comparing `cumulus_library-0.2.1/cumulus_library/schema/columns.py` & `cumulus_library-0.3.0/cumulus_library/schema/columns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # pylint: disable=W,C,R
 from enum import Enum, EnumMeta
-from library.schema.typesystem import Datatypes, Coding, Vocab
-from library.schema.valueset import Gender, Race, Ethnicity
-from library.schema.valueset import DurationUnits
-from library.schema.valueset import EncounterCode
-from library.schema.valueset import ObservationInterpretationDetection
-
-from library.schema import future
+from cumulus_library.schema.typesystem import Datatypes, Coding, Vocab
+from cumulus_library.schema.valueset import Gender, Race, Ethnicity
+from cumulus_library.schema.valueset import DurationUnits
+from cumulus_library.schema.valueset import EncounterCode
+from cumulus_library.schema.valueset import ObservationInterpretationDetection
 
 
 class ColumnEnum(Enum):
     # Counts
     cnt = Datatypes.Int, "Count"
     cnt_subject = Datatypes.Int, "Count Patients"
     cnt_encounter = Datatypes.Int, "Count Encounters"
```

### Comparing `cumulus_library-0.2.1/cumulus_library/schema/counts.py` & `cumulus_library-0.3.0/cumulus_library/schema/counts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=W,C,R
-from library.schema.valueset import DurationUnits
-from library.schema.columns import ColumnEnum as Column
-from library.errors import LibraryError
+from cumulus_library.schema.valueset import DurationUnits
+from cumulus_library.schema.columns import ColumnEnum as Column
+from cumulus_library.errors import LibraryError
 
 ##################################################
 # Google Style Guide
 #
 # https://google.github.io/styleguide/pyguide.html
 # Design by composition composition for
 #
```

### Comparing `cumulus_library-0.2.1/cumulus_library/schema/typesystem.py` & `cumulus_library-0.3.0/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/schema/valueset.py` & `cumulus_library-0.3.0/cumulus_library/schema/valueset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pylint: disable=W,C,R
 from enum import Enum
-from library.schema.typesystem import Coding, Vocab
+from cumulus_library.schema.typesystem import Coding, Vocab
 
 ################################################################################
 # FHIR ValueSets
 ################################################################################
 
 
 class ValueSet(Enum):
```

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/core/condition.sql` & `cumulus_library-0.3.0/cumulus_library/studies/core/condition.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/core/documentreference.sql` & `cumulus_library-0.3.0/cumulus_library/studies/core/documentreference.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/core/encounter.sql` & `cumulus_library-0.3.0/cumulus_library/studies/core/encounter.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/core/fhir_define.sql` & `cumulus_library-0.3.0/cumulus_library/studies/core/fhir_define.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/core/manifest.toml` & `cumulus_library-0.3.0/cumulus_library/studies/core/manifest.toml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 file_names = [
     "setup.sql",
     "fhir_define.sql",
     "patient.sql",
     "encounter.sql",
     "documentreference.sql",
     "condition.sql",
+    "observation.sql",
     "observation_lab.sql",
+    "observation_vital_signs.sql",
     "medication_request.sql",
     "study_period.sql",
 ]
 
 [export_config]
 export_list = [
     "core__count_patient",
```

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/core/medication_request.sql` & `cumulus_library-0.3.0/cumulus_library/studies/core/medication_request.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/core/observation_lab.sql` & `cumulus_library-0.3.0/cumulus_library/studies/core/observation_lab.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/core/patient.sql` & `cumulus_library-0.3.0/cumulus_library/studies/core/patient.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/core/patient_extensions.py` & `cumulus_library-0.3.0/cumulus_library/studies/core/patient_extensions.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/core/setup.sql` & `cumulus_library-0.3.0/cumulus_library/studies/core/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/core/study_period.sql` & `cumulus_library-0.3.0/cumulus_library/studies/core/study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/template/counts.sql` & `cumulus_library-0.3.0/cumulus_library/studies/template/counts.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-0.3.0/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/template/manifest.toml` & `cumulus_library-0.3.0/cumulus_library/studies/template/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/template/setup.sql` & `cumulus_library-0.3.0/cumulus_library/studies/template/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/vocab/ICD10.bsv` & `cumulus_library-0.3.0/cumulus_library/studies/vocab/ICD10.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/vocab/ICD9.bsv` & `cumulus_library-0.3.0/cumulus_library/studies/vocab/ICD9.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/studies/vocab/vocab_icd_builder.py` & `cumulus_library-0.3.0/cumulus_library/studies/vocab/vocab_icd_builder.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/study_parser.py` & `cumulus_library-0.3.0/cumulus_library/study_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """ Contains classes for loading study data based on manifest.toml files """
 import inspect
 import sys
 
 from importlib.machinery import SourceFileLoader
-from pathlib import Path
+from pathlib import Path, PosixPath
 from typing import List, Optional
 
 import toml
 
 from rich.progress import Progress, TaskID, track
 
 from cumulus_library.base_runner import BaseRunner
-from cumulus_library.helper import query_console_output, load_text, parse_sql
+from cumulus_library.helper import (
+    query_console_output,
+    load_text,
+    parse_sql,
+    get_progress_bar,
+)
 from cumulus_library.template_sql.templates import (
     get_show_tables,
     get_show_views,
     get_drop_view_table,
 )
 
 StrList = List[str]
@@ -123,29 +128,34 @@
         path = Path(f"{str(project_path)}/data_export/{self.get_study_prefix()}/")
         if path.exists():
             for file in path.glob("*"):
                 file.unlink()
 
     # SQL related functions
     def clean_study(
-        self, cursor: object, schema_name: str, verbose: bool = False
+        self,
+        cursor: object,
+        schema_name: str,
+        verbose: bool = False,
+        prefix: str = None,
     ) -> List:
         """Removes tables beginning with the study prefix from the database schema
 
         :param cursor: A PEP-249 compatible cursor object
         :param schema_name: The name of the schema containing the study tables
         :verbose: toggle from progress bar to query output, optional
         :returns: list of dropped tables (for unit testing only)
 
         TODO: If we need to support additional databases, we may need to investigate
         additional ways to get a list of table prefixes
         """
         if not schema_name:
             raise ValueError("No database provided")
-        prefix = self.get_study_prefix()
+        if not prefix:
+            prefix = self.get_study_prefix()
         view_sql = get_show_views(schema_name, prefix)
         table_sql = get_show_tables(schema_name, prefix)
         view_table_list = []
         for query_and_type in [[view_sql, "VIEW"], [table_sql, "TABLE"]]:
             cursor.execute(query_and_type[0])
             for db_row_tuple in cursor:
                 # this check handles athena reporting views as also being tables,
@@ -167,15 +177,15 @@
             if any(
                 view_table[0].startswith(f"{self.get_study_prefix()}__{word}_")
                 for word in RESERVED_TABLE_KEYWORDS
             ):
                 view_table_list.remove(view_table)
 
         # We want to only show a progress bar if we are :not: printing SQL lines
-        with Progress(disable=verbose) as progress:
+        with get_progress_bar(disable=verbose) as progress:
             task = progress.add_task(
                 f"Removing {self.get_study_prefix()} study artifacts...",
                 total=len(view_table_list),
                 visible=not verbose,
             )
             self._execute_drop_queries(cursor, verbose, view_table_list, progress, task)
         return view_table_list
@@ -252,15 +262,15 @@
         queries = []
         for file in self.get_sql_file_list():
             for query in parse_sql(load_text(f"{self._study_path}/{file}")):
                 queries.append([query, file])
         if len(queries) == 0:
             return []
         # We want to only show a progress bar if we are :not: printing SQL lines
-        with Progress(disable=verbose) as progress:
+        with get_progress_bar(disable=verbose) as progress:
             task = progress.add_task(
                 f"Creating {self.get_study_prefix()} study in db...",
                 total=len(queries),
                 visible=not verbose,
             )
             self._execute_build_queries(
                 cursor,
@@ -341,15 +351,15 @@
                     "You can debug issues with this query using `sqlfluff lint`, "
                     "or by executing the query directly against the database.\n"
                     f"Error: {e}",
                 )
 
     # Database exporting functions
 
-    def export_study(self, cursor: object) -> List:
+    def export_study(self, cursor: object, data_path: PosixPath) -> List:
         """Exports csvs/parquet extracts of tables listed in export_list
 
         :param cursor: A PEP-249 compatible cursor object
         :returns: list of executed queries (for unit testing only)
 
         TODO: If we need to support additional databases, we may need to investigate
         additional ways to convert the query to a pandas object
@@ -358,14 +368,13 @@
         queries = []
         for table in track(
             self.get_export_table_list(),
             description=f"Exporting {self.get_study_prefix()} counts...",
         ):
             query = f"select * from {table}"
             dataframe = cursor.execute(query).as_pandas()
-            project_path = Path(__file__).resolve().parents[1]
-            path = Path(f"{str(project_path)}/data_export/{self.get_study_prefix()}/")
+            path = Path(f"{str(data_path)}/{self.get_study_prefix()}/")
             path.mkdir(parents=True, exist_ok=True)
             dataframe.to_csv(f"{path}/{table}.csv", index=False)
             dataframe.to_parquet(f"{path}/{table}.parquet", index=False)
             queries.append(query)
         return queries
```

### Comparing `cumulus_library-0.2.1/cumulus_library/template_sql/ctas.sql.jinja` & `cumulus_library-0.3.0/cumulus_library/template_sql/ctas.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/template_sql/extension_denormalize.sql.jinja` & `cumulus_library-0.3.0/cumulus_library/template_sql/extension_denormalize.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.1/cumulus_library/template_sql/templates.py` & `cumulus_library-0.3.0/cumulus_library/template_sql/templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,14 +74,32 @@
             schema_name=schema_name,
             table_name=table_name,
             dataset=dataset,
             table_cols=table_cols,
         )
 
 
+def get_create_view_query(
+    view_name: str, dataset: List[List[str]], view_cols: List[str]
+) -> str:
+    """Generates a create view as query for inserting static data into athena
+
+    :param view_name: The name of the athena table to create
+    :param dataset: Array of data arrays to insert, i.e. [['1','3'],['2','4']]
+    :param table_cols: Comma deleniated column names, i.e. ['first,second']
+    """
+    path = Path(__file__).parent
+    with open(f"{path}/create_view_as.sql.jinja") as cvas:
+        return Template(cvas.read()).render(
+            view_name=view_name,
+            dataset=dataset,
+            view_cols=view_cols,
+        )
+
+
 def get_insert_into_query(
     table_name: str, table_cols: List[str], dataset: List[List[str]]
 ) -> str:
     """Generates an insert query for adding data to an existing athena table
 
     :param schema_name: The athena query to create the table in
     :param table_name: The name of the athena table to create
```

### Comparing `cumulus_library-0.2.1/pyproject.toml` & `cumulus_library-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cumulus-library"
-version = "0.2.1"
+version = "0.3.0"
 # In order to support 3.12, we wil need to refactor out load_module, which is
 # targeted for deprecation in that version.
 requires-python = ">= 3.9, <3.12"
 dependencies = [
     "ctakesclient >= 1.3",
     "fhirclient >= 4.1",
     "Jinja2 > 3",
@@ -31,14 +31,15 @@
 [project.optional-dependencies]
 dev = [
     "black",
     "pylint",
 ]
 test = [
     "pytest",
+    "requests-mock"
 ]
 
 [project.urls]
 Home = "https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/"
 Documentation = "https://docs.smarthealthit.org/cumulus/"
 Source = "https://github.com/smart-on-fhir/cumulus-library-core"
```

### Comparing `cumulus_library-0.2.1/PKG-INFO` & `cumulus_library-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 0.2.1
+Version: 0.3.0
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
 Requires-Python: >= 3.9, <3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,15 @@
 Requires-Dist: requests >= 2.28
 Requires-Dist: rich >= 13.2
 Requires-Dist: sqlfluff == 2.0.2
 Requires-Dist: toml >= 0.10
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: pylint ; extra == "dev"
 Requires-Dist: pytest ; extra == "test"
+Requires-Dist: requests-mock ; extra == "test"
 Project-URL: Documentation, https://docs.smarthealthit.org/cumulus/
 Project-URL: Home, https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/
 Project-URL: Source, https://github.com/smart-on-fhir/cumulus-library-core
 Provides-Extra: dev
 Provides-Extra: test
 
 # Cumulus Library - Core
```

