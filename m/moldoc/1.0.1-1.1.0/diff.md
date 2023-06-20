# Comparing `tmp/moldoc-1.0.1.tar.gz` & `tmp/moldoc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moldoc-1.0.1.tar", last modified: Tue Jun 20 13:28:13 2023, max compression
+gzip compressed data, was "moldoc-1.1.0.tar", last modified: Tue Jun 20 14:39:00 2023, max compression
```

## Comparing `moldoc-1.0.1.tar` & `moldoc-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:28:13.464856 moldoc-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:28:13.448856 moldoc-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:28:13.452856 moldoc-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 13:27:36.000000 moldoc-1.0.1/.github/workflows/publish_release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-20 13:27:36.000000 moldoc-1.0.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 13:27:36.000000 moldoc-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-20 13:27:36.000000 moldoc-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-20 13:28:13.464856 moldoc-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-20 13:27:36.000000 moldoc-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)   117976 2023-06-20 13:27:36.000000 moldoc-1.0.1/configuration.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-20 13:27:36.000000 moldoc-1.0.1/justfile
--rw-r--r--   0 runner    (1001) docker     (123)  1268442 2023-06-20 13:27:36.000000 moldoc-1.0.1/moldoc.gif
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-20 13:27:36.000000 moldoc-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:28:13.464856 moldoc-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:28:13.448856 moldoc-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:28:13.452856 moldoc-1.0.1/src/moldoc/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:28:13.456856 moldoc-1.0.1/src/moldoc/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:28:13.460856 moldoc-1.0.1/src/moldoc/_internal/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/javascript/atoms.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/javascript/bonds.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/javascript/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/javascript/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/javascript/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/javascript/mesh_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/javascript/scene_config.py
--rw-r--r--   0 runner    (1001) docker     (123)   351667 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/molDraw.js
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/moldoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)   551410 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/_internal/three.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:27:36.000000 moldoc-1.0.1/src/moldoc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 13:28:13.000000 moldoc-1.0.1/src/moldoc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:28:13.456856 moldoc-1.0.1/src/moldoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-20 13:28:13.000000 moldoc-1.0.1/src/moldoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-20 13:28:13.000000 moldoc-1.0.1/src/moldoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:28:13.000000 moldoc-1.0.1/src/moldoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 13:28:13.000000 moldoc-1.0.1/src/moldoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 13:28:13.000000 moldoc-1.0.1/src/moldoc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:28:13.460856 moldoc-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-20 13:27:36.000000 moldoc-1.0.1/tests/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-20 13:27:36.000000 moldoc-1.0.1/tests/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:28:13.460856 moldoc-1.0.1/tests/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:28:13.460856 moldoc-1.0.1/tests/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:27:36.000000 moldoc-1.0.1/tests/source/_static/empty
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-20 13:27:36.000000 moldoc-1.0.1/tests/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-06-20 13:27:36.000000 moldoc-1.0.1/tests/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.331547 moldoc-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.323547 moldoc-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.327547 moldoc-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 14:38:19.000000 moldoc-1.1.0/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-20 14:38:19.000000 moldoc-1.1.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 14:38:19.000000 moldoc-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-20 14:38:19.000000 moldoc-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-20 14:39:00.331547 moldoc-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-20 14:38:19.000000 moldoc-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   117976 2023-06-20 14:38:19.000000 moldoc-1.1.0/configuration.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-20 14:38:19.000000 moldoc-1.1.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)  1268442 2023-06-20 14:38:19.000000 moldoc-1.1.0/moldoc.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-20 14:38:19.000000 moldoc-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:39:00.331547 moldoc-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.323547 moldoc-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.327547 moldoc-1.1.0/src/moldoc/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.327547 moldoc-1.1.0/src/moldoc/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.327547 moldoc-1.1.0/src/moldoc/_internal/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/bonds.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/mesh_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/javascript/scene_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   351667 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/molDraw.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/moldoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551410 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/_internal/three.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:38:19.000000 moldoc-1.1.0/src/moldoc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 14:39:00.000000 moldoc-1.1.0/src/moldoc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.327547 moldoc-1.1.0/src/moldoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-20 14:39:00.000000 moldoc-1.1.0/src/moldoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-20 14:39:00.000000 moldoc-1.1.0/src/moldoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:39:00.000000 moldoc-1.1.0/src/moldoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 14:39:00.000000 moldoc-1.1.0/src/moldoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 14:39:00.000000 moldoc-1.1.0/src/moldoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.327547 moldoc-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-20 14:38:19.000000 moldoc-1.1.0/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-20 14:38:19.000000 moldoc-1.1.0/tests/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.331547 moldoc-1.1.0/tests/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:39:00.331547 moldoc-1.1.0/tests/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:38:19.000000 moldoc-1.1.0/tests/source/_static/empty
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-20 14:38:19.000000 moldoc-1.1.0/tests/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-06-20 14:38:19.000000 moldoc-1.1.0/tests/source/index.rst
```

### Comparing `moldoc-1.0.1/.github/workflows/publish_release.yaml` & `moldoc-1.1.0/.github/workflows/publish_release.yaml`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/.github/workflows/tests.yaml` & `moldoc-1.1.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/LICENSE` & `moldoc-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/PKG-INFO` & `moldoc-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moldoc
-Version: 1.0.1
+Version: 1.1.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/moldoc
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `moldoc-1.0.1/README.rst` & `moldoc-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/configuration.jpg` & `moldoc-1.1.0/configuration.jpg`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/moldoc.gif` & `moldoc-1.1.0/moldoc.gif`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/pyproject.toml` & `moldoc-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/src/moldoc/_internal/javascript/atoms.py` & `moldoc-1.1.0/src/moldoc/_internal/javascript/atoms.py`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/src/moldoc/_internal/javascript/material.py` & `moldoc-1.1.0/src/moldoc/_internal/javascript/material.py`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/src/moldoc/_internal/javascript/mesh_config.py` & `moldoc-1.1.0/src/moldoc/_internal/javascript/mesh_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from moldoc._internal.javascript.color import color_to_javascript
 from moldoc._internal.javascript.material import material_to_javascript
 from moldoc.molecule import Atom, Molecule, MoleculeConfig
 
 
 def get_mesh_config(
     molecule: Molecule,
+    molecule_config: MoleculeConfig | None,
 ) -> str:
     mesh_config = []
     atoms = molecule.get_atoms()
 
     atom_size_function = _get_atom_size_function(atoms)
     if atom_size_function is not None:
         mesh_config.append(atom_size_function)
 
     atom_color_function = _get_atom_color_function(atoms)
     if atom_color_function is not None:
         mesh_config.append(atom_color_function)
 
