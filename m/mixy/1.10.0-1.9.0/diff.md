# Comparing `tmp/mixy-1.10.0.tar.gz` & `tmp/mixy-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixy-1.10.0.tar", max compression
+gzip compressed data, was "mixy-1.9.0.tar", max compression
```

## Comparing `mixy-1.10.0.tar` & `mixy-1.9.0.tar`

### file list

```diff
@@ -1,45 +1,43 @@
--rw-r--r--   0        0        0     1072 2023-06-20 01:22:54.078996 mixy-1.10.0/LICENSE
--rw-r--r--   0        0        0     1962 2023-06-20 01:22:54.078996 mixy-1.10.0/README.md
--rw-r--r--   0        0        0       48 2023-06-20 01:23:17.115489 mixy-1.10.0/mixy/__init__.py
--rw-r--r--   0        0        0      474 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/cache_handler.py
--rw-r--r--   0        0        0      981 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/cached_vars_handler.py
--rw-r--r--   0        0        0     3859 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/cli.py
--rw-r--r--   0        0        0      932 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/constants.py
--rw-r--r--   0        0        0     1280 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/context.py
--rw-r--r--   0        0        0     1185 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/exceptions.py
--rw-r--r--   0        0        0      868 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/git_manager.py
--rw-r--r--   0        0        0      596 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/github_manager.py
--rw-r--r--   0        0        0     2290 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/logger_builder.py
--rw-r--r--   0        0        0      508 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/merge_strategies.py
--rw-r--r--   0        0        0        0 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/models/__init__.py
--rw-r--r--   0        0        0     2816 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/models/base.py
--rw-r--r--   0        0        0     1824 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/models/directory_dependency.py
--rw-r--r--   0        0        0      765 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/models/file_dependency.py
--rw-r--r--   0        0        0     1520 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/models/git_dependency.py
--rw-r--r--   0        0        0      239 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/models/log_level.py
--rw-r--r--   0        0        0      970 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/models/mixy_dependency.py
--rw-r--r--   0        0        0      175 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/models/mixy_file.py
--rw-r--r--   0        0        0     1628 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/models/project.py
--rw-r--r--   0        0        0      208 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/models/template_var.py
--rw-r--r--   0        0        0      391 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/preloaded_resolver.py
--rw-r--r--   0        0        0      420 2023-06-20 01:22:54.078996 mixy-1.10.0/mixy/prompt_resolver.py
--rw-r--r--   0        0        0        0 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/protocols/__init__.py
--rw-r--r--   0        0        0      232 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/protocols/dependency.py
--rw-r--r--   0        0        0      373 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/protocols/git_manager_protocol.py
--rw-r--r--   0        0        0      250 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/protocols/merge_strategy.py
--rw-r--r--   0        0        0      241 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/protocols/mergeable.py
--rw-r--r--   0        0        0      186 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/protocols/renderable.py
--rw-r--r--   0        0        0      540 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/protocols/repository_provider.py
--rw-r--r--   0        0        0      242 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/protocols/resolver_protocol.py
--rw-r--r--   0        0        0      276 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/protocols/var_protocol.py
--rw-r--r--   0        0        0      355 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/protocols/vars_handler_protocol.py
--rw-r--r--   0        0        0        0 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/settings/__init__.py
--rw-r--r--   0        0        0      210 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/settings/cache_settings.py
--rw-r--r--   0        0        0      215 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/settings/jinja_settings.py
--rw-r--r--   0        0        0      611 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/settings/logging_settings.py
--rw-r--r--   0        0        0      173 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/settings/project_settings.py
--rw-r--r--   0        0        0     1524 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/settings/settings.py
--rw-r--r--   0        0        0      838 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/settings/sources.py
--rw-r--r--   0        0        0     7936 2023-06-20 01:22:54.082996 mixy-1.10.0/mixy/utils.py
--rw-r--r--   0        0        0     1243 2023-06-20 01:23:17.127489 mixy-1.10.0/pyproject.toml
--rw-r--r--   0        0        0     2682 1970-01-01 00:00:00.000000 mixy-1.10.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-15 17:56:45.162233 mixy-1.9.0/LICENSE
+-rw-r--r--   0        0        0     1149 2023-04-15 17:56:45.162233 mixy-1.9.0/README.md
+-rw-r--r--   0        0        0       47 2023-04-15 17:57:06.126198 mixy-1.9.0/mixy/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/builders/__init__.py
+-rw-r--r--   0        0        0     1987 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/builders/logger_builder.py
+-rw-r--r--   0        0        0     3894 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/cli.py
+-rw-r--r--   0        0        0      932 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/constants.py
+-rw-r--r--   0        0        0      600 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/context.py
+-rw-r--r--   0        0        0     1185 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/exceptions.py
+-rw-r--r--   0        0        0     1296 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/git_repository.py
+-rw-r--r--   0        0        0     1035 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/github_repository.py
+-rw-r--r--   0        0        0      465 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/merge_strategies.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/models/__init__.py
+-rw-r--r--   0        0        0     2782 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/models/base.py
+-rw-r--r--   0        0        0     1170 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/models/directory_dependency.py
+-rw-r--r--   0        0        0      765 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/models/file_dependency.py
+-rw-r--r--   0        0        0     1223 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/models/git_dependency.py
+-rw-r--r--   0        0        0     1317 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/models/github_dependency.py
+-rw-r--r--   0        0        0      239 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/models/log_level.py
+-rw-r--r--   0        0        0     1550 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/models/project.py
+-rw-r--r--   0        0        0     1658 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/models/project_variables.py
+-rw-r--r--   0        0        0     1420 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/preloaded_resolver.py
+-rw-r--r--   0        0        0     1960 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/prompt_resolver.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/protocols/__init__.py
+-rw-r--r--   0        0        0      331 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/protocols/basic_resolver.py
+-rw-r--r--   0        0        0      183 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/protocols/choices_resolver.py
+-rw-r--r--   0        0        0      232 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/protocols/dependency.py
+-rw-r--r--   0        0        0      250 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/protocols/merge_strategy.py
+-rw-r--r--   0        0        0      241 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/protocols/mergeable.py
+-rw-r--r--   0        0        0      186 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/protocols/renderable.py
+-rw-r--r--   0        0        0      540 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/protocols/repository_provider.py
+-rw-r--r--   0        0        0      162 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/protocols/secrets_resolver.py
+-rw-r--r--   0        0        0      294 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/protocols/variable_resolver.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/settings/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/settings/cache_settings.py
+-rw-r--r--   0        0        0      215 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/settings/jinja_settings.py
+-rw-r--r--   0        0        0      611 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/settings/logging_settings.py
+-rw-r--r--   0        0        0      173 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/settings/project_settings.py
+-rw-r--r--   0        0        0     1524 2023-04-15 17:56:45.162233 mixy-1.9.0/mixy/settings/settings.py
+-rw-r--r--   0        0        0      838 2023-04-15 17:56:45.166233 mixy-1.9.0/mixy/settings/sources.py
+-rw-r--r--   0        0        0     7945 2023-04-15 17:56:45.166233 mixy-1.9.0/mixy/utils.py
+-rw-r--r--   0        0        0     1278 2023-04-15 17:57:06.134198 mixy-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1868 1970-01-01 00:00:00.000000 mixy-1.9.0/PKG-INFO
```

### Comparing `mixy-1.10.0/LICENSE` & `mixy-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mixy-1.10.0/mixy/cli.py` & `mixy-1.9.0/mixy/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,57 @@
-from enum import Enum
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any
 
 import tomllib
 import typer
 import yaml
 from jinja2 import Environment, StrictUndefined
 
