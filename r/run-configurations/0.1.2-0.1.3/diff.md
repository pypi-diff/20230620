# Comparing `tmp/run_configurations-0.1.2.tar.gz` & `tmp/run_configurations-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_configurations-0.1.2.tar", last modified: Thu Apr  6 11:13:09 2023, max compression
+gzip compressed data, was "run_configurations-0.1.3.tar", last modified: Tue Jun 20 10:43:55 2023, max compression
```

## Comparing `run_configurations-0.1.2.tar` & `run_configurations-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bvolkmer  (1000) bvolkmer  (1000)        0 2023-04-06 11:13:09.119139 run_configurations-0.1.2/
--rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)     1059 2023-03-30 17:50:05.000000 run_configurations-0.1.2/LICENCE
--rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)     1837 2023-04-06 11:13:09.119139 run_configurations-0.1.2/PKG-INFO
--rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)     1514 2023-04-06 10:57:59.000000 run_configurations-0.1.2/README.md
-drwxrwxr-x   0 bvolkmer  (1000) bvolkmer  (1000)        0 2023-04-06 11:13:09.115139 run_configurations-0.1.2/run_configurations.egg-info/
--rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)     1837 2023-04-06 11:13:09.000000 run_configurations-0.1.2/run_configurations.egg-info/PKG-INFO
--rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)      302 2023-04-06 11:13:09.000000 run_configurations-0.1.2/run_configurations.egg-info/SOURCES.txt
--rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)        1 2023-04-06 11:13:09.000000 run_configurations-0.1.2/run_configurations.egg-info/dependency_links.txt
--rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)       46 2023-04-06 11:13:09.000000 run_configurations-0.1.2/run_configurations.egg-info/entry_points.txt
--rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)        6 2023-04-06 11:13:09.000000 run_configurations-0.1.2/run_configurations.egg-info/requires.txt
--rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)       19 2023-04-06 11:13:09.000000 run_configurations-0.1.2/run_configurations.egg-info/top_level.txt
--rwxrwxr-x   0 bvolkmer  (1000) bvolkmer  (1000)     8126 2023-04-06 10:54:57.000000 run_configurations-0.1.2/run_configurations.py
--rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)       38 2023-04-06 11:13:09.119139 run_configurations-0.1.2/setup.cfg
--rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)      752 2023-04-06 11:11:11.000000 run_configurations-0.1.2/setup.py
+drwxrwxr-x   0 bvolkmer  (1000) bvolkmer  (1000)        0 2023-06-20 10:43:55.201639 run_configurations-0.1.3/
+-rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)     1059 2023-03-30 17:50:05.000000 run_configurations-0.1.3/LICENCE
+-rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)     2252 2023-06-20 10:43:55.201639 run_configurations-0.1.3/PKG-INFO
+-rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)     1906 2023-06-20 10:21:48.000000 run_configurations-0.1.3/README.md
+drwxrwxr-x   0 bvolkmer  (1000) bvolkmer  (1000)        0 2023-06-20 10:43:55.201639 run_configurations-0.1.3/run_configurations.egg-info/
+-rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)     2252 2023-06-20 10:43:55.000000 run_configurations-0.1.3/run_configurations.egg-info/PKG-INFO
+-rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)      302 2023-06-20 10:43:55.000000 run_configurations-0.1.3/run_configurations.egg-info/SOURCES.txt
+-rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)        1 2023-06-20 10:43:55.000000 run_configurations-0.1.3/run_configurations.egg-info/dependency_links.txt
+-rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)       46 2023-06-20 10:43:55.000000 run_configurations-0.1.3/run_configurations.egg-info/entry_points.txt
+-rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)        6 2023-06-20 10:43:55.000000 run_configurations-0.1.3/run_configurations.egg-info/requires.txt
+-rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)       19 2023-06-20 10:43:55.000000 run_configurations-0.1.3/run_configurations.egg-info/top_level.txt
+-rwxrwxr-x   0 bvolkmer  (1000) bvolkmer  (1000)     9481 2023-06-20 10:29:09.000000 run_configurations-0.1.3/run_configurations.py
+-rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)       38 2023-06-20 10:43:55.201639 run_configurations-0.1.3/setup.cfg
+-rw-rw-r--   0 bvolkmer  (1000) bvolkmer  (1000)      781 2023-06-20 10:33:34.000000 run_configurations-0.1.3/setup.py
```

### Comparing `run_configurations-0.1.2/LICENCE` & `run_configurations-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `run_configurations-0.1.2/PKG-INFO` & `run_configurations-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: run_configurations
-Version: 0.1.2
-Summary: A small script that allows quickly executing run configurations from the command line including shell completions 
-Home-page: https://github.com/bvolkmer/run_configurations
-Author: Benedikt Volkmer
-License: MIT
-Description-Content-Type: text/markdown
-
 A small script that allows quickly executing run configurations from the command
 line including shell completions.
 
 A run configurations can be any executable placed in a `.run_configs` directory
 in any parent of the current working directory. Configurations are always
 executed in the directory containing the `.run_configs` folder to get the same
 behavior independent of the current working directory.
@@ -19,14 +10,20 @@
 Usage: rc [OPTIONS] RUN_CONFIG [ARGS]...
 
   Run a run config
 
   A run config can be any executable file in the .run_configs directory.
 
 Options:
+  -f, --fork                      Fork process and return immediately. If -s
+                                  is also supplied the screen session will
+                                  start detached.
+  -n, --null-pipe                 Use a null pipe instead of a PTY. Is ignored
+                                  if -s is supplied
+  -s, --screen                    Run in a screen session.
   -e, --edit                      Edit run config instead of running.
   -l, --list                      List available run configs.
   -x, --make-executable           Make run config executable if it isn't
                                   already.
   --base-dir DIRECTORY            Base directory to run from. Defaults to the
                                   first directory containing a .run_configs
                                   directory. Should contain a .run_configs
```

