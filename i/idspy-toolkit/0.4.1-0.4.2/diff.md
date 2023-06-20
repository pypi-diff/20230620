# Comparing `tmp/idspy_toolkit-0.4.1.tar.gz` & `tmp/idspy_toolkit-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idspy_toolkit-0.4.1.tar", last modified: Mon Jun 12 10:50:43 2023, max compression
+gzip compressed data, was "idspy_toolkit-0.4.2.tar", last modified: Tue Jun 20 17:10:01 2023, max compression
```

## Comparing `idspy_toolkit-0.4.1.tar` & `idspy_toolkit-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-12 10:50:43.095178 idspy_toolkit-0.4.1/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1599 2023-06-08 14:59:54.000000 idspy_toolkit-0.4.1/LICENSE
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     5436 2023-06-12 10:50:43.082233 idspy_toolkit-0.4.1/PKG-INFO
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2841 2023-06-12 10:46:26.000000 idspy_toolkit-0.4.1/README.rst
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-12 10:50:42.042017 idspy_toolkit-0.4.1/idspy_toolkit/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      611 2023-06-12 09:28:55.000000 idspy_toolkit-0.4.1/idspy_toolkit/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    14707 2023-06-12 09:28:01.000000 idspy_toolkit-0.4.1/idspy_toolkit/accessor.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2182 2023-06-08 14:59:30.000000 idspy_toolkit-0.4.1/idspy_toolkit/constants.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    10769 2023-06-12 09:28:19.000000 idspy_toolkit-0.4.1/idspy_toolkit/converter.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2245 2023-06-12 09:29:10.000000 idspy_toolkit-0.4.1/idspy_toolkit/snippets.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8365 2023-06-12 09:29:21.000000 idspy_toolkit-0.4.1/idspy_toolkit/toolkit.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7094 2023-06-12 09:29:32.000000 idspy_toolkit-0.4.1/idspy_toolkit/utils.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-12 10:50:42.428149 idspy_toolkit-0.4.1/idspy_toolkit.egg-info/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     5436 2023-06-12 10:50:40.000000 idspy_toolkit-0.4.1/idspy_toolkit.egg-info/PKG-INFO
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      548 2023-06-12 10:50:41.000000 idspy_toolkit-0.4.1/idspy_toolkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        1 2023-06-12 10:50:40.000000 idspy_toolkit-0.4.1/idspy_toolkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       65 2023-06-12 10:50:40.000000 idspy_toolkit-0.4.1/idspy_toolkit.egg-info/requires.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       14 2023-06-12 10:50:40.000000 idspy_toolkit-0.4.1/idspy_toolkit.egg-info/top_level.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7857 2023-06-12 09:25:37.000000 idspy_toolkit-0.4.1/pyproject.toml
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       38 2023-06-12 10:50:43.099905 idspy_toolkit-0.4.1/setup.cfg
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       39 2023-06-08 15:03:37.000000 idspy_toolkit-0.4.1/setup.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-12 10:50:42.971318 idspy_toolkit-0.4.1/tests/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     6344 2023-06-12 10:04:40.000000 idspy_toolkit-0.4.1/tests/test_accessor.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     6459 2023-06-12 10:05:13.000000 idspy_toolkit-0.4.1/tests/test_converter_hdf5.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1493 2023-06-08 14:51:39.000000 idspy_toolkit-0.4.1/tests/test_hdf5_io.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2542 2023-06-12 10:05:30.000000 idspy_toolkit-0.4.1/tests/test_ids_browse.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1397 2023-06-08 14:51:40.000000 idspy_toolkit-0.4.1/tests/test_snippets.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2217 2023-06-12 10:05:47.000000 idspy_toolkit-0.4.1/tests/test_utils.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 17:10:00.977416 idspy_toolkit-0.4.2/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1599 2023-06-08 14:59:54.000000 idspy_toolkit-0.4.2/LICENSE
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4711 2023-06-20 17:10:00.963415 idspy_toolkit-0.4.2/PKG-INFO
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2033 2023-06-20 17:09:32.000000 idspy_toolkit-0.4.2/README.rst
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 17:09:59.788453 idspy_toolkit-0.4.2/idspy_toolkit/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      611 2023-06-20 16:49:28.000000 idspy_toolkit-0.4.2/idspy_toolkit/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    15133 2023-06-20 16:42:29.000000 idspy_toolkit-0.4.2/idspy_toolkit/accessor.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2645 2023-06-20 16:42:43.000000 idspy_toolkit-0.4.2/idspy_toolkit/constants.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    10923 2023-06-20 16:47:28.000000 idspy_toolkit-0.4.2/idspy_toolkit/converter.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1997 2023-06-20 16:47:41.000000 idspy_toolkit-0.4.2/idspy_toolkit/snippets.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8357 2023-06-20 16:49:53.000000 idspy_toolkit-0.4.2/idspy_toolkit/toolkit.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8518 2023-06-20 16:50:19.000000 idspy_toolkit-0.4.2/idspy_toolkit/utils.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 17:10:00.246192 idspy_toolkit-0.4.2/idspy_toolkit.egg-info/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4711 2023-06-20 17:09:58.000000 idspy_toolkit-0.4.2/idspy_toolkit.egg-info/PKG-INFO
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      548 2023-06-20 17:09:58.000000 idspy_toolkit-0.4.2/idspy_toolkit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        1 2023-06-20 17:09:58.000000 idspy_toolkit-0.4.2/idspy_toolkit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       69 2023-06-20 17:09:58.000000 idspy_toolkit-0.4.2/idspy_toolkit.egg-info/requires.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       14 2023-06-20 17:09:58.000000 idspy_toolkit-0.4.2/idspy_toolkit.egg-info/top_level.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7906 2023-06-20 16:46:04.000000 idspy_toolkit-0.4.2/pyproject.toml
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       38 2023-06-20 17:10:00.982430 idspy_toolkit-0.4.2/setup.cfg
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       39 2023-06-12 10:54:27.000000 idspy_toolkit-0.4.2/setup.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 17:10:00.844191 idspy_toolkit-0.4.2/tests/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7600 2023-06-20 16:48:35.000000 idspy_toolkit-0.4.2/tests/test_accessor.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     6561 2023-06-20 16:48:49.000000 idspy_toolkit-0.4.2/tests/test_converter_hdf5.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1493 2023-06-08 14:51:39.000000 idspy_toolkit-0.4.2/tests/test_hdf5_io.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2542 2023-06-12 10:05:30.000000 idspy_toolkit-0.4.2/tests/test_ids_browse.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1397 2023-06-08 14:51:40.000000 idspy_toolkit-0.4.2/tests/test_snippets.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4192 2023-06-20 16:45:10.000000 idspy_toolkit-0.4.2/tests/test_utils.py
```

### Comparing `idspy_toolkit-0.4.1/LICENSE` & `idspy_toolkit-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.1/PKG-INFO` & `idspy_toolkit-0.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idspy_toolkit
-Version: 0.4.1
+Version: 0.4.2
 Summary: Tools to manipulate the IDSPy Dictionaries
 Author-email: Guillaume Fuhr <guillaume.fuhr@univ-amu.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CNRS, contributor: Y. Camenen
         Copyright (c) 2023, Aix-Marseille Univ., contributor: G. Fuhr
         All rights reserved.
