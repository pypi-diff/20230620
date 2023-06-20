# Comparing `tmp/sphinxcontrib-chapeldomain-0.0.8.tar.gz` & `tmp/sphinxcontrib-chapeldomain-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinxcontrib-chapeldomain-0.0.8.tar", last modified: Thu Feb 26 03:43:21 2015, max compression
+gzip compressed data, was "dist/sphinxcontrib-chapeldomain-0.0.9.tar", last modified: Thu Feb 26 19:22:32 2015, max compression
```

## Comparing `sphinxcontrib-chapeldomain-0.0.8.tar` & `sphinxcontrib-chapeldomain-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tvandoren  (4285)      513        0 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/
--rw-r--r--   0 tvandoren  (4285)      513    11357 2014-12-09 21:37:31.000000 sphinxcontrib-chapeldomain-0.0.8/LICENSE
--rw-r--r--   0 tvandoren  (4285)      513       35 2014-12-09 22:59:15.000000 sphinxcontrib-chapeldomain-0.0.8/MANIFEST.in
--rw-r--r--   0 tvandoren  (4285)      513     3316 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/PKG-INFO
--rw-r--r--   0 tvandoren  (4285)      513     1787 2015-01-27 18:36:12.000000 sphinxcontrib-chapeldomain-0.0.8/README.rst
--rw-r--r--   0 tvandoren  (4285)      513       59 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/setup.cfg
--rw-r--r--   0 tvandoren  (4285)      513     1734 2015-02-04 00:59:17.000000 sphinxcontrib-chapeldomain-0.0.8/setup.py
-drwxr-xr-x   0 tvandoren  (4285)      513        0 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib/
--rw-r--r--   0 tvandoren  (4285)      513      252 2014-12-10 05:31:11.000000 sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib/__init__.py
--rw-r--r--   0 tvandoren  (4285)      513    37928 2015-02-26 03:36:46.000000 sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib/chapeldomain.py
-drwxr-xr-x   0 tvandoren  (4285)      513        0 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib_chapeldomain.egg-info/
--rw-r--r--   0 tvandoren  (4285)      513        1 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib_chapeldomain.egg-info/dependency_links.txt
--rw-r--r--   0 tvandoren  (4285)      513       14 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib_chapeldomain.egg-info/namespace_packages.txt
--rw-r--r--   0 tvandoren  (4285)      513        1 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib_chapeldomain.egg-info/not-zip-safe
--rw-r--r--   0 tvandoren  (4285)      513     3316 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib_chapeldomain.egg-info/PKG-INFO
--rw-r--r--   0 tvandoren  (4285)      513       24 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib_chapeldomain.egg-info/requires.txt
--rw-r--r--   0 tvandoren  (4285)      513      478 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib_chapeldomain.egg-info/SOURCES.txt
--rw-r--r--   0 tvandoren  (4285)      513       14 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib_chapeldomain.egg-info/top_level.txt
-drwxr-xr-x   0 tvandoren  (4285)      513        0 2015-02-26 03:43:21.000000 sphinxcontrib-chapeldomain-0.0.8/test/
--rw-r--r--   0 tvandoren  (4285)      513    23309 2015-02-26 03:36:46.000000 sphinxcontrib-chapeldomain-0.0.8/test/test_chapeldomain.py
+drwxr-xr-x   0 tvandoren  (4285)      513        0 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/
+-rw-r--r--   0 tvandoren  (4285)      513    11357 2014-12-09 21:37:31.000000 sphinxcontrib-chapeldomain-0.0.9/LICENSE
+-rw-r--r--   0 tvandoren  (4285)      513       35 2014-12-09 22:59:15.000000 sphinxcontrib-chapeldomain-0.0.9/MANIFEST.in
+-rw-r--r--   0 tvandoren  (4285)      513     3316 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/PKG-INFO
+-rw-r--r--   0 tvandoren  (4285)      513     1787 2015-01-27 18:36:12.000000 sphinxcontrib-chapeldomain-0.0.9/README.rst
+-rw-r--r--   0 tvandoren  (4285)      513       59 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/setup.cfg
+-rw-r--r--   0 tvandoren  (4285)      513     1734 2015-02-04 00:59:17.000000 sphinxcontrib-chapeldomain-0.0.9/setup.py
+drwxr-xr-x   0 tvandoren  (4285)      513        0 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib/
+-rw-r--r--   0 tvandoren  (4285)      513      252 2014-12-10 05:31:11.000000 sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib/__init__.py
+-rw-r--r--   0 tvandoren  (4285)      513    38089 2015-02-26 19:19:31.000000 sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib/chapeldomain.py
+drwxr-xr-x   0 tvandoren  (4285)      513        0 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib_chapeldomain.egg-info/
+-rw-r--r--   0 tvandoren  (4285)      513        1 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib_chapeldomain.egg-info/dependency_links.txt
+-rw-r--r--   0 tvandoren  (4285)      513       14 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib_chapeldomain.egg-info/namespace_packages.txt
+-rw-r--r--   0 tvandoren  (4285)      513        1 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib_chapeldomain.egg-info/not-zip-safe
+-rw-r--r--   0 tvandoren  (4285)      513     3316 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib_chapeldomain.egg-info/PKG-INFO
+-rw-r--r--   0 tvandoren  (4285)      513       24 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib_chapeldomain.egg-info/requires.txt
+-rw-r--r--   0 tvandoren  (4285)      513      478 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib_chapeldomain.egg-info/SOURCES.txt
+-rw-r--r--   0 tvandoren  (4285)      513       14 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib_chapeldomain.egg-info/top_level.txt
+drwxr-xr-x   0 tvandoren  (4285)      513        0 2015-02-26 19:22:32.000000 sphinxcontrib-chapeldomain-0.0.9/test/
+-rw-r--r--   0 tvandoren  (4285)      513    28023 2015-02-26 19:19:31.000000 sphinxcontrib-chapeldomain-0.0.9/test/test_chapeldomain.py
```

### Comparing `sphinxcontrib-chapeldomain-0.0.8/LICENSE` & `sphinxcontrib-chapeldomain-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-chapeldomain-0.0.8/PKG-INFO` & `sphinxcontrib-chapeldomain-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sphinxcontrib-chapeldomain
-Version: 0.0.8
+Version: 0.0.9
 Summary: Chapel domain for Sphinx
 Home-page: https://github.com/chapel-lang/sphinxcontrib-chapeldomain
 Author: Chapel Team
 Author-email: chapel-developers@lists.sourceforge.net
 License: Apache License v2.0
 Download-URL: https://pypi.python.org/pypi/sphinxcontrib-chapeldomain
 Description: Chapel Domain for Sphinx
