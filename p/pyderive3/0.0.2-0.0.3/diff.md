# Comparing `tmp/pyderive3-0.0.2.tar.gz` & `tmp/pyderive3-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyderive3-0.0.2.tar", last modified: Fri May 26 22:06:24 2023, max compression
+gzip compressed data, was "pyderive3-0.0.3.tar", last modified: Tue Jun 20 16:47:30 2023, max compression
```

## Comparing `pyderive3-0.0.2.tar` & `pyderive3-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-26 22:06:24.262397 pyderive3-0.0.2/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2320 2023-05-26 22:06:24.262397 pyderive3-0.0.2/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1895 2023-05-25 03:21:30.000000 pyderive3-0.0.2/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-26 22:06:24.258397 pyderive3-0.0.2/pyderive/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1118 2023-05-25 02:50:26.000000 pyderive3-0.0.2/pyderive/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3212 2023-05-25 07:08:25.000000 pyderive3-0.0.2/pyderive/abc.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     9862 2023-05-26 22:02:21.000000 pyderive3-0.0.2/pyderive/compile.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     8833 2023-05-25 23:25:33.000000 pyderive3-0.0.2/pyderive/dataclass.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5284 2023-05-26 21:59:25.000000 pyderive3-0.0.2/pyderive/parse.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-26 22:06:24.262397 pyderive3-0.0.2/pyderive3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2320 2023-05-26 22:06:24.000000 pyderive3-0.0.2/pyderive3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      279 2023-05-26 22:06:24.000000 pyderive3-0.0.2/pyderive3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-05-26 22:06:24.000000 pyderive3-0.0.2/pyderive3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       18 2023-05-26 22:06:24.000000 pyderive3-0.0.2/pyderive3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        9 2023-05-26 22:06:24.000000 pyderive3-0.0.2/pyderive3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-05-26 22:06:24.262397 pyderive3-0.0.2/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      708 2023-05-25 07:09:26.000000 pyderive3-0.0.2/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-20 16:47:30.588375 pyderive3-0.0.3/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2816 2023-06-20 16:47:30.588375 pyderive3-0.0.3/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2391 2023-06-20 16:45:30.000000 pyderive3-0.0.3/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-20 16:47:30.588375 pyderive3-0.0.3/pyderive/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1091 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3212 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/abc.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2980 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/compat.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    10059 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/compile.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    11349 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/dataclasses.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5695 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/parse.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-20 16:47:30.588375 pyderive3-0.0.3/pyderive/tests/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      119 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/tests/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2642 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/tests/dataclasses.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-20 16:47:30.588375 pyderive3-0.0.3/pyderive3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2816 2023-06-20 16:47:30.000000 pyderive3-0.0.3/pyderive3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      357 2023-06-20 16:47:30.000000 pyderive3-0.0.3/pyderive3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-06-20 16:47:30.000000 pyderive3-0.0.3/pyderive3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       18 2023-06-20 16:47:30.000000 pyderive3-0.0.3/pyderive3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        9 2023-06-20 16:47:30.000000 pyderive3-0.0.3/pyderive3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-06-20 16:47:30.588375 pyderive3-0.0.3/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      708 2023-06-20 16:45:55.000000 pyderive3-0.0.3/setup.py
```

### Comparing `pyderive3-0.0.2/PKG-INFO` & `pyderive3-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyderive3
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python3 Custom Data Class Helpers
 Home-page: https://github.com/imgurbot12/pyderive
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -84,14 +84,49 @@
 foo = Foo(1, 'boo')
 print(foo)
 
 for f in fields(foo):
     print(f.name, f.custom_attr)
 ```
 
+###### Backwards Compatibility
+```python
+import pyderive
+import dataclasses
+
+@dataclasses.dataclass
+class Foo:
+    a: int
+    b: int = dataclasses.field(repr=False)
+
+@pyderive.dataclass
+class Bar(Foo):
+    c: int = pyderive.field(frozen=True)
+
+f = Bar(1, 2, 3)
+print(f)
+```
+
+###### Monkey Patching
+
+```python
+from pyderive import compat
+compat.monkey_patch()
+
+from dataclasses import dataclass, field
+
+@dataclass
+class Foo:
+    a: int
+    b: int = field(frozen=True)
+
+f = Foo(1, 2)
+print(f)
+```
+
 ##### Low Level Dataclass Compilation Tools
 
 ```python
 from pyderive import *
 
 class Foo:
     foo: int
