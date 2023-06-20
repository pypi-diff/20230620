# Comparing `tmp/markyp-0.1910.0.tar.gz` & `tmp/markyp-0.2306.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/markyp-0.1910.0.tar", last modified: Mon Oct 14 17:47:18 2019, max compression
+gzip compressed data, was "markyp-0.2306.0.tar", last modified: Mon Jun 19 14:24:13 2023, max compression
```

## Comparing `markyp-0.1910.0.tar` & `markyp-0.2306.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2019-10-14 17:47:18.000000 markyp-0.1910.0/
--rw-r--r--   0 peter      (501) staff       (20)     8783 2019-10-14 17:47:18.000000 markyp-0.1910.0/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)     6574 2019-06-17 19:48:07.000000 markyp-0.1910.0/README.md
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2019-10-14 17:47:18.000000 markyp-0.1910.0/markyp/
--rw-r--r--   0 peter      (501) staff       (20)     1512 2019-10-14 15:30:32.000000 markyp-0.1910.0/markyp/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)    11810 2019-09-11 12:57:11.000000 markyp-0.1910.0/markyp/elements.py
--rw-r--r--   0 peter      (501) staff       (20)     2722 2019-09-11 11:51:40.000000 markyp-0.1910.0/markyp/formatters.py
--rw-r--r--   0 peter      (501) staff       (20)     8075 2019-09-13 08:13:50.000000 markyp-0.1910.0/markyp/parser.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2019-10-14 17:47:18.000000 markyp-0.1910.0/markyp.egg-info/
--rw-r--r--   0 peter      (501) staff       (20)     8783 2019-10-14 17:47:18.000000 markyp-0.1910.0/markyp.egg-info/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)      298 2019-10-14 17:47:18.000000 markyp-0.1910.0/markyp.egg-info/SOURCES.txt
--rw-r--r--   0 peter      (501) staff       (20)        1 2019-10-14 17:47:18.000000 markyp-0.1910.0/markyp.egg-info/dependency_links.txt
--rw-r--r--   0 peter      (501) staff       (20)        7 2019-10-14 17:47:18.000000 markyp-0.1910.0/markyp.egg-info/top_level.txt
--rw-r--r--   0 peter      (501) staff       (20)       38 2019-10-14 17:47:18.000000 markyp-0.1910.0/setup.cfg
--rw-r--r--   0 peter      (501) staff       (20)     2545 2019-10-14 13:32:16.000000 markyp-0.1910.0/setup.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2019-10-14 17:47:18.000000 markyp-0.1910.0/test/
--rw-r--r--   0 peter      (501) staff       (20)    17898 2019-09-11 11:50:20.000000 markyp-0.1910.0/test/test_elements.py
--rw-r--r--   0 peter      (501) staff       (20)     2857 2019-05-08 08:53:30.000000 markyp-0.1910.0/test/test_formatters.py
--rw-r--r--   0 peter      (501) staff       (20)      521 2019-03-01 08:20:47.000000 markyp-0.1910.0/test/test_init.py
--rw-r--r--   0 peter      (501) staff       (20)     4253 2019-09-13 07:27:38.000000 markyp-0.1910.0/test/test_parser.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-19 14:24:13.117523 markyp-0.2306.0/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1067 2023-06-19 14:11:00.000000 markyp-0.2306.0/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7790 2023-06-19 14:24:13.113523 markyp-0.2306.0/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6710 2023-06-19 14:11:00.000000 markyp-0.2306.0/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-19 14:24:13.113523 markyp-0.2306.0/markyp/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1503 2023-06-19 14:12:16.000000 markyp-0.2306.0/markyp/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11810 2023-06-19 14:11:00.000000 markyp-0.2306.0/markyp/elements.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2722 2023-06-19 14:11:00.000000 markyp-0.2306.0/markyp/formatters.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8304 2023-06-19 14:11:00.000000 markyp-0.2306.0/markyp/parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1321 2023-06-19 14:11:00.000000 markyp-0.2306.0/markyp/utils.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-19 14:24:13.113523 markyp-0.2306.0/markyp.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7790 2023-06-19 14:24:13.000000 markyp-0.2306.0/markyp.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      341 2023-06-19 14:24:13.000000 markyp-0.2306.0/markyp.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-19 14:24:13.000000 markyp-0.2306.0/markyp.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        7 2023-06-19 14:24:13.000000 markyp-0.2306.0/markyp.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-19 14:24:13.117523 markyp-0.2306.0/setup.cfg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2545 2023-06-19 14:11:00.000000 markyp-0.2306.0/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-19 14:24:13.113523 markyp-0.2306.0/test/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    17898 2023-06-19 14:11:00.000000 markyp-0.2306.0/test/test_elements.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2857 2023-06-19 14:11:00.000000 markyp-0.2306.0/test/test_formatters.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      521 2023-06-19 14:11:00.000000 markyp-0.2306.0/test/test_init.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4691 2023-06-19 14:11:00.000000 markyp-0.2306.0/test/test_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1359 2023-06-19 14:11:00.000000 markyp-0.2306.0/test/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `markyp-0.1910.0/PKG-INFO` & `markyp-0.2306.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,158 +1,16 @@
 Metadata-Version: 2.1
 Name: markyp
-Version: 0.1910.0
+Version: 0.2306.0
 Summary: Python 3 tools for creating markup documents.
 Home-page: https://github.com/volfpeter/markyp
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 License: MIT
-Description: [![Build Status](https://travis-ci.org/volfpeter/markyp.svg?branch=master)](https://travis-ci.org/volfpeter/markyp)
-        [![Downloads](https://pepy.tech/badge/markyp)](https://pepy.tech/project/markyp)
-        [![Downloads](https://pepy.tech/badge/markyp/month)](https://pepy.tech/project/markyp/month)
-        [![Downloads](https://pepy.tech/badge/markyp/week)](https://pepy.tech/project/markyp/week)
-        
-        # markyp
-        
-        Python 3 tools for creating markup documents.
-        
-        ## Installation
-        
-        The project is listed on the Python Package Index, it can be installed simply by executing `pip install markyp`.
-        
-        ## General concepts
-        
-        Element creation in `markyp` and its derivates usually works as follows:
-        
-        - If an element can have children, then the positional arguments passed to the component become the children of the created element.
-        - If an element can have attributes, then keyword arguments that are not listed explicitly on the argument list (i.e. `**kwargs`) are turned into element attributes.
-        - Explicitly declared keyword arguments work as documented.
-        
-        The markup defined by the created elements can be obtained by converting to root element to string (`str()`) or by using the root element's `markup` property.
-        
-        ## Getting started
-        
-        Creating new `markyp` element types is typically as simple as deriving new classes with the right name from the base elements that are provided by the project. The following example shows the creation of some HTML elements:
-        
-        ```Python
-        from markyp import ElementType
-        from markyp.elements import Element, StringElement
-        
-        class html(Element):
-            __slots__ = ()
-        
-            def __str__(self) -> str:
-                return f"<!DOCTYPE html>\n{(super().__str__())}"
-        
-        class head(Element):
-            __slots__ = ()
-        
-        class body(Element):
-            __slots__ = ()
-        
-        class title(StringElement):
-            __slots__ = ()
-        
-        class p(Element):
-            __slots__ = ()
-        
-            @property
-            def inline_children(self) -> bool:
-                return True
-        
-        class code(StringElement):
-            __slots__ = ()
-        
-        class ul(Element):
-            __slots__ = ()
-        
-        class li(Element):
-            __slots__ = ()
-        ```
-        
-        Once you have defined the basic components that are required by your project, you can make document creation easier by creating higher order functions that convert your data into markup elements.
-        
-        ```Python
-        def create_unordered_list(*items: ElementType) -> ul:
-            """Creates an unordered list from the received arguments."""
-            return ul(
-                *(li(item, class_="fancy-list-item", style="color:blue;") for item in items),
-                class_="fancy-list"
-            )
-        ```
-        
-        When everything is in place, a document can be created simply by instantiating the elements that make up the document. Notice that during element construction, positional arguments are treated as children elements and keyword arguments are treated as element attributes, allowing you to create documents using a markup-like syntax.
-        
-        ```Python
-        document = html(
-            head(title("Hello World!")),
-            body(
-                p(code("markyp"), "HTML example.", style="font-weight:bold;"),
-                p("Creating lists is easy as", style="color:blue;"),
-                create_unordered_list("One", p("Two", style="font-style:italic;"), "Three"),
-                style="font-size:20px"
-            )
-        )
-        ```
-        
-        At this point, you have a Python object representing your document. The actual markup is created only when you convert this object into a string using either the `str()` method or the `markup` property of the element.
-        
-        ```Python
-        print(document)
-        ```
-        
-        ## Domain-specific `markyp` extensions
-        
-        `markyp` extensions should follow the `markyp-{domain-or-extension-name}` naming convention. Here is a list of domain-specific extensions:
-        
-        - `markyp-rss`: RSS 2 implementation at https://github.com/volfpeter/markyp-rss, contribution is welcome.
-        - `markyp-html`: HTML implementation at https://github.com/volfpeter/markyp-html, contribution is welcome.
-        - `markyp-highlightjs`: HTML code highlighting using `highlight.js` at https://github.com/volfpeter/markyp-highlightjs, contribution is welcome.markyp-highlightjs
-        - `markyp-bootstrap4`: Bootstrap 4 implementation at https://github.com/volfpeter/markyp-bootstrap4, contribution is welcome.
-        
-        If you have created an open source `markyp` extension, please let us know and we will include your project in this list.
-        
-        ## Community guidelines
-        
-        In general, please treat each other with respect and follow the below guidelines to interact with the project:
-        
-        - _Questions, feedback_: Open an issue with a `[Question] <issue-title>` title.
-        - _Bug reports_: Open an issue with a `[Bug] <issue-title>` title, an adequate description of the bug, and a code snippet that reproduces the issue if possible.
-        - _Feature requests and ideas_: Open an issue with an `[Enhancement] <issue-title>` title and a clear description of the enhancement proposal.
-        
-        ## Contribution guidelines
-        
-        Every form of contribution is welcome, including documentation improvements, tests, bug fixes, and feature implementations.
-        
-        Please follow these guidelines to contribute to the project:
-        
-        - Make sure your changes match the documentation and coding style of the project, including [PEP 484](https://www.python.org/dev/peps/pep-0484/) type annotations.
-        - `mypy` is used to type-check the codebase, submitted code should not produce typing errors. See [this page](http://mypy-lang.org/) for more information on `mypy`.
-        - _Small_ fixes can be submitted simply by creating a pull request.
-        - Non-trivial changes should have an associated [issue](#community-guidelines) in the issue tracker that commits must reference (typically by adding `#refs <issue-id>` to the end of commit messages).
-        - Please write [tests](#testing) for the changes you make (if applicable).
-        
-        If you have any questions about contributing to the project, please contact the project owner.
-        
-        ## Testing
-        
-        As mentioned in the [contribution guidelines](#contribution-guidelines), the project is type-checked using `mypy`, so first of all, the project must pass `mypy`'s static code analysis.
-        
-        The project is tested using `pytest`. The chosen test layout is that tests are outside the application code, see [this page](https://docs.pytest.org/en/latest/goodpractices.html#tests-outside-application-code) for details on what it means in practice.
-        
-        If `pytest` is installed, the test set can be executed using the `pytest test` command from within the project directory.
-        
-        If `pytest-cov` is also installed, a test coverage report can be generated by executing `pytest test --cov markyp` from the root directory of the project.
-        
-        ## License - MIT
-        
-        The library is open-sourced under the conditions of the MIT [license](https://choosealicense.com/licenses/mit/).
-        
 Keywords: markup generator utility xml html rss
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
@@ -162,7 +20,150 @@
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Build Status](https://travis-ci.org/volfpeter/markyp.svg?branch=master)](https://travis-ci.org/volfpeter/markyp)
+[![Downloads](https://pepy.tech/badge/markyp)](https://pepy.tech/project/markyp)
+[![Downloads](https://pepy.tech/badge/markyp/month)](https://pepy.tech/project/markyp/month)
+[![Downloads](https://pepy.tech/badge/markyp/week)](https://pepy.tech/project/markyp/week)
+
+# markyp
+
+Python 3 tools for creating markup documents.
+
+## Installation
+
+The project is listed on the Python Package Index, it can be installed simply by executing `pip install markyp`.
+
+## General concepts
+
+Element creation in `markyp` and its derivates usually works as follows:
+
+- If an element can have children, then the positional arguments passed to the component become the children of the created element.
+- If an element can have attributes, then keyword arguments that are not listed explicitly on the argument list (i.e. `**kwargs`) are turned into element attributes.
+- Explicitly declared keyword arguments work as documented.
+
+The markup defined by the created elements can be obtained by converting to root element to string (`str()`) or by using the root element's `markup` property.
+
+## Getting started
+
+Creating new `markyp` element types is typically as simple as deriving new classes with the right name from the base elements that are provided by the project. The following example shows the creation of some HTML elements:
+
+```Python
+from markyp import ElementType
+from markyp.elements import Element, StringElement
+
+class html(Element):
+    __slots__ = ()
+
+    def __str__(self) -> str:
+        return f"<!DOCTYPE html>\n{(super().__str__())}"
+
+class head(Element):
+    __slots__ = ()
+
+class body(Element):
+    __slots__ = ()
+
+class title(StringElement):
+    __slots__ = ()
+
+class p(Element):
+    __slots__ = ()
+
+    @property
+    def inline_children(self) -> bool:
+        return True
+
+class code(StringElement):
+    __slots__ = ()
+
+class ul(Element):
+    __slots__ = ()
+
+class li(Element):
+    __slots__ = ()
+```
+
+Once you have defined the basic components that are required by your project, you can make document creation easier by creating higher order functions that convert your data into markup elements.
+
+```Python
+def create_unordered_list(*items: ElementType) -> ul:
+    """Creates an unordered list from the received arguments."""
+    return ul(
+        *(li(item, class_="fancy-list-item", style="color:blue;") for item in items),
+        class_="fancy-list"
+    )
+```
+
+When everything is in place, a document can be created simply by instantiating the elements that make up the document. Notice that during element construction, positional arguments are treated as children elements and keyword arguments are treated as element attributes, allowing you to create documents using a markup-like syntax.
+
+```Python
+document = html(
+    head(title("Hello World!")),
+    body(
+        p(code("markyp"), "HTML example.", style="font-weight:bold;"),
+        p("Creating lists is easy as", style="color:blue;"),
+        create_unordered_list("One", p("Two", style="font-style:italic;"), "Three"),
+        style="font-size:20px"
+    )
+)
+```
+
+At this point, you have a Python object representing your document. The actual markup is created only when you convert this object into a string using either the `str()` method or the `markup` property of the element.
+
+```Python
+print(document)
+```
+
+## Domain-specific `markyp` extensions
+
+`markyp` extensions should follow the `markyp-{domain-or-extension-name}` naming convention. Here is a list of domain-specific extensions:
+
+- `markyp-rss`: RSS 2 implementation at https://github.com/volfpeter/markyp-rss, contribution is welcome.
+- `markyp-html`: HTML implementation at https://github.com/volfpeter/markyp-html, contribution is welcome.
+- `markyp-highlightjs`: HTML code highlighting using `highlight.js` at https://github.com/volfpeter/markyp-highlightjs, contribution is welcome.
+- `markyp-bootstrap4`: Bootstrap 4 implementation at https://github.com/volfpeter/markyp-bootstrap4, contribution is welcome.
+- `markyp-fontawesome`: Font Awesome icons for `markyp-html`-based web pages at https://github.com/volfpeter/markyp-fontawesome, contribution is welcome.
+
+If you have created an open source `markyp` extension, please let us know and we will include your project in this list.
+
+## Community guidelines
+
+In general, please treat each other with respect and follow the below guidelines to interact with the project:
+
+- _Questions, feedback_: Open an issue with a `[Question] <issue-title>` title.
+- _Bug reports_: Open an issue with a `[Bug] <issue-title>` title, an adequate description of the bug, and a code snippet that reproduces the issue if possible.
+- _Feature requests and ideas_: Open an issue with an `[Enhancement] <issue-title>` title and a clear description of the enhancement proposal.
+
+## Contribution guidelines
+
+Every form of contribution is welcome, including documentation improvements, tests, bug fixes, and feature implementations.
+
+Please follow these guidelines to contribute to the project:
+
+- Make sure your changes match the documentation and coding style of the project, including [PEP 484](https://www.python.org/dev/peps/pep-0484/) type annotations.
+- `mypy` is used to type-check the codebase, submitted code should not produce typing errors. See [this page](http://mypy-lang.org/) for more information on `mypy`.
+- _Small_ fixes can be submitted simply by creating a pull request.
+- Non-trivial changes should have an associated [issue](#community-guidelines) in the issue tracker that commits must reference (typically by adding `#refs <issue-id>` to the end of commit messages).
+- Please write [tests](#testing) for the changes you make (if applicable).
+
+If you have any questions about contributing to the project, please contact the project owner.
+
+## Testing
+
+As mentioned in the [contribution guidelines](#contribution-guidelines), the project is type-checked using `mypy`, so first of all, the project must pass `mypy`'s static code analysis.
+
+The project is tested using `pytest`. The chosen test layout is that tests are outside the application code, see [this page](https://docs.pytest.org/en/latest/goodpractices.html#tests-outside-application-code) for details on what it means in practice.
+
+If `pytest` is installed, the test set can be executed using the `pytest test` command from within the project directory.
+
+If `pytest-cov` is also installed, a test coverage report can be generated by executing `pytest test --cov markyp` from the root directory of the project.
+
+## License - MIT
+
+The library is open-sourced under the conditions of the MIT [license](https://choosealicense.com/licenses/mit/).
```

### Comparing `markyp-0.1910.0/README.md` & `markyp-0.2306.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -94,16 +94,17 @@
 
 ## Domain-specific `markyp` extensions
 
 `markyp` extensions should follow the `markyp-{domain-or-extension-name}` naming convention. Here is a list of domain-specific extensions:
 
 - `markyp-rss`: RSS 2 implementation at https://github.com/volfpeter/markyp-rss, contribution is welcome.
 - `markyp-html`: HTML implementation at https://github.com/volfpeter/markyp-html, contribution is welcome.
-- `markyp-highlightjs`: HTML code highlighting using `highlight.js` at https://github.com/volfpeter/markyp-highlightjs, contribution is welcome.markyp-highlightjs
+- `markyp-highlightjs`: HTML code highlighting using `highlight.js` at https://github.com/volfpeter/markyp-highlightjs, contribution is welcome.
 - `markyp-bootstrap4`: Bootstrap 4 implementation at https://github.com/volfpeter/markyp-bootstrap4, contribution is welcome.
+- `markyp-fontawesome`: Font Awesome icons for `markyp-html`-based web pages at https://github.com/volfpeter/markyp-fontawesome, contribution is welcome.
 
 If you have created an open source `markyp` extension, please let us know and we will include your project in this list.
 
 ## Community guidelines
 
 In general, please treat each other with respect and follow the below guidelines to interact with the project:
```

### Comparing `markyp-0.1910.0/markyp/__init__.py` & `markyp-0.2306.0/markyp/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Type declarations and the most basic building blocks of `markyp`.
 """
 
-from typing import Any, Dict, TypeVar, Union
+from typing import Any, Dict, Union
 
 __author__ = "Peter Volf"
 __copyright__ = "Copyright 2019, Peter Volf"
 __email__ = "do.volfp@gmail.com"
 __license__ = "MIT"
 __url__ = "https://github.com/volfpeter/markyp"
-__version__ = "0.1910.0"
+__version__ = "0.2306.0"
 
 
 __all__ = ("IElement", "ElementType", "PropertyValue", "PropertyDict", "is_element")
 
 
 class IElement(object):
     """
```

### Comparing `markyp-0.1910.0/markyp/elements.py` & `markyp-0.2306.0/markyp/elements.py`

 * *Files identical despite different names*

### Comparing `markyp-0.1910.0/markyp/formatters.py` & `markyp-0.2306.0/markyp/formatters.py`

 * *Files identical despite different names*

### Comparing `markyp-0.1910.0/markyp/parser.py` & `markyp-0.2306.0/markyp/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,25 @@
     def element_name(self) -> str:
         """
         Inherited.
         """
         return self._tag
 
 
+class IgnoreElement(IElement):
+    """
+    Element to use in `ParserRule`s for tags that should not be parsed.
+    """
+
+    __slots__ = ()
+
+    def __new__(cls, *args, **kwargs) -> None:
+        return None
+
+
 class Parser:
     """
     `markyp` element parser.
 
     The parser accepts the following types of rules:
 
     - `IElement` classes / factory types: Class that handles tags whose name matches the class' name.
@@ -206,21 +217,18 @@
     def _get_children(self, node: ET.Element) -> Sequence[ElementType]:
         """
         Returns the children elements of the given `etree` element as `markyp` elements.
 
         Arguments:
             node: The node whose children are required.
         """
-        return (
-            [self.convert(item) for item in node]
-            if self._is_empty_string(node.text)
-            else [node.text.strip()]
-            if node.text
-            else []
-        )
+        if self._is_empty_string_or_none(node.text):
+            return [e for e in (self.convert(item) for item in node) if e is not None]
+        else:
+            return [node.text.strip()]  # type: ignore
 
     def _get_properties(self, node: ET.Element) -> PropertyDict:
         """
         Returns the properties of the given `etree` element.
 
         Argument:
             node: The node whose children are required.
@@ -258,16 +266,16 @@
             if issubclass(rule, IElement):
                 return rule.__name__, rule
         except TypeError:
             pass
 
         raise ValueError(f"Invalid factory rule: {rule}")
 
-    def _is_empty_string(self, value: Optional[str]) -> bool:
+    def _is_empty_string_or_none(self, value: Optional[str]) -> bool:
         """
-        Returns whether the given value is an empty string.
+        Returns whether the given value is an empty string or `None`.
 
         Arguments:
             value: The value to check.
         """
         return value is None or value.strip() == ""
```

### Comparing `markyp-0.1910.0/markyp.egg-info/PKG-INFO` & `markyp-0.2306.0/markyp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,158 +1,16 @@
 Metadata-Version: 2.1
 Name: markyp
-Version: 0.1910.0
+Version: 0.2306.0
 Summary: Python 3 tools for creating markup documents.
 Home-page: https://github.com/volfpeter/markyp
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 License: MIT
-Description: [![Build Status](https://travis-ci.org/volfpeter/markyp.svg?branch=master)](https://travis-ci.org/volfpeter/markyp)
-        [![Downloads](https://pepy.tech/badge/markyp)](https://pepy.tech/project/markyp)
-        [![Downloads](https://pepy.tech/badge/markyp/month)](https://pepy.tech/project/markyp/month)
-        [![Downloads](https://pepy.tech/badge/markyp/week)](https://pepy.tech/project/markyp/week)
-        
-        # markyp
-        
-        Python 3 tools for creating markup documents.
-        
-        ## Installation
-        
-        The project is listed on the Python Package Index, it can be installed simply by executing `pip install markyp`.
-        
-        ## General concepts
-        
-        Element creation in `markyp` and its derivates usually works as follows:
-        
-        - If an element can have children, then the positional arguments passed to the component become the children of the created element.
-        - If an element can have attributes, then keyword arguments that are not listed explicitly on the argument list (i.e. `**kwargs`) are turned into element attributes.
-        - Explicitly declared keyword arguments work as documented.
-        
-        The markup defined by the created elements can be obtained by converting to root element to string (`str()`) or by using the root element's `markup` property.
-        
-        ## Getting started
-        
-        Creating new `markyp` element types is typically as simple as deriving new classes with the right name from the base elements that are provided by the project. The following example shows the creation of some HTML elements:
-        
-        ```Python
-        from markyp import ElementType
-        from markyp.elements import Element, StringElement
-        
-        class html(Element):
-            __slots__ = ()
-        
-            def __str__(self) -> str:
-                return f"<!DOCTYPE html>\n{(super().__str__())}"
-        
-        class head(Element):
-            __slots__ = ()
-        
-        class body(Element):
-            __slots__ = ()
-        
-        class title(StringElement):
-            __slots__ = ()
-        
-        class p(Element):
-            __slots__ = ()
-        
-            @property
-            def inline_children(self) -> bool:
-                return True
-        
-        class code(StringElement):
-            __slots__ = ()
-        
-        class ul(Element):
-            __slots__ = ()
-        
-        class li(Element):
-            __slots__ = ()
-        ```
-        
-        Once you have defined the basic components that are required by your project, you can make document creation easier by creating higher order functions that convert your data into markup elements.
-        
-        ```Python
-        def create_unordered_list(*items: ElementType) -> ul:
-            """Creates an unordered list from the received arguments."""
-            return ul(
-                *(li(item, class_="fancy-list-item", style="color:blue;") for item in items),
-                class_="fancy-list"
-            )
-        ```
-        
-        When everything is in place, a document can be created simply by instantiating the elements that make up the document. Notice that during element construction, positional arguments are treated as children elements and keyword arguments are treated as element attributes, allowing you to create documents using a markup-like syntax.
-        
-        ```Python
-        document = html(
-            head(title("Hello World!")),
-            body(
-                p(code("markyp"), "HTML example.", style="font-weight:bold;"),
-                p("Creating lists is easy as", style="color:blue;"),
-                create_unordered_list("One", p("Two", style="font-style:italic;"), "Three"),
-                style="font-size:20px"
-            )
-        )
-        ```
-        
-        At this point, you have a Python object representing your document. The actual markup is created only when you convert this object into a string using either the `str()` method or the `markup` property of the element.
-        
-        ```Python
-        print(document)
-        ```
-        
-        ## Domain-specific `markyp` extensions
-        
-        `markyp` extensions should follow the `markyp-{domain-or-extension-name}` naming convention. Here is a list of domain-specific extensions:
-        
-        - `markyp-rss`: RSS 2 implementation at https://github.com/volfpeter/markyp-rss, contribution is welcome.
-        - `markyp-html`: HTML implementation at https://github.com/volfpeter/markyp-html, contribution is welcome.
-        - `markyp-highlightjs`: HTML code highlighting using `highlight.js` at https://github.com/volfpeter/markyp-highlightjs, contribution is welcome.markyp-highlightjs
-        - `markyp-bootstrap4`: Bootstrap 4 implementation at https://github.com/volfpeter/markyp-bootstrap4, contribution is welcome.
-        
-        If you have created an open source `markyp` extension, please let us know and we will include your project in this list.
-        
-        ## Community guidelines
-        
-        In general, please treat each other with respect and follow the below guidelines to interact with the project:
-        
-        - _Questions, feedback_: Open an issue with a `[Question] <issue-title>` title.
-        - _Bug reports_: Open an issue with a `[Bug] <issue-title>` title, an adequate description of the bug, and a code snippet that reproduces the issue if possible.
-        - _Feature requests and ideas_: Open an issue with an `[Enhancement] <issue-title>` title and a clear description of the enhancement proposal.
-        
-        ## Contribution guidelines
-        
-        Every form of contribution is welcome, including documentation improvements, tests, bug fixes, and feature implementations.
-        
-        Please follow these guidelines to contribute to the project:
-        
-        - Make sure your changes match the documentation and coding style of the project, including [PEP 484](https://www.python.org/dev/peps/pep-0484/) type annotations.
-        - `mypy` is used to type-check the codebase, submitted code should not produce typing errors. See [this page](http://mypy-lang.org/) for more information on `mypy`.
-        - _Small_ fixes can be submitted simply by creating a pull request.
-        - Non-trivial changes should have an associated [issue](#community-guidelines) in the issue tracker that commits must reference (typically by adding `#refs <issue-id>` to the end of commit messages).
-        - Please write [tests](#testing) for the changes you make (if applicable).
-        
-        If you have any questions about contributing to the project, please contact the project owner.
-        
-        ## Testing
-        
-        As mentioned in the [contribution guidelines](#contribution-guidelines), the project is type-checked using `mypy`, so first of all, the project must pass `mypy`'s static code analysis.
-        
-        The project is tested using `pytest`. The chosen test layout is that tests are outside the application code, see [this page](https://docs.pytest.org/en/latest/goodpractices.html#tests-outside-application-code) for details on what it means in practice.
-        
-        If `pytest` is installed, the test set can be executed using the `pytest test` command from within the project directory.
-        
-        If `pytest-cov` is also installed, a test coverage report can be generated by executing `pytest test --cov markyp` from the root directory of the project.
-        
-        ## License - MIT
-        
-        The library is open-sourced under the conditions of the MIT [license](https://choosealicense.com/licenses/mit/).
-        
 Keywords: markup generator utility xml html rss
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
@@ -162,7 +20,150 @@
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Build Status](https://travis-ci.org/volfpeter/markyp.svg?branch=master)](https://travis-ci.org/volfpeter/markyp)
+[![Downloads](https://pepy.tech/badge/markyp)](https://pepy.tech/project/markyp)
+[![Downloads](https://pepy.tech/badge/markyp/month)](https://pepy.tech/project/markyp/month)
+[![Downloads](https://pepy.tech/badge/markyp/week)](https://pepy.tech/project/markyp/week)
+
+# markyp
+
+Python 3 tools for creating markup documents.
+
+## Installation
+
+The project is listed on the Python Package Index, it can be installed simply by executing `pip install markyp`.
+
+## General concepts
+
+Element creation in `markyp` and its derivates usually works as follows:
+
+- If an element can have children, then the positional arguments passed to the component become the children of the created element.
+- If an element can have attributes, then keyword arguments that are not listed explicitly on the argument list (i.e. `**kwargs`) are turned into element attributes.
+- Explicitly declared keyword arguments work as documented.
+
+The markup defined by the created elements can be obtained by converting to root element to string (`str()`) or by using the root element's `markup` property.
+
+## Getting started
+
+Creating new `markyp` element types is typically as simple as deriving new classes with the right name from the base elements that are provided by the project. The following example shows the creation of some HTML elements:
+
+```Python
+from markyp import ElementType
+from markyp.elements import Element, StringElement
+
+class html(Element):
+    __slots__ = ()
+
+    def __str__(self) -> str:
+        return f"<!DOCTYPE html>\n{(super().__str__())}"
+
+class head(Element):
+    __slots__ = ()
+
+class body(Element):
+    __slots__ = ()
+
+class title(StringElement):
+    __slots__ = ()
+
+class p(Element):
+    __slots__ = ()
+
+    @property
+    def inline_children(self) -> bool:
+        return True
+
+class code(StringElement):
+    __slots__ = ()
+
+class ul(Element):
+    __slots__ = ()
+
+class li(Element):
+    __slots__ = ()
+```
+
+Once you have defined the basic components that are required by your project, you can make document creation easier by creating higher order functions that convert your data into markup elements.
+
+```Python
+def create_unordered_list(*items: ElementType) -> ul:
+    """Creates an unordered list from the received arguments."""
+    return ul(
+        *(li(item, class_="fancy-list-item", style="color:blue;") for item in items),
+        class_="fancy-list"
+    )
+```
+
+When everything is in place, a document can be created simply by instantiating the elements that make up the document. Notice that during element construction, positional arguments are treated as children elements and keyword arguments are treated as element attributes, allowing you to create documents using a markup-like syntax.
+
+```Python
+document = html(
+    head(title("Hello World!")),
+    body(
+        p(code("markyp"), "HTML example.", style="font-weight:bold;"),
+        p("Creating lists is easy as", style="color:blue;"),
+        create_unordered_list("One", p("Two", style="font-style:italic;"), "Three"),
+        style="font-size:20px"
+    )
+)
+```
+
+At this point, you have a Python object representing your document. The actual markup is created only when you convert this object into a string using either the `str()` method or the `markup` property of the element.
+
+```Python
+print(document)
+```
+
+## Domain-specific `markyp` extensions
+
+`markyp` extensions should follow the `markyp-{domain-or-extension-name}` naming convention. Here is a list of domain-specific extensions:
+
+- `markyp-rss`: RSS 2 implementation at https://github.com/volfpeter/markyp-rss, contribution is welcome.
+- `markyp-html`: HTML implementation at https://github.com/volfpeter/markyp-html, contribution is welcome.
+- `markyp-highlightjs`: HTML code highlighting using `highlight.js` at https://github.com/volfpeter/markyp-highlightjs, contribution is welcome.
+- `markyp-bootstrap4`: Bootstrap 4 implementation at https://github.com/volfpeter/markyp-bootstrap4, contribution is welcome.
+- `markyp-fontawesome`: Font Awesome icons for `markyp-html`-based web pages at https://github.com/volfpeter/markyp-fontawesome, contribution is welcome.
+
+If you have created an open source `markyp` extension, please let us know and we will include your project in this list.
+
+## Community guidelines
+
+In general, please treat each other with respect and follow the below guidelines to interact with the project:
+
+- _Questions, feedback_: Open an issue with a `[Question] <issue-title>` title.
+- _Bug reports_: Open an issue with a `[Bug] <issue-title>` title, an adequate description of the bug, and a code snippet that reproduces the issue if possible.
+- _Feature requests and ideas_: Open an issue with an `[Enhancement] <issue-title>` title and a clear description of the enhancement proposal.
+
+## Contribution guidelines
+
+Every form of contribution is welcome, including documentation improvements, tests, bug fixes, and feature implementations.
+
+Please follow these guidelines to contribute to the project:
+
+- Make sure your changes match the documentation and coding style of the project, including [PEP 484](https://www.python.org/dev/peps/pep-0484/) type annotations.
+- `mypy` is used to type-check the codebase, submitted code should not produce typing errors. See [this page](http://mypy-lang.org/) for more information on `mypy`.
+- _Small_ fixes can be submitted simply by creating a pull request.
+- Non-trivial changes should have an associated [issue](#community-guidelines) in the issue tracker that commits must reference (typically by adding `#refs <issue-id>` to the end of commit messages).
+- Please write [tests](#testing) for the changes you make (if applicable).
+
+If you have any questions about contributing to the project, please contact the project owner.
+
+## Testing
+
+As mentioned in the [contribution guidelines](#contribution-guidelines), the project is type-checked using `mypy`, so first of all, the project must pass `mypy`'s static code analysis.
+
+The project is tested using `pytest`. The chosen test layout is that tests are outside the application code, see [this page](https://docs.pytest.org/en/latest/goodpractices.html#tests-outside-application-code) for details on what it means in practice.
+
+If `pytest` is installed, the test set can be executed using the `pytest test` command from within the project directory.
+
+If `pytest-cov` is also installed, a test coverage report can be generated by executing `pytest test --cov markyp` from the root directory of the project.
+
+## License - MIT
+
+The library is open-sourced under the conditions of the MIT [license](https://choosealicense.com/licenses/mit/).
```

### Comparing `markyp-0.1910.0/setup.py` & `markyp-0.2306.0/setup.py`

 * *Files identical despite different names*

### Comparing `markyp-0.1910.0/test/test_elements.py` & `markyp-0.2306.0/test/test_elements.py`

 * *Files identical despite different names*

### Comparing `markyp-0.1910.0/test/test_formatters.py` & `markyp-0.2306.0/test/test_formatters.py`

 * *Files identical despite different names*

### Comparing `markyp-0.1910.0/test/test_init.py` & `markyp-0.2306.0/test/test_init.py`

 * *Files identical despite different names*

### Comparing `markyp-0.1910.0/test/test_parser.py` & `markyp-0.2306.0/test/test_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from markyp.elements import (
     ChildrenOnlyElement,
     Element,
     EmptyElement,
     SelfClosedElement,
     StringElement,
 )
-from markyp.parser import AnyElement, Converter, Parser, ParserRule
+from markyp.parser import AnyElement, IgnoreElement, Converter, Parser, ParserRule
 
 
 def test_converter():
     element = get_elements()
     markup = element.markup
     converted_element = get_converted_elements()
     converted_markup = converted_element.markup
@@ -60,14 +60,15 @@
 def get_elements():
     return ChildrenOnlyElement(
         Element("Children", attr1="1"),
         EmptyElement(attr1="11", attr2="22"),
         SelfClosedElement(attr1="111", attr2="222"),
         StringElement("String children"),
         AnyElement("AnyElement content", element_tag="Any", attr="any-element"),
+        SelfClosedElement(),
     )
 
 
 def get_converted_elements():
     return ChildrenOnlyElement(
         Element("Children", attr1="1", converter="applied"),
         EmptyElement(attr1="11", attr2="22", converter="applied"),
@@ -75,14 +76,15 @@
         StringElement("String children", converter="applied"),
         AnyElement(
             "AnyElement content",
             element_tag="Any",
             attr="any-element",
             converter="applied",
         ),
+        SelfClosedElement(converter="applied"),
     )
 
 
 def assert_elements_equal(foo: ElementType, bar: ElementType):
     assert type(foo) == type(bar)
 
     if isinstance(foo, str):
@@ -96,37 +98,58 @@
         assert len(foo.children) == len(bar.children)  # type: ignore
         for i in range(len(foo.children)):  # type: ignore
             assert_elements_equal(foo.children[i], bar.children[i])  # type: ignore
 
 
 def get_parsers(converter=None):
     parser_1 = Parser(
-        ChildrenOnlyElement, Element, EmptyElement, SelfClosedElement, StringElement
+        ChildrenOnlyElement,
+        Element,
+        EmptyElement,
+        SelfClosedElement,
+        StringElement,
+        IgnoreElement,
     )
     parser_2 = Parser()
     parser_2.add_rules(
-        [ChildrenOnlyElement, Element, EmptyElement, SelfClosedElement, StringElement]
+        [
+            ChildrenOnlyElement,
+            Element,
+            EmptyElement,
+            SelfClosedElement,
+            StringElement,
+            IgnoreElement,
+        ]
     )
     parser_3 = Parser(("Element", ErrorElement), ("EmptyElement", ErrorElement))
     parser_3.set_rules(
-        [ChildrenOnlyElement, Element, EmptyElement, SelfClosedElement, StringElement]
+        [
+            ChildrenOnlyElement,
+            Element,
+            EmptyElement,
+            SelfClosedElement,
+            StringElement,
+            IgnoreElement,
+        ]
     )
     parser_4 = Parser(
         ("ChildrenOnlyElement", ChildrenOnlyElement),
         ("Element", Element),
         ("EmptyElement", EmptyElement),
         ("SelfClosedElement", SelfClosedElement),
         ("StringElement", StringElement),
+        ("IgnoreElement", IgnoreElement),
     )
     parser_5 = Parser(
         ParserRule("ChildrenOnlyElement", ChildrenOnlyElement),
         ParserRule("Element", Element),
         ParserRule("EmptyElement", EmptyElement),
         ParserRule("SelfClosedElement", SelfClosedElement),
         ParserRule("StringElement", StringElement),
+        ParserRule("IgnoreElement", IgnoreElement),
     )
 
     parsers = (parser_1, parser_2, parser_3, parser_4, parser_5)
     for p in parsers:
         p.converter(converter)
 
     return parsers
```

