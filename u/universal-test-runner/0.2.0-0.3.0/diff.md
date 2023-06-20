# Comparing `tmp/universal_test_runner-0.2.0.tar.gz` & `tmp/universal_test_runner-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal_test_runner-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "universal_test_runner-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `universal_test_runner-0.2.0.tar` & `universal_test_runner-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-06-05 07:04:09.894832 universal_test_runner-0.2.0/LICENSE
--rw-r--r--   0        0        0     3707 2023-06-17 06:38:49.383842 universal_test_runner-0.2.0/README.md
--rw-r--r--   0        0        0     1198 2023-06-17 06:36:07.561918 universal_test_runner-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 05:21:33.982200 universal_test_runner-0.2.0/universal_test_runner/__init__.py
--rw-r--r--   0        0        0     1570 2023-06-18 18:24:18.266813 universal_test_runner-0.2.0/universal_test_runner/context.py
--rw-r--r--   0        0        0     2481 2023-06-18 18:24:02.933515 universal_test_runner-0.2.0/universal_test_runner/matchers.py
--rw-r--r--   0        0        0     1080 2023-06-18 18:06:08.532252 universal_test_runner-0.2.0/universal_test_runner/runner.py
--rw-r--r--   0        0        0     4803 1970-01-01 00:00:00.000000 universal_test_runner-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-05 07:04:09.894832 universal_test_runner-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4145 2023-06-20 00:04:36.575042 universal_test_runner-0.3.0/README.md
+-rw-r--r--   0        0        0     1306 2023-06-20 07:30:24.762970 universal_test_runner-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 05:21:33.982200 universal_test_runner-0.3.0/universal_test_runner/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-19 22:38:42.426279 universal_test_runner-0.3.0/universal_test_runner/cli.py
+-rw-r--r--   0        0        0     1784 2023-06-19 22:41:04.042871 universal_test_runner-0.3.0/universal_test_runner/context.py
+-rw-r--r--   0        0        0     3559 2023-06-20 07:19:47.780665 universal_test_runner-0.3.0/universal_test_runner/matchers.py
+-rw-r--r--   0        0        0      812 2023-06-19 22:38:32.764857 universal_test_runner-0.3.0/universal_test_runner/runner.py
+-rw-r--r--   0        0        0     5301 1970-01-01 00:00:00.000000 universal_test_runner-0.3.0/PKG-INFO
```

### Comparing `universal_test_runner-0.2.0/LICENSE` & `universal_test_runner-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `universal_test_runner-0.2.0/README.md` & `universal_test_runner-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,31 +18,40 @@
 
 1. The runner itself should need no configuration - it Just Works
 2. It should pass all arguments through to the underlying test command
 3. It should have wide language and test runner support; please open an issue if your use case isn't supported!
 
 ## Usage
 
-Once installed, the command `t` will be available. Run that in a folder with tests and it'll do its best to run your unit tests.
+Once installed, the command `t` will be available. Run that in a folder with tests and it'll do its best to run your unit tests:
 
 ```
 % t
 ====================== test session starts ======================
 platform darwin -- Python 3.11.0, pytest-7.3.1, pluggy-1.0.0
 rootdir: /Users/david/projects/universal-test-runner
 collected 37 items
 
 tests/test_matchers.py .........................          [ 67%]
 tests/test_runner.py ............                         [100%]
 
 ====================== 37 passed in 0.04s =======================
 ```
 
+It passes all arguments and environment modifications down to the chosen test runner.
+
 If it can't guess the testing method, it will tell you so. Feel free to open an issue to request wider language support!
 
+### Debugging
+
+The package also ships a program to surface info about itself: `universal-test-runner`. It has a few key pieces of functionality:
+
+- the `universal-test-runner --version` flag, which prints info about your installed package version
+- the `universal-test-runner debug` command, which prints info about which matcher would run (and why)
+
 ## Supported Languages
 
 1. Python
    - uses `pytest` if you've run `pytest` before
    - looks for a `tests.py` file if not
 2. Rust
    - `cargo test`
```

### Comparing `universal_test_runner-0.2.0/pyproject.toml` & `universal_test_runner-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [project]
 name = "universal-test-runner"
-version = "0.2.0"
+version = "0.3.0"
 
 authors = [{ name = "David Brownman", email = "beamneocube@gmail.com" }]
 description = "Universal, language-aware unit test runner."
 readme = "README.md"
 license = { file = "LICENSE" }
 
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
-  "Natural Language :: English",
+  "Topic :: Software Development :: Testing",
 ]
-keywords = ["testing"]
+keywords = ["testing", "test-runner", "pytest"]
 