+from mixy.builders.logger_builder import LoggerBuilder
 from mixy.context import Context
-from mixy.exceptions import MissingProjectConfigurationError, ProjectAlreadyExistsError
-from mixy.logger_builder import LoggerBuilder
+from mixy.exceptions import (
+    MissingProjectConfigurationError,
+    ProjectAlreadyExistsError,
+)
 from mixy.models.project import Project
 from mixy.preloaded_resolver import PreloadedResolver
+from mixy.prompt_resolver import PromptResolver
+from mixy.protocols.variable_resolver import VariableResolver
 from mixy.settings.project_settings import ProjectSettings
 from mixy.settings.settings import settings
 from mixy.utils import clear_directory
 
 app = typer.Typer(pretty_exceptions_show_locals=False)
 logger = LoggerBuilder.with_settings(settings.logs, __name__)
 
 
-class SupportedConfigFormat(Enum):
-    YAML = (".yaml", ".yml")
-    TOML = ".toml"
-
-
 def update_settings(project_settings: ProjectSettings) -> None:
     logger.info("Updating the settings with project settings")
     settings.jinja.merge_with(project_settings.jinja)
 
 
-def load_file_data(config_file: Path) -> dict:
-    if config_file.suffix in SupportedConfigFormat.YAML.value:
-        with config_file.open() as file:
-            return yaml.safe_load(file) or {}
-    elif config_file.suffix == SupportedConfigFormat.TOML.value:
-        return tomllib.loads(config_file.read_text()) or {}
-    else:
-        raise ValueError("Unsupported project configuration format.")
-
-
-def validate_and_get_project(destination: Path, config_file: Path) -> Project:
+def get_project(destination: Path, config_file: Path) -> Project:
     if not config_file.is_file():
         raise MissingProjectConfigurationError(config_file)
 
     logger.info(f"Reading the project from {config_file}")