```

### Comparing `pyderive3-0.0.2/README.md` & `pyderive3-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -70,14 +70,49 @@
 foo = Foo(1, 'boo')
 print(foo)
 
 for f in fields(foo):
     print(f.name, f.custom_attr)
 ```
 
+###### Backwards Compatibility
+```python
+import pyderive
+import dataclasses
+
+@dataclasses.dataclass
+class Foo:
+    a: int
+    b: int = dataclasses.field(repr=False)
+
+@pyderive.dataclass
+class Bar(Foo):
+    c: int = pyderive.field(frozen=True)
+
+f = Bar(1, 2, 3)
+print(f)
+```
+
+###### Monkey Patching
+
+```python
+from pyderive import compat
+compat.monkey_patch()
+
+from dataclasses import dataclass, field
+
+@dataclass
+class Foo:
+    a: int
+    b: int = field(frozen=True)
+
+f = Foo(1, 2)
+print(f)
+```
+
 ##### Low Level Dataclass Compilation Tools
 
 ```python
 from pyderive import *
 
 class Foo:
     foo: int
```

### Comparing `pyderive3-0.0.2/pyderive/__init__.py` & `pyderive3-0.0.3/pyderive/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 Custom DataClass Compilation Helpers
 """
 from typing import Type, Any
 
 from .abc import *
 from .parse import *
 from .compile import *
-from .dataclass import *
+from .dataclasses import *
+from . import compat
 
 #** Variables **#
 __all__ = [
+    'compat',
+
+    'MISSING',
     'InitVar',
     'FrozenInstanceError',
     'Fields',
     'DefaultFactory',
     'FieldType',
     'FieldDef',
     'Field',
@@ -36,19 +40,14 @@
     'field',
     'fields',
     'asdict',
     'dataclass',
     'DataClassLike',
 
     'BaseField',
- 
-    # compat exports
-    'InitVar',
-    'MISSING',
-    'FrozenInstanceError',
 ]
 
 #** Classes **#
 
 @dataclass(recurse=True)
 class BaseField(FieldDef):
     """dataclass field instance w/ better defaults"""
```

### Comparing `pyderive3-0.0.2/pyderive/abc.py` & `pyderive3-0.0.3/pyderive/abc.py`

 * *Files identical despite different names*

### Comparing `pyderive3-0.0.2/pyderive/compile.py` & `pyderive3-0.0.3/pyderive/compile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 DataClass Compiler Utilities
 """
 from reprlib import recursive_repr
 from types import FunctionType
