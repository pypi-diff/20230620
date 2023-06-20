# Comparing `tmp/godoo_cli-0.5.0.tar.gz` & `tmp/godoo_cli-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godoo_cli-0.5.0.tar", max compression
+gzip compressed data, was "godoo_cli-0.5.1.tar", max compression
```

## Comparing `godoo_cli-0.5.0.tar` & `godoo_cli-0.5.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     7633 2023-06-07 09:56:53.914171 godoo_cli-0.5.0/LICENSE
--rw-r--r--   0        0        0     7304 2023-06-07 09:56:53.914171 godoo_cli-0.5.0/README.md
--rw-r--r--   0        0        0     5004 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       61 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/__init__.py
--rw-r--r--   0        0        0       88 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/__main__.py
--rw-r--r--   0        0        0     1963 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/cli.py
--rw-r--r--   0        0        0     5596 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/cli_common.py
--rw-r--r--   0        0        0      293 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/__init__.py
--rw-r--r--   0        0        0     5929 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/bootstrap.py
--rw-r--r--   0        0        0     1173 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/config.py
--rw-r--r--   0        0        0       28 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/db/__init__.py
--rw-r--r--   0        0        0      311 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/db/cli.py
--rw-r--r--   0        0        0     1801 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/db/connection.py
--rw-r--r--   0        0        0     1325 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/db/passwords.py
--rw-r--r--   0        0        0    10763 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/launch.py
--rw-r--r--   0        0        0      177 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/rpc/__init__.py
--rw-r--r--   0        0        0      710 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/rpc/cli.py
--rw-r--r--   0        0        0     2301 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/rpc/importer.py
--rw-r--r--   0        0        0     3623 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/rpc/modules.py
--rw-r--r--   0        0        0     4000 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/rpc/translations.py
--rw-r--r--   0        0        0     1619 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/shell.py
--rw-r--r--   0        0        0     8544 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/source_get.py
--rw-r--r--   0        0        0     4562 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/commands/test.py
--rw-r--r--   0        0        0      161 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/git/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/git/git_odoo.py
--rw-r--r--   0        0        0     3296 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/git/git_odoo_addons.py
--rw-r--r--   0        0        0     6460 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/git/git_repo.py
--rw-r--r--   0        0        0     4585 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/git/git_url.py
--rw-r--r--   0        0        0     1575 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/git/zip_download.py
--rw-r--r--   0        0        0       49 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/helpers/__init__.py
--rw-r--r--   0        0        0     2225 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/helpers/bootstrap.py
--rw-r--r--   0        0        0      386 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/helpers/cli.py
--rw-r--r--   0        0        0     8895 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/helpers/odoo_files.py
--rw-r--r--   0        0        0     3277 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/helpers/odoo_manifest.py
--rw-r--r--   0        0        0     2766 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/helpers/system.py
--rw-r--r--   0        0        0       22 2023-06-07 09:56:53.918171 godoo_cli-0.5.0/src/godoo_cli/version.py
--rw-r--r--   0        0        0     9324 1970-01-01 00:00:00.000000 godoo_cli-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-06-20 17:50:48.696537 godoo_cli-0.5.1/LICENSE
+-rw-r--r--   0        0        0     7304 2023-06-20 17:50:48.696537 godoo_cli-0.5.1/README.md
+-rw-r--r--   0        0        0     5004 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/__init__.py
+-rw-r--r--   0        0        0       88 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/__main__.py
+-rw-r--r--   0        0        0     1963 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/cli.py
+-rw-r--r--   0        0        0     5596 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/cli_common.py
+-rw-r--r--   0        0        0      293 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/__init__.py
+-rw-r--r--   0        0        0     5929 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/bootstrap.py
+-rw-r--r--   0        0        0     1173 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/config.py
+-rw-r--r--   0        0        0       28 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/db/__init__.py
+-rw-r--r--   0        0        0      311 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/db/cli.py
+-rw-r--r--   0        0        0     1801 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/db/connection.py
+-rw-r--r--   0        0        0     1325 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/db/passwords.py
+-rw-r--r--   0        0        0    10763 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/launch.py
+-rw-r--r--   0        0        0      177 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/rpc/__init__.py
+-rw-r--r--   0        0        0      897 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/rpc/cli.py
+-rw-r--r--   0        0        0     1484 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/rpc/config_parameters.py
+-rw-r--r--   0        0        0     2278 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/rpc/importer.py
+-rw-r--r--   0        0        0     4828 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/rpc/modules.py
+-rw-r--r--   0        0        0     4000 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/rpc/translations.py
+-rw-r--r--   0        0        0     1619 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/shell.py
+-rw-r--r--   0        0        0     8544 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/source_get.py
+-rw-r--r--   0        0        0     4562 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/commands/test.py
+-rw-r--r--   0        0        0      161 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/git/__init__.py
+-rw-r--r--   0        0        0     1299 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/git/git_odoo.py
+-rw-r--r--   0        0        0     3296 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/git/git_odoo_addons.py
+-rw-r--r--   0        0        0     6460 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/git/git_repo.py
+-rw-r--r--   0        0        0     4585 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/git/git_url.py
+-rw-r--r--   0        0        0     1575 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/git/zip_download.py
+-rw-r--r--   0        0        0       49 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/helpers/__init__.py
+-rw-r--r--   0        0        0     2225 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/helpers/bootstrap.py
+-rw-r--r--   0        0        0      386 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/helpers/cli.py
+-rw-r--r--   0        0        0     8895 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/helpers/odoo_files.py
+-rw-r--r--   0        0        0     3277 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/helpers/odoo_manifest.py
+-rw-r--r--   0        0        0     2766 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/helpers/system.py
+-rw-r--r--   0        0        0       22 2023-06-20 17:50:48.700537 godoo_cli-0.5.1/src/godoo_cli/version.py
+-rw-r--r--   0        0        0     9324 1970-01-01 00:00:00.000000 godoo_cli-0.5.1/PKG-INFO
```

### Comparing `godoo_cli-0.5.0/LICENSE` & `godoo_cli-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/README.md` & `godoo_cli-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/pyproject.toml` & `godoo_cli-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gOdoo-cli"
-version = "0.5.0"
+version = "0.5.1"
 description = "Wrapper around Odoo-Bin with some convinience RPC functions."
 authors = ["Joshua Kreuder <Joshua_Kreuder@outlook.com>"]
 license = "LGPL-3"
 readme = "README.md"
 packages = [{include = "godoo_cli",  from = "src"}]
 repository = "https://github.com/OpenJKSoftware/gOdoo"
 keywords = ["odoo", "godoo","devcontainer"]
