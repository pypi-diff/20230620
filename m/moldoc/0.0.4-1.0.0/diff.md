# Comparing `tmp/moldoc-0.0.4.tar.gz` & `tmp/moldoc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moldoc-0.0.4.tar", last modified: Sat Jun 17 13:36:11 2023, max compression
+gzip compressed data, was "moldoc-1.0.0.tar", last modified: Mon Jun 19 17:00:32 2023, max compression
```

## Comparing `moldoc-0.0.4.tar` & `moldoc-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,49 @@
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-06-17 13:36:11.774025 moldoc-0.0.4/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1053 2023-06-17 13:13:28.000000 moldoc-0.0.4/LICENSE
--rw-r--r--   0 lukas     (1000) lukas     (1000)      210 2023-06-17 13:36:11.774025 moldoc-0.0.4/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5615 2023-06-17 13:13:28.000000 moldoc-0.0.4/README.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2023-06-17 13:36:11.774025 moldoc-0.0.4/setup.cfg
--rw-r--r--   0 lukas     (1000) lukas     (1000)      672 2023-06-17 13:13:28.000000 moldoc-0.0.4/setup.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-06-17 13:36:11.770692 moldoc-0.0.4/src/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-06-17 13:36:11.770692 moldoc-0.0.4/src/moldoc/
--rw-r--r--   0 lukas     (1000) lukas     (1000)       70 2023-06-17 13:28:21.000000 moldoc-0.0.4/src/moldoc/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-06-17 13:36:11.774025 moldoc-0.0.4/src/moldoc/javascript/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      259 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1915 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/atoms.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      386 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/bonds.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)       88 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/bool.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      292 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/color.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4311 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/material.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2793 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/mesh_config.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      930 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/scene_config.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)   351667 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/molDraw.js
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3193 2023-06-17 13:14:12.000000 moldoc-0.0.4/src/moldoc/moldoc.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5409 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/molecule.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)   551410 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/three.min.js
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-06-17 13:36:11.774025 moldoc-0.0.4/src/moldoc.egg-info/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      210 2023-06-17 13:36:11.000000 moldoc-0.0.4/src/moldoc.egg-info/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)      575 2023-06-17 13:36:11.000000 moldoc-0.0.4/src/moldoc.egg-info/SOURCES.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2023-06-17 13:36:11.000000 moldoc-0.0.4/src/moldoc.egg-info/dependency_links.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        7 2023-06-17 13:36:11.000000 moldoc-0.0.4/src/moldoc.egg-info/requires.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        7 2023-06-17 13:36:11.000000 moldoc-0.0.4/src/moldoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:32.473449 moldoc-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:32.457449 moldoc-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:32.465449 moldoc-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-19 17:00:06.000000 moldoc-1.0.0/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-19 17:00:06.000000 moldoc-1.0.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-19 17:00:06.000000 moldoc-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-19 17:00:06.000000 moldoc-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-19 17:00:32.473449 moldoc-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-19 17:00:06.000000 moldoc-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   117976 2023-06-19 17:00:06.000000 moldoc-1.0.0/configuration.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-19 17:00:06.000000 moldoc-1.0.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)  1268442 2023-06-19 17:00:06.000000 moldoc-1.0.0/moldoc.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-19 17:00:06.000000 moldoc-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 17:00:32.473449 moldoc-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:32.457449 moldoc-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:32.465449 moldoc-1.0.0/src/moldoc/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:32.469449 moldoc-1.0.0/src/moldoc/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:32.473449 moldoc-1.0.0/src/moldoc/_internal/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/javascript/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/javascript/bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/javascript/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/javascript/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/javascript/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/javascript/mesh_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/javascript/scene_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   351667 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/molDraw.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/moldoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551410 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/_internal/three.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:06.000000 moldoc-1.0.0/src/moldoc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 17:00:32.000000 moldoc-1.0.0/src/moldoc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:32.469449 moldoc-1.0.0/src/moldoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-19 17:00:32.000000 moldoc-1.0.0/src/moldoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-19 17:00:32.000000 moldoc-1.0.0/src/moldoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:00:32.000000 moldoc-1.0.0/src/moldoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-19 17:00:32.000000 moldoc-1.0.0/src/moldoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 17:00:32.000000 moldoc-1.0.0/src/moldoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:32.473449 moldoc-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-19 17:00:06.000000 moldoc-1.0.0/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-19 17:00:06.000000 moldoc-1.0.0/tests/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:32.473449 moldoc-1.0.0/tests/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:32.473449 moldoc-1.0.0/tests/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 17:00:06.000000 moldoc-1.0.0/tests/source/_static/empty
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-19 17:00:06.000000 moldoc-1.0.0/tests/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-06-19 17:00:06.000000 moldoc-1.0.0/tests/source/index.rst
```

### Comparing `moldoc-0.0.4/LICENSE` & `moldoc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.4/README.rst` & `moldoc-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.4/src/moldoc/javascript/material.py` & `moldoc-1.0.0/src/moldoc/_internal/javascript/material.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,152 +1,131 @@
 from typing import Optional, TypeVar
 