-    project_config = load_file_data(config_file)
+    if config_file.suffix in (".yaml", ".yml"):
+        project_config = yaml.safe_load(config_file.open()) or {}
+    elif config_file.suffix == ".toml":
+        project_config = tomllib.loads(config_file.read_text()) or {}
+    else:
+        # TODO make this a custom exception
+        raise Exception("Unsupported project configuration format.")
     return Project(destination=destination, **project_config)
 
 
-def check_and_empty_project(force: bool, project: Project) -> None:
-    if force:
-        logger.info("The force option was used, emptying the project")
-        project.empty()
-
-    if not project.is_empty:
-        raise ProjectAlreadyExistsError(project.destination)
-
-
-def create_project(project: Project, context: Optional[Path] = None) -> None:
-    update_settings(project.settings)
-    ctx = Context(env=Environment(undefined=StrictUndefined, **settings.jinja.dict()))
-
-    if context is not None:
-        logger.info(f"Importing the provided context: {context}")
-        context_data: dict[str, Any] = yaml.safe_load(context.read_text()) or {}
-        ctx.resolver = PreloadedResolver(context_data)
-
-    logger.info("Creating the project")
-    project.create(ctx)
+def resolve_missing_variables(
+    config: Project, resolver: VariableResolver
+) -> dict[str, Any]:
+    return config.variables.resolve(resolver)
 
 
 @app.command(help="Create a new project.")
 def create(
     project_file: Path,
     destination: Path,
     context: Path = typer.Option(
@@ -80,37 +59,61 @@
         "--context",
         "-c",
         help="Use a YAML file to resolve the project variables.",
     ),
     force: bool = typer.Option(
         False, "--force", "-f", help="Overwrite the project if it already exists."
     ),
-) -> None:
+):
     try:
         logger.info(f"Creating the project using: {project_file.absolute()}")
