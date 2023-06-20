# Comparing `tmp/wc-shortcodes-0.1.0.tar.gz` & `tmp/wc-shortcodes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-shortcodes-0.1.0.tar", last modified: Sun Feb  6 19:39:27 2022, max compression
+gzip compressed data, was "wc-shortcodes-0.1.1.tar", last modified: Tue Jun 20 13:59:26 2023, max compression
```

## Comparing `wc-shortcodes-0.1.0.tar` & `wc-shortcodes-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-02-06 19:39:27.460142 wc-shortcodes-0.1.0/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      297 2022-02-05 07:48:50.000000 wc-shortcodes-0.1.0/CHANGELOG.md
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1072 2022-02-05 07:48:50.000000 wc-shortcodes-0.1.0/LICENSE
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       88 2022-02-06 19:39:16.000000 wc-shortcodes-0.1.0/MANIFEST.in
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      208 2022-02-06 19:09:43.000000 wc-shortcodes-0.1.0/Makefile
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2801 2022-02-06 19:39:27.460142 wc-shortcodes-0.1.0/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1881 2022-02-06 19:37:34.000000 wc-shortcodes-0.1.0/README.md
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       79 2022-02-06 19:39:27.460142 wc-shortcodes-0.1.0/setup.cfg
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1587 2022-02-06 19:39:01.000000 wc-shortcodes-0.1.0/setup.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      553 2022-02-05 07:48:50.000000 wc-shortcodes-0.1.0/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-02-06 19:39:27.460142 wc-shortcodes-0.1.0/wc_shortcodes/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       63 2022-02-05 07:48:50.000000 wc-shortcodes-0.1.0/wc_shortcodes/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-02-06 19:39:27.460142 wc-shortcodes-0.1.0/wc_shortcodes/contrib/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-02-05 07:48:50.000000 wc-shortcodes-0.1.0/wc_shortcodes/contrib/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-02-06 19:39:27.460142 wc-shortcodes-0.1.0/wc_shortcodes/contrib/django/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2022-02-05 07:48:50.000000 wc-shortcodes-0.1.0/wc_shortcodes/contrib/django/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      283 2022-02-05 07:48:50.000000 wc-shortcodes-0.1.0/wc_shortcodes/contrib/django/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3532 2022-02-06 19:09:30.000000 wc-shortcodes-0.1.0/wc_shortcodes/parser.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1970 2022-02-06 19:34:00.000000 wc-shortcodes-0.1.0/wc_shortcodes/registry.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     7684 2022-02-06 19:33:05.000000 wc-shortcodes-0.1.0/wc_shortcodes/transformer.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2022-02-06 19:39:27.460142 wc-shortcodes-0.1.0/wc_shortcodes.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2801 2022-02-06 19:39:27.000000 wc-shortcodes-0.1.0/wc_shortcodes.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      479 2022-02-06 19:39:27.000000 wc-shortcodes-0.1.0/wc_shortcodes.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2022-02-06 19:39:27.000000 wc-shortcodes-0.1.0/wc_shortcodes.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      148 2022-02-06 19:39:27.000000 wc-shortcodes-0.1.0/wc_shortcodes.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       14 2022-02-06 19:39:27.000000 wc-shortcodes-0.1.0/wc_shortcodes.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-20 13:59:26.894721 wc-shortcodes-0.1.1/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      436 2023-06-20 13:59:06.000000 wc-shortcodes-0.1.1/CHANGELOG.md
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1072 2022-09-20 08:50:23.000000 wc-shortcodes-0.1.1/LICENSE
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)       88 2022-09-20 08:50:23.000000 wc-shortcodes-0.1.1/MANIFEST.in
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      208 2022-09-20 08:50:23.000000 wc-shortcodes-0.1.1/Makefile
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2898 2023-06-20 13:59:26.894721 wc-shortcodes-0.1.1/PKG-INFO
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1878 2022-09-20 08:50:23.000000 wc-shortcodes-0.1.1/README.md
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)       79 2023-06-20 13:59:26.894721 wc-shortcodes-0.1.1/setup.cfg
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1587 2022-09-20 08:50:23.000000 wc-shortcodes-0.1.1/setup.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-20 13:59:26.894721 wc-shortcodes-0.1.1/tests/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     2429 2022-09-20 08:50:23.000000 wc-shortcodes-0.1.1/tests/test_parser.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     1059 2023-06-20 13:55:57.000000 wc-shortcodes-0.1.1/tests/test_registry.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     2930 2023-06-20 13:56:12.000000 wc-shortcodes-0.1.1/tests/test_transformer.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      553 2022-09-20 08:50:23.000000 wc-shortcodes-0.1.1/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-20 13:59:26.894721 wc-shortcodes-0.1.1/wc_shortcodes/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)       63 2023-06-20 13:56:49.000000 wc-shortcodes-0.1.1/wc_shortcodes/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-20 13:59:26.894721 wc-shortcodes-0.1.1/wc_shortcodes/contrib/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-shortcodes-0.1.1/wc_shortcodes/contrib/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-20 13:59:26.894721 wc-shortcodes-0.1.1/wc_shortcodes/contrib/django/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        0 2022-09-20 08:50:23.000000 wc-shortcodes-0.1.1/wc_shortcodes/contrib/django/__init__.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      283 2022-09-20 08:50:23.000000 wc-shortcodes-0.1.1/wc_shortcodes/contrib/django/apps.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     3532 2023-06-20 13:42:13.000000 wc-shortcodes-0.1.1/wc_shortcodes/parser.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     2134 2023-06-20 13:56:03.000000 wc-shortcodes-0.1.1/wc_shortcodes/registry.py
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     7742 2023-06-20 13:48:58.000000 wc-shortcodes-0.1.1/wc_shortcodes/transformer.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-06-20 13:59:26.894721 wc-shortcodes-0.1.1/wc_shortcodes.egg-info/
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)     2898 2023-06-20 13:59:26.000000 wc-shortcodes-0.1.1/wc_shortcodes.egg-info/PKG-INFO
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      549 2023-06-20 13:59:26.000000 wc-shortcodes-0.1.1/wc_shortcodes.egg-info/SOURCES.txt
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)        1 2023-06-20 13:59:26.000000 wc-shortcodes-0.1.1/wc_shortcodes.egg-info/dependency_links.txt
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)      148 2023-06-20 13:59:26.000000 wc-shortcodes-0.1.1/wc_shortcodes.egg-info/requires.txt
+-rwxrwxrwx   0 preusx    (1000) preusx    (1000)       14 2023-06-20 13:59:26.000000 wc-shortcodes-0.1.1/wc_shortcodes.egg-info/top_level.txt
```

### Comparing `wc-shortcodes-0.1.0/LICENSE` & `wc-shortcodes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-shortcodes-0.1.0/PKG-INFO` & `wc-shortcodes-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: wc-shortcodes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple shortcodes resolver utility lib.
-Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,15 +77,15 @@
 This configuration was made for performance reasons.
 
 For example if there is, lets say, 10 same shortcuts with different parameters passed inside one text. It's obvious that whose 10 items will do same work for 10 times. So to prevent such unefficiency multihandlers had been added.
 
 ```python
 @registry.register(multiple=True)
 def shortcode(
-  # They receive all current entities as `*args`.
+  # They receive all current entities as list.
   entities: List[Entity],
   context={}
 ) -> List[str]:
   return [
     # And must return result in the exact same order as they have been passed.
     entity.content for entity in entities
   ]
@@ -112,11 +110,14 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.1]
+### Fixed
+- Empty registry entities matcher finds `''` key. Not anymore.
+- Register code with empty name prohibited since now.
+
 ## [0.1.0]
 Initial version.
-
-
```