-dependencies = []
+dependencies = ["click==8.1.3"]
 
 [project.optional-dependencies]
 test = ["pytest==7.3.1", "responses==0.23.1", "pyright==1.1.309"]
 release = ["twine==4.0.2", "build==0.10.0"]
 
 [project.urls]
 "Homepage" = "https://github.com/xavdid/universal-test-runner"
 "Bug Tracker" = "https://github.com/xavdid/universal-test-runner/issues"
 "Author" = "https://xavd.id"
 "Changelog" = "https://github.com/xavdid/universal-test-runner/blob/main/CHANGELOG.md"
 
 [project.scripts]
 t = "universal_test_runner.runner:run"
+universal-test-runner = "universal_test_runner.cli:cli"
 
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 # needed so the LSP performs typechecking
 [tool.pyright]
```

### Comparing `universal_test_runner-0.2.0/universal_test_runner/runner.py` & `universal_test_runner-0.3.0/universal_test_runner/runner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,30 @@
-import os
 import subprocess
 import sys
-from pathlib import Path
 
 from universal_test_runner.context import Context
-from universal_test_runner.matchers import ALL_MATCHERS
+from universal_test_runner.matchers import find_test_command
 
 
-def run_test_command(context: Context) -> int:
-    for matcher in ALL_MATCHERS:
-        if not matcher.matches(context):
-            continue
-
-        command = [*matcher.command, *context.args]
-
-        try:
-            return subprocess.run(command).returncode
-        except FileNotFoundError:
-            # e.g. if `pytest` is run, but not installed
-            # we capture the error so there's not a Python traceback shown
-            print("command not found:", command[0])
-            return 1
-    else:
+def run_test_command(command: list[str]) -> int:
+    if not command:
         print("no testing method found!")
         return 1
 
+    try:
+        return subprocess.run(command).returncode
+    except FileNotFoundError:
+        # e.g. if `pytest` is run, but not installed
+        # we capture the error so there's not a Python traceback shown
+        print(f"command not found: {command[0]}")
+        return 1
 
-def run():
-    current_dir = os.getcwd()
-
-    c = Context(
-        # sorting makes the file list deterministic
-        sorted(Path(current_dir).iterdir()),
-        # pass any arguments to the test runner through to the test command
-        sys.argv[1:],
-    )
 
-    sys.exit(run_test_command(c))
+# not a click handler, since this is just a passthrough for the underlying test runner
+def run():
+    context = Context.from_invocation()
+    command = find_test_command(context)
+    sys.exit(run_test_command(command))
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `universal_test_runner-0.2.0/PKG-INFO` & `universal_test_runner-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: universal-test-runner
-Version: 0.2.0
+Version: 0.3.0
 Summary: Universal, language-aware unit test runner.
-Keywords: testing
+Keywords: testing,test-runner,pytest
 Author-email: David Brownman <beamneocube@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: click==8.1.3
 Requires-Dist: twine==4.0.2 ; extra == "release"
 Requires-Dist: build==0.10.0 ; extra == "release"
 Requires-Dist: pytest==7.3.1 ; extra == "test"
 Requires-Dist: responses==0.23.1 ; extra == "test"
 Requires-Dist: pyright==1.1.309 ; extra == "test"
 Project-URL: Author, https://xavd.id
 Project-URL: Bug Tracker, https://github.com/xavdid/universal-test-runner/issues
@@ -44,31 +45,40 @@
 
 1. The runner itself should need no configuration - it Just Works
 2. It should pass all arguments through to the underlying test command
 3. It should have wide language and test runner support; please open an issue if your use case isn't supported!
 
 ## Usage
 
-Once installed, the command `t` will be available. Run that in a folder with tests and it'll do its best to run your unit tests.
+Once installed, the command `t` will be available. Run that in a folder with tests and it'll do its best to run your unit tests:
 
 ```
 % t
 ====================== test session starts ======================
 platform darwin -- Python 3.11.0, pytest-7.3.1, pluggy-1.0.0
 rootdir: /Users/david/projects/universal-test-runner
 collected 37 items
 
 tests/test_matchers.py .........................          [ 67%]
 tests/test_runner.py ............                         [100%]
 
 ====================== 37 passed in 0.04s =======================
 ```
 
+It passes all arguments and environment modifications down to the chosen test runner.
+
 If it can't guess the testing method, it will tell you so. Feel free to open an issue to request wider language support!
 
+### Debugging
+
+The package also ships a program to surface info about itself: `universal-test-runner`. It has a few key pieces of functionality:
+
+- the `universal-test-runner --version` flag, which prints info about your installed package version
+- the `universal-test-runner debug` command, which prints info about which matcher would run (and why)
+
 ## Supported Languages
 
 1. Python
    - uses `pytest` if you've run `pytest` before
    - looks for a `tests.py` file if not
 2. Rust
    - `cargo test`
```

