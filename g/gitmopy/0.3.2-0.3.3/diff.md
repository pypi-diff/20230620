# Comparing `tmp/gitmopy-0.3.2.tar.gz` & `tmp/gitmopy-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitmopy-0.3.2.tar", max compression
+gzip compressed data, was "gitmopy-0.3.3.tar", max compression
```

## Comparing `gitmopy-0.3.2.tar` & `gitmopy-0.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-06-16 22:59:50.534602 gitmopy-0.3.2/LICENSE
--rw-r--r--   0        0        0     7683 2023-06-18 20:40:56.282671 gitmopy-0.3.2/README.md
--rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.3.2/gitmopy/__init__.py
--rw-r--r--   0        0        0    14362 2023-06-18 20:57:59.788436 gitmopy-0.3.2/gitmopy/cli.py
--rw-r--r--   0        0        0     5913 2023-06-18 20:32:40.124115 gitmopy-0.3.2/gitmopy/git.py
--rw-r--r--   0        0        0     2989 2023-06-16 22:57:56.570034 gitmopy-0.3.2/gitmopy/history.py
--rw-r--r--   0        0        0     8085 2023-06-18 20:57:59.722229 gitmopy-0.3.2/gitmopy/prompt.py
--rw-r--r--   0        0        0    20342 2023-06-18 20:17:35.746117 gitmopy-0.3.2/gitmopy/utils.py
--rw-r--r--   0        0        0      578 2023-06-18 20:56:57.856741 gitmopy-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     8664 1970-01-01 00:00:00.000000 gitmopy-0.3.2/setup.py
--rw-r--r--   0        0        0     8311 1970-01-01 00:00:00.000000 gitmopy-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-16 22:59:50.534602 gitmopy-0.3.3/LICENSE
+-rw-r--r--   0        0        0     7683 2023-06-19 21:42:16.941940 gitmopy-0.3.3/README.md
+-rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.3.3/gitmopy/__init__.py
+-rw-r--r--   0        0        0    14527 2023-06-19 23:07:26.703805 gitmopy-0.3.3/gitmopy/cli.py
+-rw-r--r--   0        0        0     5913 2023-06-19 21:42:16.943635 gitmopy-0.3.3/gitmopy/git.py
+-rw-r--r--   0        0        0     2989 2023-06-16 22:57:56.570034 gitmopy-0.3.3/gitmopy/history.py
+-rw-r--r--   0        0        0     8106 2023-06-19 23:04:51.808559 gitmopy-0.3.3/gitmopy/prompt.py
+-rw-r--r--   0        0        0    20657 2023-06-19 23:04:40.117543 gitmopy-0.3.3/gitmopy/utils.py
+-rw-r--r--   0        0        0      578 2023-06-19 23:06:00.492550 gitmopy-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8664 1970-01-01 00:00:00.000000 gitmopy-0.3.3/setup.py
+-rw-r--r--   0        0        0     8311 1970-01-01 00:00:00.000000 gitmopy-0.3.3/PKG-INFO
```

### Comparing `gitmopy-0.3.2/LICENSE` & `gitmopy-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.2/README.md` & `gitmopy-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.2/gitmopy/cli.py` & `gitmopy-0.3.3/gitmopy/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     CONFIG_PATH,
     HISTORY_PATH,
     _sentinels,
     load_config,
     message_from_commit_dict,
     print_staged_files,
     resolve_path,
+    terminal_separator,
 )
 
 app = typer.Typer()
 gitmojis_setup()
 
 
 def catch_keyboard_interrupt(func, *args, **kwargs):
