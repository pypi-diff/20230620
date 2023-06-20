# Comparing `tmp/rgx-1.3.3.tar.gz` & `tmp/rgx-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgx-1.3.3.tar", max compression
+gzip compressed data, was "rgx-1.3.4.tar", max compression
```

## Comparing `rgx-1.3.3.tar` & `rgx-1.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-04-04 01:15:41.282839 rgx-1.3.3/LICENSE
--rw-r--r--   0        0        0    16342 2023-04-04 01:15:41.282839 rgx-1.3.3/README.md
--rw-r--r--   0        0        0      493 2023-04-04 01:15:41.282839 rgx-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      129 2023-04-04 01:15:41.282839 rgx-1.3.3/rgx/__init__.py
--rw-r--r--   0        0        0    27430 2023-04-04 01:15:41.282839 rgx-1.3.3/rgx/entities.py
--rw-r--r--   0        0        0      933 2023-04-04 01:15:41.282839 rgx-1.3.3/rgx/meta.py
--rw-r--r--   0        0        0      663 2023-04-04 01:15:41.282839 rgx-1.3.3/rgx/unicode_meta.py
--rw-r--r--   0        0        0    17063 1970-01-01 00:00:00.000000 rgx-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-20 14:04:14.103178 rgx-1.3.4/LICENSE
+-rw-r--r--   0        0        0    16342 2023-06-20 14:04:14.103178 rgx-1.3.4/README.md
+-rw-r--r--   0        0        0      493 2023-06-20 14:04:14.103178 rgx-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-06-20 14:04:14.103178 rgx-1.3.4/rgx/__init__.py
+-rw-r--r--   0        0        0    29580 2023-06-20 14:04:14.103178 rgx-1.3.4/rgx/entities.py
+-rw-r--r--   0        0        0      933 2023-06-20 14:04:14.103178 rgx-1.3.4/rgx/meta.py
+-rw-r--r--   0        0        0      663 2023-06-20 14:04:14.103178 rgx-1.3.4/rgx/unicode_meta.py
+-rw-r--r--   0        0        0    17063 1970-01-01 00:00:00.000000 rgx-1.3.4/PKG-INFO
```

### Comparing `rgx-1.3.3/LICENSE` & `rgx-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rgx-1.3.3/README.md` & `rgx-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `rgx-1.3.3/rgx/entities.py` & `rgx-1.3.4/rgx/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,27 +59,31 @@
     A universal pattern constructor.
 
     - With a string, returns a literan pattern. with `escape=False` returns an unescaped pattern.
     - With a tuple, returns a non-capturing group of patterns (or just one pattern if tuple has one element)
     - With a list, returns a character group (`[...]`). List must consist of strings and CharRange
 
     """
+    if isinstance(literal, RegexPattern):
+        return literal
+
     if isinstance(literal, str):
         if not escape:
             return UnescapedLiteral(literal)
         if len(literal) == 1:
             return Chars([literal])
         return Literal(literal)
+
     if isinstance(literal, tuple):
         if len(literal) == 1:
             return pattern(literal[0])
         return NonCapturingGroup(Concat(*literal))
+
     if isinstance(literal, list):
         return Chars(literal)
-    return literal
 
 
 def respect_priority(contents_: AnyRegexPattern, other_priority: int) -> RegexPattern:
     contents: RegexPattern = pattern(contents_)
     if contents.priority < other_priority:
         return NonCapturingGroup(contents)
     return contents
@@ -92,14 +96,17 @@
         """
         Internal method
 
         Returns a generator, that can be joined to get a pattern string representation
         """
         return NotImplemented
 
+    def case_insensitive(self) -> RegexPattern:
+        return self.set_flags("i")
+
     def render_str(self, flags: str = "") -> str:
         """
 
         Renders given pattern into a string with specified global flags.
 
         """
         contents: Iterable[str]
@@ -384,14 +391,17 @@
 
     def __init__(self, *contents: AnyRegexPattern):
         self.contents = pattern(contents)
 
     def render_prefix(self) -> StrGen:
         yield self.prefix
 
+    def case_insensitive(self):
+        return self.__class__(self.contents.case_insensitive())
+
     def render(self) -> StrGen:
         yield "("
         yield from self.render_prefix()
         yield from self.contents.render()
         yield ")"
 
 
@@ -522,14 +532,36 @@
                 "Can't exclude non-Chars pattern, don't really know how..."
             )
         result = []
         for part in self.contents:
             result.extend(part.exclude(chars))
         return Chars(result)
 
+    def case_insensitive(self) -> Chars:
+        contents: list[CharRange] = []
+
+        for part in self.contents:
+            start_char = chr(part.start)
+            stop_char = chr(part.stop)
+
+            is_lower = start_char.islower() and stop_char.islower()
+            is_upper = start_char.isupper() and stop_char.isupper()
+
+            if is_lower:
+                upper_chars = map(ord, map(str.upper, (start_char, stop_char)))
+                contents.append(CharRange(*upper_chars))
+
+            elif is_upper:
+                lower_chars = map(ord, map(str.lower, (start_char, stop_char)))
+                contents.append(CharRange(*lower_chars))
+
+            contents.append(part)
+
+        return Chars(contents)
+
 
 class ReversedChars(RegexPattern):
     def __init__(self, contents: Sequence[CharType]):
         self.contents = list(merge_chars(contents))
 
     def render(self) -> StrGen:
         yield "["
@@ -539,14 +571,17 @@
                 yield from char.render()
             elif char in Chars.non_special:
                 yield char
             else:
                 yield re.escape(char)
         yield "]"
 
+    def case_insensitive(self):
+        return self.reverse().case_insensitive().reverse()
+
     def reverse(self) -> Chars:
         return Chars(self.contents)
 
     @overload
     def __or__(self, other: ReversedChars) -> ReversedChars:
         ...
 
@@ -715,27 +750,37 @@
 
     def __init__(self, *contents: AnyRegexPattern) -> None:
         self.contents = [respect_priority(part, self.priority) for part in contents]
 
     def __add__(self, other: AnyRegexPattern) -> Concat:
         return Concat(*self.contents, other)
 
+    def case_insensitive(self):
+        new = Concat()
+        new.contents = [part.case_insensitive() for part in self.contents]
+        return new
+
     def render(self) -> StrGen:
         for part in self.contents:
             yield from part.render()
 
 
 class Option(RegexPattern):
     priority = 0 * priority_step
 
     def __init__(self, *alternatives: AnyRegexPattern):
         self.alternatives = [
             respect_priority(alternative, self.priority) for alternative in alternatives
         ]
 
+    def case_insensitive(self) -> RegexPattern:
+        new = Option()
+        new.alternatives = [part.case_insensitive() for part in self.alternatives]
+        return new
+
     def render(self) -> StrGen:
         if not self.alternatives:
             return
         yield from self.alternatives[0].render()
         for alternative in self.alternatives[1:]:
             yield "|"
             yield from alternative.render()
@@ -748,14 +793,17 @@
 
 
 class LocalFlags(RegexPattern):
     def __init__(self, contents: AnyRegexPattern, flags: str):
         self.contents = pattern(contents)
         self.flags = flags
 
+    def case_insensitive(self) -> RegexPattern:
+        return LocalFlags(self.contents.case_insensitive(), self.flags)
+
     def render(self) -> StrGen:
         yield "(?"
         yield self.flags
         yield ":"
         yield from self.contents.render()
         yield ")"
 
@@ -791,14 +839,22 @@
         if max_count is not None and max_count < 0:
             raise ValueError("Quantifier upper bound cannot be less than 0")
 
         self.min_count = min_count
         self.max_count = max_count
         self.lazy = lazy
 
+    def case_insensitive(self) -> RegexPattern:
+        new = self.contents.case_insensitive().repeat(self.min_count)
+        if self.max_count is None:
+            new = new.or_more()
+        else:
+            new = new.to(self.max_count)
+        return new
+
     def repeat(self, count: int, lazy: bool = False) -> Range:
         """
 
         The logic here should be carefully thought through.
         If we multiply a fixed-size pattern a{X} by Y, we generally DO NOT get a{X*Y}
         If we multiply a .or_less() pattern a{,X} by Y, we get a{,X*Y}
         If we multiply a pattern a{1,X} (X!=1) by Y, we get a{Y,X*Y}
@@ -904,14 +960,18 @@
     ```
     """
 
     def __init__(self, name: str, contents: Optional[AnyRegexPattern] = None):
         self.name = name
         self.contents = pattern(contents) if contents is not None else None
 
+    def case_insensitive(self) -> RegexPattern:
+        contents = self.contents.case_insensitive() if self.contents else None
+        return NamedPattern(self.name, contents)
+
     def render(self) -> StrGen:
         yield "(?P"
         if self.contents:
             yield "<"
             yield self.name
             yield ">"
             yield from self.contents.render()
@@ -951,14 +1011,21 @@
     def __init__(
         self, group: int, true_option: AnyRegexPattern, false_option: AnyRegexPattern
     ) -> None:
         self.group = group
         self.true_option = respect_priority(true_option, Option.priority + 1)
         self.false_option = respect_priority(false_option, Option.priority + 1)
 
+    def case_insensitive(self) -> RegexPattern:
+        return ConditionalPattern(
+            self.group,
+            self.true_option.case_insensitive(),
+            self.false_option.case_insensitive(),
+        )
+
     def render(self) -> StrGen:
         yield "(?("
         yield str(self.group)
         yield ")"
         yield from self.true_option.render()
         yield "|"
         yield from self.false_option.render()
```

### Comparing `rgx-1.3.3/rgx/meta.py` & `rgx-1.3.4/rgx/meta.py`

 * *Files identical despite different names*

### Comparing `rgx-1.3.3/rgx/unicode_meta.py` & `rgx-1.3.4/rgx/unicode_meta.py`

 * *Files identical despite different names*

### Comparing `rgx-1.3.3/PKG-INFO` & `rgx-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgx
-Version: 1.3.3
+Version: 1.3.4
 Summary: Typed, simple and readable regexp generation
 Home-page: https://github.com/evtn/rgx
 License: MIT
 Keywords: regex,regexp,regular expressions
 Author: Dmitry Gritsenko
 Author-email: rgx@evtn.ru
 Requires-Python: >=3.7,<4.0
```