-from .bool import bool_to_javascript
-from ..molecule import (
+from moldoc._internal.javascript.bool import bool_to_javascript
+from moldoc.molecule import (
     Material,
     MeshLambertMaterial,
     MeshNormalMaterial,
     MeshPhongMaterial,
     MeshPhysicalMaterial,
     MeshStandardMaterial,
-    MeshToonMaterial,
 )
 
 
 def material_to_javascript(material: Material) -> str:
-    # This is a type-safe switch
-    return {  # type: ignore
-        MeshLambertMaterial: _lambert_to_javascript,
-        MeshNormalMaterial: _normal_to_javascript,
-        MeshPhongMaterial: _phong_to_javascript,
-        MeshPhysicalMaterial: _physical_to_javascript,
-        MeshStandardMaterial: _standard_to_javascript,
-        MeshToonMaterial: _toon_to_javascript,
-    }[type(material)](material)
+    match material:
+        case MeshLambertMaterial():
+            return (
+                "material:(color)=>"
+                "new THREE.MeshLambertMaterial({color:color})"
+            )
+        case MeshNormalMaterial():
+            return "material:(color)=>new THREE.MeshNormalMaterial()"
+        case MeshPhongMaterial():
+            return _phong_to_javascript(material)
+        case MeshPhysicalMaterial():
+            return _physical_to_javascript(material)
+        case MeshStandardMaterial():
+            return _standard_to_javascript(material)
 
 
-def _lambert_to_javascript(material: MeshLambertMaterial) -> str:
-    return (
-        'material:(color)=>'
-        'new THREE.MeshLambertMaterial({color:color})'
-    )
-
-
-def _normal_to_javascript(material: MeshNormalMaterial) -> str:
-    return 'material:(color)=>new THREE.MeshNormalMaterial()'
-
-
-def _phong_to_javascript(
-    material: MeshPhongMaterial,
-) -> str:
-
+def _phong_to_javascript(material: MeshPhongMaterial) -> str:
     shininess = _property_to_javascript(
-        property_name='shininess',
+        property_name="shininess",
         property_value=material.get_shininess(),
     )
     reflectivity = _property_to_javascript(
-        property_name='reflectivity',
+        property_name="reflectivity",
         property_value=material.get_reflectivity(),
     )
     flat_shading = _property_to_javascript(
-        property_name='flatShading',
+        property_name="flatShading",
         property_value=material.get_flat_shading(),
     )
     return (
-        'material:'
-        '(color)=>new THREE.MeshPhongMaterial({'
-        'color:color'
+        "material:"
+        "(color)=>new THREE.MeshPhongMaterial({"
+        "color:color"
         f'{"," if shininess else ""}{shininess}'
         f'{"," if reflectivity else ""}{reflectivity}'
         f'{"," if flat_shading else ""}{flat_shading}'
-        '})'
+        "})"
     )
 
 
-def _physical_to_javascript(
-    material: MeshPhysicalMaterial,
-) -> str:
+def _physical_to_javascript(material: MeshPhysicalMaterial) -> str:
     clearcoat = _property_to_javascript(
-        property_name='clearcoat',
+        property_name="clearcoat",
         property_value=material.get_clearcoat(),
     )
     clearcoat_roughness = _property_to_javascript(
-        property_name='clearcoat_roughness',
+        property_name="clearcoat_roughness",
         property_value=material.get_clearcoat_roughness(),
     )
     roughness = _property_to_javascript(
-        property_name='roughness',
+        property_name="roughness",
         property_value=material.get_roughness(),
     )
     metalness = _property_to_javascript(
-        property_name='metalness',
+        property_name="metalness",
         property_value=material.get_metalness(),
     )
     reflectivity = _property_to_javascript(
-        property_name='reflectivity',
+        property_name="reflectivity",
         property_value=material.get_reflectivity(),
     )
     flat_shading = _property_to_javascript(
-        property_name='flat_shading',
+        property_name="flat_shading",
         property_value=material.get_flat_shading(),
     )
     return (
-        'material:'
-        '(color)=>new THREE.MeshPhysicalMaterial({'
-        'color:color'
+        "material:"
+        "(color)=>new THREE.MeshPhysicalMaterial({"
+        "color:color"
         f'{"," if clearcoat else ""}{clearcoat}'
         f'{"," if clearcoat_roughness else ""}{clearcoat_roughness}'
         f'{"," if roughness else ""}{roughness}'
         f'{"," if metalness else ""}{metalness}'
         f'{"," if reflectivity else ""}{reflectivity}'
         f'{"," if flat_shading else ""}{flat_shading}'
-        '})'
+        "})"
     )
 
 
-def _standard_to_javascript(
-    material: MeshStandardMaterial,
-) -> str:
+def _standard_to_javascript(material: MeshStandardMaterial) -> str:
     metalness = _property_to_javascript(
-        property_name='metalness',
+        property_name="metalness",
         property_value=material.get_metalness(),
     )
     roughness = _property_to_javascript(
-        property_name='roughness',
+        property_name="roughness",
         property_value=material.get_roughness(),
     )
     flat_shading = _property_to_javascript(
-        property_name='flatShading',
+        property_name="flatShading",
         property_value=material.get_flat_shading(),
     )
     return (
-        'material:'
-        '(color)=>new THREE.MeshStandardMaterial({'
-        'color:color'
+        "material:"
+        "(color)=>new THREE.MeshStandardMaterial({"
+        "color:color"
         f'{"," if metalness else ""}{metalness}'
         f'{"," if roughness else ""}{roughness}'
         f'{"," if flat_shading else ""}{flat_shading}'
-        '})'
+        "})"
     )
 
 
-def _toon_to_javascript(
-    material: MeshToonMaterial,
-) -> str:
-    ...
-
-
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 def _property_to_javascript(
     property_name: str,
     property_value: Optional[T],
 ) -> str:
-
     if property_value is None:
-        return ''
+        return ""
 
     if isinstance(property_value, bool):
-        return f'{property_name}:{bool_to_javascript(property_value)}'
+        return f"{property_name}:{bool_to_javascript(property_value)}"
 
-    return f'{property_name}:{property_value}'
+    return f"{property_name}:{property_value}"
```

### Comparing `moldoc-0.0.4/src/moldoc/javascript/mesh_config.py` & `moldoc-1.0.0/src/moldoc/_internal/javascript/mesh_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from typing import Optional, Iterable
+from typing import Iterable, Optional
 
-from .color import color_to_javascript
-from .material import material_to_javascript
-from ..molecule import Atom, Molecule, MoleculeConfig
+from moldoc._internal.javascript.color import color_to_javascript
+from moldoc._internal.javascript.material import material_to_javascript
+from moldoc.molecule import Atom, Molecule, MoleculeConfig
 
 
 def get_mesh_config(
     molecule: Molecule,
 ) -> str:
-
     mesh_config = []
     atoms = molecule.get_atoms()
 
     atom_size_function = _get_atom_size_function(atoms)
     if atom_size_function is not None:
         mesh_config.append(atom_size_function)
 
@@ -20,89 +19,84 @@
     if atom_color_function is not None:
         mesh_config.append(atom_color_function)
 
     molecule_config = molecule.get_config()
     if molecule_config is not None:
         atom_scale = molecule_config.get_atom_scale()
         if atom_scale is not None:
-            mesh_config.append(f'atomScale:{atom_scale}')
+            mesh_config.append(f"atomScale:{atom_scale}")
 
         material = molecule_config.get_material()
         if material is not None:
             mesh_config.append(material_to_javascript(material))
 
     return ",".join(mesh_config)
 
 
 def _get_atom_size_function(
     atoms: Iterable[Atom],
 ) -> Optional[str]:
-
     atom_size_cases = tuple(_get_atom_size_cases(atoms))
     if atom_size_cases:
         return (
-            'atomSize:atom=>{switch(md.id(atom)){'
+            "atomSize:atom=>{switch(md.id(atom)){"
             f'{"".join(atom_size_cases)}'
-            'default:return md.size(md.chemicalSymbol(atom));'
-            '}}'
+            "default:return md.size(md.chemicalSymbol(atom));"
+            "}}"
         )
 
     return None
 
 
 def _get_atom_size_cases(
     atoms: Iterable[Atom],
 ) -> Iterable[str]:
-
     for atom_id, atom in enumerate(atoms):
         config = atom.get_config()
         if config is not None:
             size = config.get_size()
             if size is not None:
-                yield f'case {atom_id}:return {size};'
+                yield f"case {atom_id}:return {size};"
 
 
 def _get_atom_color_function(
     atoms: Iterable[Atom],
 ) -> Optional[str]:
-
     atom_color_cases = tuple(_get_atom_color_cases(atoms))
     if atom_color_cases:
         return (
-            'atomColor:atom=>{switch(md.id(atom)){'
+            "atomColor:atom=>{switch(md.id(atom)){"
             f'{"".join(atom_color_cases)}'
-            'default:return md.color(md.chemicalSymbol(atom));'
-            '}}'
+            "default:return md.color(md.chemicalSymbol(atom));"
+            "}}"
         )
     return None
 
 
 def _get_atom_color_cases(
     atoms: Iterable[Atom],
 ) -> Iterable[str]:
-
     for atom_id, atom in enumerate(atoms):
         config = atom.get_config()
         if config is not None:
             color = config.get_color()
             if color is not None:
                 color_js = color_to_javascript(color)
-                yield f'case {atom_id}:return {color_js};'
+                yield f"case {atom_id}:return {color_js};"
 
 
 def _molecule_config_to_javascript(
     config: Optional[MoleculeConfig],
 ) -> Optional[str]:
-
     if config is None:
         return None
 
     javascript = []
 
     material = config.get_material()
     if material is not None:
         javascript.append(material_to_javascript(material))
 
     if javascript:
-        return ','.join(javascript)
+        return ",".join(javascript)
 
     return None
```

### Comparing `moldoc-0.0.4/src/moldoc/javascript/scene_config.py` & `moldoc-1.0.0/src/moldoc/_internal/javascript/scene_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 from typing import Optional
 
-from .color import color_to_javascript
-from .bool import bool_to_javascript
-from ..molecule import MoleculeConfig
+from moldoc._internal.javascript.bool import bool_to_javascript
+from moldoc._internal.javascript.color import color_to_javascript
+from moldoc.molecule import MoleculeConfig
 
 
 def get_scene_config(
     container_id: str,
     molecule_config: Optional[MoleculeConfig],
 ) -> str:
-
     scene_config = {
         "containerId": f'"{container_id}"',
-        **_get_scene_config(molecule_config)
+        **_get_scene_config(molecule_config),
     }
 
-    return ",".join(
-        f'{key}:{value}' for key, value in scene_config.items()
-    )
+    return ",".join(f"{key}:{value}" for key, value in scene_config.items())
 
 
-def _get_scene_config(config: Optional[MoleculeConfig]) -> dict:
-    result = {}
+def _get_scene_config(config: Optional[MoleculeConfig]) -> dict[str, str]:
+    result: dict[str, str] = {}
 
     if config is None:
         return result
 
     background_color = config.get_background_color()
     if background_color is not None:
-        result['backgroundColor'] = color_to_javascript(
+        result["backgroundColor"] = color_to_javascript(
             color=background_color,
         )
 
     is_outlined = config.is_outlined()
     if is_outlined is not None:
-        result['outline'] = bool_to_javascript(is_outlined)
+        result["outline"] = bool_to_javascript(is_outlined)
 
     return result
```

### Comparing `moldoc-0.0.4/src/moldoc/molDraw.js` & `moldoc-1.0.0/src/moldoc/_internal/molDraw.js`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.4/src/moldoc/molecule.py` & `moldoc-1.0.0/src/moldoc/_internal/molecule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from __future__ import annotations
-
-from typing import Iterable, Optional
+from typing import Iterable, Optional, TypeAlias
 
 
 class Color:
     def __init__(self, red: int, green: int, blue: int) -> None:
         self._red = red
         self._green = green
         self._blue = blue
@@ -21,15 +19,14 @@
 
 class AtomConfig:
     def __init__(
         self,
         color: Optional[Color] = None,
         size: Optional[float] = None,
     ) -> None:
-
         self._color = color
         self._size = size
 
     def get_color(self) -> Optional[Color]:
         return self._color
 
     def get_size(self) -> Optional[float]:
@@ -39,15 +36,14 @@
 class Atom:
     def __init__(
         self,
         atomic_number: int,
         position: tuple[float, float, float],
         config: Optional[AtomConfig] = None,
     ) -> None:
-
         self._atomic_number = atomic_number
         self._position = position
         self._config = config
 
     def get_atomic_number(self) -> int:
         return self._atomic_number
 
@@ -61,74 +57,67 @@
 class Bond:
     def __init__(
         self,
         atom1_id: int,
         atom2_id: int,
         order: int,
     ) -> None:
-
         self._atom1_id = atom1_id
         self._atom2_id = atom2_id
         self._order = order
 
     def get_atom1_id(self) -> int:
         return self._atom1_id
 
     def get_atom2_id(self) -> int:
         return self._atom2_id
 
     def get_order(self) -> int:
         return self._order
 
 
-class Material:
-    pass
-
-
-class MeshLambertMaterial(Material):
+class MeshLambertMaterial:
     pass
 
 
-class MeshNormalMaterial(Material):
+class MeshNormalMaterial:
     pass
 
 
-class MeshPhongMaterial(Material):
+class MeshPhongMaterial:
     def __init__(
         self,
         shininess: Optional[float] = None,
         reflectivity: Optional[float] = None,
         flat_shading: Optional[bool] = None,
     ) -> None:
-
         self._shininess = shininess
         self._reflectivity = reflectivity
         self._flat_shading = flat_shading
 
     def get_shininess(self) -> Optional[float]:
         return self._shininess
 
     def get_reflectivity(self) -> Optional[float]:
         return self._reflectivity
 
     def get_flat_shading(self) -> Optional[bool]:
         return self._flat_shading
 
 
-class MeshPhysicalMaterial(Material):
+class MeshPhysicalMaterial:
     def __init__(
         self,
         clearcoat: Optional[float] = None,
         clearcoat_roughness: Optional[float] = None,
         roughness: Optional[float] = None,
         metalness: Optional[float] = None,
         reflectivity: Optional[float] = None,
         flat_shading: Optional[bool] = None,
     ) -> None:
-
         self._clearcoat = clearcoat
         self._clearcoat_roughness = clearcoat_roughness
         self._roughness = roughness
         self._metalness = metalness
         self._reflectivity = reflectivity
         self._flat_shading = flat_shading
 
@@ -147,49 +136,52 @@
     def get_reflectivity(self) -> Optional[float]:
         return self._reflectivity
 
     def get_flat_shading(self) -> Optional[bool]:
         return self._flat_shading
 
 
-class MeshStandardMaterial(Material):
+class MeshStandardMaterial:
     def __init__(
         self,
         metalness: Optional[float] = None,
         roughness: Optional[float] = None,
         flat_shading: Optional[bool] = None,
     ) -> None:
-
         self._metalness = metalness
         self._roughness = roughness
         self._flat_shading = flat_shading
 
     def get_metalness(self) -> Optional[float]:
         return self._metalness
 
     def get_roughness(self) -> Optional[float]:
         return self._roughness
 
     def get_flat_shading(self) -> Optional[bool]:
         return self._flat_shading
 
 
-class MeshToonMaterial(Material):
-    pass
+Material: TypeAlias = (
+    MeshLambertMaterial
+    | MeshNormalMaterial
+    | MeshPhongMaterial
+    | MeshPhysicalMaterial
+    | MeshStandardMaterial
+)
 
 
 class MoleculeConfig:
     def __init__(
         self,
         atom_scale: Optional[float] = None,
         material: Optional[Material] = None,
         background_color: Optional[Color] = None,
-        is_outlined: Optional[bool] = None
+        is_outlined: Optional[bool] = None,
     ) -> None:
-
         self._atom_scale = atom_scale
         self._material = material
         self._background_color = background_color
         self._is_outlined = is_outlined
 
     def get_atom_scale(self) -> Optional[float]:
         return self._atom_scale
@@ -207,15 +199,14 @@
 class Molecule:
     def __init__(
         self,
         atoms: Iterable[Atom],
         bonds: Iterable[Bond],
         config: Optional[MoleculeConfig] = None,
     ) -> None:
-
         self._atoms = tuple(atoms)
         self._bonds = tuple(bonds)
         self._config = config
 
     def get_atoms(self) -> tuple[Atom, ...]:
         return self._atoms
```

### Comparing `moldoc-0.0.4/src/moldoc/three.min.js` & `moldoc-1.0.0/src/moldoc/_internal/three.min.js`

 * *Files identical despite different names*

