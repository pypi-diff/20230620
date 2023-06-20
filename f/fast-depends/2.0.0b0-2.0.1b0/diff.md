# Comparing `tmp/fast_depends-2.0.0b0.tar.gz` & `tmp/fast_depends-2.0.1b0.tar.gz`

## Comparing `fast_depends-2.0.0b0.tar` & `fast_depends-2.0.1b0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/_compat.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/types.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/use.py
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/core/__init__.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/core/build.py
--rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/core/model.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/dependencies/__init__.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/dependencies/model.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/dependencies/provider.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/LICENSE
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/README.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/pyproject.toml
--rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 fast_depends-2.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/_compat.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/types.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/use.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/core/__init__.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/core/build.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/core/model.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/dependencies/__init__.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/dependencies/model.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/dependencies/provider.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/LICENSE
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/README.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 fast_depends-2.0.1b0/PKG-INFO
```

### Comparing `fast_depends-2.0.0b0/CONTRIBUTING.md` & `fast_depends-2.0.1b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.0b0/.github/workflows/documentation.yml` & `fast_depends-2.0.1b0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.0b0/.github/workflows/publish_coverage.yml` & `fast_depends-2.0.1b0/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.0b0/.github/workflows/publish_pypi.yml` & `fast_depends-2.0.1b0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.0b0/.github/workflows/tests.yml` & `fast_depends-2.0.1b0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.0b0/fast_depends/use.py` & `fast_depends-2.0.1b0/fast_depends/use.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from contextlib import AsyncExitStack, ExitStack
 from functools import wraps
 from typing import Any, Awaitable, Callable, Optional, Union
 
 from typing_extensions import ParamSpec, TypeVar
+
 from fast_depends.core import CallModel, build_call_model
 from fast_depends.dependencies import dependency_provider, model
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
@@ -16,50 +17,74 @@
     use_cache: bool = True,
     cast: bool = True,
 ) -> Any:  # noqa: N802
     return model.Depends(call=dependency, use_cache=use_cache, cast=cast)
 
 
 def inject(
-    func: Union[Callable[P, T], Callable[P, Awaitable[T]]],
+    func: Optional[Union[Callable[P, T], Callable[P, Awaitable[T]]]] = None,
     *,
     dependency_overrides_provider: Optional[Any] = dependency_provider,
     wrap_dependant: Callable[[CallModel], CallModel] = lambda x: x,
 ) -> Union[Callable[P, T], Callable[P, Awaitable[T]]]:
-    model = wrap_dependant(build_call_model(func))
+    decorator = _wrap_inject(
+        dependency_overrides_provider=dependency_overrides_provider,
+        wrap_dependant=wrap_dependant,
+    )
+
+    if func is None:
+        return decorator
+
+    else:
+        return decorator(func)
 
+
+def _wrap_inject(
+    dependency_overrides_provider: Optional[Any],
+    wrap_dependant: Callable[[CallModel], CallModel],
+) -> Callable[
+    [Union[Callable[P, T], Callable[P, Awaitable[T]]]],
+    Union[Callable[P, T], Callable[P, Awaitable[T]]],
+]:
     if (
         dependency_overrides_provider
         and getattr(dependency_overrides_provider, "dependency_overrides", None)
         is not None
     ):
         overrides = dependency_overrides_provider.dependency_overrides
     else:
         overrides = None
 
-    if model.is_async:
-
-        @wraps(func)
-        async def call_func(*args: P.args, **kwargs: P.kwargs) -> T:
-            async with AsyncExitStack() as stack:
-                return await model.asolve(
-                    *args,
-                    stack=stack,
-                    dependency_overrides=overrides,
-                    cache_dependencies={},
-                    **kwargs,
-                )
-
-    else:
+    def func_wrapper(
+        func: Union[Callable[P, T], Callable[P, Awaitable[T]]]
+    ) -> Union[Callable[P, T], Callable[P, Awaitable[T]]]:
+        model = wrap_dependant(build_call_model(func))
+
+        if model.is_async:
+
+            @wraps(func)
+            async def injected_wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
+                async with AsyncExitStack() as stack:
+                    return await model.asolve(
+                        *args,
+                        stack=stack,
+                        dependency_overrides=overrides,
+                        cache_dependencies={},
+                        **kwargs,
+                    )
+
+        else:
+
+            @wraps(func)
+            def injected_wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
+                with ExitStack() as stack:
+                    return model.solve(
+                        *args,
+                        stack=stack,
+                        dependency_overrides=overrides,
+                        cache_dependencies={},
+                        **kwargs,
+                    )
 
-        @wraps(func)
-        def call_func(*args: P.args, **kwargs: P.kwargs) -> T:
-            with ExitStack() as stack:
-                return model.solve(
-                    *args,
-                    stack=stack,
-                    dependency_overrides=overrides,
-                    cache_dependencies={},
-                    **kwargs,
-                )
+        return wraps(func)(injected_wrapper)
 
-    return wraps(func)(call_func)
+    return func_wrapper
```

### Comparing `fast_depends-2.0.0b0/fast_depends/utils.py` & `fast_depends-2.0.1b0/fast_depends/utils.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.0b0/fast_depends/core/build.py` & `fast_depends-2.0.1b0/fast_depends/core/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
         elif default is inspect._empty:
             class_fields[param.name] = (annotation, ...)
 
         else:
             class_fields[param.name] = (annotation, default)
 
-    if return_annotation is not inspect._empty:
+    if cast and return_annotation is not inspect._empty:
         response_model = create_model(
             "ResponseModel", response=(return_annotation, ...)
         )
     else:
         response_model = None
 
     func_model = create_model(name, **class_fields)
```

### Comparing `fast_depends-2.0.0b0/fast_depends/core/model.py` & `fast_depends-2.0.1b0/fast_depends/core/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         self.response_model = response_model
 
         self.arguments = []
         self.alias_arguments = []
 
         if PYDANTIC_V2:
             fields = self.model.model_fields
-        else:
+        else:  # pragma: no cover
             fields = self.model.__fields__
 
         for name, f in fields.items():
             self.arguments.append(name)
             self.alias_arguments.append(f.alias or name)
 
         self.dependencies = dependencies or {}
```

### Comparing `fast_depends-2.0.0b0/fast_depends/dependencies/model.py` & `fast_depends-2.0.1b0/fast_depends/dependencies/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.0b0/fast_depends/library/model.py` & `fast_depends-2.0.1b0/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.0b0/LICENSE` & `fast_depends-2.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.0b0/README.md` & `fast_depends-2.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.0b0/pyproject.toml` & `fast_depends-2.0.1b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.0b0/PKG-INFO` & `fast_depends-2.0.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 2.0.0b0
+Version: 2.0.1b0
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

