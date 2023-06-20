# Comparing `tmp/eventb-to-txt-1.4.tar.gz` & `tmp/eventb-to-txt-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventb-to-txt-1.4.tar", last modified: Mon Mar 15 12:10:03 2021, max compression
+gzip compressed data, was "eventb-to-txt-1.5.tar", last modified: Tue Jun 20 10:25:36 2023, max compression
```

## Comparing `eventb-to-txt-1.4.tar` & `eventb-to-txt-1.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 12:10:03.075292 eventb-to-txt-1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2021-03-15 12:10:03.075292 eventb-to-txt-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2021-03-15 12:09:54.000000 eventb-to-txt-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 12:10:03.071292 eventb-to-txt-1.4/eventb_to_txt/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-15 12:09:54.000000 eventb-to-txt-1.4/eventb_to_txt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2021-03-15 12:09:54.000000 eventb-to-txt-1.4/eventb_to_txt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-03-15 12:09:54.000000 eventb-to-txt-1.4/eventb_to_txt/abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)     3868 2021-03-15 12:09:54.000000 eventb-to-txt-1.4/eventb_to_txt/context.py
--rw-r--r--   0 runner    (1001) docker     (121)    10679 2021-03-15 12:09:54.000000 eventb-to-txt-1.4/eventb_to_txt/machine.py
--rw-r--r--   0 runner    (1001) docker     (121)     4501 2021-03-15 12:09:54.000000 eventb-to-txt-1.4/eventb_to_txt/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 12:10:03.075292 eventb-to-txt-1.4/eventb_to_txt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2021-03-15 12:10:02.000000 eventb-to-txt-1.4/eventb_to_txt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-03-15 12:10:02.000000 eventb-to-txt-1.4/eventb_to_txt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-15 12:10:02.000000 eventb-to-txt-1.4/eventb_to_txt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-03-15 12:10:02.000000 eventb-to-txt-1.4/eventb_to_txt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-03-15 12:10:02.000000 eventb-to-txt-1.4/eventb_to_txt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-15 12:10:03.075292 eventb-to-txt-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-03-15 12:09:54.000000 eventb-to-txt-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:25:36.003524 eventb-to-txt-1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 10:25:28.000000 eventb-to-txt-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-20 10:25:36.003524 eventb-to-txt-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-20 10:25:28.000000 eventb-to-txt-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:25:35.999524 eventb-to-txt-1.5/eventb_to_txt/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 10:25:28.000000 eventb-to-txt-1.5/eventb_to_txt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-20 10:25:28.000000 eventb-to-txt-1.5/eventb_to_txt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-20 10:25:28.000000 eventb-to-txt-1.5/eventb_to_txt/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-20 10:25:28.000000 eventb-to-txt-1.5/eventb_to_txt/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-06-20 10:25:28.000000 eventb-to-txt-1.5/eventb_to_txt/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-20 10:25:28.000000 eventb-to-txt-1.5/eventb_to_txt/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:25:36.003524 eventb-to-txt-1.5/eventb_to_txt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-20 10:25:35.000000 eventb-to-txt-1.5/eventb_to_txt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-20 10:25:35.000000 eventb-to-txt-1.5/eventb_to_txt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:25:35.000000 eventb-to-txt-1.5/eventb_to_txt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 10:25:35.000000 eventb-to-txt-1.5/eventb_to_txt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 10:25:35.000000 eventb-to-txt-1.5/eventb_to_txt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:25:36.003524 eventb-to-txt-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-20 10:25:28.000000 eventb-to-txt-1.5/setup.py
```

### Comparing `eventb-to-txt-1.4/PKG-INFO` & `eventb-to-txt-1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: eventb-to-txt
-Version: 1.4
+Version: 1.5
 Summary: Event-B to txt converter
 Home-page: https://github.com/17451k/eventb-to-txt
 Author: Ilya Shchepetkov
 Author-email: ilya.shchepetkov@yandex.ru
 License: LICENSE.txt