```

### Comparing `godoo_cli-0.5.0/src/godoo_cli/cli.py` & `godoo_cli-0.5.1/src/godoo_cli/cli.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/cli_common.py` & `godoo_cli-0.5.1/src/godoo_cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/commands/bootstrap.py` & `godoo_cli-0.5.1/src/godoo_cli/commands/bootstrap.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/commands/config.py` & `godoo_cli-0.5.1/src/godoo_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/commands/db/connection.py` & `godoo_cli-0.5.1/src/godoo_cli/commands/db/connection.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/commands/db/passwords.py` & `godoo_cli-0.5.1/src/godoo_cli/commands/db/passwords.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/commands/launch.py` & `godoo_cli-0.5.1/src/godoo_cli/commands/launch.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/commands/rpc/cli.py` & `godoo_cli-0.5.1/src/godoo_cli/commands/rpc/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import typer
 
+from .config_parameters import set_config_parameter
 from .importer import import_to_odoo
-from .modules import install_modules
+from .modules import install_modules, uninstall_modules
 from .translations import dump_translations
 
 
 def modules_cli_app():
     app = typer.Typer(
         no_args_is_help=True,
         help="Wrapper around Odoo modules. (Install/upgrade, etc)",
     )
 
     app.command(name="install")(install_modules)
+    app.command(name="uninstall")(uninstall_modules)
     app.command(name="dump-translation")(dump_translations)
     return app
 
 
 def rpc_cli_app():
     app = typer.Typer(
         no_args_is_help=True,
         help="Functions that act on a running Odoo instance via RPC.",
     )
 
     app.add_typer(
         typer_instance=modules_cli_app(),
         name="modules",
     )
+    app.command(name="set-config-param")(set_config_parameter)
     app.command("import")(import_to_odoo)
 
     return app
```

### Comparing `godoo_cli-0.5.0/src/godoo_cli/commands/rpc/importer.py` & `godoo_cli-0.5.1/src/godoo_cli/commands/rpc/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,11 +60,11 @@
         raise ValueError("Provided import Paths: %s doesn't exist", ", ".join(missing_paths))
 
     for path in read_paths:
         import_data(
             odoo_api=odoo_api,
             read_path=path.absolute(),
             data_regex=file_regex,
-            product_image_regex="" if path.is_file() else product_image_regex,
-            check_dataset_timestamp="" if path.is_file() else check_data_timestamp,
+            product_image_regex=False if path.is_file() else product_image_regex,
+            check_dataset_timestamp=check_data_timestamp,
             skip_existing_ids=skip_existing_ids,
         )
```

### Comparing `godoo_cli-0.5.0/src/godoo_cli/commands/rpc/modules.py` & `godoo_cli-0.5.1/src/godoo_cli/commands/rpc/translations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,129 @@
 import logging