-from typing import Type, List, Optional, Any, Callable, Dict
+from typing import Iterator, Type, List, Optional, Any, Callable, Dict
 
 from .abc import *
 
 #** Variables **#
 __all__ = [
     'POST_INIT',
     'HDF',
@@ -112,48 +112,53 @@
     locals:  Dict[str, Any] = {}
     globals: Dict[str, Any] = {HDF_VAR: HDF}
     args, post, body, kwonly = ['self'], [], [], []
     for field in fields:
         # build parameter code
         name  = field.name
         param = _init_param(field)
-        if field.field_type == FieldType.INIT_VAR:
-            if field.default_factory is not MISSING:
-                raise TypeError(
-                    f'init field {name!r} cannot have a default factory')
-            post.append(name)
+        value = _init_value(field, globals)
         if field.init:
             if kw_only or field.kw_only:
                 kwonly.append(param)
             else:
                 args.append(param)
+        if field.field_type == FieldType.INIT_VAR:
+            if field.default_factory is not MISSING:
+                raise TypeError(
+                    f'init field {name!r} cannot have a default factory')
+            post.append(name)
+            continue
         # build body code
-        value  = _init_value(field, globals)
         assign = _init_assign(self_name, name, value, frozen or field.frozen)
         body.append(assign)
     # ensure body exists
-    if post_init or post:
+    if post_init:
         params = ', '.join(post)
         body.append(f'self.{POST_INIT}({params})')
     if not body:
         body.append('pass')
     # generate function args/kwargs
     if kwonly:
         args.append('*')
         args.extend(kwonly)
     return _create_fn('__init__', args, body, locals, globals)
 
+def _stdfields(fields: Fields) -> Iterator[FieldDef]:
+    """retrieve only standard fields from fields-list"""
+    return (f for f in fields if f.field_type == FieldType.STANDARD)
+
 def create_repr(fields: Fields) -> Callable:
     """
     generate simple repr-function for the following field-structure
 
     :param fields: ordered field used to generate repr-func
     :param return: repr-function
     """
-    names = [f.name for f in fields if f.repr] 
+    names = [f.name for f in _stdfields(fields) if f.repr]
     body  = 'return self.__class__.__qualname__ + f"(' + \
         ', '.join(f'{name}={{self.{name}!r}}' for name in names) + ')"'
     func = _create_fn('__repr__', ['self'], [body])
     return recursive_repr('...')(func)
 
 def _tuple_str(params: List[str], prefix: Optional[str] = None) -> str:
     """generate tuple string for the given params"""
@@ -167,15 +172,15 @@
     generate compare function w/ the following function name/operation
 
     :param fields: ordered fields used to generate compare-func
     :param func:   function name string
     :param op:     function compare operation
     :return:       compare-function
     """
-    names  = [f.name for f in fields if f.compare]
+    names  = [f.name for f in _stdfields(fields) if f.compare]
     self_t  = _tuple_str(names, 'self') 
     other_t = _tuple_str(names, 'other')  
     return _create_fn(func, ['self', 'other'], [
          'if other.__class__ is self.__class__:',
         f' return {self_t} {op} {other_t}',
          'raise NotImplemented',
     ])
@@ -183,15 +188,15 @@
 def create_hash(fields: Fields) -> Callable:
     """
     generate hash-function for hashable fields
 
     :param fields: ordered fields used to generate hash-function
     :return:       hash-function
     """
-    names   = [f.name for f in fields if f.hash]
+    names   = [f.name for f in _stdfields(fields) if f.hash]
     names_t = _tuple_str(names, 'self')
     return _create_fn('__hash__', ['self'], [f'return hash({names_t})'])
 
 def assign_func(cls: Type, func: Callable, 
     name: Optional[str] = None, overwrite: bool = False) -> bool:
     """
     assign function to the object and modify qualname
@@ -211,17 +216,18 @@
     return False
 
 def add_slots(cls: Type, fields: Fields, frozen: bool = False) -> Type:
     """
     generate slots for fields connected to the given class object
 
     :param cls:    class-object to assign slots onto
-    :param struct: field structure to control slot definition
+    :param fields: field structure to control slot definition
     :return:       updated class object
     """
+    fields   = list(_stdfields(fields))
     cls_dict = dict(cls.__dict__)
     if '__slots__' in cls_dict:
         raise TypeError(f'{cls.__name__} already specifies __slots__')
     # ensure slots don't overlap with bases-classes and assign to dict
     slots      = [f.name for f in fields]
     bases      = cls.__mro__[1:-1]
     base_slots = {s for b in bases for s in getattr(b, '__slots__', [])}
@@ -245,28 +251,24 @@
             f'for name, value in zip({names_t}, state):',
             f' object.__setattr__(self, name, value)'
         ])
         assign_func(cls, getstate)
         assign_func(cls, setstate)
     return cls
 
-def freeze_fields(cls: Type, struct: FlatStruct, frozen: bool = False):
+def freeze_fields(cls: Type, fields: Fields, frozen: bool = False):
     """
     add custom __setattr__/__delattr__ funcs to prevent field modification
 
     :param cls:    class object to assign functions to
-    :param struct: field structure to control frozen status
+    :param fields: field structure to control frozen status
     :param frozen: override field frozen status
     """
