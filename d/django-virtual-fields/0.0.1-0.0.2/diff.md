# Comparing `tmp/django_virtual_fields-0.0.1.tar.gz` & `tmp/django_virtual_fields-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_virtual_fields-0.0.1.tar", max compression
+gzip compressed data, was "django_virtual_fields-0.0.2.tar", max compression
```

## Comparing `django_virtual_fields-0.0.1.tar` & `django_virtual_fields-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1981 2023-06-12 01:48:08.660253 django_virtual_fields-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      106 2023-06-12 01:48:08.664253 django_virtual_fields-0.0.1/virtual_fields/__init__.py
--rw-r--r--   0        0        0      160 2023-06-12 01:48:08.664253 django_virtual_fields-0.0.1/virtual_fields/__init__.pyi
--rw-r--r--   0        0        0     3851 2023-06-12 01:48:08.664253 django_virtual_fields-0.0.1/virtual_fields/_compat.py
--rw-r--r--   0        0        0      102 2023-06-12 01:48:08.664253 django_virtual_fields-0.0.1/virtual_fields/apps.py
--rw-r--r--   0        0        0    16031 2023-06-12 01:48:08.664253 django_virtual_fields-0.0.1/virtual_fields/fields.py
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 django_virtual_fields-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2002 2023-06-20 05:53:46.410532 django_virtual_fields-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-06-20 05:53:46.410532 django_virtual_fields-0.0.2/virtual_fields/__init__.py
+-rw-r--r--   0        0        0      160 2023-06-20 05:53:46.410532 django_virtual_fields-0.0.2/virtual_fields/__init__.pyi
+-rw-r--r--   0        0        0     5936 2023-06-20 05:53:46.410532 django_virtual_fields-0.0.2/virtual_fields/_compat.py
+-rw-r--r--   0        0        0      662 2023-06-20 05:53:46.410532 django_virtual_fields-0.0.2/virtual_fields/_util.py
+-rw-r--r--   0        0        0      102 2023-06-20 05:53:46.410532 django_virtual_fields-0.0.2/virtual_fields/apps.py
+-rw-r--r--   0        0        0    16564 2023-06-20 05:53:46.410532 django_virtual_fields-0.0.2/virtual_fields/fields.py
+-rw-r--r--   0        0        0     5900 2023-06-20 05:53:46.410532 django_virtual_fields-0.0.2/virtual_fields/models.py
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 django_virtual_fields-0.0.2/PKG-INFO
```

### Comparing `django_virtual_fields-0.0.1/pyproject.toml` & `django_virtual_fields-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Django-Virtual-Fields"
-version = "0.0.1"
+version = "0.0.2"
 description = "Virtual `django` fields."
 authors = ["David Kyalo <davidmkyalo@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
@@ -34,14 +34,15 @@
 black = "*"
 ipython = "^8.10.0"
 django-polymorphic = "^3.1.0"
 tox = "^4.4.8"
 psycopg = "^3.1.8"
 mysqlclient = "^2.1.1"
 django-debug-toolbar = "^4.1.0"
+devtools = "^0.11.0"
 
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
```

### Comparing `django_virtual_fields-0.0.1/virtual_fields/fields.py` & `django_virtual_fields-0.0.2/virtual_fields/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import inspect
 from collections import abc
+from enum import Enum
 from functools import reduce
 from logging import getLogger
 from operator import methodcaller, or_
 from threading import RLock
-from types import new_class
+from types import GenericAlias, new_class
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Final,
     Generic,
     NamedTuple,
@@ -25,91 +27,74 @@
     Combinable,
     Expression,
     ExpressionWrapper,
     F,
     Value,
 )
 from django.db.models.functions import Cast, Coalesce
+from django.db.models.query_utils import PathInfo
+from django.db.models.sql.compiler import SQLCompiler
+from django.db.models.sql.query import Query
 from django.dispatch import receiver
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 from typing_extensions import Self
 
+from ._compat import add_virtual_field_support
+from ._util import _db_instance_qs
+
 if TYPE_CHECKING:
-    from ._compat import Model
+    from .models import VirtualizedModel
 
 __all__ = [
     "VirtualField",
 ]
 
 _T_Field = TypeVar("_T_Field", bound=m.Field, covariant=True)
 _T_Model = TypeVar("_T_Model", bound="Model", covariant=True)
 _T_Expr = TypeVar("_T_Expr", Combinable, m.Q)
 _T_Fn = abc.Callable[..., Any]
 
 logger = getLogger(__name__)
 
-_virtual_field_models = set()
 
 DEFERRED = models_mod.DEFERRED
 
 
-def _add_virtual_field_support(model: type[_T_Model]):
-    if not (model in _virtual_field_models or model._meta.abstract):
-        _virtual_field_models.add(model)
-        m.signals.post_save.connect(_post_save_receiver, model, weak=False)
-
-    return model
-
-
-@receiver(m.signals.class_prepared, weak=False)
-def __on_class_prepared(sender: type[_T_Model], **kwds):
-    if sender not in _virtual_field_models:
-        bases = {*sender.__mro__[1:-1]}
-        (bases & _virtual_field_models) and _add_virtual_field_support(sender)
-
-
-def _post_save_receiver(sender, instance: _T_Model, **kwargs):
-    dct = instance.__dict__
-    for n, f in instance.__class__._meta.cached_virtual_fields.items():
-        if (at := f.attname) in dct:
-            delattr(instance, at)
-
-
 def _attrsetter_decorator(name: str, typ: type = Any, *, call=False):
     def decorator(self, val: typ = None):
         def setter(v):
             getattr(self, name)(v) if call else setattr(self, name, v)
 
         return setter if val is None else setter(val)
 
     return decorator
 
 
-def _db_instance_qs(obj: _T_Model, using=None, *, filter=True):
-    man = obj.__class__._meta.base_manager
-    qs: m.Manager[_T_Model] = man.db_manager(using, hints={"instance": obj})
-    return qs.all() if filter is False else qs.filter(pk=obj.pk)
-
-
 def coalesced(expr: _T_Expr, /, *exprs: _T_Expr):
     return (
         Coalesce(expr, *exprs)
         if exprs
         else expr
         if isinstance(expr, Expression)
         else ExpressionWrapper(expr, None)
     )
 
 
-class FieldPathInfo(NamedTuple):
-    path: list
+class Behaviour(str, Enum):
+    NOOP = "NOOP"
+    DELETE = "DELETE"
+    RELOAD = "RELOAD"
+
+
+class FieldPath(NamedTuple):
+    info: list[PathInfo]
     field: _T_Field
-    targets: tuple = ()
-    name: tuple[str] = ()
+    targets: tuple[_T_Field, ...] = ()
+    name: list[str] = ()
     src: "VirtualField" = None
 
 
 class VirtualFieldDescriptor:
     field: "VirtualField"
     cache: bool = None
     func: _T_Fn = None
@@ -163,18 +148,24 @@
     def get_default(self):
         ...
 
     get_default = None
 
 
 class VirtualField(m.Field, Generic[_T_Field]):
+    vars().update(Behaviour.__members__)
+    if TYPE_CHECKING:
+        NOOP: Final[Behaviour] = ...
+        DELETE: Final[Behaviour] = ...
+        RELOAD: Final[Behaviour] = ...
+
     description = _("A virtual field. Uses query annotations to return computed value.")
     expressions: m.expressions.Combinable | m.Q | str
     empty_strings_allowed = False
-    defer: bool = False
+    defer: bool = True
     cache: bool | None
     concrete: bool | None
     model: _T_Model
     base_descriptor_class = VirtualFieldDescriptor
     fget: _T_Fn | None
     fset: _T_Fn | None
     fdel: _T_Fn | None
@@ -191,14 +182,15 @@
         },
     }
     _output_type_: Final[type[_T_Field]] = None
     _output_args_: ClassVar = None
     _output_kwargs_: ClassVar = None
     _init_defaults_ = {
         # "null": True,
+        "default": DEFERRED,
         "editable": False,
         "serialize": False,
     }
     _base_field_kwargs_ = (
         "verbose_name",
         "name",
         "primary_key",
@@ -222,47 +214,47 @@
         "validators",
         "error_mess testages",
         "db_comment",
     )
 
     def __class_getitem__(cls, params):
         out: type[_T_Field] = params[0] if isinstance(params, (tuple, list)) else params