-from typing import Any, List
+from base64 import b64decode
+from pathlib import Path
 
 import typer
-from godoo_rpc import OdooApiWrapper
 from godoo_rpc.login import wait_for_odoo
 
 from ...cli_common import CommonCLI
+from ...helpers.odoo_files import get_odoo_module_paths
+from .modules import rpc_get_modules
 
 CLI = CommonCLI()
 LOGGER = logging.getLogger(__name__)
 
 
-def rpc_get_modules(odoo_api: OdooApiWrapper, module_query: str, valid_module_names: List[str] = None):
-    """Get ir.module.module records by a query search string.
+def _dump_translation_for_module(module, target_path: Path):
+    """Dump Translation of a module into POT file.
 
     Parameters
     ----------
-    odoo_api : OdooApiWrapper
-        Odoo Wrapper
-    module_query : str
-        Custom query. Module name. Comma sep list of modules or % wildcards are supported
-    valid_module_names : List[str], optional
-        only allow certain model names to be returned, by default None
-
-    Returns
-    -------
-    _type_
-        _description_
+    module : _type_
+        rpc record of module to export
+    target_path : Path
+        target pot path
     """
-    mod_env = odoo_api.session.env["ir.module.module"]
-    mod_env.update_list()
+    trans_exp_mod = module.env["base.language.export"]
+
+    LOGGER.info("Exporting: %s --> %s", module.name, str(target_path))
+    trans_wiz_id = trans_exp_mod.create({"format": "po", "modules": [module.id]})
+    trans_wiz = trans_exp_mod.browse([trans_wiz_id])
+    trans_wiz.act_getfile()
+    trans_wiz = trans_exp_mod.browse([trans_wiz_id])
+    target_path.parent.mkdir(exist_ok=True)
+    target_path.write_bytes(b64decode(trans_wiz.data))
 
-    base_domain = []
-    if "," in module_query:
-        search_domain = [("name", "in", module_query.split(","))]
-    else:
-        if "%" in module_query:
-            search_domain = [("name", "=ilike", module_query)]
-        else:
-            search_domain = [("name", "=", module_query)]
-
-    if valid_module_names:
-        base_domain.insert(1, "&")
-        base_domain.append(("name", "in", valid_module_names))
-
-    LOGGER.debug("Searching for Modules with Domain: %s", base_domain + search_domain)
-    if ids := mod_env.search(base_domain + search_domain):
-        modules = mod_env.browse(ids)
-        LOGGER.debug("Found Modules: %s", [(m.id, m.name, m.state) for m in modules])
-        return modules
-
-
-def rpc_install_modules(
-    modules: Any,
-    upgrade: bool = True,
+
+def _dump_translations(
+    modules,
+    workspace_addon_path: Path,
+    upgrade_modules: bool = True,
 ):
-    """Install and upgrade Modules to Database.
+    """Dump translations of given Modules into their addon folders.
 
     Parameters
     ----------
-    modules : Iterable RPC ir.module.module records
-        List of
-    upgrade : bool, optional
-        Upgrade module if already installed, by default True
+    odoo_api : OdooApiWrapper
+        Odoo Api Wrapper
+    modules : _type_
+        Api Models of modules
+    workspace_addon_path : Path
+        path where those modules are installed
+    upgrade_modules : bool, optional
+        Wether to upgrade modules before dumping, by default True
     """
-    did_something = False
-    install_module_ids = [m.id for m in modules if m.state == "uninstalled"]
-    if install_module_ids:
-        install_modules = modules.browse(install_module_ids)
-        LOGGER.info("Installing Module: " + ", ".join(install_modules.mapped("name")))
-        install_modules.button_immediate_install()
-        did_something = True
-
-    if upgrade and (
-        up_module_ids := [m.id for m in modules if m.state == "installed" and m.id not in install_module_ids]
-    ):
-        up_modules = modules.browse(up_module_ids)
-        LOGGER.info("Updating Module: " + ", ".join(up_modules.mapped("name")))
-        up_modules.button_immediate_upgrade()
-        did_something = True
-    return did_something
+
+    if upgrade_modules:
+        LOGGER.info("Upgrading Modules: '%s'", ", ".join(modules.mapped("name")))
+        modules.button_immediate_upgrade()
+
+    for mod in modules:
+        ex_path: Path = workspace_addon_path / mod.name / "i18n"
+        pot_path: Path = ex_path / (mod.name + ".pot")
+        _dump_translation_for_module(mod, pot_path)
+
+
+def complete_workspace_addon_names(ctx: typer.Context, incomplete: str):
+    """Autocomplete handler that searches modules in Workspace_addon_path
+
+    Parameters
+    ----------
+    ctx : typer.Context
+        Contains calling parameters
+    incomplete : str
+        Incomplete current entry
+
+    Yields
+    ------
+    str
+        folder name
+    """
+    workspace_folder = ctx.params.get("workspace_addon_path")
+    if not workspace_folder:
+        return
+    workspace_folder = Path(workspace_folder)
+    addon_folders = get_odoo_module_paths(workspace_folder)
+    for fold in addon_folders:
+        if not incomplete or fold.name.startswith(incomplete):
+            yield fold.name
 
 
 @CLI.arg_annotator