-    molecule_config = molecule.get_config()
     if molecule_config is not None:
         atom_scale = molecule_config.get_atom_scale()
         if atom_scale is not None:
             mesh_config.append(f"atomScale:{atom_scale}")
 
         material = molecule_config.get_material()
         if material is not None:
```

### Comparing `moldoc-1.0.1/src/moldoc/_internal/javascript/scene_config.py` & `moldoc-1.1.0/src/moldoc/_internal/javascript/scene_config.py`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/src/moldoc/_internal/molDraw.js` & `moldoc-1.1.0/src/moldoc/_internal/molDraw.js`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/src/moldoc/_internal/moldoc.py` & `moldoc-1.1.0/src/moldoc/_internal/moldoc.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from sphinx.util.docutils import SphinxDirective
 from sphinx.writers.html5 import HTML5Translator
 
 from moldoc._internal.javascript.atoms import get_atom_array
 from moldoc._internal.javascript.bonds import get_bond_array
 from moldoc._internal.javascript.mesh_config import get_mesh_config
 from moldoc._internal.javascript.scene_config import get_scene_config
-from moldoc.molecule import Molecule
+from moldoc.molecule import Molecule, MoleculeConfig
 from moldoc.version import __version__
 
 
 class MolDocNode(nodes.Body, nodes.Element):
     def __init__(
         self,
         moldoc_name: str,
@@ -44,14 +44,21 @@
             molecule=globals_["moldoc_display_molecule"],
         )
         return [node]
 
 
 def html_moldoc(self: HTML5Translator, node: MolDocNode) -> None:
     molecule = node.get_molecule()
