# Comparing `tmp/commitizen-3.3.0.tar.gz` & `tmp/commitizen-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.3.0.tar", max compression
+gzip compressed data, was "commitizen-3.4.0.tar", max compression
```

## Comparing `commitizen-3.3.0.tar` & `commitizen-3.4.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-06-13 15:08:53.658482 commitizen-3.3.0/LICENSE
--rw-r--r--   0        0        0      609 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/__version__.py
--rw-r--r--   0        0        0     8543 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/bump.py
--rw-r--r--   0        0        0    11894 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/changelog.py
--rw-r--r--   0        0        0     3455 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    16940 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    13915 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/bump.py
--rw-r--r--   0        0        0     7269 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5075 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/check.py
--rw-r--r--   0        0        0     3435 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/info.py
--rw-r--r--   0        0        0    12935 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/commands/version.py
--rw-r--r--   0        0        0     1235 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/config/__init__.py
--rw-r--r--   0        0        0      898 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1568 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1746 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1431 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1213 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     2983 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7115 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3121 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      287 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3272 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/defaults.py
--rw-r--r--   0        0        0     4575 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/factory.py
--rw-r--r--   0        0        0     6900 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/out.py
--rw-r--r--   0        0        0     7014 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     2376 2023-06-13 15:08:53.658482 commitizen-3.3.0/commitizen/version_types.py
--rw-r--r--   0        0        0     5750 2023-06-13 15:08:53.658482 commitizen-3.3.0/docs/README.md
--rw-r--r--   0        0        0     3938 2023-06-13 15:08:53.670482 commitizen-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-20 08:11:51.512833 commitizen-3.4.0/LICENSE
+-rw-r--r--   0        0        0      609 2023-06-20 08:11:51.512833 commitizen-3.4.0/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-20 08:11:51.512833 commitizen-3.4.0/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-20 08:11:51.512833 commitizen-3.4.0/commitizen/__version__.py
+-rw-r--r--   0        0        0     4609 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/bump.py
+-rw-r--r--   0        0        0    11712 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/changelog.py
+-rw-r--r--   0        0        0     3455 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    17490 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    13971 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7142 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5075 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3435 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/info.py
+-rw-r--r--   0        0        0    12966 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1235 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1568 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1746 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1431 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1213 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     2983 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7070 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3121 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      287 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3176 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/defaults.py
+-rw-r--r--   0        0        0     4706 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/factory.py
+-rw-r--r--   0        0        0     6900 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/out.py
+-rw-r--r--   0        0        0     7109 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     9690 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/version_schemes.py
+-rw-r--r--   0        0        0     5750 2023-06-20 08:11:51.516833 commitizen-3.4.0/docs/README.md
+-rw-r--r--   0        0        0     4202 2023-06-20 08:11:51.528833 commitizen-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.4.0/PKG-INFO
```

### Comparing `commitizen-3.3.0/LICENSE` & `commitizen-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/__init__.py` & `commitizen-3.4.0/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/changelog.py` & `commitizen-3.4.0/commitizen/changelog.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,61 +20,49 @@
 - [x] Generate full or partial changelog
 - [x] Include in tree from file all the extra comments added manually
 - [x] Add unreleased value
 - [x] hook after message is parsed (add extra information like hyperlinks)
 - [x] hook after changelog is generated (api calls)
 - [x] add support for change_type maps
 """
-
 from __future__ import annotations
 
 import os
 import re
-import sys
-import typing
 from collections import OrderedDict, defaultdict
 from datetime import date
-from typing import Callable, Iterable
+from typing import TYPE_CHECKING, Callable, Iterable, cast
 
 from jinja2 import Environment, PackageLoader
-from packaging.version import InvalidVersion, Version
 
-from commitizen import defaults
 from commitizen.bump import normalize_tag
 from commitizen.exceptions import InvalidConfigurationError, NoCommitsFoundError
 from commitizen.git import GitCommit, GitTag
+from commitizen.version_schemes import DEFAULT_SCHEME, Pep440, InvalidVersion
 
-if sys.version_info >= (3, 8):
-    from commitizen.version_types import VersionProtocol
-else:
-    # workaround mypy issue for 3.7 python
-    VersionProtocol = typing.Any
+if TYPE_CHECKING:
+    from commitizen.version_schemes import VersionScheme
 
 
 def get_commit_tag(commit: GitCommit, tags: list[GitTag]) -> GitTag | None:
     return next((tag for tag in tags if tag.rev == commit.rev), None)
 
 
-def get_version(tag: GitTag) -> Version | None:
-    version = None
-    try:
-        version = Version(tag.name)
-    except InvalidVersion:
-        pass
-    return version
-
-
 def tag_included_in_changelog(
-    tag: GitTag, used_tags: list, merge_prerelease: bool
+    tag: GitTag,
+    used_tags: list,
+    merge_prerelease: bool,
+    scheme: VersionScheme = DEFAULT_SCHEME,
 ) -> bool:
     if tag in used_tags:
         return False
 
-    version = get_version(tag)
-    if version is None:
+    try:
+        version = scheme(tag.name)
+    except InvalidVersion:
         return False
 
     if merge_prerelease and version.is_prerelease:
         return False
 
     return True
 
@@ -84,14 +72,15 @@
     tags: list[GitTag],
     commit_parser: str,
     changelog_pattern: str,
     unreleased_version: str | None = None,
     change_type_map: dict[str, str] | None = None,
     changelog_message_builder_hook: Callable | None = None,
     merge_prerelease: bool = False,
+    scheme: VersionScheme = DEFAULT_SCHEME,
 ) -> Iterable[dict]:
     pat = re.compile(changelog_pattern)
     map_pat = re.compile(commit_parser, re.MULTILINE)
     body_map_pat = re.compile(commit_parser, re.MULTILINE | re.DOTALL)
     current_tag: GitTag | None = None
 
     # Check if the latest commit is not tagged
@@ -109,15 +98,15 @@
 
     changes: dict = defaultdict(list)
     used_tags: list = [current_tag]
     for commit in commits:
         commit_tag = get_commit_tag(commit, tags)
 
         if commit_tag is not None and tag_included_in_changelog(
-            commit_tag, used_tags, merge_prerelease
+            commit_tag, used_tags, merge_prerelease, scheme=scheme
         ):
             used_tags.append(commit_tag)
             yield {
                 "version": current_tag_name,
                 "date": current_tag_date,
                 "changes": changes,
             }
@@ -182,32 +171,34 @@
     loader = PackageLoader("commitizen", "templates")
     env = Environment(loader=loader, trim_blocks=True)
     jinja_template = env.get_template("keep_a_changelog_template.j2")
     changelog: str = jinja_template.render(tree=tree)
     return changelog
 
 
-def parse_version_from_markdown(value: str) -> str | None:
+def parse_version_from_markdown(
+    value: str, scheme: VersionScheme = Pep440
+) -> str | None:
     if not value.startswith("#"):
         return None
-    m = re.search(defaults.version_parser, value)
+    m = scheme.parser.search(value)
     if not m:
         return None
-    return m.groupdict().get("version")
+    return cast(str, m.group("version"))
 
 
 def parse_title_type_of_line(value: str) -> str | None:
     md_title_parser = r"^(?P<title>#+)"
     m = re.search(md_title_parser, value)
     if not m:
         return None
     return m.groupdict().get("title")
 
 
-def get_metadata(filepath: str) -> dict:
+def get_metadata(filepath: str, scheme: VersionScheme = Pep440) -> dict:
     unreleased_start: int | None = None
     unreleased_end: int | None = None
     unreleased_title: str | None = None
     latest_version: str | None = None
     latest_version_position: int | None = None
     if not os.path.isfile(filepath):
         return {
@@ -232,15 +223,15 @@
             elif (
                 isinstance(unreleased_title, str)
                 and parse_title_type_of_line(line) == unreleased_title
             ):
                 unreleased_end = index
 
             # Try to find the latest release done
-            version = parse_version_from_markdown(line)
+            version = parse_version_from_markdown(line, scheme)
             if version:
                 latest_version = version
                 latest_version_position = index
                 break  # there's no need for more info
         if unreleased_start is not None and unreleased_end is None:
             unreleased_end = index
     return {
@@ -324,38 +315,34 @@
     return accumulator
 
 
 def get_oldest_and_newest_rev(
     tags: list[GitTag],
     version: str,
     tag_format: str,
-    version_type_cls: type[VersionProtocol] | None = None,
+    scheme: VersionScheme | None = None,
 ) -> tuple[str | None, str | None]:
     """Find the tags for the given version.
 
     `version` may come in different formats:
     - `0.1.0..0.4.0`: as a range
     - `0.3.0`: as a single version
     """
     oldest: str | None = None
     newest: str | None = None
     try:
         oldest, newest = version.split("..")
     except ValueError:
         newest = version
 
-    newest_tag = normalize_tag(
-        newest, tag_format=tag_format, version_type_cls=version_type_cls
-    )
+    newest_tag = normalize_tag(newest, tag_format=tag_format, scheme=scheme)
 
     oldest_tag = None
     if oldest:
-        oldest_tag = normalize_tag(
-            oldest, tag_format=tag_format, version_type_cls=version_type_cls
-        )
+        oldest_tag = normalize_tag(oldest, tag_format=tag_format, scheme=scheme)
 
     tags_range = get_smart_tag_range(tags, newest=newest_tag, oldest=oldest_tag)
     if not tags_range:
         raise NoCommitsFoundError("Could not find a valid revision range.")
 
     oldest_rev: str | None = tags_range[-1].name
     newest_rev = newest_tag
```

### Comparing `commitizen-3.3.0/commitizen/changelog_parser.py` & `commitizen-3.4.0/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/cli.py` & `commitizen-3.4.0/commitizen/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 from functools import partial
 from types import TracebackType
 
 import argcomplete
 from decli import cli
 
-from commitizen import commands, config, out, version_types
+from commitizen import commands, config, out, version_schemes
 from commitizen.exceptions import (
     CommitizenException,
     ExitCode,
     ExpectedExit,
     NoCommandFoundError,
 )
 
@@ -201,26 +201,32 @@
                     {
                         "name": ["--prerelease-offset"],
                         "type": int,
                         "default": None,
                         "help": "start pre-releases with this offset",
                     },
                     {
+                        "name": ["--version-scheme"],
+                        "help": "choose version scheme",
+                        "default": None,
+                        "choices": version_schemes.KNOWN_SCHEMES,
+                    },
+                    {
+                        "name": ["--version-type"],
+                        "help": "Deprecated, use --version-scheme",
+                        "default": None,
+                        "choices": version_schemes.KNOWN_SCHEMES,
+                    },
+                    {
                         "name": "manual_version",
                         "type": str,
                         "nargs": "?",
                         "help": "bump to the given version (e.g: 1.5.3)",
                         "metavar": "MANUAL_VERSION",
                     },
-                    {
-                        "name": ["--version-type"],
-                        "help": "choose version type",
-                        "default": None,
-                        "choices": version_types.VERSION_TYPES,
-                    },
                 ],
             },
             {
                 "name": ["changelog", "ch"],
                 "help": (
                     "generate changelog (note that it will overwrite existing file)"
                 ),
@@ -271,14 +277,20 @@
                         "action": "store_true",
                         "default": False,
                         "help": (
                             "collect all changes from prereleases into next non-prerelease. "
                             "If not set, it will include prereleases in the changelog"
                         ),
                     },
+                    {
+                        "name": ["--version-scheme"],
+                        "help": "choose version scheme",
+                        "default": None,
+                        "choices": version_schemes.KNOWN_SCHEMES,
+                    },
                 ],
             },
             {
                 "name": ["check"],
                 "help": "validates that a commit message matches the commitizen schema",
                 "func": commands.Check,
                 "arguments": [
@@ -350,15 +362,15 @@
     },
 }
 
 original_excepthook = sys.excepthook
 
 
 def commitizen_excepthook(
-    type, value, traceback, debug=False, no_raise: list[int] = None
+    type, value, traceback, debug=False, no_raise: list[int] | None = None
 ):
     traceback = traceback if isinstance(traceback, TracebackType) else None
     if not no_raise:
         no_raise = []
     if isinstance(value, CommitizenException):
         if value.message:
             value.output_method(value.message)
```

### Comparing `commitizen-3.3.0/commitizen/cmd.py` & `commitizen-3.4.0/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/commands/bump.py` & `commitizen-3.4.0/commitizen/commands/bump.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import os
 from logging import getLogger
+import warnings
 
 import questionary
-from commitizen import bump, cmd, factory, git, hooks, out, version_types
+
+from commitizen import bump, cmd, factory, git, hooks, out
 from commitizen.commands.changelog import Changelog
 from commitizen.config import BaseConfig
 from commitizen.exceptions import (
     BumpCommitFailedError,
     BumpTagFailedError,
     DryRunExit,
     ExpectedExit,
@@ -17,15 +19,15 @@
     NoneIncrementExit,
     NoPatternMapError,
     NotAGitProjectError,
     NotAllowed,
     NoVersionSpecifiedError,
 )
 from commitizen.providers import get_provider
-from packaging.version import InvalidVersion, Version
+from commitizen.version_schemes import get_version_scheme, InvalidVersion
 
 logger = getLogger("commitizen")
 
 
 class Bump:
     """Show prompt for the user to create a guided commit."""
 
@@ -58,18 +60,25 @@
         )
         self.changelog_to_stdout = arguments["changelog_to_stdout"]
         self.no_verify = arguments["no_verify"]
         self.check_consistency = arguments["check_consistency"]
         self.retry = arguments["retry"]
         self.pre_bump_hooks = self.config.settings["pre_bump_hooks"]
         self.post_bump_hooks = self.config.settings["post_bump_hooks"]
-        version_type = arguments["version_type"] or self.config.settings.get(
-            "version_type"
+        deprecated_version_type = arguments.get("version_type")
+        if deprecated_version_type:
+            warnings.warn(
+                DeprecationWarning(
+                    "`--version-type` parameter is deprecated and will be removed in commitizen 4. "
+                    "Please use `--version-scheme` instead"
+                )
+            )
+        self.scheme = get_version_scheme(
+            self.config, arguments["version_scheme"] or deprecated_version_type
         )
-        self.version_type = version_type and version_types.VERSION_TYPES[version_type]
 
     def is_initial_tag(self, current_tag_version: str, is_yes: bool = False) -> bool:
         """Check if reading the whole git tree up to HEAD is needed."""
         is_initial = False
         if not git.tag_exist(current_tag_version):
             if is_yes:
                 is_initial = True
@@ -104,18 +113,17 @@
             commits, regex=bump_pattern, increments_map=bump_map
         )
         return increment
 
     def __call__(self):  # noqa: C901
         """Steps executed to bump."""
         provider = get_provider(self.config)
-        current_version: str = provider.get_version()
 
         try:
-            current_version_instance: Version = Version(current_version)
+            current_version = self.scheme(provider.get_version())
         except TypeError:
             raise NoVersionSpecifiedError()
 
         tag_format: str = self.bump_settings["tag_format"]
         bump_commit_message: str = self.bump_settings["bump_message"]
         version_files: list[str] = self.bump_settings["version_files"]
         major_version_zero: bool = self.bump_settings["major_version_zero"]
@@ -152,23 +160,23 @@
 
             if prerelease_offset:
                 raise NotAllowed(
                     "--prerelease-offset cannot be combined with MANUAL_VERSION"
                 )
 
         if major_version_zero:
-            if not current_version.startswith("0."):
+            if not current_version.release[0] == 0:
                 raise NotAllowed(
                     f"--major-version-zero is meaningless for current version {current_version}"
                 )
 
         current_tag_version: str = bump.normalize_tag(
             current_version,
             tag_format=tag_format,
-            version_type_cls=self.version_type,
+            scheme=self.scheme,
         )
 
         is_initial = self.is_initial_tag(current_tag_version, is_yes)
         if is_initial:
             commits = git.get_commits()
         else:
             commits = git.get_commits(current_tag_version)
@@ -176,61 +184,55 @@
         # If user specified changelog_to_stdout, they probably want the
         # changelog to be generated as well, this is the most intuitive solution
         if not self.changelog and self.changelog_to_stdout:
             self.changelog = True
 
         # No commits, there is no need to create an empty tag.
         # Unless we previously had a prerelease.
-        if not commits and not current_version_instance.is_prerelease:
+        if not commits and not current_version.is_prerelease:
             raise NoCommitsFoundError("[NO_COMMITS_FOUND]\n" "No new commits found.")
 
         if manual_version:
             try:
-                new_version = Version(manual_version)
+                new_version = self.scheme(manual_version)
             except InvalidVersion as exc:
                 raise InvalidManualVersion(
                     "[INVALID_MANUAL_VERSION]\n"
                     f"Invalid manual version: '{manual_version}'"
                 ) from exc
         else:
             if increment is None:
                 increment = self.find_increment(commits)
 
             # It may happen that there are commits, but they are not eligible
             # for an increment, this generates a problem when using prerelease (#281)
-            if (
-                prerelease
-                and increment is None
-                and not current_version_instance.is_prerelease
-            ):
+            if prerelease and increment is None and not current_version.is_prerelease:
                 raise NoCommitsFoundError(
                     "[NO_COMMITS_FOUND]\n"
                     "No commits found to generate a pre-release.\n"
                     "To avoid this error, manually specify the type of increment with `--increment`"
                 )
 
             # Increment is removed when current and next version
             # are expected to be prereleases.
-            if prerelease and current_version_instance.is_prerelease:
+            if prerelease and current_version.is_prerelease:
                 increment = None
 
-            new_version = bump.generate_version(
-                current_version,
+            new_version = current_version.bump(
                 increment,
                 prerelease=prerelease,
                 prerelease_offset=prerelease_offset,
                 devrelease=devrelease,
                 is_local_version=is_local_version,
-                version_type_cls=self.version_type,
             )
 
         new_tag_version = bump.normalize_tag(
             new_version,
             tag_format=tag_format,
-            version_type_cls=self.version_type,
+            scheme=self.scheme,
         )
         message = bump.create_commit_message(
             current_version, new_version, bump_commit_message
         )
 
         # Report found information
         information = f"{message}\n" f"tag to create: {new_tag_version}\n"
@@ -287,28 +289,28 @@
             c = cmd.run(git_add_changelog_and_version_files_command)
 
         # Do not perform operations over files or git.
         if dry_run:
             raise DryRunExit()
 
         bump.update_version_in_files(
-            current_version,
+            str(current_version),
             str(new_version),
             version_files,
             check_consistency=self.check_consistency,
         )
 
         provider.set_version(str(new_version))
 
         if self.pre_bump_hooks:
             hooks.run(
                 self.pre_bump_hooks,
                 _env_prefix="CZ_PRE_",
                 is_initial=is_initial,
-                current_version=current_version,
+                current_version=str(current_version),
                 current_tag_version=current_tag_version,
                 new_version=new_version.public,
                 new_tag_version=new_tag_version,
                 message=message,
                 increment=increment,
                 changelog_file_name=changelog_cmd.file_name if self.changelog else None,
             )
@@ -342,15 +344,15 @@
             raise BumpTagFailedError(c.err)
 
         if self.post_bump_hooks:
             hooks.run(
                 self.post_bump_hooks,
                 _env_prefix="CZ_POST_",
                 was_initial=is_initial,
-                previous_version=current_version,
+                previous_version=str(current_version),
                 previous_tag_version=current_tag_version,
                 current_version=new_version.public,
                 current_tag_version=new_tag_version,
                 message=message,
                 increment=increment,
                 changelog_file_name=changelog_cmd.file_name if self.changelog else None,
             )
```

### Comparing `commitizen-3.3.0/commitizen/commands/changelog.py` & `commitizen-3.4.0/commitizen/commands/changelog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import os.path
 from difflib import SequenceMatcher
 from operator import itemgetter
 from typing import Callable
 
-from commitizen import bump, changelog, defaults, factory, git, out, version_types
+from commitizen import bump, changelog, defaults, factory, git, out
 from commitizen.config import BaseConfig
 from commitizen.exceptions import (
     DryRunExit,
     NoCommitsFoundError,
     NoPatternMapError,
     NoRevisionError,
     NotAGitProjectError,
     NotAllowed,
 )
 from commitizen.git import GitTag, smart_open
-from packaging.version import parse
+from commitizen.version_schemes import get_version_scheme
 
 
 class Changelog:
     """Generate a changelog based on the commit history."""
 
     def __init__(self, config: BaseConfig, args):
         if not git.is_git_project():
@@ -36,20 +36,21 @@
             "changelog_file"
         )
         self.incremental = args["incremental"] or self.config.settings.get(
             "changelog_incremental"
         )
         self.dry_run = args["dry_run"]
 
-        self.current_version = (
-            args.get("current_version") or self.config.settings.get("version") or ""
-        )
-        self.current_version_instance = (
-            parse(self.current_version) if self.current_version else None
+        self.scheme = get_version_scheme(self.config, args.get("version_scheme"))
+
+        current_version = (
+            args.get("current_version", config.settings.get("version")) or ""
         )
+        self.current_version = self.scheme(current_version) if current_version else None
+
         self.unreleased_version = args["unreleased_version"]
         self.change_type_map = (
             self.config.settings.get("change_type_map") or self.cz.change_type_map
         )
         self.change_type_order = (
             self.config.settings.get("change_type_order")
             or self.cz.change_type_order
@@ -59,17 +60,14 @@
         self.tag_format = args.get("tag_format") or self.config.settings.get(
             "tag_format"
         )
         self.merge_prerelease = args.get(
             "merge_prerelease"
         ) or self.config.settings.get("changelog_merge_prerelease")
 
-        version_type = self.config.settings.get("version_type")
-        self.version_type = version_type and version_types.VERSION_TYPES[version_type]
-
     def _find_incremental_rev(self, latest_version: str, tags: list[GitTag]) -> str:
         """Try to find the 'start_rev'.
 
         We use a similarity approach. We know how to parse the version from the markdown
         changelog, but not the whole tag, we don't even know how's the tag made.
 
         This 'smart' function tries to find a similarity between the found version number
