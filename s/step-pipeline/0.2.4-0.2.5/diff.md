# Comparing `tmp/step_pipeline-0.2.4.tar.gz` & `tmp/step_pipeline-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/step_pipeline-0.2.4.tar", last modified: Thu Jun  1 18:51:32 2023, max compression
+gzip compressed data, was "dist/step_pipeline-0.2.5.tar", last modified: Tue Jun 20 16:38:20 2023, max compression
```

## Comparing `step_pipeline-0.2.4.tar` & `step_pipeline-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/
--rw-r--r--   0 weisburd   (502) staff       (20)     1060 2021-05-21 18:58:34.000000 step_pipeline-0.2.4/LICENSE
--rw-r--r--   0 weisburd   (502) staff       (20)     2368 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/PKG-INFO
--rw-r--r--   0 weisburd   (502) staff       (20)     1445 2022-03-18 01:37:01.000000 step_pipeline-0.2.4/README.md
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/integration_tests/
--rw-r--r--   0 weisburd   (502) staff       (20)        0 2022-05-24 22:25:36.000000 step_pipeline-0.2.4/integration_tests/__init__.py
--rw-r--r--   0 weisburd   (502) staff       (20)      553 2022-10-12 17:27:55.000000 step_pipeline-0.2.4/integration_tests/batch_pipeline1.py
--rw-r--r--   0 weisburd   (502) staff       (20)      450 2022-03-03 16:33:56.000000 step_pipeline-0.2.4/integration_tests/integration_test1.py
--rw-r--r--   0 weisburd   (502) staff       (20)     1062 2022-05-24 22:58:13.000000 step_pipeline-0.2.4/integration_tests/integration_test2.py
--rw-r--r--   0 weisburd   (502) staff       (20)     1387 2022-05-24 23:01:47.000000 step_pipeline-0.2.4/integration_tests/integration_test3.py
--rw-r--r--   0 weisburd   (502) staff       (20)       38 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/setup.cfg
--rw-r--r--   0 weisburd   (502) staff       (20)     2109 2023-06-01 18:51:10.000000 step_pipeline-0.2.4/setup.py
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline/
--rw-r--r--   0 weisburd   (502) staff       (20)      267 2023-05-17 16:33:11.000000 step_pipeline-0.2.4/step_pipeline/__init__.py
--rw-r--r--   0 weisburd   (502) staff       (20)    43539 2023-05-17 19:22:29.000000 step_pipeline-0.2.4/step_pipeline/batch.py
--rw-r--r--   0 weisburd   (502) staff       (20)      223 2022-03-16 16:43:41.000000 step_pipeline-0.2.4/step_pipeline/constants.py
--rw-r--r--   0 weisburd   (502) staff       (20)    13598 2022-10-10 22:13:19.000000 step_pipeline-0.2.4/step_pipeline/io.py
--rw-r--r--   0 weisburd   (502) staff       (20)     2278 2022-03-16 17:33:05.000000 step_pipeline-0.2.4/step_pipeline/main.py
--rw-r--r--   0 weisburd   (502) staff       (20)    50464 2023-05-31 13:10:30.000000 step_pipeline-0.2.4/step_pipeline/pipeline.py
--rw-r--r--   0 weisburd   (502) staff       (20)    14717 2023-05-25 22:02:37.000000 step_pipeline-0.2.4/step_pipeline/utils.py
--rw-r--r--   0 weisburd   (502) staff       (20)    14714 2022-07-04 19:59:27.000000 step_pipeline-0.2.4/step_pipeline/wdl.py
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline.egg-info/
--rw-r--r--   0 weisburd   (502) staff       (20)     2368 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 weisburd   (502) staff       (20)      661 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 weisburd   (502) staff       (20)        1 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 weisburd   (502) staff       (20)      100 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline.egg-info/requires.txt
--rw-r--r--   0 weisburd   (502) staff       (20)       38 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/step_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-01 18:51:32.000000 step_pipeline-0.2.4/tests/
--rw-r--r--   0 weisburd   (502) staff       (20)        0 2021-05-21 03:13:52.000000 step_pipeline-0.2.4/tests/__init__.py
--rw-r--r--   0 weisburd   (502) staff       (20)    10927 2022-07-04 19:59:27.000000 step_pipeline-0.2.4/tests/utils_tests.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-20 16:38:20.000000 step_pipeline-0.2.5/
+-rw-r--r--   0 weisburd   (502) staff       (20)     1060 2021-05-21 18:58:34.000000 step_pipeline-0.2.5/LICENSE
+-rw-r--r--   0 weisburd   (502) staff       (20)     2368 2023-06-20 16:38:20.000000 step_pipeline-0.2.5/PKG-INFO
+-rw-r--r--   0 weisburd   (502) staff       (20)     1445 2022-03-18 01:37:01.000000 step_pipeline-0.2.5/README.md
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-20 16:38:20.000000 step_pipeline-0.2.5/integration_tests/
+-rw-r--r--   0 weisburd   (502) staff       (20)        0 2022-05-24 22:25:36.000000 step_pipeline-0.2.5/integration_tests/__init__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)      553 2022-10-12 17:27:55.000000 step_pipeline-0.2.5/integration_tests/batch_pipeline1.py
+-rw-r--r--   0 weisburd   (502) staff       (20)      450 2022-03-03 16:33:56.000000 step_pipeline-0.2.5/integration_tests/integration_test1.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1062 2022-05-24 22:58:13.000000 step_pipeline-0.2.5/integration_tests/integration_test2.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     1387 2022-05-24 23:01:47.000000 step_pipeline-0.2.5/integration_tests/integration_test3.py
+-rw-r--r--   0 weisburd   (502) staff       (20)       38 2023-06-20 16:38:20.000000 step_pipeline-0.2.5/setup.cfg
+-rw-r--r--   0 weisburd   (502) staff       (20)     2109 2023-06-20 16:03:37.000000 step_pipeline-0.2.5/setup.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-20 16:38:20.000000 step_pipeline-0.2.5/step_pipeline/
+-rw-r--r--   0 weisburd   (502) staff       (20)      267 2023-05-17 16:33:11.000000 step_pipeline-0.2.5/step_pipeline/__init__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    43539 2023-05-17 19:22:29.000000 step_pipeline-0.2.5/step_pipeline/batch.py
+-rw-r--r--   0 weisburd   (502) staff       (20)      223 2022-03-16 16:43:41.000000 step_pipeline-0.2.5/step_pipeline/constants.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    13700 2023-06-20 16:01:43.000000 step_pipeline-0.2.5/step_pipeline/io.py
+-rw-r--r--   0 weisburd   (502) staff       (20)     2278 2022-03-16 17:33:05.000000 step_pipeline-0.2.5/step_pipeline/main.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    50961 2023-06-20 16:01:43.000000 step_pipeline-0.2.5/step_pipeline/pipeline.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    14775 2023-06-20 16:01:43.000000 step_pipeline-0.2.5/step_pipeline/utils.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    14714 2022-07-04 19:59:27.000000 step_pipeline-0.2.5/step_pipeline/wdl.py
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-20 16:38:20.000000 step_pipeline-0.2.5/step_pipeline.egg-info/
+-rw-r--r--   0 weisburd   (502) staff       (20)     2368 2023-06-20 16:38:20.000000 step_pipeline-0.2.5/step_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 weisburd   (502) staff       (20)      661 2023-06-20 16:38:20.000000 step_pipeline-0.2.5/step_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)        1 2023-06-20 16:38:20.000000 step_pipeline-0.2.5/step_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)      100 2023-06-20 16:38:20.000000 step_pipeline-0.2.5/step_pipeline.egg-info/requires.txt
+-rw-r--r--   0 weisburd   (502) staff       (20)       38 2023-06-20 16:38:20.000000 step_pipeline-0.2.5/step_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-06-20 16:38:20.000000 step_pipeline-0.2.5/tests/
+-rw-r--r--   0 weisburd   (502) staff       (20)        0 2021-05-21 03:13:52.000000 step_pipeline-0.2.5/tests/__init__.py
+-rw-r--r--   0 weisburd   (502) staff       (20)    10927 2022-07-04 19:59:27.000000 step_pipeline-0.2.5/tests/utils_tests.py
```

### Comparing `step_pipeline-0.2.4/LICENSE` & `step_pipeline-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `step_pipeline-0.2.4/PKG-INFO` & `step_pipeline-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: step_pipeline
-Version: 0.2.4
+Version: 0.2.5
 Summary: Pipeline library that simplifies creation of pipelines that run on top of hail Batch and other compute enviornments
 Home-page: https://github.com/broadinstitute/step_pipeline
 License: MIT
 Keywords: pipelines,workflows,hail,Batch,cromwell,Terra,dsub,SGE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `step_pipeline-0.2.4/README.md` & `step_pipeline-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `step_pipeline-0.2.4/integration_tests/batch_pipeline1.py` & `step_pipeline-0.2.5/integration_tests/batch_pipeline1.py`

 * *Files identical despite different names*

