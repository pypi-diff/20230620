# Comparing `tmp/delvewheel-1.3.7.tar.gz` & `tmp/delvewheel-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delvewheel-1.3.7.tar", last modified: Tue May 16 15:22:27 2023, max compression
+gzip compressed data, was "delvewheel-1.3.8.tar", last modified: Tue Jun 20 13:56:33 2023, max compression
```

## Comparing `delvewheel-1.3.7.tar` & `delvewheel-1.3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 15:22:27.239392 delvewheel-1.3.7/
--rw-rw-rw-   0        0        0     1073 2023-05-16 15:21:43.000000 delvewheel-1.3.7/LICENSE
--rw-rw-rw-   0        0        0    10414 2023-05-16 15:22:27.239392 delvewheel-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     9294 2023-05-16 15:21:43.000000 delvewheel-1.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 15:22:27.239392 delvewheel-1.3.7/delvewheel/
--rw-rw-rw-   0        0        0        0 2023-05-16 15:21:43.000000 delvewheel-1.3.7/delvewheel/__init__.py
--rw-rw-rw-   0        0        0     5169 2023-05-16 15:21:43.000000 delvewheel-1.3.7/delvewheel/__main__.py
--rw-rw-rw-   0        0        0   138609 2023-05-16 15:21:43.000000 delvewheel-1.3.7/delvewheel/_dll_list.py
--rw-rw-rw-   0        0        0    32890 2023-05-16 15:21:43.000000 delvewheel-1.3.7/delvewheel/_dll_utils.py
--rw-rw-rw-   0        0        0       23 2023-05-16 15:21:43.000000 delvewheel-1.3.7/delvewheel/_version.py
--rw-rw-rw-   0        0        0    38757 2023-05-16 15:21:43.000000 delvewheel-1.3.7/delvewheel/_wheel_repair.py
-drwxrwxrwx   0        0        0        0 2023-05-16 15:22:27.239392 delvewheel-1.3.7/delvewheel.egg-info/
--rw-rw-rw-   0        0        0    10414 2023-05-16 15:22:27.000000 delvewheel-1.3.7/delvewheel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-05-16 15:22:27.000000 delvewheel-1.3.7/delvewheel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 15:22:27.000000 delvewheel-1.3.7/delvewheel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-16 15:22:27.000000 delvewheel-1.3.7/delvewheel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 15:22:27.000000 delvewheel-1.3.7/delvewheel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 15:22:27.000000 delvewheel-1.3.7/delvewheel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2023-05-16 15:21:43.000000 delvewheel-1.3.7/pyproject.toml
--rw-rw-rw-   0        0        0     1214 2023-05-16 15:22:27.239392 delvewheel-1.3.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 13:56:33.017228 delvewheel-1.3.8/
+-rw-rw-rw-   0        0        0     1073 2023-06-20 13:55:53.000000 delvewheel-1.3.8/LICENSE
+-rw-rw-rw-   0        0        0    10414 2023-06-20 13:56:33.017228 delvewheel-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9294 2023-06-20 13:55:53.000000 delvewheel-1.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 13:56:33.017228 delvewheel-1.3.8/delvewheel/
+-rw-rw-rw-   0        0        0        0 2023-06-20 13:55:53.000000 delvewheel-1.3.8/delvewheel/__init__.py
+-rw-rw-rw-   0        0        0     5156 2023-06-20 13:55:53.000000 delvewheel-1.3.8/delvewheel/__main__.py
+-rw-rw-rw-   0        0        0   139059 2023-06-20 13:55:53.000000 delvewheel-1.3.8/delvewheel/_dll_list.py
+-rw-rw-rw-   0        0        0    33153 2023-06-20 13:55:53.000000 delvewheel-1.3.8/delvewheel/_dll_utils.py
+-rw-rw-rw-   0        0        0       23 2023-06-20 13:55:53.000000 delvewheel-1.3.8/delvewheel/_version.py
+-rw-rw-rw-   0        0        0    38741 2023-06-20 13:55:53.000000 delvewheel-1.3.8/delvewheel/_wheel_repair.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:56:33.017228 delvewheel-1.3.8/delvewheel.egg-info/
+-rw-rw-rw-   0        0        0    10414 2023-06-20 13:56:33.000000 delvewheel-1.3.8/delvewheel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-06-20 13:56:33.000000 delvewheel-1.3.8/delvewheel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:56:33.000000 delvewheel-1.3.8/delvewheel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-20 13:56:33.000000 delvewheel-1.3.8/delvewheel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-06-20 13:56:33.000000 delvewheel-1.3.8/delvewheel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-20 13:56:33.000000 delvewheel-1.3.8/delvewheel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2023-06-20 13:55:53.000000 delvewheel-1.3.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1214 2023-06-20 13:56:33.017228 delvewheel-1.3.8/setup.cfg
```

### Comparing `delvewheel-1.3.7/LICENSE` & `delvewheel-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `delvewheel-1.3.7/PKG-INFO` & `delvewheel-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delvewheel
-Version: 1.3.7
+Version: 1.3.8
 Summary: Self-contained wheels for Windows
 Home-page: https://github.com/adang1345/delvewheel
 Author: Aohan Dang
 Author-email: adang1345@gmail.com
 License: MIT
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `delvewheel-1.3.7/README.md` & `delvewheel-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `delvewheel-1.3.7/delvewheel/__main__.py` & `delvewheel-1.3.8/delvewheel/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,13 +68,13 @@
             wr = WheelRepair(wheel, args.extract_dir, add_dlls, no_dlls, args.ignore_in_wheel, args.v, args.test.split(','))
             if args.command == 'show':
                 wr.show()
             else:  # args.command == 'repair'
                 no_mangles = set(dll_name.lower() for dll_name in args.no_mangle.split(os.pathsep) if dll_name)
                 wr.repair(args.target, no_mangles, args.no_mangle_all, args.strip, args.lib_sdir, args.no_diagnostic)
     else:  # args.command == 'needed'
-        for dll_name in sorted(_dll_utils.get_direct_needed(args.file, True, False, args.v), key=str.lower):
+        for dll_name in sorted(_dll_utils.get_direct_needed(args.file, args.v), key=str.lower):
             print(dll_name)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `delvewheel-1.3.7/delvewheel/_dll_list.py` & `delvewheel-1.3.8/delvewheel/_dll_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,24 @@
     'cp311-win_amd64': {'vcruntime140.dll', 'vcruntime140_1.dll'},
     'cp311-win_arm64': {'vcruntime140.dll', 'vcruntime140_1.dll'},
     'cp312-win32': {'vcruntime140.dll'},
     'cp312-win_amd64': {'vcruntime140.dll', 'vcruntime140_1.dll'},
     'cp312-win_arm64': {'vcruntime140.dll', 'vcruntime140_1.dll'},
 }
 
