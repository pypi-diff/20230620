# Comparing `tmp/cycept-0.0.5.tar.gz` & `tmp/cycept-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycept-0.0.5.tar", last modified: Sun May 14 16:21:22 2023, max compression
+gzip compressed data, was "cycept-0.0.6.tar", last modified: Tue Jun 20 13:25:46 2023, max compression
```

## Comparing `cycept-0.0.5.tar` & `cycept-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-05-14 16:21:22.385956 cycept-0.0.5/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1068 2023-04-01 21:39:01.000000 cycept-0.0.5/LICENSE
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     8681 2023-05-14 16:21:22.385956 cycept-0.0.5/PKG-INFO
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     7263 2023-05-14 03:17:33.000000 cycept-0.0.5/README.md
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-05-14 16:21:22.385956 cycept-0.0.5/cycept/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     2875 2023-04-18 11:56:30.000000 cycept-0.0.5/cycept/__init__.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    32043 2023-05-14 15:43:54.000000 cycept-0.0.5/cycept/call.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     4600 2023-05-03 20:25:08.000000 cycept-0.0.5/cycept/compile.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    25042 2023-05-14 15:59:16.000000 cycept-0.0.5/cycept/core.py
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-05-14 16:21:22.385956 cycept-0.0.5/cycept/tests/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      974 2023-05-14 00:06:11.000000 cycept-0.0.5/cycept/tests/__init__.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    20384 2023-05-14 11:06:32.000000 cycept-0.0.5/cycept/tests/test_bench.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    12469 2023-05-14 15:49:16.000000 cycept-0.0.5/cycept/tests/test_cycept.py
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-05-14 16:21:22.385956 cycept-0.0.5/cycept.egg-info/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     8681 2023-05-14 16:21:22.000000 cycept-0.0.5/cycept.egg-info/PKG-INFO
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      328 2023-05-14 16:21:22.000000 cycept-0.0.5/cycept.egg-info/SOURCES.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        1 2023-05-14 16:21:22.000000 cycept-0.0.5/cycept.egg-info/dependency_links.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      182 2023-05-14 16:21:22.000000 cycept-0.0.5/cycept.egg-info/requires.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        7 2023-05-14 16:21:22.000000 cycept-0.0.5/cycept.egg-info/top_level.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1745 2023-05-14 16:18:21.000000 cycept-0.0.5/pyproject.toml
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       38 2023-05-14 16:21:22.385956 cycept-0.0.5/setup.cfg
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-06-20 13:25:46.675572 cycept-0.0.6/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1068 2023-04-01 21:39:01.000000 cycept-0.0.6/LICENSE
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     8681 2023-06-20 13:25:46.675572 cycept-0.0.6/PKG-INFO
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     7263 2023-05-14 03:17:33.000000 cycept-0.0.6/README.md
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-06-20 13:25:46.675572 cycept-0.0.6/cycept/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     2875 2023-04-18 11:56:30.000000 cycept-0.0.6/cycept/__init__.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    32037 2023-05-29 18:01:59.000000 cycept-0.0.6/cycept/call.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     4600 2023-05-03 20:25:08.000000 cycept-0.0.6/cycept/compile.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    25251 2023-06-20 12:55:24.000000 cycept-0.0.6/cycept/core.py
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-06-20 13:25:46.675572 cycept-0.0.6/cycept/tests/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      974 2023-05-14 00:06:11.000000 cycept-0.0.6/cycept/tests/__init__.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    21012 2023-05-19 20:22:49.000000 cycept-0.0.6/cycept/tests/test_bench.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    12632 2023-06-20 12:39:21.000000 cycept-0.0.6/cycept/tests/test_cycept.py
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-06-20 13:25:46.675572 cycept-0.0.6/cycept.egg-info/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     8681 2023-06-20 13:25:46.000000 cycept-0.0.6/cycept.egg-info/PKG-INFO
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      328 2023-06-20 13:25:46.000000 cycept-0.0.6/cycept.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        1 2023-06-20 13:25:46.000000 cycept-0.0.6/cycept.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      182 2023-06-20 13:25:46.000000 cycept-0.0.6/cycept.egg-info/requires.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        7 2023-06-20 13:25:46.000000 cycept-0.0.6/cycept.egg-info/top_level.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1745 2023-06-20 13:18:06.000000 cycept-0.0.6/pyproject.toml
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       38 2023-06-20 13:25:46.675572 cycept-0.0.6/setup.cfg
```

### Comparing `cycept-0.0.5/LICENSE` & `cycept-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cycept-0.0.5/PKG-INFO` & `cycept-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycept
-Version: 0.0.5
+Version: 0.0.6
 Summary: Effortless just-in-time compilation of Python functions, powered by Cython
 Author-email: Jeppe Dakin <jeppe_dakin@hotmail.com>
 Project-URL: Download, https://pypi.python.org/pypi/cycept
 Project-URL: Changelog, https://github.com/jmd-dk/cycept/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/jmd-dk/cycept/issues
 Project-URL: Source code, https://github.com/jmd-dk/cycept
 Classifier: Intended Audience :: Developers
