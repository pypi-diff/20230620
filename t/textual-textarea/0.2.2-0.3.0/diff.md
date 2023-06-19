# Comparing `tmp/textual_textarea-0.2.2.tar.gz` & `tmp/textual_textarea-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_textarea-0.2.2.tar", max compression
+gzip compressed data, was "textual_textarea-0.3.0.tar", max compression
```

## Comparing `textual_textarea-0.2.2.tar` & `textual_textarea-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1068 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/LICENSE
--rw-r--r--   0        0        0     4020 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/README.md
--rw-r--r--   0        0        0     1555 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       71 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/__init__.py
--rw-r--r--   0        0        0      491 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/__main__.py
--rw-r--r--   0        0        0      175 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/cancellable_input.py
--rw-r--r--   0        0        0     1028 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/colors.py
--rw-r--r--   0        0        0     1091 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/containers.py
--rw-r--r--   0        0        0     2021 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/error_modal.py
--rw-r--r--   0        0        0     3212 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/key_handlers.py
--rw-r--r--   0        0        0      681 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/messages.py
--rw-r--r--   0        0        0        0 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/py.typed
--rw-r--r--   0        0        0      450 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/serde.py
--rw-r--r--   0        0        0    26349 2023-06-15 18:38:15.941105 textual_textarea-0.2.2/src/textual_textarea/textarea.py
--rw-r--r--   0        0        0     4950 1970-01-01 00:00:00.000000 textual_textarea-0.2.2/setup.py
--rw-r--r--   0        0        0     4818 1970-01-01 00:00:00.000000 textual_textarea-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4475 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/README.md
+-rw-r--r--   0        0        0     1555 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/__main__.py
+-rw-r--r--   0        0        0      175 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/cancellable_input.py
+-rw-r--r--   0        0        0     1028 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/colors.py
+-rw-r--r--   0        0        0     3510 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/comments.py
+-rw-r--r--   0        0        0     1091 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/containers.py
+-rw-r--r--   0        0        0     2021 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/error_modal.py
+-rw-r--r--   0        0        0     3374 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/key_handlers.py
+-rw-r--r--   0        0        0      681 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/messages.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/py.typed
+-rw-r--r--   0        0        0      450 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/serde.py
+-rw-r--r--   0        0        0    28491 2023-06-19 22:39:20.785678 textual_textarea-0.3.0/src/textual_textarea/textarea.py
+-rw-r--r--   0        0        0     5418 1970-01-01 00:00:00.000000 textual_textarea-0.3.0/setup.py
+-rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 textual_textarea-0.3.0/PKG-INFO
```

### Comparing `textual_textarea-0.2.2/LICENSE` & `textual_textarea-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.2.2/README.md` & `textual_textarea-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 pip install textual-textarea
 ```
 
 ## Features
 Full-featured text editor experience with VS-Code-like bindings, in your Textual App:
 - Syntax highlighting and support for themes.
 - Move cursor and scroll with mouse or keys (including <kbd>ctrl+arrow</kbd>, <kbd>PgUp/Dn</kbd>,  <kbd>Home/End</kbd>).
-- Select text using <kbd>shift</kbd>.
+- Select text using <kbd>shift</kbd> or click and drag.
 - Open (<kbd>ctrl+o</kbd>) and save (<kbd>ctrl+s</kbd>) files.
 - Cut (<kbd>ctrl+x</kbd>), copy (<kbd>ctrl+c</kbd>), paste (<kbd>ctrl+u/v</kbd>), optionally using the system clipboard.
 - Comment selections with <kbd>ctrl+/</kbd>.
 - Indent and dedent (optionally for a multiline selection) to tab stops with <kbd>Tab</kbd> and <kbd>shift+Tab</kbd>.
 - Automatic completions of quotes and brackets.
 - Quit with <kbd>ctrl+q</kbd>.
 
@@ -72,14 +72,26 @@
 ta = self.query_one(TextArea)
 old_cursor = ta.cursor
 ta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible
 cursor_line_number = ta.cursor.lno
 cursor_x_position = ta.cursor.pos
 ```
 