-        out, base, final = get_origin(out) or out, cls._output_type_, cls
+        out, base, final = (get_origin(out) or out), cls._output_type_, cls
 
         if base is None and isinstance(out, type) and issubclass(out, m.Field):
             assert base is None or issubclass(
                 out, base
             ), f"must be a subtype of {base.__name__}"
-            cache = cls.__output_typed_
-            if (final := cache.get(out)) is None:
+            cache, ck = cls.__output_typed_, (cls, out)
+            if (final := cache.get(ck)) is None:
                 with cls.__out_lock:
                     if (final := cache.get(out)) is None:
                         name = f"{out.__name__.replace('Field', '')}{cls.__name__}"
                         module, qualname = cls.__module__, f"{cls.__qualname__}.{name}"
                         by_typ = cls._output_types_default_kwargs_
                         kwds = reduce(
                             or_,
                             filter(None, map(by_typ.get, out.__mro__[::-1])),
                             cls._output_kwargs_ or {},
                         )
-                        cache[out] = final = new_class(
+                        cache[ck] = final = new_class(
                             name,
                             (cls[_T_Field],),
                             None,
                             methodcaller(
                                 "update",
                                 {
                                     "__module__": module,
                                     "__qualname__": qualname,
                                     "_output_type_": out,
                                     "_output_field_kwargs_": kwds,
                                 },
                             ),
                         )
-        return super(cls, final).__class_getitem__(params)
+        return GenericAlias(final, params)
 
     def __new__(cls: type[Self], *a, output_field: _T_Field = None, **kw):
         if output_field is not None:
             typ, bound = output_field.__class__, cls._output_type_
             if bound is None:
                 cls = cls[typ]
                 cls = get_origin(cls) or cls
@@ -334,20 +326,42 @@
 
     getter = _attrsetter_decorator("fget", _T_Fn)
     setter = _attrsetter_decorator("fset", _T_Fn)
     deleter = _attrsetter_decorator("fdel", _T_Fn)
     expression = _attrsetter_decorator("set_source_expressions", _T_Fn, call=True)
 
     @cached_property
-    def cache(self):
-        return (None, None, None) == (self.fget, self.fset, self.fdel)
+    def on_model_add(self):
+        return self.on_model_save
 
     @cached_property
-    def defer(self):
-        return self.fget is not None
+    def on_model_save(self):
+        cache, defer, computable = self.cache, self.defer, self.is_computable
+        match (cache, defer, computable or self.has_joins):
+            case (True, _, True):
+                return self.DELETE
+            case (True, True, _):
+                return self.DELETE
+            case (True, False, _):
+                return self.RELOAD
+        return self.NOOP
+
+    @cached_property
+    def on_model_refresh(self):
+        cache, defer, computable = self.cache, self.defer, self.is_computable
+        match (cache, defer, computable):
+            case (True, _, True):
+                return self.DELETE
+            case (True, True, _):
+                return self.DELETE
+        return self.NOOP
+
+    @cached_property
+    def cache(self):
+        return (None, None, None) == (self.fget, self.fset, self.fdel)
 
     @cached_property
     def output_field(self) -> _T_Field:
         return self._output_field or self.source_output_field
 
     @cached_property
     def final_expression(self):
@@ -383,54 +397,69 @@
         return annotation
 
     @cached_property
     def descriptor_class(self):
         fget, fset, fdel = self.get_fget(), self.get_fset(), self.get_fdel()
         return self._define_descriptor_class(fget, fset, fdel, cached=self.cache)
 
+    @cached_property
+    def has_joins(self):
+        for path in filter(None, self._iter_source_field_paths()):
+            if path.info or (path.field and path.field.is_relation):
+                return True
+        return False
+
+    @cached_property
+    def is_computable(self) -> bool:
+        return self.fget is not None
+
     def get_col(self, alias, output_field=None):
+        if not self.has_joins:
+            return self.cached_col
+
+        call = query = this = None
+        try:
+            call = (inspect.stack()[1:2] or (None,))[0]
+            if not (hasattr(call, "frame") and hasattr(call.frame, "f_locals")):
+                pass
+            elif (this := call.frame.f_locals.get("self")) is not None:
+                query = this.query if isinstance(this, SQLCompiler) else this
+                if isinstance(query, Query) and self.name not in query.annotations:
+                    return self.final_expression.resolve_expression(query)
+        finally:
+            del call, query, this
+
         return self.cached_col
 
     def get_internal_type(self):  # pragma: no cover
         return "VirtualField"
 
     def clean(self, value, model_instance):
         return self.output_field.clean(value, model_instance)
 
     def formfield(self, **kwargs):
         return self.output_field.formfield(**kwargs)
 
     def contribute_to_class(self, cls, name, private_only=None):
+        from .models import ImplementsVirtualFields, VirtualizedModel
+
         super().contribute_to_class(cls, name, private_only is not False)
-        _add_virtual_field_support(cls)
-        # self.column or setattr(cls, self.attname, self.descriptor_class(self))
+
+        add_virtual_field_support(cls)
         assert isinstance(getattr(cls, self.attname), self.descriptor_class)
 
     def set_attributes_from_name(self, name):
         super().set_attributes_from_name(name)
         self.concrete = not self.defer
 
-    # def get_db_prep_value(self, *args, **kwds):
-    #     return (self.output_field or super()).get_db_prep_value(*args, **kwds)
-
-    # def get_prep_value(self, value):
-    #     """Perform preliminary non-db specific value checks and conversions."""
-    #     return (self.output_field or super()).get_prep_value(value)
-
-    # def get_attname_column(self):
-    #     """Sets column to `None` for deferred fields to prevent selection."""
-    #     attname, column = super().get_attname_column()
-    #     return attname, None if self.defer else column
-
     def set_source_expressions(self, *expressions):
         self.expressions = expressions
 
     def add_to_query(self, qs: m.QuerySet[_T_Model], alias=None, select=True):
-        name = self.name
-        qs.query.add_annotation(F(name), alias or name, select)
+        qs.query.add_annotation(self.final_expression, alias or self.name, select)
         return qs
 
     def get_queryset_for_object(self, obj: _T_Model):
         return self.add_to_query(_db_instance_qs(obj))
 
     def get_fget(self):
         fget = self.fget
@@ -486,28 +515,23 @@
                 elif hasattr(v, "resolve_expression"):
                     yield v
                 elif isinstance(v, str):
                     yield F(v)
                 else:
                     yield Value(v)
 
-    def __get_flat_source_expressions(self):  # pragma: no cover
-        raw = self.raw_expression
-        return (f if isinstance(f, F) else None for f in raw.flatten())
-
-    def __get_source_fields(
-        self, *, recursive=None, src: "VirtualField" = None
-    ):  # pragma: no cover
+    def _iter_source_field_paths(self, *, recursive=None, src: "VirtualField" = None):
         f: _T_Field | VirtualField
+        raw = self.raw_expression
         opts, qs, deep = self.model._meta, self._queryset, recursive is not False
         to_path = qs.query.names_to_path.__get__(qs.query)
 
-        for expr in filter(None, self.__get_flat_source_expressions()):
-            if expr is None:
+        for expr in raw.flatten():
+            if not isinstance(expr, F):
                 yield None
             else:
                 path = to_path(expr.name.split(LOOKUP_SEP), opts)
-                info = FieldPathInfo(*path, src=src)
-                if deep is True is hasattr(f := info.field, "get_source_fields"):
-                    yield from f.__get_source_fields(recursive=recursive, src=self)
+                info = FieldPath(*path, src=src)
+                if deep is True is hasattr(f := info.field, "_iter_source_field_paths"):
+                    yield from f._iter_source_field_paths(recursive=recursive, src=self)
                 else:
                     yield info
```

### Comparing `django_virtual_fields-0.0.1/PKG-INFO` & `django_virtual_fields-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-virtual-fields
-Version: 0.0.1
+Version: 0.0.2
 Summary: Virtual `django` fields.
 License: MIT
 Author: David Kyalo
 Author-email: davidmkyalo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