@@ -96,16 +97,18 @@
     Args:
         repo (Repo): The git repository.
 
     Returns:
         bool: Whether the user wants to continue or not.
     """
     gitmojis_setup()
+    print()
+    print(terminal_separator())
     prompt_txt = (
-        "\n🔄 [u]Ready to commit again[/u]. Press [b green]enter[/b green] "
+        "🔄 [u]Ready to commit again[/u]. Press [b green]enter[/b green] "
         + "to commit again"
     )
 
     print()
     remotes_diff = format_remotes_diff(repo)
     if remotes_diff:
         print(remotes_diff)
@@ -118,19 +121,19 @@
 
     print(prompt_txt + " or [b red]q[/b red] to quit.", end="")
 
     commit_again = typer.prompt(
         "", default="enter", show_default=False, prompt_suffix=""
     )
     if remotes_diff:
-        if commit_again == "s":
-            pull_cli(repo, remote)
         if commit_again in {"p", "s"}:
+            if commit_again == "s":
+                pull_cli(repo, remote)
             push_cli(repo, remote)
-        return should_commit_again(repo, remote)
+            return should_commit_again(repo, remote)
 
     commit_again = commit_again != "q"
 
     if commit_again:
         print()
 
     return commit_again
@@ -329,15 +332,15 @@
                 to_add = catch_keyboard_interrupt(git_add_prompt, status)
                 if to_add is _sentinels["stop"]:
                     break
                 elif to_add is _sentinels["restart"]:
                     continue
                 elif not to_add:
                     print("[yellow]No file selected, nothing to commit.[/yellow]")
-                    if should_commit_again(repo, remote):
+                    if keep_alive and should_commit_again(repo, remote):
                         # user wants to commit again: start over
                         continue
                     # user wants to stop: break loop
                     break
             else:
                 # there are staged files: list them to user
                 if add:
@@ -379,16 +382,20 @@
             save_to_history(commit_dict)
 
         # commit
         repo.index.commit(commit_message)
 
         if push:
             push_cli(repo, remote)
-        if not keep_alive or not should_commit_again(repo, remote):
-            break
+
+        if keep_alive and should_commit_again(repo, remote):
+            # user wants to commit again
+            continue
+        # stop here
+        break
 
     print("\nDone 🥳\n")
 
 
 @app.command(
     help="Configure gitmopy",
 )
```

### Comparing `gitmopy-0.3.2/gitmopy/git.py` & `gitmopy-0.3.3/gitmopy/git.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.2/gitmopy/history.py` & `gitmopy-0.3.3/gitmopy/history.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.2/gitmopy/prompt.py` & `gitmopy-0.3.3/gitmopy/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from gitmopy.utils import (
     APP_PATH,
     DEFAULT_CHOICES,
     GITMOJIS,
     load_config,
     safe_capitalize,
     save_config,
-    separator,
+    choice_separator,
 )
 
 
 class GMPCompleter(Completer):
     def __init__(self, key: str, max_results: Optional[int] = 10):
         """
         A completer that completes a text prompt from the user's history.
@@ -218,20 +218,20 @@
         status (dict): Dictionary of files grouped by status.
 
     Returns:
         list: List of all the files selected by the user.
     """
     choices = []
     if len(status["unstaged"]) > 0:
-        choices.append(separator("Unstaged files"))
+        choices.append(choice_separator("Unstaged files"))
     for s in status["unstaged"]:
         choices.append(Choice(s, s, True))
 
     if len(status["untracked"]) > 0:
-        choices.append(separator("Untracked files"))
+        choices.append(choice_separator("Untracked files"))
     for s in status["untracked"]:
         choices.append(Choice(s, s, True))
 
     selected = inquirer.checkbox(
         message="Select files to add for the commit.",
         instruction="Use 'space' to (de-)select, 'enter' to validate.",
         choices=choices,
```

### Comparing `gitmopy-0.3.2/gitmopy/utils.py` & `gitmopy-0.3.3/gitmopy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Utility functions and constants for ``gitmopy``.
 """
 from os.path import expandvars
 from pathlib import Path
+from shutil import get_terminal_size
 from typing import Dict, List, Union
 
 import typer
 from InquirerPy.separator import Separator
 from rich import print
 from yaml import safe_dump, safe_load
 
@@ -145,23 +146,23 @@
     message = f"{commit_dict['emoji']} "
     if commit_dict["scope"]:
         message += f"({commit_dict['scope']}): "
     message += f"{commit_dict['title']}\n\n{commit_dict['message']}"
     return message.strip()
 
 
