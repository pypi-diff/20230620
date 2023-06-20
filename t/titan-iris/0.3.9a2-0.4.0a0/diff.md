# Comparing `tmp/titan-iris-0.3.9a2.tar.gz` & `tmp/titan-iris-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.3.9a2.tar", last modified: Tue Apr  4 06:56:06 2023, max compression
+gzip compressed data, was "titan-iris-0.4.0a0.tar", last modified: Tue Jun 20 08:29:12 2023, max compression
```

## Comparing `titan-iris-0.3.9a2.tar` & `titan-iris-0.4.0a0.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:56:06.914348 titan-iris-0.3.9a2/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-04 06:56:06.914348 titan-iris-0.3.9a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 06:56:06.918348 titan-iris-0.3.9a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:56:06.902348 titan-iris-0.3.9a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:56:06.910348 titan-iris-0.3.9a2/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/src/iris/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:56:06.910348 titan-iris-0.3.9a2/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    23192 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:56:06.914348 titan-iris-0.3.9a2/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-04 06:56:06.000000 titan-iris-0.3.9a2/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-04 06:56:06.000000 titan-iris-0.3.9a2/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 06:56:06.000000 titan-iris-0.3.9a2/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-04 06:56:06.000000 titan-iris-0.3.9a2/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-04 06:56:06.000000 titan-iris-0.3.9a2/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-04 06:56:06.000000 titan-iris-0.3.9a2/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 06:56:06.914348 titan-iris-0.3.9a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-04 06:55:49.000000 titan-iris-0.3.9a2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.171455 titan-iris-0.4.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-20 08:29:12.171455 titan-iris-0.4.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 08:29:12.171455 titan-iris-0.4.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.159454 titan-iris-0.4.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.163454 titan-iris-0.4.0a0/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.167454 titan-iris-0.4.0a0/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.167454 titan-iris-0.4.0a0/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/safe_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.171455 titan-iris-0.4.0a0/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-20 08:29:12.000000 titan-iris-0.4.0a0/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-20 08:29:12.000000 titan-iris-0.4.0a0/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:29:12.000000 titan-iris-0.4.0a0/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 08:29:12.000000 titan-iris-0.4.0a0/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-20 08:29:12.000000 titan-iris-0.4.0a0/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 08:29:12.000000 titan-iris-0.4.0a0/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.171455 titan-iris-0.4.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/tests/test_sdk.py
```

### Comparing `titan-iris-0.3.9a2/.gitignore` & `titan-iris-0.4.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.3.9a2/Dockerfile` & `titan-iris-0.4.0a0/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.3.9a2/setup.py` & `titan-iris-0.4.0a0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""The titan-iris module is a Python SDK for the TitanML platform."""
 from setuptools import find_packages, setup
 
 setup(
     name="titan-iris",
     install_requires=[
         "typer ~= 0.7.0",
         "rich ~= 13.3.1",
@@ -11,14 +12,15 @@
         "python-dotenv ~= 0.19.1",
         "docker ~= 6.0.1",
         "tqdm ~=4.64.1",
         "wget ~= 3.2",
         "jmespath ~= 1.0",
         "tritonclient[http] ~= 2.30.0",
         "numpy >= 1.20.0",
+        "trogon ~= 0.2.1",
     ],
     entry_points={"console_scripts": ["iris = iris.main:main"]},
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     use_scm_version={"root": ".."},
     setup_requires=["setuptools_scm"],
```

### Comparing `titan-iris-0.3.9a2/src/iris/config.yaml` & `titan-iris-0.4.0a0/src/iris/config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 runner_path: "/backend/"
+metrics_path: "/post-metrics/"
 keyfile_name: .tytn_key
 
 environment: prod
 
 # testing
 auth0_test_domain: titanml.eu.auth0.com
 auth0_test_client_id: q5MTyNxFNoyULA75MspCVx0wJBqlDNhY
@@ -19,10 +20,11 @@
 prod_base: https://api.titanml.co
 
 auth0_algorithm: ['RS256']
 auth0_audience: "https://seshat/"
 auth0_flow: "device"
 
 authenticate: true
+telemetry: true
 log_level: WARNING
 
 base_image: "tytn/hephaestus:latest"
```

### Comparing `titan-iris-0.3.9a2/src/iris/main.py` & `titan-iris-0.4.0a0/src/iris/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,46 @@
-"""
-This is the main file for the sdk cli. It is responsible for handling the cli commands and passing them to the sdk module.
-"""
+"""This is the main file for the sdk cli.
 
+It is responsible for handling the cli commands and passing them to the sdk module.
+"""
+import json
+import logging
 from enum import Enum
 from logging import getLogger
 from pathlib import Path
 
 # ───────────────────────────────────────────────────── imports ────────────────────────────────────────────────────── #
 from typing import List, Optional
 
 import typer
 import yaml
-
+from trogon import Trogon
+from typer.main import get_group
 import iris.sdk as sdk
 
+from .sdk.utils import exception_to_json_error, json_output_decorator
+
 logger = getLogger(__name__)
 logger.setLevel(sdk.conf_mgr.LOG_LEVEL)
 
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 #                                                   sdk CLI Module                                                     #
 
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 
 # create the typer object
 main = typer.Typer()
 
 
 def conf_callback(ctx: typer.Context, param: typer.CallbackParam, value: str):
     """This is a typer callback that loads a yaml file (value) and uses it to override the command line arguments.
-       If this is provided as the callback for an argument with is_eager=True, it runs before loading the other arguments
-       and provides them from the yaml. If they're set manually, they get overriden in the config
+
+       If this is provided as the callback for an argument with is_eager=True,
+       it runs before loading the other arguments and provides them from the yaml.
+       If they're set manually, they get overriden in the config.
 
     Args:
         ctx (typer.Context): the typer context
         param (typer.CallbackParam): the typer param (name?)
         value (str): the value of the param (the filepath of the yaml)
 
     Raises:
@@ -54,153 +61,262 @@
         except Exception as ex:
             raise typer.BadParameter(str(ex))
     return value
 
 
 @main.command()
 def login():
-    """Login to the iris client."""
+    """Login to iris."""
     try:
         user_name = sdk.login()
         print(f"Logged in as {user_name}")
     except Exception as e:
-        typer.secho(f"Error: {e}", fg=typer.colors.RED, err=True)
-        raise typer.Exit(1)
+        json_error = exception_to_json_error(e)
+        print(json_error)
+        raise typer.Abort()
 
 
 @main.command()
 def logout():
-    """Logout from the iris client."""
+    """Logout from iris."""
     try:
         logged_out = sdk.logout()
         if logged_out:
             print("Successfully logged out")
         else:
             raise Exception("Failed to logout")
     except Exception as e:
-        typer.secho(f"Error: {e}", fg=typer.colors.RED, err=True)
-        raise typer.Exit(1)
+        json_error = exception_to_json_error(e)
+        print(json_error)
+        raise typer.Abort()
 
 
-class Task(str, Enum):
-    sequence_classification = "sequence_classification"
-    glue = "glue"
-    question_answering = "question_answering"
+@main.command()
+def version():
+    """Print the version of iris."""
+    from importlib.metadata import version
 
+    print(version("titan-iris"))
 
-class Object(str, Enum):
-    experiment = "experiment"
-    artefact = "artefact"
 
+@main.command()
+def ui(ctx: typer.Context):
+    """Run the tui.
 
-class Artefact(str, Enum):
-    model = "model"
-    dataset = "dataset"
+    Args:
+        ctx (typer.Context): The typer context
+    """
+    Trogon(get_group(main), click_context=ctx).run()
 
 
 class Task(str, Enum):
+    """The task to optimize the model for."""
+
     sequence_classification = "sequence_classification"
     glue = "glue"
     question_answering = "question_answering"
     token_classification = "token_classification"
+    language_modelling = "language_modelling"
 
 
 class Object(str, Enum):
+    """The various kinds of API objects that the TitanML platform supports."""
+
     experiment = "experiment"
     artefact = "artefact"
+    inference_session = "inference-session"
 
 
 class Artefact(str, Enum):
+    """Artefacts: models, datasets, etc."""
+
     model = "model"
     dataset = "dataset"
 
 