```

### Comparing `sphinxcontrib-chapeldomain-0.0.8/README.rst` & `sphinxcontrib-chapeldomain-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-chapeldomain-0.0.8/setup.py` & `sphinxcontrib-chapeldomain-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib/chapeldomain.py` & `sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib/chapeldomain.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from sphinx.locale import l_, _
 from sphinx.roles import XRefRole
 from sphinx.util.compat import Directive
 from sphinx.util.docfields import Field, TypedField
 from sphinx.util.nodes import make_refnode
 
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 
 # regex for parsing proc, iter, class, record, etc.
 chpl_sig_pattern = re.compile(
     r"""^ ((?:\w+\s+)*                   # optional: prefixes
            (?:proc|iter|class|record)\s+ #   must end with keyword
           )?
@@ -47,15 +47,15 @@
           $""", re.VERBOSE)
 
 # regex for parsing attribute and data directives.
 chpl_attr_sig_pattern = re.compile(
     r"""^ ((?:\w+\s+)*)?          # optional: prefixes
           ([\w$.]*\.)?            # class name(s)
           ([\w$]+)                # const, var, param, etc name
-          (\s* [:=] \s* [^:=]+)?  # optional: type
+          (\s* [:=] \s* .+)?      # optional: type
           $""", re.VERBOSE)
 
 
 # This would be the ideal way to create a chapelerific desc_returns similar to
 # addnodes.desc_returns. However, due to some update issue, the
 # nodes._add_node_class_names() call does not seem to make chapel_desc_returns
 # to the sphinx html write. So, we'll just use addnodes.desc_returns