-    fields = []
-    for name in struct.order:
-        field = struct.fields[name]
-        if frozen or field.frozen:
-            fields.append(repr(name))
-    names   = _tuple_str(fields)
+    fnames = [repr(f.name) for f in _stdfields(fields) if frozen or f.frozen]
+    names   = _tuple_str(fnames)
     globals = {'cls': cls, 'FrozenInstanceError': FrozenInstanceError}
     ifstmt  = f'if name in {names}:'
     setattr = _create_fn('__setattr__', ['self', 'name', 'value'], [
         ifstmt,
         ' raise FrozenInstanceError(f"cannot assign to field {name!r}")',
         'super(cls, self).__setattr__(name, value)'
     ], globals=globals)
```

### Comparing `pyderive3-0.0.2/pyderive/dataclass.py` & `pyderive3-0.0.3/pyderive/dataclasses.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,31 +5,36 @@
 import copy
 from typing import * 
 from typing_extensions import dataclass_transform, runtime_checkable
 
 from .abc import *
 from .parse import *
 from .compile import *
+from .compat import is_stddataclass, convert_params
 
 #** Variables **#
 __all__ = [
     'InitVar', 
     'MISSING', 
     'DataClassLike',
+    'FrozenInstanceError',
  
     'is_dataclass',
     'field', 
     'fields',
     'asdict',
     'dataclass'
 ]
 
 #: dataclass fields attribute
 FIELD_ATTR = '__datafields__'
 
+#: dataclas params attribute
+PARAMS_ATTR = '__dataparams__'
+
 #: field generic type
 F = TypeVar('F', bound=FieldDef)
 
 #: type for type-alias
 TypeT = Type[T]
 
 #: typehint for dataclass creator function
@@ -58,19 +63,14 @@
     (True,  False, True,  True ): _hash_err,
     (True,  True,  False, False): _hash_add,
     (True,  True,  False, True ): _hash_err,
     (True,  True,  True,  False): _hash_add,
     (True,  True,  True,  True ): _hash_err,
 }
 
-@runtime_checkable
-class DataClassLike(Generic[F], Protocol):
-    """Protocol for DataClass-Like Objects"""
-    __datafields__: List[F]
-
 #** Functions **#
 
 def field(*_, **kwargs) -> Any:
     """
     specify field configurations for a dataclass attribute
     """
     return Field('', MISSING, **kwargs)
@@ -81,31 +81,35 @@
 
     :param cls: object-type/instance to check
     :return:    true if object is a dataclass
     """
     return hasattr(cls, FIELD_ATTR)
 
 @overload
-def fields(cls: Any) -> List[FieldDef]:
+def fields(cls: Any, all_types: bool = False) -> List[FieldDef]:
     ...
 
 @overload
-def fields(cls: DataClassLike[F]) -> List[F]:
+def fields(cls: 'DataClassLike[F]', all_types: bool = False) -> List[F]:
     ...
 
-def fields(cls: Union[DataClassLike[F], Any]) -> Union[List[F], List[FieldDef]]:
+def fields(cls, all_types: bool = False):
     """
     retrieve fields associated w/ the given dataclass
 