### Comparing `step_pipeline-0.2.4/integration_tests/integration_test2.py` & `step_pipeline-0.2.5/integration_tests/integration_test2.py`

 * *Files identical despite different names*

### Comparing `step_pipeline-0.2.4/integration_tests/integration_test3.py` & `step_pipeline-0.2.5/integration_tests/integration_test3.py`

 * *Files identical despite different names*

### Comparing `step_pipeline-0.2.4/setup.py` & `step_pipeline-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         os.system("rm -rf dist")
         os.system("python3.7 setup.py sdist"
                   "&& python3.7 setup.py bdist_wheel"
                   "&& python3.7 -m twine upload dist/*whl dist/*gz")
 
 setup(
     name='step_pipeline',
-    version="0.2.4",
+    version="0.2.5",
     description="Pipeline library that simplifies creation of pipelines that run on top of hail Batch and other compute enviornments",
     install_requires=install_requires,
     cmdclass={
         'coverage': CoverageCommand,
         'publish': PublishCommand,
     },
     long_description_content_type="text/markdown",
```

### Comparing `step_pipeline-0.2.4/step_pipeline/batch.py` & `step_pipeline-0.2.5/step_pipeline/batch.py`

 * *Files identical despite different names*

### Comparing `step_pipeline-0.2.4/step_pipeline/io.py` & `step_pipeline-0.2.5/step_pipeline/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,34 +296,38 @@
         return self._localization_root_dir
 
 
 class OutputSpec:
     """An OutputSpec stores metadata about an output file or directory from a Step"""
 
     def __init__(
-            self,
-            local_path=None,
-            output_dir=None,
-            output_path=None,
-            name=None,
-            delocalize_by=None):
+        self,
+        local_path=None,
+        output_dir=None,
+        output_path=None,
+        name=None,
+        delocalize_by=None,
+        optional=False,
+    ):
         """OutputSpec constructor
 
         Args:
             local_path (str): Local (within container) path of file or directory to delocalize. The path can include *
                 wildcards.
             output_dir (str): Optional destination directory.
             output_path (str): Optional destination path - either absolute, or relative to output_dir.
             name (str): Optional name for this output.
             delocalize_by (Delocalize): Approach to use to delocalize this path.
+            optional (bool): Whether this output is optional.
         """
         self._local_path = local_path
         self._local_dir = os.path.dirname(local_path)
         self._name = name
         self._delocalize_by = delocalize_by