@@ -142,48 +140,48 @@
         tags = git.get_tags()
         if not tags:
             tags = []
 
         end_rev = ""
 
         if self.incremental:
-            changelog_meta = changelog.get_metadata(self.file_name)
+            changelog_meta = changelog.get_metadata(self.file_name, self.scheme)
             latest_version = changelog_meta.get("latest_version")
             if latest_version:
                 latest_tag_version: str = bump.normalize_tag(
                     latest_version,
                     tag_format=self.tag_format,
-                    version_type_cls=self.version_type,
+                    scheme=self.scheme,
                 )
                 start_rev = self._find_incremental_rev(latest_tag_version, tags)
 
         if self.rev_range:
             start_rev, end_rev = changelog.get_oldest_and_newest_rev(
                 tags,
                 version=self.rev_range,
                 tag_format=self.tag_format,
-                version_type_cls=self.version_type,
+                scheme=self.scheme,
             )
 
         commits = git.get_commits(start=start_rev, end=end_rev, args="--topo-order")
         if not commits and (
-            self.current_version_instance is None
-            or not self.current_version_instance.is_prerelease
+            self.current_version is None or not self.current_version.is_prerelease
         ):
             raise NoCommitsFoundError("No commits found")
 
         tree = changelog.generate_tree_from_commits(
             commits,
             tags,
             commit_parser,
             changelog_pattern,
             unreleased_version,
             change_type_map=change_type_map,
             changelog_message_builder_hook=changelog_message_builder_hook,
             merge_prerelease=merge_prerelease,
+            scheme=self.scheme,
         )
         if self.change_type_order:
             tree = changelog.order_changelog_tree(tree, self.change_type_order)
         changelog_out = changelog.render_changelog(tree)
         changelog_out = changelog_out.lstrip("\n")
 
         if self.dry_run:
