# Comparing `tmp/xtuples-0.0.8.tar.gz` & `tmp/xtuples-0.0.9.tar.gz`

## Comparing `xtuples-0.0.8.tar` & `xtuples-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    28408 2020-02-02 00:00:00.000000 xtuples-0.0.8/README.ipynb
--rw-r--r--   0        0        0     7004 2020-02-02 00:00:00.000000 xtuples-0.0.8/docs/index.html
--rw-r--r--   0        0        0    22834 2020-02-02 00:00:00.000000 xtuples-0.0.8/docs/json.html
--rw-r--r--   0        0        0   106349 2020-02-02 00:00:00.000000 xtuples-0.0.8/docs/xtuples.html
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 xtuples-0.0.8/src/xtuples/__about__.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 xtuples-0.0.8/src/xtuples/__init__.py
--rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 xtuples-0.0.8/src/xtuples/json.py
--rw-r--r--   0        0        0    21657 2020-02-02 00:00:00.000000 xtuples-0.0.8/src/xtuples/xtuples.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 xtuples-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 xtuples-0.0.8/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xtuples-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 xtuples-0.0.8/README.md
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 xtuples-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    16081 2020-02-02 00:00:00.000000 xtuples-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    28655 2020-02-02 00:00:00.000000 xtuples-0.0.9/README.ipynb
+-rw-r--r--   0        0        0     7004 2020-02-02 00:00:00.000000 xtuples-0.0.9/docs/index.html
+-rw-r--r--   0        0        0    22834 2020-02-02 00:00:00.000000 xtuples-0.0.9/docs/json.html
+-rw-r--r--   0        0        0   106349 2020-02-02 00:00:00.000000 xtuples-0.0.9/docs/xtuples.html
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 xtuples-0.0.9/src/xtuples/__about__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 xtuples-0.0.9/src/xtuples/__init__.py
+-rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 xtuples-0.0.9/src/xtuples/json.py
+-rw-r--r--   0        0        0    21950 2020-02-02 00:00:00.000000 xtuples-0.0.9/src/xtuples/xtuples.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 xtuples-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 xtuples-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xtuples-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 xtuples-0.0.9/README.md
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 xtuples-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    16081 2020-02-02 00:00:00.000000 xtuples-0.0.9/PKG-INFO
```

### Comparing `xtuples-0.0.8/README.ipynb` & `xtuples-0.0.9/README.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996141975308642%*

 * *Differences: {"'cells'": "{26: {'source': ['#### Creation']}, 33: {'source': ['Memory usage is very similar "*

 * *            "(though very slightly larger for the iTuple than for the raw list):']}, 44: "*

 * *            "{'source': ['#### Append']}, insert: [(32, OrderedDict([('cell_type', 'markdown'), "*

 * *            "('metadata', OrderedDict()), ('source', ['#### Memory'])])), (48, "*

 * *            "OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), ('source', "*

 * *            "['#### Prepend / Extend'])]))]}"}*

```diff
@@ -319,15 +319,15 @@
                 "For instance, iTuple is a relatively minimal wrapper around the built in tuple."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Creation & Memory"
+                "#### Creation"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "As such, iTuple creation time is fairly similar to that of a raw list, at least when amortised over long enough sequences (though is generally slower for shorter ones):"
@@ -409,15 +409,22 @@
                 "%timeit list(range(10 ** 6))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Memory usage is very similar:"
+                "#### Memory"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Memory usage is very similar (though very slightly larger for the iTuple than for the raw list):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
             "outputs": [
@@ -553,15 +560,15 @@
                 "It is worth noting that per element indexing is not all that common using xtuples (as the canonical implementation is much more likely to use .map() and co)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Append / Extend"
+                "#### Append"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Appending is *much* slower, which is clearly to some extent a 'gotcha'."
@@ -597,14 +604,21 @@
                 "So, as with elementwise indexing, in the context of a canonical implementation of an entire function, performance is generally on par (if not better) with xtuples as with the equivalent built-ins."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "#### Prepend / Extend"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "Prepending to the tuple is *much* faster than with the list, though the relevant comparison is probably a deque (given that list is not at all optimised for left-append):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "metadata": {},
```