-        project = validate_and_get_project(destination, project_file)
-        check_and_empty_project(force, project)
-        create_project(project, context)
+        project = get_project(destination, project_file)
+        project.destination = destination
+
+        if force:
+            logger.info("The force option was used, emptying the project")
+            project.empty()
+
+        if not project.is_empty:
+            raise ProjectAlreadyExistsError(project.destination)
+
+        update_settings(project.settings)
+        ctx = Context(
+            env=Environment(undefined=StrictUndefined, **settings.jinja.dict())
+        )
+
+        if context is not None:
+            logger.info(f"Importing the provided context: {context}")
+            context_data: dict[str, Any] = yaml.safe_load(context.read_text()) or {}
+            ctx.update(
+                **resolve_missing_variables(project, PreloadedResolver(context_data))
+            )
+        else:
+            logger.info("Resolving missing variables")
+            ctx.update(**resolve_missing_variables(project, PromptResolver()))
+
+        logger.info("Rendering the project")
+        project = project.render(ctx)
+
+        logger.info("Resolving dependencies")
+        project.resolve_dependencies(ctx)
+
         logger.info("Project creation complete")
-    except (
-        typer.Abort,
-        MissingProjectConfigurationError,
-        ProjectAlreadyExistsError,
-    ) as e:
-        logger.error(f"Project creation failed: {str(e)}")
-    except Exception as e:
-        logger.exception(f"Unexpected error occurred while creating project: {e}")
+    except typer.Abort as e:
+        raise e
+    except Exception:
+        logger.exception("Project creation failed")
 
     if not settings.cache.enabled:
         logger.info("Cache is disabled, removing the cached dependencies")
         clear()
 
 
 @app.command(help="Clear the program's cache.")
-def clear() -> None:
+def clear():
     logger.info("Clearing the cache")
     clear_directory(settings.cache.location)
     logger.info("Cache cleared successfully")
 
 
 def main() -> None:
     app()
```

### Comparing `mixy-1.10.0/mixy/constants.py` & `mixy-1.9.0/mixy/constants.py`

 * *Files identical despite different names*

### Comparing `mixy-1.10.0/mixy/exceptions.py` & `mixy-1.9.0/mixy/exceptions.py`

 * *Files identical despite different names*

### Comparing `mixy-1.10.0/mixy/git_manager.py` & `mixy-1.9.0/mixy/git_repository.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,43 @@
-from dataclasses import dataclass
 from pathlib import Path
 from typing import Self
 
 from git.repo import Repo
 
 
-@dataclass
-class GitManager:
-    repo: Repo
+class GitRepository(Repo):
+    def is_branch_behind(self, branch: str) -> bool:
+        local_branch = self.heads[branch]
+        remote_branch = local_branch.tracking_branch()
+        if remote_branch is None:
+            return False
+        self.remote().fetch()
+        commits_behind = self.iter_commits(f"{local_branch}..{remote_branch}")
+        return next(commits_behind, None) is not None
 
     @property
     def location(self) -> Path | None:
-        loc = self.repo.working_tree_dir
+        loc = self.working_tree_dir
         return None if loc is None else Path(loc)
 
     @classmethod
     def cache_or_clone(cls, url: str, dest: Path) -> Self:
         if dest.is_dir():
-            return cls(Repo(dest))
-        repo = Repo.clone_from(url, dest)
-        return cls(repo)
+            return cls(dest)
+        repo = cls.clone_from(url, dest)
+        return cls(repo.common_dir)
 
     def checkout(self, version: str) -> None:
-        self.repo.git.checkout(version)
+        self.git.checkout(version)
 
     def fetch(self, tags: bool = True) -> None:
-        self.repo.remotes.origin.fetch(tags=tags)
+        self.remotes.origin.fetch(tags=tags)
 
     def pull(self, tags: bool = True) -> None:
-        if self.repo.head.is_detached:
-            self.repo.git.checkout("-")
-        self.repo.remotes.origin.pull(tags=tags)
+        if self.head.is_detached:
+            self.git.checkout("-")
+        self.remotes.origin.pull(tags=tags)
+
+    def sync(self) -> None:
+        self.fetch()
+        if self.is_branch_behind(self.active_branch.name):
+            self.pull()
```

### Comparing `mixy-1.10.0/mixy/logger_builder.py` & `mixy-1.9.0/mixy/builders/logger_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import logging
 import os
 import sys
 from pathlib import Path