@@ -503,23 +503,25 @@
 class ChapelModuleLevel(ChapelObject):
     """Chapel module level functions, types, and variables (i.e. data directives)
     descriptions.
     """
 
     @property
     def chpl_type_name(self):
-        """Returns iterator or procedure or '' depending on object type."""
-        if not self.objtype.endswith('function'):
+        """Returns type, iterator, or procedure or '' depending on
+        object type.
+        """
+        if self.objtype == 'type':
+            return 'type'
+        elif not self.objtype.endswith('function'):
             return ''
         elif self.objtype.startswith('iter'):
             return 'iterator'
         elif self.objtype == 'function':
             return 'procedure'
-        elif self.objtype == 'type':
-            return 'type'
         else:
             return ''
 
     def get_signature_prefix(self, sig):
         """Return signature prefix based on sig. May include portion of the sig text,
         if relevant (e.g. `proc foo()` will return `proc` here.
         """
@@ -532,18 +534,21 @@
     def get_index_text(self, modname, name_cls):
         """Return text for index entry based on object type."""
         if self.objtype.endswith('function'):
             if not modname:
                 return _('%s() (built-in %s)') % \
                     (name_cls[0], self.chpl_type_name)
             return _('%s() (in module %s)') % (name_cls[0], modname)
-        elif self.objtype in ('data'):
+        elif self.objtype in ('data', 'type'):
             if not modname:
-                return _('%s (built-in variable)') % name_cls[0]
-            return _('%s() (in module %s)') % (name_cls[0], modname)
+                type_name = self.objtype
+                if type_name == 'data':
+                    type_name = 'variable'
+                return _('%s (built-in %s)') % (name_cls[0], type_name)
+            return _('%s (in module %s)') % (name_cls[0], modname)
         else:
             return ''
 
 
 class ChapelXRefRole(XRefRole):
     """Chapel cross-referencing role. Extends base XRefRole with special link
     processing method. The Chapel link processing knows how to match a chapel
```

### Comparing `sphinxcontrib-chapeldomain-0.0.8/sphinxcontrib_chapeldomain.egg-info/PKG-INFO` & `sphinxcontrib-chapeldomain-0.0.9/sphinxcontrib_chapeldomain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sphinxcontrib-chapeldomain
-Version: 0.0.8
+Version: 0.0.9
 Summary: Chapel domain for Sphinx
 Home-page: https://github.com/chapel-lang/sphinxcontrib-chapeldomain
 Author: Chapel Team
 Author-email: chapel-developers@lists.sourceforge.net
 License: Apache License v2.0
 Download-URL: https://pypi.python.org/pypi/sphinxcontrib-chapeldomain
 Description: Chapel Domain for Sphinx
```

### Comparing `sphinxcontrib-chapeldomain-0.0.8/test/test_chapeldomain.py` & `sphinxcontrib-chapeldomain-0.0.9/test/test_chapeldomain.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import unittest
 
 # For python 2.6 and lower, use unittest2.
 if sys.version_info[0] == 2 and sys.version_info[1] < 7:
     import unittest2 as unittest
 
 from sphinxcontrib.chapeldomain import (
-    ChapelDomain, ChapelModuleIndex, ChapelObject,
+    ChapelDomain, ChapelModuleIndex, ChapelModuleLevel, ChapelObject,
     chpl_sig_pattern, chpl_attr_sig_pattern,
 )
 
 
 class ChapelDomainTests(unittest.TestCase):
     """ChapelDomain tests."""
 
@@ -30,15 +30,15 @@
 
 class ChapelModuleIndexTests(unittest.TestCase):
     """ChapelModuleIndex tests."""
 
     @classmethod
     def setUpClass(cls):
         """Initalize sphinx locale stuff."""
-        super(cls, ChapelModuleIndexTests).setUpClass()
+        super(ChapelModuleIndexTests, cls).setUpClass()
         import sphinx.locale
         sphinx.locale.init([], 'en')
 
     def setUp(self):
         """Add some useful values to this instance."""
         self.modules = {
             # Regular sub-module.
@@ -152,16 +152,25 @@
         ]
 
         contents, collapse = index.generate()
         self.assertTrue(collapse)
         self.assertEqual(expected_contents, contents)
 
 
-class ChapelObjectTests(unittest.TestCase):
-    """ChapelObject tests."""
+class ChapelObjectTestCase(unittest.TestCase):
+    """Helper for ChapelObject related tests."""
+
+    object_cls = ChapelObject
+
+    @classmethod
+    def setUpClass(cls):
+        """Initalize sphinx locale stuff."""
+        super(ChapelObjectTestCase, cls).setUpClass()
+        import sphinx.locale
+        sphinx.locale.init([], 'en')
 
     def new_obj(self, objtype, **kwargs):
         """Return new mocked out ChapelObject"""
         default_args = {
             'name': 'my-chpl',
             'arguments': mock.Mock('arguments'),
             'options': mock.Mock('options'),
@@ -169,18 +178,120 @@
             'lineno': mock.Mock('lineno'),
             'content_offset': mock.Mock('content_offset'),
             'block_text': mock.Mock('block_text'),
             'state': mock.Mock('state'),
             'state_machine': mock.Mock('state_machine'),
         }
         default_args.update(kwargs)
-        o = ChapelObject(**default_args)
+        o = self.object_cls(**default_args)
         o.objtype = objtype
         return o
 
+
+class ChapelModuleLevelTests(ChapelObjectTestCase):
+    """ChapelModuleLevel tests."""
+
+    object_cls = ChapelModuleLevel
+
+    def test_get_index_text__function__no_mod(self):
+        """Verify get_index_text() for function without module."""
+        mod = self.new_obj('function')
+        expected_text = 'myProc() (built-in procedure)'
+        actual_text = mod.get_index_text(None, ('myProc',))
+        self.assertEqual(expected_text, actual_text)
+
+    def test_get_index_text__function__mod(self):
+        """Verify get_index_text() for function with module."""
+        mod = self.new_obj('function')
+        expected_text = 'myProc() (in module MyMod)'
+        actual_text = mod.get_index_text('MyMod', ('myProc',))
+        self.assertEqual(expected_text, actual_text)
+
+    def test_get_index_text__iter__no_mod(self):
+        """Verify get_index_text() for function without module."""
+        mod = self.new_obj('iterfunction')
+        expected_text = 'myProc() (built-in iterator)'
+        actual_text = mod.get_index_text(None, ('myProc',))
+        self.assertEqual(expected_text, actual_text)
+
+    def test_get_index_text__iter__mod(self):
+        """Verify get_index_text() for function with module."""
+        mod = self.new_obj('iterfunction')
+        expected_text = 'myProc() (in module MyMod)'
+        actual_text = mod.get_index_text('MyMod', ('myProc',))
+        self.assertEqual(expected_text, actual_text)
+
+    def test_get_index_text__data__no_mod(self):
+        """Verify get_index_text() for data without module."""
+        mod = self.new_obj('data')
+        expected_text = 'myThing (built-in variable)'
+        actual_text = mod.get_index_text(None, ('myThing',))
+        self.assertEqual(expected_text, actual_text)
+
+    def test_get_index_text__data__mod(self):
+        """Verify get_index_text() for data with module."""
+        mod = self.new_obj('data')
+        expected_text = 'myThing (in module MyMod)'
+        actual_text = mod.get_index_text('MyMod', ('myThing',))
+        self.assertEqual(expected_text, actual_text)
+
+    def test_get_index_text__type__no_mod(self):
+        """Verify get_index_text() for type without module."""
+        mod = self.new_obj('type')
+        expected_text = 'myType (built-in type)'
+        actual_text = mod.get_index_text(None, ('myType',))
+        self.assertEqual(expected_text, actual_text)
+
+    def test_get_index_text__type__mod(self):
+        """Verify get_index_text() for type with module."""
+        mod = self.new_obj('type')
+        expected_text = 'myType (in module MyMod)'
+        actual_text = mod.get_index_text('MyMod', ('myType',))
+        self.assertEqual(expected_text, actual_text)
+
+    def test_get_index_text__other(self):
+        """Verify get_index_text() returns empty string for object types other than
+        function, attribute, and type.
+        """
+        for objtype in ('other', 'attribute', 'class', 'module', 'method', 'itermethod'):
+            mod = self.new_obj(objtype)
+            self.assertEqual('', mod.get_index_text('MyMod', ('myThing',)))
+
+    def test_chpl_type_name(self):
+        """Verify chpl_type_name property for different objtypes."""
+        test_cases = [
+            ('function', 'procedure'),
+            ('iterfunction', 'iterator'),
+            ('type', 'type'),
+            ('data', ''),
+            ('method', ''),
+            ('itermethod', ''),
+        ]
+        for objtype, expected_type in test_cases:
+            mod = self.new_obj(objtype)
+            self.assertEqual(expected_type, mod.chpl_type_name)
+
+    def test_needs_arglist(self):
+        """Verify needs_arglist()."""
+        test_cases = [
+            ('function', True),
+            ('iterfunction', True),
+            ('type', False),
+            ('data', False),
+            ('method', False),
+            ('itermethod', False),
+        ]
+        for objtype, expected in test_cases:
+            mod = self.new_obj(objtype)
+            self.assertEqual(expected, mod.needs_arglist())
+
+
+class ChapelObjectTests(ChapelObjectTestCase):
+    """ChapelObject tests."""
+
     def test_init(self):
         """Verify ChapelObject can be initialized."""
         self.assertIsNotNone(self.new_obj('blah'))
 
     def test_is_attr_like__true(self):
         """Verify _is_attr_like return True for data and
         attribute directives.
