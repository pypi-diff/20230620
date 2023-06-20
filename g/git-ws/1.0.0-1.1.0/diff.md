# Comparing `tmp/git_ws-1.0.0.tar.gz` & `tmp/git_ws-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_ws-1.0.0.tar", max compression
+gzip compressed data, was "git_ws-1.1.0.tar", max compression
```

## Comparing `git_ws-1.0.0.tar` & `git_ws-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    15893 2023-03-24 09:50:58.637207 git_ws-1.0.0/README.md
--rw-r--r--   0        0        0     4339 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/__init__.py
--rw-r--r--   0        0        0      834 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/__main__.py
--rw-r--r--   0        0        0     2325 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/_basemodel.py
--rw-r--r--   0        0        0    19415 2023-06-07 20:20:04.547206 git_ws-1.0.0/gitws/_cli/__init__.py
--rw-r--r--   0        0        0     4378 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/_cli/common.py
--rw-r--r--   0        0        0     8808 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/_cli/config.py
--rw-r--r--   0        0        0     4801 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/_cli/dep.py
--rw-r--r--   0        0        0     3705 2023-03-27 21:51:51.061952 git_ws-1.0.0/gitws/_cli/info.py
--rw-r--r--   0        0        0     4213 2023-03-22 22:59:30.360352 git_ws-1.0.0/gitws/_cli/manifest.py
--rw-r--r--   0        0        0     4757 2023-06-07 20:20:04.547206 git_ws-1.0.0/gitws/_cli/options.py
--rw-r--r--   0        0        0     2612 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/_cli/remote.py
--rw-r--r--   0        0        0     5497 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/_filerefupdater.py
--rw-r--r--   0        0        0     3693 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/_url.py
--rw-r--r--   0        0        0     4438 2023-06-07 20:20:04.547206 git_ws-1.0.0/gitws/_util.py
--rw-r--r--   0        0        0    15719 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/appconfig.py
--rw-r--r--   0        0        0     6184 2023-04-16 19:53:26.936660 git_ws-1.0.0/gitws/clone.py
--rw-r--r--   0        0        0     2142 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/const.py
--rw-r--r--   0        0        0    38080 2023-06-07 20:20:04.547206 git_ws-1.0.0/gitws/datamodel.py
--rw-r--r--   0        0        0     4033 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/deptree.py
--rw-r--r--   0        0        0     5509 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/exceptions.py
--rw-r--r--   0        0        0    22171 2023-06-07 20:20:04.551206 git_ws-1.0.0/gitws/git.py
--rw-r--r--   0        0        0    33393 2023-06-07 20:20:04.551206 git_ws-1.0.0/gitws/gitws.py
--rw-r--r--   0        0        0    13343 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/iters.py
--rw-r--r--   0        0        0     1537 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/manifestfinder.py
--rw-r--r--   0        0        0    11828 2023-06-07 20:20:04.551206 git_ws-1.0.0/gitws/workspace.py
--rw-r--r--   0        0        0     1429 2023-03-22 22:59:30.364352 git_ws-1.0.0/gitws/workspacefinder.py
--rw-r--r--   0        0        0     2684 2023-06-07 20:40:24.211022 git_ws-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    16774 1970-01-01 00:00:00.000000 git_ws-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    15974 2023-06-20 18:41:05.854444 git_ws-1.1.0/README.md
+-rw-r--r--   0        0        0     4339 2023-03-22 22:59:30.360352 git_ws-1.1.0/gitws/__init__.py
+-rw-r--r--   0        0        0      834 2023-03-22 22:59:30.360352 git_ws-1.1.0/gitws/__main__.py
+-rw-r--r--   0        0        0     2325 2023-03-22 22:59:30.360352 git_ws-1.1.0/gitws/_basemodel.py
+-rw-r--r--   0        0        0    19327 2023-06-20 13:28:27.189898 git_ws-1.1.0/gitws/_cli/__init__.py
+-rw-r--r--   0        0        0     4378 2023-03-22 22:59:30.360352 git_ws-1.1.0/gitws/_cli/common.py
+-rw-r--r--   0        0        0     8808 2023-03-22 22:59:30.360352 git_ws-1.1.0/gitws/_cli/config.py
+-rw-r--r--   0        0        0     4599 2023-06-20 16:55:40.871316 git_ws-1.1.0/gitws/_cli/dep.py
+-rw-r--r--   0        0        0     3705 2023-03-27 21:51:51.061952 git_ws-1.1.0/gitws/_cli/info.py
+-rw-r--r--   0        0        0     4213 2023-03-22 22:59:30.360352 git_ws-1.1.0/gitws/_cli/manifest.py
+-rw-r--r--   0        0        0     4846 2023-06-20 13:28:38.638111 git_ws-1.1.0/gitws/_cli/options.py
+-rw-r--r--   0        0        0     2524 2023-06-20 13:28:58.494479 git_ws-1.1.0/gitws/_cli/remote.py
+-rw-r--r--   0        0        0     5497 2023-03-22 22:59:30.364352 git_ws-1.1.0/gitws/_filerefupdater.py
+-rw-r--r--   0        0        0     3693 2023-03-22 22:59:30.364352 git_ws-1.1.0/gitws/_url.py
+-rw-r--r--   0        0        0     4438 2023-06-07 20:20:04.547206 git_ws-1.1.0/gitws/_util.py
+-rw-r--r--   0        0        0    15719 2023-03-22 22:59:30.364352 git_ws-1.1.0/gitws/appconfig.py
+-rw-r--r--   0        0        0     6184 2023-04-16 19:53:26.936660 git_ws-1.1.0/gitws/clone.py
+-rw-r--r--   0        0        0     2142 2023-03-22 22:59:30.364352 git_ws-1.1.0/gitws/const.py
+-rw-r--r--   0        0        0    38080 2023-06-07 20:20:04.547206 git_ws-1.1.0/gitws/datamodel.py
+-rw-r--r--   0        0        0     4033 2023-03-22 22:59:30.364352 git_ws-1.1.0/gitws/deptree.py
+-rw-r--r--   0        0        0     5509 2023-03-22 22:59:30.364352 git_ws-1.1.0/gitws/exceptions.py
+-rw-r--r--   0        0        0    22171 2023-06-07 20:20:04.551206 git_ws-1.1.0/gitws/git.py
+-rw-r--r--   0        0        0    33461 2023-06-20 16:55:26.167033 git_ws-1.1.0/gitws/gitws.py
+-rw-r--r--   0        0        0    13343 2023-03-22 22:59:30.364352 git_ws-1.1.0/gitws/iters.py
+-rw-r--r--   0        0        0     1537 2023-03-22 22:59:30.364352 git_ws-1.1.0/gitws/manifestfinder.py
+-rw-r--r--   0        0        0    11828 2023-06-07 20:20:04.551206 git_ws-1.1.0/gitws/workspace.py
+-rw-r--r--   0        0        0     1429 2023-03-22 22:59:30.364352 git_ws-1.1.0/gitws/workspacefinder.py
+-rw-r--r--   0        0        0     2684 2023-06-20 18:42:08.187662 git_ws-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16855 1970-01-01 00:00:00.000000 git_ws-1.1.0/PKG-INFO
```

### Comparing `git_ws-1.0.0/README.md` & `git_ws-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 [![PyPI Version](https://badge.fury.io/py/git-ws.svg)](https://badge.fury.io/py/git-ws)
-[![PyPI Downloads](https://img.shields.io/pypi/dm/git-ws.svg?label=pypi%20downloads)](https://pypi.python.org/pypi/git-ws)
 [![Python Build](https://github.com/c0fec0de/git-ws/actions/workflows/main.yml/badge.svg)](https://github.com/c0fec0de/git-ws/actions/workflows/main.yml)
 [![Documentation](https://readthedocs.org/projects/git-ws/badge/?version=latest)](https://git-ws.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/c0fec0de/git-ws/badge.svg?branch=main)](https://coveralls.io/github/c0fec0de/git-ws?branch=main)
 [![python-versions](https://img.shields.io/pypi/pyversions/git-ws.svg)](https://pypi.python.org/pypi/git-ws)
 [![pylint](https://img.shields.io/badge/linter-pylint-%231674b1?style=flat)](https://www.pylint.org/)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+[Documentation](https://git-ws.readthedocs.io/en/latest/) -
+[PyPI](https://pypi.org/project/git-ws/) -
+[Sources](https://github.com/c0fec0de/git-ws) -
+[Issues](https://github.com/c0fec0de/git-ws/issues)
+
 # Git Workspace - Multi Repository Management Tool
 
 * [Installation](https://github.com/c0fec0de/git-ws#-installation)
 * [Usage](https://github.com/c0fec0de/git-ws#-usage)
 * [Getting Started](https://github.com/c0fec0de/git-ws#-getting-started)
 * [Cheat-Sheet](https://github.com/c0fec0de/git-ws#%EF%B8%8F-cheat-sheet)
 * [Python API](https://github.com/c0fec0de/git-ws#-python-api)
```

### Comparing `git_ws-1.0.0/gitws/__init__.py` & `git_ws-1.1.0/gitws/__init__.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/__main__.py` & `git_ws-1.1.0/gitws/__main__.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/_basemodel.py` & `git_ws-1.1.0/gitws/_basemodel.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/_cli/__init__.py` & `git_ws-1.1.0/gitws/_cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,15 +513,14 @@
 @click.argument("value")
 @pass_context
 def default(context, manifest_path, name, value):
     """
     Set DEFAULT in Manifest to VALUE.
     """
     with exceptionhandling(context):
-        manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         defaults = manifest_spec.defaults.update_fromstr({name: value if value else None})
         manifest_spec = manifest_spec.update(defaults=defaults)
         manifest_spec.save(manifest_path)
 
 
 @main.command(name="group-filters")
@@ -531,15 +530,14 @@
 def group_filters(context, manifest_path, value):
     """
     Set Group Filter to VALUE.
 
     The group filter selects/deselects dependencies based on their path and/or groups.
     """
     with exceptionhandling(context):
-        manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         manifest_spec = manifest_spec.update_fromstr({"group-filters": value if value else None})
         manifest_spec.save(manifest_path)
 
 
 @main.command()
 @projects_option()
```

### Comparing `git_ws-1.0.0/gitws/_cli/common.py` & `git_ws-1.1.0/gitws/_cli/common.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/_cli/config.py` & `git_ws-1.1.0/gitws/_cli/config.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/_cli/dep.py` & `git_ws-1.1.0/gitws/_cli/dep.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with Git Workspace. If not, see <https://www.gnu.org/licenses/>.
 
 """Dependency Commands."""
-from pathlib import Path
-
 import click
 import tomlkit
 
 from gitws import ManifestSpec, ProjectSpec
 from gitws._util import as_dict
 
 from .common import exceptionhandling, pass_context
@@ -61,15 +59,14 @@
     with_groups=None,
     submodules=None,
 ):
     """
     Add Dependency NAME.
     """
     with exceptionhandling(context):
-        manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         dependencies = list(manifest_spec.dependencies)
         dependencies.append(
             ProjectSpec(name=name).update_fromstr(
                 {
                     "remote": remote,
                     "sub-url": sub_url,
@@ -99,15 +96,14 @@
 @click.argument("value")
 @pass_context
 def set_(context, manifest_path, dep, attribute, value):
     """
     Set ATTRIBUTE For Dependency DEP to VALUE.
     """
     with exceptionhandling(context):
-        manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         dependencies = list(manifest_spec.dependencies)
         for idx, dependency in enumerate(dependencies):
             if dependency.name == dep:
                 break
         else:
             raise ValueError(f"Unknown dependency {dep!r}")
@@ -120,15 +116,14 @@
 @manifest_option(initial=True)
 @pass_context
 def list_(context, manifest_path):
     """
     List Dependencies.
     """
     with exceptionhandling(context):
-        manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         doc = tomlkit.document()
         doc.add("dependencies", as_dict(manifest_spec)["dependencies"])
         click.echo(tomlkit.dumps(doc))
 
 
 @dep.command()
@@ -136,15 +131,14 @@
 @manifest_option(initial=True)
 @pass_context
 def delete(context, name, manifest_path):
     """
     Delete Dependency NAME.
     """
     with exceptionhandling(context):
-        manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         dependencies = list(manifest_spec.dependencies)
         for idx, dep in enumerate(manifest_spec.dependencies):
             if dep.name == name:
                 break
         else:
             raise ValueError(f"Unknown dependency {name!r}")
```

### Comparing `git_ws-1.0.0/gitws/_cli/info.py` & `git_ws-1.1.0/gitws/_cli/info.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/_cli/manifest.py` & `git_ws-1.1.0/gitws/_cli/manifest.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/_cli/options.py` & `git_ws-1.1.0/gitws/_cli/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,20 @@
     if initial:
         help_ = f"Manifest file. '{MANIFEST_PATH_DEFAULT!s}' by default."
         default = MANIFEST_PATH_DEFAULT
     else:
         help_ = "Manifest file. Initial/Configuration settings by default."
         default = None
     return click.option(
-        "--manifest", "-M", "manifest_path", type=click.Path(dir_okay=False), default=default, help=help_
+        "--manifest",
+        "-M",
+        "manifest_path",
+        type=click.Path(dir_okay=False, path_type=Path),
+        default=default,
+        help=help_,
     )
 
 
 def update_option():
     """Update Option."""
     return click.option("--update", "-U", is_flag=True, help="Run 'git ws update' too.")
 
@@ -86,30 +91,30 @@
 
 def output_option():
     """Manifest Output Option."""
     return click.option(
         "--output",
         "-O",
         "output",
-        type=click.Path(dir_okay=False),
+        type=click.Path(dir_okay=False, path_type=Path),
         help="Write Manifest to file instead of STDOUT.",
     )
 
 
 def ws_path_option(nomain: bool = False):
     """Workspace Path Option."""
     if nomain:
         descr = "Workspace Path. Parent directory of main project by default."
     else:
         descr = "Workspace Path. Parent directory of main project or current working directory by default."
     return click.option(
         "--ws-path",
         "-w",
         "ws_path",
-        type=click.Path(file_okay=False),
+        type=click.Path(file_okay=False, path_type=Path),
         help=descr,
     )
 
 
 def main_path_option():
     """Main Repository Path."""
     return click.argument("main_path", nargs=-1, type=click.UNPROCESSED)
```

### Comparing `git_ws-1.0.0/gitws/_cli/remote.py` & `git_ws-1.1.0/gitws/_cli/remote.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 @manifest_option(initial=True)
 @pass_context
 def add(context, name, url_base, manifest_path):
     """
     Add Remote NAME with URL_BASE.
     """
     with exceptionhandling(context):
-        manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         remotes = list(manifest_spec.remotes)
         remotes.append(Remote(name=name, url_base=url_base))
         manifest_spec = manifest_spec.update(remotes=remotes)
         manifest_spec.save(manifest_path)
 
 
@@ -70,15 +69,14 @@
 @manifest_option(initial=True)
 @pass_context
 def delete(context, name, manifest_path):
     """
     Delete Remote NAME.
     """
     with exceptionhandling(context):
-        manifest_path = Path(manifest_path)
         manifest_spec = ManifestSpec.load(manifest_path)
         remotes = list(manifest_spec.remotes)
         for idx, remote in enumerate(manifest_spec.remotes):
             if remote.name == name:
                 break
         else:
             raise ValueError(f"Unknown dependency {name!r}")
```

### Comparing `git_ws-1.0.0/gitws/_filerefupdater.py` & `git_ws-1.1.0/gitws/_filerefupdater.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/_url.py` & `git_ws-1.1.0/gitws/_url.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/_util.py` & `git_ws-1.1.0/gitws/_util.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/appconfig.py` & `git_ws-1.1.0/gitws/appconfig.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/clone.py` & `git_ws-1.1.0/gitws/clone.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/const.py` & `git_ws-1.1.0/gitws/const.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/datamodel.py` & `git_ws-1.1.0/gitws/datamodel.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/deptree.py` & `git_ws-1.1.0/gitws/deptree.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/exceptions.py` & `git_ws-1.1.0/gitws/exceptions.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/git.py` & `git_ws-1.1.0/gitws/git.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/gitws.py` & `git_ws-1.1.0/gitws/gitws.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,17 +170,17 @@
                            This value is written to the configuration.
             depth: Shallow Clone Depth.
             force: Ignore that the workspace exists.
             secho: :any:`click.secho` like print method for verbose output.
         """
         _LOGGER.debug(
             "GitWS.create(%r, main_path=%r, manifest_path=%r, group-filters=%r)",
-            str(path),
-            str(main_path),
-            str(manifest_path),
+            str(path) if path else None,
+            str(main_path) if main_path else None,
+            str(manifest_path) if manifest_path else None,
             group_filters,
         )
         # Relative to main_path if given, or workspace path as fallback
         # We need to resolve in inverted order, otherwise the manifest_path is broken
         # ``manifest_path`` can be absolute or relative to ``base_path``. we need it relative to ``base_path``.
         manifest_path_rel = resolve_relative(manifest_path or MANIFEST_PATH_DEFAULT, base=(main_path or path))
         if main_path:
```

### Comparing `git_ws-1.0.0/gitws/iters.py` & `git_ws-1.1.0/gitws/iters.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/manifestfinder.py` & `git_ws-1.1.0/gitws/manifestfinder.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/workspace.py` & `git_ws-1.1.0/gitws/workspace.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/gitws/workspacefinder.py` & `git_ws-1.1.0/gitws/workspacefinder.py`

 * *Files identical despite different names*

### Comparing `git_ws-1.0.0/pyproject.toml` & `git_ws-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-ws"
-version = "1.0.0"
+version = "1.1.0"
 description = "Git Workspace - Multi Repository Management Tool"
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 authors = [
     "c0fec0de <c0fec0de@gmail.com>",
     "Martin Höher <martin@rpdev.net>",
 ]
```

### Comparing `git_ws-1.0.0/PKG-INFO` & `git_ws-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-ws
-Version: 1.0.0
+Version: 1.1.0
 Summary: Git Workspace - Multi Repository Management Tool
 License: LGPL-3.0-or-later
 Author: c0fec0de
 Author-email: c0fec0de@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
@@ -18,22 +18,26 @@
 Requires-Dist: click (>=6.7.0,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: tomlkit (>=0.11.5,<1.0.0)
 Description-Content-Type: text/markdown
 
 [![PyPI Version](https://badge.fury.io/py/git-ws.svg)](https://badge.fury.io/py/git-ws)
-[![PyPI Downloads](https://img.shields.io/pypi/dm/git-ws.svg?label=pypi%20downloads)](https://pypi.python.org/pypi/git-ws)
 [![Python Build](https://github.com/c0fec0de/git-ws/actions/workflows/main.yml/badge.svg)](https://github.com/c0fec0de/git-ws/actions/workflows/main.yml)
 [![Documentation](https://readthedocs.org/projects/git-ws/badge/?version=latest)](https://git-ws.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/c0fec0de/git-ws/badge.svg?branch=main)](https://coveralls.io/github/c0fec0de/git-ws?branch=main)
 [![python-versions](https://img.shields.io/pypi/pyversions/git-ws.svg)](https://pypi.python.org/pypi/git-ws)
 [![pylint](https://img.shields.io/badge/linter-pylint-%231674b1?style=flat)](https://www.pylint.org/)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+[Documentation](https://git-ws.readthedocs.io/en/latest/) -
+[PyPI](https://pypi.org/project/git-ws/) -
+[Sources](https://github.com/c0fec0de/git-ws) -
+[Issues](https://github.com/c0fec0de/git-ws/issues)
+
 # Git Workspace - Multi Repository Management Tool
 
 * [Installation](https://github.com/c0fec0de/git-ws#-installation)
 * [Usage](https://github.com/c0fec0de/git-ws#-usage)
 * [Getting Started](https://github.com/c0fec0de/git-ws#-getting-started)
 * [Cheat-Sheet](https://github.com/c0fec0de/git-ws#%EF%B8%8F-cheat-sheet)
 * [Python API](https://github.com/c0fec0de/git-ws#-python-api)
```

