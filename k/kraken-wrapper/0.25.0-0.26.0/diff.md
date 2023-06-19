# Comparing `tmp/kraken_wrapper-0.25.0.tar.gz` & `tmp/kraken_wrapper-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_wrapper-0.25.0.tar", max compression
+gzip compressed data, was "kraken_wrapper-0.26.0.tar", max compression
```

## Comparing `kraken_wrapper-0.25.0.tar` & `kraken_wrapper-0.26.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      988 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/LICENSE
--rw-r--r--   0        0        0      433 2023-06-19 14:25:27.366905 kraken_wrapper-0.25.0/README.md
--rw-r--r--   0        0        0     2174 2023-06-19 15:38:30.030178 kraken_wrapper-0.25.0/pyproject.toml
--rw-r--r--   0        0        0      134 2023-06-19 15:38:30.030178 kraken_wrapper-0.25.0/src/kraken/wrapper/__init__.py
--rw-r--r--   0        0        0     6258 2023-06-19 15:38:25.250142 kraken_wrapper-0.25.0/src/kraken/wrapper/_buildend_venv.py
--rw-r--r--   0        0        0     3374 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/_buildenv.py
--rw-r--r--   0        0        0     5311 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/_buildenv_manager.py
--rw-r--r--   0        0        0     3674 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/_buildenv_pex.py
--rw-r--r--   0        0        0     3250 2023-06-19 15:38:25.250142 kraken_wrapper-0.25.0/src/kraken/wrapper/_config.py
--rw-r--r--   0        0        0     4605 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/_lockfile.py
--rw-r--r--   0        0        0     3564 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/_option_sets.py
--rw-r--r--   0        0        0     4222 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/_pex.py
--rw-r--r--   0        0        0    16230 2023-06-19 15:38:25.250142 kraken_wrapper-0.25.0/src/kraken/wrapper/main.py
--rw-r--r--   0        0        0        0 2023-05-15 12:38:11.992918 kraken_wrapper-0.25.0/src/kraken/wrapper/py.typed
--rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 kraken_wrapper-0.25.0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.0/LICENSE
+-rw-r--r--   0        0        0      378 2023-06-19 22:14:09.973885 kraken_wrapper-0.26.0/README.md
+-rw-r--r--   0        0        0     2174 2023-06-19 22:48:11.871966 kraken_wrapper-0.26.0/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-06-19 22:48:11.871966 kraken_wrapper-0.26.0/src/kraken/wrapper/__init__.py
+-rw-r--r--   0        0        0     7660 2023-06-19 22:14:09.973885 kraken_wrapper-0.26.0/src/kraken/wrapper/_buildend_venv.py
+-rw-r--r--   0        0        0     3478 2023-06-19 22:14:09.973885 kraken_wrapper-0.26.0/src/kraken/wrapper/_buildenv.py
+-rw-r--r--   0        0        0     5311 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.0/src/kraken/wrapper/_buildenv_manager.py
+-rw-r--r--   0        0        0     3674 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.0/src/kraken/wrapper/_buildenv_pex.py
+-rw-r--r--   0        0        0     3250 2023-06-19 15:38:25.250142 kraken_wrapper-0.26.0/src/kraken/wrapper/_config.py
+-rw-r--r--   0        0        0     4605 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.0/src/kraken/wrapper/_lockfile.py
+-rw-r--r--   0        0        0     3564 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.0/src/kraken/wrapper/_option_sets.py
+-rw-r--r--   0        0        0     4222 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.0/src/kraken/wrapper/_pex.py
+-rw-r--r--   0        0        0    15814 2023-06-19 22:14:09.973885 kraken_wrapper-0.26.0/src/kraken/wrapper/main.py
+-rw-r--r--   0        0        0        0 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.0/src/kraken/wrapper/py.typed
+-rw-r--r--   0        0        0     1451 1970-01-01 00:00:00.000000 kraken_wrapper-0.26.0/PKG-INFO
```

### Comparing `kraken_wrapper-0.25.0/LICENSE` & `kraken_wrapper-0.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.25.0/pyproject.toml` & `kraken_wrapper-0.26.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-wrapper"
-version = "0.25.0"
+version = "0.26.0"
 description = ""
 authors = ["Unknown <me@unknown.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "kraken/wrapper", from = "src" }]
 classifiers = []
 keywords = []
@@ -18,15 +18,15 @@
 Documentation = "https://kraken-build.github.io/kraken-build/"
 Homepage = "https://kraken-build.github.io/kraken-build/"
 Repository = "https://github.com/kraken-build/kraken-build/"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
 keyring = "^23.8.2"
-kraken-common = "^0.25.0"
+kraken-common = "^0.26.0"
 pex = "^2.1.103"
 setuptools = ">=33.0.0"  # For pkg_resources
 termcolor = "^1.1.0"
 rich = "^13.4.2"
 
 # NOTE(@NiklasRosenstein): Need to pin transitive dependency markdown-it under 3.0 because it dropped Python 3.9
 #       support after that version. Technically this shouldn't be a big issue for runtime, but Mypy checks site
```

### Comparing `kraken_wrapper-0.25.0/src/kraken/wrapper/_buildend_venv.py` & `kraken_wrapper-0.26.0/src/kraken/wrapper/_buildend_venv.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import logging
 import os
+import shlex
 import subprocess
 import sys
 from pathlib import Path
 from typing import List, NoReturn
 
 from kraken.common import EnvironmentType, RequirementSpec, findpython, safe_rmpath
 from kraken.common.pyenv import VirtualEnvInfo
+from typing_extensions import Literal
 
-from ._buildenv import KRAKEN_MAIN_IMPORT_SNIPPET, BuildEnv, general_get_installed_distributions
+from ._buildenv import KRAKEN_MAIN_IMPORT_SNIPPET, BuildEnv, BuildEnvError, general_get_installed_distributions
 from ._lockfile import Distribution
 
 logger = logging.getLogger(__name__)
 
 
 def find_python_interpreter(constraint: str) -> str:
     """
@@ -34,27 +36,52 @@
     """
 
     def __init__(self, path: Path, incremental: bool = False) -> None:
         self._path = path
         self._venv = VirtualEnvInfo(self._path)
         self._incremental = incremental
 
+    def _run_command(
+        self, command: List[str], operation_name: str, log_file: Path, mode: Literal["a", "w"] = "w"
+    ) -> None:
+        log_file.parent.mkdir(parents=True, exist_ok=True)
+        with log_file.open(mode) as fp:
+            offset = fp.tell()
+            try:
+                subprocess.check_call(command, stdout=fp, stderr=fp)
+                return
+            except (subprocess.CalledProcessError, FileNotFoundError) as e:
+                exc = e
+        with log_file.open() as fp:
+            fp.seek(offset)
+            logger.error(
+                "'%s' failed (exit code: %d, command: %s). Output:\n\n%s",
+                operation_name,
+                exc.returncode if isinstance(exc, subprocess.CalledProcessError) else -1,
+                "$ " + " ".join(map(shlex.quote, command)),
+                fp.read(),
+            )
+            raise BuildEnvError(f"The command {command} failed.") from exc
+
     # BuildEnv
 
     def get_path(self) -> Path:
         return self._path
 
     def get_type(self) -> EnvironmentType:
         return EnvironmentType.VENV
 
     def get_installed_distributions(self) -> List[Distribution]:
         python = self._venv.get_bin("python")
         return general_get_installed_distributions([str(python), "-c", f"{KRAKEN_MAIN_IMPORT_SNIPPET}\nmain()"])
 
     def build(self, requirements: RequirementSpec, transitive: bool) -> None:
+        create_log = self._path.with_name(self._path.name + ".log") / "create.txt"
+        install_log = self._path.with_name(self._path.name + ".log") / "install.txt"
+
         if not self._incremental and self._path.exists():
             logger.debug("Removing existing virtual environment at %s", self._path)
             safe_rmpath(self._path)
 
         python_bin = str(self._venv.get_bin("python"))
 
         # If a virtual environment already exists, we should ensure that it matches the given interpreter constraint.
@@ -87,24 +114,24 @@
             else:
                 logger.info(
                     "No interpreter constraint specified, using current Python interpreter (%s)", sys.executable
                 )
                 python_origin_bin = sys.executable
 
             command = [python_origin_bin, "-m", "venv", str(self._path)]
-            logger.debug("Creating virtual environment at %s: %s", self._path, " ".join(command))
-            subprocess.check_call(command)
+            logger.info("Creating virtual environment at %s", os.path.relpath(self._path))
+            self._run_command(command, operation_name="Create virtual environment", log_file=create_log)
 
             # Upgrade Pip.
             command = [python_bin, "-m", "pip", "install", "--upgrade", "pip"]
-            logger.debug("Upgrading Pip: %s", command)
-            subprocess.check_call(command)
+            logger.info("Upgrading Pip in virtual environment.")
+            self._run_command(command, operation_name="Upgrade Pip", log_file=create_log, mode="a")
 
         else:
-            logger.debug("Reusing virtual environment at %s", self._path)
+            logger.info("Reusing virtual environment at %s", self._path)
 
         # Install requirements.
         command = [
             python_bin,
             "-m",
             "pip",
             "install",
@@ -113,16 +140,17 @@
             "--no-input",
         ]
         # Must enable transitive resolution because lock files are not currently cross platform (see kraken-wrapper#2).
         # if not transitive:
         #     command += ["--no-deps"]
         # TODO (@NiklasRosenstein): Handle requirements interpreter constraint (see kraken-wrapper#5).
         command += requirements.to_args()
+        logger.info("Installing dependencies.")
         logger.debug("Installing into build environment with Pip: %s", " ".join(command))
-        subprocess.check_call(command)
+        self._run_command(command, operation_name="Install dependencies", log_file=install_log)
 
         # Make sure the pythonpath from the requirements is encoded into the enviroment.
         command = [python_bin, "-c", "from sysconfig import get_path; print(get_path('purelib'))"]
         site_packages = Path(subprocess.check_output(command).decode().strip())
         pth_file = site_packages / "krakenw.pth"
         if requirements.pythonpath:
             logger.debug("Writing .pth file at %s", pth_file)
```

### Comparing `kraken_wrapper-0.25.0/src/kraken/wrapper/_buildenv.py` & `kraken_wrapper-0.26.0/src/kraken/wrapper/_buildenv.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,11 +91,17 @@
 
     def set(self, metadata: BuildEnvMetadata) -> None:
         self.path.parent.mkdir(parents=True, exist_ok=True)
         self.path.write_text(json.dumps(metadata.to_json()))
         self._metadata = metadata
 
 
+class BuildEnvError(Exception):
+    """
+    An error occurred while building the environment.
+    """
+
+
 def general_get_installed_distributions(kraken_command_prefix: Sequence[str]) -> list[Distribution]:
     command = [*kraken_command_prefix, "query", "env"]
     output = subprocess.check_output(command).decode()
     return [Distribution(x["name"], x["version"], x["requirements"], x["extras"]) for x in json.loads(output)]
```

### Comparing `kraken_wrapper-0.25.0/src/kraken/wrapper/_buildenv_manager.py` & `kraken_wrapper-0.26.0/src/kraken/wrapper/_buildenv_manager.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.25.0/src/kraken/wrapper/_buildenv_pex.py` & `kraken_wrapper-0.26.0/src/kraken/wrapper/_buildenv_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.25.0/src/kraken/wrapper/_config.py` & `kraken_wrapper-0.26.0/src/kraken/wrapper/_config.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.25.0/src/kraken/wrapper/_lockfile.py` & `kraken_wrapper-0.26.0/src/kraken/wrapper/_lockfile.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.25.0/src/kraken/wrapper/_option_sets.py` & `kraken_wrapper-0.26.0/src/kraken/wrapper/_option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.25.0/src/kraken/wrapper/_pex.py` & `kraken_wrapper-0.26.0/src/kraken/wrapper/_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.25.0/src/kraken/wrapper/main.py` & `kraken_wrapper-0.26.0/src/kraken/wrapper/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 from __future__ import annotations
 
 import argparse
-import builtins
 import getpass
 import logging
 import os
 import shlex
 import sys
 import time
-from functools import partial
 from pathlib import Path
 from textwrap import indent
 from typing import NamedTuple, NoReturn
 
 from kraken.common import (
     AsciiTable,
     BuildscriptMetadata,
     EnvironmentType,
     GitAwareProjectFinder,
     LoggingOptions,
     RequirementSpec,
     TomlConfigFile,
     datetime_to_iso8601,
-    deprecated_get_requirement_spec_from_file_header,
     inline_text,
 )
+from kraken.common.exceptions import exit_on_known_exceptions
 from termcolor import colored
 
 from . import __version__
+from ._buildenv import BuildEnvError
 from ._buildenv_manager import BuildEnvManager
 from ._config import DEFAULT_CONFIG_PATH, AuthModel
 from ._lockfile import Lockfile, calculate_lockfile
 from ._option_sets import AuthOptions, EnvOptions
 
 BUILDENV_PATH = Path("build/.kraken/venv")
 BUILDSCRIPT_FILENAME = ".kraken.py"
 BUILD_SUPPORT_DIRECTORY = "build-support"
 LOCK_FILENAME = ".kraken.lock"
 _FormatterClass = lambda prog: argparse.RawTextHelpFormatter(prog, max_help_position=60, width=120)  # noqa: 731
 logger = logging.getLogger(__name__)
-print = partial(builtins.print, "[krakenw]", flush=True)
-eprint = partial(print, file=sys.stderr)
 
 
 def _get_argument_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         "krakenw",
         formatter_class=_FormatterClass,
         description=inline_text(
@@ -94,32 +91,32 @@
 
 
 def lock(prog: str, argv: list[str], manager: BuildEnvManager, project: Project) -> NoReturn:
     parser = _get_lock_argument_parser(prog)
     parser.parse_args(argv)
 
     if not manager.exists():
-        print("error: cannot lock without a build environment")
+        logger.error("cannot lock without a build environment")
         sys.exit(1)
 
     environment = manager.get_environment()
     distributions = environment.get_installed_distributions()
     lockfile, extra_distributions = calculate_lockfile(project.requirements, distributions)
 
     if environment.get_type() == EnvironmentType.VENV:
         extra_distributions.discard("pip")  # We'll always have that in a virtual env.
 
     if extra_distributions:
-        eprint("found extra distributions in build enviroment:", ", ".join(extra_distributions))
+        logger.warning("Found extra distributions in your Kraken build enviroment: %s", ", ".join(extra_distributions))
 
     had_lockfile = project.lockfile_path.exists()
     lockfile.write_to(project.lockfile_path)
     manager.set_locked(lockfile)
 
-    eprint("lock file", "updated" if had_lockfile else "created", f"({project.lockfile_path})")
+    logger.info("Lock file %s (%s)", "updated" if had_lockfile else "created", os.path.relpath(project.lockfile_path))
     sys.exit(0)
 
 
 def _get_auth_argument_parser(prog: str) -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         prog,
         formatter_class=_FormatterClass,
@@ -180,15 +177,15 @@
 
 
 def list_pythons(prog: str, argv: list[str]) -> NoReturn:
     import rich
     from kraken.common import findpython
 
     if argv:
-        eprint(f"{prog}: error: unexpected arguments")
+        logger.error(f"{prog}: unexpected arguments")
         sys.exit(1)
 
     interpreters = findpython.evaluate_candidates(findpython.get_candidates(), findpython.InterpreterVersionCache())
     table = findpython.build_rich_table(interpreters)
     rich.print(table)
     sys.exit(0)
 
@@ -230,73 +227,74 @@
     install = reinstall or upgrade or not exists
 
     operation: str
     reason: str | None = None
 
     if not exists:
         env_type = env_type or env_type or manager.get_environment().get_type()
-        operation = "initializing"
+        operation = "Initializing"
     elif upgrade:
-        operation = "upgrading"
+        operation = "Upgrading"
     elif reinstall:
-        operation = "reinstalling"
+        operation = "Reinstalling"
     else:
-        operation = "reusing"
+        operation = "Reusing"
 
     current_type = manager.get_environment().get_type()
     if env_type is not None:
         type_changed = exists and env_type != current_type
         if not install and type_changed:
             install = True
             manager.remove()
-            operation = "re-initializing"
+            operation = "Re-initializing"
             reason = f"type changed from {current_type.name}"
         elif install and type_changed:
             reason = f"type changed from {current_type.name}"
 
     if not install and exists:
         metadata = manager.get_metadata()
         if project.lockfile and metadata.requirements_hash != project.lockfile.to_pinned_requirement_spec().to_hash(
             metadata.hash_algorithm
         ):
             install = True
-            operation = "re-initializing"
+            operation = "Re-initializing"
             reason = "outdated compared to lockfile"
         if not project.lockfile and metadata.requirements_hash != project.requirements.to_hash(metadata.hash_algorithm):
             install = True
-            operation = "re-initializing"
+            operation = "Re-initializing"
             reason = "outdated compared to requirements"
 
     if install:
         if not project.lockfile or upgrade:
             source_name = "requirements"
             source = project.requirements
+            source_file = project.requirements_path
             transitive = True
         else:
             source_name = "lock file"
             source = project.lockfile.to_pinned_requirement_spec()
+            source_file = project.lockfile_path
             transitive = False
 
         env_type = env_type or manager.get_environment().get_type()
-        eprint(
+        logger.info(
+            "%s build environment from %s (%s)%s",
             operation,
-            "build environment of type",
-            env_type.name,
-            "from",
             source_name,
-            f"({reason})" if reason else "",
+            os.path.relpath(source_file),
+            f" ({reason})" if reason else "",
         )
 
         tstart = time.perf_counter()
         manager.install(source, env_type, transitive)
         duration = time.perf_counter() - tstart
-        eprint(f"operation complete after {duration:.3f}s")
+        logger.info("Operation complete after %.3fs.", duration)
 
     else:
-        eprint(operation, "build environment of type", current_type.name)
+        logger.info("%s build environment of type %s", operation, current_type.name)
 
 
 class Project(NamedTuple):
     directory: Path
     requirements_path: Path
     requirements: RequirementSpec
     lockfile_path: Path
@@ -312,63 +310,55 @@
     :param directory: The directory for which to load the build project details for.
     :param outdated_check: If enabled, performs a check to see if the requirements that the lockfile was
         generated with is outdated compared to the project requirements.
     """
 
     project_info = GitAwareProjectFinder.default().find_project(directory)
     if not project_info:
-        eprint("error: no buildscript")
+        logger.error("no buildscript")
         sys.exit(1)
     script, runner = project_info
 
     # Load requirement spec from build script.
-    logger.debug('loading requirements from "%s" (runner: %s)', script, runner)
+    logger.debug('Loading requirements from "%s" (runner: %s)', script, runner)
 
-    # For backwards compatibility, support loading the requirements from the comment header.
-    requirements = deprecated_get_requirement_spec_from_file_header(script)
-    if requirements is not None:
-        eprint(
-            "error: The # ::requirements header is deprecated and support for it will be removed in a future version "
-            "of kraken-wrapper. Please use the `buildscript()` function from the `kraken.common` package "
-            "from now on.\n\n%s\n"
-            % indent(runner.get_buildscript_call_recommendation(requirements.to_metadata()), "    "),
+    # Extract the metadata provided by the buildscript() function call at the top of the build script.
+    if not runner.has_buildscript_call(script):
+        metadata = BuildscriptMetadata(requirements=["kraken-core"])
+        logger.error(
+            "Kraken build scripts must call the `buildscript()` function to be compatible with Kraken wrapper. "
+            "Please add something like this at the top of your build script:\n\n%s\n"
+            % indent(runner.get_buildscript_call_recommendation(metadata), "    "),
         )
+        sys.exit(1)
 
-    # Otherwise, extract the relevant data from the buildscript() call instead.
-    else:
-        if not runner.has_buildscript_call(script):
-            metadata = BuildscriptMetadata(requirements=["kraken-core"])
-            eprint(
-                "Kraken build scripts must call the `buildscript()` function to be compatible with Kraken wrapper. "
-                "Please add something like this at the top of your build script:\n\n%s\n"
-                % indent(runner.get_buildscript_call_recommendation(metadata), "    "),
-            )
-            sys.exit(1)
-
-        with BuildscriptMetadata.capture() as future:
-            runner.execute_script(script, {})
-        assert future.done()
-        requirements = RequirementSpec.from_metadata(future.result())
-
-    # Derive the lockfile path.
-    lockfile_path = script.with_suffix(".lock")
+    with BuildscriptMetadata.capture() as future:
+        runner.execute_script(script, {})
+    assert future.done()
+    requirements = RequirementSpec.from_metadata(future.result())
 
     # Load lockfile if it exists.
+    lockfile_path = script.with_suffix(".lock")
     if lockfile_path.is_file():
         logger.debug('loading lockfile from "%s"', lockfile_path)
         lockfile = Lockfile.from_path(lockfile_path)
         if outdated_check and lockfile and lockfile.requirements != requirements:
-            eprint(f'lock file "{lockfile_path}" is outdated compared to requirements in "{script}"')
-            eprint("consider updating the lock file with `krakenw --upgrade lock`")
+            logger.warning(
+                'Lock file "%s" is outdated compared to requirements in "%s". Consider updating the lock file with '
+                '"krakenw --upgrade lock"',
+                os.path.relpath(lockfile_path),
+                os.path.relpath(script),
+            )
     else:
         lockfile = None
 
     return Project(script.parent, script, requirements, lockfile_path, lockfile)
 
 
+@exit_on_known_exceptions(BuildEnvError, exit_code=2)
 def main() -> NoReturn:
     parser = _get_argument_parser()
     args = parser.parse_args()
     logging_options = LoggingOptions.collect(args)
     logging_options.init_logging()
     env_options = EnvOptions.collect(args)
 
@@ -396,22 +386,22 @@
 
     # Execute environment operations before delegating the command.
 
     is_lock_command = cmd in ("lock", "l")
 
     if env_options.status:
         if cmd or argv:
-            eprint("error: --status option must be used alone")
+            logger.error("--status option must be used alone")
             sys.exit(1)
         _print_env_status(manager, project)
         sys.exit(0)
 
     if env_options.uninstall:
         if cmd or argv:
-            eprint("error: --uninstall option must be used alone")
+            logger.error("--uninstall option must be used alone")
             sys.exit(1)
         manager.remove()
         sys.exit(0)
     if env_options.any() or not is_lock_command:
         _ensure_installed(
             manager,
             project,
@@ -427,14 +417,14 @@
     elif cmd in ("l", "lock"):
         lock(f"{parser.prog} lock", argv, manager, project)
 
     else:
         if project.directory.absolute() != Path.cwd():
             argv = ["-p", str(project.directory)] + argv
         command = [cmd, *argv]
-        eprint("$", " ".join(map(shlex.quote, ["kraken"] + command)))
+        logger.info("$ %s", " ".join(map(shlex.quote, ["kraken"] + command)))
         environment = manager.get_environment()
         environment.dispatch_to_kraken_cli(command)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `kraken_wrapper-0.25.0/PKG-INFO` & `kraken_wrapper-0.26.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kraken-wrapper
-Version: 0.25.0
+Version: 0.26.0
 Summary: 
 License: MIT
 Author: Unknown
 Author-email: me@unknown.org
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keyring (>=23.8.2,<24.0.0)
-Requires-Dist: kraken-common (>=0.25.0,<0.26.0)
+Requires-Dist: kraken-common (>=0.26.0,<0.27.0)
 Requires-Dist: markdown-it-py (<3.0.0)
 Requires-Dist: pex (>=2.1.103,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: setuptools (>=33.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/kraken-build/kraken-build/issues
 Project-URL: Documentation, https://kraken-build.github.io/kraken-build/
@@ -30,11 +30,11 @@
 This projects implements `krakenw`, the wrapper CLI for the Kraken build system that enables reproducible builds
 via lock files and executing builds from inside subdirectories.
 
 For more information, check out the [Kraken Documentation](https://kraken-build.github.io/docs/).
 
 __Installation__
 
-You need Python 3.7+, <3.11 (currently limited due to an incompatibility with Dill).
+You need Python 3.7 or newer:
 
     $ pipx install kraken-wrapper
```