@@ -585,14 +696,18 @@
             ('config param MyMod.DEBUG: bool', 'config param ', 'MyMod.', 'DEBUG', ': bool'),
             ('var RandomStreamPrivate_lock$: _syncvar(bool)', 'var ', None, 'RandomStreamPrivate_lock$', ': _syncvar(bool)'),
             ('var RandomStreamPrivate_lock$: sync bool', 'var ', None, 'RandomStreamPrivate_lock$', ': sync bool'),
             ('const RS$.lock$: sync MyMod$.MyClass$.bool', 'const ', 'RS$.', 'lock$', ': sync MyMod$.MyClass$.bool'),
             ('type commDiagnostics = chpl_commDiagnostics', 'type ', None, 'commDiagnostics', ' = chpl_commDiagnostics'),
             ('type age = int(64)', 'type ', None, 'age', ' = int(64)'),
             ('type MyMod.BigAge=BigNum.BigInt', 'type ', 'MyMod.', 'BigAge', '=BigNum.BigInt'),
+            ('const x = false', 'const ', None, 'x', ' = false'),
+            ('config const MyC.x: int(64) = 5', 'config const ', 'MyC.', 'x', ': int(64) = 5'),
+            ('config param n: uint(64) = 5: uint(64)', 'config param ', None, 'n', ': uint(64) = 5: uint(64)'),
+            ('var MyM.MyC.x = 4: uint(64)', 'var ', 'MyM.MyC.', 'x', ' = 4: uint(64)'),
         ]
         for sig, prefix, class_name, attr, type_name in test_cases:
             self.check_sig(sig, prefix, class_name, attr, type_name)
 
 
 if __name__ == '__main__':
     unittest.main()
```

