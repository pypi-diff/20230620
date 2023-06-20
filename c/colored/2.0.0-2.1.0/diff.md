# Comparing `tmp/colored-2.0.0.tar.gz` & `tmp/colored-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colored-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "colored-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `colored-2.0.0.tar` & `colored-2.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2303 2023-06-19 14:25:45.000000 colored-2.0.0/README.md
--rw-r--r--   0        0        0      305 2023-06-19 14:25:45.000000 colored-2.0.0/colored/__init__.py
--rw-r--r--   0        0        0      553 2023-06-19 14:25:45.000000 colored-2.0.0/colored/attributes.py
--rw-r--r--   0        0        0      599 2023-06-19 14:25:45.000000 colored-2.0.0/colored/background.py
--rw-r--r--   0        0        0     8475 2023-06-19 14:25:45.000000 colored-2.0.0/colored/colored.py
--rw-r--r--   0        0        0      844 2023-06-19 14:25:45.000000 colored-2.0.0/colored/exceptions.py
--rw-r--r--   0        0        0      599 2023-06-19 14:25:45.000000 colored-2.0.0/colored/foreground.py
--rw-r--r--   0        0        0     1789 2023-06-19 14:25:45.000000 colored-2.0.0/colored/hexadecimal.py
--rw-r--r--   0        0        0    12818 2023-06-19 14:25:45.000000 colored-2.0.0/colored/library.py
--rw-r--r--   0        0        0      991 2023-06-19 14:25:45.000000 colored-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3130 1970-01-01 00:00:00.000000 colored-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2349 2023-06-20 09:00:52.000000 colored-2.1.0/README.md
+-rw-r--r--   0        0        0      300 2023-06-20 09:00:52.000000 colored-2.1.0/colored/__init__.py
+-rw-r--r--   0        0        0      558 2023-06-20 09:00:52.000000 colored-2.1.0/colored/attributes.py
+-rw-r--r--   0        0        0      583 2023-06-20 09:00:52.000000 colored-2.1.0/colored/background.py
+-rw-r--r--   0        0        0     8093 2023-06-20 09:00:52.000000 colored-2.1.0/colored/colored.py
+-rw-r--r--   0        0        0      844 2023-06-20 09:00:52.000000 colored-2.1.0/colored/exceptions.py
+-rw-r--r--   0        0        0      583 2023-06-20 09:00:52.000000 colored-2.1.0/colored/foreground.py
+-rw-r--r--   0        0        0     1802 2023-06-20 09:00:52.000000 colored-2.1.0/colored/hexadecimal.py
+-rw-r--r--   0        0        0    14896 2023-06-20 09:00:52.000000 colored-2.1.0/colored/library.py
+-rw-r--r--   0        0        0      991 2023-06-20 09:00:52.000000 colored-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 colored-2.1.0/PKG-INFO
```

### Comparing `colored-2.0.0/README.md` & `colored-2.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 The colors work with most terminals and terminals emulators.
 <a href="https://en.wikipedia.org/wiki/ANSI_escape_code" target="_blank">ANSI/VT100 escape sequences</a> can be used in every programming languages.
 
 Colored is powerful and easy to use:
 
 ```python title="Python 3.9.17"
+>>> from colored import Fore, Back, Style
+>>>
 >>> Fore.red
 '\x1b[38;5;1m'
 >>>
 >>> Back.red
 '\x1b[48;5;1m'
 >>>
 >>> Style.reset
```

#### html2text {}

```diff
@@ -2,17 +2,18 @@
 About Colored, it's a simple Python library for color and formatting in
 terminal. Collection of color codes and names for 256 color terminal setups. A
 list of [256 colors](https://dslackw.gitlab.io/colored/formatting/colors/#full-
 chart-256-foreground-and-background-colors) for Xterm, containing an example of
 the displayed color, Xterm Name, Xterm Number and HEX. The colors work with
 most terminals and terminals emulators. ANSI/VT100_escape_sequences can be used
 in every programming languages. Colored is powerful and easy to use: ```python