+# Ex-post arguments which are now shared between athena, pontus and post. Define once here to avoid duplication.
+MODEL_ARG = typer.Option(..., "--model", "-m", help="The models to optimize.")
+DATASET_ARG = typer.Option(..., "--dataset", "-d", help="The dataset to optimize the model with.")
+TASK_ARG = typer.Option(..., "--task", "-t", help="The task to optimize the model for.")
+SUBSET_ARG = typer.Option(None, "--subset", "-ss", help="The subset of a dataset to optimize on")
+NAME_ARG = typer.Option(
+    "",
+    "--name",
+    "-n",
+    help="The name to use for this job. Visible in the TitanML Hub.",
+)
+FILE_ARG = typer.Option(
+    "",
+    "--file",
+    "-f",
+    help="Load the options from a config file",
+    callback=conf_callback,
+    is_eager=True,
+)
+TEST_ARG = typer.Option(
+    False,
+    "--short-run",
+    "-s",
+    help="Truncates the run after 1 batch and 1 epoch. \
+            Will provide bad results, but useful to check that the model and dataset choices are valid.",
+)
+NUM_LABELS_ARG = typer.Option(
+    None,
+    "--num-labels",
+    "-nl",
+    help="Number of labels. Required for task sequence_classification",
+)
+
+TEXT_FIELDS_ARG = typer.Option(
+    None,
+    "--text-fields",
+    "-tf",
+    help="Text fields. Required for task sequence_classification",
+)
+
+HAS_NEGATIVE_ARG = typer.Option(
+    False,
+    "--has-negative",
+    "-hn",
+    help="Has negative. Required for question_answering",
+)
+LABEL_NAMES_ARG = typer.Option(
+    None,
+    "--label-names",
+    "-ln",
+    help="Names of token labels. Required for task token_classification. \
+            Specify as a mapping with no spaces: -ln 0:label1 -ln 1:label2",
+)
+HEADERS_ARG = typer.Option(
+    [],
+    "--headers",
+    "-H",
+    help="Headers to send with the get request. \
+            Should be provided as colon separated key value pairs: -h a:b -h c:d -> {a:b, c:d}",
+)
+
+BATCH_SIZE_ARG = typer.Option("16", "--batch-size", "-bs", help="The batch size to use for training.")
+LEARNING_RATE_ARG = typer.Option("2e-5", "--learning-rate", "-lr", help="The learning rate to use for training.")
+JSON_ARG = typer.Option(
+    False,
+    "--json",
+    "-j",
+    help="Print output as JSON. Default: Rich output",
+)
+
+
 @main.command()
 def post(
-    model: str = typer.Option(..., "--model", "-m", help="The model to optimize."),
-    dataset: str = typer.Option(
-        ..., "--dataset", "-d", help="The dataset to optimize the model with."
-    ),
-    task: Task = typer.Option(
-        ..., "--task", "-t", help="The task to optimize the model for."
-    ),
-    experiment_name: str = typer.Option(
-        "",
-        "--name",
-        "-n",
-        help="The name to use for this job. Visible in the titan web interface.",
-    ),
-    file: str = typer.Option(
-        "",
-        "--file",
-        "-f",
-        help="Load the options from a config file",
-        callback=conf_callback,
-        is_eager=True,
-    ),
-    test: bool = typer.Option(
-        False,
-        "--short-run",
-        "-s",
-        help="Truncates the run after 1 batch and 1 epoch. Will provide bad results, but useful to check that the model and dataset choices are valid.",
-    ),
-    num_labels: int = typer.Option(
-        None,
-        "--num-labels",
-        "-nl",
-        help="Number of labels. Required for task sequence_classification",
-    ),
-    text_fields: Optional[List[str]] = typer.Option(
-        None,
-        "--text-fields",
-        "-tf",
-        help="Text fields. Required for task sequence_classification",
-    ),
-    has_negative: bool = typer.Option(
-        False,
-        "--has-negative",
-        "-hn",
-        help="Has negative. Required for question_answering",
-    ),
-    label_names: Optional[List[str]] = typer.Option(
-        None,
-        "--label-names",
-        "-ln",
-        help="Names of token labels. Required for task token_classification. Specify as a mapping with no spaces: -ln 0:label1 -ln 1:label2",
-    ),
-    headers: List[str] = typer.Option(
-        [],
-        "--headers",
-        "-h",
-        help="Headers to send with the get request. Should be provided as colon separated key value pairs: -h a:b -h c:d -> {a:b, c:d}",
-    ),
+    model: str = MODEL_ARG,
+    dataset: str = DATASET_ARG,
+    task: Task = TASK_ARG,
+    subset: Optional[str] = SUBSET_ARG,
+    experiment_name: str = NAME_ARG,
+    file: str = FILE_ARG,
+    test: bool = TEST_ARG,
+    num_labels: int = NUM_LABELS_ARG,
+    text_fields: Optional[List[str]] = TEXT_FIELDS_ARG,
+    has_negative: bool = HAS_NEGATIVE_ARG,
+    label_names: Optional[List[str]] = LABEL_NAMES_ARG,
+    headers: List[str] = HEADERS_ARG,
+    json_output: bool = JSON_ARG,
+):
+    """Submit a pipelining job (currently defaults to distillation)."""
+    dispatch("athena", **locals(), batch_size="auto", learning_rate=None, num_epochs="5")
+
+
+@main.command()
+def distil(
+    model: str = MODEL_ARG,
+    dataset: str = DATASET_ARG,
+    task: Task = TASK_ARG,
+    subset: Optional[str] = SUBSET_ARG,
+    experiment_name: str = NAME_ARG,
+    file: str = FILE_ARG,
+    test: bool = TEST_ARG,
+    num_labels: int = NUM_LABELS_ARG,
+    text_fields: Optional[List[str]] = TEXT_FIELDS_ARG,
+    has_negative: bool = HAS_NEGATIVE_ARG,
+    label_names: Optional[List[str]] = LABEL_NAMES_ARG,
+    headers: List[str] = HEADERS_ARG,
+    json_output: bool = JSON_ARG,
+):
+    """Submit a knowledge distillation job."""
+    dispatch("athena", **locals(), batch_size=None, learning_rate=None, num_epochs="5")
+
+
+@main.command()
+def finetune(
+    model: str = MODEL_ARG,
+    dataset: str = DATASET_ARG,
+    task: Task = TASK_ARG,
+    subset: Optional[str] = SUBSET_ARG,
+    experiment_name: str = NAME_ARG,
+    test: bool = TEST_ARG,
+    num_labels: int = NUM_LABELS_ARG,
+    text_fields: Optional[List[str]] = TEXT_FIELDS_ARG,
+    has_negative: bool = HAS_NEGATIVE_ARG,
+    label_names: Optional[List[str]] = LABEL_NAMES_ARG,
+    headers: List[str] = HEADERS_ARG,
+    batch_size: str = BATCH_SIZE_ARG,
+    learning_rate: float = LEARNING_RATE_ARG,
+    json_output: bool = JSON_ARG,
+    num_epochs: str = typer.Option(3, "--num-epochs", "-ep", help="The number of epochs to finetune for."),
+    file: str = FILE_ARG,
+):
+    """Submit a finetuning job."""
+    dispatch("pontus", **locals())
+
+
+def dispatch(
+    type,
+    model,
+    dataset,
+    task,
+    subset,
+    experiment_name,
+    file,
+    test,
+    num_labels,
+    text_fields,
+    has_negative,
+    label_names,
+    headers,
+    batch_size,
+    learning_rate,
+    num_epochs,
+    json_output,
 ):
-    """Dispatch a job to the titan platform"""
+    """Dispatch a job to the TitanML platform. Distil, Post and Athena ultimately run through here."""
     # get the enum value as task
     headers = {x.partition(":")[0]: x.partition(":")[-1] for x in headers}
     task = task.value
     try:
         # baseline flags
-        flags = {"model": model, "dataset": dataset, "task": task, "test": test}
+        flags = {
+            "model": model,
+            "dataset": dataset,
+            "task": task,
+            "test": test,
+            "subset": subset,
+            "type": type,
+            "num_epochs": num_epochs,
+        }
         # lots of argument checking
         if experiment_name != "":
             flags.update({"name": experiment_name})
         if task == "sequence_classification":
             # sequence of task specific flags
             # if the flag shouldn't be accepted, set error_message to the error string to print.
             # if it should be, and you want to warn, print, but don't set error_message
             error_message = False
             if num_labels is None:
-                error_message = (
-                    "Please provide the number of labels (--num-labels, -nl)"
-                )
-            if text_fields is None:
-                error_message = (
-                    "Please provide the text fields to tokenize (--text-fields, -tf)"
-                )
+                error_message = "Please provide the number of labels (--num-labels, -nl)"
+            if text_fields is None or len(text_fields) == 0:
+                error_message = "Please provide the text fields to tokenize (--text-fields, -tf)"
             if label_names is not None and len(label_names) > 0:
                 print("label_names is not necessary for sequence classification tasks")
             if has_negative:
                 print("has_negative is not necessary for sequence classification tasks")
             if error_message:
                 raise typer.Abort(error_message)
             else:
@@ -237,50 +353,88 @@
                 raise typer.Abort()
             else:
                 pass
         elif task == "token_classification":
             error_message = False
             if num_labels is not None:
                 print("num_labels is not necessary for token classification tasks")
-            if text_fields is None:
-                error_message = (
-                    "Please provide the text fields to tokenize (--text-fields, -tf)"
-                )
             if label_names is None:
                 error_message = "Please provide the label names of the tokens"
             if not all(":" in x for x in label_names):
                 error_message = "Label names should be specified as a map, e.g. '-ln 0:PER -ln 1:ORG ...'"
             if error_message:
                 raise typer.Abort(error_message)
             else:
-                label_names_dict = {
-                    int(i): label
-                    for i, label in map(lambda x: x.split(":"), label_names)
-                }
+                label_names_dict = {int(i): label for i, label in map(lambda x: x.split(":"), label_names)}
                 label_names_num = len(list(label_names_dict.keys()))
                 max_label_num = max(i for i in label_names_dict.keys())
                 min_label_num = min(i for i in label_names_dict.keys())
                 if max_label_num != (len(list(label_names_dict.keys())) - 1):
                     print("Label names must have continuous indices")
                     raise typer.Abort()
 
                 if min_label_num != 0:
                     print("Label indices must start at zero")
                     raise typer.Abort()
 
                 label_names_list = [label_names_dict[i] for i in range(label_names_num)]
                 flags.update({"label_names": label_names_list})
+
+        elif task == "language_modelling" or task == "language_modeling":
+            # sequence of task specific flags
+            # if the flag shouldn't be accepted, set error_message to the error string to print.
+            # if it should be, and you want to warn, print, but don't set error_message
+            error_message = False
+            if type == "athena":
+                error_message = "Knowledge distillation is not yet supported for language modelling."
+            if num_labels is not None:
+                print("num_labels is not necessary for language modelling tasks")
+            if label_names is not None and len(label_names) > 0:
+                print("label_names is not necessary for language modelling tasks")
+            if has_negative:
+                print("has_negative is not necessary for language modelling tasks")
+            if error_message:
+                raise typer.Abort(error_message)
+            else:
+                flags.update({"text_fields": text_fields})
         else:
             print(f"Unrecognised task {task}")
             raise typer.Abort()
+
+        if num_epochs.isdigit() and int(num_epochs) >= 99:
+            logging.warning(
+                "Woah there cowboy, that's a mighty high number of epochs you got there. "
+                "Are you sure you didn't mistype it?"
+            )
+        if batch_size:
+            if batch_size == "auto":
+                flags["batch_size"] = batch_size
+            elif "." not in batch_size and batch_size.isdigit():
+                n = int(batch_size)
+                if not ((n != 0) and (n & (n - 1) == 0)):  # Check if batch size is power of 2.
+                    print(
+                        "Note that batch sizes which are a base-2 value (2,4,16,32,64,128...) will result in faster "
+                        "training."
+                    )
+                flags["batch_size"] = int(batch_size)
+            else:
+                print(f"Unrecognised batch size format {batch_size}")
+                raise typer.Abort()
+
+        if learning_rate:
+            try:
+                flags["learning_rate"] = float(learning_rate)
+            except ValueError:
+                print(f"Unrecognised learning rate format {batch_size}")
+                raise typer.Abort()
+
         # post the resulting flags