-def install_modules(
-    module_name_query: str = typer.Argument(
-        ..., help=r"Module Internal name(s), comma seperated. Will use ilike Match if \% is present"
+def dump_translations(
+    module_query=typer.Argument(
+        ...,
+        help="Module Name(s) comma Seperated. Add % to force =ilike match. Only works in workspace addon path",
+        autocompletion=complete_workspace_addon_names,
     ),
+    workspace_addon_path=CLI.odoo_paths.workspace_addon_path,
     rpc_host=CLI.rpc.rpc_host,
     rpc_database=CLI.rpc.rpc_db_name,
     rpc_user=CLI.rpc.rpc_user,
     rpc_password=CLI.rpc.rpc_password,
-    upgrade: bool = typer.Option(True, help="Upgrae Module if already installed"),
+    no_upgrade_modules: bool = typer.Option(
+        False, "--no-upgrade-modules", help="don't upgrade modules before exporting"
+    ),
 ):
-    """Install or upgrade module. Can act on multiple modules with % wildcard"""
+    """Dump Translations of module to <module_folder>/i18n/<module_name>.pot"""
+    addon_path = workspace_addon_path
+    addon_folders = get_odoo_module_paths(addon_path)
+    valid_module_names = [str(p.stem) for p in addon_folders]
+    LOGGER.debug("Found modules:\n%s", "\n".join(["\t" + mn for mn in valid_module_names]))
 
     odoo_api = wait_for_odoo(
         odoo_host=rpc_host,
         odoo_db=rpc_database,
         odoo_user=rpc_user,
         odoo_password=rpc_password,
     )
 
-    if modules := rpc_get_modules(odoo_api, module_name_query):
-        if rpc_install_modules(modules, upgrade=upgrade):
-            return
-        else:
-            LOGGER.warn("Found Modules, but didn't do anything on DB.")
-    else:
-        LOGGER.warn("Could not find modules with Query: '%s'", module_name_query)
-    return CLI.returner(1)
+    modules = rpc_get_modules(odoo_api, module_query, valid_module_names)
+    if not modules:
+        LOGGER.warning("No installed Modules found for Query string: '%s'", module_query)
+        return CLI.returner(1)
+
+    _dump_translations(
+        modules=modules,
+        workspace_addon_path=addon_path,
+        upgrade_modules=not no_upgrade_modules,
+    )
```

### Comparing `godoo_cli-0.5.0/src/godoo_cli/commands/shell.py` & `godoo_cli-0.5.1/src/godoo_cli/commands/shell.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/commands/source_get.py` & `godoo_cli-0.5.1/src/godoo_cli/commands/source_get.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/commands/test.py` & `godoo_cli-0.5.1/src/godoo_cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/git/git_odoo.py` & `godoo_cli-0.5.1/src/godoo_cli/git/git_odoo.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/git/git_odoo_addons.py` & `godoo_cli-0.5.1/src/godoo_cli/git/git_odoo_addons.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/git/git_repo.py` & `godoo_cli-0.5.1/src/godoo_cli/git/git_repo.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/git/git_url.py` & `godoo_cli-0.5.1/src/godoo_cli/git/git_url.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/git/zip_download.py` & `godoo_cli-0.5.1/src/godoo_cli/git/zip_download.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/helpers/bootstrap.py` & `godoo_cli-0.5.1/src/godoo_cli/helpers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/helpers/odoo_files.py` & `godoo_cli-0.5.1/src/godoo_cli/helpers/odoo_files.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/helpers/odoo_manifest.py` & `godoo_cli-0.5.1/src/godoo_cli/helpers/odoo_manifest.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/src/godoo_cli/helpers/system.py` & `godoo_cli-0.5.1/src/godoo_cli/helpers/system.py`

 * *Files identical despite different names*

### Comparing `godoo_cli-0.5.0/PKG-INFO` & `godoo_cli-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godoo-cli
-Version: 0.5.0
+Version: 0.5.1
 Summary: Wrapper around Odoo-Bin with some convinience RPC functions.
 Home-page: https://github.com/OpenJKSoftware/gOdoo
 License: LGPL-3
 Keywords: odoo,godoo,devcontainer
 Author: Joshua Kreuder
 Author-email: Joshua_Kreuder@outlook.com
 Requires-Python: >=3.8.1,<3.12
```