### Comparing `wc-shortcodes-0.1.0/README.md` & `wc-shortcodes-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 This configuration was made for performance reasons.
 
 For example if there is, lets say, 10 same shortcuts with different parameters passed inside one text. It's obvious that whose 10 items will do same work for 10 times. So to prevent such unefficiency multihandlers had been added.
 
 ```python
 @registry.register(multiple=True)
 def shortcode(
-  # They receive all current entities as `*args`.
+  # They receive all current entities as list.
   entities: List[Entity],
   context={}
 ) -> List[str]:
   return [
     # And must return result in the exact same order as they have been passed.
     entity.content for entity in entities
   ]
```

### Comparing `wc-shortcodes-0.1.0/setup.py` & `wc-shortcodes-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `wc-shortcodes-0.1.0/tox.ini` & `wc-shortcodes-0.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `wc-shortcodes-0.1.0/wc_shortcodes/parser.py` & `wc-shortcodes-0.1.1/wc_shortcodes/parser.py`

 * *Files identical despite different names*

### Comparing `wc-shortcodes-0.1.0/wc_shortcodes/registry.py` & `wc-shortcodes-0.1.1/wc_shortcodes/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,17 @@
         self,
         name: str,
         resolver: Callable,
         /,
         multiple: bool = False,
         autoresolve_content: bool = True
     ) -> CodeDefinition:
+        assert name != '' and not name.isspace(), 'Code name must not be empty.'
+        assert name != '<lambda>', 'Lambda function should be named to register.'
+
         if self.has(name):
             # TODO: Add own library exceptions.
             raise KeyError(
                 f'Code resolver for "{name}" already registered.\n'
                 'Remove it and only then add a new one.'
             )
```

### Comparing `wc-shortcodes-0.1.0/wc_shortcodes/transformer.py` & `wc-shortcodes-0.1.1/wc_shortcodes/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 
     parts.append(content[start:])
 
     return ''.join(parts)
 
 
 def find_entities(registry: 'CodesRegistry', content: str) -> List[parser.Entity]:
+    if len(registry.definitions) == 0:
+        return []
+
     # TODO: Make api method to get names in registry:
     matches = '|'.join(re.escape(x) for x in registry.definitions.keys())
 
     return parser.find_entities(content, name_regex=f'({matches})')
 
 
 class ResolveState:
```

### Comparing `wc-shortcodes-0.1.0/wc_shortcodes.egg-info/PKG-INFO` & `wc-shortcodes-0.1.1/wc_shortcodes.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: wc-shortcodes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple shortcodes resolver utility lib.
-Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -79,15 +77,15 @@
 This configuration was made for performance reasons.
 
 For example if there is, lets say, 10 same shortcuts with different parameters passed inside one text. It's obvious that whose 10 items will do same work for 10 times. So to prevent such unefficiency multihandlers had been added.
 
 ```python
 @registry.register(multiple=True)
 def shortcode(
-  # They receive all current entities as `*args`.
+  # They receive all current entities as list.
   entities: List[Entity],
   context={}
 ) -> List[str]:
   return [
     # And must return result in the exact same order as they have been passed.
     entity.content for entity in entities
   ]
@@ -112,11 +110,14 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.1]
+### Fixed
+- Empty registry entities matcher finds `''` key. Not anymore.
+- Register code with empty name prohibited since now.
+
 ## [0.1.0]
 Initial version.
-
-
```

