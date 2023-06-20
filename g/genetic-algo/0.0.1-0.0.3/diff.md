# Comparing `tmp/genetic-algo-0.0.1.tar.gz` & `tmp/genetic-algo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genetic-algo-0.0.1.tar", last modified: Sun Jun  4 19:41:11 2023, max compression
+gzip compressed data, was "genetic-algo-0.0.3.tar", last modified: Tue Jun 20 18:49:39 2023, max compression
```

## Comparing `genetic-algo-0.0.1.tar` & `genetic-algo-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 19:41:11.043917 genetic-algo-0.0.1/
--rw-rw-rw-   0        0        0      115 2023-06-04 19:41:10.000000 genetic-algo-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-06-04 19:41:11.042983 genetic-algo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-05-28 10:00:20.000000 genetic-algo-0.0.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 genetic-algo-0.0.1/build.py
-drwxrwxrwx   0        0        0        0 2023-06-04 19:41:11.028864 genetic-algo-0.0.1/genetic_algo/
--rw-rw-rw-   0        0        0     8793 2023-06-04 19:39:54.000000 genetic-algo-0.0.1/genetic_algo/attributes.py
--rw-rw-rw-   0        0        0     5518 2023-05-28 10:08:23.000000 genetic-algo-0.0.1/genetic_algo/base.py
--rw-rw-rw-   0        0        0      448 2023-06-03 06:46:07.000000 genetic-algo-0.0.1/genetic_algo/document.py
--rw-rw-rw-   0        0        0     5955 2023-06-03 06:57:31.000000 genetic-algo-0.0.1/genetic_algo/driver.py
--rw-rw-rw-   0        0        0    12195 2023-06-03 06:44:36.000000 genetic-algo-0.0.1/genetic_algo/environment.py
--rw-rw-rw-   0        0        0     4988 2023-06-04 19:39:54.000000 genetic-algo-0.0.1/genetic_algo/solution.py
-drwxrwxrwx   0        0        0        0 2023-06-04 19:41:11.041406 genetic-algo-0.0.1/genetic_algo.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-06-04 19:41:10.000000 genetic-algo-0.0.1/genetic_algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-06-04 19:41:10.000000 genetic-algo-0.0.1/genetic_algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 19:41:10.000000 genetic-algo-0.0.1/genetic_algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-04 19:41:10.000000 genetic-algo-0.0.1/genetic_algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-04 19:41:10.000000 genetic-algo-0.0.1/genetic_algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      645 2023-06-04 19:41:03.000000 genetic-algo-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       20 2023-05-28 10:10:01.000000 genetic-algo-0.0.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 10:10:01.000000 genetic-algo-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 19:41:11.043917 genetic-algo-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1601 2023-06-04 19:40:33.000000 genetic-algo-0.0.1/setup.py
--rw-rw-rw-   0        0        0     2645 2023-06-03 07:02:29.000000 genetic-algo-0.0.1/test.py
+drwxrwxrwx   0        0        0        0 2023-06-20 18:49:39.462435 genetic-algo-0.0.3/
+-rw-rw-rw-   0        0        0      115 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-06-20 18:49:39.461435 genetic-algo-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-05-28 10:00:20.000000 genetic-algo-0.0.3/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 genetic-algo-0.0.3/build.py
+drwxrwxrwx   0        0        0        0 2023-06-20 18:49:39.444844 genetic-algo-0.0.3/genetic_algo/
+-rw-rw-rw-   0        0        0     8934 2023-06-20 16:13:53.000000 genetic-algo-0.0.3/genetic_algo/attributes.py
+-rw-rw-rw-   0        0        0     5518 2023-05-28 10:08:23.000000 genetic-algo-0.0.3/genetic_algo/base.py
+-rw-rw-rw-   0        0        0      448 2023-06-03 06:46:07.000000 genetic-algo-0.0.3/genetic_algo/document.py
+-rw-rw-rw-   0        0        0     5955 2023-06-03 06:57:31.000000 genetic-algo-0.0.3/genetic_algo/driver.py
+-rw-rw-rw-   0        0        0    15381 2023-06-18 09:15:27.000000 genetic-algo-0.0.3/genetic_algo/environment.py
+-rw-rw-rw-   0        0        0     4841 2023-06-20 18:47:51.000000 genetic-algo-0.0.3/genetic_algo/solution.py
+drwxrwxrwx   0        0        0        0 2023-06-20 18:49:39.460435 genetic-algo-0.0.3/genetic_algo.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/genetic_algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/genetic_algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/genetic_algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/genetic_algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/genetic_algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      645 2023-06-20 18:49:39.000000 genetic-algo-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       38 2023-06-18 08:47:03.000000 genetic-algo-0.0.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2023-06-18 08:47:03.000000 genetic-algo-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 18:49:39.462435 genetic-algo-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2023-06-20 18:49:27.000000 genetic-algo-0.0.3/setup.py
+-rw-rw-rw-   0        0        0     2645 2023-06-03 07:02:29.000000 genetic-algo-0.0.3/test.py
```

### Comparing `genetic-algo-0.0.1/PKG-INFO` & `genetic-algo-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetic-algo
-Version: 0.0.1
+Version: 0.0.3
 Summary: A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `genetic-algo-0.0.1/README.md` & `genetic-algo-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.1/build.py` & `genetic-algo-0.0.3/build.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.1/genetic_algo/attributes.py` & `genetic-algo-0.0.3/genetic_algo/attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # attributes.py
 
 from typing import (
-    Self, Iterable, Any, Optional, Type, Union
+    Self, Iterable, Any, Optional,
+    Type, Union, Generic, TypeVar
 )
 import string
 import random
 from abc import ABCMeta
 
 from represent import BaseModel, Modifiers
 
@@ -54,38 +55,40 @@
         :return: The new definition object.
         """
 
         return Arguments(*self.args, **self.kwargs)
     # end copy
 # end Arguments
 
-class Attribute(BaseModel, metaclass=ABCMeta):
+_V = TypeVar("_V")
+
+class Attribute(BaseModel, Generic[_V], metaclass=ABCMeta):
     """A class to represent an attribute of a solution."""
 
     NAME: Optional[str] = None
 
     EXCLUDED: Iterable[Any] = []
 
     arguments = Arguments()
 
     modifiers = Modifiers(**BaseModel.modifiers)
 
     modifiers.properties = True
 
-    def __init__(self, value: Any, name: Optional[str] = None) -> None:
+    def __init__(self, value: _V, name: Optional[str] = None) -> None:
         """
         Defines the class attributes.
 
         :param value: The value of the attribute.
         :param name: The name of the attribute.
         """
 
         self.name = name or self.NAME
 
-        self._value = value
+        self._value: _V = value
     # end __init__
 
     def __hash__(self) -> int:
         """
         Returns the hash of the object.
 
         :return: The hash of the object.
@@ -107,15 +110,15 @@
             (type(self) is type(other)) and
             (self.name == other.name) and
             (self.value == other.value)
         )
     # end __eq__
 
     @property
-    def value(self) -> Any:
+    def value(self) -> _V:
         """
         Returns the value of the attribute.
 
         :return: The value.
         """
 
         if not isinstance(self._value, Attribute):
@@ -141,15 +144,15 @@
             pass
         # end while
 
         return cls(value=value)
     # end build
 
     @classmethod
-    def generate(cls, *args: Any, **kwargs: Any) -> Any:
+    def generate(cls, *args: Any, **kwargs: Any) -> _V:
         """
         Generates the random attribute value.
 
         :param args: Any positional arguments.
         :param kwargs: Any keyword arguments.
 
         :return: The attribute value.
@@ -165,15 +168,17 @@
 
         return type(self)(value=self._value, name=self.name)
     # end copy
 # end Attribute
 
 Number = Union[int, float]
 
-class NumericAttribute(Attribute):
+_NV = TypeVar("_NV", int, float)
+
+class NumericAttribute(Attribute[Number], Generic[_NV]):
     """A class to represent an attribute of a solution."""
 
     BASE: Type[Number] = float
 
     FLOOR: Number = None
     ROOF: Number = None
     STEP: Optional[Number] = None
@@ -255,35 +260,35 @@
                 f"{cls} 'base' must be an int "
                 f"or a float when , not {base}."
             )
         # end if
     # end generate
 # end NumericAttribute
 
-class IntegerAttribute(NumericAttribute):
+class IntegerAttribute(NumericAttribute[int]):
     """A class to represent an attribute of a solution."""
 
     BASE = int
 
     FLOOR = 0
     ROOF = 100
     STEP = 1
 # end IntegerAttribute
 
-class FloatAttribute(NumericAttribute):
+class FloatAttribute(NumericAttribute[float]):
     """A class to represent an attribute of a solution."""
 
     BASE = float
 
     FLOOR = 0.0
     ROOF = 1.0
     STEP = 0.01
 # end FloatAttribute
 
-class StringAttribute(Attribute):
+class StringAttribute(Attribute[str]):
     """A class to represent an attribute of a solution."""
 
     SOURCE: Iterable[str] = string.ascii_lowercase
     SEPARATOR: str = ""
 
     LENGTH: int = 10
 
@@ -340,19 +345,19 @@
             )
         # end if
 
         return separator.join(random.choices(list(source), k=length))
     # end generate
 # end StringAttribute
 
-class BooleanAttribute(Attribute):
+class BooleanAttribute(Attribute[bool]):
     """A class to represent an attribute of a solution."""
 
     @classmethod
-    def generate(cls) -> str:
+    def generate(cls) -> bool:
         """
         Generates the random attribute value.
 
         :return: The attribute value.
         """
 
         return random.choice([True, False])
```