@@ -38,59 +38,26 @@
 Project-URL: repository, https://gitlab.com/gkdb/imas-gk/-/tree/main/idspy_toolkit
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 IDSPy Toolkit
 =============
 
-Changelog :
-  * v 0.4.1
-
-   - correction of a bug with numpy.array having ndim=0 `#7 <https://gitlab.com/gkdb/imas-gk/-/issues/7>`_
-   - improved error message when trying to reach the root of an IDS using a path as string `#8 <https://gitlab.com/gkdb/imas-gk/-/issues/8>`_
-   - list_ids_members returns only all the ids members and not anymore ids root path also
-   - add possibility to overwrite HDF5 file written
-
-  * v 0.4.0
-
-   - pypi packaging
-   - tests using tox
-   - increase code coverage
-
-  * v 0.3.0
-
-    - GitLab Release
-    - HDF5 interface added
-
-  * v 0.2.1
-
-    - BUG correction on IDS attributes
-    - Numpy.Array Implementation (still work in progress)
-
-  * v 0.2.0
-
-    - Removal of AccessLayer MetaData
-
-  * v 0.1.1
-
-    - First Experimental Release
-
-
-
 This module contains a serie of function to help mange and manipulate IDSPy dataclasses
 
  * fill_missing_values
  * ids_to_hdf5
  * hdf5_to_ids
  * get_ids_value_from_string
  * set_ids_value_from_string
```

### Comparing `idspy_toolkit-0.4.1/README.rst` & `idspy_toolkit-0.4.2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,10 @@
 IDSPy Toolkit
 =============
 
-Changelog :
-  * v 0.4.1
-
-   - correction of a bug with numpy.array having ndim=0 `#7 <https://gitlab.com/gkdb/imas-gk/-/issues/7>`_
-   - improved error message when trying to reach the root of an IDS using a path as string `#8 <https://gitlab.com/gkdb/imas-gk/-/issues/8>`_
-   - list_ids_members returns only all the ids members and not anymore ids root path also
-   - add possibility to overwrite HDF5 file written
-
-  * v 0.4.0
-
-   - pypi packaging
-   - tests using tox
-   - increase code coverage
-
-  * v 0.3.0
-
-    - GitLab Release
-    - HDF5 interface added
-
-  * v 0.2.1
-
-    - BUG correction on IDS attributes
-    - Numpy.Array Implementation (still work in progress)
-
-  * v 0.2.0
-
-    - Removal of AccessLayer MetaData
-
-  * v 0.1.1
-
-    - First Experimental Release
-
-
-
 This module contains a serie of function to help mange and manipulate IDSPy dataclasses
 
  * fill_missing_values
  * ids_to_hdf5
  * hdf5_to_ids
  * get_ids_value_from_string
  * set_ids_value_from_string