-from typing import Self, TextIO
+from typing import TextIO
 
 from mixy.models.log_level import LogLevel
 from mixy.settings.logging_settings import LoggingSettings
 
 
 class LoggerBuilder:
     def __init__(self, name: str, level: LogLevel = LogLevel.DEBUG) -> None:
         self.name = name
         self.level = level
         self.logger = logging.getLogger(self.name)
-        self.logger.setLevel(
-            self.level.value if self.level.value is not None else logging.NOTSET
-        )
+        self.logger.setLevel(self.level.value)
 
     @staticmethod
     def with_settings(
         settings: LoggingSettings, name: str, level: LogLevel = LogLevel.DEBUG
     ) -> logging.Logger:
         builder = LoggerBuilder(name, level)
         if settings.file_level != LogLevel.DISABLED:
@@ -31,34 +29,30 @@
                 settings.console_level, settings.logging_format
             )
         return builder.build()
 
     def _configure_handler(
         self, handler: logging.Handler, level: LogLevel, log_format: str
     ) -> None:
-        handler.setLevel(level.value if level.value is not None else logging.NOTSET)
+        handler.setLevel(level.value)
         handler.setFormatter(logging.Formatter(log_format))
 
     def with_console_logging(
         self, level: LogLevel, log_format: str, stream: TextIO = ...
-    ) -> Self:
+    ) -> "LoggerBuilder":
         stream = sys.stderr if stream is ... else stream
         handler = logging.StreamHandler(stream)
         self._configure_handler(handler, level, log_format)
         self.logger.addHandler(handler)
         return self
 
-    def with_file_logging(self, dest: Path, level: LogLevel, log_format: str) -> Self:
-        dest = Path(dest)
-        try:
-            os.makedirs(dest.parent, exist_ok=True)
-            handler = logging.FileHandler(dest)
-        except Exception as e:
-            raise Exception(
-                f"Failed to setup file handler at location {dest}. Error: {str(e)}"
-            ) from e
+    def with_file_logging(
+        self, dest: Path, level: LogLevel, log_format: str
+    ) -> "LoggerBuilder":
+        os.makedirs(dest.parent, exist_ok=True)
+        handler = logging.FileHandler(dest)
         self._configure_handler(handler, level, log_format)
         self.logger.addHandler(handler)
         return self
 
     def build(self) -> logging.Logger:
         return self.logger
```

### Comparing `mixy-1.10.0/mixy/models/base.py` & `mixy-1.9.0/mixy/models/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 
     def _recursive_render(self, obj: Any, context: Context) -> Any:
         if isinstance(obj, str):
             return context.render(obj)
         elif isinstance(obj, Path):
             return Path(context.render(str(obj)))
         elif isinstance(obj, RenderableBaseModel):
-            obj.render(context)
-            return obj
+            return obj.render(context)
         elif isinstance(obj, dict):
             return {k: self._recursive_render(v, context) for k, v in obj.items()}
         elif isinstance(obj, list):
             return [self._recursive_render(x, context) for x in obj]
         elif hasattr(obj, "__dict__"):
             fields: dict[str, Any] = obj.__dict__
             for k, v in fields.items():
@@ -46,38 +45,38 @@
                     continue
                 new_value = self._recursive_render(v, context)
                 setattr(obj, k, new_value)
             return obj
         else:
             return obj
 
-    def render(self, context: Context) -> None:
+    def render(self, context: Context) -> Self:
         templated = self.dict(
             exclude={name: True for name in self._RENDERABLE_EXCLUDES}
         )
         not_templated = self.dict(
             include={name: True for name in self._RENDERABLE_EXCLUDES}
         )
         resolved_templated = self._recursive_render(templated, context)
         resolved: dict[str, Any] = {
             **resolved_templated,
             **not_templated,
         }