+# Dependency relationships to ignore.
+ignore_dependency = {
+    # Some versions of msvcp140.dll have a delay-load dependency on
+    # concrt140.dll, apparently to support Windows XP
+    # (https://learn.microsoft.com/en-us/cpp/parallel/concrt/overview-of-the-concurrency-runtime?view=msvc-170#dlls).
+    # This dependency is unnecessary for our purposes because we target Windows
+    # 7 or higher.
+    'msvcp140.dll': {'concrt140.dll'}
+}
+
 # Set of regular expressions of DLLs whose names should not be mangled.
 no_mangle_regexes = {}
 
 # ignore_names_x86 is a set containing the lowercase names of all DLLs that can
 # be assumed to be present on 32-bit x86 Windows 7 SP1 or later. These are all
 # the files with extension .dll or .drv found in C:\Windows\SysWOW64 on vanilla
 # installations of Windows 7 SP1 x64, 8 x64, 8.1 x64, 10 x64, 10 arm64, 11 x64,
```

### Comparing `delvewheel-1.3.7/delvewheel/_dll_utils.py` & `delvewheel-1.3.8/delvewheel/_dll_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,38 +242,29 @@
             if name == item.lower():
                 path = os.path.join(directory, item)
                 if os.path.isfile(path) and get_arch(path) == arch:
                     return path
     return None
 
 
-def get_direct_needed(lib_path: str, include_delay_imports: bool, lower: bool, verbose: int) -> set:
+def get_direct_needed(lib_path: str, verbose: int) -> set:
     """Given the path to a shared library, return a set containing the DLL
-    names of all its direct dependencies.
-
-    If include_delay_imports is True, delay-loaded dependencies are included.
-    Otherwise, they are not included.
-
-    If lower is True, the DLL names are all lowercase. Otherwise, they are in
-    the original case."""
+    names of all its direct dependencies. Regular and delay-load dependencies
+    are included. The DLL names are in the original case."""
     with PEContext(lib_path, None, True, verbose) as pe:
         imports = []
-        if include_delay_imports:
-            attrs = ('DIRECTORY_ENTRY_IMPORT', 'DIRECTORY_ENTRY_DELAY_IMPORT')
-        else:
-            attrs = ('DIRECTORY_ENTRY_IMPORT',)
-        for attr in attrs:
+        for attr in ('DIRECTORY_ENTRY_IMPORT', 'DIRECTORY_ENTRY_DELAY_IMPORT'):
             if hasattr(pe, attr):
                 imports = itertools.chain(imports, getattr(pe, attr))
+        lib_name_lower = os.path.basename(lib_path).lower()
         needed = set()
         for entry in imports:
             name = entry.dll.decode('utf-8')
-            if lower:
-                name = name.lower()
-            needed.add(name)
+            if lib_name_lower not in _dll_list.ignore_dependency or name.lower() not in _dll_list.ignore_dependency[lib_name_lower]:
+                needed.add(name)
     return needed
 
 
 def get_direct_mangleable_needed(lib_path: str, no_dlls: set, no_mangles: set, verbose: int) -> list:
     """Given the path to a shared library, return a deterministically-ordered
     list containing the lowercase DLL names of all direct dependencies that
     belong in the wheel and should be name-mangled.