-title="Python 3.9.17" >>> Fore.red '\x1b[38;5;1m' >>> >>> Back.red '\x1b
-[48;5;1m' >>> >>> Style.reset '\x1b[0m' >>> >>> print(f'{Fore.white}
-{Back.green}Colored is Awesome!!!{Style.reset}') ```
+title="Python 3.9.17" >>> from colored import Fore, Back, Style >>> >>>
+Fore.red '\x1b[38;5;1m' >>> >>> Back.red '\x1b[48;5;1m' >>> >>> Style.reset
+'\x1b[0m' >>> >>> print(f'{Fore.white}{Back.green}Colored is Awesome!!!
+{Style.reset}') ```
 >>>  Colored is Awesome!!!
 ## Installing Open up a terminal and install colored with pip command: ```bash
 $ pip install colored ``` Alternatively, you can grab the latest source code
 from GitLab: ```bash $ git clone https://gitlab.com/dslackw/colored.git $ cd
 colored $ pip install . ``` ## Usage The [User Guide](https://
 dslackw.gitlab.io/colored/user_guide/user_guide/#user-guide) is the place to go
 to learn how to use the library. The [API Reference](https://dslackw.gitlab.io/
```

### Comparing `colored-2.0.0/colored/attributes.py` & `colored-2.1.0/colored/attributes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from .library import format_codes, styles
+from .library import Library
 from .exceptions import InvalidStyle
 
 
 class MetaStyle(type):
     """ Overrides AttributeError when __getattr__ called. """
     def __getattr__(cls, color):
         raise InvalidStyle(f'{InvalidStyle.__name__}: {color}')
 
 
 class Style(metaclass=MetaStyle):
 
-    ESC: str = format_codes['ESC']
-    END: str = format_codes['END']
+    ESC: str = Library.ESC
+    END: str = Library.END
+    STYLES: dict = Library.STYLES
 
-    for style, code in styles.items():
+    for style, code in STYLES.items():
         vars()[style] = f'{ESC}{code}{END}'
         vars()[style.upper()] = f'{ESC}{code}{END}'
```

### Comparing `colored-2.0.0/colored/background.py` & `colored-2.1.0/colored/foreground.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from .library import format_codes, colors
 from .exceptions import InvalidColor
+from .library import Library
 
 
-class MetaBack(type):
+class MetaFore(type):
     """ Overrides AttributeError when __getattr__ called. """
     def __getattr__(cls, color):
         raise InvalidColor(f'{InvalidColor.__name__}: {color}')
 
 
-class Back(metaclass=MetaBack):
+class Fore(metaclass=MetaFore):
 
-    ESC: str = format_codes['ESC']
-    END: str = format_codes['END']
-    BACK: str = format_codes['BACK']
-
-    for color, code in colors.items():
-        vars()[color] = f'{ESC}{BACK}{code}{END}'
-        vars()[color.upper()] = f'{ESC}{BACK}{code}{END}'
+    END: str = Library.END
+    COLORS: dict = Library.COLORS
+    FOREGROUND: str = Library.FOREGROUND
+
+    for color, code in COLORS.items():
+        vars()[color] = f'{FOREGROUND}{code}{END}'
+        vars()[color.upper()] = f'{FOREGROUND}{code}{END}'
```

### Comparing `colored-2.0.0/colored/colored.py` & `colored-2.1.0/colored/colored.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,93 +2,96 @@
 # -*- coding: utf-8 -*-
 
 import os
 import sys
 import platform
 from typing import Any
 
+from .library import Library
 from .hexadecimal import Hex
-from .library import format_codes, colors, hex_colors, styles, DEFAULT_BACKGROUND
 from .exceptions import InvalidColor, InvalidHexColor, InvalidStyle
 
 
 TTY_AWARE = True
 IS_TTY = sys.stdout.isatty() and sys.stderr.isatty()
 
 _win_vterm_mode = None
 
 
 class Colored:
 
     def __init__(self, color: Any):
         self.color: str = str(color).lower()
-        self.ESC: str = format_codes['ESC']
-        self.END: str = format_codes['END']
-        self.FORE: str = f"{self.ESC}{format_codes['FORE']}"
-        self.BACK: str = f"{self.ESC}{format_codes['BACK']}"
-        self.hexadecimal: str = str()
+        self.hex_color: str = str()
         self.hex = Hex()
+        self.ESC: str = Library.ESC
+        self.END: str = Library.END
+        self.FOREGROUND: str = Library.FOREGROUND
+        self.BACKGROUND: str = Library.BACKGROUND
+        self.COLORS: dict = Library.COLORS
+        self.HEX_COLORS: dict = Library.HEX_COLORS
+        self.STYLES: dict = Library.STYLES
 
         self.enable_windows_terminal_mode()
 
     def attribute(self) -> str:
         """ Return an attribute. """
         self._is_style_exist()
 
         if not self.enabled():
             return str()
 
         if self.color.isdigit():
             return f'{self.ESC}{self.color}{self.END}'
 
-        return f'{self.ESC}{styles[self.color]}{self.END}'
+        return f'{self.ESC}{self.STYLES[self.color]}{self.END}'
 
     def foreground(self) -> str:
         """ Returns a foreground color. """
         self._is_color_exist()
 
         if not self.enabled():
             return str()
 
         if self.color.isdigit():
-            return f'{self.FORE}{self.color}{self.END}'
+            return f'{self.FOREGROUND}{self.color}{self.END}'
         elif self.color.startswith('#'):
-            return f'{self.FORE}{self.hexadecimal}{self.END}'
+            return f'{self.FOREGROUND}{self.hex_color}{self.END}'
 
-        return f'{self.FORE}{colors[self.color]}{self.END}'
+        return f'{self.FOREGROUND}{self.COLORS[self.color]}{self.END}'
 
     def background(self) -> str:
         """ Returns a background color. """
         self._is_color_exist()
 
         if not self.enabled():
             return str()
 
         if self.color.isdigit():
-            return f'{self.BACK}{self.color}{self.END}'
+            return f'{self.BACKGROUND}{self.color}{self.END}'
         elif self.color.startswith('#'):
-            return f'{self.BACK}{self.hexadecimal}{self.END}'
+            return f'{self.BACKGROUND}{self.hex_color}{self.END}'
 
-        return f'{self.BACK}{colors[self.color]}{self.END}'
+        return f'{self.BACKGROUND}{self.COLORS[self.color]}{self.END}'
 
     def _is_color_exist(self) -> None:
         """ Checks for valid color by name or by hex style name or number,
             and raise a InvalidColor or InvalidHexColor exception if it doesn't exist. """
         if self.color.startswith('#'):
-            if self.color not in hex_colors.values():
+            if self.color not in self.HEX_COLORS.values():
                 raise InvalidColor(f'{InvalidHexColor.__name__}: {self.color}')
-            self.hexadecimal: str = self.hex.find(self.color)
+            self.hex_color: str = self.hex.find(self.color)
 
-        elif self.color not in colors.keys() and self.color not in colors.values():
+        elif self.color not in self.COLORS.keys() and self.color not in self.COLORS.values():
             raise InvalidColor(f'{InvalidColor.__name__}: {self.color}')
 
     def _is_style_exist(self) -> None:
         """ Checks for valid style and raise a InvalidStyle exception
             if it doesn't exist. """
-        if self.color not in styles.keys() and self.color not in styles.values():
+        if self.color not in self.STYLES.keys() and self.color not in self.STYLES.values():
             raise InvalidStyle(f'{InvalidStyle.__name__}: {self.color}')
 
     @staticmethod
     def enable_windows_terminal_mode() -> Any:
         """ Contribution by:
             Andreas Fredrik Klasson
             Magnus Heskestad
@@ -172,14 +175,24 @@
 
 
 def back(color: Any) -> str:
     """ Alias for Colored().background() """
     return Colored(color).background()
 
 
+def cprint(text: str, foreground='', background='', formatting='', reset=True, **kwargs) -> None:
+    """ Looks like a patch to a built-in python print() function that allows
+    to pass colored text and style, to this function. """
+    styling: str = Colored(formatting).attribute()
+    back_color: str = Colored(background).background()
+    fore_color: str = Colored(foreground).foreground()
+    terminator: str = Colored('reset').attribute() if reset else ''
+    print(f"{styling}{back_color}{fore_color}{text}{terminator}",  **kwargs)
+
+
 def stylize(text: str, formatting: str, reset=True) -> str:
     """ Conveniently styles your text as and resets ANSI codes at its end. """
     terminator: str = style('reset') if reset else ''
     return f'{"".join(formatting)}{text}{terminator}'
 
 
 def _c0wrap(attr: str) -> str:
@@ -210,39 +223,7 @@
         Jay Deiman
 
     Makes all interactions here tty aware. This means that if either
     stdout or stderr are directed to something other than a tty,
     colorization will not be added. """
     global TTY_AWARE
     TTY_AWARE = awareness
-
-
-def show_colour(foreground: Any, background='', formatting='', message='') -> None:
-    """ Useful function that allows to show the color.
-        Sometimes when we are developing an app we need to see the color
-        behavior before use it. """
-    if isinstance(foreground, str):
-        if foreground.startswith('#'):
-            foreground = int(_find_hex_code(foreground))
-
-    if isinstance(foreground, int):
-        for name, code in colors.items():
-            if code == str(foreground):
-                foreground: Any = name
-                break
-
-    if background:
-        background: str = back(background)
-    else:
-        background: str = DEFAULT_BACKGROUND
-
-    if not message:
-        message: str = f'This is the color: {foreground}'
-
-    print(f"{style(formatting)}{background}{fore(foreground)}{message}{style('reset')}")
-
-
-def _find_hex_code(color) -> int:
-    """ Returns the first matching HEX color. """
-    for code, hex_color in hex_colors.items():
-        if hex_color == color:
-            return code
```

### Comparing `colored-2.0.0/colored/exceptions.py` & `colored-2.1.0/colored/exceptions.py`

 * *Files identical despite different names*

### Comparing `colored-2.0.0/colored/hexadecimal.py` & `colored-2.1.0/colored/hexadecimal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from .library import hex_colors
+from .library import Library
 
 
 class Hex:
 
     def find(self, color: str) -> str:
         """ Contribution by Fredrik Klasson """
 
         # Extend shorthand #ABC -> #AABBCC, like in CSS
 
         if len(color) == 4:
             color: str = '#' + color[1] * 2 + color[2] * 2 + color[3] * 2
 
         # Try an exact lookup, trying to favor lower numbers
         # (e.g. find 10 instead of 46 for #00FF00)
-        for code, hex_color in hex_colors.items():
+        for code, hex_color in Library.HEX_COLORS.items():
             if hex_color == color:
                 return code
 
         # Try to find nearest match using a simple least squares fit.
         # We could try to factor in human perception bias by weighting
         # as suggested by <https://stackoverflow.com/a/1847112> but for
         # now lets just KISS and make upp our minds later, no?
@@ -28,15 +28,15 @@
 
         # The reference color
         r, g, b = (int(color[1:3], 16), int(color[3:5], 16), int(color[5:7], 16))
 
         min_cube_d: int = self.cube(0xFFFFFF)
         nearest: str = '15'
 
-        for code, hex_color in hex_colors.items():
+        for code, hex_color in Library.HEX_COLORS.items():
             cube_d: int = self.fit(hex_color[1:3], r) + self.fit(hex_color[3:5], g) + self.fit(hex_color[5:7], b)
             if cube_d < min_cube_d:
                 min_cube_d: int = cube_d
                 nearest: int = code
 
         return nearest
```

### Comparing `colored-2.0.0/colored/library.py` & `colored-2.1.0/colored/library.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,550 +1,552 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+from dataclasses import dataclass
 
-format_codes: dict = {
-    'ESC': '\x1b[',
-    'FORE': '38;5;',
-    'BACK': '48;5;',
-    'END': 'm'
-}
 
-DEFAULT_FOREGROUND: str = f"{format_codes['ESC']}{format_codes['FORE']}"
-DEFAULT_BACKGROUND: str = f"{format_codes['ESC']}{format_codes['BACK']}"
+@dataclass
+class Library:
 
-styles: dict = {
-    'bold': '1',
-    'dim': '2',
-    'italic': '3',
-    'underlined': '4',
-    'blink': '5',
-    'reverse': '7',
-    'hidden': '8',
-    'strikeout': '9',
-    'reset': '0',
-    'res_bold': '21',
-    'res_dim': '22',
-    'res_underlined': '24',
-    'res_blink': '25',
-    'res_reverse': '27',
-    'res_hidden': '28',
-    '': ''
-}
+    ESC: str = '\x1b['
+    FOREGROUND: str = f'{ESC}38;5;'
+    BACKGROUND: str = f'{ESC}48;5;'
+    END: str = 'm'
 
-colors: dict = {
-    'black': '0',
-    'red': '1',
-    'green': '2',
-    'yellow': '3',
-    'blue': '4',
-    'magenta': '5',
-    'cyan': '6',
-    'light_gray': '7',
-    'dark_gray': '8',
-    'light_red': '9',
-    'light_green': '10',
-    'light_yellow': '11',
-    'light_blue': '12',
-    'light_magenta': '13',
-    'light_cyan': '14',
-    'white': '15',
-    'grey_0': '16',
-    'navy_blue': '17',
-    'dark_blue': '18',
-    'blue_3a': '19',
-    'blue_3b': '20',
-    'blue_1': '21',
-    'dark_green': '22',
-    'deep_sky_blue_4a': '23',
-    'deep_sky_blue_4b': '24',
-    'deep_sky_blue_4c': '25',
-    'dodger_blue_3': '26',
-    'dodger_blue_2': '27',
-    'green_4': '28',
-    'spring_green_4': '29',
-    'turquoise_4': '30',
-    'deep_sky_blue_3a': '31',
-    'deep_sky_blue_3b': '32',
-    'dodger_blue_1': '33',
-    'green_3a': '34',
-    'spring_green_3a': '35',
-    'dark_cyan': '36',
-    'light_sea_green': '37',
-    'deep_sky_blue_2': '38',
-    'deep_sky_blue_1': '39',
-    'green_3b': '40',
-    'spring_green_3b': '41',
-    'spring_green_2a': '42',
-    'cyan_3': '43',
-    'dark_turquoise': '44',
-    'turquoise_2': '45',
-    'green_1': '46',
-    'spring_green_2b': '47',
-    'spring_green_1': '48',
-    'medium_spring_green': '49',
-    'cyan_2': '50',
-    'cyan_1': '51',
-    'dark_red_1': '52',
-    'deep_pink_4a': '53',
-    'purple_4a': '54',
-    'purple_4b': '55',
-    'purple_3': '56',
-    'blue_violet': '57',
-    'orange_4a': '58',
-    'grey_37': '59',
-    'medium_purple_4': '60',
-    'slate_blue_3a': '61',
-    'slate_blue_3b': '62',
-    'royal_blue_1': '63',
-    'chartreuse_4': '64',
-    'dark_sea_green_4a': '65',
-    'pale_turquoise_4': '66',
-    'steel_blue': '67',
-    'steel_blue_3': '68',
-    'cornflower_blue': '69',
-    'chartreuse_3a': '70',
-    'dark_sea_green_4b': '71',
-    'cadet_blue_2': '72',
-    'cadet_blue_1': '73',
-    'sky_blue_3': '74',
-    'steel_blue_1a': '75',
-    'chartreuse_3b': '76',
-    'pale_green_3a': '77',
-    'sea_green_3': '78',
-    'aquamarine_3': '79',
-    'medium_turquoise': '80',
-    'steel_blue_1b': '81',
-    'chartreuse_2a': '82',
-    'sea_green_2': '83',
-    'sea_green_1a': '84',
-    'sea_green_1b': '85',
-    'aquamarine_1a': '86',
-    'dark_slate_gray_2': '87',
-    'dark_red_2': '88',
-    'deep_pink_4b': '89',
-    'dark_magenta_1': '90',
-    'dark_magenta_2': '91',
-    'dark_violet_1a': '92',
-    'purple_1a': '93',
-    'orange_4b': '94',
-    'light_pink_4': '95',
-    'plum_4': '96',
-    'medium_purple_3a': '97',
-    'medium_purple_3b': '98',
-    'slate_blue_1': '99',
-    'yellow_4a': '100',
-    'wheat_4': '101',
-    'grey_53': '102',
-    'light_slate_grey': '103',
-    'medium_purple': '104',
-    'light_slate_blue': '105',
-    'yellow_4b': '106',
-    'dark_olive_green_3a': '107',
-    'dark_green_sea': '108',
-    'light_sky_blue_3a': '109',
-    'light_sky_blue_3b': '110',
-    'sky_blue_2': '111',
-    'chartreuse_2b': '112',
-    'dark_olive_green_3b': '113',
-    'pale_green_3b': '114',
-    'dark_sea_green_3a': '115',
-    'dark_slate_gray_3': '116',
-    'sky_blue_1': '117',
-    'chartreuse_1': '118',
-    'light_green_2': '119',
-    'light_green_3': '120',
-    'pale_green_1a': '121',
-    'aquamarine_1b': '122',
-    'dark_slate_gray_1': '123',
-    'red_3a': '124',
-    'deep_pink_4c': '125',
-    'medium_violet_red': '126',
-    'magenta_3a': '127',
-    'dark_violet_1b': '128',
-    'purple_1b': '129',
-    'dark_orange_3a': '130',
-    'indian_red_1a': '131',
-    'hot_pink_3a': '132',
-    'medium_orchid_3': '133',
-    'medium_orchid': '134',
-    'medium_purple_2a': '135',
-    'dark_goldenrod': '136',
-    'light_salmon_3a': '137',
-    'rosy_brown': '138',
-    'grey_63': '139',
-    'medium_purple_2b': '140',
-    'medium_purple_1': '141',
-    'gold_3a': '142',
-    'dark_khaki': '143',
-    'navajo_white_3': '144',
-    'grey_69': '145',
-    'light_steel_blue_3': '146',
-    'light_steel_blue': '147',
-    'yellow_3a': '148',
-    'dark_olive_green_3': '149',
-    'dark_sea_green_3b': '150',
-    'dark_sea_green_2': '151',
-    'light_cyan_3': '152',
-    'light_sky_blue_1': '153',
-    'green_yellow': '154',
-    'dark_olive_green_2': '155',
-    'pale_green_1b': '156',
-    'dark_sea_green_5b': '157',
-    'dark_sea_green_5a': '158',
-    'pale_turquoise_1': '159',
-    'red_3b': '160',
-    'deep_pink_3a': '161',
-    'deep_pink_3b': '162',
-    'magenta_3b': '163',
-    'magenta_3c': '164',
-    'magenta_2a': '165',
-    'dark_orange_3b': '166',
-    'indian_red_1b': '167',
-    'hot_pink_3b': '168',
-    'hot_pink_2': '169',
-    'orchid': '170',
-    'medium_orchid_1a': '171',
-    'orange_3': '172',
-    'light_salmon_3b': '173',
-    'light_pink_3': '174',
-    'pink_3': '175',
-    'plum_3': '176',
-    'violet': '177',
-    'gold_3b': '178',
-    'light_goldenrod_3': '179',
-    'tan': '180',
-    'misty_rose_3': '181',
-    'thistle_3': '182',
-    'plum_2': '183',
-    'yellow_3b': '184',
-    'khaki_3': '185',
-    'light_goldenrod_2a': '186',
-    'light_yellow_3': '187',
-    'grey_84': '188',
-    'light_steel_blue_1': '189',
-    'yellow_2': '190',
-    'dark_olive_green_1a': '191',
-    'dark_olive_green_1b': '192',
-    'dark_sea_green_1': '193',
-    'honeydew_2': '194',
-    'light_cyan_1': '195',
-    'red_1': '196',
-    'deep_pink_2': '197',
-    'deep_pink_1a': '198',
-    'deep_pink_1b': '199',
-    'magenta_2b': '200',
-    'magenta_1': '201',
-    'orange_red_1': '202',
-    'indian_red_1c': '203',
-    'indian_red_1d': '204',
-    'hot_pink_1a': '205',
-    'hot_pink_1b': '206',
-    'medium_orchid_1b': '207',
-    'dark_orange': '208',
-    'salmon_1': '209',
-    'light_coral': '210',
-    'pale_violet_red_1': '211',
-    'orchid_2': '212',
-    'orchid_1': '213',
-    'orange_1': '214',
-    'sandy_brown': '215',
-    'light_salmon_1': '216',
-    'light_pink_1': '217',
-    'pink_1': '218',
-    'plum_1': '219',
-    'gold_1': '220',
-    'light_goldenrod_2b': '221',
-    'light_goldenrod_2c': '222',
-    'navajo_white_1': '223',
-    'misty_rose1': '224',
-    'thistle_1': '225',
-    'yellow_1': '226',
-    'light_goldenrod_1': '227',
-    'khaki_1': '228',
-    'wheat_1': '229',
-    'cornsilk_1': '230',
-    'grey_100': '231',
-    'grey_3': '232',
-    'grey_7': '233',
-    'grey_11': '234',
-    'grey_15': '235',
-    'grey_19': '236',
-    'grey_23': '237',
-    'grey_27': '238',
-    'grey_30': '239',
-    'grey_35': '240',
-    'grey_39': '241',
-    'grey_42': '242',
-    'grey_46': '243',
-    'grey_50': '244',
-    'grey_54': '245',
-    'grey_58': '246',
-    'grey_62': '247',
-    'grey_66': '248',
-    'grey_70': '249',
-    'grey_74': '250',
-    'grey_78': '251',
-    'grey_82': '252',
-    'grey_85': '253',
-    'grey_89': '254',
-    'grey_93': '255',
-}
+    STYLES = {
+        '': '',
+        'bold': '1',
+        'dim': '2',
+        'italic': '3',
+        'underlined': '4',
+        'blink': '5',
+        'reverse': '7',
+        'hidden': '8',
+        'strikeout': '9',
+        'reset': '0',
+        'res_bold': '21',
+        'res_dim': '22',
+        'res_underlined': '24',
+        'res_blink': '25',
+        'res_reverse': '27',
+        'res_hidden': '28',
+    }
 
-hex_colors: dict = {
-    '0': '#000000',
-    '1': '#800000',
-    '2': '#008000',
-    '3': '#808000',
-    '4': '#000080',
-    '5': '#800080',
-    '6': '#008080',
-    '7': '#c0c0c0',
-    '8': '#808080',
-    '9': '#ff0000',
-    '10': '#00ff00',
-    '11': '#ffff00',
-    '12': '#0000ff',
-    '13': '#ff00ff',
-    '14': '#00ffff',
-    '15': '#ffffff',
-    '16': '#000000',
-    '17': '#00005f',
-    '18': '#000087',
-    '19': '#0000af',
-    '20': '#0000d7',
-    '21': '#0000ff',
-    '22': '#005f00',
-    '23': '#005f5f',
-    '24': '#005f87',
-    '25': '#005faf',
-    '26': '#005fd7',
-    '27': '#005fff',
-    '28': '#008700',
-    '29': '#00875f',
-    '30': '#008787',
-    '31': '#0087af',
-    '32': '#0087d7',
-    '33': '#0087ff',
-    '34': '#00af00',
-    '35': '#00af5f',
-    '36': '#00af87',
-    '37': '#00afaf',
-    '38': '#00afd7',
-    '39': '#00afff',
-    '40': '#00d700',
-    '41': '#00d75f',
-    '42': '#00d787',
-    '43': '#00d7af',
-    '44': '#00d7d7',
-    '45': '#00d7ff',
-    '46': '#00ff00',
-    '47': '#00ff5f',
-    '48': '#00ff87',
-    '49': '#00ffaf',
-    '50': '#00ffd7',
-    '51': '#00ffff',
-    '52': '#5f0000',
-    '53': '#5f005f',
-    '54': '#5f0087',
-    '55': '#5f00af',
-    '56': '#5f00d7',
-    '57': '#5f00ff',
-    '58': '#5f5f00',
-    '59': '#5f5f5f',
-    '60': '#5f5f87',
-    '61': '#5f5faf',
-    '62': '#5f5fd7',
-    '63': '#5f5fff',
-    '64': '#5f8700',
-    '65': '#5f875f',
-    '66': '#5f8787',
-    '67': '#5f87af',
-    '68': '#5f87d7',
-    '69': '#5f87ff',
-    '70': '#5faf00',
-    '71': '#5faf5f',
-    '72': '#5faf87',
-    '73': '#5fafaf',
-    '74': '#5fafd7',
-    '75': '#5fafff',
-    '76': '#5fd700',
-    '77': '#5fd75f',
-    '78': '#5fd787',
-    '79': '#5fd7af',
-    '80': '#5fd7d7',
-    '81': '#5fd7ff',
-    '82': '#5fff00',
-    '83': '#5fff5f',
-    '84': '#5fff87',
-    '85': '#5fffaf',
-    '86': '#5fffd7',
-    '87': '#5fffff',
-    '88': '#870000',
-    '89': '#87005f',
-    '90': '#870087',
-    '91': '#8700af',
-    '92': '#8700d7',
-    '93': '#8700ff',
-    '94': '#875f00',
-    '95': '#875f5f',
-    '96': '#875f87',
-    '97': '#875faf',
-    '98': '#875fd7',
-    '99': '#875fff',
-    '100': '#878700',
-    '101': '#87875f',
-    '102': '#878787',
-    '103': '#8787af',
-    '104': '#8787d7',
-    '105': '#8787ff',
-    '106': '#87af00',
-    '107': '#87af5f',
-    '108': '#87af87',
-    '109': '#87afaf',
-    '110': '#87afd7',
-    '111': '#87afff',
-    '112': '#87d700',
-    '113': '#87d75f',
-    '114': '#87d787',
-    '115': '#87d7af',
-    '116': '#87d7d7',
-    '117': '#87d7ff',
-    '118': '#87ff00',
-    '119': '#87ff5f',
-    '120': '#87ff87',
-    '121': '#87ffaf',
-    '122': '#87ffd7',
-    '123': '#87ffff',
-    '124': '#af0000',
-    '125': '#af005f',
-    '126': '#af0087',
-    '127': '#af00af',
-    '128': '#af00d7',
-    '129': '#af00ff',
-    '130': '#af5f00',
-    '131': '#af5f5f',
-    '132': '#af5f87',
-    '133': '#af5faf',
-    '134': '#af5fd7',
-    '135': '#af5fff',
-    '136': '#af8700',
-    '137': '#af875f',
-    '138': '#af8787',
-    '139': '#af87af',
-    '140': '#af87d7',
-    '141': '#af87ff',
-    '142': '#afaf00',
-    '143': '#afaf5f',
-    '144': '#afaf87',
-    '145': '#afafaf',
-    '146': '#afafd7',
-    '147': '#afafff',
-    '148': '#afd700',
-    '149': '#afd75f',
-    '150': '#afd787',
-    '151': '#afd7af',
-    '152': '#afd7d7',
-    '153': '#afd7ff',
-    '154': '#afff00',
-    '155': '#afff5f',
-    '156': '#afff87',
-    '157': '#afffaf',
-    '158': '#afffd7',
-    '159': '#afffff',
-    '160': '#d70000',
-    '161': '#d7005f',
-    '162': '#d70087',
-    '163': '#d700af',
-    '164': '#d700d7',
-    '165': '#d700ff',
-    '166': '#d75f00',
-    '167': '#d75f5f',
-    '168': '#d75f87',
-    '169': '#d75faf',
-    '170': '#d75fd7',
-    '171': '#d75fff',
-    '172': '#d78700',
-    '173': '#d7875f',
-    '174': '#d78787',
-    '175': '#d787af',
-    '176': '#d787d7',
-    '177': '#d787ff',
-    '178': '#d7af00',
-    '179': '#d7af5f',
-    '180': '#d7af87',
-    '181': '#d7afaf',
-    '182': '#d7afd7',
-    '183': '#d7afff',
-    '184': '#d7d700',
-    '185': '#d7d75f',
-    '186': '#d7d787',
-    '187': '#d7d7af',
-    '188': '#d7d7d7',
-    '189': '#d7d7ff',
-    '190': '#d7ff00',
-    '191': '#d7ff5f',
-    '192': '#d7ff87',
-    '193': '#d7ffaf',
-    '194': '#d7ffd7',
-    '195': '#d7ffff',
-    '196': '#ff0000',
-    '197': '#ff005f',
-    '198': '#ff0087',
-    '199': '#ff00af',
-    '200': '#ff00d7',
-    '201': '#ff00ff',
-    '202': '#ff5f00',
-    '203': '#ff5f5f',
-    '204': '#ff5f87',
-    '205': '#ff5faf',
-    '206': '#ff5fd7',
-    '207': '#ff5fff',
-    '208': '#ff8700',
-    '209': '#ff875f',
-    '210': '#ff8787',
-    '211': '#ff87af',
-    '212': '#ff87d7',
-    '213': '#ff87ff',
-    '214': '#ffaf00',
-    '215': '#ffaf5f',
-    '216': '#ffaf87',
-    '217': '#ffafaf',
-    '218': '#ffafd7',
-    '219': '#ffafff',
-    '220': '#ffd700',
-    '221': '#ffd75f',
-    '222': '#ffd787',
-    '223': '#ffd7af',
-    '224': '#ffd7d7',
-    '225': '#ffd7ff',
-    '226': '#ffff00',
-    '227': '#ffff5f',
-    '228': '#ffff87',
-    '229': '#ffffaf',
-    '230': '#ffffd7',
-    '231': '#ffffff',
-    '232': '#080808',
-    '233': '#121212',
-    '234': '#1c1c1c',
-    '235': '#262626',
-    '236': '#303030',
-    '237': '#3a3a3a',
-    '238': '#444444',
-    '239': '#4e4e4e',
-    '240': '#585858',
-    '241': '#626262',
-    '242': '#6c6c6c',
-    '243': '#767676',
-    '244': '#808080',
-    '245': '#8a8a8a',
-    '246': '#949494',
-    '247': '#9e9e9e',
-    '248': '#a8a8a8',
-    '249': '#b2b2b2',
-    '250': '#bcbcbc',
-    '251': '#c6c6c6',
-    '252': '#d0d0d0',
-    '253': '#dadada',
-    '254': '#e4e4e4',
-    '255': '#eeeeee'
-}
+    COLORS = {
+        '': '',
+        'black': '0',
+        'red': '1',
+        'green': '2',
+        'yellow': '3',
+        'blue': '4',
+        'magenta': '5',
+        'cyan': '6',
+        'light_gray': '7',
+        'dark_gray': '8',
+        'light_red': '9',
+        'light_green': '10',
+        'light_yellow': '11',
+        'light_blue': '12',
+        'light_magenta': '13',
+        'light_cyan': '14',
+        'white': '15',
+        'grey_0': '16',
+        'navy_blue': '17',
+        'dark_blue': '18',
+        'blue_3a': '19',
+        'blue_3b': '20',
+        'blue_1': '21',
+        'dark_green': '22',
+        'deep_sky_blue_4a': '23',
+        'deep_sky_blue_4b': '24',
+        'deep_sky_blue_4c': '25',
+        'dodger_blue_3': '26',
+        'dodger_blue_2': '27',
+        'green_4': '28',
+        'spring_green_4': '29',
+        'turquoise_4': '30',
+        'deep_sky_blue_3a': '31',
+        'deep_sky_blue_3b': '32',
+        'dodger_blue_1': '33',
+        'green_3a': '34',
+        'spring_green_3a': '35',
+        'dark_cyan': '36',
+        'light_sea_green': '37',
+        'deep_sky_blue_2': '38',
+        'deep_sky_blue_1': '39',
+        'green_3b': '40',
+        'spring_green_3b': '41',
+        'spring_green_2a': '42',
+        'cyan_3': '43',
+        'dark_turquoise': '44',
+        'turquoise_2': '45',
+        'green_1': '46',
+        'spring_green_2b': '47',
+        'spring_green_1': '48',
+        'medium_spring_green': '49',
+        'cyan_2': '50',
+        'cyan_1': '51',
+        'dark_red_1': '52',
+        'deep_pink_4a': '53',
+        'purple_4a': '54',
+        'purple_4b': '55',
+        'purple_3': '56',
+        'blue_violet': '57',
+        'orange_4a': '58',
+        'grey_37': '59',
+        'medium_purple_4': '60',
+        'slate_blue_3a': '61',
+        'slate_blue_3b': '62',
+        'royal_blue_1': '63',
+        'chartreuse_4': '64',
+        'dark_sea_green_4a': '65',
+        'pale_turquoise_4': '66',
+        'steel_blue': '67',
+        'steel_blue_3': '68',
+        'cornflower_blue': '69',
+        'chartreuse_3a': '70',
+        'dark_sea_green_4b': '71',
+        'cadet_blue_2': '72',
+        'cadet_blue_1': '73',
+        'sky_blue_3': '74',
+        'steel_blue_1a': '75',
+        'chartreuse_3b': '76',
+        'pale_green_3a': '77',
+        'sea_green_3': '78',
+        'aquamarine_3': '79',
+        'medium_turquoise': '80',
+        'steel_blue_1b': '81',
+        'chartreuse_2a': '82',
+        'sea_green_2': '83',
+        'sea_green_1a': '84',
+        'sea_green_1b': '85',
+        'aquamarine_1a': '86',
+        'dark_slate_gray_2': '87',
+        'dark_red_2': '88',
+        'deep_pink_4b': '89',
+        'dark_magenta_1': '90',
+        'dark_magenta_2': '91',
+        'dark_violet_1a': '92',
+        'purple_1a': '93',
+        'orange_4b': '94',
+        'light_pink_4': '95',
+        'plum_4': '96',
+        'medium_purple_3a': '97',
+        'medium_purple_3b': '98',
+        'slate_blue_1': '99',
+        'yellow_4a': '100',
+        'wheat_4': '101',
+        'grey_53': '102',
+        'light_slate_grey': '103',
+        'medium_purple': '104',
+        'light_slate_blue': '105',
+        'yellow_4b': '106',
+        'dark_olive_green_3a': '107',
+        'dark_green_sea': '108',
+        'light_sky_blue_3a': '109',
+        'light_sky_blue_3b': '110',
+        'sky_blue_2': '111',
+        'chartreuse_2b': '112',
+        'dark_olive_green_3b': '113',
+        'pale_green_3b': '114',
+        'dark_sea_green_3a': '115',
+        'dark_slate_gray_3': '116',
+        'sky_blue_1': '117',
+        'chartreuse_1': '118',
+        'light_green_2': '119',
+        'light_green_3': '120',
+        'pale_green_1a': '121',
+        'aquamarine_1b': '122',
+        'dark_slate_gray_1': '123',
+        'red_3a': '124',
+        'deep_pink_4c': '125',
+        'medium_violet_red': '126',
+        'magenta_3a': '127',
+        'dark_violet_1b': '128',
+        'purple_1b': '129',
+        'dark_orange_3a': '130',
+        'indian_red_1a': '131',
+        'hot_pink_3a': '132',
+        'medium_orchid_3': '133',
+        'medium_orchid': '134',
+        'medium_purple_2a': '135',
+        'dark_goldenrod': '136',
+        'light_salmon_3a': '137',
+        'rosy_brown': '138',
+        'grey_63': '139',
+        'medium_purple_2b': '140',
+        'medium_purple_1': '141',
+        'gold_3a': '142',
+        'dark_khaki': '143',
+        'navajo_white_3': '144',
+        'grey_69': '145',
+        'light_steel_blue_3': '146',
+        'light_steel_blue': '147',
+        'yellow_3a': '148',
+        'dark_olive_green_3': '149',
+        'dark_sea_green_3b': '150',
+        'dark_sea_green_2': '151',
+        'light_cyan_3': '152',
+        'light_sky_blue_1': '153',
+        'green_yellow': '154',
+        'dark_olive_green_2': '155',
+        'pale_green_1b': '156',
+        'dark_sea_green_5b': '157',
+        'dark_sea_green_5a': '158',
+        'pale_turquoise_1': '159',
+        'red_3b': '160',
+        'deep_pink_3a': '161',
+        'deep_pink_3b': '162',
+        'magenta_3b': '163',
+        'magenta_3c': '164',
+        'magenta_2a': '165',
+        'dark_orange_3b': '166',
+        'indian_red_1b': '167',
+        'hot_pink_3b': '168',
+        'hot_pink_2': '169',
+        'orchid': '170',
+        'medium_orchid_1a': '171',
+        'orange_3': '172',
+        'light_salmon_3b': '173',
+        'light_pink_3': '174',
+        'pink_3': '175',
+        'plum_3': '176',
+        'violet': '177',
+        'gold_3b': '178',
+        'light_goldenrod_3': '179',
+        'tan': '180',
+        'misty_rose_3': '181',
+        'thistle_3': '182',
+        'plum_2': '183',
+        'yellow_3b': '184',
+        'khaki_3': '185',
+        'light_goldenrod_2a': '186',
+        'light_yellow_3': '187',
+        'grey_84': '188',
+        'light_steel_blue_1': '189',
+        'yellow_2': '190',
+        'dark_olive_green_1a': '191',
+        'dark_olive_green_1b': '192',
+        'dark_sea_green_1': '193',
+        'honeydew_2': '194',
+        'light_cyan_1': '195',
+        'red_1': '196',
+        'deep_pink_2': '197',
+        'deep_pink_1a': '198',
+        'deep_pink_1b': '199',
+        'magenta_2b': '200',
+        'magenta_1': '201',
+        'orange_red_1': '202',
+        'indian_red_1c': '203',
+        'indian_red_1d': '204',
+        'hot_pink_1a': '205',
+        'hot_pink_1b': '206',
+        'medium_orchid_1b': '207',
+        'dark_orange': '208',
+        'salmon_1': '209',
+        'light_coral': '210',
+        'pale_violet_red_1': '211',
+        'orchid_2': '212',
+        'orchid_1': '213',
+        'orange_1': '214',
+        'sandy_brown': '215',
+        'light_salmon_1': '216',
+        'light_pink_1': '217',
+        'pink_1': '218',
+        'plum_1': '219',
+        'gold_1': '220',
+        'light_goldenrod_2b': '221',
+        'light_goldenrod_2c': '222',
+        'navajo_white_1': '223',
+        'misty_rose1': '224',
+        'thistle_1': '225',
+        'yellow_1': '226',
+        'light_goldenrod_1': '227',
+        'khaki_1': '228',
+        'wheat_1': '229',
+        'cornsilk_1': '230',
+        'grey_100': '231',
+        'grey_3': '232',
+        'grey_7': '233',
+        'grey_11': '234',
+        'grey_15': '235',
+        'grey_19': '236',
+        'grey_23': '237',
+        'grey_27': '238',
+        'grey_30': '239',
+        'grey_35': '240',
+        'grey_39': '241',
+        'grey_42': '242',
+        'grey_46': '243',
+        'grey_50': '244',
+        'grey_54': '245',
+        'grey_58': '246',
+        'grey_62': '247',
+        'grey_66': '248',
+        'grey_70': '249',
+        'grey_74': '250',
+        'grey_78': '251',
+        'grey_82': '252',
+        'grey_85': '253',
+        'grey_89': '254',
+        'grey_93': '255',
+    }
+
+    HEX_COLORS = {
+        '': '',
+        '0': '#000000',
+        '1': '#800000',
+        '2': '#008000',
+        '3': '#808000',
+        '4': '#000080',
+        '5': '#800080',
+        '6': '#008080',
+        '7': '#c0c0c0',
+        '8': '#808080',
+        '9': '#ff0000',
+        '10': '#00ff00',
+        '11': '#ffff00',
+        '12': '#0000ff',
+        '13': '#ff00ff',
+        '14': '#00ffff',
+        '15': '#ffffff',
+        '16': '#000000',
+        '17': '#00005f',
+        '18': '#000087',
+        '19': '#0000af',
+        '20': '#0000d7',
+        '21': '#0000ff',
+        '22': '#005f00',
+        '23': '#005f5f',
+        '24': '#005f87',
+        '25': '#005faf',
+        '26': '#005fd7',
+        '27': '#005fff',
+        '28': '#008700',
+        '29': '#00875f',
+        '30': '#008787',
+        '31': '#0087af',
+        '32': '#0087d7',
+        '33': '#0087ff',
+        '34': '#00af00',
+        '35': '#00af5f',
+        '36': '#00af87',
+        '37': '#00afaf',
+        '38': '#00afd7',
+        '39': '#00afff',
+        '40': '#00d700',
+        '41': '#00d75f',
+        '42': '#00d787',
+        '43': '#00d7af',
+        '44': '#00d7d7',
+        '45': '#00d7ff',
+        '46': '#00ff00',
+        '47': '#00ff5f',
+        '48': '#00ff87',
+        '49': '#00ffaf',
+        '50': '#00ffd7',
+        '51': '#00ffff',
+        '52': '#5f0000',
+        '53': '#5f005f',
+        '54': '#5f0087',
+        '55': '#5f00af',
+        '56': '#5f00d7',
+        '57': '#5f00ff',
+        '58': '#5f5f00',
+        '59': '#5f5f5f',
+        '60': '#5f5f87',
+        '61': '#5f5faf',
+        '62': '#5f5fd7',
+        '63': '#5f5fff',
+        '64': '#5f8700',
+        '65': '#5f875f',
+        '66': '#5f8787',
+        '67': '#5f87af',
+        '68': '#5f87d7',
+        '69': '#5f87ff',
+        '70': '#5faf00',
+        '71': '#5faf5f',
+        '72': '#5faf87',
+        '73': '#5fafaf',
+        '74': '#5fafd7',
+        '75': '#5fafff',
+        '76': '#5fd700',
+        '77': '#5fd75f',
+        '78': '#5fd787',
+        '79': '#5fd7af',
+        '80': '#5fd7d7',
+        '81': '#5fd7ff',
+        '82': '#5fff00',
+        '83': '#5fff5f',
+        '84': '#5fff87',
+        '85': '#5fffaf',
+        '86': '#5fffd7',
+        '87': '#5fffff',
+        '88': '#870000',
+        '89': '#87005f',
+        '90': '#870087',
+        '91': '#8700af',
+        '92': '#8700d7',
+        '93': '#8700ff',
+        '94': '#875f00',
+        '95': '#875f5f',
+        '96': '#875f87',
+        '97': '#875faf',
+        '98': '#875fd7',
+        '99': '#875fff',
+        '100': '#878700',
+        '101': '#87875f',
+        '102': '#878787',
+        '103': '#8787af',
+        '104': '#8787d7',
+        '105': '#8787ff',
+        '106': '#87af00',
+        '107': '#87af5f',
+        '108': '#87af87',
+        '109': '#87afaf',
+        '110': '#87afd7',
+        '111': '#87afff',
+        '112': '#87d700',
+        '113': '#87d75f',
+        '114': '#87d787',
+        '115': '#87d7af',
+        '116': '#87d7d7',
+        '117': '#87d7ff',
+        '118': '#87ff00',
+        '119': '#87ff5f',
+        '120': '#87ff87',
+        '121': '#87ffaf',
+        '122': '#87ffd7',
+        '123': '#87ffff',
+        '124': '#af0000',
+        '125': '#af005f',
+        '126': '#af0087',
+        '127': '#af00af',
+        '128': '#af00d7',
+        '129': '#af00ff',
+        '130': '#af5f00',
+        '131': '#af5f5f',
+        '132': '#af5f87',
+        '133': '#af5faf',
+        '134': '#af5fd7',
+        '135': '#af5fff',
+        '136': '#af8700',
+        '137': '#af875f',
+        '138': '#af8787',
+        '139': '#af87af',
+        '140': '#af87d7',
+        '141': '#af87ff',
+        '142': '#afaf00',
+        '143': '#afaf5f',
+        '144': '#afaf87',
+        '145': '#afafaf',
+        '146': '#afafd7',
+        '147': '#afafff',
+        '148': '#afd700',
+        '149': '#afd75f',
+        '150': '#afd787',
+        '151': '#afd7af',
+        '152': '#afd7d7',
+        '153': '#afd7ff',
+        '154': '#afff00',
+        '155': '#afff5f',
+        '156': '#afff87',
+        '157': '#afffaf',
+        '158': '#afffd7',
+        '159': '#afffff',
+        '160': '#d70000',
+        '161': '#d7005f',
+        '162': '#d70087',
+        '163': '#d700af',
+        '164': '#d700d7',
+        '165': '#d700ff',
+        '166': '#d75f00',
+        '167': '#d75f5f',
+        '168': '#d75f87',
+        '169': '#d75faf',
+        '170': '#d75fd7',
+        '171': '#d75fff',
+        '172': '#d78700',
+        '173': '#d7875f',
+        '174': '#d78787',
+        '175': '#d787af',
+        '176': '#d787d7',
+        '177': '#d787ff',
+        '178': '#d7af00',
+        '179': '#d7af5f',
+        '180': '#d7af87',
+        '181': '#d7afaf',
+        '182': '#d7afd7',
+        '183': '#d7afff',
+        '184': '#d7d700',
+        '185': '#d7d75f',
+        '186': '#d7d787',
+        '187': '#d7d7af',
+        '188': '#d7d7d7',
+        '189': '#d7d7ff',
+        '190': '#d7ff00',
+        '191': '#d7ff5f',
+        '192': '#d7ff87',
+        '193': '#d7ffaf',
+        '194': '#d7ffd7',
+        '195': '#d7ffff',
+        '196': '#ff0000',
+        '197': '#ff005f',
+        '198': '#ff0087',
+        '199': '#ff00af',
+        '200': '#ff00d7',
+        '201': '#ff00ff',
+        '202': '#ff5f00',
+        '203': '#ff5f5f',
+        '204': '#ff5f87',
+        '205': '#ff5faf',
+        '206': '#ff5fd7',
+        '207': '#ff5fff',
+        '208': '#ff8700',
+        '209': '#ff875f',
+        '210': '#ff8787',
+        '211': '#ff87af',
+        '212': '#ff87d7',
+        '213': '#ff87ff',
+        '214': '#ffaf00',
+        '215': '#ffaf5f',
+        '216': '#ffaf87',
+        '217': '#ffafaf',
+        '218': '#ffafd7',
+        '219': '#ffafff',
+        '220': '#ffd700',
+        '221': '#ffd75f',
+        '222': '#ffd787',
+        '223': '#ffd7af',
+        '224': '#ffd7d7',
+        '225': '#ffd7ff',
+        '226': '#ffff00',
+        '227': '#ffff5f',
+        '228': '#ffff87',
+        '229': '#ffffaf',
+        '230': '#ffffd7',
+        '231': '#ffffff',
+        '232': '#080808',
+        '233': '#121212',
+        '234': '#1c1c1c',
+        '235': '#262626',
+        '236': '#303030',
+        '237': '#3a3a3a',
+        '238': '#444444',
+        '239': '#4e4e4e',
+        '240': '#585858',
+        '241': '#626262',
+        '242': '#6c6c6c',
+        '243': '#767676',
+        '244': '#808080',
+        '245': '#8a8a8a',
+        '246': '#949494',
+        '247': '#9e9e9e',
+        '248': '#a8a8a8',
+        '249': '#b2b2b2',
+        '250': '#bcbcbc',
+        '251': '#c6c6c6',
+        '252': '#d0d0d0',
+        '253': '#dadada',
+        '254': '#e4e4e4',
+        '255': '#eeeeee'
+    }
```

### Comparing `colored-2.0.0/pyproject.toml` & `colored-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "colored"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Simple python library for color and formatting to terminal"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ['xterm', 'color', 'vt100', 'ansi', 'terminal', 'python']
```

### Comparing `colored-2.0.0/PKG-INFO` & `colored-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colored
-Version: 2.0.0
+Version: 2.1.0
 Summary: Simple python library for color and formatting to terminal
 Keywords: xterm,color,vt100,ansi,terminal,python
 Author-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -31,14 +31,16 @@
 
 The colors work with most terminals and terminals emulators.
 <a href="https://en.wikipedia.org/wiki/ANSI_escape_code" target="_blank">ANSI/VT100 escape sequences</a> can be used in every programming languages.
 
 Colored is powerful and easy to use:
 
 ```python title="Python 3.9.17"
+>>> from colored import Fore, Back, Style
+>>>
 >>> Fore.red
 '\x1b[38;5;1m'
 >>>
 >>> Back.red
 '\x1b[48;5;1m'
 >>>
 >>> Style.reset
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colored Version: 2.0.0 Summary: Simple python
+Metadata-Version: 2.1 Name: colored Version: 2.1.0 Summary: Simple python
 library for color and formatting to terminal Keywords:
 xterm,color,vt100,ansi,terminal,python Author-email: Dimitris Zlatanidis
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Other Classifier: Operating System :: POSIX ::
 Linux Classifier: Operating System :: Microsoft :: Windows Classifier:
@@ -13,17 +13,18 @@
 images/colored.png] ## About Colored, it's a simple Python library for color
 and formatting in terminal. Collection of color codes and names for 256 color
 terminal setups. A list of [256 colors](https://dslackw.gitlab.io/colored/
 formatting/colors/#full-chart-256-foreground-and-background-colors) for Xterm,
 containing an example of the displayed color, Xterm Name, Xterm Number and HEX.
 The colors work with most terminals and terminals emulators. ANSI/VT100_escape
 sequences can be used in every programming languages. Colored is powerful and
-easy to use: ```python title="Python 3.9.17" >>> Fore.red '\x1b[38;5;1m' >>>
->>> Back.red '\x1b[48;5;1m' >>> >>> Style.reset '\x1b[0m' >>> >>> print(f'
-{Fore.white}{Back.green}Colored is Awesome!!!{Style.reset}') ```
+easy to use: ```python title="Python 3.9.17" >>> from colored import Fore,
+Back, Style >>> >>> Fore.red '\x1b[38;5;1m' >>> >>> Back.red '\x1b[48;5;1m' >>>
+>>> Style.reset '\x1b[0m' >>> >>> print(f'{Fore.white}{Back.green}Colored is
+Awesome!!!{Style.reset}') ```
 >>>  Colored is Awesome!!!
 ## Installing Open up a terminal and install colored with pip command: ```bash
 $ pip install colored ``` Alternatively, you can grab the latest source code
 from GitLab: ```bash $ git clone https://gitlab.com/dslackw/colored.git $ cd
 colored $ pip install . ``` ## Usage The [User Guide](https://
 dslackw.gitlab.io/colored/user_guide/user_guide/#user-guide) is the place to go
 to learn how to use the library. The [API Reference](https://dslackw.gitlab.io/
```