-Description: ![test](https://github.com/17451k/eventb-to-txt/workflows/test/badge.svg)
-        [![Coverage Status](https://coveralls.io/repos/github/17451k/eventb-to-txt/badge.svg?branch=master)](https://coveralls.io/github/17451k/eventb-to-txt?branch=master)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/eventb-to-txt.svg)](https://pypi.python.org/pypi/eventb-to-txt/)
-        [![PyPI version](https://badge.fury.io/py/eventb-to-txt.svg)](https://badge.fury.io/py/eventb-to-txt)
-        
-        # Event-B to txt converter
-        The eventb-to-txt script simply converts Event-B machines and contexts (.bum and .buc files) to the plain text. This text itself is a valid Event-B model that can be used in the CamilleX editor.
-        
-        Compatible with Event-B models created with Rodin 3.0 and above.
-        
-        ## Installation
-        ```
-            $ python3 -m pip install eventb-to-txt
-        ```
-        
-        ## Usage
-        ```
-            usage: eventb-to-txt [-h] [-o PATH] [-m] [in_path]
-        
-            positional arguments:
-            in_path              path to the Event-B model directory or zipfile
-        
-            optional arguments:
-            -h, --help           show this help message and exit
-            -o PATH, --out PATH  PATH to the output directory
-            -m, --merge          merge all generated txt files into a single txt file
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![test](https://github.com/17451k/eventb-to-txt/workflows/test/badge.svg)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/eventb-to-txt.svg)](https://pypi.python.org/pypi/eventb-to-txt/)
+[![PyPI version](https://badge.fury.io/py/eventb-to-txt.svg)](https://badge.fury.io/py/eventb-to-txt)
+
+# Event-B to txt converter
+The eventb-to-txt script simply converts Event-B machines and contexts (.bum and .buc files) to the plain text. This text itself is a valid Event-B model that can be used in the CamilleX editor.
+
+Compatible with Event-B models created with Rodin 3.0 and above.
+
+## Installation
+```
+    $ python3 -m pip install eventb-to-txt
+```
+
+## Usage
+```
+    usage: eventb-to-txt [-h] [-o PATH] [-m] [in_path]
+
+    positional arguments:
+    in_path              path to the Event-B model directory or zipfile
+
+    optional arguments:
+    -h, --help           show this help message and exit
+    -o PATH, --out PATH  PATH to the output directory
+    -m, --merge          merge all generated txt files into a single txt file
+```
```

### Comparing `eventb-to-txt-1.4/README.md` & `eventb-to-txt-1.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 ![test](https://github.com/17451k/eventb-to-txt/workflows/test/badge.svg)
-[![Coverage Status](https://coveralls.io/repos/github/17451k/eventb-to-txt/badge.svg?branch=master)](https://coveralls.io/github/17451k/eventb-to-txt?branch=master)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/eventb-to-txt.svg)](https://pypi.python.org/pypi/eventb-to-txt/)
 [![PyPI version](https://badge.fury.io/py/eventb-to-txt.svg)](https://badge.fury.io/py/eventb-to-txt)
 
 # Event-B to txt converter
 The eventb-to-txt script simply converts Event-B machines and contexts (.bum and .buc files) to the plain text. This text itself is a valid Event-B model that can be used in the CamilleX editor.
 
 Compatible with Event-B models created with Rodin 3.0 and above.
```

### Comparing `eventb-to-txt-1.4/eventb_to_txt/__main__.py` & `eventb-to-txt-1.5/eventb_to_txt/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,18 +24,24 @@
                         dest="in_path", nargs=argparse.OPTIONAL, default=os.getcwd())
 
     args = parser.parse_args(args)
 
     if not os.path.exists(args.in_path):
         sys.exit('{!r} path does not exist'.format(args.in_path))
 
-    try:
-        os.makedirs(args.out_path, exist_ok=True)
-    except (OSError, PermissionError, TypeError, AttributeError) as e:
-        sys.exit("{}: Can't create output directory {!r}".format(type(e).__name__, args.out_path))
+    if args.out_path == '-':
+        args.merge = True
+    else:
+        try:
+            os.makedirs(args.out_path, exist_ok=True)
+        except (OSError, PermissionError, TypeError, AttributeError) as e:
+            sys.exit("{}: Can't create output directory {!r}".format(type(e).__name__, args.out_path))
+
+    if os.path.isfile(args.in_path):
+        args.merge = False
 
     is_zipfile = False
     if zipfile.is_zipfile(args.in_path):
         is_zipfile = True
 
         tmp_in = tempfile.mkdtemp()
 
@@ -52,12 +58,13 @@
         raise SystemExit(e)
     except (OSError, PermissionError) as e:
         raise SystemExit("{}: {}".format(type(e).__name__, e))
 
     if is_zipfile:
         shutil.rmtree(args.in_path)
 
-    print('Txt files were successfully generated')
+    if args.out_path != '-':
+        print('Txt files were successfully generated')
 
 
 if __name__ == '__main__':
     main(sys.argv[1:])
```

### Comparing `eventb-to-txt-1.4/eventb_to_txt/abstract.py` & `eventb-to-txt-1.5/eventb_to_txt/abstract.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,27 +22,25 @@
     def __init__(self, component):
         self.path = component
         self.head = {'name': os.path.basename(os.path.splitext(self.path)[0])}
 
     def get_component_name(self):
         return self.head['name']
 
-    def _print_comment(self, data, f):
+    def _to_str_comment(self, data):
+        res = ''
         if data.get('comment'):
             if data['comment'].strip():
-                f.write(' // ')
+                res += ' // '
                 comment = data['comment'].replace('\r\n', '\n')
                 comment = comment.replace('\n', ' ')
-                f.write(comment)
+                res += comment
             else:
                 comment = data['comment'].replace('\r\n', '\n')
-                f.write(comment)
+                res += comment
 
-        f.write('\n')
+        res += '\n'
+        return res
 
-    def _post_process_file(self, path):
+    def _post_process_str(self, string):
         # trim trailing whitespaces
-        lines = ''.join([line.rstrip() + '\n' for line in open(path).readlines()])
-
-        # save file with LF line endings
-        with io.open(path, 'w', newline='\n') as f:
-            f.writelines(lines)
+        return ''.join([line.rstrip() + '\n' for line in string.splitlines()])
```

### Comparing `eventb-to-txt-1.4/eventb_to_txt/context.py` & `eventb-to-txt-1.5/eventb_to_txt/context.py`

 * *Files 22% similar despite different names*

```diff
@@ -67,85 +67,70 @@
         if self.THEOREM in attrs:
             axiom['theorem'] = attrs[self.THEOREM]
         if self.COMMENT in attrs:
             axiom['comment'] = attrs[self.COMMENT]
 
         self.axioms.append(axiom)
 
+    def __str__(self):
+        res = (self.__to_str_context_head() +
+               self.__to_str_sets() +
+               self.__to_str_constants() +
+               self.__to_str_axioms() +
+               'end\n')
+        return self._post_process_str(res)
+
     def to_txt(self, out_path, merge=False):
         exists = os.path.exists(out_path)
 
         with open(out_path, 'a', encoding="utf8") as f:
             if merge and exists:
                 f.write('\n\n')
 
-            self.__print_context_head(f)
-            self.__print_sets(f)
-            self.__print_constants(f)
-            self.__print_axioms(f)
-
-            f.write('end\n')
-
-        self._post_process_file(out_path)
+            f.write(str(self))
 
-    def __print_context_head(self, f):
-        f.write('context ' + self.get_component_name())
-
-        self._print_comment(self.head, f)
+    def __to_str_context_head(self):
+        res = ('context ' + self.get_component_name() +
+               self._to_str_comment(self.head))
 
         if self.extends:
-            f.write(self.TAB + 'extends')
-
-            for extenders in self.extends:
-                f.write(' ' + extenders)
-
-            f.write('\n')
+            res += self.TAB + 'extends ' + ' '.join(self.extends) + '\n'
 
-        f.write('\n')
+        res += '\n'
+        return res
 
-    def __print_sets(self, f):
+    def __to_str_sets(self):
         if not self.sets:
-            return
+            return ''
 
-        f.write('sets\n')
+        pr_line = lambda x: self.TAB + x['id'] + self._to_str_comment(x)
+        return 'sets\n' + ''.join(map(pr_line, self.sets)) + '\n'
 
-        for st in self.sets:
-            f.write(self.TAB + st['id'])
-
-            self._print_comment(st, f)
-        f.write('\n')
-
-    def __print_constants(self, f):
+    def __to_str_constants(self):
         if not self.constants:
-            return
-
-        f.write('constants\n')
+            return ''
 
-        for const in self.constants:
-            f.write(self.TAB + const['id'])
+        pr_line = lambda x: self.TAB + x['id'] + self._to_str_comment(x)
+        return 'constants\n' + ''.join(map(pr_line, self.constants)) + '\n'
 
-            self._print_comment(const, f)
-        f.write('\n')
-
-    def __print_axioms(self, f):
+    def __to_str_axioms(self):
         if not self.axioms:
-            return
-
-        f.write('axioms\n')
+            return ''
 
-        for axiom in self.axioms:
-            self.__print_axiom(axiom, f)
-        f.write('\n')
+        return ('axioms\n' +
+                ''.join(map(lambda x: self.__to_str_axiom(x),
+                            self.axioms)) +
+                '\n')
 
-    def __print_axiom(self, axiom, f):
+    def __to_str_axiom(self, axiom):
         predicate = axiom['predicate'].replace('\r\n', '\n')
         predicate = predicate.replace('\n', '\n' + self.TAB * 2)
         predicate = predicate.replace('\t', self.TAB)
 
-        f.write(self.TAB)
+        res = self.TAB
 
         if 'theorem' in axiom:
-            f.write('theorem ')
-
-        f.write('@' + axiom['label'] + ':\n' + self.TAB * 2 + predicate)
+            res += 'theorem '
 
-        self._print_comment(axiom, f)
+        res += ('@' + axiom['label'] + ':\n' + self.TAB * 2 + predicate)
+        res += self._to_str_comment(axiom)
+        return res
```

### Comparing `eventb-to-txt-1.4/eventb_to_txt/machine.py` & `eventb-to-txt-1.5/eventb_to_txt/machine.py`

 * *Files 24% similar despite different names*

```diff
@@ -173,200 +173,184 @@
             action['comment'] = attrs[self.COMMENT]
 
         if 'actions' not in event:
             event['actions'] = []
 
         event['actions'].append(action)
 
+    def __str__(self):
+        res = (self.__to_str_machine_head() +
+               self.__to_str_variables() +
+               self.__to_str_invariants() +
+               self.__to_str_variant() +
+               self.__to_str_events() +
+               'end\n')
+        return self._post_process_str(res)
+
     def to_txt(self, out_path, merge=False):
         exists = os.path.exists(out_path)
 
         with open(out_path, 'a', encoding="utf8") as f:
             if merge and exists:
                 f.write('\n\n')
 
-            self.__print_machine_head(f)
-            self.__print_variables(f)
-            self.__print_invariants(f)
-            self.__print_variant(f)
-            self.__print_events(f)
-
-            f.write('end\n')
-
-        self._post_process_file(out_path)
+            f.write(str(self))
 
-    def __print_machine_head(self, f):
-        f.write('machine ' + self.get_component_name())
-
-        self._print_comment(self.head, f)
+    def __to_str_machine_head(self):
+        res = ('machine ' + self.get_component_name() +
+               self._to_str_comment(self.head))
 
         if self.refines:
-            f.write(self.TAB + 'refines ' + self.refines + '\n')
+            res += self.TAB + 'refines ' + self.refines + '\n'
 
         if self.sees:
-            f.write(self.TAB + 'sees')
-
-            for seers in self.sees:
-                f.write(' ' + seers)
+            res += self.TAB + 'sees ' + ' '.join(self.sees) + '\n'
 
-            f.write('\n')
+        res += '\n'
+        return res
 
-        f.write('\n')
-
-    def __print_variables(self, f):
+    def __to_str_variables(self):
         if not self.variables:
-            return
-
-        f.write('variables' + '\n')
-
-        for var in self.variables:
-            f.write(self.TAB + var['id'])
+            return ''
 
-            self._print_comment(var, f)
+        pr_line = lambda x: self.TAB + x['id'] + self._to_str_comment(x)
+        return ('variables\n' +
+                ''.join(map(pr_line, self.variables)) + '\n')
 
-        f.write('\n')
-
-    def __print_invariants(self, f):
+    def __to_str_invariants(self):
         if not self.invariants:
-            return
-
-        f.write('invariants' + '\n')
+            return ''
 
-        for inv in self.invariants:
-            self.__print_invariant(inv, f)
+        return ('invariants\n' +
+                ''.join(map(lambda x: self.__to_str_invariant(x),
+                            self.invariants)) + '\n')
 
-        f.write('\n')
-
-    def __print_invariant(self, inv, f):
+    def __to_str_invariant(self, inv):
         predicate = inv['predicate'].replace('\r\n', '\n')
         predicate = predicate.replace('\n', '\n' + self.TAB * 2)
         predicate = predicate.replace('\t', self.TAB)
 
-        f.write(self.TAB)
+        res = self.TAB
 
         if 'theorem' in inv:
-            f.write('theorem ')
-
-        f.write('@' + inv['label'] + ':\n' + self.TAB * 2 + predicate)
+            res += 'theorem '
 
-        self._print_comment(inv, f)
+        res += '@' + inv['label'] + ':\n' + self.TAB * 2 + predicate
+        res += self._to_str_comment(inv)
+        return res
 
-    def __print_variant(self, f):
+    def __to_str_variant(self):
         if not self.variant:
-            return
-
-        f.write('variant\n')
-        f.write(self.TAB + self.variant["expression"])
+            return ''
 
-        self._print_comment(self.variant, f)
+        return ('variant\n' +
+                self.TAB + self.variant["expression"] +
+                self._to_str_comment(self.variant) + '\n')
 
-        f.write('\n')
-
-    def __print_events(self, f):
+    def __to_str_events(self):
         if not self.events:
-            return
-
-        f.write('events' + '\n')
+            return ''
 
-        for event in self.events:
-            self.__print_event(event, f)
+        return ('events\n' +
+                ''.join(map(lambda x: self.__to_str_event(x),
+                            self.events)))
 
-    def __print_event(self, event, f):
-        self.__print_event_head(event, f)
+    def __to_str_event(self, event):
+        res = self.__to_str_event_head(event)
 
         if 'parameters' in event:
-            f.write(self.TAB + self.HALFTAB + 'any\n')
-
-            for param in event['parameters']:
-                f.write(self.TAB * 2 + param['id'])
-
-                self._print_comment(param, f)
+            res += (self.TAB + self.HALFTAB + 'any\n' +
+                    ''.join(map(lambda x:
+                                self.TAB * 2 + x['id'] + self._to_str_comment(x),
+                                event['parameters'])))
 
         if 'guards' in event:
-            f.write(self.TAB + self.HALFTAB + 'where\n')
-
-            for guard in event['guards']:
-                self.__print_guard(guard, f)
+            res += (self.TAB + self.HALFTAB + 'where\n' +
+                    ''.join(map(lambda x: self.__to_str_guard(x),
+                                event['guards'])))
 
         if 'witnesses' in event:
-            f.write(self.TAB + self.HALFTAB + 'with\n')
-
-            for witness in event['witnesses']:
-                self.__print_witness(witness, f)
+            res += (self.TAB + self.HALFTAB + 'with\n' +
+                    ''.join(map(lambda x: self.__to_str_witness(x),
+                                event['witnesses'])))
 
         if 'actions' in event:
-            f.write(self.TAB + self.HALFTAB + 'then\n')
-
-            for action in event['actions']:
-                self.__print_action(action, f)
+            res += (self.TAB + self.HALFTAB + 'then\n' +
+                    ''.join(map(lambda x: self.__to_str_action(x),
+                                event['actions'])))
 
-        f.write(self.TAB + 'end\n\n')
+        res += self.TAB + 'end\n\n'
+        return res
 
-    def __print_event_head(self, event, f):
-        f.write(self.TAB)
+    def __to_str_event_head(self, event):
+        res = self.TAB
 
         if event['convergence'] == '1':
-            f.write("convergent ")
+            res += "convergent "
         elif event['convergence'] == '2':
-            f.write("anticipated ")
+            res += "anticipated "
 
-        f.write('event ' + event['label'])
+        res += 'event ' + event['label']
 
         if 'refines' in event:
             if event['extended'] == 'true':
-                f.write(' extends ' + event['refines'])
+                res += ' extends ' + event['refines']
             else:
-                f.write(' refines ' + event['refines'])
+                res += ' refines ' + event['refines']
         else:
             if event['extended'] == 'true':
-                f.write(' extends ' + event['label'])
+                res += ' extends ' + event['label']
 
-        self._print_comment(event, f)
+        res += self._to_str_comment(event)
+        return res
 
-    def __print_guard(self, guard, f):
-        f.write(self.TAB * 2)
+    def __to_str_guard(self, guard):
+        res = self.TAB * 2
 
         if 'theorem' in guard:
-            f.write('theorem ')
+            res += 'theorem '
 
-        f.write('@' + guard['label'] + ': ')
+        res += '@' + guard['label'] + ': '
 
         additional_tab = len(guard['label']) + 2
         if 'theorem' in guard:
             additional_tab += len('theorem ')
 
         replacement = '\n' + self.TAB * 2 + ' ' * additional_tab
         predicate = guard['predicate'].replace('\r\n', '\n')
         predicate = predicate.replace('\n', replacement)
         predicate = predicate.replace('\t', self.TAB)
 
-        f.write(predicate)
+        res += predicate
 
-        self._print_comment(guard, f)
+        res += self._to_str_comment(guard)
+        return res
 
-    def __print_witness(self, witness, f):
-        f.write(self.TAB * 2 + '@' + witness['label'] + ': ')
+    def __to_str_witness(self, witness):
+        res = self.TAB * 2 + '@' + witness['label'] + ': '
 
         additional_tab = len(witness['label']) + 2
 
         replacement = '\n' + self.TAB * 2 + ' ' * additional_tab
         predicate = witness['predicate'].replace('\r\n', '\n')
         predicate = predicate.replace('\n', replacement)
         predicate = predicate.replace('\t', self.TAB)
 
-        f.write(predicate)
+        res += predicate
 
-        self._print_comment(witness, f)
+        res += self._to_str_comment(witness)
+        return res
 
-    def __print_action(self, action, f):
-        f.write(self.TAB * 2 + '@' + action['label'] + ': ')
+    def __to_str_action(self, action):
+        res = self.TAB * 2 + '@' + action['label'] + ': '
 
         additional_tab = len(action['label']) + 2
 
         replacement = '\n' + self.TAB * 2 + ' ' * additional_tab
         assignment = action['assignment'].replace('\r\n', '\n')
         assignment = assignment.replace('\n', replacement)
         assignment = assignment.replace('\t', self.TAB)
 
-        f.write(assignment)
+        res += assignment
 
-        self._print_comment(action, f)
+        res += self._to_str_comment(action)
+        return res
```

### Comparing `eventb-to-txt-1.4/eventb_to_txt/model.py` & `eventb-to-txt-1.5/eventb_to_txt/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,31 +8,44 @@
 
 from eventb_to_txt.context import Context
 from eventb_to_txt.machine import Machine
 
 
 class Model():
     def __init__(self, model_path):
-        context_files = self.__find_context_files(model_path)
-        machine_files = self.__find_machine_files(model_path)
+        context_files = []
+        machine_files = []
+
+        if os.path.isdir(model_path):
+            context_files = self.__find_context_files(model_path)
+            machine_files = self.__find_machine_files(model_path)
+        elif os.path.isfile(model_path):
+            if model_path.endswith('.buc'):
+                context_files = [model_path]
+            elif model_path.endswith('.bum'):
+                machine_files = [model_path]
 
         if not context_files and not machine_files:
             raise RuntimeError('It seems that the specified directory does not contain any Event-B models')
 
         self.model_objs = self.__parse_model(context_files, machine_files)
 
     @staticmethod
     def find_model_paths(in_path):
         model_paths = set()
 
-        for path in Model.__find_context_files(in_path):
-            model_paths.add(os.path.dirname(path))
-
-        for path in Model.__find_machine_files(in_path):
-            model_paths.add(os.path.dirname(path))
+        if os.path.isdir(in_path):
+            for path in Model.__find_context_files(in_path):
+                model_paths.add(os.path.dirname(path))
+
+            for path in Model.__find_machine_files(in_path):
+                model_paths.add(os.path.dirname(path))
+        elif os.path.isfile(in_path):
+            if in_path.endswith('.buc') or in_path.endswith('.bum'):
+                model_paths.add(in_path)
 
         if not model_paths:
             raise RuntimeError('It seems that the specified directory does not contain any Event-B models')
 
         return model_paths
 
     @staticmethod
@@ -129,14 +142,19 @@
         txt_hash = dict()
 
         if merge:
             queue = self.__get_print_queue()
         else:
             queue = self.model_objs
 
+        if out_path == '-':
+            for el in queue:
+                print(el, end='')
+            return
+
         for el in queue:
             if merge:
                 model_name = os.path.basename(os.path.dirname(el.path))
 
                 txt_hash[el] = os.path.join(out_path, model_name + ".txt")
             else:
                 txt_hash[el] = os.path.join(out_path, el.get_component_name() + ".txt")
```

### Comparing `eventb-to-txt-1.4/eventb_to_txt.egg-info/PKG-INFO` & `eventb-to-txt-1.5/eventb_to_txt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: eventb-to-txt
-Version: 1.4
+Version: 1.5
 Summary: Event-B to txt converter
 Home-page: https://github.com/17451k/eventb-to-txt
 Author: Ilya Shchepetkov
 Author-email: ilya.shchepetkov@yandex.ru
 License: LICENSE.txt
-Description: ![test](https://github.com/17451k/eventb-to-txt/workflows/test/badge.svg)
-        [![Coverage Status](https://coveralls.io/repos/github/17451k/eventb-to-txt/badge.svg?branch=master)](https://coveralls.io/github/17451k/eventb-to-txt?branch=master)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/eventb-to-txt.svg)](https://pypi.python.org/pypi/eventb-to-txt/)
-        [![PyPI version](https://badge.fury.io/py/eventb-to-txt.svg)](https://badge.fury.io/py/eventb-to-txt)
-        
-        # Event-B to txt converter
-        The eventb-to-txt script simply converts Event-B machines and contexts (.bum and .buc files) to the plain text. This text itself is a valid Event-B model that can be used in the CamilleX editor.
-        
-        Compatible with Event-B models created with Rodin 3.0 and above.
-        
-        ## Installation
-        ```
-            $ python3 -m pip install eventb-to-txt
-        ```
-        
-        ## Usage
-        ```
-            usage: eventb-to-txt [-h] [-o PATH] [-m] [in_path]
-        
-            positional arguments:
-            in_path              path to the Event-B model directory or zipfile
-        
-            optional arguments:
-            -h, --help           show this help message and exit
-            -o PATH, --out PATH  PATH to the output directory
-            -m, --merge          merge all generated txt files into a single txt file
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![test](https://github.com/17451k/eventb-to-txt/workflows/test/badge.svg)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/eventb-to-txt.svg)](https://pypi.python.org/pypi/eventb-to-txt/)
+[![PyPI version](https://badge.fury.io/py/eventb-to-txt.svg)](https://badge.fury.io/py/eventb-to-txt)
+
+# Event-B to txt converter
+The eventb-to-txt script simply converts Event-B machines and contexts (.bum and .buc files) to the plain text. This text itself is a valid Event-B model that can be used in the CamilleX editor.
+
+Compatible with Event-B models created with Rodin 3.0 and above.
+
+## Installation
+```
+    $ python3 -m pip install eventb-to-txt
+```
+
+## Usage
+```
+    usage: eventb-to-txt [-h] [-o PATH] [-m] [in_path]
+
+    positional arguments:
+    in_path              path to the Event-B model directory or zipfile
+
+    optional arguments:
+    -h, --help           show this help message and exit
+    -o PATH, --out PATH  PATH to the output directory
+    -m, --merge          merge all generated txt files into a single txt file
+```
```

### Comparing `eventb-to-txt-1.4/setup.py` & `eventb-to-txt-1.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Use of this source code is governed by the MIT license that can be
 # found in the LICENSE file.
 
 import setuptools
 
 setuptools.setup(
     name='eventb-to-txt',
-    version='1.4',
+    version='1.5',
     author='Ilya Shchepetkov',
     author_email='ilya.shchepetkov@yandex.ru',
     license='LICENSE.txt',
     description="Event-B to txt converter",
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     python_requires=">=3.5",
@@ -23,13 +23,14 @@
     },
     classifiers=(
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: Implementation :: CPython",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X"
     )
 )
```