```

### Comparing `idspy_toolkit-0.4.1/idspy_toolkit/__init__.py` & `idspy_toolkit-0.4.2/idspy_toolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from idspy_toolkit.toolkit import fill_default_values_ids, list_ids_members,\
     get_ids_classes_as_dict
 from idspy_toolkit.converter import ids_to_hdf5, hdf5_to_ids
 from idspy_toolkit.accessor import get_ids_value_from_string, \
     set_ids_value_from_string, copy_ids
 from idspy_toolkit.utils import get_field_with_type
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 __all__ = [
     "__version__",
     "fill_default_values_ids",
     "ids_to_hdf5",
     "hdf5_to_ids",
     "get_ids_value_from_string",
```

### Comparing `idspy_toolkit-0.4.1/idspy_toolkit/accessor.py` & `idspy_toolkit-0.4.2/idspy_toolkit/accessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import dataclasses
 from dataclasses import Field
 from typing import get_type_hints, Any, get_origin, TypeVar, Type, Union
 from typing_extensions import Protocol
-from idspy_toolkit.utils import camel2snake,  extract_ndarray_info
+from idspy_toolkit.utils import camel2snake,  extract_ndarray_info, _imas_default_values
 import inspect
 from numpy import ndarray
-
+from idspy_toolkit.snippets import _IDS_LIST_DELIMITER
 
 class DataClass(Protocol):
     __dataclass_fields__: dict[str, Any]
 
 
 DC = TypeVar("DC", bound=DataClass)
 
@@ -126,15 +126,15 @@
     try:
         path_members = __split_path(path, str(type(ids)))
         current_attr = ids
     except IndexError:
         raise KeyError("get_ids_value_from_string does not allow to get a full IDS, just IDS members")
 
     for idx, subpath in enumerate(path_members):
-        if "#" in subpath:
+        if _IDS_LIST_DELIMITER in subpath:
             name, offset = subpath.strip().split("#")
             offset = int(offset)
             name = camel2snake(name)
             # TODO: check that return value of getattr is a list as expected
             list_attr = getattr(current_attr, name, None)
             len_list_attr = len(list_attr)
 
@@ -164,31 +164,33 @@
 
     :param var_type: A type to create a variable from.
     :type var_type: Any
     :return: A variable created from the given type.
     :rtype: Any
     :raises TypeError: If the input type is not a dataclass or a supported built-in type.
     :raises TypeError: If the input type is a dataclass that has a field_clazz with an unsupported type.
+    :TODO: write default values
     """
 
     if dataclasses.is_dataclass(var_type):
         dict_args = {}
         for f in dataclasses.fields(var_type):
             arg_type, is_list = get_type_arg(var_type, f.name)
             if is_list is True:
                 dict_args.update({f.name: list()})
             else:
                 if "ndarray" in str(arg_type):
                     shape, dtype = extract_ndarray_info(str(arg_type))
                     dict_args.update({f.name: ndarray(shape=shape, dtype=dtype)})
                 else:
-                    dict_args.update({f.name: arg_type()})
+                    # managing dataclasses can be tricky depending on IMAS conventions
+                    dict_args.update({f.name: _imas_default_values(arg_type)})
         return var_type(**dict_args)
     else:
-        return var_type()
+        return _imas_default_values(var_type)
 
 
 def set_ids_value_from_string(ids: Type[DC], path: str, value: Any, create_missing: bool = True):
     """
     Sets the value of an attribute in a nested dataclass given its path.
 
     :param ids: the nested dataclass instance to modify
@@ -215,15 +217,15 @@
     path_members = __split_path(path, str(type(ids)))
     current_attr = ids
 
     for idx, subpath in enumerate(path_members[:-1]):
         old_attr = current_attr
 
         # '#' indicates current item is a list element
-        if "#" in subpath:
+        if _IDS_LIST_DELIMITER in subpath:
             name, offset = subpath.strip().split("#")
             offset = int(offset)
             name = camel2snake(name)
             list_attr = getattr(current_attr, name, None)
             len_list_attr = len(list_attr)
             type_arg_list, _ = get_type_arg(old_attr, name)
             # TODO: exact role of create missing
@@ -261,15 +263,15 @@
 
     if isinstance(current_attr, (list, tuple)):
         raise AttributeError(f"attribute [{path_members[-2]}] is a list so it must be used as {path_members[-2]}#XXXX")
     if current_attr is None:
         raise AttributeError(f"attribute [{path_members[-2]}] is missing in the IDS {type(ids)}")
 
     # last attribute correspond to a list element
-    if "#" in path_members[-1]:
+    if _IDS_LIST_DELIMITER in path_members[-1]:
         name, offset = path_members[-1].strip().split("#")
         offset = int(offset)
         attr_value = getattr(current_attr, name)
         if isinstance(attr_value, (list, tuple)):
             return setattr(current_attr, name[offset], value)
         else:
             raise AttributeError(f"attribute {name} is of type {type(attr_value)} and not list")
@@ -281,24 +283,24 @@
         raise ValueError(
             f"value for attr {path_members[-1]} is of type {type(value)} and should be of type {attr_type}")
 
     setattr(current_attr, path_members[-1], value)
 
 
 def copy_ids(dest_ids: Type[DC], source_ids: Type[DC],
-             ignore_missing=False, keep_source_ids=False, bytes_to_str=True) -> None:
+             ignore_missing=False, keep_source_ids:bool=True, bytes_to_str:bool=True) -> None:
     """
     Copy the fields of the dataclass given at source_ids in the dataclass dest_ids.
 
     Args:
         dest_ids (dataclass): The destination dataclass to copy the fields to.
         source_ids (dataclass): The source dataclass to copy the fields from.
         ignore_missing (bool, optional): If True, missing fields in dest_ids are ignored. Otherwise, a KeyError is
         raised. Defaults to False.
-        keep_source_ids (bool, optional): If True, the source fields are set to None after being copied to the
+        keep_source_ids (bool, optional): If False, the source fields are set to None after being copied to the
         destination dataclass. Defaults to False.
         bytes_to_str (bool, optional): If True, bytes fields are decoded to str if the destination field_clazz is of type str.
          Otherwise, they are copied as bytes. Defaults to True.
 
     Raises:
         TypeError: If dest_ids or source_ids is not a dataclass.
         KeyError: If ignore_missing is False and a field_clazz is missing in dest_ids.
@@ -312,27 +314,29 @@
 
         # recursively call copy_ids for nested dataclasses
         if dataclasses.is_dataclass(field_value):
             nested_dest = getattr(dest_ids, field_name)
             if not dataclasses.is_dataclass(nested_dest):
                 raise TypeError("Both dest_ids and source_ids must be dataclasses.")
             copy_ids(nested_dest, field_value, ignore_missing, keep_source_ids, bytes_to_str)
-            if keep_source_ids:
+            if keep_source_ids is False:
                 setattr(source_ids, field_name, None)
         else:
             # check if the field_clazz is present in the destination dataclass
             if not ignore_missing and not hasattr(dest_ids, field_name):
                 raise KeyError(f"Field {field_name} is missing from dest_ids.")
 
             # get the field_clazz type from the destination dataclass
             field_type = get_type_hints(dest_ids)[field_name]
 
             # convert bytes to str if needed
             if bytes_to_str and isinstance(field_value, bytes) and issubclass(field_type, str):
                 field_value = field_value.decode()
 
+           # if field_value in ([], None, ()):
+           #     field_value = _imas_default_values(field_type)
             # set the field_clazz value in the destination dataclass
             setattr(dest_ids, field_name, field_value)
 
             # set the source field_clazz to None if keep_source_ids is True
-            if keep_source_ids:
+            if keep_source_ids is False:
                 setattr(source_ids, field_name, None)
```

### Comparing `idspy_toolkit-0.4.1/idspy_toolkit/converter.py` & `idspy_toolkit-0.4.2/idspy_toolkit/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,19 @@
             created_dataset = 1
             try:
                 parent_group.create_dataset(value_name, data=value, )
             except TypeError:
                 print(f"error raised for {value_name}:{value}/{type(value)}")
                 raise
     else:
-        parent_group.create_dataset(value_name, data=value, )
-
+        try:
+            parent_group.create_dataset(value_name, data=value, )
+        except TypeError:
+            print("typeerror for ",parent_group, value_name, value)
+            raise
     return created_dataset
 
 
 def get_inner_type_list(item: Union[list, tuple]) -> Union[Any, None]:
     test_var = item
 
     while isinstance(test_var, (list, tuple)):
@@ -165,15 +168,15 @@
         structure
 
         """
         pass
 
     def __check_all_fields_none(current_ids, default_vals_list):
         number_fields = len(list(dataclasses.fields(current_ids)))