```

### Comparing `commitizen-3.3.0/commitizen/commands/check.py` & `commitizen-3.4.0/commitizen/commands/check.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/commands/commit.py` & `commitizen-3.4.0/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/commands/init.py` & `commitizen-3.4.0/commitizen/commands/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 from commitizen import cmd, factory, out
 from commitizen.__version__ import __version__
 from commitizen.config import BaseConfig, JsonConfig, TomlConfig, YAMLConfig
 from commitizen.cz import registry
 from commitizen.defaults import config_files
 from commitizen.exceptions import InitFailedError, NoAnswersError
 from commitizen.git import get_latest_tag_name, get_tag_names, smart_open
-from commitizen.version_types import VERSION_TYPES
-from packaging.version import Version
+from commitizen.version_schemes import KNOWN_SCHEMES, Version, get_version_scheme
 
 
 class ProjectInfo:
     """Discover information about the current folder."""
 
     @property
     def has_pyproject(self) -> bool:
@@ -92,17 +91,17 @@
 
         # Collect information
         try:
             config_path = self._ask_config_path()  # select
             cz_name = self._ask_name()  # select
             version_provider = self._ask_version_provider()  # select
             tag = self._ask_tag()  # confirm & select
-            version = Version(tag)
+            version_scheme = self._ask_version_scheme()  # select
+            version = get_version_scheme(self.config, version_scheme)(tag)
             tag_format = self._ask_tag_format(tag)  # confirm & text