@@ -288,20 +279,22 @@
             if hasattr(pe, attr):
                 imports = itertools.chain(imports, getattr(pe, attr))
         needed = []
         lib_arch = MachineType.machine_field_to_type(pe.FILE_HEADER.Machine)
         if not lib_arch:
             raise ValueError(f'{lib_path} has an unsupported CPU architecture')
         ignore_names = _dll_list.ignore_names[lib_arch]
+        lib_name_lower = os.path.basename(lib_path).lower()
         for entry in imports:
             dll_name = entry.dll.decode('utf-8').lower()
             if dll_name not in ignore_names and \
                     dll_name not in no_dlls and \
                     not any(r.fullmatch(dll_name) for r in _dll_list.ignore_regexes) and \
                     dll_name not in no_mangles and \
+                    (lib_name_lower not in _dll_list.ignore_dependency or dll_name not in _dll_list.ignore_dependency[lib_name_lower]) and \
                     not any(r.fullmatch(dll_name) for r in _dll_list.no_mangle_regexes):
                 needed.append(dll_name)
     return needed
 
 
 def get_all_needed(lib_path: str,
                    no_dlls: set,
@@ -340,19 +333,21 @@
                 for attr in ('DIRECTORY_ENTRY_IMPORT', 'DIRECTORY_ENTRY_DELAY_IMPORT'):
                     if hasattr(pe, attr):
                         imports = itertools.chain(imports, getattr(pe, attr))
                 lib_arch = MachineType.machine_field_to_type(pe.FILE_HEADER.Machine)
                 if not lib_arch:
                     raise ValueError(f'{lib_path} has an unsupported CPU architecture')
                 ignore_names = _dll_list.ignore_names[lib_arch]
+                lib_name_lower = os.path.basename(lib_path).lower()
                 for entry in imports:
                     dll_name = entry.dll.decode('utf-8').lower()
                     if dll_name not in ignore_names and \
                             not any(r.fullmatch(dll_name) for r in _dll_list.ignore_regexes) and \
-                            dll_name not in no_dlls:
+                            dll_name not in no_dlls and \
+                            (lib_name_lower not in _dll_list.ignore_dependency or dll_name not in _dll_list.ignore_dependency[lib_name_lower]):
                         dll_path = find_library(dll_name, wheel_dirs, lib_arch)
                         if dll_path:
                             stack.append(dll_path)
                         elif on_error == 'raise':
                             raise FileNotFoundError(f'Unable to find library: {dll_name}')
                         else:
                             not_found.add(dll_name)
```

### Comparing `delvewheel-1.3.7/delvewheel/_wheel_repair.py` & `delvewheel-1.3.8/delvewheel/_wheel_repair.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 # 1. an identifying string such as the delvewheel version
 # 2. the name of the directory containing the vendored DLLs
 _patch_init_template_v2 = """
 
 {0}# start delvewheel patch
 def _delvewheel_init_patch_{1}():
     import os
-    import sys
     libs_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, {2!r}))
     if os.path.isdir(libs_dir):
         os.add_dll_directory(libs_dir)
 
 
 _delvewheel_init_patch_{1}()
 del _delvewheel_init_patch_{1}
```

### Comparing `delvewheel-1.3.7/delvewheel.egg-info/PKG-INFO` & `delvewheel-1.3.8/delvewheel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delvewheel
-Version: 1.3.7
+Version: 1.3.8
 Summary: Self-contained wheels for Windows
 Home-page: https://github.com/adang1345/delvewheel
 Author: Aohan Dang
 Author-email: adang1345@gmail.com
 License: MIT
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `delvewheel-1.3.7/setup.cfg` & `delvewheel-1.3.8/setup.cfg`

 * *Files identical despite different names*