-        list_default = []
+        list_default:list[Union[None, Any]] = []
         for field in dataclasses.fields(current_ids):
             field_value = getattr(current_ids, field.name)
             if isinstance(field_value, (list, tuple)):
                 if len(field_value) == 0:
                     list_default.append(None)
             elif isinstance(field_value, np.ndarray):
                 if field_value.ndim == 0:
```

### Comparing `idspy_toolkit-0.4.1/idspy_toolkit/snippets.py` & `idspy_toolkit-0.4.2/idspy_toolkit/snippets.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dataclasses import is_dataclass
 from dataclasses import Field, fields
 from typing import Union, Any
 import inspect
 
 _IDS_LIST_DELIMITER = "#"
 
+
 def _format_ids_substring(number: int, delimiter: str = "#") -> str:
     """
         return format for IDS list index.
 
         Args:
             number (int): index to consider.
 
@@ -55,14 +56,7 @@
     by alphabetic order and number after the # increasing.
 
     :param h5keylist: The list of strings to sort.
     :param delimiter: The delimiter used to separate elements, default=/.
     :Returns: list: The sorted list of strings.
     """
     return sorted(h5keylist, key=lambda x: (x.count(delimiter), x.strip().lower()))
-
-    #
-    # dataclasses_list = {}
-    # for name, obj in inspect.getmembers(module_alias):
-    #     if inspect.isclass(obj) and hasattr(obj, "__annotations__"):
-    #         dataclasses_list.update({name:obj})
-    # return dataclasses_list
```

### Comparing `idspy_toolkit-0.4.1/idspy_toolkit/toolkit.py` & `idspy_toolkit-0.4.2/idspy_toolkit/toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 from idspy_toolkit.utils import snake2camel, extract_ndarray_info, _imas_default_values
 from idspy_toolkit.accessor import get_type_arg
 
 
 class DataClass(Protocol):
     __dataclass_fields__: dict[str, Any]
 