+        self._optional = optional
 
         if delocalize_by and not isinstance(delocalize_by, Delocalize):
             raise ValueError(f"localize_by arg: {delocalize_by} is not an instance of the Delocalize enum")
 
         # define self._output_filename
         if output_path:
             self._output_filename = os.path.basename(output_path)
```

### Comparing `step_pipeline-0.2.4/step_pipeline/main.py` & `step_pipeline-0.2.5/step_pipeline/main.py`

 * *Files identical despite different names*

### Comparing `step_pipeline-0.2.4/step_pipeline/pipeline.py` & `step_pipeline-0.2.5/step_pipeline/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,15 +714,14 @@
     def input(self, source_path=None, name=None, localize_by=None):
         """Specifies an input file or directory.
 
         Args:
             source_path (str): Path of input file or directory to localize.
             name (str): Optional name for this input.
             localize_by (Localize): How this path should be localized.
-
         Return:
             InputSpec: An object that describes the specified input file or directory.
         """
         localize_by = localize_by or self._localize_by
 
         # validate inputs
         if source_path is not None and not isinstance(source_path, str):
@@ -844,27 +843,31 @@
         """If an output path is specified as a relative path, it will be relative to this dir.
 
         Args:
             path (str): Directory path.
         """
         self._output_dir = path
 