-            version_type = self._ask_version_type()  # select
             update_changelog_on_bump = self._ask_update_changelog_on_bump()  # confirm
             major_version_zero = self._ask_major_version_zero(version)  # confirm
         except KeyboardInterrupt:
             raise InitFailedError("Stopped by user")
 
         # Initialize configuration
         if "toml" in config_path:
@@ -110,15 +109,15 @@
         elif "json" in config_path:
             self.config = JsonConfig(data="{}", path=config_path)
         elif "yaml" in config_path:
             self.config = YAMLConfig(data="", path=config_path)
         values_to_add = {}
         values_to_add["name"] = cz_name
         values_to_add["tag_format"] = tag_format
-        values_to_add["version_type"] = version_type
+        values_to_add["version_scheme"] = version_scheme
 
         if version_provider == "commitizen":
             values_to_add["version"] = version.public
         else:
             values_to_add["version_provider"] = version_provider
 
         if update_changelog_on_bump:
@@ -249,27 +248,27 @@
             "Choose the source of the version:",
             choices=choices,
             style=self.cz.style,
             default=default,
         ).unsafe_ask()
         return version_provider
 
-    def _ask_version_type(self) -> str:
-        """Ask for setting: version_type"""
+    def _ask_version_scheme(self) -> str:
+        """Ask for setting: version_scheme"""
         default = "semver"
         if self.project_info.is_python:
             default = "pep440"
 