-    :param cls: dataclass object class instance
-    :return:    field dictionary
+    :param cls:       dataclass object class instance
+    :param all_types: return all field-types or just standard fields
+    :return:          field dictionary
     """
     if not is_dataclass(cls):
         raise TypeError('fields() should with a dataclass type or instance')
-    return getattr(cls, FIELD_ATTR)
+    fields = getattr(cls, FIELD_ATTR)
+    if not all_types:
+        fields = [f for f in fields if f.field_type == FieldType.STANDARD]
+    return fields
 
 def _asdict_inner(obj, rec: int, factory: Type[dict], lvl: int):
     """inner dictionary-ify function to convert dataclass fields into dict"""
     # stop recursin after limit
     if rec > 0 and lvl >= rec:
         return obj
     # dataclass
@@ -155,20 +159,42 @@
     slots:       bool = False,
     recurse:     bool = False,
     field:       Type[FieldDef] = Field,
 ) -> TypeT:
     # valdiate settings
     if order and not eq:
         raise ValueError('eq must be true if order is true')
+    # convert params for stdlib dataclasses
+    isdataclass = is_dataclass(cls)
+    if not isdataclass and is_stddataclass(cls):
+        convert_params(cls)
     # parse and conregate fields
     struct = parse_fields(cls, factory=field, recurse=recurse)
     fields = flatten_fields(struct)
     freeze = frozen or any(f.frozen for f in fields)
+    # validate settings and save fields/params
+    params = DataParams(init, repr, eq, order, unsafe_hash, 
+        frozen, match_args, kw_only, slots, recurse, field)
+    if isdataclass:
+        ofields = getattr(cls, FIELD_ATTR)
+        oparams = getattr(cls, PARAMS_ATTR)
+        # ensure there are no frozen conflicts
+        if frozen and not (oparams.frozen or all(f.frozen for f in ofields)):
+            raise TypeError(
+                'cannot inherit frozen dataclass from a non-frozen one')
+        if not frozen and (oparams.frozen or any(f.frozen for f in ofields)):
+            raise TypeError(
+                'cannot inherit non-frozen dataclass from a frozen one')
+    # ensure slots dont conflict with partially frozen dataclasses
+    if slots and not frozen and any(f.frozen for f in fields):
+        raise TypeError(
+            'cannot assign slots for partially frozen dataclass')
     # assign fields to dataclass
     setattr(cls, FIELD_ATTR, fields)
+    setattr(cls, PARAMS_ATTR, params)
     # build functions
     if init or init is None:
         overwrite = init is True
         post_init = hasattr(cls, POST_INIT)
         initfunc  = create_init(fields, kw_only, post_init, frozen)
         assign_func(cls, initfunc, overwrite=overwrite)
     if repr or repr is None:
@@ -182,15 +208,15 @@
             fname = f'__{name}__'
             func  = create_compare(fields, fname, op)
             if assign_func(cls, func):
                 raise TypeError(f'Cannot override attibute {fname} '
                                 f'in class {cls.__name__}. Consider '
                                 'using functools.total_ordering')
     if freeze:
-        freeze_fields(cls, struct, frozen)
+        freeze_fields(cls, fields, frozen)
     # build hash function based on current state
     class_dict  = cls.__dict__
     class_eq    = class_dict.get('__eq__', None)
     class_hash  = class_dict.get('__hash__', MISSING)
     explicit    = not (class_hash in (MISSING, None) and class_eq)
     hash_args   = (bool(unsafe_hash), bool(eq), bool(frozen), explicit)
     hash_action = HASH_ACTIONS[hash_args]
@@ -259,7 +285,54 @@
     :param field:       field-factory baseclass
     :return:            dataclass type object
     """
     @dataclass_transform(field_specifiers=(FieldDef, Field, field))
     def wrapper(cls: TypeT) -> TypeT:
         return _process_class(cls, **kw)
     return wrapper if cls is None else wrapper(cls)