-        self.merge_with(self.__class__(**resolved))
+        return self.__class__(**resolved)
 
 
 class NameBasedEnum(Enum):
     @classmethod
     def __get_validators__(cls):
         cls.name_lookup = {k: v for k, v in cls.__members__.items()}
         cls.value_lookup = {v.value: v for _, v in cls.__members__.items()}
         yield cls.validate
 
     @classmethod
-    def validate(cls, v) -> Self:
+    def validate(cls, v):
         if isinstance(v, cls):
             return v
         if v in cls.value_lookup:
             return cls.value_lookup[v]
         if v in cls.name_lookup:
             return cls.name_lookup[v]
```

### Comparing `mixy-1.10.0/mixy/models/directory_dependency.py` & `mixy-1.9.0/mixy/models/directory_dependency.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,34 @@
 from pathlib import Path
 from typing import Iterator, Literal
 
-import tomllib
 from pydantic.types import DirectoryPath
 
 from mixy.context import Context
-from mixy.models.mixy_dependency import MixyDependency
 from mixy.protocols.dependency import Dependency
 from mixy.utils import get_directory_contents, join_local_path
 
 from .base import RenderableBaseModel
 from .file_dependency import FileDependency
-from .template_var import TemplateVar
 
 
 class DirectoryDependency(RenderableBaseModel):
     src_type: Literal["directory"] = "directory"
     src: DirectoryPath
-    dest: Path = Path("/")
-    ignores: list[str] = [".mixy"]
+    dest: Path
+    ignores: list[str] = []
 
     @property
     def iter_dependencies(self) -> Iterator[Dependency]:
         dir_content = get_directory_contents(self.src, self.ignores)
         for x in dir_content:
             dest = Path("/").joinpath(x.relative_to(self.src))
             if x.is_dir():
                 yield DirectoryDependency(src=x, dest=dest, ignores=self.ignores)
-            elif x.suffix == ".mixy":
-                yield MixyDependency(src=x, dest=dest)
             else:
                 yield FileDependency(src=x, dest=dest)
 
-    def _load_template_vars(self, vars_file: Path) -> dict[str, TemplateVar]:
-        with open(vars_file, "rb") as f:
-            data = tomllib.load(f)
-        return {k: TemplateVar(**v) for k, v in data.items()}
-
     def resolve(self, into_dir: Path, context: Context) -> None:
         abs_dest = join_local_path(into_dir, self.dest)
         abs_dest.mkdir(exist_ok=True, parents=True)
-        vars_file = self.src / ".mixy" / "vars.toml"
-        if vars_file.exists():
-            template_vars = self._load_template_vars(vars_file)
-            context = Context.derive_from(context, **template_vars)
-
         for d in self.iter_dependencies:
             d.resolve(abs_dest, context)
```

### Comparing `mixy-1.10.0/mixy/models/file_dependency.py` & `mixy-1.9.0/mixy/models/file_dependency.py`

 * *Files identical despite different names*

### Comparing `mixy-1.10.0/mixy/models/project.py` & `mixy-1.9.0/mixy/models/project.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,52 +5,45 @@
 from typing_extensions import Annotated
 
 from mixy.context import Context
 from mixy.models.base import RenderableBaseModel
 from mixy.models.directory_dependency import DirectoryDependency
 from mixy.models.file_dependency import FileDependency
 from mixy.models.git_dependency import GitDependency
-from mixy.models.mixy_dependency import MixyDependency
-from mixy.models.template_var import TemplateVar
+from mixy.models.github_dependency import GitHubDependency
+from mixy.models.project_variables import ProjectVariables
 from mixy.settings.project_settings import ProjectSettings
 from mixy.utils import clear_directory
 
 ProjectDependency = Annotated[
-    Union[
-        DirectoryDependency,
-        FileDependency,
-        GitDependency,
-        MixyDependency,
-    ],
+    Union[DirectoryDependency, FileDependency, GitDependency, GitHubDependency],
     Field(discriminator="src_type"),
 ]
 
 
 class Project(RenderableBaseModel):