-
 DC = TypeVar("DC", bound=DataClass)
 
 
-
 def get_ids_classes_as_dict(module_alias) -> dict[str, Type]:
     """
     Extracts the names of all dataclasses in the specified module.
 
     Args:
         module_alias (module): A module object or an alias to a module.
 
@@ -125,15 +123,14 @@
                         _list_ids(sub_ids, list_attrs, named_group=named_group,
                                   flat_idx=i)
             elif is_dataclass_instance(field_value):
                 # call recursive function
                 _list_ids(field_value, list_attrs, named_group=named_group)
             else:
                 list_attrs.append(named_group)
-
     # browse the ids
     _list_ids(ids, list_members, )
     return list_members
 
 
 def __fill_default_values_ids(parent_ids, member_name: str, member_type: Type,
                               root_type: Union[Type, None]):
@@ -171,15 +168,14 @@
                         )
             else:
                 setattr(parent_ids,
                         member_name,
                         member_type()
                         )
         except TypeError:
-
             # otherwise we suppose it's a forwardref and so type can be infered from name
             try:
                 setattr(parent_ids,
                         member_name,
                         getattr(root_type, snake2camel(member_name))()
                         )
             # and final case, current item is of type list[item] or deeper kind of list
```

### Comparing `idspy_toolkit-0.4.1/idspy_toolkit/utils.py` & `idspy_toolkit-0.4.2/idspy_toolkit/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,39 +49,48 @@
         return a default value for a given type
     :TODO : handle numpy array
     :param guessed_type:
     :return: default value of the corresponding type
     """
 
     if type(guessed_type) == type:
-        guessed_type = guessed_type()
+        try:
+            guessed_type = guessed_type()
+        # TypeError occurs if guessed_type corresponds to a numpy array
+        # since constructor needs at least a shape in that case
+        except TypeError:
+            return np.array([])
         if isinstance(guessed_type, bool):
             return False
         elif isinstance(guessed_type, int):
             return int(999999999)
         elif isinstance(guessed_type, float):
             return float(9.0e40)
         elif isinstance(guessed_type, str):
             return str("")
         elif isinstance(guessed_type, complex):
             return complex(9.0e40, -9.0e40)
         elif isinstance(guessed_type, (list, tuple)):
             return []
         else:
-            print(guessed_type, type(guessed_type))
-            return None
+            if dataclasses.is_dataclass(guessed_type):
+                return guessed_type
+            else:
+                print("unknow type found", guessed_type, type(guessed_type))
+                return None
     else:
         return [_imas_default_values(get_args(guessed_type)[0]), ]
 
 
-def __get_field_type(field) -> Type:
+def __get_field_type(field: Field[Any]) -> Type:
     """
-
-    :param field:
-    :return:
+        return the type of a dataclass field
+    :param field: name of the dataclass field
+    :return: type of the field
+    :TODO : check function when used with numpy array
     """
     try:
         field_type = tuple(x for x in field.type.__args__ if x != type(None))[0]
     except AttributeError:
         field_type = field.type
 
     return field_type
@@ -102,55 +111,75 @@
     # if member_descriptor is passed as argument, throw an exception
     if isdatadescriptor(ids_field):
         raise TypeError(f"argument ids_field {ids_field} cannot be a class member descriptor")
     # check if member is of type field
     extracted_field = ids_field
     if is_dataclass_field(ids, ids_field):
         if isinstance(ids_field, str):