### Comparing `run_configurations-0.1.2/run_configurations.py` & `run_configurations-0.1.3/run_configurations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 #!/usr/bin/env python3
 
 import logging
 import os
+import subprocess
 import stat
 import sys
 from pathlib import Path
+from typing import Any
+from shutil import which
+from typing import List, Tuple
 
 import click
 
 RUN_CONFIGS_DIR: str = ".run_configs"
 
 
 PathNotFoundError = Exception
@@ -39,15 +43,15 @@
     )
 
 
 def get_rc_dir(base_dir: Path) -> Path:
     return base_dir / RUN_CONFIGS_DIR
 
 
-def get_run_configs(base_dir: Path, incomplete: str = "") -> list[Path]:
+def get_run_configs(base_dir: Path, incomplete: str = "") -> List[Path]:
     return [
         rc
         for rc in filter(
             lambda p: p.name.startswith(incomplete), get_rc_dir(base_dir).glob("**/*")
         )
         if rc.is_file() and os.access(str(rc.absolute()), os.X_OK)
     ]
@@ -142,14 +146,32 @@
     return
 
 
 @click.command()
 @click.argument("run_config", type=RunConfigType())
 @click.argument("args", nargs=-1)
 @click.option(
+    "--fork",
+    "-f",
+    is_flag=True,
+    help="Fork process and return immediately. If -s is also supplied the screen session will start detached.",
+)
+@click.option(
+    "--null-pipe",
+    "-n",
+    is_flag=True,
+    help="Use a null pipe instead of a PTY. Is ignored if -s is supplied",
+)
+@click.option(
+    "--screen",
+    "-s",
+    is_flag=True,
+    help="Run in a screen session.",
+)
+@click.option(
     "--edit",
     "-e",
     is_flag=True,
     help="Edit run config instead of running.",
 )
 @click.option(
     "--list",
@@ -211,23 +233,31 @@
     callback=set_log_level,
 )
 @click.version_option()
 @click.pass_context
 def cli(
     ctx: click.Context,
     run_config: str,
-    args: tuple[str],
+    args: Tuple[str],
     base_dir: Path,
     make_executable: bool = False,
     edit: bool = False,
+    fork: bool = False,
+    null_pipe: bool = False,
+    screen: bool = False,
 ) -> None:
     """Run a run config
 
     A run config can be any executable file in the .run_configs directory.
     """
+    if null_pipe and screen:
+        logging.warning("Ignoring null pipe because screen is enabled.")
+    if screen and which("screen") is None:
+        logging.error("screen not found. Please install screen.")
+        ctx.exit(1)
     logging.debug(f"Parameter: {ctx.params}")
     rc_dir = get_rc_dir(base_dir)
     logging.debug(f"Base dir: {base_dir}")
     rc = rc_dir / run_config
     logging.debug(f"Run config: {rc}")
     if edit:
         editor = os.getenv("EDITOR", "vim")
@@ -259,19 +289,35 @@
             "Run config not executable. Change permissions?", abort=True
         ):
             logging.debug(f"Making {rc} executable")
             os.chmod(
                 str(rc.absolute()), os.stat(str(rc.absolute())).st_mode | stat.S_IEXEC
             )
     logging.debug(f"Changing directory to {base_dir}")
-    os.chdir(base_dir)
-    args_list = list(args) if len(args) > 0 else []
-    logging.debug(f"Executing {rc} with args {args_list}")
+    prog_args = list(args) if len(args) > 0 else []
+    logging.debug(f"Executing {rc} with args {prog_args}")
+    prog = str(rc.absolute())
+    prog_args.insert(0, prog)
+    if screen:
+        prog_args.insert(0, "screen")
+        if fork:
+            prog_args.insert(1, "-d")
+            prog_args.insert(2, "-m")
+    logging.debug(f"Executing {prog_args}")
+
+    process_args: dict[str, Any] = dict(cwd=base_dir, env=os.environ)
+    if null_pipe and not screen:
+        process_args["stdout"] = subprocess.DEVNULL
+        process_args["stderr"] = subprocess.DEVNULL
     try:
-        os.execv(str(rc.absolute()), [str(rc)] + args_list)
+        proc = subprocess.Popen(
+            prog_args, start_new_session=fork and not screen, **process_args
+        )
+        if not fork:
+            proc.wait()
     except OSError as e:
         logging.error(f"Error executing {rc}: {e}")
         raise click.FileError(rc, f"{e}")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `run_configurations-0.1.2/setup.py` & `run_configurations-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from pathlib import Path
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 
 setup(
     name="run_configurations",
     version=VERSION,
     author="Benedikt Volkmer",
     description=(
         "A small script that allows quickly executing run configurations from "
@@ -13,14 +13,15 @@
     ),
     license="MIT",
     license_files=["LICENSE"],
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/bvolkmer/run_configurations",
     py_modules=["run_configurations"],
+    python_requires=">=3.8",
     install_requires=[
         "click",
     ],
     entry_points={
         "console_scripts": [
             "rc = run_configurations:cli",
         ]
```