-        version_type: str = questionary.select(
-            "Choose version type scheme: ",
-            choices=[*VERSION_TYPES],
+        scheme: str = questionary.select(
+            "Choose version scheme: ",
+            choices=list(KNOWN_SCHEMES),
             style=self.cz.style,
             default=default,
         ).unsafe_ask()
-        return version_type
+        return scheme
 
     def _ask_major_version_zero(self, version: Version) -> bool:
         """Ask for setting: major_version_zero"""
         if version.major > 0:
             return False
         major_version_zero: bool = questionary.confirm(
             "Keep major version zero (0.x) during breaking changes",
```

### Comparing `commitizen-3.3.0/commitizen/commands/version.py` & `commitizen-3.4.0/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/config/__init__.py` & `commitizen-3.4.0/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/config/base_config.py` & `commitizen-3.4.0/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/config/json_config.py` & `commitizen-3.4.0/commitizen/config/json_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/config/toml_config.py` & `commitizen-3.4.0/commitizen/config/toml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/config/yaml_config.py` & `commitizen-3.4.0/commitizen/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/cz/__init__.py` & `commitizen-3.4.0/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/cz/base.py` & `commitizen-3.4.0/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.4.0/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 
 class ConventionalCommitsCz(BaseCommitizen):
     bump_pattern = defaults.bump_pattern
     bump_map = defaults.bump_map
     bump_map_major_version_zero = defaults.bump_map_major_version_zero
     commit_parser = defaults.commit_parser
-    version_parser = defaults.version_parser
     change_type_map = {
         "feat": "Feat",
         "fix": "Fix",
         "refactor": "Refactor",
         "perf": "Perf",
     }
     changelog_pattern = defaults.bump_pattern
```

### Comparing `commitizen-3.3.0/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.4.0/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/cz/customize/customize.py` & `commitizen-3.4.0/commitizen/cz/customize/customize.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/cz/jira/jira.py` & `commitizen-3.4.0/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/cz/jira/jira_info.txt` & `commitizen-3.4.0/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/defaults.py` & `commitizen-3.4.0/commitizen/defaults.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
 
 class Settings(TypedDict, total=False):
     name: str
     version: str | None
     version_files: list[str]
     version_provider: str | None
+    version_scheme: str | None
+    version_type: str | None
     tag_format: str | None
     bump_message: str | None
     allow_abort: bool
     changelog_file: str
     changelog_incremental: bool
     changelog_start_rev: str | None
     changelog_merge_prerelease: bool
@@ -48,15 +50,14 @@
     use_shortcuts: bool
     style: list[tuple[str, str]] | None
     customize: CzSettings
     major_version_zero: bool
     pre_bump_hooks: list[str] | None
     post_bump_hooks: list[str] | None
     prerelease_offset: int
-    version_type: str | None
 
 
 name: str = "cz_conventional_commits"
 config_files: list[str] = [
     "pyproject.toml",
     ".cz.toml",
     ".cz.json",
@@ -66,28 +67,28 @@
 ]
 
 DEFAULT_SETTINGS: Settings = {
     "name": "cz_conventional_commits",
     "version": None,
     "version_files": [],
     "version_provider": "commitizen",
+    "version_scheme": None,
     "tag_format": None,  # example v$version
     "bump_message": None,  # bumped v$current_version to $new_version
     "allow_abort": False,
     "changelog_file": "CHANGELOG.md",
     "changelog_incremental": False,
     "changelog_start_rev": None,
     "changelog_merge_prerelease": False,
     "update_changelog_on_bump": False,
     "use_shortcuts": False,
     "major_version_zero": False,
     "pre_bump_hooks": [],
     "post_bump_hooks": [],
     "prerelease_offset": 0,
-    "version_type": None,
 }
 
 MAJOR = "MAJOR"
 MINOR = "MINOR"
 PATCH = "PATCH"
 
 bump_pattern = r"^(((BREAKING[\-\ ]CHANGE|feat|fix|refactor|perf)(\(.+\))?(!)?)|\w+!):"
@@ -111,8 +112,7 @@
         (r"^perf", PATCH),
     )
 )
 change_type_order = ["BREAKING CHANGE", "Feat", "Fix", "Refactor", "Perf"]
 bump_message = "bump: version $current_version → $new_version"
 
 commit_parser = r"^((?P<change_type>feat|fix|refactor|perf|BREAKING CHANGE)(?:\((?P<scope>[^()\r\n]*)\)|\()?(?P<breaking>!)?|\w+!):\s(?P<message>.*)?"  # noqa
