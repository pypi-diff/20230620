# Comparing `tmp/openai-pygenerator-0.4.4.tar.gz` & `tmp/openai-pygenerator-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-pygenerator-0.4.4.tar", last modified: Mon Jun 19 20:29:48 2023, max compression
+gzip compressed data, was "openai-pygenerator-0.4.5.tar", last modified: Tue Jun 20 09:14:24 2023, max compression
```

## Comparing `openai-pygenerator-0.4.4.tar` & `openai-pygenerator-0.4.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.847030 openai-pygenerator-0.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.843029 openai-pygenerator-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.843029 openai-pygenerator-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-19 20:29:48.847030 openai-pygenerator-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/mypy-tests.ini
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-19 20:29:48.847030 openai-pygenerator-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.843029 openai-pygenerator-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.847030 openai-pygenerator-0.4.4/src/openai_pygenerator/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/src/openai_pygenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/src/openai_pygenerator/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/src/openai_pygenerator/openai_pygenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.847030 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-19 20:29:48.000000 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-19 20:29:48.000000 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 20:29:48.000000 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 20:29:48.000000 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-19 20:29:48.000000 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 20:29:48.000000 openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 20:29:48.847030 openai-pygenerator-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-19 20:29:30.000000 openai-pygenerator-0.4.4/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:14:24.561960 openai-pygenerator-0.4.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:14:24.549960 openai-pygenerator-0.4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:14:24.557960 openai-pygenerator-0.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-20 09:14:24.561960 openai-pygenerator-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/mypy-tests.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-20 09:14:24.561960 openai-pygenerator-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:14:24.549960 openai-pygenerator-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:14:24.557960 openai-pygenerator-0.4.5/src/openai_pygenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/src/openai_pygenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/src/openai_pygenerator/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/src/openai_pygenerator/openai_pygenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/src/openai_pygenerator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:14:24.561960 openai-pygenerator-0.4.5/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-20 09:14:24.000000 openai-pygenerator-0.4.5/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-20 09:14:24.000000 openai-pygenerator-0.4.5/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:14:24.000000 openai-pygenerator-0.4.5/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 09:14:24.000000 openai-pygenerator-0.4.5/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 09:14:24.000000 openai-pygenerator-0.4.5/src/openai_pygenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 09:14:24.000000 openai-pygenerator-0.4.5/src/openai_pygenerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:14:24.561960 openai-pygenerator-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-20 09:14:06.000000 openai-pygenerator-0.4.5/tests/test_gpt.py
```

### Comparing `openai-pygenerator-0.4.4/.github/workflows/python-package.yml` & `openai-pygenerator-0.4.5/.github/workflows/python-package.yml`

 * *Files 7% similar despite different names*

```diff
@@ -26,12 +26,11 @@
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install .[dev]
     - name: Pre-commit tests
       run: |
-        export PYTHONPATH="./src"
         pre-commit run --all-files
     - name: Test with pytest
       run: |
         pytest
```

### Comparing `openai-pygenerator-0.4.4/.github/workflows/python-publish.yml` & `openai-pygenerator-0.4.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.4/.pre-commit-config.yaml` & `openai-pygenerator-0.4.5/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 # mypy
 - repo: https://github.com/pre-commit/mirrors-mypy
   rev: 'v1.2.0'  # Use the sha / tag you want to point at
   hooks:
     - id: mypy
       exclude: 'jupyter-book/.*|tests/.*'
-      args: [--config=mypy.ini]
+      args: [--config=mypy.ini, --explicit-package-bases]
       additional_dependencies: [ pandas-stubs ]
 
 # mypy for tests
 - repo: https://github.com/pre-commit/mirrors-mypy
   rev: 'v1.2.0'  # Use the sha / tag you want to point at
   hooks:
     - id: mypy
```

### Comparing `openai-pygenerator-0.4.4/.pylintrc` & `openai-pygenerator-0.4.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.4/LICENSE.txt` & `openai-pygenerator-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.4/PKG-INFO` & `openai-pygenerator-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.4
+Version: 0.4.5
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai-pygenerator-0.4.4/README.md` & `openai-pygenerator-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.4/pyproject.toml` & `openai-pygenerator-0.4.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-data]
-"*" = ["py.typed"]
+openai_pygenerator = ["py.typed"]
 
 [tool.setuptools_scm]
 write_to = "src/version.py"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
```

### Comparing `openai-pygenerator-0.4.4/src/openai_pygenerator/example.py` & `openai-pygenerator-0.4.5/src/openai_pygenerator/example.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     print(working)
 
     heading("Session transcript:")
     print(session.transcript)
 
 
 def creative_answer(prompt: str, num_completions: int = 1) -> Completions:
-    return high_temp_completions([user_message(prompt)], n=num_completions)
+    return high_temp_completions([user_message(prompt)], num_completions)
 
 
 def pick_color(num_completions: int) -> Completions:
     return creative_answer(
         "Pick a color at random and then just tell me your choice, e.g. 'red'",
         num_completions,
     )
```

### Comparing `openai-pygenerator-0.4.4/src/openai_pygenerator/openai_pygenerator.py` & `openai-pygenerator-0.4.5/src/openai_pygenerator/openai_pygenerator.py`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/PKG-INFO` & `openai-pygenerator-0.4.5/src/openai_pygenerator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.4
+Version: 0.4.5
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openai-pygenerator-0.4.4/src/openai_pygenerator.egg-info/SOURCES.txt` & `openai-pygenerator-0.4.5/src/openai_pygenerator.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 setup.cfg
 setup.py
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 src/openai_pygenerator/__init__.py
 src/openai_pygenerator/example.py
 src/openai_pygenerator/openai_pygenerator.py
+src/openai_pygenerator/py.typed
 src/openai_pygenerator.egg-info/PKG-INFO
 src/openai_pygenerator.egg-info/SOURCES.txt
 src/openai_pygenerator.egg-info/dependency_links.txt
 src/openai_pygenerator.egg-info/entry_points.txt
 src/openai_pygenerator.egg-info/requires.txt
 src/openai_pygenerator.egg-info/top_level.txt
 tests/test_gpt.py
```

### Comparing `openai-pygenerator-0.4.4/tests/test_gpt.py` & `openai-pygenerator-0.4.5/tests/test_gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from openai_pygenerator import (
     GPT_MAX_RETRIES,
     ChatSession,
     Completer,
     Completion,
     Completions,
+    History,
     Role,
     content,
     gpt_completions,
     role,
     transcript,
     user_message,
 )
@@ -105,15 +106,15 @@
     result = list(transcript(iter(test_messages)))
     for i in range(10):
         assert result[i] == test_message(i)
 
 
 def test_chat_session():
     def completer(response: str) -> Completer:
-        def mock_complete(_history: Completions, _n: int) -> Completions:
+        def mock_complete(_history: History, _n: int) -> Completions:
             yield {"role": "assistant", "content": response}
 
         return mock_complete
 
     session = ChatSession(completer("response1"))
     result = session.ask("First question")
     assert result == "response1"
```