+#### Getting and Setting The Language
+
+Syntax highlighting and comment insertion depends on the configured language for the TextArea.
+
+The TextArea exposes a `language` property that returns `None` or a string that is equal to the short name of the [Pygments lexer](https://pygments.org/docs/lexers/) for the currently configured language:
+
+```python
+ta = self.query_one(TextArea)
+old_language = ta.language
+ta.language = "python"
+```
+
 #### Getting Theme Colors
 
 If you would like the rest of your app to match the colors from the TextArea's theme, they are exposed via the `theme_colors` property.
 
 ```python
 ta = self.query_one(TextArea)
 color = ta.theme_colors.contrast_text_color
@@ -105,8 +117,8 @@
     class Submitted(Message, bubble=True):
         def __init__(self, text: str) -> None:
             super().__init__()
             self.text = text
 
     async def action_submit(self) -> None:
         self.post_message(self.Submitted(self.text))
-```
+```
```

### Comparing `textual_textarea-0.2.2/pyproject.toml` & `textual_textarea-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textual-textarea"
-version = "0.2.2"
+version = "0.3.0"
 description = "A text area (multi-line input) with syntax highlighting for Textual"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 homepage = "https://github.com/tconbeer/textual-textarea"
 repository = "https://github.com/tconbeer/textual-textarea"
 readme = "README.md"
 packages = [{ include = "textual_textarea", from = "src" }]
```

### Comparing `textual_textarea-0.2.2/src/textual_textarea/colors.py` & `textual_textarea-0.3.0/src/textual_textarea/colors.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.2.2/src/textual_textarea/containers.py` & `textual_textarea-0.3.0/src/textual_textarea/containers.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.2.2/src/textual_textarea/error_modal.py` & `textual_textarea-0.3.0/src/textual_textarea/error_modal.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.2.2/src/textual_textarea/key_handlers.py` & `textual_textarea-0.3.0/src/textual_textarea/key_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import re
 from typing import List, NamedTuple
 
 from textual import log
+from textual.events import MouseEvent
 
 WWB = re.compile(r"\W*\w+\b")
 
 
 class Cursor(NamedTuple):
     lno: int
     pos: int
 
+    @classmethod
+    def from_mouse_event(cls, event: MouseEvent) -> "Cursor":
+        return Cursor(event.y, event.x - 1)
+
 
 def handle_arrow(key: str, lines: List[str], cursor: Cursor) -> Cursor:
     arrow = key.split("+")[-1]
     if "ctrl" in key:
         assert arrow not in ("up", "down"), "ctrl+up/down should be handled first"
         if arrow == "right":
             return _handle_ctrl_right(lines, cursor)
```

### Comparing `textual_textarea-0.2.2/src/textual_textarea/messages.py` & `textual_textarea-0.3.0/src/textual_textarea/messages.py`

 * *Files identical despite different names*

### Comparing `textual_textarea-0.2.2/src/textual_textarea/textarea.py` & `textual_textarea-0.3.0/src/textual_textarea/textarea.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from textual.binding import Binding
 from textual.reactive import reactive
 from textual.widget import Widget
 from textual.widgets import Input, Static
 
 from textual_textarea.cancellable_input import CancellableInput
 from textual_textarea.colors import WidgetColors
+from textual_textarea.comments import INLINE_MARKERS
 from textual_textarea.containers import FooterContainer, TextContainer
 from textual_textarea.error_modal import ErrorModal
 from textual_textarea.key_handlers import Cursor, handle_arrow
 from textual_textarea.messages import TextAreaCursorMoved, TextAreaScrollOne
 from textual_textarea.serde import deserialize_lines, serialize_lines
 
 BRACKETS = {
@@ -40,14 +41,15 @@
 
     lines: reactive[List[str]] = reactive(lambda: list(" "))
     cursor: reactive[Cursor] = reactive(Cursor(0, 0))
     selection_anchor: reactive[Union[Cursor, None]] = reactive(None)
     clipboard: List[str] = list()
     cursor_visible: reactive[bool] = reactive(True)
     use_system_clipboard: bool = True
+    language: reactive[Union[str, None]] = reactive(None)
 
     def __init__(
         self,
         theme_colors: WidgetColors,
         language: Union[str, None] = None,
         theme: str = "monokai",
         use_system_clipboard: bool = True,
@@ -164,28 +166,37 @@
             event.stop()
             self.cursor = Cursor(0, 0)
         elif event.key in ("ctrl+end", "ctrl+a"):
             event.stop()
             self.cursor = Cursor(lno=len(self.lines) - 1, pos=len(self.lines[-1]) - 1)
         elif event.key == "ctrl+underscore":  # actually ctrl+/
             event.stop()
-            lines, first, last = self._get_selected_lines(selection_before)
-            stripped_lines = [line.lstrip() for line in lines]
-            indents = [len(line) - len(line.lstrip()) for line in lines]
-            if all([line.startswith("-- ") for line in stripped_lines]):
-                no_comment_lines = [line[3:] for line in stripped_lines]
-                self.lines[first.lno : last.lno + 1] = [
-                    f"{' ' * indent}{stripped_line}"
-                    for indent, stripped_line in zip(indents, no_comment_lines)
-                ]
-            else:
-                self.lines[first.lno : last.lno + 1] = [
-                    f"{' ' * indent}-- {stripped_line}"
-                    for indent, stripped_line in zip(indents, stripped_lines)
-                ]
+            if self.inline_comment_marker:
+                lines, first, last = self._get_selected_lines(selection_before)
+                stripped_lines = [line.lstrip() for line in lines]
+                indents = [len(line) - len(line.lstrip()) for line in lines]
+                if all(
+                    [
+                        line.startswith(self.inline_comment_marker)
+                        for line in stripped_lines
+                    ]
+                ):
+                    no_comment_lines = [
+                        line[len(self.inline_comment_marker) :].lstrip()
+                        for line in stripped_lines
+                    ]
+                    self.lines[first.lno : last.lno + 1] = [
+                        f"{' ' * indent}{line}"
+                        for indent, line in zip(indents, no_comment_lines)
+                    ]
+                else:
+                    self.lines[first.lno : last.lno + 1] = [
+                        f"{' ' * indent}{self.inline_comment_marker} {stripped_line}"
+                        for indent, stripped_line in zip(indents, stripped_lines)
+                    ]
         elif event.key in ("ctrl+c", "ctrl+x"):
             event.stop()
             if selection_before:
                 lines, first, last = self._get_selected_lines(selection_before)
             else:  # no selection, copy whole line
                 lines, first, last = (
                     [self.lines[self.cursor.lno], ""],
@@ -287,14 +298,17 @@
             )
 
         self.update(self._content)
 
     def watch_cursor(self) -> None:
         self._scroll_to_cursor()
 
+    def watch_language(self, language: str) -> None:
+        self.inline_comment_marker = INLINE_MARKERS.get(language)
+
     @property
     def _content(self) -> RenderableType:
         syntax = Syntax(
             "\n".join(self.lines),
             lexer=self.language,
             theme=self.theme,
         )
@@ -511,15 +525,15 @@
                 (https://pygments.org/docs/lexers/), e.g., "python", "sql", "as3".
             theme (str): Must be name of a Pygments style (https://pygments.org/styles/),
                 e.g., "bw", "github-dark", "solarized-light".
         """
         super().__init__(
             *children, name=name, id=id, classes=classes, disabled=disabled
         )
-        self.language = language
+        self._language = language
         self.theme = theme
         self.theme_colors = WidgetColors.from_theme(self.theme)
         self.use_system_clipboard = use_system_clipboard
 
     @property
     def text(self) -> str:
         """
@@ -551,18 +565,36 @@
         """
         Args:
             cursor (Union[Cursor, Tuple[int, int]]): The position (line number, pos)
             to move the cursor to
         """
         self.text_input.move_cursor(cursor[1], cursor[0])
 
+    @property
+    def language(self) -> Union[str, None]:
+        """
+        Returns
+            str | None: The Pygments short name of the active language
+        """
+        return self.text_input.language
+
+    @language.setter
+    def language(self, language: str) -> None:
+        """
+        Args:
+            langage (str | None): The Pygments short name for the new language
+        """
+        self.text_input.language = language
+
     def compose(self) -> ComposeResult:
         with TextContainer():
             yield TextInput(
-                language=self.language, theme=self.theme, theme_colors=self.theme_colors
+                language=self._language,
+                theme=self.theme,
+                theme_colors=self.theme_colors,
             )
         yield FooterContainer(theme_colors=self.theme_colors)
 
     def on_mount(self) -> None:
         self.styles.background = self.theme_colors.bgcolor
         self.text_container = self.query_one(TextContainer)
         self.text_input = self.query_one(TextInput)
@@ -584,23 +616,54 @@
         )
         input.styles.background = self.theme_colors.bgcolor
         input.styles.border = "round", self.theme_colors.contrast_text_color
         input.styles.color = self.theme_colors.contrast_text_color
         self.footer.mount(input)
         input.focus()
 
-    def on_click(self, event: events.Click) -> None:
+    def on_mouse_down(self, event: events.MouseDown) -> None:
         """
-        Moves the cursor to the click.
+        Moves the anchor and cursor to the click.
         """
+        event.stop()
+        self.capture_mouse()
         self.text_input.cursor_visible = True
         self.text_input.blink_timer.reset()
+        self.text_input.selection_anchor = Cursor.from_mouse_event(event)
         self.text_input.move_cursor(event.x - 1, event.y)
         self.text_input.focus()
 
+    def on_mouse_move(self, event: events.MouseMove) -> None:
+        """
+        Updates the cursor if the button is pressed
+        """
+        if event.button == 1:
+            self.text_input.move_cursor(event.x - 1, event.y)
+
+    def on_mouse_up(self, event: events.MouseUp) -> None:
+        """
+        Moves the cursor to the click.
+        """
+        event.stop()
+        self.release_mouse()
+        self.text_input.cursor_visible = True
+        self.text_input.blink_timer.reset()
+        if self.text_input.selection_anchor == Cursor.from_mouse_event(event):
+            # simple click
+            self.text_input.selection_anchor = None
+        else:
+            self.text_input.move_cursor(event.x - 1, event.y)
+        self.text_input.focus()
+
+    def on_click(self, event: events.Click) -> None:
+        """
+        Click duplicates MouseUp and MouseDown, so we just capture and kill this event.
+        """
+        event.stop()
+
     def on_text_area_cursor_moved(self, event: TextAreaCursorMoved) -> None:
         """
         Scrolls the container so the cursor is visible.
         """
         event.stop()
         container = self.text_container
         x_buffer = container.window_region.width // 4
```

### Comparing `textual_textarea-0.2.2/setup.py` & `textual_textarea-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['pyperclip>=1.8.2,<2.0.0', 'textual>=0.21.0,<1.0.0']
 
 setup_kwargs = {
     'name': 'textual-textarea',
-    'version': '0.2.2',
+    'version': '0.3.0',
     'description': 'A text area (multi-line input) with syntax highlighting for Textual',
-    'long_description': '# Textual Textarea\n![Textual Textarea Screenshot](textarea.png)\n\n## Installation\n\n```\npip install textual-textarea\n```\n\n## Features\nFull-featured text editor experience with VS-Code-like bindings, in your Textual App:\n- Syntax highlighting and support for themes.\n- Move cursor and scroll with mouse or keys (including <kbd>ctrl+arrow</kbd>, <kbd>PgUp/Dn</kbd>,  <kbd>Home/End</kbd>).\n- Select text using <kbd>shift</kbd>.\n- Open (<kbd>ctrl+o</kbd>) and save (<kbd>ctrl+s</kbd>) files.\n- Cut (<kbd>ctrl+x</kbd>), copy (<kbd>ctrl+c</kbd>), paste (<kbd>ctrl+u/v</kbd>), optionally using the system clipboard.\n- Comment selections with <kbd>ctrl+/</kbd>.\n- Indent and dedent (optionally for a multiline selection) to tab stops with <kbd>Tab</kbd> and <kbd>shift+Tab</kbd>.\n- Automatic completions of quotes and brackets.\n- Quit with <kbd>ctrl+q</kbd>.\n\n## Usage\n\n### Initializing the Widget\n\nThe TextArea is a Textual Widget. You can add it to a Textual\napp using `compose` or `mount`:\n\n```python\nfrom textual_textarea import TextArea\nfrom textual.app import App, ComposeResult\n\nclass TextApp(App, inherit_bindings=False):\n    def compose(self) -> ComposeResult:\n        yield TextArea(language="python", theme="solarized-dark")\n\n    def on_mount(self) -> None:\n        ta = self.query_one(TextArea)\n        ta.focus()\n\napp = TextApp()\napp.run()\n```\n\nIn addition to the standard Widget arguments, TextArea accepts three additional, optional arguments when initializing the widget:\n\n- language (str): Must be `None` or the short name of a [Pygments lexer](https://pygments.org/docs/lexers/), e.g., `python`, `sql`, `as3`. Defaults to `None`.\n- theme (str): Must be name of a [Pygments style](https://pygments.org/styles/), e.g., `bw`, `github-dark`, `solarized-light`. Defaults to `monokai`.\n- use_system_clipboard (bool): Set to `False` to make the TextArea\'s copy and paste operations ignore the system clipboard. Defaults to `True`.\n\nThe TextArea supports many actions and key bindings. **For proper binding of `ctrl+c` to the COPY action,\nyou must initialize your App with `inherit_bindings=False`** (as shown above), so that `ctrl+c` does not quit the app. The TextArea implements `ctrl+q` as quit; you way wish to mimic that in your app so that other in-focus widgets use the same behavior.\n\n### Interacting with the Widget\n\n#### Getting and Setting Text\n\nThe TextArea exposes a `text` property that contains the full text contained in the widget. You can retrieve or set the text by interacting with this property:\n\n```python\nta = self.query_one(TextArea)\nold_text = ta.text\nta.text = "New Text!\\n\\nMany Lines!"\n```\n\n\n#### Getting and Setting The Cursor Position\n\nThe TextArea exposes a `cursor` property that returns a NamedTuple with the position of the cursor. The tuple is (line_number, x_pos):\n\n```python\nta = self.query_one(TextArea)\nold_cursor = ta.cursor\nta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible\ncursor_line_number = ta.cursor.lno\ncursor_x_position = ta.cursor.pos\n```\n\n#### Getting Theme Colors\n\nIf you would like the rest of your app to match the colors from the TextArea\'s theme, they are exposed via the `theme_colors` property.\n\n```python\nta = self.query_one(TextArea)\ncolor = ta.theme_colors.contrast_text_color\nbgcolor = ta.theme_colors.bgcolor\nhighlight = ta.theme_colors.selection_bgcolor\n```\n\n\n#### Adding Bindings and other Behavior\n\nYou can subclass TextArea to add your own behavior. This snippet adds an action that posts a Submitted message containing the text of the TextArea when the user presses <kbd>ctrl+j</kbd>:\n\n```python\nfrom textual.message import Message\nfrom textual_textarea import TextArea\n\n\nclass CodeEditor(TextArea):\n    BINDINGS = [\n        ("ctrl+j", "submit", "Run Query"),\n    ]\n\n    class Submitted(Message, bubble=True):\n        def __init__(self, text: str) -> None:\n            super().__init__()\n            self.text = text\n\n    async def action_submit(self) -> None:\n        self.post_message(self.Submitted(self.text))\n```',
+    'long_description': '# Textual Textarea\n![Textual Textarea Screenshot](textarea.png)\n\n## Installation\n\n```\npip install textual-textarea\n```\n\n## Features\nFull-featured text editor experience with VS-Code-like bindings, in your Textual App:\n- Syntax highlighting and support for themes.\n- Move cursor and scroll with mouse or keys (including <kbd>ctrl+arrow</kbd>, <kbd>PgUp/Dn</kbd>,  <kbd>Home/End</kbd>).\n- Select text using <kbd>shift</kbd> or click and drag.\n- Open (<kbd>ctrl+o</kbd>) and save (<kbd>ctrl+s</kbd>) files.\n- Cut (<kbd>ctrl+x</kbd>), copy (<kbd>ctrl+c</kbd>), paste (<kbd>ctrl+u/v</kbd>), optionally using the system clipboard.\n- Comment selections with <kbd>ctrl+/</kbd>.\n- Indent and dedent (optionally for a multiline selection) to tab stops with <kbd>Tab</kbd> and <kbd>shift+Tab</kbd>.\n- Automatic completions of quotes and brackets.\n- Quit with <kbd>ctrl+q</kbd>.\n\n## Usage\n\n### Initializing the Widget\n\nThe TextArea is a Textual Widget. You can add it to a Textual\napp using `compose` or `mount`:\n\n```python\nfrom textual_textarea import TextArea\nfrom textual.app import App, ComposeResult\n\nclass TextApp(App, inherit_bindings=False):\n    def compose(self) -> ComposeResult:\n        yield TextArea(language="python", theme="solarized-dark")\n\n    def on_mount(self) -> None:\n        ta = self.query_one(TextArea)\n        ta.focus()\n\napp = TextApp()\napp.run()\n```\n\nIn addition to the standard Widget arguments, TextArea accepts three additional, optional arguments when initializing the widget:\n\n- language (str): Must be `None` or the short name of a [Pygments lexer](https://pygments.org/docs/lexers/), e.g., `python`, `sql`, `as3`. Defaults to `None`.\n- theme (str): Must be name of a [Pygments style](https://pygments.org/styles/), e.g., `bw`, `github-dark`, `solarized-light`. Defaults to `monokai`.\n- use_system_clipboard (bool): Set to `False` to make the TextArea\'s copy and paste operations ignore the system clipboard. Defaults to `True`.\n\nThe TextArea supports many actions and key bindings. **For proper binding of `ctrl+c` to the COPY action,\nyou must initialize your App with `inherit_bindings=False`** (as shown above), so that `ctrl+c` does not quit the app. The TextArea implements `ctrl+q` as quit; you way wish to mimic that in your app so that other in-focus widgets use the same behavior.\n\n### Interacting with the Widget\n\n#### Getting and Setting Text\n\nThe TextArea exposes a `text` property that contains the full text contained in the widget. You can retrieve or set the text by interacting with this property:\n\n```python\nta = self.query_one(TextArea)\nold_text = ta.text\nta.text = "New Text!\\n\\nMany Lines!"\n```\n\n\n#### Getting and Setting The Cursor Position\n\nThe TextArea exposes a `cursor` property that returns a NamedTuple with the position of the cursor. The tuple is (line_number, x_pos):\n\n```python\nta = self.query_one(TextArea)\nold_cursor = ta.cursor\nta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible\ncursor_line_number = ta.cursor.lno\ncursor_x_position = ta.cursor.pos\n```\n\n#### Getting and Setting The Language\n\nSyntax highlighting and comment insertion depends on the configured language for the TextArea.\n\nThe TextArea exposes a `language` property that returns `None` or a string that is equal to the short name of the [Pygments lexer](https://pygments.org/docs/lexers/) for the currently configured language:\n\n```python\nta = self.query_one(TextArea)\nold_language = ta.language\nta.language = "python"\n```\n\n#### Getting Theme Colors\n\nIf you would like the rest of your app to match the colors from the TextArea\'s theme, they are exposed via the `theme_colors` property.\n\n```python\nta = self.query_one(TextArea)\ncolor = ta.theme_colors.contrast_text_color\nbgcolor = ta.theme_colors.bgcolor\nhighlight = ta.theme_colors.selection_bgcolor\n```\n\n\n#### Adding Bindings and other Behavior\n\nYou can subclass TextArea to add your own behavior. This snippet adds an action that posts a Submitted message containing the text of the TextArea when the user presses <kbd>ctrl+j</kbd>:\n\n```python\nfrom textual.message import Message\nfrom textual_textarea import TextArea\n\n\nclass CodeEditor(TextArea):\n    BINDINGS = [\n        ("ctrl+j", "submit", "Run Query"),\n    ]\n\n    class Submitted(Message, bubble=True):\n        def __init__(self, text: str) -> None:\n            super().__init__()\n            self.text = text\n\n    async def action_submit(self) -> None:\n        self.post_message(self.Submitted(self.text))\n```\n',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tconbeer/textual-textarea',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `textual_textarea-0.2.2/PKG-INFO` & `textual_textarea-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-textarea
-Version: 0.2.2
+Version: 0.3.0
 Summary: A text area (multi-line input) with syntax highlighting for Textual
 Home-page: https://github.com/tconbeer/textual-textarea
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 pip install textual-textarea
 ```
 
 ## Features
 Full-featured text editor experience with VS-Code-like bindings, in your Textual App:
 - Syntax highlighting and support for themes.
 - Move cursor and scroll with mouse or keys (including <kbd>ctrl+arrow</kbd>, <kbd>PgUp/Dn</kbd>,  <kbd>Home/End</kbd>).
-- Select text using <kbd>shift</kbd>.
+- Select text using <kbd>shift</kbd> or click and drag.
 - Open (<kbd>ctrl+o</kbd>) and save (<kbd>ctrl+s</kbd>) files.
 - Cut (<kbd>ctrl+x</kbd>), copy (<kbd>ctrl+c</kbd>), paste (<kbd>ctrl+u/v</kbd>), optionally using the system clipboard.
 - Comment selections with <kbd>ctrl+/</kbd>.
 - Indent and dedent (optionally for a multiline selection) to tab stops with <kbd>Tab</kbd> and <kbd>shift+Tab</kbd>.
 - Automatic completions of quotes and brackets.
 - Quit with <kbd>ctrl+q</kbd>.
 
@@ -92,14 +92,26 @@
 ta = self.query_one(TextArea)
 old_cursor = ta.cursor
 ta.cursor = (999, 0)  # the cursor will move as close to line 999, pos 0 as possible
 cursor_line_number = ta.cursor.lno
 cursor_x_position = ta.cursor.pos
 ```
 
+#### Getting and Setting The Language
+
+Syntax highlighting and comment insertion depends on the configured language for the TextArea.
+
+The TextArea exposes a `language` property that returns `None` or a string that is equal to the short name of the [Pygments lexer](https://pygments.org/docs/lexers/) for the currently configured language:
+
+```python
+ta = self.query_one(TextArea)
+old_language = ta.language
+ta.language = "python"
+```
+
 #### Getting Theme Colors
 
 If you would like the rest of your app to match the colors from the TextArea's theme, they are exposed via the `theme_colors` property.
 
 ```python
 ta = self.query_one(TextArea)
 color = ta.theme_colors.contrast_text_color
@@ -126,7 +138,8 @@
         def __init__(self, text: str) -> None:
             super().__init__()
             self.text = text
 
     async def action_submit(self) -> None:
         self.post_message(self.Submitted(self.text))
 ```
+
```