-    _RENDERABLE_EXCLUDES = {"settings", "vars"}
+    _RENDERABLE_EXCLUDES = {"settings", "variables"}
 
     dependencies: list[ProjectDependency]
     destination: Path
 
     settings: ProjectSettings = ProjectSettings()
-    vars: dict[str, TemplateVar] = {}
+    variables: ProjectVariables = ProjectVariables()
 
     @property
     def exists(self) -> bool:
         return self.destination.exists()
 
     @property
     def is_empty(self) -> bool:
         if not self.exists:
             return True
         return not any(self.destination.iterdir())
 
-    def create(self, context: Context) -> None:
-        context = Context.derive_from(context, **self.vars)
-        self.render(context)
+    def resolve_dependencies(self, context: Context) -> None:
         self.destination.mkdir(exist_ok=True)
         for dependency in self.dependencies:
             dependency.resolve(self.destination, context)
 
     def empty(self) -> None:
         if self.exists:
             clear_directory(self.destination)
```

### Comparing `mixy-1.10.0/mixy/protocols/repository_provider.py` & `mixy-1.9.0/mixy/protocols/repository_provider.py`

 * *Files identical despite different names*

### Comparing `mixy-1.10.0/mixy/settings/logging_settings.py` & `mixy-1.9.0/mixy/settings/logging_settings.py`

 * *Files identical despite different names*

### Comparing `mixy-1.10.0/mixy/settings/settings.py` & `mixy-1.9.0/mixy/settings/settings.py`

 * *Files identical despite different names*

### Comparing `mixy-1.10.0/mixy/settings/sources.py` & `mixy-1.9.0/mixy/settings/sources.py`

 * *Files identical despite different names*

### Comparing `mixy-1.10.0/mixy/utils.py` & `mixy-1.9.0/mixy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import re
 import shutil
 import subprocess
 from datetime import datetime, timezone, tzinfo
 from pathlib import Path
 from typing import Any, Iterable, Iterator, List, Mapping, Optional
 
-from mixy.constants import GIT_PROTOCOLS_PREFIXES
+from mixy.constants import (
+    GIT_PROTOCOLS_PREFIXES,
+)
 from mixy.exceptions import InvalidCommandError
 
 
 def extract_repo_name(url: str) -> str:
     """
     Extracts the repository name from a given URL.
```

### Comparing `mixy-1.10.0/pyproject.toml` & `mixy-1.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "mixy"
-version = "1.10.0"
+version = "1.9.0"
 description = ""
 authors = ["Alexis Beaulieu <alexisbeaulieu97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/alexisbeaulieu97/Mixy"
 repository = "https://github.com/alexisbeaulieu97/Mixy"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 jinja2 = "^3.1.2"
-typer = { extras = ["all"], version = "^0.7.0" }
+typer = {extras = ["all"], version = "^0.7.0"}
 pyyaml = "^6.0"
 pydantic = "^1.10.2"
 requests = "^2.28.1"
 gitpython = "^3.1.29"
 
 
 [tool.poetry.group.dev.dependencies]
@@ -27,22 +27,23 @@
 pytest-cov = "^4.0.0"
 pylint = "^2.15.9"
 flake8 = "^6.0.0"
 pyfakefs = "^5.0.0"
 vulture = "^2.7"
 pytest-mock = "^3.10.0"
 semgrep = "^1.14.0"
-bandit = { extras = ["toml"], version = "^1.7.4" }
+bandit = {extras = ["toml"], version = "^1.7.4"}
 
 [tool.poetry.scripts]
 mixy = "mixy.cli:main"
 
 [tool.semantic_release]
 version_variable = ["mixy/__init__.py:__version__"]
 version_toml = ["pyproject.toml:tool.poetry.version"]
+version_pattern = ["VERSION:{version}"]
 branch = "main"
 upload_to_repository = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 
 [build-system]
 requires = ["poetry-core"]
```