-    def output(self, local_path, output_path=None, output_dir=None, name=None, delocalize_by=None):
+    def output(self, local_path, output_path=None, output_dir=None, name=None, delocalize_by=None, optional=False):
         """Specify a Step output file or directory.
 
         Args:
             local_path (str): The file or directory path within the execution container's file system.
             output_path (str): Optional destination path to which the local_path should be delocalized.
             output_dir (str): Optional destination directory to which the local_path should be delocalized.
                 It is expected that either output_path will be specified, or an output_dir value will be provided as an
                 argument to this method or previously (such as by calling the step.output_dir(..) setter method).
-                If both output_path and output_dir are specified and output_path is a relative path, it is interpretted
+                If both output_path and output_dir are specified and output_path is a relative path, it is interpreted
                 as being relative to output_dir.
             name (str): Optional name for this output.
             delocalize_by (Delocalize): How this path should be delocalized.
+            optional (bool): If True, this output is considered optional and, although it will be delocalized, steps
+                that didn't produce this output will still be skipped even if this output is missing. This is useful
+                for modifying existing pipelines to output additional files (eg. log files) without this triggering a
+                rerun of previously steps that completed previously without generating these files.
 
         Returns:
             OutputSpec: An object describing this output.
         """
 
         delocalize_by = delocalize_by or self._delocalize_by
         if delocalize_by is None:
@@ -872,14 +875,15 @@
 
         output_spec = OutputSpec(
             local_path=local_path,
             output_dir=output_dir or self._output_dir,
             output_path=output_path,
             name=name,
             delocalize_by=delocalize_by,
+            optional=optional,
         )
 
         self._preprocess_output_spec(output_spec)
 
         self._output_specs.append(output_spec)
 
         return output_spec
```

### Comparing `step_pipeline-0.2.4/step_pipeline/utils.py` & `step_pipeline-0.2.5/step_pipeline/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
             return True
 
     return False
 
 
 def all_outputs_exist(step, verbose=False):
     """Returns True if all of the Step's output files already exist"""
-    return files_exist([output_spec.output_path for output_spec in step._output_specs], verbose=verbose)
+    return files_exist([output_spec.output_path for output_spec in step._output_specs if not output_spec._optional], verbose=verbose)
 
 
 def files_exist(file_paths, verbose=False):
     """Returns True if all of the files exist"""
     for file_path in file_paths:
         if not _path_exists__cached(file_path, verbose=verbose):
             return False
@@ -307,15 +307,15 @@
     return oldest_output_modified_date is not None and latest_input_modified_date <= oldest_output_modified_date
 
 
 def are_outputs_up_to_date(step, verbose=False):
     """Returns True if all of the Step's outputs already exist and are newer than all inputs"""
 
     input_paths = [input_spec.original_source_path for input_spec in step._input_specs]
-    output_paths = [output_spec.output_path for output_spec in step._output_specs]
+    output_paths = [output_spec.output_path for output_spec in step._output_specs if not output_spec._optional]
 
     return are_output_files_up_to_date(input_paths, output_paths, verbose=verbose)
 
 
 class GoogleStorageException(Exception):
     pass
```

### Comparing `step_pipeline-0.2.4/step_pipeline/wdl.py` & `step_pipeline-0.2.5/step_pipeline/wdl.py`

 * *Files identical despite different names*

### Comparing `step_pipeline-0.2.4/step_pipeline.egg-info/PKG-INFO` & `step_pipeline-0.2.5/step_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: step-pipeline
-Version: 0.2.4
+Version: 0.2.5
 Summary: Pipeline library that simplifies creation of pipelines that run on top of hail Batch and other compute enviornments
 Home-page: https://github.com/broadinstitute/step_pipeline
 License: MIT
 Keywords: pipelines,workflows,hail,Batch,cromwell,Terra,dsub,SGE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `step_pipeline-0.2.4/step_pipeline.egg-info/SOURCES.txt` & `step_pipeline-0.2.5/step_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `step_pipeline-0.2.4/tests/utils_tests.py` & `step_pipeline-0.2.5/tests/utils_tests.py`

 * *Files identical despite different names*