+
+#** Classes **#
+
+@runtime_checkable
+class DataClassLike(Generic[F], Protocol):
+    """Protocol for DataClass-Like Objects"""
+    __datafields__: List[F]
+
+class DataParams:
+    """Pseudo Dataclass to store parameters used to generate dataclass"""
+    __slots__ = (
+        'init', 
+        'repr',
+        'eq', 
+        'order', 
+        'unsafe_hash', 
+        'frozen', 
+        'match_args', 
+        'kw_only', 
+        'slots', 
+        'recurse', 
+        'field')
+
+    def __init__(self,
+        init:        Optional[bool],
+        repr:        Optional[bool],
+        eq:          bool,
+        order:       bool,
+        unsafe_hash: bool,
+        frozen:      bool,
+        match_args:  bool,
+        kw_only:     bool,
+        slots:       bool,
+        recurse:     bool,
+        field:       Type[FieldDef],
+    ):
+        self.init        = init
+        self.repr        = repr
+        self.eq          = eq
+        self.order       = order
+        self.unsafe_hash = unsafe_hash
+        self.frozen      = frozen
+        self.match_args  = match_args
+        self.kw_only     = kw_only
+        self.slots       = slots
+        self.recurse     = recurse
+        self.field       = field
```

### Comparing `pyderive3-0.0.2/pyderive/parse.py` & `pyderive3-0.0.3/pyderive/parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 DataClass Parsing Tools
 """
 from typing import Type, Optional, ClassVar, get_origin
 
 from .abc import *
+from .compat import is_stddataclass, convert_fields
 
 #** Variables **#
 __all__ = [
     'DERIVE_ATTR',
 
     'remove_field',
     'parse_fields',
@@ -59,27 +60,32 @@
         base = bases.pop()
         if base is object:
             continue
         # skip if recursive and already compiled
         if recurse and hash(base) in COMPILED:
             continue
         COMPILED.add(hash(base))
+        # convert stdlib dataclass fields to valid class-struct
+        parent = getattr(base, DERIVE_ATTR, None)
+        if parent is None and is_stddataclass(base):
+            fields = convert_fields(base, ftype)
+            names  = [f.name for f in fields]
+            parent = ClassStruct(names, {f.name:f for f in fields})
         # process fields
-        parent      = getattr(base, DERIVE_ATTR, None)
         fields      = ClassStruct(parent=parent)
         annotations = getattr(base, '__annotations__', {})
         for name, anno in annotations.items():
-            # retrieve default-value of variable (if exists)
-            default = getattr(base, name, MISSING)
-            if delete and hasattr(base, name):
-                delattr(base, name)
             # handle ClassVar
             if get_origin(anno) is ClassVar:
                 remove_field(fields, name)
                 continue
+            # retrieve default-value of variable (if exists)
+            default = getattr(base, name, MISSING)
+            if delete and hasattr(base, name):
+                delattr(base, name)
             # preserve order of fields and add vardef
             if name not in fields.order:
                 fields.order.append(name)
             # assign field based on value
             if isinstance(default, ftype):
                 field      = default
                 field.name = name
@@ -125,21 +131,24 @@
     # order heigharchy from farthest-parent to class-itself
     heigharchy = [fields]
     while fields.parent:
         fields = fields.parent
         heigharchy.insert(0, fields)
     # sort fields
     struct = FlatStruct()
-    kwargs = False # track when kwargs have been spotted
+    kwargs = set() # track when kwargs have been spotted
     for fields in heigharchy:
         for name in fields.order:
             field   = fields.fields[name]
             default = has_default(field)
-            kwargs  = kwargs or (default and field.init and not field.kw_only)
             missing = name not in struct.fields
+            if default and field.init and not field.kw_only:
+                kwargs.add(name)
+            elif name in kwargs:
+                kwargs.remove(name)
             # raise error if non-kwarg found after kwargs start
             if order_kw and kwargs and missing and not default:
                 raise TypeError(
                     f'non-default argument {name!r} follows default argument')
             # append vardef to order and set/replace definition
             if missing:
                 struct.order.append(name)
```

### Comparing `pyderive3-0.0.2/pyderive3.egg-info/PKG-INFO` & `pyderive3-0.0.3/pyderive3.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyderive3
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python3 Custom Data Class Helpers
 Home-page: https://github.com/imgurbot12/pyderive
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -84,14 +84,49 @@
 foo = Foo(1, 'boo')
 print(foo)
 
 for f in fields(foo):
     print(f.name, f.custom_attr)
 ```
 
+###### Backwards Compatibility
+```python
+import pyderive
+import dataclasses
+
+@dataclasses.dataclass
+class Foo:
+    a: int
+    b: int = dataclasses.field(repr=False)
+
+@pyderive.dataclass
+class Bar(Foo):
+    c: int = pyderive.field(frozen=True)
+
+f = Bar(1, 2, 3)
+print(f)
+```
+
+###### Monkey Patching
+
+```python
+from pyderive import compat
+compat.monkey_patch()
+
+from dataclasses import dataclass, field
+
+@dataclass
+class Foo:
+    a: int
+    b: int = field(frozen=True)
+
+f = Foo(1, 2)
+print(f)
+```
+
 ##### Low Level Dataclass Compilation Tools
 
 ```python
 from pyderive import *
 
 class Foo:
     foo: int
```

### Comparing `pyderive3-0.0.2/setup.py` & `pyderive3-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pyderive3',
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pyderive',
     description="Python3 Custom Data Class Helpers",
     long_description=readme,
     long_description_content_type="text/markdown",
```