+
+    default_molecule_config = self.config.moldoc_default_molecule_config
+    if (config := molecule.get_config()) is not None:
+        molecule_config = default_molecule_config.update(config)
+    else:
+        molecule_config = default_molecule_config
+
     moldoc_node_id = node.get_moldoc_name()
 
     if not getattr(self, "moldoc_scripts_added", False):
         self.body.append(
             '<script src="/_static/three.min.js"></script>'
             '<script src="/_static/molDraw.js"></script>'
             "<script>const md=molDraw;"
@@ -71,18 +78,18 @@
         'console.log("There was an issue with your molecule.");'
         "console.log(md.fromLeft()(maybeMolecule));"
         "}"
         "else"
         "{"
         "const molecule=md.fromRight()(maybeMolecule);"
         "const scene=md.scene({"
-        f"{get_scene_config(moldoc_node_id, molecule.get_config())}"
+        f"{get_scene_config(moldoc_node_id, molecule_config)}"
         "});"
         "const meshes=md.meshes({"
-        f"{get_mesh_config(molecule)}"
+        f"{get_mesh_config(molecule, molecule_config)}"
         "})(molecule);"
         "md.drawMol(scene(meshes));"
         "}"
     )
 
     self.body.append(
         f'<div id="{moldoc_node_id}" style="height:25vh;"></div>'
@@ -110,12 +117,18 @@
 def setup(app: Sphinx) -> dict:
     app.connect("build-finished", copy_asset_files)
     app.add_directive("moldoc", MolDoc)
     app.add_node(
         node=MolDocNode,
         html=(html_moldoc, None),
     )
+    app.add_config_value(
+        "moldoc_default_molecule_config",
+        MoleculeConfig(),
+        "html",
+        [MoleculeConfig],
+    )
     return {
         "version": __version__,
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `moldoc-1.0.1/src/moldoc/_internal/molecule.py` & `moldoc-1.1.0/src/moldoc/_internal/molecule.py`

 * *Files 15% similar despite different names*

```diff
@@ -191,14 +191,40 @@
 
     def get_background_color(self) -> Optional[Color]:
         return self._background_color
 
     def is_outlined(self) -> Optional[bool]:
         return self._is_outlined
 
+    def update(self, other: "MoleculeConfig") -> "MoleculeConfig":
+        atom_scale = (
+            self._atom_scale
+            if other._atom_scale is None
+            else other._atom_scale
+        )
+        material = (
+            self._material if other._material is None else other._material
+        )
+        background_color = (
+            self._background_color
+            if other._background_color is None
+            else other._background_color
+        )
+        is_outlined = (
+            self._is_outlined
+            if other._is_outlined is None
+            else other._is_outlined
+        )
+        return MoleculeConfig(
+            atom_scale=atom_scale,
+            material=material,
+            background_color=background_color,
+            is_outlined=is_outlined,
+        )
+
 
 class Molecule:
     def __init__(
         self,
         atoms: Iterable[Atom],
         bonds: Iterable[Bond],
         config: Optional[MoleculeConfig] = None,
```

### Comparing `moldoc-1.0.1/src/moldoc/_internal/three.min.js` & `moldoc-1.1.0/src/moldoc/_internal/three.min.js`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/src/moldoc/molecule.py` & `moldoc-1.1.0/src/moldoc/molecule.py`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/src/moldoc.egg-info/PKG-INFO` & `moldoc-1.1.0/src/moldoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moldoc
-Version: 1.0.1
+Version: 1.1.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/moldoc
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `moldoc-1.0.1/src/moldoc.egg-info/SOURCES.txt` & `moldoc-1.1.0/src/moldoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/tests/Makefile` & `moldoc-1.1.0/tests/Makefile`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/tests/make.bat` & `moldoc-1.1.0/tests/make.bat`

 * *Files identical despite different names*

### Comparing `moldoc-1.0.1/tests/source/conf.py` & `moldoc-1.1.0/tests/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
-
+import moldoc.molecule as molecule
 
 # -- Project information -----------------------------------------------------
 
 project = "moldoc-test"
 copyright = "2021, Lukas Turcani"
 author = "Lukas Turcani"
 
@@ -27,14 +27,18 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "moldoc",
 ]
 
+moldoc_default_molecule_config = molecule.MoleculeConfig(
+    background_color=molecule.Color(32, 32, 32),
+)
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns: list[str] = []
```

### Comparing `moldoc-1.0.1/tests/source/index.rst` & `moldoc-1.1.0/tests/source/index.rst`

 * *Files identical despite different names*