-        sdk.post(headers, **flags)
-    except Exception as e:
-        typer.secho(f"Error: {e}", fg=typer.colors.RED, err=True)
-        raise typer.Exit(1)
+        sdk.post(headers, **flags, json_output=json_output)
+    except Exception:
+        raise typer.Abort()
 
 
 @main.command()
 def get(
     object: Object = typer.Argument("experiment", help="What type of object to get"),
     id: Optional[str] = typer.Option(
         None,
@@ -290,203 +444,221 @@
     ),
     query: Optional[str] = typer.Option(
         None,
         "--query",
         "-q",
         help="A JMESPath string, to filter the objects returned by the API. Evaluated client-side.",
     ),
-    headers: List[str] = typer.Option(
-        [],
-        "--headers",
-        "-h",
-        help="Headers to send with the get request. Should be provided as colon separated key value pairs: -h a:b -h c:d -> {a:b, c:d}",
-    ),
+    headers: List[str] = HEADERS_ARG,
+    json_output: Optional[bool] = JSON_ARG,
 ):
-    """Get objects from the TYTN api."""
+    """Get objects from the TitanML Store."""
     # get the string from the enum
     headers = {x.partition(":")[0]: x.partition(":")[-1] for x in headers}
     object = object.value
     try:
-        sdk.get(object, id, query, headers)
-    except Exception as e:
-        typer.secho(f"Error: {e}", fg=typer.colors.RED, err=True)
-        raise typer.Exit(1)
+        sdk.get(object, id, query, headers, json_output=json_output)
+    except Exception:
+        raise typer.Abort()
 
 
 @main.command()
 def delete(
     object: Object = typer.Argument("experiment", help="What type of object to delete"),
     id: Optional[str] = typer.Option(
         ...,
         "--id",
         "-i",
         help="Which object to delete",
     ),
+    json_output: bool = JSON_ARG,
 ):
-    """delete objects from the TYTN api."""
+    """Delete objects from the TitanML store."""
     # delete the string from the enum
     object = object.value
     try:
-        response = sdk.delete(object, id)
-        print(response)
-    except Exception as e:
-        typer.secho(f"Error: {e}", fg=typer.colors.RED, err=True)
-        raise typer.Exit(1)
+        sdk.delete(object, id, verbose=True, json_output=json_output)
+    except Exception:
+        raise typer.Abort()
 
 
 @main.command()
 def pull(
-    image: str = typer.Argument(
-        ..., help="The image to pull. Should be displayed in the titan web interface."
-    )
+    image: str = typer.Argument(..., help="The image to pull. Should be displayed in the TitanML Hub."),
+    json_output: bool = JSON_ARG,
 ):
     """Pull the titan-optimized server docker image."""
     try:
-        sdk.pull(image)
+        sdk.pull(image, json_output=json_output)
     except Exception as e:
-        typer.secho(f"Error: {e}", fg=typer.colors.RED, err=True)
-        raise typer.Exit(1)
+        json_error = exception_to_json_error(e)
+        print(json_error)
+        raise typer.Abort()
 
 
 @main.command()
 def download(
-    image: str = typer.Argument(
-        ..., help="The model to pull. Should be displayed in the titan web interface."
-    )
+    image: str = typer.Argument(..., help="The model to pull. Should be displayed in the TitanML Hub."),
+    json_output: bool = JSON_ARG,
 ):
     """Download the titan-optimized onnx model."""
     try:
-        sdk.download(image)
+        sdk.download(image, json_output=json_output)
     except Exception as e:
-        typer.secho(f"Error: {e}", fg=typer.colors.RED, err=True)
-        raise typer.Exit(1)
+        json_error = exception_to_json_error(e)
+        print(json_error)
+        raise typer.Abort()
 
 
 @main.command()
 def infer(
-    target: str = typer.Option(
-        "localhost", "--target", help="The url to run the server on."
-    ),
-    port: int = typer.Option(
-        8000, "--port", "-p", help="The port to run the server on."
-    ),
-    task: Task = typer.Option(
-        ..., "--task", "-t", help="The task to optimize the model for."
-    ),
-    use_cpu: bool = typer.Option(
-        False,
-        "--use-cpu",
-        help="Whether to use the CPU. If False, the GPU will be used. Choose CPU only when the opmitized model is in CPU format(OnnxRuntime). The default will be False. (using TensorRT)  ",
+    target: str = typer.Option("localhost", "--target", help="The url to run the server on."),
+    port: int = typer.Option(8000, "--port", "-p", help="The port to run the server on."),
+    task: Task = typer.Option(..., "--task", help="The task to optimize the model for."),
+    runtime: str = typer.Option(
+        "trt",
+        "--runtime",
+        help="The runtime to use. Can be one of 'trt', 'onnx'. Defaults to 'trt'.",
     ),
     text: List[str] = typer.Option(
         ...,
         "--text",
-        "-t",
-        help="The text to run the server in. In classification tasks, this is the TEXT to be classified. In question answering tasks, this is the QUESTION to be answered.",
+        help="The text to run the server in. In classification tasks, this is the TEXT to be classified. \
+            In question answering tasks, this is the QUESTION to be answered.",
     ),
     context: Optional[str] = typer.Option(
         "",
         "--context",
         "-c",
         help="The context in question answering tasks. Only used in question answering tasks.",
     ),
 ):
     """Run inference on a model."""
-
     url = f"{target}:{port}"
+
     try:
         if task == "sequence_classification":
             if context is None or context != "":
                 print("context is not necessary for classification tasks")
                 raise typer.Abort()
-            res = sdk.infer(url, task, use_cpu, text)
+            res = sdk.infer(url, task, runtime, text)
             print(res)
         elif task == "question_answering":
             if context is None or context == "":
                 print("context is required for question answering tasks")
                 raise typer.Abort()
             if len(text) != 1:
                 print("text should only contain one question")
                 raise typer.Abort()
-            res = sdk.infer(url, task, use_cpu, text, context)
+            res = sdk.infer(url, task, runtime, text, context)
             print(res)
         else:
             print(f"Unrecognised task {task}")
             raise typer.Abort()
     except Exception as e:
-        typer.secho(f"Error: {e}", fg=typer.colors.RED, err=True)
-        raise typer.Exit(1) from e
+        json_error = exception_to_json_error(e)
+        print(json_error)
+        raise typer.Abort() from e
+
+
+@main.command()
+def demo(
+    target: str = typer.Option("localhost", "--target", help="The url to run the server on."),
+    port: int = typer.Option(8000, "--port", "-p", help="The port to run the server on."),
+):
+    """Run the gradio demo.
+
+    Here the target and port are the same as the infer command, which is where the triton server is running.
+    The default is localhost:8000.
+    """
+    url = f"{target}:{port}"
+    try:
+        from iris.gradio.run import run
+
+        run(url)
+    except Exception as e:
+        json_error = exception_to_json_error(e)
+        print(json_error)
+        raise typer.Abort()
 
 
 @main.command()
 def upload(
     src: Path = typer.Argument(
         ...,
-        help="The location of the artefact on disk. Should be a folder, containing either a model or a dataset. For more information on the supported formats, see the titan documentation.",
-    ),
-    name: str = typer.Argument(
-        None, help="The name of the artefact. Displayed in the titan web interface."
+        help="The location of the artefact on disk. Should be a folder, containing either a model or a dataset.\
+              For more information on the supported formats, see the TitanML documentation.",
     ),
+    name: str = typer.Argument(None, help="The name of the artefact. Displayed in the TitanML Hub."),
     description: str = typer.Argument(
         None,
-        help="A short description of the artefact. Displayed in the titan web interface.",
+        help="A short description of the artefact. Displayed in the TitanML Hub.",
+    ),
+    json_output: bool = typer.Option(
+        False,
+        "--json",
+        "-j",
+        help="Print output as JSON (default: Rich output)",
     ),
 ):
-    """Upload an artefact to the titan hub."""
+    """Upload an artefact to the TitanML Hub."""
     try:
-        sdk.upload(name, src, description)
+        sdk.upload(name, src, description, json_output=json_output)
     except Exception as e:
-        typer.secho(f"Error: {e}", fg=typer.colors.RED, err=True)
-        raise typer.Exit(1)
+        json_error = exception_to_json_error(e)
+        print(json_error)
+        raise typer.Abort()
 
 
+@json_output_decorator
 @main.command()
 def status(
-    id: int = typer.Option(
-        ..., "--id", "-i", help="The id of the experiment to get the status of"
-    ),
-    headers: List[str] = typer.Option(
-        [],
-        "--headers",
-        "-h",
-        help="Headers to send with the get request. Should be provided as colon separated key value pairs: -h a:b -h c:d -> {a:b, c:d}",
-    ),
+    id: str = typer.Option(..., "--id", "-i", help="The id of the experiment to get the status of"),
+    headers: List[str] = HEADERS_ARG,
+    json_output: bool = JSON_ARG,
 ):
-    """Get the status of an experiment"""
+    """Get the status of an experiment."""
     headers = {x.partition(":")[0]: x.partition(":")[-1] for x in headers}
+    summary = ""
     try:
         summary = sdk.get(
             "experiment",
             id,
             "experiment.jobs[*].{name:name, status:status, message:message, results:results}",
-            verbose=False,
-            headers=headers,
+            headers,
+            json_output=json_output,
         )
-        tag_from_name = (
-            lambda name: name.partition("-")[0] + ":" + name.rpartition("_")[-1]
-        )
-        import json
-
-        response = json.loads(summary)["response"]
-        for i in range(len(response)):
-            response[i]["name"] = tag_from_name(response[i]["name"])
-        response = json.dumps(response, indent=4)
-        print(response)
-    except Exception as e:
-        typer.secho(f"Error: {e}", fg=typer.colors.RED, err=True)
-        raise typer.Exit(1)
+        return summary
+    except Exception:
+        raise typer.Abort()
 
 
 @main.command()
 def makesafe(
     model: str = typer.Argument("model", help="The model to convert to safe_tensors"),
 ):
     """Convert a non-safetensor model into a safetensor model, including for models with shared weights."""
     try:
         sdk.makesafe(model)
     except Exception as e:
-        typer.secho(f"Error: {e}", fg=typer.colors.RED, err=True)
-        raise typer.Exit(1)
+        json_error = exception_to_json_error(e)
+        print(json_error)
+        raise typer.Abort()
+
+
+@main.command()
+def query(artefact_id: str, data: str = typer.Option("", "--data", "-d")):
+    """Create/query an inference endpoint for a given model.
+
+    The data should be a json string, with the following format:
+    """
+    try:
+        data = json.dumps(data)
+    except Exception:
+        print({"status": "Failed", "message": "data should be a json string"})
+        raise typer.Abort()
+    response = sdk.query(artefact_id, data)
+    print(response)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `titan-iris-0.3.9a2/src/iris/sdk/auth_utils.py` & `titan-iris-0.4.0a0/src/iris/sdk/auth_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-This module contains the authentication utils for the iris package
-"""
+"""This module contains the authentication utils for the iris package."""
 # ───────────────────────────────────────────────────── imports ────────────────────────────────────────────────────── #
 
 import functools
 import json
 import logging
 import os
 import time
+from pathlib import Path
+from typing import Union
 
 import jwt
 import requests
 import typer
 from auth0.v3.authentication.token_verifier import (
     AsymmetricSignatureVerifier,
     TokenVerifier,
 )
+from requests import Response
 from rich import print
 
 from .conf_manager import conf_mgr
 
 # internal imports
 from .exception import (
     EndpointNotFoundError,
     InvalidLoginError,
     KeyFileDoesntExistError,
     KeyFileExpiredError,
-    UnprocessableEntityError,
 )
 
 # Logger config
 logging.basicConfig(
     format="%(asctime)s - %(levelname)s - %(name)s - %(message)s",
     datefmt="%m/%d/%Y %H:%M:%S",
 )
@@ -39,42 +39,41 @@
 
 
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 #                                                      Auth Utils                                                      #
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 
 
-def validate_token(id_token):
-    """
-    Verify the token and its precedence
-    :param id_token:
+def validate_token(id_token: str) -> None:
+    """Verify the token and its precedence.
+
+    Args:
+        id_token (str): The token to be verified
     """
     jwks_url = f"https://{conf_mgr.AUTH0_DOMAIN}/.well-known/jwks.json"
     issuer = f"https://{conf_mgr.AUTH0_DOMAIN}/"
     sv = AsymmetricSignatureVerifier(jwks_url)
-    tv = TokenVerifier(
-        signature_verifier=sv, issuer=issuer, audience=conf_mgr.AUTH0_CLIENT_ID
-    )
+    tv = TokenVerifier(signature_verifier=sv, issuer=issuer, audience=conf_mgr.AUTH0_CLIENT_ID)
     tv.verify(id_token)
 
 
-def client_credentials_flow():
+def client_credentials_flow() -> None:
+    """Runs the client credentials flow and stores the user object in the keyfile.
+
+    Raises:
+        InvalidLoginError: If there's an error during login
+    """
     logger.debug("starting client_credentials_flow")
-    try:
-        client_id = os.environ["AUTH0_CLIENT_ID"]
-    except KeyError:
-        raise InvalidLoginError(
-            "AUTH0_CLIENT_ID must be provided as an environment variable when client_credentials_flow is used"
-        )
+    client_id = conf_mgr.AUTH0_CLIENT_ID
 
     try:
-        client_secret = os.environ["AUTH0_CLIENT_SECRET"]
+        client_secret = os.environ["IRIS_AUTH0_CLIENT_SECRET"]
     except KeyError:
         raise InvalidLoginError(
-            "AUTH0_CLIENT_SECRET must be provided as an environment variable when client_credentials_flow is used"
+            "IRIS_AUTH0_CLIENT_SECRET must be provided as an environment variable when client_credentials_flow is used"
         )
 
     url = f"https://{conf_mgr.AUTH0_DOMAIN}/oauth/token"
     payload = {
         "client_id": client_id,
         "client_secret": client_secret,
         "audience": "https://seshat/",
@@ -84,20 +83,20 @@
     headers = {"content-type": "application/json"}
 
     response = requests.post(url, json=payload, headers=headers)
 
     token_data = response.json()
 
     conf_mgr.access_token = token_data.get("access_token", None)
-    conf_mgr.current_user = os.environ["AUTH0_CLIENT_ID"]
+    conf_mgr.current_user = client_id
 
 
-def device_authorization_flow():
-    """
-    Runs the device authorization flow and stores the user object in memory
+def device_authorization_flow() -> None:
+    """Runs the device authorization flow and stores the user object in the keyfile.
+
     Prints (by design) since it's an interactive flow.
     """
     logger.debug("initiating device authorization flow")
     device_code_payload = {
         "client_id": conf_mgr.AUTH0_CLIENT_ID,
         "scope": "openid profile",
         "audience": conf_mgr.AUTH0_AUDIENCE,
@@ -128,20 +127,16 @@
     }
 
     authenticated = False
     time_waited = 0
     while not authenticated:
         logger.debug(f"Waiting for input... {time_waited}s")
 
-        logger.debug(
-            f"Posting {token_payload} to https://{conf_mgr.AUTH0_DOMAIN}/oauth/token"
-        )
-        token_response = requests.post(
-            f"https://{conf_mgr.AUTH0_DOMAIN}/oauth/token", data=token_payload
-        )
+        logger.debug(f"Posting {token_payload} to https://{conf_mgr.AUTH0_DOMAIN}/oauth/token")
+        token_response = requests.post(f"https://{conf_mgr.AUTH0_DOMAIN}/oauth/token", data=token_payload)
 
         token_data = token_response.json()
 
         if token_response.status_code == 200:
             validate_token(token_data["id_token"])
 
             logger.debug("Token verified!")
@@ -160,90 +155,107 @@
             print(token_data["error_description"])
             raise typer.Exit(code=1)
         else:
             time.sleep(device_code_data["interval"])
             time_waited += device_code_data["interval"]
 
 
-def store_credentials(filename):
+def store_credentials(filename: Union[Path, str]) -> None:
+    """Store the credentials in filename.
+
+    Args:
+        filename (Path | str): The filename in which to store the credentials.
+    """
     json.dump(
         {"current_user": conf_mgr.current_user, "access_token": conf_mgr.access_token},
         open(filename, "w"),
     )
 
 
-def load_credentials(filename):
+def load_credentials(filename: Union[Path, str]) -> None:
+    """Load the credentials from filename.
+
+    Args:
+        filename (Path | str): The filename from which to load the credentials.
+
+    Raises:
+        KeyFileDoesntExistError: _description_
+    """
     try:
         credentials = json.load(open(filename, "r"))
     except FileNotFoundError:
         logger.debug("Keyfile doesnt exist")
         raise KeyFileDoesntExistError
 
     conf_mgr.current_user = credentials["current_user"]
     conf_mgr.access_token = credentials["access_token"]
 
 
 def auth(fn: callable):
-    """A decorator to add the key to the function kwargs
+    """A decorator to add the key from the storage to the function kwargs.
+
+    Reruns the login flow on expiry
+
     Args:
         fn (callable): The function to decorate
     Returns:
-        callable: The decorated function
+        callable: The decorated function.
     """
 
     @functools.wraps(fn)
     def auth0_wrapper(*args, **kwargs):
         if conf_mgr.CREDENTIALS_FLOW == "device":
             try:
-                logger.debug(f"Loading credentials from conf_mgr.CREDENTIALS_PATH")
+                logger.debug("Loading credentials from conf_mgr.CREDENTIALS_PATH")
                 logger.debug(f"{conf_mgr.current_user}")
                 load_credentials(conf_mgr.CREDENTIALS_PATH)
 
                 expired = conf_mgr.current_user["exp"] < time.time()
-                logger.debug(
-                    f"Expired: {expired}: {conf_mgr.current_user['exp']}, {time.time()}"
-                )
+                logger.debug(f"Expired: {expired}: {conf_mgr.current_user['exp']}, {time.time()}")
                 if expired:
                     print("Credentials expired. Please login again.")
                     raise KeyFileExpiredError
-            except (KeyFileDoesntExistError, KeyFileExpiredError) as e:
+            except (KeyFileDoesntExistError, KeyFileExpiredError):
                 # if the keyfile doesn't exist, or the keyfile has expired, try and login
                 try:
                     device_authorization_flow()
                 except Exception as e:
                     # if we can't login, just reraise
                     raise e
                 else:
                     # on successful login, store the credentials
-                    store_credentials(
-                        conf_mgr.CREDENTIALS_PATH
-                    )  # store if no errors in login
+                    store_credentials(conf_mgr.CREDENTIALS_PATH)  # store if no errors in login
 
         elif conf_mgr.CREDENTIALS_FLOW == "client_credentials":
             logger.info(f"authenticating with {conf_mgr.CREDENTIALS_FLOW} flow")
             # no storing credentials for client_credentials flow
             client_credentials_flow()
         else:
             raise ValueError(f"Flow {conf_mgr.CREDENTIALS_FLOW} not recognised")
         return fn(*args, **kwargs)
 
     @functools.wraps(fn)
     def dummy_wrapper(*args, **kwargs):
+        """Dummy wrapper, if authenticate is disabled.
+
+        Args:
+            *args: The args to pass to the function
+            **kwargs: The kwargs to pass to the function
+        """
         logger.debug("in dummy wrapper")
         return fn(*args, **kwargs)
 
     # if conf_mgr.AUTHENTICATE is not set, then don't set the token
     # on the config manager, and don't send it on requests.
     # NOTE: This will likely cause those requests to fail.
     return auth0_wrapper if conf_mgr.AUTHENTICATE else dummy_wrapper
 
 
-def handle_bad_response(response, endpoint):
-    """Given a bad response from endpoint, return
-       an appropriate exception
+def handle_bad_response(response: Response, endpoint: str):
+    """Given a bad response from endpoint, return an appropriate exception.
 
     Args:
         response (requests.Response): the response object
         endpoint (str): The endpoint that was queried for the response
 
     Returns:
         Exception: The exception to handle.
```

### Comparing `titan-iris-0.3.9a2/src/iris/sdk/exception.py` & `titan-iris-0.4.0a0/src/iris/sdk/exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-"""
-Iris Exception Types
-"""
+"""Iris Exception Types."""
 # ───────────────────────────────────────────────────── imports ────────────────────────────────────────────────────── #
 
 from typing import Optional
 
-
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 #                                                Iris Exception Types                                                  #
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 
 
 class IrisException(Exception):
-    """Error raised when occurs an unidentified internal error in the iris package"""
+    """Error raised when occurs an unidentified internal error in the iris package."""
 
     message = "Iris Command Error"
 
     def __init__(self, message: Optional[str] = None, details: Optional[str] = None):
-        """
+        """Create an IrisException.
+
         Args:
             message (str): Error message. This will replace the defined class message.
             details (str): Details about the error.
         """
         self.message = self._compose_message(message=message, details=details)
         super().__init__(self.message)
 
     def __str__(self):
+        """String representation of the error."""
         return self.message
 
-    def _compose_message(
-        self, message: Optional[str] = None, details: Optional[str] = None
-    ) -> str:
-        """Composition of the error message
+    def _compose_message(self, message: Optional[str] = None, details: Optional[str] = None) -> str:
+        """Composition of the error message.
 
         Args:
             message (str): Error message. This will replace the defined class message.
             details (str): Details about the error.
 
         Returns:
             message (str): A message  error with the following format:
@@ -44,110 +41,119 @@
         return " - ".join([msg for msg in [message or self.message, details] if msg])
 
 
 # ────────────────────────────────────────────── BAD REQUEST Exceptions ────────────────────────────────────────────── #
 
 
 class InvalidLoginError(IrisException):
-    """Error raised when the login is invalid"""
+    """Error raised when the login is invalid."""
 
     message = "Invalid login credentials. Are you logged in?"
 
 
 class EndpointNotFoundError(IrisException):
-    """Error raised when the endpoint is not found"""
+    """Error raised when the endpoint is not found."""
 
     message = "Endpoint not found: "
 
 
 class BadRequestError(IrisException):
-    """Error raised when there are input data errors"""
+    """Error raised when there are input data errors."""
 
     message = "Bad request error. Please check your input data"
 
 
 class UnprocessableEntityError(IrisException):
-    """Error raised when there are input data errors"""
+    """Error raised when there are input data errors."""
 
     message = "Unprocessable entity error. Please check your input data"
 
 
 class DownloadLinkNotFoundError(IrisException):
-    """Error raised when the download link is not found"""
+    """Error raised when the download link is not found."""
 
     message = "Download link not found"
 
 
 class KeyFileDoesntExistError(IrisException):
-    """Error raised when the keyfile is not found, which means that the user is not logged in"""
+    """Error raised when the keyfile is not found, which means that the user is not logged in."""
 
     message = "Keyfile doesn't exist. User should login"
 
 
 class KeyFileExpiredError(IrisException):
-    """Error raised when the user stored key has expired"""
+    """Error raised when the user stored key has expired."""
 
     message = "Stored key has expired. Please login again"
 
 
 class InvalidCommandError(IrisException):
-    """Error raised when the command is invalid"""
+    """Error raised when the command is invalid."""
 
     message = "Invalid command. Please check your command again!"
 
 
 class DownloadLinkExpiredError(IrisException):
-    """Error raised when the download link is expired"""
+    """Error raised when the download link is expired."""
 
     message = "This download link is already expired. This expire time is: "
 
 
 class ArtefactNotFoundError(IrisException):
-    """Error raised when attempting to upload a nonexistent artefact"""
+    """Error raised when attempting to upload a nonexistent artefact."""
 
     message = "File not found"
 
 
 class ArtefactTypeNotAFolderError(IrisException):
-    """Error raised when attempting to upload an artefact which is not a folder"""
+    """Error raised when attempting to upload an artefact which is not a folder."""
 
     message = "Only directories are supported as a container for artefact uploads."
 
 
 class ArtefactTypeInferError(IrisException):
-    """Error raised when attempting to upload an artefact whose type cannot be ascertained due to lacking the format to
-    be considered any of the artefact types."""
+    """Artefact type inference error.
+
+    Error raised when attempting to upload an artefact whose type
+    cannot be ascertained due to lacking the format to be considered any of the artefact types.
+    """
 
     message = "The contents of the given directory do not match the format of any permitted artefact type."
 
 
 class UnsafeTensorsError(IrisException):
-    """Error raised when attempting to upload a model (artefact) which does not contain a .safetensors file"""
+    """Error raised when attempting to upload a model (artefact) which does not contain a .safetensors file."""
 
     message = (
         "Only models safely saved using safetensors are compatible. Use Iris makesafe <model> to convert the model, "
         "or see https://huggingface.co/docs/safetensors/index"
     )
 
 
 class MissingTokenizerError(IrisException):
-    """Error raised when attempting to upload a model (artefact) which doesn't have a tokenizer"""
+    """Error raised when attempting to upload a model (artefact) which doesn't have a tokenizer."""
 
     message = "Only models saved alongside tokenizers are compatible."
 
 
 class InvalidDatasetFormatError(IrisException):
-    """Error raised when a dataset is missing train.csv and val.csv"""
+    """Error raised when a dataset is missing train.csv and val.csv."""
 
     message = "Folders with (at least) train.csv and val.csv are the only permitted formats for datasets"
 
 
 class UnknownFamilyError(IrisException):
-    """Error raised when a model's tokenizer_config.json file has a missing or unrecognised 'tokenizer_class'"""
+    """Error raised when a model's tokenizer_config.json file has a missing or unrecognised 'tokenizer_class'."""
 
     message = "Unrecognized tokenizer class"
 
 
 class UploadOnPostError(IrisException):
-    """Error raised when a local model provided to Iris Post for upload fails to upload properly"""
+    """Error raised when a local model provided to Iris Post for upload fails to upload properly."""
 
     message = "Specified local model could not be uploaded. Try 'iris upload <model>' for a more specific diagnosis'"
+
+
+class JobStillRunningError(IrisException):
+    """Error raised when a job is still running."""
+
+    message = "Job still running. Please wait until it finishes."
```

### Comparing `titan-iris-0.3.9a2/src/iris/sdk/iris_sdk.py` & `titan-iris-0.4.0a0/src/iris/sdk/iris_sdk.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,143 @@
-"""
-This module will contain all the sdk functions for the iris command sdk, including login, logout, get, post, pull.
-"""
+"""This module will contain all the sdk functions for the iris command sdk, including login, logout, get, post, pull."""
 import ast
 import hashlib
 import json
 import logging
 import os
 from datetime import datetime
+from importlib import util
 from pathlib import Path
 from typing import List, Optional, Union
 from urllib.parse import urljoin
-from importlib import util
 
 # for iris infer
 import numpy as np
 
 # for iris pull
 import requests
 import tritonclient.http
 from rich import print
+from rich.console import Console
+from rich.table import Table
 
 # internal imports
 from .auth_utils import auth, handle_bad_response
 from .conf_manager import conf_mgr
 from .exception import (
     ArtefactNotFoundError,
+    ArtefactTypeInferError,
     ArtefactTypeNotAFolderError,
     BadRequestError,
     InvalidCommandError,
     InvalidDatasetFormatError,
+    JobStillRunningError,
     MissingTokenizerError,
+    UnknownFamilyError,
     UnsafeTensorsError,
     UploadOnPostError,
-    ArtefactTypeInferError,
-    UnknownFamilyError,
 )
-from .utils import download_model, dump, pull_image, make_targz, upload_from_file
+from .utils import (
+    download_model,
+    dump,
+    json_output_decorator,
+    make_targz,
+    pull_image,
+    telemetry_decorator,
+    upload_from_file,
+)
+
+try:
+    from importlib import metadata
+except ImportError:  # for Python<3.8
+    import importlib_metadata as metadata
+
 
 # ───────────────────────────────────────────────────── imports ────────────────────────────────────────────────────── #
 
 
 # Whether to use tqdm for progress bars
 TQDM = True
 
 # ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 #                                                  IRIS USERS SDK                                                     #
 # ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 
-
 # ------------------------------------      Setup Logger      ------------------------------------ #
 # Logger config
 logging.basicConfig(
     format="%(asctime)s - %(levelname)s - %(name)s - %(message)s",
     datefmt="%m/%d/%Y %H:%M:%S",
 )
 logger = logging.getLogger(__name__)
 logger.setLevel(conf_mgr.LOG_LEVEL)
 
 
 # --------------------------------------      iris login    -------------------------------------- #
 @auth
 def login():
+    """Login to Iris."""
     logger.debug("logging in")
     return conf_mgr.current_user["name"]
 
 
 # --------------------------------------     iris logout    -------------------------------------- #
 
 
 def logout():
+    """Logout from iris.
+
+    Just deletes the keyfile.
+    """
     logger.info("logging out")
     path = Path.home() / Path(conf_mgr.config.keyfile_name)
     if path.exists():
         path.unlink()
     if not path.exists():
         return True
     else:
         return False
 
 
 # --------------------------------------      iris post     -------------------------------------- #
 
 
 @auth
-def post(headers: dict = {}, **flags):
+@telemetry_decorator
+@json_output_decorator
+def post(
+    headers: dict = None,
+    json_output: bool = False,
+    **flags: dict,
+) -> None:
+    """Dispatch a job to iris.
+
+    Args:
+        headers (dict, optional): Additional headers to add. Defaults to {}.
+        json_output(bool, optional): Whether to return the response as a json object. Defaults to False.
+        **flags (dict): The flags to send to the server. These must conform to the API specification.
+
+    Raises:
+        UploadOnPostError: If there's an error uploading the artefact.
+        handle_bad_response(...): If there's a bad response from the server.
+    """
+    if headers is None:
+        headers = {}
     endpoint = "experiment"
     # detype the flags, so we can send them
-    payload = {k: str(val) for k, val in flags.items()}
+    payload = {k: str(val) if val is not None else None for k, val in flags.items()}
     logger.debug(f"Dispatching job with payload {payload}")
     url = urljoin(conf_mgr.runner_url, f"{endpoint}/")
 
     for local_artefact_field in ["model", "dataset"]:
         local_artefact = payload[local_artefact_field]
         if os.path.exists(local_artefact):
             print(
-                f"Local {local_artefact_field} found. If you intended to use a huggingface module then rename the local file."
+                f"Local {local_artefact_field} found. \
+                If you intended to use a huggingface module then rename the local file."
             )  # todo
             local_uuid = upload(
                 name=local_artefact.split("/")[-1],
                 src=local_artefact,
                 description="Experiment model",
                 internal_artefact_type=local_artefact_field,
             )  # todo add more data to the uploaded model?
@@ -106,280 +145,321 @@
                 payload[local_artefact_field] = local_uuid
             else:
                 raise UploadOnPostError
 
     headers.update({"Authorization": f"Bearer {conf_mgr.access_token}"})
     response = requests.post(url=url, headers=headers, data=payload)
     if not response.ok:
-        raise handle_bad_response(response, endpoint)
+        raise handle_bad_response(response, endpoint)  # already returns json object
     else:
-        print(dump(response))
+        if json_output:
+            return dump(response)
+        else:
+            return response
 
 
 # --------------------------------------       iris get     -------------------------------------- #
 
 
 @auth
+@telemetry_decorator
+@json_output_decorator
 def get(
     object: str = "experiment",
     id: Optional[str] = None,
     query: Optional[str] = None,
-    headers: dict = {},
-    verbose=True,
+    headers: dict = None,
+    verbose: bool = True,
+    json_output: bool = False,
 ):
-    """Get objects from the titan API
+    """Get objects from the TitanML Store.
 
     Args:
         object (str, optional): The object to get. Defaults to "experiment".
         id (Optional[str], optional): The id of the object. Defaults to None.
-        query (Optional[str], optional): A JMESPath query to run against the returned json. Defaults to None, i.e. return everything.
+        query (Optional[str], optional): A JMESPath query to run against the returned json.
+                                         Defaults to None, i.e. return everything.
         headers (dict): Custom headers to send with the get request
+        verbose (bool): Whether to print the response
+        json_output (bool): Whether to return the response as a json object
+
     Returns:
         (str) A json response, formatted as: {"status": <http_response>, "response": <queried_json_response>}
     """
+    if headers is None:
+        headers = {}
+
     logger.debug(f"Getting from ... {conf_mgr.base}, auth from {conf_mgr.AUTH0_DOMAIN}")
     logger.debug(f"Applying custom headers {headers}")
-    endpoint = object + "/" + (str(id) if id is not None else "")
+    endpoint = str(object) + "/"
+    if id:
+        endpoint += id
     url = urljoin(conf_mgr.runner_url, endpoint)
     headers.update({"Authorization": f"Bearer {conf_mgr.access_token}"})
 
-    try:
-        response = requests.get(url=url, headers=headers)
-    except requests.exceptions.ConnectionError as e:
-        print(
-            json.dumps(
-                {
-                    "status": "failed",
-                    "message": f"Connection error: Error reaching {url}",
-                },
-                indent=4,
-            )
-        )
-        raise Exception("Connection error")
-    except requests.exceptions.MissingSchema as e:
-        print(
-            json.dumps(
-                {
-                    "status": "failed",
-                    "message": f"Scheme error: iris target specified improperly. base={conf_mgr.base}, runner_url: {conf_mgr.runner_url}, endpoint={endpoint} result={url} ",
-                },
-                indent=4,
-            )
-        )
-        raise Exception("Scheme error")
-    except Exception as e:
-        print(e)
-        raise e
+    response = requests.get(url=url, headers=headers)
 
     if not response.ok:
         raise handle_bad_response(response, url)
     else:
-        dumped_response = dump(response, query)
-        if verbose:
-            print(dumped_response)
-        return dumped_response
+        try:
+            dumped_response = dump(response, query)
+            return dumped_response
+        except json.JSONDecodeError:
+            print("JSON decoding error occurred.")
+            print(response)
+            return None
+
+
+# --------------------------------------     iris delete    -------------------------------------- #
+
+console = Console()
 
 
 @auth
+@telemetry_decorator
 def delete(
     object: str,
     id: Optional[str],
-    verbose=True,
+    verbose: bool = True,
+    json_output: bool = False,
 ):
-    """Get objects from the titan API
+    """Get objects from the TitanML Store.
 
     Args:
         object (str, optional): The object to get. Defaults to "experiment".
         id (str): The id of the object to delete
+        verbose (bool, optional): Whether to print the response. Defaults to True.
+        json_output (bool, optional): Whether to return the response as a json object. Defaults to False.
+
     Returns:
-        (str) A json response, formatted as: {"status": <http_response>, "response": <queried_json_response>}
+        (str) A json response, formatted as:
+        {"status": <http_response>, "response": <queried_json_response>}
     """
     logger.debug(f"Getting from ... {conf_mgr.base}, auth from {conf_mgr.AUTH0_DOMAIN}")
-    endpoint = object + "/" + (str(id) if id is not None else "")
+    endpoint = object + "/" + str(id) if id is not None else ""
     url = urljoin(conf_mgr.runner_url, endpoint)
     headers = {"Authorization": f"Bearer {conf_mgr.access_token}"}
 
     response = requests.delete(url=url, headers=headers)
     if not response.ok:
         raise handle_bad_response(response, endpoint)
     else:
         if response.status_code == 204:
-            return {"status": "success"}
-
-        dumped_response = dump(response)
-        if verbose:
-            print(dumped_response)
-        return dumped_response
+            if json_output:
+                result = json.dumps({"status": "success"}, indent=4)
+                print(result)
+            else:
+                table = Table(show_header=True, header_style="bold magenta")
+                table.add_column("Status", style="dim", width=12)
+                table.add_row("success")
+                console.print(table)
+        return None
 
 
 # --------------------------------------     iris download  -------------------------------------- #
 
 
 @auth
-def download(experiment_cmd: str):
-    """Downloading the models to local machine
+@telemetry_decorator
+def download(experiment_cmd: str, json_output: bool = False):
+    """Downloading the models to local machine.
 
     Args:
         experiment_cmd (str): pulling command string. it should be formatted as <experiment_id>:<job_tag>
+        json_output (bool, optional): Whether to return the response as a json object. Defaults to False.
 
     Raises:
         InvalidCommandError: Invalid command error
         BadRequestError: Bad request error
         ArtefactNotFoundError: Artefact not found error
 
     Returns:
         model_name: name of the model
         task_name: name of the task
         baseline_model_name: name of the baseline model
         baseline: whether the model is baseline or not
     """
-
     # create a model_storage folder if it doesn't exist
     Path("model_storage").mkdir(parents=True, exist_ok=True)
 
     # parse the command string
-    args = experiment_cmd.split(":")
-    if len(args) != 2:
+    experiment_id_name, _, job_tag = experiment_cmd.rpartition(":")
+
+    # check if the job tag is valid
+    if job_tag not in {"baseline", "fp16", "XS", "S", "M"}:
+        raise InvalidCommandError
+
+    experiment_id, _, experiment_name = experiment_id_name.partition("-")
+
+    # check if the experiment id is valid
+    if experiment_id == "":
         raise InvalidCommandError
-    experiment_id = args[0]
-    job_tag = args[1]
+
+    # check if the experiment name is valid
+    if experiment_name == "" and not json_output:
+        print(f"Downloading model_id {experiment_id} with job tag {job_tag} ...")
+    elif not json_output:
+        print(f"Downloading model {experiment_name} with job tag {job_tag} ...")
 
     # get the experiment info
     endpoint = "experiment"
     url = urljoin(conf_mgr.runner_url, f"{endpoint}/{experiment_id}")
     headers = {"Authorization": f"Bearer {conf_mgr.access_token}"}
 
     response = requests.get(url=url, headers=headers)
     response_json = response.json()
 
     # check if the request is successful
     if response_json["status"] != "success":
         raise BadRequestError
 
     jobs_list = response_json["experiment"]["jobs"]
+    tasks_list = jobs_list[0]["tasks"]
 
     model_uuid = None
     baseline = False
     download_url, model_name, task_name, baseline_model_name = None, None, None, None
     # loop through the jobs list and find the job with the same tag
-    for i in range(len(jobs_list)):
-        if job_tag == jobs_list[i]["name"].split("_")[-1]:
-            model_uuid = jobs_list[i]["out_art_id"]
-            model_name = jobs_list[i]["name"]
-            task_name = jobs_list[i]["flags"]["task"]
-            baseline_model_name = jobs_list[i]["flags"]["model.teacher"]
-
-            if baseline_model_name == "null":
-                baseline_model_name = jobs_list[i]["flags"]["model.student"]
-                baseline = True
+    for i in range(len(tasks_list)):
+        if job_tag == tasks_list[i]["name"].split("_")[-1]:
+            model_uuid = tasks_list[i]["out_art_id"]
+            model_name = tasks_list[i]["name"]
+            task_name = tasks_list[i]["flags"]["task"]
+
+            results = tasks_list[i]["results"]
+            status = tasks_list[i]["status"]
+
+            # check if the job is still running
+            if results is None and status == "active":
+                raise JobStillRunningError
+
+            # check if the baseline model is available
+            # if baseline_model_name == "null":
+            #     baseline_model_name = jobs_list[i]["flags"]["model.student"]
+            #     baseline = True
 
+            # check if text fields is valid in sequence classification task
             if task_name == "sequence_classification":
-                text_fields = ast.literal_eval(
-                    jobs_list[i]["flags"]["data.text_fields"]
-                )  # convert string to list
+                text_fields = ast.literal_eval(tasks_list[i]["flags"]["data.text_fields"])  # convert string to list
                 if len(text_fields) == 1:
                     task_name = "sequence_classification"
                 elif len(text_fields) == 2:
                     task_name = "pair_classification"
                 else:
                     raise ValueError("Invalid number of text fields")
 
+            # check if dataset name is valid in glue task
             if task_name == "glue":
-                dataset_name = jobs_list[i]["flags"][
-                    "data.dataset_config_name"
-                ]  # convert string to list
+                dataset_name = tasks_list[i]["flags"]["data.dataset_config_name"]  # convert string to list
                 if dataset_name in {"sst2", "cola"}:
                     task_name = "sequence_classification"  # cola and sst2 only has one sentence as input
                 else:
                     task_name = "pair_classification"
 
+            # check if artifact is available
             if model_uuid is None:
                 raise ArtefactNotFoundError
             url = urljoin(
                 conf_mgr.runner_url,
                 f"artefact/link/{model_uuid}/download?refresh=true",
             )
+            # get the download url
             response = requests.get(url=url, headers=headers)
             response_json = response.json()
             download_url = response_json["link"]["link"]
             break
 
     # download the model
     if download_url is not None:
-        download_model(download_url, model_name)
-    print(f"\nModel {model_name} downloaded successfully")
+        download_model(download_url, model_name, json_output=json_output)
+    if json_output:
+        print(json.dumps(response_json, indent=4))
+    else:
+        print(f"\nModel {model_name} downloaded successfully")
     return model_name, task_name, baseline_model_name, baseline
 
 
 # --------------------------------------      iris pull     -------------------------------------- #
 
 
 @auth
-def pull(experiment_cmd: str):
-    """download the model and pull the hephaestus image from the server
+@telemetry_decorator
+def pull(experiment_cmd: str, json_output: bool = False):
+    """Download the model and pull the hephaestus image from the server.
 
     Args:
         experiment_cmd (str): pulling command string. it should be formatted as <experiment_id>:<job_tag>
+        json_output (bool, optional): Whether to return the response as a json object. Defaults to False.
 
     """
-
     # parse the command string
     args = experiment_cmd.split(":")
     if len(args) != 2:
         raise InvalidCommandError
-    experiment_id = args[0]
-    job_tag = args[1]
+    experiment_id: str = args[0].lower()
+    job_tag: str = args[1]
 
     # download the model
     logger.info("***Executing pull command***")
-    model_name, task_name, baseline_model_name, baseline = download.__wrapped__(
-        experiment_cmd
+    model_name, task_name, baseline_model_name, baseline = download(
+        experiment_cmd, json_output=json_output
     )  # this is a hack to get the function to work without the auth decorator
 
     # pull the image
     logger.info("Pulling image from the server")
     pull_image(
         model_folder_path=f"model_storage/{model_name}/models",
         container_name=f"iris-triton-{experiment_id}",
         job_tag=job_tag,
         task_name=task_name,
         baseline_model_name=baseline_model_name,
         baseline=baseline,
+        json_output=json_output,
     )
     logger.info("All done!")
+    if json_output:
+        result = {"status": "success"}
+        return json.dumps(result, indent=4)
 
 
 # --------------------------------------    iris upload     -------------------------------------- #
 
 
 @auth
+@telemetry_decorator
 def upload(
     name: str,
     src: Union[str, Path],
     description: str,
     internal_artefact_type: Optional[str] = None,
+    json_output: bool = False,
 ):
-    """Upload an artefact to the titan hub
+    """Upload an artefact to the TitanML Store.
 
     Args:
         internal_artefact_type (Union[str, None]): One of ['model','dataset'] - the type of artefact purpotedly being
         uploaded when calling from iris post.
         name (str): The name of the artefact
         src (Union[str, Path]): The source of the artefact on disk
         description (str): A short description of the artefact.
+        json_output (bool, optional): Whether to return the response as a json object. Defaults to False.
 
     Raises:
         ArtefactNotFoundError: If the path to the artefact doesn't exist.
         UnsafeTensorsError: If the artefact is a model, and the model has not been saved in safetensors format.
     """
     # cast from path to str.
     src = str(src)
 
     metadata = {}
 
+    # cast object from path to str within the metadata dictionary
+    metadata["src"] = str(Path(src))
+
     endpoint = "artefact"
     url = urljoin(conf_mgr.runner_url, f"{endpoint}/")
     headers = {"Authorization": f"Bearer {conf_mgr.access_token}"}
 
     # Catches if you accidentally put a tilde in quotes:
     if src[0] == "~":
         src = os.path.expanduser(src)
@@ -418,17 +498,15 @@
             raise MissingTokenizerError()
 
         # Family examples: DebertaV2, Albert, DistilBert, Roberta, Electra, Bert
         # Detect model family
         with open(os.path.join(src, "tokenizer_config.json"), "r") as f:
             tokenizer_class = json.load(f).get("tokenizer_class", None)
         if tokenizer_class:
-            metadata["local_model_family"] = tokenizer_class.replace(
-                "Tokenizer", ""
-            ).lower()
+            metadata["local_model_family"] = tokenizer_class.replace("Tokenizer", "").lower()
         else:
             raise UnknownFamilyError()
 
     elif internal_artefact_type == "dataset" or val_file_check or train_file_check:
         art_type = "dataset"
         if not val_file_check and train_file_check:
             raise InvalidDatasetFormatError()
@@ -447,15 +525,15 @@
 
     post_req_data = {
         "name": name,
         "artefact_type": art_type,
         "description": description,
         "ext": ext,
         "src": src,
-        "metadata": json.dumps(metadata),
+        "metadata": json.dumps({k: str(v) for k, v in metadata.items()}),
         "hash": hashval,
     }
 
     logger.debug(f"posting {post_req_data} to {url}")
     post_req_response = requests.post(url=url, headers=headers, data=post_req_data)
     if not post_req_response.ok:
         logger.debug("post unsuccessful")
@@ -464,171 +542,183 @@
         # On succesful response receipt:
         logger.debug("post successful")
 
         # Check if artefact-already-exists response has been received.
         if post_req_response.status_code == 202:
             existing_artefact = post_req_response.json()["artefact"]
             created_time = str(
-                datetime.strptime(
-                    existing_artefact["time_created"], "%Y-%m-%dT%H:%M:%S.%fZ"
-                ).strftime("%d-%m-%Y %H:%M:%S")
+                datetime.strptime(existing_artefact["time_created"], "%Y-%m-%dT%H:%M:%S.%fZ").strftime(
+                    "%d-%m-%Y %H:%M:%S"
+                )
             )
             # Return artefact data for found/existing artefact.
             if not internal_artefact_type:
-                print(
-                    f"Artefact was already uploaded at {created_time} with ID: {existing_artefact['uuid']}"
-                )
+                print(f"Artefact was already uploaded at {created_time} with ID: {existing_artefact['uuid']}")
             return existing_artefact["uuid"]
 
     data = post_req_response.json()["artefact"]
     art_uuid = data["uuid"]
     endpoint = "artefact/link/" + art_uuid + "/upload"
     url = urljoin(conf_mgr.runner_url, f"{endpoint}")
     logger.debug(f"Getting link from {url}")
     get_link_resp = requests.get(url=url, headers=headers)
     upl_link = get_link_resp.json()["link"]["link"]
     logger.debug(f"got link {upl_link}")
 
-    print("Beginning upload...")
+    if not json_output:
+        print("Beginning upload...")
 
     # Upload file
-    upload_response = upload_from_file(tarred, upl_link)
+    upload_response = upload_from_file(tarred, upl_link, json_output=json_output)
 
     # If Upload completes succesfully, send the hash to seshat in a patch request. Patch req confirms matching hash,
     # then returns the artefact ID for further use by user.
     if upload_response is not None and upload_response.status_code == 200:
         endpoint = "artefact"
-        print(f"Upload Complete -  Validating {art_type} server-side")
+        if not json_output:
+            print(f"Upload Complete -  Validating {art_type} server-side")
         url = urljoin(conf_mgr.runner_url, f"{endpoint}/{art_uuid}")
-        patch_req_response = requests.patch(
-            url=url, headers=headers, data={"hashval": hashval}
-        )
+        patch_req_response = requests.patch(url=url, headers=headers, data={"hashval": hashval})
         if not patch_req_response.ok:
             raise handle_bad_response(patch_req_response, endpoint)
         else:
-            print(
-                f"Upload validated. This {art_type} can now be used in experiments by referring to it by UUID: {art_uuid}"
-            )
-            print(f"Alternatively, you can continue to use the {art_type}'s filepath.")
+            if json_output:
+                result = {"status": "success", "artefact id": str(art_uuid)}
+                print(json.dumps(result, indent=4))
+            else:
+                print(
+                    f"Upload validated. This {art_type} can now be used in experiments \
+                    by referring to it by UUID: {art_uuid}"
+                )
+                print(f"Alternatively, you can continue to use the {art_type}'s filepath.")
             return art_uuid
     else:
         print("Upload failed")
-        print(dump(upload_response))
+        for key, value in upload_response.items():
+            if isinstance(value, Path):
+                upload_response[key] = str(value)
+        return dump(upload_response)
 
 
 # --------------------------------------      iris infer    -------------------------------------- #
 
 
+@telemetry_decorator
 def infer(
     url: str,
     task_name: str,
-    use_cpu: bool,
     text: List[str],
     context: Optional[str] = None,
+    runtime: str = "trt",
 ):
-    """infer the hosted tytn model using triton client
+    """Infer the hosted tytn model using triton client.
 
     Args:
         port (int): port number of the triton server
         task_name (str): task name of the model (sequence_classification, question_answering)
-        use_cpu (bool): whether to use cpu or not
+        runtime (str): choose the runtime for inference (trt, onnx)
         text (str): input text field used for inference
-        context (Optional[str]): input context field used for inference. Only used in question_answering task. Defaults to None.
+        context (Optional[str]): input context field used for inference. Only used in question_answering task.
+                                    Defaults to None.
+        url (str): The url of the triton server
+
+
     Returns:
         infer_res(dict): dictionary of the inference result
     """
+    # check if the runtime is valid
+    print("runtime is ", runtime)
+    if runtime not in ["trt", "onnx"]:
+        raise ValueError("runtime must be either trt or onnx")
 
-    model_name = (
-        "transformer_onnx_inference" if use_cpu else "transformer_tensorrt_inference"
-    )
+    model_name = "transformer_onnx_inference" if runtime == "onnx" else "transformer_tensorrt_inference"
     model_version = "1"
     batch_size = 1
 
     triton_client = tritonclient.http.InferenceServerClient(url=url, verbose=False)
 
-    model_metadata = triton_client.get_model_metadata(
-        model_name=model_name, model_version=model_version
-    )
-    model_config = triton_client.get_model_config(
-        model_name=model_name, model_version=model_version
-    )
+    triton_client.get_model_metadata(model_name=model_name, model_version=model_version)
+    triton_client.get_model_config(model_name=model_name, model_version=model_version)
     text_1, text_2 = None, None
     if task_name == "sequence_classification":
         if len(text) == 1:
             # if only one text is provided, this is a single sentence classification task inference
-            text_1 = tritonclient.http.InferInput(
-                name="TEXT", shape=(batch_size,), datatype="BYTES"
-            )
+            text_1 = tritonclient.http.InferInput(name="TEXT", shape=(batch_size,), datatype="BYTES")
             text_1.set_data_from_numpy(np.asarray([text[0]] * batch_size, dtype=object))
         elif len(text) == 2:
             # if two texts are provided, this is a pair sentence classification task inference
-            text_1 = tritonclient.http.InferInput(
-                name="TEXT_1", shape=(batch_size,), datatype="BYTES"
-            )
-            text_2 = tritonclient.http.InferInput(
-                name="TEXT_2", shape=(batch_size,), datatype="BYTES"
-            )
+            text_1 = tritonclient.http.InferInput(name="TEXT_1", shape=(batch_size,), datatype="BYTES")
+            text_2 = tritonclient.http.InferInput(name="TEXT_2", shape=(batch_size,), datatype="BYTES")
             text_1.set_data_from_numpy(np.asarray([text[0]] * batch_size, dtype=object))
             text_2.set_data_from_numpy(np.asarray([text[1]] * batch_size, dtype=object))
         else:
-            raise ValueError(
-                "Invalid number of texts provided for sequence classification task"
-            )
+            raise ValueError("Invalid number of texts provided for sequence classification task")
     elif task_name == "question_answering":
         if context is None:
             raise ValueError("Context must be provided for question answering task")
-        text_1 = tritonclient.http.InferInput(
-            name="QUESTION", shape=(batch_size,), datatype="BYTES"
-        )
-        text_2 = tritonclient.http.InferInput(
-            name="CONTEXT", shape=(batch_size,), datatype="BYTES"
-        )
+        text_1 = tritonclient.http.InferInput(name="QUESTION", shape=(batch_size,), datatype="BYTES")
+        text_2 = tritonclient.http.InferInput(name="CONTEXT", shape=(batch_size,), datatype="BYTES")
         text_1.set_data_from_numpy(np.asarray([text[0]] * batch_size, dtype=object))
         text_2.set_data_from_numpy(np.asarray([context] * batch_size, dtype=object))
     else:
         raise ValueError("Invalid task name provided")
 
     # bind outputs to the server
-    outputs = tritonclient.http.InferRequestedOutput(name="outputs", binary_data=False)
+    outputs = tritonclient.http.InferRequestedOutput(name="logits", binary_data=False)
 
     infer_res = triton_client.infer(
         model_name=model_name,
         model_version=model_version,
         inputs=[text_1, text_2] if text_2 is not None else [text_1],
         outputs=[outputs],
     )
-    return json.loads(infer_res.as_numpy("outputs").item())
+    return json.loads(infer_res.as_numpy("logits").item())
 
 
 # --------------------------------------     iris makesafe    -------------------------------------- #
 
 
 def makesafe(
     model: str,
 ):
-    """Convert a model's weights to the safetensors format
+    """Convert a model's weights to the safetensors format.
 
     Args:
         model (str): The path of the local model to be converted.
     """
-
     if not os.path.exists(model):
-        print("Model not found at given location")
-        return
+        raise FileNotFoundError
     # else
     print("Checking for requirements...")
-    failed_packages = list(
-        filter(
-            lambda x: not util.find_spec(x), ["torch", "safetensors", "transformers"]
-        )
-    )
+    failed_packages = list(filter(lambda x: not util.find_spec(x), ["torch", "safetensors", "transformers"]))
     if failed_packages:
         print(
             "To use the safetensors convert, you must have the following packages installed: ",
             failed_packages,
         )
         print("NB: These packages do not need to be installed with gpu support.")
         return
+    if metadata.version("transformers") < "4.27.0":
+        print(
+            "To use makesafe you must have transformers >= 4.27.0. You currently have "
+            + metadata.version("transformers")
+        )
+        return
     # else
     from .safe_convert import do_convert
 
     do_convert(model)
+
+
+# --------------------------------------     iris test    -------------------------------------- #
+
+
+@auth
+@telemetry_decorator
+def query(artefact: str, data: dict):
+    """Simple inference test."""
+    endpoint = "inference-session"
+    url = urljoin(conf_mgr.runner_url, f"{endpoint}/{artefact}")
+    headers = {"Authorization": f"Bearer {conf_mgr.access_token}"}
+
+    response = requests.post(url=url, headers=headers, json=data)
+    return response.json()
```

### Comparing `titan-iris-0.3.9a2/src/iris/sdk/safe_convert.py` & `titan-iris-0.4.0a0/src/iris/sdk/safe_convert.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+"""Safetensors conversion script."""
 import os
 from collections import defaultdict
+from pathlib import Path
+from typing import Sequence, Union
+
 import torch
 from safetensors.torch import load_file, save_file
 from transformers import AutoModel
 
 
-def shared_pointers(tensors):
-    """
-    Finds all pointers who share a matrix value.
+def shared_pointers(tensors: Sequence[torch.Tensor]):
+    """Finds all pointers who share a matrix value.
 
     Args:
         tensors: The tensors stored in a model's state_dict
 
     Returns:
         object: A list of lists of pointers which point to a given tensor, where this is more than 1.
     """
@@ -21,23 +24,27 @@
     failing = []
     for ptr, names in ptrs.items():
         if len(names) > 1:
             failing.append(names)
     return failing
 
 
-def check_file_size(sf_filename: str, pt_filename: str):
-    """
+def check_file_size(sf_filename: str, pt_filename: str) -> None:
+    """Check file sizes.
+
     Checks that only shared tensors have been replaced by asserting that the input and output
     weights files are the same size.
 
     Args:
         sf_filename: Filename of the converted safetensor file.
         pt_filename: Filename of the input model file.
 
+    Raises:
+        RuntimeError: If the file sizes are different by more than 1%.
+
     """
     sf_size = os.stat(sf_filename).st_size
     pt_size = os.stat(pt_filename).st_size
 
     if (sf_size - pt_size) / pt_size > 0.01:
         raise RuntimeError(
             f"""The file size different is more than 1%:
@@ -47,16 +54,15 @@
         )
 
 
 def convert_file(
     pt_filename: str,
     sf_filename: str,
 ):
-    """
-    Converts a standard pytorch model into a safetensors-saved one.
+    """Converts a standard pytorch model into a safetensors-saved one.
 
     Args:
         pt_filename: Filename of input pytorch model.
         sf_filename: Filename to which output safetensors file is to be saved.
     """
     loaded = torch.load(pt_filename, map_location="cpu")
     if "state_dict" in loaded:
@@ -81,24 +87,27 @@
     for k in loaded:
         pt_tensor = loaded[k]
         sf_tensor = reloaded[k]
         if not torch.equal(pt_tensor, sf_tensor):
             raise RuntimeError(f"The output tensors do not match for key {k}")
 
 
-def do_convert(model_path):
-    """
-    Takes an input model, checks if it is already in safetenors format, else attempts to convert it by two methods.
+def do_convert(model_path: Union[Path, str]) -> None:
+    """Takes an input model, and tries to convert it to safetensors.
+
+    Checks if it is already in safetenors format, else attempts to convert it by two methods.
     Method 1: The safetensors/transformers safe_serialization=True method (quicker, works for non-shared-weight models).
     Method 2: Adaptation of weight-sharing-compatible conversion in convert_file.
     Method 2 is adapted from https://github.com/huggingface/safetensors/issues/98
+
     Args:
-        model_path (str): an input pytorch model path (pointing to a folder which contains pytorch_model.bin)
+        model_path (str): an input pytorch model path (pointing to a folder which contains pytorch_model.bin).
 
-    Returns None.
+    Returns:
+        None.
 
     """
     sf_filename = os.path.join(model_path, "model.safetensors")
     if os.path.exists(sf_filename):
         print("Model is already in safetensors format")
         return
 
@@ -106,11 +115,12 @@
 
     try:
         model = AutoModel.from_pretrained(model_path)
         model.save_pretrained(model_path, safe_serialization=True)
         print("Conversion completed.")
     except RuntimeError:
         print(
-            "Basic conversion method failed (likely due to the selected model using shared weights), attempting secondary method..."
+            "Basic conversion method failed (likely due to the selected model using shared weights), \
+                attempting secondary method..."
         )
         convert_file(model_path + "/pytorch_model.bin", sf_filename)
         print("Conversion completed.")
```

### Comparing `titan-iris-0.3.9a2/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.4.0a0/src/titan_iris.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 requirements.txt
 requirements_dev.txt
 setup.cfg
 setup.py
 src/iris/__init__.py
 src/iris/config.yaml
 src/iris/main.py
+src/iris/gradio/__init__.py
+src/iris/gradio/run.py
 src/iris/sdk/__init__.py
 src/iris/sdk/auth_utils.py
 src/iris/sdk/conf_manager.py
 src/iris/sdk/exception.py
 src/iris/sdk/iris_sdk.py
 src/iris/sdk/safe_convert.py
 src/iris/sdk/utils.py
 src/titan_iris.egg-info/PKG-INFO
 src/titan_iris.egg-info/SOURCES.txt
 src/titan_iris.egg-info/dependency_links.txt
 src/titan_iris.egg-info/entry_points.txt
 src/titan_iris.egg-info/requires.txt
 src/titan_iris.egg-info/top_level.txt
-tests/test_cli.py
+tests/test_cli.py
+tests/test_sdk.py
```