-            field_value = getattr(ids, ids_field)
+            field_value = getattr(ids, ids_field, None)
             extracted_field = [x for x in dataclasses.fields(ids) if ids_field == x.name][0]
         else:
-            field_value = getattr(ids, ids_field.name)
+            field_value = getattr(ids, ids_field.name, None)
     # or a string representing a fieldname
     elif hasattr(ids, "__dataclass_fields__"):
         if ids.__dataclass_fields__.get(ids_field, None) is not None:
             extracted_field: dict[str, Any] = ids.__dataclass_fields__.get(ids_field)
             field_value = getattr(ids, extracted_field.name)
-    else:
-        raise ValueError(f"argument {str(ids_field)} does not represent a fieldname of the class {str(ids)}")
+        else:
+            raise ValueError(f"argument {str(ids_field)} does not represent a fieldname of the class {str(ids)}")
 
     expected_field_type = __get_field_type(extracted_field)
     if field_value is None:
         return None, expected_field_type
 
     if isinstance(field_value, (tuple, list)):
         if len(field_value) == 0:
             return field_value, expected_field_type
         else:
             if not isinstance(field_value[0], expected_field_type):
                 raise TypeError(
                     f"field {extracted_field.name} should be a list of  {str(expected_field_type)} and not a list of {type(field_value[0])}")
+    if isinstance(field_value, np.ndarray):
+        if field_value.ndim == 0:
+            field_value = field_value[()]
+    raise_error_type = False
     if not isinstance(field_value, expected_field_type):
+        # check if
+        if expected_field_type is int:
+            if not np.issubdtype(type(field_value), np.integer):
+                raise_error_type = True
+        elif expected_field_type is float:
+            if not np.issubdtype(type(field_value), np.inexact):
+                raise_error_type = True
+        else:
+            raise_error_type = True
+    if raise_error_type is True:
         raise TypeError(
             f"field {extracted_field.name} should be {str(expected_field_type)} and not {type(field_value)}")
 
     return field_value, expected_field_type
 
 
 def _get_all_subdataclasses(member, current_dict: dict) -> None:
     if not dataclasses.is_dataclass(member):
         return
-
+    current_dict.update({str(type(member)).split('.')[-1][:-2]: member})
     for attr in dataclasses.fields(member):
         if "ForwardRef" in str(attr.type):
             fwd_type = str(attr.type).split("ForwardRef")[1][2:-3]
             current_dict.update({fwd_type: getattr(member, fwd_type.split(".")[1])})
             _get_all_subdataclasses(getattr(member, fwd_type.split(".")[1])(), current_dict)
         else:
+
             current_var_type = __get_field_type(attr)
+            if str(current_var_type) == "typing.Any":
+                continue
+            # if var is of type numpy array or ndarray
+            if "numpy." in str(current_var_type):
+                continue
             if isinstance(current_var_type, (_GenericAlias,)) or isinstance(current_var_type(), (str, int, float)):
                 continue
 
             _get_all_subdataclasses(current_var_type(), current_dict)
 
 
 def get_all_class(module_name, current_dict: dict) -> None:
@@ -158,17 +187,19 @@
         create a dict where all keys are strings of  all dataclasses of the module
         :param module_name: name of the ids module
         :param current_dict: generated dict
         :return : None
     """
 
     correspondance_table = {x[0]: x[1] for x in getmembers(module_name, predicate=isclass) if
-                            (x[0].startswith("__") is False)}
+                            (x[0].startswith("__") is False) and ("ndarray" not in x[0])}
+    print(list(correspondance_table.keys()))
     for k, v in correspondance_table.items():
         member = v()
+
         _get_all_subdataclasses(member, current_dict)
 
 
 def extract_ndarray_info(expr: str):
     data_type_equiv = {'int': np.int32, 'float': np.float64, 'complex': np.complex128, 'str': str}
     pattern = r".*ndarray\[\((.*?)\),\s*(\w+)\]"
```

### Comparing `idspy_toolkit-0.4.1/idspy_toolkit.egg-info/PKG-INFO` & `idspy_toolkit-0.4.2/idspy_toolkit.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idspy-toolkit
-Version: 0.4.1
+Version: 0.4.2
 Summary: Tools to manipulate the IDSPy Dictionaries
 Author-email: Guillaume Fuhr <guillaume.fuhr@univ-amu.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CNRS, contributor: Y. Camenen
         Copyright (c) 2023, Aix-Marseille Univ., contributor: G. Fuhr
         All rights reserved.
@@ -38,59 +38,26 @@
 Project-URL: repository, https://gitlab.com/gkdb/imas-gk/-/tree/main/idspy_toolkit
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 IDSPy Toolkit
 =============
 
-Changelog :
-  * v 0.4.1
-
-   - correction of a bug with numpy.array having ndim=0 `#7 <https://gitlab.com/gkdb/imas-gk/-/issues/7>`_
-   - improved error message when trying to reach the root of an IDS using a path as string `#8 <https://gitlab.com/gkdb/imas-gk/-/issues/8>`_
-   - list_ids_members returns only all the ids members and not anymore ids root path also
-   - add possibility to overwrite HDF5 file written
-
-  * v 0.4.0
-
-   - pypi packaging
-   - tests using tox
-   - increase code coverage
-
-  * v 0.3.0
-
-    - GitLab Release
-    - HDF5 interface added
-
-  * v 0.2.1
-
-    - BUG correction on IDS attributes
-    - Numpy.Array Implementation (still work in progress)
-
-  * v 0.2.0
-
-    - Removal of AccessLayer MetaData
-
-  * v 0.1.1
-
-    - First Experimental Release
-
-
-
 This module contains a serie of function to help mange and manipulate IDSPy dataclasses
 
  * fill_missing_values
  * ids_to_hdf5
  * hdf5_to_ids
  * get_ids_value_from_string
  * set_ids_value_from_string
```

### Comparing `idspy_toolkit-0.4.1/idspy_toolkit.egg-info/SOURCES.txt` & `idspy_toolkit-0.4.2/idspy_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.1/pyproject.toml` & `idspy_toolkit-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,35 +6,36 @@
     "setuptools>=61.0.0",
     "wheel",
 ]
 # build-backend = "setuptools.build_meta"
 
 [project]
 name = 'idspy_toolkit'
-version = '0.4.1'
+version = '0.4.2'
 description = 'Tools to manipulate the IDSPy Dictionaries'
 readme = 'README.rst'
 authors = [
   { name = 'Guillaume Fuhr', email='guillaume.fuhr@univ-amu.fr' },
 ]
 license = {file = 'LICENSE'}
-requires-python = '>=3.10'
+requires-python = '>=3.9'
 dependencies = [
-  "idspy_dictionaries>=0.3.1",
+  "idspy_dictionaries>=33801.0.0",
 "numpy>=1.22",
 "h5py"
 ]
 
 classifiers = [
     'Development Status :: 4 - Beta',
     'Environment :: Console',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Topic :: Scientific/Engineering'
 ]
```

### Comparing `idspy_toolkit-0.4.1/tests/test_accessor.py` & `idspy_toolkit-0.4.2/tests/test_accessor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pytest
 import dataclasses
 from typing import Optional
 from numpy import ndarray
 
 from tests.classes_skels import *
 from idspy_toolkit.accessor import get_ids_value_from_string, \
-    set_ids_value_from_string, is_list_member, copy_ids, get_type_arg
-from idspy_toolkit.toolkit import list_ids_members
+    set_ids_value_from_string, is_list_member, copy_ids, get_type_arg, create_instance_from_type
+from idspy_toolkit.utils import _imas_default_values
 
 @dataclasses.dataclass
 class SubSubClass:
     member_subsubclass_aa: Optional[str] = dataclasses.field(default=""
                                                              )
     member_subsubclass_bb: Optional[int] = dataclasses.field(default=999999999
                                                              )
-    member_subsubclass_cc: Optional[float] = dataclasses.field(default=None
+    member_subsubclass_cc: Optional[float] = dataclasses.field(default=9.4e40
                                                                )
 
 
 @dataclasses.dataclass
 class SubClass:
     member_subclass: Optional[SubSubClass] = dataclasses.field(
         default=None
@@ -54,21 +54,21 @@
 @dataclasses.dataclass
 class DbgMainDataClass:
     field1: str
     field2: int
     subfield_list: list[DbgSubDataClass]
 
 
-@dataclasses.dataclass(slots=True)
+@dataclasses.dataclass
 class SubDataClass:
     subfield1: str
     subfield2: int
 
 
-@dataclasses.dataclass(slots=True)
+@dataclasses.dataclass
 class MainDataClass:
     field1: str
     field2: int
     subfield: SubDataClass
     subfield_list: list[SubDataClass]
 
 
@@ -165,7 +165,35 @@
     # Test setting a value in a list subfield without specifying an index
     with pytest.raises(ValueError):
         set_ids_value_from_string(test_mc, "subfield_list", "new_value")
 
     # Test setting a value in a list subfield with an invalid index
     with pytest.raises(AttributeError):
         set_ids_value_from_string(test_mc, "subfield_list#0001/subfield2#99", 999)
+
+
+
+
+@dataclasses.dataclass
+class MyClass:
+    my_list: list[int]
+    my_string: str
+
+
+def test_create_instance_from_type():
+    assert isinstance(create_instance_from_type(int), int)
+    assert isinstance(create_instance_from_type(float), float)
+    assert isinstance(create_instance_from_type(str), str)
+    assert isinstance(create_instance_from_type(list), list)
+    assert isinstance(create_instance_from_type(tuple), list)
+    assert isinstance(create_instance_from_type(bool), bool)
+    assert isinstance(create_instance_from_type(complex), complex)
+   # assert isinstance(create_instance_from_type(ndarray), ndarray)
+
+    assert create_instance_from_type(int) == _imas_default_values(int)
+    assert create_instance_from_type(float) == _imas_default_values(float)
+    assert create_instance_from_type(str) == _imas_default_values(str)
+    assert create_instance_from_type(list) == _imas_default_values(list)
+    assert create_instance_from_type(tuple) == _imas_default_values(list)
+    assert create_instance_from_type(bool) == _imas_default_values(bool)
+    assert create_instance_from_type(complex) == _imas_default_values(complex)
+    #assert create_instance_from_type(ndarray) == _imas_default_values(ndarray)
```

### Comparing `idspy_toolkit-0.4.1/tests/test_converter_hdf5.py` & `idspy_toolkit-0.4.2/tests/test_converter_hdf5.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import pytest
 import h5py
 from tests.classes_skels import *
 from idspy_toolkit.converter import ids_to_hdf5, get_inner_type_list, hdf5_to_ids, _is_list_empty, _is_item_list
 from random import randrange
 from typing import Union
 from numpy import array
+
 import numpy as np
 
+
 @pytest.fixture(scope="function")
 def hdf5_file(tmp_path_factory):
     fn = tmp_path_factory.mktemp("data") / "class_ids_{0:04d}.h5".format(randrange(0, 9999))
     return fn
 
 
 def _parse_hdf5(list_to_check: list, name: str) -> Union[None, int]:
@@ -121,50 +123,49 @@
     assert isinstance(get_inner_type_list([2, ]), int)
     assert get_inner_type_list([[]]) is None
     assert isinstance(get_inner_type_list([[2, ], ]), int)
     assert isinstance(get_inner_type_list([[[2, ], [3, 4]]]), int)
     assert isinstance(get_inner_type_list([[{3: 4, 5: 6}, ], ]), dict)
 
 
-
 def test_structure_dataclass_list_nested(hdf5_file):
-    myclass = baseclass(
+    myclass = BaseClass(
         list_member=[
             subclass(member_subclass=subsubclass(member_subsubclass_aa="123", member_subsubclass_bb=12345)), subclass(),
         ], )
     ids_to_hdf5(myclass, hdf5_file)
-    read_class = baseclass()
+
+    read_class = BaseClass()
     hdf5_to_ids(hdf5_file, read_class)
 
     assert len(read_class.list_member) == 1
     assert read_class.list_member[0] == myclass.list_member[0]
 
+
 def test_structure_dataclass_array_0d(hdf5_file):
     myclass = ArrayClass()
     myclass.val_array_0d = array(42.)
     ids_to_hdf5(myclass, hdf5_file)
-
     read_class = ArrayClass()
     hdf5_to_ids(hdf5_file, read_class)
-
-
-    assert read_class == myclass
-    assert read_class.val_array_0d == myclass.val_array_0d
+    assert np.testing.assert_array_equal(read_class.val_array_1d, myclass.val_array_1d) is None
+    assert np.testing.assert_array_equal(read_class.val_array_0d, myclass.val_array_0d) is None
     assert isinstance(read_class.val_array_0d, np.floating) == True
     assert isinstance(read_class.val_array_0d, np.ndarray) == False
 
+
 def test_is_list_empty():
-    assert _is_list_empty([]) == True
-    assert _is_list_empty(()) == True
-    assert _is_list_empty(np.array([])) == True
-    assert _is_list_empty(np.array(1)) == False
-    assert _is_list_empty([1, 2, 3]) == False
-    assert _is_list_empty("not a list") == False
+    assert _is_list_empty([]) is True
+    assert _is_list_empty(()) is True
+    assert _is_list_empty(np.array([])) is True
+    assert _is_list_empty(np.array(1)) is False
+    assert _is_list_empty([1, 2, 3]) is False
+    assert _is_list_empty("not a list") is False
 
 
 def test_is_item_list():
-    assert _is_item_list([]) == True
-    assert _is_item_list(()) == True
-    assert _is_item_list(np.array([])) == True
-    assert _is_item_list(np.array(1)) == False
-    assert _is_item_list([1, 2, 3]) == True
-    assert _is_item_list("not a list") == False
+    assert _is_item_list([]) is True
+    assert _is_item_list(()) is True
+    assert _is_item_list(np.array([])) is True
+    assert _is_item_list(np.array(1)) is False
+    assert _is_item_list([1, 2, 3]) is True
+    assert _is_item_list("not a list") is False
```

### Comparing `idspy_toolkit-0.4.1/tests/test_hdf5_io.py` & `idspy_toolkit-0.4.2/tests/test_hdf5_io.py`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.1/tests/test_ids_browse.py` & `idspy_toolkit-0.4.2/tests/test_ids_browse.py`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.1/tests/test_snippets.py` & `idspy_toolkit-0.4.2/tests/test_snippets.py`

 * *Files identical despite different names*