-version_parser = r"(?P<version>([0-9]+)\.([0-9]+)\.([0-9]+)(?:-([0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+[0-9A-Za-z-]+)?(\w+)?)"
```

### Comparing `commitizen-3.3.0/commitizen/exceptions.py` & `commitizen-3.4.0/commitizen/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     NO_INCREMENT = 21
     UNRECOGNIZED_CHARACTERSET_ENCODING = 22
     GIT_COMMAND_ERROR = 23
     INVALID_MANUAL_VERSION = 24
     INIT_FAILED = 25
     RUN_HOOK_FAILED = 26
     VERSION_PROVIDER_UNKNOWN = 27
+    VERSION_SCHEME_UNKNOWN = 28
 
 
 class CommitizenException(Exception):
     def __init__(self, *args, **kwargs):
         self.output_method = kwargs.get("output_method") or out.error
         self.exit_code = self.__class__.exit_code
         if args:
@@ -174,7 +175,11 @@
 
 class RunHookError(CommitizenException):
     exit_code = ExitCode.RUN_HOOK_FAILED
 
 
 class VersionProviderUnknown(CommitizenException):
     exit_code = ExitCode.VERSION_PROVIDER_UNKNOWN
+
+
+class VersionSchemeUnknown(CommitizenException):
+    exit_code = ExitCode.VERSION_SCHEME_UNKNOWN
```

### Comparing `commitizen-3.3.0/commitizen/factory.py` & `commitizen-3.4.0/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/git.py` & `commitizen-3.4.0/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/hooks.py` & `commitizen-3.4.0/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/out.py` & `commitizen-3.4.0/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/commitizen/providers.py` & `commitizen-3.4.0/commitizen/providers.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import re
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Any, Callable, ClassVar, cast
 
 import importlib_metadata as metadata
 import tomlkit