```

### Comparing `cycept-0.0.5/README.md` & `cycept-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cycept-0.0.5/cycept/__init__.py` & `cycept-0.0.6/cycept/__init__.py`

 * *Files identical despite different names*

### Comparing `cycept-0.0.5/cycept/call.py` & `cycept-0.0.6/cycept/call.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
             # (e.g. 4 space indentation).
             source = ast.unparse(ast.parse(source))
         # Remove jit decorator and decorators above it
         from .core import jit
         lines = source.split('\n')
         for i, line in enumerate(lines):
             if match := re.search(r'^@(.+?)(\(|$)', line):
-                deco_name = match.group(1).strip()
+                deco_name = match[1].strip()
                 try:
                     deco_func = eval(deco_name, self.module_dict)
                 except Exception:
                     continue
                 if deco_func is jit:
                     lines = lines[i+1:]
                     break
@@ -363,15 +363,15 @@
             def visit_Attribute(self, node):
                 node = self.generic_visit(node)
                 name = asciify(node.attr)
                 return type(node)(**(vars(node) | {'attr': name}))
         self._source = UnicodeRenamer(self).rename()
         # Note that name changes caused by the above ASCIIfication
         # makes the AST, the function signature and many other attributes
-        # invalid, yet me do not flag any attributes as such.
+        # invalid, yet we do not flag any attributes as such.
 
     # Method for wrapping NumPy array variables in numpy.asarray()
     # whenever operations are used that do not work with Cython memoryviews.
     def protect_arrays(self, array_args):
         from .core import NdarrayTypeInfo
         # Find local NumPy arrays
         names = {
```

### Comparing `cycept-0.0.5/cycept/compile.py` & `cycept-0.0.6/cycept/compile.py`

 * *Files identical despite different names*

### Comparing `cycept-0.0.5/cycept/core.py` & `cycept-0.0.6/cycept/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,18 +38,20 @@
             ),
             RuntimeWarning,
         )
     path = pathlib.Path(__file__).resolve().parent
     while True:
         if (path_pyproject := path / 'pyproject.toml').is_file():
             if (tomllib := get_tomllib()) is not None:
-                info = tomllib.loads(path_pyproject.read_text('utf-8'))
-                if info['project']['name'] == 'cycept':
-                    return info['project']['version']
-                break
+                try:
+                    info = tomllib.loads(path_pyproject.read_text('utf-8'))
+                    if info['project']['name'] == 'cycept':
+                        return info['project']['version']
+                except Exception:
+                    pass
             break
         if path.parent == path:
             break
         path = path.parent
     # Get version from meta data on installed package
     try:
         return importlib.metadata.version('cycept')
@@ -562,26 +564,29 @@
     # Define and call modified function within definition module,
     # with recording of the types added as a side effect.
     # Temporarily add a reference to this module on the module of
     # the function to be jitted. Also add non-local objects referenced by
     # the function directly to the module.
     @contextlib.contextmanager
     def hack_module_dict():
-        call.module_dict[cycept_module_refname] = sys.modules['cycept.core']
+        add_module_ref = (cycept_module_refname not in call.module_dict)
+        if add_module_ref:
+            call.module_dict[cycept_module_refname] = sys.modules['cycept.core']
         nonlocals_ori = {}
         for name, val in call.nonlocals.items():
             if name in call.module_dict:
                 nonlocals_ori[name] = call.module_dict[name]
             call.module_dict[name] = val
         try:
             yield
         except Exception:
             raise
         finally:
-            call.module_dict.pop(cycept_module_refname)
+            if add_module_ref:
+                call.module_dict.pop(cycept_module_refname)
             for name in call.nonlocals:
                 call.module_dict.pop(name)
             for name, val in nonlocals_ori.items():
                 call.module_dict[name] = val
     with hack_module_dict():
         # Define modified function within definition module
         exec(source, call.module_dict)
```

### Comparing `cycept-0.0.5/cycept/tests/__init__.py` & `cycept-0.0.6/cycept/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cycept-0.0.5/cycept/tests/test_bench.py` & `cycept-0.0.6/cycept/tests/test_bench.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,30 +403,54 @@
     timings = perf(f, n)
     if setup['asserts']:
         assert timings.cycept < timings.python / 4
 
 
 def test_wallis():
     """Compute π using the Wallis product.
-    This tests the performance of floating-point operations.
+    This tests the performance of integer and floating-point operations.
     """
     def f(n):
+        i : np.int64
         π = 2
         for i in range(1, n):
             π *= 4 * i ** 2 / (4 * i ** 2 - 1)
         return π
     def f_numpy(n):
         a = 4 * np.arange(1, n, dtype=np.int64) ** 2
         return 2 * np.prod(a / (a - 1))
     n = 2_000_000
     timings = perf((f, f_numpy), n)
     if setup['asserts']:
         assert timings.cycept < timings.python / 50
 
 
+def test_leibniz():
+    """Compute π using the Leibniz formula.
+    This tests the performance of floating-point operations.
+    """
+    def f(n):
+        π = 1
+        sgn = 1
+        for i in range(3, n, 2):
+            sgn = -sgn
+            π += sgn / i
+        π *= 4
+        return π
+    def f_numpy(n):
+        denom = np.arange(1, n, 2, dtype=np.int64)
+        num = np.ones_like(denom)
+        num[1::2] = -1
+        return 4 * (num / denom).sum()
+    n = 3_000_000
+    timings = perf((f, f_numpy), n)
+    if setup['asserts']:
+        assert timings.cycept < timings.python / 10
+
+
 def test_fibonacci():
     """Compute the n'th Fibonacci number using recursion.
     This tests the performance of recursive function calls.
     """
     def f(n):
         if n < 2:
             return n
```

### Comparing `cycept-0.0.5/cycept/tests/test_cycept.py` & `cycept-0.0.6/cycept/tests/test_cycept.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,25 @@
         call = next(iter(g.__cycept__.values()))
         assert call.types['return'] == 'cython.Py_ssize_t'
     f = lambda a: 2*a
     test(f)
     test(lambda a: 2*a)
 
 
+def test_callfromjitted():
+    @jit
+    def f(a):
+        return 5*a
+    @jit
+    def g(b):
+        return f(b)
+    for _ in range(2):
+        assert g(2) == 10
+
+
 def test_closure():
     @jit
     def f(a):
         def g():
             return 5*a + 7*b
         return 1 + 2*a + 3*b + g()
     b = 2
```

### Comparing `cycept-0.0.5/cycept.egg-info/PKG-INFO` & `cycept-0.0.6/cycept.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycept
-Version: 0.0.5
+Version: 0.0.6
 Summary: Effortless just-in-time compilation of Python functions, powered by Cython
 Author-email: Jeppe Dakin <jeppe_dakin@hotmail.com>
 Project-URL: Download, https://pypi.python.org/pypi/cycept
 Project-URL: Changelog, https://github.com/jmd-dk/cycept/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/jmd-dk/cycept/issues
 Project-URL: Source code, https://github.com/jmd-dk/cycept
 Classifier: Intended Audience :: Developers
```

### Comparing `cycept-0.0.5/pyproject.toml` & `cycept-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = [
-    "setuptools >= 65.6.0, < 68",
+    "setuptools >= 65.6.0, < 69",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cycept"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name="Jeppe Dakin", email="jeppe_dakin@hotmail.com"},
 ]
 description = "Effortless just-in-time compilation of Python functions, powered by Cython"
 readme = "README.md"
 requires-python = ">= 3.9"
 dependencies = [
```