### Comparing `genetic-algo-0.0.1/genetic_algo/base.py` & `genetic-algo-0.0.3/genetic_algo/base.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.1/genetic_algo/driver.py` & `genetic-algo-0.0.3/genetic_algo/driver.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.1/genetic_algo/solution.py` & `genetic-algo-0.0.3/genetic_algo/solution.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # solution.py
 
 from typing import (
-    Self, Iterable, Optional, Type, List, Union
+    Self, Iterable, Optional, Type,
+    List, Union, Generic, TypeVar
 )
 
 from represent import BaseModel
 
 from genetic_algo.attributes import Attribute
 
 __all__ = [
@@ -108,50 +109,47 @@
             unique.append(slo1)
         # end if
     # end for
 
     return unique
 # end eliminate_repetitions
 
-class Template(BaseModel):
+_S = TypeVar("_S")
+
+Attributes = List[
+    Union[
+        Union[Attribute, Type[Attribute]],
+        Iterable[Union[Attribute, Type[Attribute]]]
+    ]
+]
+
+class Template(BaseModel, Generic[_S]):
     """A class to represent a template for solution attributes."""
 
-    SOLUTION = Solution
-    ATTRIBUTES: List[
-        Union[
-            Union[Attribute, Type[Attribute]],
-            Iterable[Union[Attribute, Type[Attribute]]]
-        ]
-    ] = []
+    SOLUTION: _S = Solution
+    ATTRIBUTES: Attributes = []
 
     def __init__(
             self,
-            solution: Optional[Type[Solution]] = None,
-            attributes: Optional[
-                List[
-                    Union[
-                        Union[Attribute, Type[Attribute]],
-                        Iterable[Union[Attribute, Type[Attribute]]]
-                    ]
-                ]
-            ] = None
+            solution: Optional[Type[_S]] = None,
+            attributes: Optional[Attributes] = None
     ) -> None:
         """
         Defines the class attributes.
 
         :param solution: The type of the solution object.
         :param attributes: The attributes of the solution.
         """
 
-        self.solution = solution or self.SOLUTION
+        self.solution: Type[_S] = solution or self.SOLUTION
 
-        self.attributes = list(attributes or []) or self.ATTRIBUTES
+        self.attributes: Attributes = list(attributes or []) or self.ATTRIBUTES
     # end __init__
 
-    def build(self) -> Solution:
+    def build(self) -> _S:
         """
         Generates the random attribute.
 
         :return: The attribute object.
         """
 
         attributes = []
```

### Comparing `genetic-algo-0.0.1/genetic_algo.egg-info/PKG-INFO` & `genetic-algo-0.0.3/genetic_algo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetic-algo
-Version: 0.0.1
+Version: 0.0.3
 Summary: A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `genetic-algo-0.0.1/pyproject.toml` & `genetic-algo-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'genetic-algo'
-version = '0.0.1'
+version = '0.0.3'
 description = 'A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `genetic-algo-0.0.1/setup.py` & `genetic-algo-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='genetic-algo',
-        version='0.0.1',
+        version='0.0.3',
         description=(
             "A framework for developing Genetic-Algorithm "
             "programs to solve problems dynamically and explicitly."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

### Comparing `genetic-algo-0.0.1/test.py` & `genetic-algo-0.0.3/test.py`

 * *Files identical despite different names*