-from packaging.version import VERSION_PATTERN, Version
 
 from commitizen.config.base_config import BaseConfig
 from commitizen.exceptions import VersionProviderUnknown
 from commitizen.git import get_tags
+from commitizen.version_schemes import get_version_scheme
 
 PROVIDER_ENTRYPOINT = "commitizen.provider"
 DEFAULT_PROVIDER = "commitizen"
 
 
 class VersionProvider(ABC):
     """
@@ -31,22 +31,20 @@
         self.config = config
 
     @abstractmethod
     def get_version(self) -> str:
         """
         Get the current version
         """
-        ...
 
     @abstractmethod
     def set_version(self, version: str):
         """
         Set the new current version
         """
-        ...
 
 
 class CommitizenProvider(VersionProvider):
     """
     Default version provider: Fetch and set version in commitizen config.
     """
 
@@ -192,15 +190,18 @@
         "$minor": r"(?P<minor>\d+)",
         "$patch": r"(?P<patch>\d+)",
         "$prerelease": r"(?P<prerelease>\w+\d+)?",
         "$devrelease": r"(?P<devrelease>\.dev\d+)?",
     }
 
     def _tag_format_matcher(self) -> Callable[[str], str | None]:
-        pattern = self.config.settings.get("tag_format") or VERSION_PATTERN
+        version_scheme = get_version_scheme(self.config)
+        pattern = (
+            self.config.settings.get("tag_format") or version_scheme.parser.pattern
+        )
         for var, tag_pattern in self.TAG_FORMAT_REGEXS.items():
             pattern = pattern.replace(var, tag_pattern)
 
         regex = re.compile(f"^{pattern}$", re.VERBOSE)
 
         def matcher(tag: str) -> str | None:
             match = regex.match(tag)
@@ -215,16 +216,16 @@
                         groups["major"],
                         f".{groups['minor']}" if groups.get("minor") else "",
                         f".{groups['patch']}" if groups.get("patch") else "",
                         groups["prerelease"] if groups.get("prerelease") else "",
                         groups["devrelease"] if groups.get("devrelease") else "",
                     )
                 )
-            elif pattern == VERSION_PATTERN:
-                return str(Version(tag))
+            elif pattern == version_scheme.parser.pattern:
+                return str(version_scheme(tag))
             return None
 
         return matcher
 
     def get_version(self) -> str:
         matcher = self._tag_format_matcher()
         return next(
```

### Comparing `commitizen-3.3.0/docs/README.md` & `commitizen-3.4.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.3.0/pyproject.toml` & `commitizen-3.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.3.0"
+version = "3.4.0"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.3.0"
+version = "3.4.0"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
@@ -85,14 +85,18 @@
 commitizen = "commitizen.providers:CommitizenProvider"
 composer = "commitizen.providers:ComposerProvider"
 npm = "commitizen.providers:NpmProvider"
 pep621 = "commitizen.providers:Pep621Provider"
 poetry = "commitizen.providers:PoetryProvider"
 scm = "commitizen.providers:ScmProvider"
 
+[tool.poetry.plugins."commitizen.scheme"]
+pep440 = "commitizen.version_schemes:Pep440"
+semver = "commitizen.version_schemes:SemVer"
+
 [tool.coverage]
     [tool.coverage.report]
     show_missing = true
     exclude_lines = [
         # Have to re-enable the standard pragma
         'pragma: no cover',
 
@@ -102,15 +106,16 @@
 
         # Don't complain if tests don't hit defensive assertion code:
         'raise AssertionError',
         'raise NotImplementedError',
 
         # Don't complain if non-runnable code isn't run:
         'if 0:',
-        'if __name__ == .__main__.:'
+        'if __name__ == .__main__.:',
+        'if TYPE_CHECKING:',
     ]
     omit = [
         'env/*',
         'venv/*',
         '.venv/*',
         '*/virtualenv/*',
         '*/virtualenvs/*',
@@ -142,7 +147,11 @@
 files = "commitizen"
 disallow_untyped_decorators = true
 disallow_subclassing_any = true
 warn_return_any = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_unused_configs = true
+
+[[tool.mypy.overrides]]
+module = "py.*"  # Legacy pytest dependencies
+ignore_missing_imports = true
```

### Comparing `commitizen-3.3.0/PKG-INFO` & `commitizen-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.3.0
+Version: 3.4.0
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
```