### Comparing `xtuples-0.0.8/docs/index.html` & `xtuples-0.0.9/docs/index.html`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.8/docs/json.html` & `xtuples-0.0.9/docs/json.html`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.8/docs/xtuples.html` & `xtuples-0.0.9/docs/xtuples.html`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.8/src/xtuples/json.py` & `xtuples-0.0.9/src/xtuples/json.py`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.8/src/xtuples/xtuples.py` & `xtuples-0.0.9/src/xtuples/xtuples.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,39 +50,39 @@
         # NOTE: here to prevent initialise instances of this
         # but rather use the decorator and typing.NamedTuple
         return
 
     @staticmethod
     def pipe(obj, f, *args, at = None, **kwargs):
         """
-        >>> example = Example(1, "a")
-        >>> example.pipe(lambda a, b: a, None)
-        Example(x=1, s='a', it=iTuple())
-        >>> example.pipe(lambda a, b: a, None, at = 1)
-        >>> example.pipe(lambda a, b: a, None, at = 'b')
-        >>> example.pipe(lambda a, b: a, a=None, at = 'b')
-        >>> example.pipe(lambda a, b: a, b=None, at = 'a')
-        Example(x=1, s='a', it=iTuple())
-        >>> example.pipe(lambda a, b: a, None, at = 0)
-        Example(x=1, s='a', it=iTuple())
+        >>> _Example = _Example(1, "a")
+        >>> _Example.pipe(lambda a, b: a, None)
+        _Example(x=1, s='a', it=iTuple())
+        >>> _Example.pipe(lambda a, b: a, None, at = 1)
+        >>> _Example.pipe(lambda a, b: a, None, at = 'b')
+        >>> _Example.pipe(lambda a, b: a, a=None, at = 'b')
+        >>> _Example.pipe(lambda a, b: a, b=None, at = 'a')
+        _Example(x=1, s='a', it=iTuple())
+        >>> _Example.pipe(lambda a, b: a, None, at = 0)
+        _Example(x=1, s='a', it=iTuple())
         """
         return pipe(f, obj, *args, at = at, **kwargs)
 
     @staticmethod
     def partial(obj, f, *args, **kwargs):
         return functools.partial(f, obj, *args, **kwargs)
 
     @classmethod
     def is_subclass(cls, t):
         """
         >>> nTuple.is_subclass(tuple)
         False
-        >>> nTuple.is_subclass(Example(1, "a"))
+        >>> nTuple.is_subclass(_Example(1, "a"))
         False
-        >>> nTuple.is_subclass(Example)
+        >>> nTuple.is_subclass(_Example)
         True
         """
         try:
             is_sub = issubclass(t, tuple)
         except:
             is_sub = False
         return (
@@ -93,39 +93,39 @@
         )
 
     @classmethod
     def is_instance(cls, obj):
         """
         >>> nTuple.is_instance(tuple)
         False
-        >>> nTuple.is_instance(Example)
+        >>> nTuple.is_instance(_Example)
         False
-        >>> nTuple.is_instance(Example(1, "a"))
+        >>> nTuple.is_instance(_Example(1, "a"))
         True
         """
         return (
             cls.is_subclass(type(obj)) and
             hasattr(obj, '_asdict') and
             hasattr(obj, '_fields')
         )
 
 
     @staticmethod
     def annotations(obj):
         """
-        >>> ex = Example(1, "a")
+        >>> ex = _Example(1, "a")
         >>> ex.pipe(ex.cls.annotations)
         {'x': <class 'int'>, 's': <class 'str'>, 'it': <class 'xtuples.xtuples.iTuple'>}
         """
         return fDict(obj.__annotations__)
 
     @classmethod
     def as_dict(cls, obj):
         """
-        >>> ex = Example(1, "a")
+        >>> ex = _Example(1, "a")
         >>> ex.pipe(ex.cls.as_dict)
         {'x': 1, 's': 'a', 'it': iTuple()}
         """
         return fDict(obj._asdict())
 
     @classmethod
     def decorate(meta, cls):
@@ -482,17 +482,21 @@
             assert False, at
 
     # args, kwargs
     def mapstar(self, f):
         return iTuple(data=itertools.starmap(f, self.data))
 
     def get(self, i):
+        if isinstance(i, slice):
+            return type(self)(data=self.data[i])
         return self.data[i]
 
     def __getitem__(self, i):
+        if isinstance(i, slice):
+            return type(self)(data=self.data[i])
         return self.data[i]
 
     def __iter__(self):
         return iter(self.data)
 
     def iter(self):
         """
@@ -547,14 +551,20 @@
     def last(self):
         """
         >>> iTuple.range(3).last()
         2
         """
         return self[-1]
 
+    def pop_first(self):
+        return self[1:]
+
+    def pop_last(self):
+        return self[:-1]
+
     def first_where(self, f):
         """
         >>> iTuple.range(3).first_where(lambda v: v > 0)
         1
         """
         for v in self:
             if f(v):
@@ -748,17 +758,17 @@
     # -----
 
 # ---------------------------------------------------------------
 
 @nTuple.decorate
 class _Example(typing.NamedTuple):
     """
-    >>> ex = Example(1, "a")
+    >>> ex = _Example(1, "a")
     >>> ex
-    Example(x=1, s='a', it=iTuple())
+    _Example(x=1, s='a', it=iTuple())
     >>> ex.cls
     <class 'xtuples.xtuples.nTuple'>
     >>> ex.pipe(lambda nt: nt.x)
     1
     >>> f = ex.partial(lambda nt, v: nt.x * v)
     >>> f(2)
     2
```

### Comparing `xtuples-0.0.8/.gitignore` & `xtuples-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.8/LICENSE.txt` & `xtuples-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.8/README.md` & `xtuples-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.8/pyproject.toml` & `xtuples-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.8/PKG-INFO` & `xtuples-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtuples
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Documentation, https://tomjrwilliams.github.io/xtuples/
 Project-URL: Issues, https://github.com/tomjrwilliams/xtuples/issues
 Project-URL: Source, https://github.com/tomjrwilliams/xtuples
 Author-email: Tom Williams <tomjrw@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