-def separator(title: str = "", width: int = 30, sep: str = "-") -> Separator:
+def choice_separator(title: str = "", width: int = 30, sep: str = "─") -> Separator:
     """
     Create an InquirerPy separator with a title.
 
     Args:
         title (str, optional): Title in-between separator characters.
             Defaults to ``""``.
         width (int, optional): Total length of sperator line. Defaults to 30.
-        sep (str, optional): Character to use around the ``title``. Defaults to ``"-"``.
+        sep (str, optional): Character to use around the ``title``. Defaults to ``"─"``.
 
     Returns:
         Separator: _description_
     """
     assert sep
     assert width > 0
     if len(title) > width - 4:
@@ -192,14 +193,26 @@
     if not s:
         return s
     if len(s) == 1:
         return s.upper()
     return s[0].upper() + s[1:]
 
 
+def terminal_separator(margin=10):
+    """
+    Create a separator for the terminal.
+
+    Returns:
+        str: Terminal separator
+    """
+    total = get_terminal_size().columns
+    sep = "─" * (total - 2 * margin)
+    return f"{' ' * margin}{sep}{' ' * margin}"
+
+
 # https://github.com/carloscuesta/gitmoji/blob/master/packages/gitmojis/src/gitmojis.json
 GITMOJIS = [
     {
         "emoji": "🎨",
         "entity": "&#x1f3a8;",
         "code": ":art:",
         "description": "Improve structure / format of the code.",
```

### Comparing `gitmopy-0.3.2/pyproject.toml` & `gitmopy-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitmopy"
-version = "0.3.2"
+version = "0.3.3"
 description = "A python command-line for gitmoji"
 authors = ["vict0rsch <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gitmopy-0.3.2/setup.py` & `gitmopy-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'typer[all]>=0.8.0']
 
 entry_points = \
 {'console_scripts': ['gitmopy = gitmopy.cli:app']}
 
 setup_kwargs = {
     'name': 'gitmopy',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'A python command-line for gitmoji',
     'long_description': '# `gitmopy`\n\nAn interactive Python implementation of the Gitmoji standard: https://gitmoji.dev/\n\n```text\npip install gitmopy\n```\n\n![demo-gitmopy](./assets/demo-gitmopy.gif)\n\n## How to use\n\n* I typically use `$ gitmopy commit --add --keep-alive`\n* Navigate through options with ⬆️ and ⬇️\n* Select option with **`space`**\n* Validate selection with **`enter`**\n* Press **`tab`** to auto-complete\n  * Press `tab` on an empty line to see history\n* Restart commit with **`crtl+c`**\n  * The keyboard interruption will be caught once, then press `enter` to restart\n\n## Suggested shortcuts\n\n```bash\nalias gpy="gitmopy"\nalias gpyc="gitmopy commit"\nalias gpya="gitmopy commit --add"\nalias gpyk="gitmopy commit --add --keep-alive"\n```\n\n![gpyk depo](assets/gpyk.png)\n\n## Examples\n\n```bash\n# Typical daily use-case\n# ----------------------\n\n# continuously commit, interactively select files to stage\n$ gitmopy commit --add --keep-alive\n\n# same using an alias, + push after every commit (could be dangerous)\n$ gpyk --push\n\n\n# Specific usage\n# --------------\n\n# commit currently staged files. Will fail if no file is staged.\n$ gitmopy commit\n\n# Enable interactive file selection if no file is currently staged. Ignored if\n# there are staged files.\n$ gitmopy commit --add\n\n# Commit continuously: don\'t leave the CLI after the first commit but restart\n# the commit procedure.\n$ gitmopy commit --keep-alive\n\n# Push to remote repositories after commit.\n# Interactively select remotes to push to if there are more than 1.\n$ gitmopy commit --push\n\n# Push to specific remotes\n$ gitmopy commit --push --remote origin --remote upstream\n\n# Make and display a commit message without staging/committing/pushing\n$ gitmopy commit --dry\n\n# configure gitmopy\n$ gitmopy config\n\n# print version, data paths and current configuration\n$ gitmopy info\n\n# print helps\n$ gitmopy --help\n$ gitmopy commit --help\n```\n\n⚠️ The sync feature is still experimental. It will `pull` then `push` but in the case of several remotes and the branch not existing on one of them, I recommend you deal with it with `git` manually.\n\n## User guide\n\n```text\n$ gitmopy info\n\ngitmopy info:\n  version : 0.1.0\n  app path: /Users/victor/.gitmopy\n  history : /Users/victor/.gitmopy/history.json\n  config  : /Users/victor/.gitmopy/config.yaml\n\nCurrent configuration:\n  skip_scope      : False\n  skip_message    : False\n  capitalize_title: True\n  enable_history  : True\n```\n\nUpdate configuration with\n\n```text\n$ gitmopy config\n$ gitmopy config\n❓ Configure gitmopy locally. Use \'space\' to (de-)select, \'enter\' to validate.\n❯ ○ Skip commit scope\n  ○ Skip commit message\n  ◉ Capitalize commit title\n  ◉ Remember commit history for auto-complete and emoji sorting\n\nConfig will be saved in /Users/victor/.gitmopy/config.yaml.\n```\n\nGet help with\n\n```text\n$ gitmopy --help\n\n Usage: gitmopy [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.             │\n│ --show-completion             Show completion for the current shell, to copy it or  │\n│                               customize the installation.                           │\n│ --help                        Show this message and exit.                           │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ──────────────────────────────────────────────────────────────────────────╮\n│ commit  Commit staged files. Use --add to interactively select files to stage if    │\n│         none is already staged                                                      │\n│ config  Configure gitmopy                                                           │\n│ info    Print gitmopy info                                                          │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n\n$ gitmopy commit --help\n\n Usage: gitmopy commit [OPTIONS]\n\n Commit staged files. Use --add to interactively select files to stage if none is\n already staged\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --repo                             TEXT  Path to the git repository [default: .]    │\n│ --add           --no-add                 Whether or not to interactively select     │\n│                                          files to stage if none is already staged   │\n│                                          [default: no-add]                          │\n│ --push          --no-push                Whether to `git push` after commit. If     │\n│                                          multiple remotes exist, you will be asked  │\n│                                          to interactively choose the ones to push   │\n│                                          to. Use --remote to skip interactive       │\n│                                          selection. Disabled by default.            │\n│                                          [default: no-push]                         │\n│ --dry           --no-dry                 Whether or not to actually commit.         │\n│                                          [default: no-dry]                          │\n│ --remote                           TEXT  Remote to push to after commit. Use to     │\n│                                          skip interactive remote selection when     │\n│                                          several exist. Use several \'--remote       │\n│                                          {remote name}\' to push to multiple remotes │\n│ --keep-alive    --no-keep-alive          Whether or not to keep the app alive after │\n│                                          commit, to be ready for another one.       │\n│                                          [default: no-keep-alive]                   │\n│ --help                                   Show this message and exit.                │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n## To Do\n\n* Features\n  * *If requested:*\n    * Install hook\n    * `git commit` flags (like `-S`)\n    * max history length (if loading the json becomes slow)\n* Tests\n  * https://typer.tiangolo.com/tutorial/testing/\n  * 👋 **Help wanted**\n* Docs\n  * Not critical\n\n## Resources\n\n`gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).\n\nIt is built thanks to:\n\n* [`typer`](https://github.com/tiangolo/typer)\n* [`InquirePy`](https://github.com/kazhala/InquirerPy)\n* [`GitPython`](https://github.com/gitpython-developers/GitPython)\n',
     'author': 'vict0rsch',
     'author_email': 'vsch@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `gitmopy-0.3.2/PKG-INFO` & `gitmopy-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitmopy
-Version: 0.3.2
+Version: 0.3.3
 Summary: A python command-line for gitmoji
 License: MIT
 Author: vict0rsch
 Author-email: vsch@pm.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

